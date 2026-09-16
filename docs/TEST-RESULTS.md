# 阶段 4 · 压力测试记录

## 测试方法

用**盲测路由**检验 8 个 skill 的 description 是否足够精准：

1. 从 8 个 `test-prompts.json` 抽出全部 48 条测试用例（24 条正向 / 16 条诱饵 / 8 条边界），
   随机打乱后生成 `work/route/router_input.md`（只含 8 条 description + 48 条提问，不含标准答案）。
2. 由一个**未接触过本项目**的 agent 充当路由器，只读该文件，为每条提问选一个 skill 或填 NONE。
3. 与标准答案比对（`work/score_route*.py`）。

评分规则：
- `should_trigger` → 必须选中本 skill；
- `should_not_trigger` → **只要没选中本 skill 就算通过**（诱饵容错为 0，其中 8 条是同书兄弟 skill 的混淆诱饵）；
- `edge_case` → 选中本 skill 或 NONE 都算通过（因为边界场景允许"判断为不适用"）。

---

## 第一轮（描述 v0.1.0）

| 指标 | 结果 |
|---|---|
| 总通过 | **43 / 48 = 89.6%** |
| 正向（24） | 20 / 24 |
| 诱饵（16） | **16 / 16 —— 零误触发** |
| 边界（8） | 7 / 8 |

### 失分点（全部是"兄弟 skill 抢调用"）

| 用例 | 提问 | 应调用 | 实际被路由到 | 性质 |
|---|---|---|---|---|
| timing-03 | 它三艘航母摆在那儿又不打，是虚张声势吗？ | timing-window-cadence | adversary-intent-read | 真歧义：既是成本题也是意图题 |
| adv-03 | 它最厉害的那个手段为什么一直不用？ | adversary-intent-read | timing-window-cadence | **真失分**：description 未覆盖"手段缺席" |
| adv-02 | 今天说妥协、昨天说打服，哪个是真的？ | adversary-intent-read | causal-chain-consistency | **真失分**：未覆盖"前后矛盾的两套说辞" |
| end-02 | 美国打不赢一个地区国家算不算输？ | endgame-scripting | strategy-tactics-audit | 真歧义：本质是胜负判定题 |
| edge-01 | 现在是"大乱斗"还是"大变局"？ | endgame-scripting | strategy-tactics-audit | 边界：阶段命名题 |

**结论**：诱饵零误触发，说明 8 个 skill 边界总体清晰；问题集中在 3 组相邻技能（意图 vs 时间 / 意图 vs 一致性 / 终局 vs 分层）。

---

## 第二轮（描述 v0.1.1，仅补 description）

按 darwin 流程做了定向修补（**只改 description，不改方法论内容**）：

| skill | 补充的触发情形 |
|---|---|
| `adversary-intent-read` | + "它最有效的那个手段为什么一直不用" + "今天说妥协昨天说打服，哪个是真的" + "摆着兵力不动是虚张声势还是真要动手"；并写明"问最后怎么收场请转 endgame-scripting" |
| `timing-window-cadence` | + "摆着高成本兵力又不打，是虚张声势吗（用维持成本反推意志）"；并写明"问真实目的请转 adversary-intent-read" |
| `endgame-scripting` | + "霸权打不赢一个地区国家算不算输"；并写明"只问战术成功与否请转 strategy-tactics-audit" |

| 指标 | 结果 |
|---|---|
| 总通过 | **48 / 48 = 100%** |
| 正向（24） | 24 / 24 |
| 诱饵（16） | 16 / 16 |
| 边界（8） | 8 / 8 |

### ⚠️ 结果解读（必须打折看）

第二轮是**定向修补后立刻复测同一套题**，属于"教到考卷上"，100% 不能理解为泛化能力已达 100%。
它的真实含义是：**这 5 个失分点已经通过 description 显式分流解决**。
真正的泛化检验需要用**未参与改写的新提问**复测——建议在接入 darwin 后按 `minimum_pass_rate: 0.8` 持续跑题库扩充版。

---

## 已知未做的测试

| 项 | 状态 |
|---|---|
| 端到端行为测试（真正让 skill 跑起来看输出质量） | 未做 —— 本轮只测"该不该调用" |
| 同源存量 skill 的互斥测试（与 7 个旧 skill 的抢调用） | 未做 —— 建议安装后合并成一个 24 条题库统一跑 |
| 中文口语输入（带错别字/口语）鲁棒性 | 未做 |
| 对抗性输入（诱导 skill 输出政治结论而非方法） | 未做 —— 这是本项目最需要补的一类测试 |

---

## 附：原始文件

- 测试用例：`skills/*/test-prompts.json`
- 盲测输入：`work/route/router_input.md`
- 第一轮输出 / 计分：`work/route/router_output.md`、`work/score_route2.py`（43/48）
- 第二轮输出 / 计分：`work/route/router_output2.md`、`work/score_route3.py`（48/48）
- 标准答案：`work/route/truth.json`
