# candidates/cases.md — 阶段 1 候选池（案例提取器）

# coverage-note:
#   执行方式: 串行降级方案（主流程执行，环境 sub-agent 通道不稳定）
#   依据: BOOK_OVERVIEW.md + COS-report.md + work/kwic/{geography,china_model}.md
#        + 2026-6-10 与 2024-2-15-12 全文 + 前一轮精读

- id: cases-01
  title: 朝鲜战争＝立国之战
  type: case
  source_chapter: 2026-5-7_原文.txt
  source_quote: |
    "咱家是不靠战争，不靠掠夺，但是这句话不对，咱家是靠战争打出来的。
     朝鲜战争的立国之战才有重重工业体系这一系列的东西。"
  summary: |
    用朝鲜战争解释中国工业体系与两弹一星的起源：一场“立威之战”换来
    安全环境与工业化前提。案例绑定“立威之战”与“工业地基”两个方法论。
  bound_to:
    - "立威之战/以战立国"
    - "工业体系是国家实力地基"
  outcome: |
    战后中国获得长期和平窗口，重工业体系逐步建立（作者观点）。
  tags: [case, war, industrial-base]

- id: cases-02
  title: 苏联败亡的“通道封死”解释
  type: case
  source_chapter: 2024-2-15（12） 处在历史当中、苏联解体的原因.txt
  source_quote: |
    "苏联从远东旅顺港到釜山港，又到咱们福建，完了又到越南港，
     最后一个到阿富汗南下印度洋，这几个点全被咱家给封死了。"
  summary: |
    把苏联解体重写为结构性失败：出海口与通道被逐点封死，
    而非单纯经济或意识形态崩溃。案例绑定“地缘通道史观”。
  bound_to:
    - "地缘出海口/通道史观"
    - "结构必然性预测法"
  outcome: |
    苏联最终解体，作者用通道封锁链解释其必然性。
  tags: [case, history, chokepoint]

- id: cases-03
  title: 美国最大的战略误判：想让俄罗斯解体
  type: case
  source_chapter: 2024-2-15（12） 处在历史当中、苏联解体的原因.txt
  source_quote: |
    "美国最大的战略误判就是认为他能让苏联解体，也能让俄罗斯解体。
     这个是他的，这属于什么呢？一厢情愿。苏联解体是因为苏联本身是加盟国体系的解体。"
  summary: |
    用“加盟国体系 vs 民族国家”区分苏联与俄罗斯：前者可被拆解，
    后者结构不同，套用同一剧本必然失败。案例绑定“剧本-演员归因框架”的反面用法。
  bound_to:
    - "剧本-演员归因框架（错误套用的代价）"
    - "国家行为由结构决定"
  outcome: |
    俄乌战争持续多年，俄罗斯未解体（作者以此自证判断）。
  tags: [case, us-russia, structural-mismatch]

- id: cases-04
  title: 俄乌战争把单极→多极提前 5-10 年
  type: case
  source_chapter: 2024-2-18.txt
  source_quote: |
    "俄乌的俄罗斯对乌克兰的军事行动……他把单极向多极化的演变至少向前推动了5到10年。"
  summary: |
    用俄乌战争作为“大变局加速器”案例：正面绞杀战暴露北约工业与组织短板，
    比贸易战更能削弱霸权。绑定“战争形态决定胜负手”与“单极→多极过渡”。
  bound_to:
    - "单极→多极过渡叙事"
    - "战争形态决定胜负手"
  outcome: |
    北约未公开下场，作者解释为“预演暴露弱点后的犹豫”。
  tags: [case, ukraine, multipolarity]

