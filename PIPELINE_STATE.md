# PIPELINE_STATE — 《七哥论国际》直播文字稿蒸馏

> 断点续跑用。每完成一个阶段更新本文件。

## 元信息

- book-slug: `qige-geopolitics`
- 内容: 主播“七哥论国际”2023-12 至 2026-08 直播文字稿 84 份（约 138 万汉字）
- 蒸馏方法: cangjie-skill (RIA-TV++)

## 阶段状态

- [x] 阶段 0 — 整书理解 (BOOK_OVERVIEW.md)
- [x] 阶段 1 — 5 路提取完成 (candidates/ 5 类齐备；sub-agent 通道不稳定，按降级方案由主流程串行补齐 4 类)
- [x] 阶段 1.5 — 三重验证 (verified.md 通过 8 单元 / rejected/)
- [x] 阶段 2 — RIA++ 构造 skill（8 个 SKILL.md）
- [x] 阶段 3 — Zettelkasten 链接 (INDEX.md / GLOSSARY.md)
- [x] 阶段 4 — 压力测试 (8×test-prompts.json + test-results.md；独立盲测通道不稳定，按降级方案主流程自测，已在各 test-results.md 标注 fallback；发现并修复 master-switch 与 proxy 的触发重叠)
- [x] 阶段 5 — 交付 (DIGEST.md 完成；用户选择“发布用”，不安装宿主；已生成 README.md 作为发布入口)

## 下一步

- 全部流水线阶段完成。用户选择“发布用”：保持仓库形式，不安装宿主；包内容自包含，可直接发布。
- 可选: 接入 darwin-skill 进化 `darwin evolve books/qige-geopolitics/`。
