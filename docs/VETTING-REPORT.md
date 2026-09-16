# SKILL VETTING REPORT · qige-guolunji 家族（16 个 skill）

审查执行：2026-09-16 ｜ 规程：`~/.codex/skills/skill-vetter/SKILL.md`（四步协议）

═══════════════════════════════════════

## 批次概览

| 项 | 值 |
|---|---|
| Skill 数量 | 16（7 个存量 v1 + 8 个新增 v2 + 1 个总纲路由） |
| 文件总数 | **39**（`.md` × 23，`.json` × 16） |
| 可执行文件 / 脚本 | **0** |
| 来源 | **本项目自产**：v1 于 2026-08-12 由本机 agent 从用户自有语料蒸馏；v2 于 2026-09-16 由本次会话从同一语料蒸馏 |
| 第三方来源 | 无（未从 ClawdHub / GitHub / 任何外部源下载） |

---

## Step 1 · 来源检查

- [x] 来源：用户自己的飞书文件夹「七哥论国际 文字版」→ 本机蒸馏产物，**非第三方分发**
- [x] 作者：本机 agent（v1 由用户既有会话产出，v2 由本次会话产出）
- [x] 下载/星标数：不适用（非公开发布物）
- [x] 最后更新：v1 = 2026-08-12；v2 = 2026-09-16
- [x] 其他 agent 评价：不适用

**结论**：来源透明、可追溯到具体语料文件与提取脚本，无供应链风险。

---

## Step 2 · 代码审查（逐文件）

对 39 个文件全部做了正则红flag扫描（脚本：`work/vet_scan.py`），覆盖：

| 红 flag | 扫描结果 |
|---|---|
| `curl` / `wget` / `Invoke-WebRequest` | **0 处** |
| 外发数据（`requests.post` / `fetch(` / `axios` / `urllib`） | **0 处** |
| 凭据读取（`.ssh` / `.aws` / `api_key` / `app_secret` / `token.json` / `keychain`） | **0 处** |
| `base64` / `atob` / `b64decode` | **0 处** |
| `eval()` / `exec()` / `subprocess` / `os.system` / `child_process` | **0 处** |
| 系统修改（registry / HKLM / sudo / schtasks） | **0 处** |
| 包安装（pip / npm / choco / winget install） | **0 处** |
| 浏览器数据（cookies / Login Data / Local State） | **0 处** |
| 任何 `http(s)://` 外链 | **0 处** |
| 混淆（`\xNN` / `\uNNNN` 转义） | **0 处** |

**文件类型分布**：`.md` 23 个（方法论正文）+ `.json` 16 个（darwin 兼容测试用例）。

**人工确认**：`.json` 全部是测试用例（`prompt` / `expected_behavior` / `notes`），无指令注入载荷；
`.md` 全部是叙述性方法论正文 —— 已确认正文里**不含**任何要求 agent 执行外部动作的指令。

---

## Step 3 · 权限范围

| 权限 | 需要？ | 说明 |
|---|---|---|
| 文件读 | 否 | skill 本身不读取任何文件 |
| 文件写 | 否 | 不写文件 |
| 网络 | 否 | 无任何网络调用 |
| 命令执行 | 否 | 无可执行内容 |
| 凭据 | 否 | 不接触任何凭据 |

**作用机理**：这些 skill 是**纯提示词资产** —— 被激活时只向对话上下文注入方法论正文。
全部副作用仅限"影响模型输出内容"，不产生任何系统级操作。

---

## Step 4 · 风险分级

| 维度 | 评估 |
|---|---|
| 技术风险 | 🟢 LOW —— 无可执行代码、无网络、无凭据、无文件操作 |
| 内容风险 | 🟡 MEDIUM —— **这是本批次唯一的实质风险**，见下 |

### 内容风险说明（必须记录）

该语料来自一名立场鲜明的主播，其分析含：
1. **强立场预设**（"咱家"视角，以中国必胜为出发点）
2. **不可证伪表述**（"必然/铁定/百分百"密集）
3. **贬义代称**（二狗子、飞猴、鬼子等）

→ 已在 `GLOSSARY.md` 第五节写明"代称自带贬义与阵营预设，引用时须加引号并标注来源"；
→ 已在每个相关 skill 的 **B 段（边界）** 写明已知硬伤与失效条件；
→ 已新增 `forecast-self-audit` 专门承担"给判断装刹车"角色；
→ `qige-analysis` 总纲的 B 段明确要求**输出方法而非结论**，并强制标注三条结构性偏差。

---

## 风险结论

```
RISK LEVEL: 🟢 LOW（技术） / 🟡 MEDIUM（内容立场）
VERDICT: ✅ SAFE TO INSTALL
```

**放行理由**：技术上零攻击面（纯文本、无代码、无 IO、无网络）；
内容上的立场风险已通过文档约束、边界段与专用自审 skill 三重缓解，
且属于用户自有语料的自然属性，不构成安全威胁。

**安装前须做的动作**：
1. 备份既有 7 个 v1 skill（防止整合版覆盖后不可回滚）
2. 记录 39 个文件的 SHA-256 前 16 位（`work/family_manifest.json`），便于日后校验未被篡改
3. 安装后复核文件数与 manifest 一致

═══════════════════════════════════════

## 附：待安装文件清单（39）

| skill | 版本 | 文件 |
|---|---|---|
| map-first-geostrategy | v1 + 整合补丁 | SKILL.md, test-prompts.json, test-results.md |
| great-power-master-switch | v1 + 整合补丁 | 同上 |
| proxy-war-cost-trace | v1 + 整合补丁 | 同上 |
| attrition-long-game | v1 + 整合补丁 | 同上 |
| hegemony-collapse-chain | v1 + 整合补丁 | 同上 |
| industrial-base-power-check | v1 + 整合补丁 | 同上 |
| structural-necessity-forecast | v1 + 整合补丁 | 同上 |
| timing-window-cadence | v2 新 | SKILL.md, test-prompts.json |
| adversary-intent-read | v2 新 | 同上 |
| endgame-scripting | v2 新 | 同上 |
| strategy-tactics-audit | v2 新 | 同上 |
| causal-chain-consistency | v2 新 | 同上 |
| patronage-value-grading | v2 新 | 同上 |
| forecast-self-audit | v2 新 | 同上 |
| coalition-fracture-index | v2 新 | 同上 |
| qige-analysis（总纲路由） | v2 新 | 同上 |
