# candidates/counter-examples.md — 阶段 1 候选池（反例/陷阱提取器）

# coverage-note:
#   执行方式: 串行降级方案（主流程执行，环境 sub-agent 通道不稳定）
#   依据: BOOK_OVERVIEW.md + COS-report.md 第 11 节 + work/kwic/{why,hegemony_power}.md
#        + 2026-3-31 美国思路全文 + 前一轮精读

- id: counter-01
  title: 跟新闻节奏的散户式判断
  type: counter-example
  source_chapter: 2024-1-12_原文.txt
  source_quote: |
    "大家很多人现你别听那个现拿新闻凑节目没啥意思……我这是战略输出，不是新闻输出。"
  failure_mode: |
    用单条新闻（某次空袭、某次表态）判断走势，随短期波动反复改判。
  mechanism: |
    新闻天然偏向事件与情绪，遮蔽结构性约束；没有时间尺度的观察者会被噪音牵着走。
  warning_signs:
    - "昨天刚下结论，今天因一条新闻改口"
    - "用'最新消息'替代长期趋势"
    - "关注'谁说了什么'多于'结构允许什么'"
  bound_to:
    - "别听新闻节奏，战略要等一等"
    - "大格局归因法"
  tags: [counter-example, information-noise, short-termism]

- id: counter-02
  title: 投降派/被舆论洗脑的认知
  type: counter-example
  source_chapter: 2024-3-6（3） 四小龙是站在 咱家功劳簿上起来的。 给小政客塞点钱就卖国_原文.txt
  source_quote: |
    "菲律宾就是这样的……给小政客塞点钱就卖国。"
  failure_mode: |
    因对方话语权强而低估己方实力，或为眼前利益出卖长期国家利益。
  mechanism: |
    舆论长期由强者定义，接受其叙事的人会默认强弱格局不可改变，
    从而在站队时选择“看起来强”的一方。
  warning_signs:
    - "用对方的评价体系衡量自己"
    - "把'谁声音大'当作'谁实力强'"
  bound_to:
    - "站立场分析法"
    - "国力三件套评估"
  tags: [counter-example, propaganda, stance]

- id: counter-03
  title: 以为轰炸/空袭能解决问题
  type: counter-example
  source_chapter: 2026-3-31 美国思路_原文.txt
  source_quote: |
    "大小霸权很迷信这种轰炸……遇到伊朗这种硬茬的，一个多月了，啥也没解决，还被反打。"
  failure_mode: |
    高估空中优势，低估地面消耗战与对方凝聚力，以为摧毁设施即可屈人之兵。
  mechanism: |
    空袭解决不了“对方选择继续打”的问题；当对方有工业自持力与民众韧性时，
    轰炸只会强化其团结。
  warning_signs:
    - "战报显示'摧毁多少目标'但没有政治成果"
    - "认为技术代差=必胜"
  bound_to:
    - "胜负看工业产能、库存与纵深"
    - "战争形态决定胜负手"
  tags: [counter-example, airpower, attrition]

- id: counter-04
  title: 以为制裁能击垮大国经济
  type: counter-example
  source_chapter: 2025-8-8_原文.txt
  source_quote: |
    "老美制裁俄罗斯没有用，啥用没有……他只能玩这个，因为别的没有。"
  failure_mode: |
    把金融制裁当万能武器，忽略目标国的工业闭环、替代市场与伙伴支撑。
  mechanism: |
    制裁依赖对方对美元体系的依赖度；体系完整的大国可转向本币结算与替代供应链。
  warning_signs:
    - "只算制裁数量，不算目标国替代能力"
    - "认为'制裁即胜利'而忽视战争/地缘成本"
  bound_to:
    - "制裁对付不了有完整工业体系的大国"
    - "霸权串行结构"
  tags: [counter-example, sanctions, economics]

- id: counter-05
  title: 低估伊朗的决心
  type: counter-example
  source_chapter: 2026-3-25_原文.txt
  source_quote: |
    "很多人还在低估伊朗的决心，就是跟老美能打到什么程度。"
  failure_mode: |
    按对方国力强弱直接推出“必败”，忽略政权存亡关头的战斗意志与持久战能力。
  mechanism: |
    防御方为政权存续而战，进攻方为可选项而战；动机不对称会抵消部分实力差。
  warning_signs:
    - "只比较GDP/军费就判胜负"
    - "忽略'没有退路'一方的动员能力"
  bound_to:
    - "被逼到墙角的玩家必然出手"
    - "胜负看工业产能、库存与纵深"
  tags: [counter-example, motivation, asymmetry]

