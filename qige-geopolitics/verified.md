# verified.md — 阶段 1.5 三重验证通过单元

> 规则: V1 跨域（≥2 个独立语境佐证）/ V2 预测力（能回答书中未明说的新问题）/ V3 独特性（非常识）。
> 通过 8 个单元，将进入阶段 2 构造独立 skill；其余候选见 rejected/。

- id: v01 (合并 frameworks-05/13/20, principles-05, cases-08/09)
  title: 地图优先的地理分析（含十字路口/通道史观）
  type: framework
  V1_cross_domain:
    passed: true
    evidence:
      - 2026-2-25: 看地图解释中东/伊朗
      - 2026-3-14: 伊朗=十字路口→美国必打
      - 2024-2-15-12: 出海口封死解释苏联败亡
      - 2026-3-21: 位置即命运（换谁坐那儿都一样）
  V2_predictive_power:
    passed: true
    novel_question: "一个从未被讨论过的内陆国（如中亚某国）发生政权更迭，会怎么发展？"
    derived_answer: "先定位它卡在哪条通道/哪块缓冲带，再推断域外大国（中美俄）谁最需要控制它，继而预测外部干预与内部更迭的走向——这是地理决定论的外推。"
  V3_exclusivity:
    passed: true
    why_not_common: "常识是'地理重要'；这里是可执行的判定流程（画连接区域→找咽喉→推宿敌），且含'位置即命运、换谁坐都一样'的反直觉断言。"
  → 进入阶段 2 作为 skill: map-first-geostrategy

- id: v02 (frameworks-03/12, principles-01 部分, cases-13)
  title: 中美总开关/大格局归因
  type: framework
  V1_cross_domain:
    passed: true
    evidence:
      - 2024-1-14: 所有热战/去美元都是中美矛盾外溢
      - 2024-1-8: 半岛博弈实为中美探底牌
      - 2026-2-25: 伊朗问题本质还是中美世界博弈
      - 2026-4-7: 小岛不是军事问题，主要矛盾是美国
  V2_predictive_power:
    passed: true
    novel_question: "某非洲小国突发军事政变，新闻只说国内原因，怎么预判后续？"
    derived_answer: "先问'该国内乱会改变中美在非洲的某条供应链/通道格局吗'，再预测域外大国会站队或默许——这是单变量归因的可复制用法（同时也提示其盲区）。"
  V3_exclusivity:
    passed: true
    why_not_common: "把'一切区域事件都是大国博弈投影'当成第一解释，是强立场方法论；反常识在于'地区内生因素权重趋零'。"
  → 进入阶段 2 作为 skill: great-power-master-switch

- id: v03 (frameworks-06/10, principles-09/10, cases-01/06/11)
  title: 工业体系国力评估
  type: framework
  V1_cross_domain:
    passed: true
    evidence:
      - 2024-3-8: 工业+体格+纵深
      - 2024-3-5-8: 没有工业给图纸也没用
      - 2026-3-7: 电力/工业/供应链是地基，老美是空的
      - 2026-3-31: 中东只有伊朗有自主工业体系
  V2_predictive_power:
    passed: true
    novel_question: "评估某新兴国家'制造业转移'前景，该看什么？"
    derived_answer: "不看工资与订单，看电力、重工业存量、工程师供给、供应链完整度与动员制度；缺地基的转移会被收割（越南/印度案例外推）。"
  V3_exclusivity:
    passed: true
    why_not_common: "反直觉排序：科技/金融/航母是上层结果，工业体系才是根基；'给你图纸也造不出来'是有攻击性的判断标准。"
  → 进入阶段 2 作为 skill: industrial-base-power-check

- id: v04 (frameworks-07/14/19, principles-12, cases-03/05/10)
  title: 霸权串行链与纸老虎验证
  type: framework
  V1_cross_domain:
    passed: true
    evidence:
      - 2023-12-22: 根基是军事→美元→资本
      - 2026-3-22: 美元硬是因为武力值确定性
      - 2026-5-2: 军事霸权瓦解=全部瓦解
      - 2026-3-31: 老美必留战略储备（升级上限）
  V2_predictive_power:
    passed: true
    novel_question: "某域外大国在次要战场被打脸但没输，如何判断其霸权是否受损？"
    derived_answer: "不看成败，看威慑是否兑现：若挑衅者未被惩罚、盟友开始观望，则承重环已松动，美元与资本链将随后承压。"
  V3_exclusivity:
    passed: true
    why_not_common: "把霸权拆成'军事→美元→资本'串行链并给出承重实验（威慑兑现测试），是独特且可操作的模型。"
  → 进入阶段 2 作为 skill: hegemony-collapse-chain

