# 七哥论国际 方法论 skill 家族 · 总索引

**family**: `qige-guolunji` · **family_version**: 2.0.0
**来源**：《七哥论国际：直播文字稿 2023-2026》，89 篇 / 148.6 万字符（剔除带货后 135.3 万）
**构成**：7 个存量 skill（v1，2026-08-12 蒸馏）+ 8 个新增 skill（v2，2026-09-16 全量蒸馏）+ 1 个总纲路由
**规模**：共 **16 个 skill**

---

## 一、为什么是「整合」而不是「合并成一个」

15 个原子 skill 两两之间的重叠度经核查后，**只有 1 组是真重复**（统战价值/谁买单，
同时出现在 `proxy-war-cost-trace` 与 `patronage-value-grading`），其余 6 组是**上下位关系**而非重复：

| 看起来重复 | 实际分工 | 处理 |
|---|---|---|
| `attrition-long-game` × `timing-window-cadence` | 前者答"谁的耐力更强/该不该拖"，后者答"窗口在几月、谁在拖" | 保留，加互指 |
| `structural-necessity-forecast` × `endgame-scripting` | 前者答"会不会升级（退路是否为零）"，后者答"最后怎么收场（最优收敛态）" | 保留，加互指 |
| `hegemony-collapse-chain` × `coalition-fracture-index` | 前者是体系三环（军事→美元→资本）塌方顺序，后者是同盟成员裂痕排序 | 保留，加互指 |
| `great-power-master-switch` × `causal-chain-consistency` | 前者做归因定位，后者是可证伪性的元规则 | 保留，加互指 |
| `industrial-base-power-check` × `strategy-tactics-audit` | 前者查工业地基，后者做战略/战术分层与制度成本账 | 保留，加互指 |
| `proxy-war-cost-trace` × `patronage-value-grading` | **真重叠**：都讲"统战价值"与"谁买单" | 保留各自内容，但用路由明确分工：决策时点归后者，成本矩阵归前者 |

**结论**：强行合并会破坏"一个 skill 只做一个方法论单元"的原子性，
并让 trigger 变模糊（v1 的实测已证明 trigger 模糊是最大失分源）。
因此本次整合的做法是 **保原子性 + 消除抢调用 + 加总纲**。

---

## 二、16 个 skill 全表

### 入口层

| skill | 用途 |
|---|---|
| **`qige-analysis`** | 总纲与路由：九步分析链 + 分派表。用户说"用七哥的方法分析"时走这里 |

### 定位层（先回答"在哪、属于哪一步"）

| skill | 一句话 | 版本 |
|---|---|---|
| `map-first-geostrategy` | 位置先于动机：咽喉、辐射圈、必争与宿敌 | v1 |
| `great-power-master-switch` | 总开关归因：是不是中美外溢、对谁有利、谁买单 | v1 |

### 约束层（回答"会不会发生、什么时候、谁撑得住"）

| skill | 一句话 | 版本 |
|---|---|---|
| `structural-necessity-forecast` | 数退路：打不赢/走不掉/谈不拢 → 结构必然 | v1 |
| `timing-window-cadence` | 标日历窗口 + 判节奏归属 + 谈判即消耗 | v2 新 |
| `attrition-long-game` | 耐力赛：强者拖、弱者赌窗口、先急者输 | v1 |
| `industrial-base-power-check` | 查工业地基（电力/重工业/供应链/工程师） | v1 |

### 读牌层（回答"它真正想干嘛、我该不该改判断"）

| skill | 一句话 | 版本 |
|---|---|---|
| `adversary-intent-read` | 读动作不读表态：异常与"缺席"即底牌 | v2 新 |
| `causal-chain-consistency` | 来龙去脉闭合检验 + 何时该停止解释 | v2 新 |
| `forecast-self-audit` | 给强判断补"除非…"，拒绝单变量与远期具体化 | v2 新 |

### 主体层（回答"谁是谁、谁付账、该不该介入"）

| skill | 一句话 | 版本 |
|---|---|---|
| `patronage-value-grading` | 统战价值打分 + 一盘棋/家族集团 + 追买单人 | v2 新 |
| `proxy-war-cost-trace` | 玩家矩阵与成本不对称，预测谁先动摇 | v1 |
| `coalition-fracture-index` | 信用锚点 + 第一道防线的口子 + 反围剿 | v2 新 |

### 评估与收场层

| skill | 一句话 | 版本 |
|---|---|---|
| `strategy-tactics-audit` | 战术/战略分栏 + 查开战权/主动权/结束权 | v2 新 |
| `hegemony-collapse-chain` | 军事可信度→美元信用→资本流动，找承重环 | v1 |
| `endgame-scripting` | 非对称胜负 → 最优收敛态 → 终局分工 → 留盼头 | v2 新 |

---

## 三、标准调用链

```
用户提问
  ↓
qige-analysis（判断是否需要走全链）
  ↓
[1] map-first-geostrategy          ← 它在哪？
[2] great-power-master-switch      ← 属于哪一步？
[3] structural-necessity-forecast  ← 退路还有几条？
[4] strategy-tactics-audit         ← 战术赢还是战略赢？
[5] timing-window-cadence          ← 什么时候动？
    attrition-long-game            ← 谁拖得起？
[6] patronage-value-grading        ← 该不该介入？
    proxy-war-cost-trace           ← 成本怎么分？
[7] industrial-base-power-check    ← 地基撑不撑？
    coalition-fracture-index       ← 同盟哪里先裂？
[8] endgame-scripting              ← 剧本怎么走？
    hegemony-collapse-chain        ← 体系怎么塌？
[9] forecast-self-audit            ← 什么情况算我错了？
  ↓
贯穿：adversary-intent-read（读牌）+ causal-chain-consistency（元规则）
```

---

## 四、安装与维护

- **安装位置**：`~/.codex/skills\<slug>\`
- **每个 skill 含**：`SKILL.md` + `test-prompts.json`（darwin 兼容，`minimum_pass_rate: 0.8`）
- **v1 的 7 个 skill 另有** `test-results.md`（2026-08-12 蒸馏时的记录）
- **统一元数据**：全部带 `family: qige-guolunji` 与 `family_version: 2.0.0`，可据此批量筛选与升级
- **升级方式**：`family_version` 递增；新增子 skill 只需带同一 `family` 标签并补进本索引

---

## 五、已知局限（与 v1 一致，未因整合而消除）

1. **未逐字通读全部语料**：v2 的 8 个 skill 走的是"5 路并行提取 + 预筛证据通读 + 原文定向检索"，
   大文件可能有漏网的方法论单元。
2. **`AI分析方法论.md` 未纳入**（用户明确要求忽略）。
3. **未评估其判断正确率**：家族蒸馏的是"他怎么分析"，不是"他分析得对不对"。
4. **抢调用测试的样本量小**：v2 首轮 43/48，定向修补 description 后复测 48/48，
   但第二轮属于"教到考卷上"，泛化能力需用新题复测。
5. **立场风险**：该语料立场鲜明（"咱家"视角），引用时应标明来源，避免把其结论当事实转述。