- id: counter-06
  title: 以为技术/代差决定一切
  type: counter-example
  source_chapter: 2024-3-5（8） 教员打下的基础_原文.txt
  source_quote: |
    "你没有工业，给你图纸，啥都给你，你给我噪音……光玩制造业，资本想收割他的时候，一波就给他带走了。"
  failure_mode: |
    把专利、图纸、单点技术当实力，忽略承接技术的工业体系与组织基础。
  mechanism: |
    技术必须由工业体系承载；没有地基的技术会被封锁、收割或无法量产。
  warning_signs:
    - "用'某项技术领先'替代'体系完整'"
    - "忽视电力、供应链、工程化能力"
  bound_to:
    - "国力三件套评估"
    - "工业体系是国家实力地基"
  tags: [counter-example, technology, industrial-base]

- id: counter-07
  title: 机会主义/投机心态
  type: counter-example
  source_chapter: 2026-3-18_原文.txt
  source_quote: |
    "谁这个能挺住，那个能挺住，完了最后你就赢了。没有那一说，你那才叫机会主义，投机分子。"
  failure_mode: |
    把胜负寄托于“对方先崩”的侥幸，而不建立自己的战略支撑点。
  mechanism: |
    投机者没有可重复的方法，一旦预期时间点落空即失去判断力；
    战略的本质是准备好条件，而不是赌时点。
  warning_signs:
    - "结论依赖单一时间点"
    - "没有'如果没发生怎么办'的预案"
  bound_to:
    - "结构必然性预测法"
    - "马拉松时间观"
  tags: [counter-example, opportunism, strategy]

- id: counter-08
  title: 必然性话语与不可证伪预测（作者自身盲区）
  type: counter-example
  source_chapter: 2023-12-22_原文.txt
  source_quote: |
    "北约下场之日，就是击穿整个西方军事神话之日……这就是大变局。"
  failure_mode: |
    用“必然/铁定/百分之百”作预测，事件未兑现时顺延或改挂触发条件，而非检验模型。
  mechanism: |
    单变量因果+宏大叙事使预测天然难证伪；反复宣称“我说过”强化自我确认。
  warning_signs:
    - "预测多用必然性词汇"
    - "未兑现时解释为'还没到时间'"
  bound_to:
    - "结构必然性预测法"
    - "所有以必然性为前提的 skill 都需边界"
  tags: [counter-example, overconfidence, falsifiability]

- id: counter-09
  title: 低估美西方制度韧性（作者自身盲区）
  type: counter-example
  source_chapter: 2024-2-15（12） 处在历史当中、苏联解体的原因.txt
  source_quote: |
    "美国分裂是必然的……从地缘角度分析，美国倒塌是必然的。"
  failure_mode: |
    用单条衰落链（去工业化/扩张过度）直接推出“必然崩盘”，
    忽略移民、科技、美元网络、盟友再动员等修复机制。
  mechanism: |
    模型里没有“帝国修复机制”变量，导致提前宣布衰亡时间表。
  warning_signs:
    - "只列衰败证据，不列修复机制"
    - "把'长期趋势'说成'近期必然'"
  bound_to:
    - "霸权串行结构"
    - "结构必然性预测法（需加修复机制权重）"
  tags: [counter-example, resilience, hegemonic-decline]

- id: counter-10
  title: 代理人论过度外推（作者自身盲区）
  type: counter-example
  source_chapter: 2026-2-25.txt
  source_quote: |
    "印度是必然会沦为看门狗的，这个我一直都说的。"
  failure_mode: |
    把所有中小国家行为归因于域外大国控制，低估其自主空间与内部博弈。
  mechanism: |
    “狗链子/看门狗”模板解释力强、省力，但会把小国的主动选择误读为幕后交易。
  warning_signs:
    - "某个小国行为反常时，第一反应是'谁在背后'"
    - "不考察其内部政治与利益结构"
  bound_to:
    - "剧本-演员归因框架"
    - "中美总开关/外溢归因"
  tags: [counter-example, agency, proxy-model]
