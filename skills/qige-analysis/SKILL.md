---
name: qige-analysis
description: |
  「七哥论国际」分析方法论总纲与路由器。当用户要求"用七哥的方法/按这套框架分析"某件国际事件，
  或提出一个跨领域的战略问题（谁占上风、最后怎么收场、该不该介入、时间在谁那边）时，
  用本 skill 走完九步分析链并分派到对应的原子 skill。触发词："用七哥的方法分析""七哥方法论"
  "按这套框架看""七哥会怎么看""他用什么逻辑得出的"；英文 "qige method / how would Qige analyze this".
  不适用：用户只问一个具体子问题（直接调用对应子 skill 即可）、或需要立场站队而非方法复现。
source_book: 《七哥论国际：直播文字稿 2023-2026》 主播"七哥"
source_chapter: 全语料 89 篇（2023-12-22 ~ 2026-09-15）综合
family: qige-guolunji
family_version: 2.0.0
tags: [methodology, router, meta, geopolitics, strategy]
related_skills:
  - slug: map-first-geostrategy
    relation: composes-with
  - slug: great-power-master-switch
    relation: composes-with
  - slug: structural-necessity-forecast
    relation: composes-with
  - slug: endgame-scripting
    relation: composes-with
---

# 七哥分析方法论 · 总纲与路由

## R — 出处 (Source)

- 2024-1-12_原文.md :: 34:08
- 2024-1-12_原文.md :: 35:32

> **说明**：为避免转载第三方直播内容，此处不保留原话引用；方法论骨架见下方 I 段（本方重述），
> 逐条出处与时间戳见仓库根目录 `SOURCES.md`。

## I — 方法论骨架 (Interpretation)

**一句话**：回地图 → 定主矛盾 → 数退路 → 分战略战术 → 算成本与时间窗 → 定棋子 → 查工业地基 → 给剧本 → 装刹车。

三条不变式（他从不放弃的底层命题）：

| 不变式 | 内容 |
|---|---|
| 主矛盾不变 | 区域事件"都是中美矛盾的外溢" |
| 位置不变 | 换个政府坐在同一位置上，行为模式趋同 |
| 耐心不对称 | 一方要速决（选举/库存/财政），一方能拖；**谁先急谁露底牌** |

---

## A1 — 九步分析链与分派表

| 步 | 动作 | 交给谁 |
|---|---|---|
| 1 | 位置先于动机：找咽喉、画辐射圈、看战线联通 | `map-first-geostrategy` |
| 2 | 定主矛盾：是不是中美外溢？对谁有利、谁买单？ | `great-power-master-switch` |
| 3 | 数退路：打不赢 / 走不掉 / 谈不拢 → 结构必然 | `structural-necessity-forecast` |
| 4 | 分层：战术打分 vs 战略打分；查开战权/主动权/结束权 | `strategy-tactics-audit` |
| 5 | 算成本与时间窗：日历节点、维持成本、谈判即消耗 | `timing-window-cadence` + `attrition-long-game` |
| 6 | 定棋子：统战价值、一盘棋 vs 家族集团、追买单人 | `patronage-value-grading`（成本矩阵细节用 `proxy-war-cost-trace`） |
| 7 | 查地基与裂痕：工业地基 / 同盟第一道防线的口子 | `industrial-base-power-check` + `coalition-fracture-index` |
| 8 | 给剧本：非对称胜负 → 最优收敛态 → 终局分工 → 留盼头 | `endgame-scripting` |
| 9 | 装刹车：补"除非…"、查单变量、拒远期具体化 | `forecast-self-audit` |

**两条贯穿全程的元规则**：`causal-chain-consistency`（该不该改判断）、`adversary-intent-read`（对手真实目的）。

---

## A2 — 触发场景 (Appropriation)

- "用七哥的方法分析一下这件事"
- "七哥会怎么看这个局"
- 用户抛出一个跨领域的大问题（谁占上风 / 最后怎么收场 / 该不该介入 / 时间在谁那边），
  没有明显落到某一个子 skill 的触发词上。

---

## E — 可执行步骤 (Execution)

1. **先查元规则**：这条信息能串进来龙去脉吗？串不起来先挂起（`causal-chain-consistency`）。
2. **按九步走，缺哪步补哪步**：不要跳步直接给结论，尤其不能跳过第 3 步（数退路）和第 9 步（装刹车）。
3. **每步调用对应子 skill**，并把该子 skill 的 E 段输出汇总。
4. **输出结构固定为四段**：
   - ① 结构与位置（1-2 步）
   - ② 约束与时间（3-5 步）
   - ③ 主体与裂痕（6-7 步）
   - ④ 剧本与失效条件（8-9 步）
5. **强制收尾**：至少一条"除非…"的失效条件 + 至少一条被忽略的本地因素。

---

## B — 边界与失效条件 (Boundary)

- **这是复现方法，不是复现结论**：本 skill 的产出应是一套可检验的推理链，
  而不是"七哥说过美国必败"这类立场转述。
- **不要把必然性话语当结论输出**：他本人大量使用"必然/铁定"，这正是其方法论最脆弱处。
  走第 9 步时必须写明证伪条件与期限。
- **已知硬伤要在输出里显式标注**：单变量归因（一切归到中美）、立场先行（以"咱家必胜"为出发点）、
  选择性追溯（只记"我早就说了"）。这三条是其体系的结构性偏差。
- **不做事实核查**：本 skill 只负责方法复现；他引用的数据（如 55% 生死线）是其情景设定，不是外部事实。
