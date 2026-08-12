# candidates/principles.md — 阶段 1 候选池（原则提取器）

# coverage-note:
#   执行方式: 串行降级方案（主流程执行，环境 sub-agent 通道不稳定）
#   依据: BOOK_OVERVIEW.md + COS-report.md + work/kwic/{prediction,war,alliance}.md
#        + concept_stats_top.csv + 前一轮对 84 篇的全文统计与精读
#   合并: 同一条原则跨篇出现即合并，source_chapter 保留主要出处

- id: principles-01
  title: 战争打不赢，说啥都没用
  type: principle
  source_chapter: 2026-4-22_原文.txt
  source_quote: |
    "战争打不赢啥都白扯，特别你是大流氓……你战争打不赢，你还想在谈判桌上谈赢了。"
  summary: |
    谈判筹码来自战场结果而非口头声明；军事上露馅的一方在谈判桌上只能胡搅蛮缠。
    判断任何停火/和谈前景时，先看双方战场态势，再看谈判姿态。
  tags: [negotiation, military, realism]

- id: principles-02
  title: 俄罗斯不能败，也不能赢得太顺利
  type: principle
  source_chapter: 2024-2-21 为什么确定两强斗...变成春秋战国时期，多极化就是分封制。.txt
  source_quote: |
    "俄罗斯不输，但不能停……就是互相消耗最好……他们都不赢咱家就赢了。"
  summary: |
    对消耗型博弈设定“双向约束”：不能让盟友/前排崩溃，也不能让一方速胜，
    理想状态是双方长期失血而自己保存实力。这是代理战争管理的核心原则。
  tags: [attrition, proxy-management, strategy]

- id: principles-03
  title: 制裁对付不了有完整工业体系的大国
  type: principle
  source_chapter: 2025-8-8_原文.txt
  source_quote: |
    "实际上老美制裁俄罗斯没有用，啥用没有……核心是欧盟的经济利益有点大。"
  summary: |
    金融制裁对中小国家有效，对拥有完整工业体系、能源自给和替代市场的大国无效，
    还会反噬制裁发起方的经济利益。评估制裁效果先看目标国的工业闭环程度。
  tags: [sanctions, industrial-base, economics]

- id: principles-04
  title: 时间在中国这边，把大变局当马拉松打
  type: principle
  source_chapter: 2026-5-24_原文.txt
  source_quote: |
    "大变局多极化是一场马拉松，这是纯是一种消耗战。但是时间肯定是在咱这边。"
  summary: |
    当己方在工业存量、人口、组织能力占优时，把长期竞争定义为“谁能撑更久”，
    拒绝速决诱惑，不因短期战报调整战略节奏。
  tags: [long-game, patience, structural-advantage]

- id: principles-05
  title: 看不明白就看地图
  type: principle
  source_chapter: 2026-2-25.txt
  source_quote: |
    "我当时就说一句话，看不明白中东局势的直接看地图。"
  summary: |
    解释复杂冲突前先回到地理事实：位置、通道、纵深、邻国矩阵。
    地图能解释的就不需要猜测动机。
  tags: [geography, first-principles, explanation]

- id: principles-06
  title: 别跟新闻节奏，战略要等一等
  type: principle
  source_chapter: 2024-3-3上地图讲解 欧战快要...是。 公知二狗和投降派别吹了_原文.txt
  source_quote: |
    "短期内他们要走缓和，那个别听那个没有用。那是新闻天天报这报那的……战略这个东西你得稍微等一等。"
  summary: |
    新闻是噪音，战略结构才是信号；判断走势不随单条新闻摇摆，
    而按结构性约束和时间表推演。
  tags: [information-filter, noise-reduction, strategy]

- id: principles-07
  title: 核门槛内解决：大国不正面开战，代理人消耗
  type: principle
  source_chapter: 2026-8-10_原文.txt
  source_quote: |
    "有蘑菇，确实这战争打的有点不解渴……现在战争你们就三下五除二就能分出胜负来，这个没啥意思。"
  summary: |
    核武器使大国间全面战争不可行，冲突以代理人、制裁、技术战等低烈度形式进行；
    判断“会不会开战”先问双方是否拥核、是否在核门槛内。
  tags: [nuclear, proxy-war, conflict-spectrum]

- id: principles-08
  title: 被逼到墙角的玩家必然出手
  type: principle
  source_chapter: 2023-12-22_原文.txt
  source_quote: |
    "北约没有理由不下场了，没有了，被逼到墙角了，没办法了。"
  summary: |
    当一方没有退路（不打就失去一切）时，升级是必然事件，而不是可选项；
    预判“敢不敢打”看退路数量，不看狠话。
  tags: [escalation, prediction, pressure]

- id: principles-09
  title: 胜负看工业产能、库存与纵深，不看武器代差
  type: principle
  source_chapter: 2026-3-31 美国思路_原文.txt
  source_quote: |
    "战争真正的玩家最终的实际上还是地面单战，大规模陆军碰陆军这种干消耗战才能决定胜负。"
  summary: |
    评估一场战争的前景，先算双方工业产能、弹药库存、后勤与战略纵深，
    武器先进程度只在高强度消耗开始前有意义。
  tags: [war, industrial-power, attrition]

- id: principles-10
  title: 没有自主工业体系的国家没有抵抗力
  type: principle
  source_chapter: 2026-3-31 美国思路_原文.txt
  source_quote: |
    "中东唯独有一个不是美式的，不是西方的东西，还有自个儿的一个导弹系统工业体系、一个无人机系统的、一个地面系统，所有就一个伊朗。"
  summary: |
    判断一个国家的抗压能力，先看它有没有自主军工与工业体系；
    依赖外部供应者的一方在危机中会被切断命脉。
  tags: [industrial-autonomy, resilience, evaluation]

- id: principles-11
  title: 真正的强者不急着决战
  type: principle
  source_chapter: 2024-1-8_原文.txt
  source_quote: |
    "咱家说实话还是……不着急，这是大战略方针，一定要压轴，压轴就一波把他们推了。"
  summary: |
    谁先沉不住气谁先暴露底牌；从容等待本身就是权力信号。
    评估双方态势时，把“着急”当作对方虚弱与失算的证据。
  tags: [timing, patience, power-signaling]

- id: principles-12
  title: 美国必留战略储备，中东投入有上限
  type: principle
  source_chapter: 2026-3-31 美国思路_原文.txt
  source_quote: |
    "老美得留这个储备，这个储备是国家储备干啥的？太平洋战争了，万一干起来他啥也没有，那不完了吗？"
  summary: |
    霸权国家在次要方向不会倾尽家底，必然保留应对主要对手的储备；
    因此次要战场的投入存在上限，可据此推断其升级意愿与体面退场节点。
  tags: [reserves, rationality, escalation-limit]
