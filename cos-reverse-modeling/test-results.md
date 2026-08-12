# test-results — cos-reverse-modeling

- **执行方式**: 主流程自测（fallback）——独立 sub-agent 盲测通道不稳定（多次 spawn 消息丢失），按 cangjie-skill 阶段 4 降级方案执行。可信度低于独立盲测。
- **测试用例**: 6 条（3 should_trigger + 2 should_not_trigger + 1 edge_case，含 1 条跨 skill 混淆诱饵）
- **通过率**: 6/6 (100%)

| id | 类型 | 判定 | 说明 |
|---|---|---|---|
| should-trigger-01 | should_trigger | 通过 | “反向建模认知操作系统”命中 description 首句 |
| should-trigger-02 | should_trigger | 通过 | “提炼分析框架和预测逻辑”命中 trigger |
| should-trigger-03 | should_trigger | 通过 | 英文 trigger 命中 |
| should-not-trigger-01 | should_not_trigger | 通过 | “总结三点”属单文本摘要，description 明确排除 |
| should-not-trigger-02 | should_not_trigger | 通过 | “用地图分析伊朗”应转 map-first-geostrategy（跨 skill 诱饵） |
| edge-01 | edge_case | 通过 | 两篇文章→触发但明确低置信度/样本不足（description 的批量前提） |

**结论**: 接受。description 已含“何时调用+何时不调用+中英 trigger”。