- id: cases-05
  title: “北约下场之日就是大变局”预测案例
  type: case
  source_chapter: 2023-12-22_原文.txt
  source_quote: |
    "北约下场之日，就是击穿整个西方军事神话之日，记住七哥这句话，这才是大变局。"
  summary: |
    作者以“北约下场”为大变局的触发器预测；北约未按原时间表下场后，
    触发器被顺延/改挂到“伊朗决战”。案例绑定“结构必然性预测法”，
    也暴露其“必然性话语”的不可证伪倾向。
  bound_to:
    - "结构必然性预测法"
    - "过度自信与确证偏差（反例见 counter-examples）"
  outcome: |
    截至语料末，北约未公开对俄下场；作者将其解释为“被逼到墙角但还没到时候”。
  tags: [case, prediction, verification-bias]

- id: cases-06
  title: 二十年剧本：2001→2010→2013→2016→2018→2022
  type: case
  source_chapter: 2026-6-10十分钟看懂近二十年局.._原文.txt
  source_quote: |
    "2010年咱家正式成为世界第一大制造业大国……2013年丝绸之路战略出炉……2016年南海危机……2018年贸易战。"
  summary: |
    用一串年份把中美博弈叙述为“中国布局—美国接招”的剧本：
    入世、制造第一、一带一路、军改、南海对峙、贸易战、俄乌。
    绑定“剧本-演员归因框架”与“马拉松时间观”。
  bound_to:
    - "剧本-演员归因框架"
    - "马拉松时间观"
  outcome: |
    作者以此解释美国每一个动作都是“被迫接招”，并预判后续剧本（中东→亚太）。
  tags: [case, timeline, us-china]

- id: cases-07
  title: 阿富汗撤军＝最大战略错误（反事实推理）
  type: case
  source_chapter: 2026-3-31 美国思路_原文.txt
  source_quote: |
    "美军不撤阿富汗，俄罗斯不带干的……阿富汗一撤，俄罗斯2022年紧接着开战了。"
  summary: |
    用反事实（如果不撤军则俄不会开战、伊朗不会腹背受敌）解释 2022 年俄乌开战。
    案例绑定“反事实测试”方法论：识别作者认为的真正因果变量。
  bound_to:
    - "反事实测试/真正因果变量识别"
    - "地缘通道（阿富汗钉子）"
  outcome: |
    2022 年俄乌开战，作者视之为该因果链的验证。
  tags: [case, counterfactual, afghanistan]

- id: cases-08
  title: 伊朗＝欧亚十字路口，美国必打
  type: case
  source_chapter: 2026-3-14_原文.txt
  source_quote: |
    "伊朗是欧亚的十字路口……你看地图你们就明白了，这很简单……拿不下老美必输。"
  summary: |
    用地理位置（连接南亚/中亚/西亚/欧洲/波斯湾、高原俯视中东）推出
    “美国不打伊朗等于自杀”。绑定“十字路口位势判定”与“地图优先”。
  bound_to:
    - "十字路口/咽喉位势判定"
    - "地图优先的地理解释法"
  outcome: |
    2026 年美伊开战，作者认为预测兑现。
  tags: [case, iran, geography]

- id: cases-09
  title: 霍尔木兹＝石油美元咽喉
  type: case
  source_chapter: 2026-2-25.txt
  source_quote: |
    "波斯湾霍尔摩斯海峡一天出来的油量占43%，占咱家的将近他妈的40%……就这一个口。"
  summary: |
    以海峡能源流量作为战略权重证据：控制/封锁霍尔木兹直接威胁美元石油体系。
    绑定“成本账/谁买单”与“霸权链承重实验”。
  bound_to:
    - "成本账/谁买单评估"
    - "霸权串行结构（军事→美元→资本）"
  outcome: |
    作者据此预测伊朗必控霍尔木兹、美元霸权被锁喉。
  tags: [case, chokepoint, dollar]

- id: cases-10
  title: 打伊朗＝美国最后一根救命稻草（跨年预测）
  type: case
  source_chapter: 2026-4-27_原文.txt
  source_quote: |
    "我说伊朗是美国最后一根救命稻草，美国打击伊朗收益巨大，但是风险也大，这是我原话。"
  summary: |
    2024 年前后即断言“打伊朗是美国最后一根救命稻草”，2026 年美伊开战后
    视之为验证。绑定“结构性必然性预测法”与“战略困境菜单”。
  bound_to:
    - "结构必然性预测法"
    - "战略困境菜单（先外围后核心）"
  outcome: |
    2026 年美伊冲突爆发，作者据此预测内塔尼亚胡与特朗普政权不稳。
  tags: [case, prediction, iran]

