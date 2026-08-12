# 《七哥论国际》地缘政治认知操作系统 — Skill 蒸馏包

> 由 cangjie-skill（RIA-TV++）从主播“七哥”2023-12 至 2026-08 的 **84 份直播文字稿（约 138 万汉字）** 蒸馏而来。
> 本包是**发布/仓库形式**：内容自包含，可直接作为 GitHub 仓库发布，或按需安装到宿主的 skills 目录。

## 这是什么

不是语料摘要，而是一组**可执行的认知模型 skill**：把七哥分析国际政治时反复使用的地缘、国力、归因、预测框架，蒸馏成 agent 可以在真实场景中调用的原子化方法论。每个 skill 都经过三重验证（跨域/预测力/独特性）与压力测试（含跨 skill 混淆诱饵），并附 darwin-skill 兼容的测试用例。

## 快速上手

1. **人类读者**：读 [DIGEST.md](./DIGEST.md)（精华长文，约 12 分钟）。
2. **要使用 skill 的 agent 用户**：把任意 skill 目录复制到宿主的 skills 目录：

```bash
# Claude Code / Codex 用户级
cp -r <skill-slug> ~/.claude/skills/    # 或 ~/.codex/skills/

# 项目级
cp -r <skill-slug> <project>/.claude/skills/
```

3. **要持续进化**：接入 darwin-skill：

```bash
darwin evolve books/qige-geopolitics/
```

## 包结构

```
qige-geopolitics/
├── README.md              # 本文件（发布入口）
├── BOOK_OVERVIEW.md       # 阶段 0：整书理解与批判（含作者局限）
├── verified.md            # 阶段 1.5：三重验证通过的 8 个单元
├── INDEX.md               # skill 总览 + 引用图 + 学习顺序
├── GLOSSARY.md            # 共享术语词典（作者用法）
├── DIGEST.md              # 面向读者的精华长文
├── PIPELINE_STATE.md      # 流水线状态（断点续跑/审计）
├── candidates/            # 阶段 1：77 条原始候选（审计用）
├── rejected/              # 阶段 1.5：淘汰单元 + 原因（可捞回）
├── evidence/              # 证据包（COS 报告、概念频次统计）
└── <skill-slug>/          # 8 个 skill，每个含：
    ├── SKILL.md           # R/I/A1/A2/E/B 六段 + frontmatter trigger
    ├── test-prompts.json  # darwin 兼容测试用例
    └── test-results.md    # 压力测试结果
```

## 8 个 skill 一览

| skill                           | 用途                                           |
| ------------------------------- | ---------------------------------------------- |
| `cos-reverse-modeling`          | 从任意评论员文本反向建模认知操作系统（元方法） |
| `map-first-geostrategy`         | 地图优先：位置→战略价值→必争逻辑→宿敌推演      |
| `industrial-base-power-check`   | 工业地基评估：电力/重工业/供应链/纵深          |
| `hegemony-collapse-chain`       | 霸权串行链：军事→美元→资本，纸老虎验证         |
| `great-power-master-switch`     | 中美总开关：区域事件外溢归因                   |
| `proxy-war-cost-trace`          | 代理人成本账：谁出钱、谁出人、谁买单           |
| `attrition-long-game`           | 消耗战/马拉松：强者拖、弱者赌                  |
| `structural-necessity-forecast` | 结构必然性预测：数退路判必打/必崩/必换政权     |

## 安全与质量说明

- 所有 skill 均为**纯 Markdown + JSON**，无脚本、无网络调用、无敏感权限，可安全审查后安装。
- 8/8 skill 通过三重验证；压力测试 6/6 通过（主流程自测 fallback，已在各 test-results.md 标注）。
- 使用提示：本包方法是“强解释力、弱证伪性”的分析工具；用其“必然性”预测时请自行补充证伪条件（详见各 skill 的 Boundary 段与 DIGEST.md“作者的局限”）。

## 审计与授权

- 语料来源：用户提供的飞书导出文字稿（84 个 docx）。
- 蒸馏方法：cangjie-skill（RIA-TV++）。
- 处理时间：2026-08-12。
- 发布前请自行补充 LICENSE（本包未内置授权条款）。
