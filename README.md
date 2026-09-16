# 七哥论国际 · 分析方法论 Skill 集

> 把一位国际时评主播在 **89 场直播 / 148.6 万字**里反复使用的分析方法，
> 逆向整理成 **16 个可被 AI agent 直接调用**的原子化 skill。
>
> ⚠️ 本仓库**不含任何原话引用**——所有描述都是提炼者的重述，出处见 [`SOURCES.md`](SOURCES.md)。请先读 [`DISCLAIMER.md`](DISCLAIMER.md)。

[![family](https://img.shields.io/badge/family-qige--guolunji-blue)]()
[![version](https://img.shields.io/badge/version-2.0.0-green)]()
[![skills](https://img.shields.io/badge/skills-16-orange)]()
[![license](https://img.shields.io/badge/license-CC%20BY--NC--SA%204.0-lightgrey)](LICENSE)

---

## 这是什么

这不是"七哥语录合集"，而是一套**方法论拆解**。

我们做的事：把主播用来得出判断的**推理结构**抽出来，做成可复用的分析流程——
而不是复述他的结论。

| 你要做的事 | 这套东西能给你的 |
|---|---|
| 理解一场冲突为什么这么走 | 一张九步分析链，每步都有可检验的判据 |
| 判断"谁占上风" | 战术/战略分层打分 + 开战权/主动权/结束权三查 |
| 预测"最后怎么收场" | 非对称胜负条件 → 最优收敛态 → 剧本化输出 |
| 评估"该不该介入" | 统战价值打分 + 谁买单追踪 |
| 给自己的判断装刹车 | 强制补"除非…"，拒绝单变量与远期具体化 |

**核心设计原则**：一个 skill 只做一个方法论单元，trigger 明确，边界写死。
每个 skill 都带 darwin 兼容的测试用例。

---

## 快速开始

### 方式一：作为 Codex / Claude Skill 安装

```bash
git clone <your-repo-url> qige-guolunji
cp -r qige-guolunji/skills/* ~/.codex/skills/
```

Windows (PowerShell)：

```powershell
git clone <your-repo-url> qige-guolunji
Copy-Item .\qige-guolunji\skills\* "$env:USERPROFILE\.codex\skills\" -Recurse -Force
```

安装后，直接提问即可自动命中对应 skill：

```
它三艘航母摆着又不打，是虚张声势吗？
谈判谈了十几轮还没结果，到底谁在拖？
美国打不赢一个地区国家算不算输？
用七哥的方法分析一下这次停火谈判。      ← 走总纲 qige-analysis
```

### 方式二：当分析清单手动用

不想装 skill，就照九步走一遍：

```
1 回地图        →  它在哪？掐着哪条咽喉？
2 定主矛盾      →  对谁有利、谁被消耗、谁买单？
3 数退路        →  打不赢 / 走不掉 / 谈不拢？
4 分两层        →  战术赢还是战略赢？结束权在谁手里？
5 算成本与时间窗 →  日历节点在哪？谁拖不起？
6 定棋子        →  统战价值打出来没有？谁付账？
7 查地基与裂痕  →  工业本底？同盟第一道防线有口子吗？
8 给剧本        →  最优收敛态是什么？排第一步/第二步/第三步
9 装刹车        →  这个判断的"除非……"是什么？
```

---

## 16 个 skill

### 入口

| skill | 用途 |
|---|---|
| **`qige-analysis`** | 总纲与路由：九步分析链 + 分派表 |

### 定位层

| skill | 一句话 |
|---|---|
| `map-first-geostrategy` | 位置先于动机：咽喉、辐射圈、必争与宿敌 |
| `great-power-master-switch` | 总开关归因：是不是大国博弈的外溢 |

### 约束层

| skill | 一句话 |
|---|---|
| `structural-necessity-forecast` | 数退路：退路为零 → 升级是结构必然 |
| `timing-window-cadence` | 标日历窗口 + 判节奏归属 + 谈判即消耗 |
| `attrition-long-game` | 耐力赛：强者拖、弱者赌窗口、先急者输 |
| `industrial-base-power-check` | 查工业地基：电力/重工业/供应链/工程师 |

### 读牌层

| skill | 一句话 |
|---|---|
| `adversary-intent-read` | 读动作不读表态：异常与"缺席"即底牌 |
| `causal-chain-consistency` | 来龙去脉闭合检验 + 何时该停止解释 |
| `forecast-self-audit` | 给强判断补"除非…"，拒绝单变量推结局 |

### 主体层

| skill | 一句话 |
|---|---|
| `patronage-value-grading` | 统战价值打分 + 盘棋/家族集团 + 追买单人 |
| `proxy-war-cost-trace` | 玩家矩阵与成本不对称，预测谁先动摇 |
| `coalition-fracture-index` | 信用锚点 + 第一道防线的口子 + 反围剿 |

### 评估与收场层

| skill | 一句话 |
|---|---|
| `strategy-tactics-audit` | 战术/战略分栏 + 查开战权/主动权/结束权 |
| `hegemony-collapse-chain` | 军事可信度→美元信用→资本流动，找承重环 |
| `endgame-scripting` | 非对称胜负 → 最优收敛态 → 终局分工 → 留盼头 |

---

## 仓库结构

```
qige-guolunji/
├── README.md                  ← 你在这里
├── LICENSE                    ← CC BY-NC-SA 4.0
├── DISCLAIMER.md              ← 来源声明 + 立场声明（请先读）
├── LICENSING.md               ← 授权决策说明
├── SOURCES.md                 ← 语料出处索引（无原话引用）
├── CHANGELOG.md
├── index.json                 ← 机器可读的技能清单
├── .codex-plugin/plugin.json  ← Codex 插件清单
├── skills/                    ← 16 个 skill（每个含 SKILL.md + test-prompts.json）
└── docs/
    ├── DIGEST.md              ← 方法论说明书（建议从这里开始读）
    ├── GLOSSARY.md            ← 黑话词典（65+ 条）
    ├── INDEX.md               ← 整合设计与去重说明
    ├── BOOK_OVERVIEW.md       ← 语料骨架与批判
    ├── VERIFICATION.md        ← 三重验证与筛选依据
    ├── TEST-RESULTS.md        ← 路由盲测记录（88/96 → 92/96）
    └── VETTING-REPORT.md      ← skill-vetter 安全审查报告
```

**建议阅读顺序**：`docs/DIGEST.md` → `docs/GLOSSARY.md` → `skills/qige-analysis/SKILL.md` → 其余按需。

---

## 质量说明

| 项 | 数据 |
|---|---|
| 语料规模 | 89 篇直播文字稿 / 148.6 万字符（2023-12 ~ 2026-09） |
| 提取方式 | 5 路并行提取器 → 148 条候选 → 三重验证 → 16 个 skill |
| 溯源校验 | 提炼依据的 160 条出处坐标逐条回查原文通过；发布版**不含任何原话引用** |
| 路由盲测 | 96 条用例：首轮 88/96 (91.7%)，修补 description 后 92/96 (95.8%) |
| 诱饵测试 | 32 / 32 —— **零误触发**（含兄弟 skill 互相抢调用的混淆诱饵） |
| 安全审查 | skill-vetter 四步协议：**0 个红 flag**（纯文本，无代码/网络/凭据） |

### 已知局限（不藏）

1. 提取器以"预筛证据通读 + 原文定向检索"为主，**未逐字通读全部 148 万字符**。
2. 路由测试的 95.8% 属于"修补后复测同一套题"，泛化能力需新题复测。
3. **未评估其判断的正确率**——本包整理的是"他怎么分析"，不是"他分析得对不对"。
4. 语料立场鲜明，详见 `DISCLAIMER.md`。

---

## 贡献

- 新 skill 请带 `family: qige-guolunji` 与 `family_version` 字段，并补进 `index.json`
- 每个 skill 必须带 `test-prompts.json`（≥3 正例 + ≥2 诱饵 + ≥1 边界，诱饵容错为 0）
- **禁止提交原话引用**：描述须为提炼者自己的重述，出处以「文件名 + 时间戳」形式写入 `SOURCES.md`
- PR 前请跑 `docs/VERIFICATION.md` 里描述的引文回验

---

## 授权

- **本仓库的整理成果**（框架描述、目录结构、测试用例、说明书）：CC BY-NC-SA 4.0
- **原始语料**：著作权归原讲者/权利人。本仓库**不含任何原话引用**，仅提供出处坐标（见 `SOURCES.md`）
- 详见 `LICENSE` 与 `LICENSING.md`