- id: cases-11
  title: 稀土反制＝首次反打美西方工业核心
  type: case
  source_chapter: 2026-2-25.txt
  source_quote: |
    "稀土这一项，我说了是美欧集团自大航海、自美国建国，有史以来的首次在工业体系核心领域被人家反打的。"
  summary: |
    用稀土出口管制作为“产业链武器化”的标志性案例：制造大国用上游材料
    反制技术封锁。绑定“经济从属于政治/产业链武器化”。
  bound_to:
    - "经济从属于政治（产业链武器化）"
    - "工业体系是国家实力地基"
  outcome: |
    作者认为美西方军工与高科技受制，贸易战胜负已分。
  tags: [case, rare-earth, supply-chain]

- id: cases-12
  title: 日本黑化暴走＝霸权跌落前的必然结果
  type: case
  source_chapter: 2026-2-25.txt
  source_quote: |
    "鬼子的暴走黑化是大变局，是美东升西降、美霸权跌落之前的一个必然结果。"
  summary: |
    把日本右翼化解释为美国霸权衰落的系统性后果，而非日本内政；
    并推出“中华民族崛起一定踩着鬼子上来”。绑定“外溢归因”与“亚太终局”。
  bound_to:
    - "中美总开关/外溢归因"
    - "亚太是结局（对日清算）"
  outcome: |
    高市早苗上台，作者视之为“黑化暴走”验证。
  tags: [case, japan, hegemonic-decline]

- id: cases-13
  title: 半岛博弈＝中美探底牌
  type: case
  source_chapter: 2024-1-8_原文.txt
  source_quote: |
    "朝韩这边……我那天说了打不起来，互相扇眼药水，就是互相探底牌，不是他俩，是中美，是中美互相探底牌。"
  summary: |
    用“外溢”框架解释半岛对峙：表面是朝韩，实质是中美在测试红线。
    绑定“大格局归因法/总开关”。
  bound_to:
    - "中美总开关/外溢归因"
    - "大格局归因法（看棋局不看单子）"
  outcome: |
    半岛未爆发大规模冲突，作者认为“探底牌”判断正确。
  tags: [case, korea, proxy]

- id: cases-14
  title: 后美国时代的中东四强平衡
  type: case
  source_chapter: 2024-1-12_原文.txt
  source_quote: |
    "以色列接受两国方案，没有刺头，老美霸权没了。中东四股力量，土耳其、伊朗、沙特、以色列这四股力量必须平衡。"
  summary: |
    用“区域平衡”设计后霸权秩序：中东由四强互制，中国扶持沙特为小工业国。
    绑定“多极化＝区域势力范围”。
  bound_to:
    - "多极化＝区域势力范围（分封制）"
    - "成本账/谁买单评估"
  outcome: |
    作者据此主张“两国方案”是对以色列最有利的结局。
  tags: [case, middle-east, order-design]

- id: cases-15
  title: 特朗普三阶段人性模型
  type: case
  source_chapter: 2026-3-31 美国思路_原文.txt
  source_quote: |
    "特朗普的三个阶段：不自信的时候说大话，恐惧恐慌的时候说胡话，平静下来的时候说实话。"
  summary: |
    用心理三阶段解读特朗普发言：大话→胡话→实话，说明其内部状态与退路铺设。
    绑定“领导人放大论/人性模型”。
  bound_to:
    - "领导人只是放大器（人性模型）"
    - "谁先急谁输（后发制人判据）"
  outcome: |
    特朗普承认可撤出霍尔木兹，作者视之为“平静说真话”阶段信号。
  tags: [case, psychology, leadership]