- id: v05 (frameworks-10/11/18, principles-02, cases-15 部分)
  title: 代理人战争与成本账
  type: framework
  V1_cross_domain:
    passed: true
    evidence:
      - 2024-2-15-9: 组织形态战争/不宣战消耗
      - 2026-4-20: 封锁成本由谁买单
      - 2026-3-31: 美俄代理人战争欧盟买单、美伊直接战争王爷买单
      - 2026-3-7: 统战价值（不可替代前排）
  V2_predictive_power:
    passed: true
    novel_question: "某大国想介入一场内战但不想亲自下场，谁会出钱、谁会出人？"
    derived_answer: "沿'谁利益受损最深→谁买单；谁有不可替代的消耗能力→谁当前排'推演，并预测成本不对称高的一方先动摇。"
  V3_exclusivity:
    passed: true
    why_not_common: "代理战争是常识，但'成本账谁买单+统战价值评估+组织形态战争'的组合判定流程不是。"
  → 进入阶段 2 作为 skill: proxy-war-cost-trace

- id: v06 (frameworks-08/09/16/17, principles-04/11)
  title: 消耗战与马拉松时间观
  type: framework
  V1_cross_domain:
    passed: true
    evidence:
      - 2024-2-21: 互相消耗最好，他们都不赢咱家就赢
      - 2024-2-2-4: 小火慢炖放血
      - 2024-1-8: 不着急、压轴后发
      - 2026-5-24: 大变局是马拉松，时间在咱这边
  V2_predictive_power:
    passed: true
    novel_question: "两家公司打价格战，一家资本雄厚一家现金流差，怎么预判策略？"
    derived_answer: "按'谁更能熬'定胜负：强者应控节奏拖长战，弱者应赌窗口速决；先急的一方暴露底牌。"
  V3_exclusivity:
    passed: true
    why_not_common: "常识是'要坚持'；这里是可操作的胜负定义（不赢即赢）与节奏控制规则（强者慢、弱者赌）。"
  → 进入阶段 2 作为 skill: attrition-long-game

- id: v07 (frameworks-21/15, principles-08, cases-05/08/10/12)
  title: 结构必然性预测
  type: framework
  V1_cross_domain:
    passed: true
    evidence:
      - 2023-12-22: 北约被逼到墙角必然下场
      - 2026-3-7: 有开战权没有结束权
      - 2026-2-25: 日本黑化暴走是必然结果
      - 2026-4-8: 内塔尼亚胡必然被清算
  V2_predictive_power:
    passed: true
    novel_question: "某在位者面临'打了必输、不打必被清算'的困局，会做什么？"
    derived_answer: "结构上必然升级搏一把（破罐子破摔），同时提前铺退路/找替罪羊；可用'退路数量'预判其是否真动手。"
  V3_exclusivity:
    passed: true
    why_not_common: "'必然性'预测不是常识性谨慎预测，而是高置信度结构推演；其独特性在于给出'没有退路=必然出手'的可检验判据。"
  → 进入阶段 2 作为 skill: structural-necessity-forecast

- id: v08 (本项目元方法；由用户提示词方法论在 84 篇语料上验证)
  title: 从政治文本反向建模认知操作系统
  type: framework
  V1_cross_domain:
    passed: true
    evidence:
      - 84 篇跨主题重复模式（概念统计+KWIC 证据）
      - 预测句/因果句/定义句三类句式全库抽取
      - 不同国家（美/俄/欧/日/印/伊）用相似分析逻辑
      - 反事实与认知盲区可独立验证
  V2_predictive_power:
    passed: true
    novel_question: "给另一位主播的全新语料，如何快速重建其认知系统？"
    derived_answer: "清洗→概念频次跨文本统计→关键句式上下文抽取→代表文本精读→重复模式归纳→盲区校验，即可产出可外推的认知操作系统说明书。"
  V3_exclusivity:
    passed: true
    why_not_common: "总结'他说了什么'是常识；'从大量表达中重建他如何观察/归因/预测的规则系统'是反直觉的元方法（观点→规则）。"
  → 进入阶段 2 作为 skill: cos-reverse-modeling

## 汇总

- 通过: 8 个 → 进入阶段 2
- 淘汰: 见 rejected/（含 frameworks-01/02/04/18/22 及 principles-03/06/07/10 等未独立成 skill 的候选；部分并入上述 8 个 skill）
