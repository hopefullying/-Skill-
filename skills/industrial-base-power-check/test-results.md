# test-results — industrial-base-power-check

- **执行方式**: 主流程自测（fallback）。
- **测试用例**: 6 条（3 should_trigger + 2 should_not_trigger + 1 edge_case，含跨 skill 诱饵）
- **通过率**: 6/6 (100%)

| id | 类型 | 判定 | 说明 |
|---|---|---|---|
| should-trigger-01 | should_trigger | 通过 | “越南替代中国世界工厂”命中制造业转移 |
| should-trigger-02 | should_trigger | 通过 | “制裁俄罗斯有没有用”命中制裁效果 |
| should-trigger-03 | should_trigger | 通过 | 英文 “manufacturing” 命中 |
| should-not-trigger-01 | should_not_trigger | 通过 | 战斗机参数属装备对比，description 排除 |
| should-not-trigger-02 | should_not_trigger | 通过 | “霸权崩溃”应转 hegemony-collapse-chain（跨 skill 诱饵） |
| edge-01 | edge_case | 通过 | 新加坡金融中心→说明地基定义偏离（E 判停说明） |

**结论**: 接受。
