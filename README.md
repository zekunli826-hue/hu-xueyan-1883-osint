# 1883年胡雪岩破产案：OSINT证据链分析

**Case ID:** OSINT-CASE-001  
**Status:** OPEN — 核心机制部分确认，关键“定点政治清算”主张未证实  
**Language:** 中文  
**License:** CC BY-NC-SA 4.0

> 这是一个用于训练情报分析方法的公开来源情报（OSINT）案例。目标不是证明预设结论，而是区分**已证事实、结构性能力、合理推断、竞争性假设与未证实叙事**。

## 研究问题

1883年胡光墉（胡雪岩）破产，究竟应如何理解以下因素之间的关系：

- 1883年上海系统性金融危机；
- 胡氏的生丝库存、信用依赖与流动性风险；
- 李鸿章—盛宣怀等官商网络的制度性信息优势；
- 胡氏破产后的清廷查抄、财政追索和西征借款“旧账”重查；
- 后世广泛传播的“延饷20日”“截留求救电报”等说法是否有一手证据支持。

## Executive Assessment

当前证据较稳健地支持：

**系统性金融危机 + 胡氏经营与流动性脆弱性 → 阜康崩溃 → 官方查抄、追欠与旧账重查进一步放大损失。**

当前公开证据**不足以确认**以下更强主张：

- 邵友濂奉命故意拖延协饷20天；
- “20天”是精确计算的资金攻击窗口；
- 盛宣怀截留胡光墉向左宗棠求救的电报；
- 李鸿章—盛宣怀预先设计了一套以电报、协饷和挤兑为工具的定点破产方案。

因此，本案例采用的当前工作假设是：

> **H3：市场与经营风险触发 + 行政财政机制事后放大。**

“预谋性定点政治打击”保留为待验证假设，而不写入事实层。

## 关键图表

### 1. 权力网络
![Power network](figures/power_network.png)

### 2. 信息网络
![Information network](figures/information_network.png)

### 3. 资金网络
![Funding network](figures/funding_network.png)

### 4. 关键时间线
![Timeline](figures/timeline.png)

## 仓库结构

```text
hu-xueyan-1883-osint/
├── README.md
├── LICENSE.md
├── CITATION.cff
├── .gitignore
├── report/
│   └── full_report_zh.md
├── analysis/
│   ├── methodology.md
│   ├── ach.md
│   └── red_team.md
├── sources/
│   ├── source_register.csv
│   └── archive_targets.md
└── figures/
    ├── power_network.png
    ├── information_network.png
    ├── funding_network.png
    └── timeline.png
```

## 分析纪律

本项目明确区分五个层级：

| 层级 | 含义 | 例子 |
|---|---|---|
| F — Fact | 有可靠材料直接支持 | 1883年上海出现大范围钱庄、商号危机 |
| C — Capability | 行为体具备某种结构性能力 | 盛宣怀在电报与招商局体系中具有信息与组织优势 |
| I — Inference | 基于事实作出的合理推断 | 这种制度位置可能提高其危机期间的信息可见度 |
| H — Hypothesis | 需要继续验证的竞争性解释 | 是否利用信息优势定点打击胡氏 |
| U — Unverified | 流行但缺少可靠一手闭环的叙事 | “截留求救电报”“精准拖延20天” |

**Capability ≠ Action；Sequence ≠ Causation；Access ≠ Use。**

## 主要纠错

相较于最初版本，本仓库作出以下关键修订：

1. 不再声称“政治清算贡献度显著高于市场因素”，因为无法识别历史反事实并量化贡献度。
2. 不再把“李鸿章—盛宣怀掌握电报/招商局资源”直接等同于“实际截报或制造挤兑”。
3. 左宗棠1883年时任两江总督兼南洋通商大臣，不应描述为“远在西北、只能依赖驿路”。
4. 李鸿章1883年9月27日电令盛宣怀整顿招商局，其现有可见材料直接说明的背景是上海市面紧张与招商局债务压力，不能直接推断为“打胡”。
5. 徐润等大商人和大量钱庄同期受创，是评估“单点打击”假说时必须考虑的反证背景。
6. 胡氏破产后户部重新追查已奏销的西征借款“行用补水”等旧账，是目前政治—行政放大机制中较扎实的一组证据。
7. ACH不再用“支持证据条数”简单计票，而是关注证据对不同假设的诊断性。

## 关键公开来源

- 招商局历史博物馆：**《1883年上海金融风潮》**  
  https://1872.cmhk.com/shuyuan/195.html
- 招商局历史博物馆：**《从1885年盛宣怀入主招商局看晚清新式工商企业中的官商关系》**  
  https://1872.cmhk.com/shuyuan/321.html
- 暨南大学历史学系 / 吴烨舟：**《胡光墉破产案中的西征借款“旧账”清查》**  
  https://lsx.jnu.edu.cn/2016/0330/c1984a18138/page.psp
- 湖南省相关公开历史资料：左宗棠1881年出任两江总督兼南洋通商大臣  
  https://www.hnstb.gov.cn/plus/view-287-1.html
- 湖南省纪委监委公开历史资料：阎敬铭1882年任户部尚书并整顿部务  
  https://www.sxfj.gov.cn/jing_cai_zhuan_ti/267e63/10908389.shtml

完整来源登记及证据用途见 [`sources/source_register.csv`](sources/source_register.csv)。

## 下一步 Collection Priorities

最高优先级不是继续搜通俗故事，而是寻找能区分竞争假设的一手材料：

- 1883年9—12月李鸿章—盛宣怀往来函电中是否直接出现“胡光墉/阜康/协饷/上海道”等关键词；
- 邵友濂公牍中是否存在某笔协饷“延缓20日”的明确命令、日期、金额和理由；
- 电报局收发报记录中是否存在胡氏致左宗棠电报被拒发、缓发或扣留的记录；
- 汇丰、怡和等档案中，胡氏债务催收是否有官员干预证据；
- 户部对“行用补水”旧账重新起案的承办、批转与决策链。

## 方法说明

本案例主要采用：

- Timeline reconstruction
- Three-network analysis：资金网 / 信息网 / 权力网
- ACH（Analysis of Competing Hypotheses）
- Source grading
- Red-team review
- Intelligence gaps / collection priorities

详见 [`analysis/methodology.md`](analysis/methodology.md)。

## Disclaimer

本仓库是历史OSINT与情报分析训练项目，不是对任何历史人物动机的最终定性。对存在争议的主张，仓库尽量明确标注证据状态与置信程度。若发现新的原始档案，应优先依据原件更新当前判断。
