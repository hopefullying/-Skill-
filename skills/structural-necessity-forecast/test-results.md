# test-results — structural-necessity-forecast

- **执行方式**: 主流程自测（fallback）。
- **测试用例**: 6 条（3 should_trigger + 2 should_not_trigger + 1 edge_case，含跨 skill 诱饵）
- **通过率**: 6/6 (100%)

| id | 类型 | 判定 | 说明 |
|---|---|---|---|
| should-trigger-01 | should_trigger | 通过 | “被逼墙角会不会孤注一掷”命中退路计数 |
| should-trigger-02 | should_trigger | 通过 | “内塔尼亚胡会不会下台”命中政权更替联动 |
| should-trigger-03 | should_trigger | 通过 | 英文 “no way out / escalate” 命中 |
| should-not-trigger-01 | should_not_trigger | 通过 | 联合国投票查询属事实查询，排除 |
| should-not-trigger-02 | should_not_trigger | 通过 | “美元信用先崩”应转 hegemony-collapse-chain（跨 skill 诱饵） |
| edge-01 | edge_case | 通过 | 黑天鹅后“必然”预测→重新评估信息充分性，必要时降级为结构区间（E 判停） |

**结论**: 接受。
