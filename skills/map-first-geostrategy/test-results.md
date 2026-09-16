# test-results — map-first-geostrategy

- **执行方式**: 主流程自测（fallback）——独立 sub-agent 盲测通道不稳定，按降级方案执行。
- **测试用例**: 6 条（3 should_trigger + 2 should_not_trigger + 1 edge_case，含跨 skill 诱饵）
- **通过率**: 6/6 (100%)

| id | 类型 | 判定 | 说明 |
|---|---|---|---|
| should-trigger-01 | should_trigger | 通过 | “霍尔木兹海峡为什么重要”命中咽喉/海峡 trigger |
| should-trigger-02 | should_trigger | 通过 | “内陆国地理位置影响命运”命中地缘/缓冲带 |
| should-trigger-03 | should_trigger | 通过 | 英文 “strategically important” 命中 |
| should-not-trigger-01 | should_not_trigger | 通过 | 美联储利率属纯金融，description 排除 |
| should-not-trigger-02 | should_not_trigger | 通过 | “谁能耗得起贸易战”应转 attrition-long-game（跨 skill 诱饵） |
| edge-01 | edge_case | 通过 | 无咽喉内陆国→说明地理权重低并转其他框架（E5 判停） |

**结论**: 接受。
