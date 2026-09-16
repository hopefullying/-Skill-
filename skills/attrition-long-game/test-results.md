# test-results — attrition-long-game

- **执行方式**: 主流程自测（fallback）。
- **测试用例**: 6 条（3 should_trigger + 2 should_not_trigger + 1 edge_case，含跨 skill 诱饵）
- **通过率**: 6/6 (100%)

| id | 类型 | 判定 | 说明 |
|---|---|---|---|
| should-trigger-01 | should_trigger | 通过 | “科技战谁能耗得起”命中耐力判断 |
| should-trigger-02 | should_trigger | 通过 | “对方加码是不是急了”命中先急信号 |
| should-trigger-03 | should_trigger | 通过 | 英文 “who can outlast / long game” 命中 |
| should-not-trigger-01 | should_not_trigger | 通过 | 股票短线操作属短期交易，description 排除 |
| should-not-trigger-02 | should_not_trigger | 通过 | “军事神话击穿霸权崩”应转 hegemony-collapse-chain（跨 skill 诱饵） |
| edge-01 | edge_case | 通过 | 现金流三个月→触发但判停转“先止血”（E 判停条件） |

**结论**: 接受。
