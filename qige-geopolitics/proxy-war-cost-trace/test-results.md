# test-results — proxy-war-cost-trace

- **执行方式**: 主流程自测（fallback）。
- **测试用例**: 6 条（3 should_trigger + 2 should_not_trigger + 1 edge_case，含跨 skill 诱饵）
- **通过率**: 6/6 (100%)

| id | 类型 | 判定 | 说明 |
|---|---|---|---|
| should-trigger-01 | should_trigger | 通过 | “代理人战争谁会先撑不住”命中 |
| should-trigger-02 | should_trigger | 通过 | “俄乌谁买单”命中买单矩阵 |
| should-trigger-03 | should_trigger | 通过 | 英文 “who is paying / proxy war” 命中 |
| should-not-trigger-01 | should_not_trigger | 通过 | GDP 差距属数据计算，排除 |
| should-not-trigger-02 | should_not_trigger | 通过 | “伊朗位置为什么重要”应转 map-first-geostrategy（跨 skill 诱饵） |
| edge-01 | edge_case | 通过 | 无外部支持内战→不适用代理框架，转内部资源分析（B 段判停） |

**结论**: 接受。
