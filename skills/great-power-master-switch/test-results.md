# test-results — great-power-master-switch

- **执行方式**: 主流程自测（fallback）。
- **测试用例**: 6 条（3 should_trigger + 2 should_not_trigger + 1 edge_case，含跨 skill 诱饵）
- **通过率**: 6/6 (100%)

| id | 类型 | 判定 | 说明 |
|---|---|---|---|
| should-trigger-01 | should_trigger | 通过 | “政变背后是不是大国博弈”命中外溢/归因 |
| should-trigger-02 | should_trigger | 通过 | “对中美谁有利”命中总开关 |
| should-trigger-03 | should_trigger | 通过 | 英文 “US-China rivalry” 命中 |
| should-not-trigger-01 | should_not_trigger | 通过 | 欧盟法规总结属信息任务，排除 |
| should-not-trigger-02 | should_not_trigger | 通过 | “内战谁出钱出人”应转 proxy-war-cost-trace（跨 skill 诱饵） |
| edge-01 | edge_case | 通过 | 选举内政影响外交→先内政后外交衔接，说明边界 |

**修复记录**: 自测发现 description 中“谁买单”一词与 proxy-war-cost-trace 抢调用；已改为“谁受益最大”，并在 description 末尾显式注明“出钱/出人/成本账转 proxy-war-cost-trace”。

**结论**: 接受（修复后）。
