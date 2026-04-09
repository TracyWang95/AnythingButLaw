<div align="center">

# 法外功夫 AnythingButLaw.skill

> *法学院教你法律，但客户的问题从来不只是法律。*

[![MIT License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Claude Code](https://img.shields.io/badge/Claude_Code-skill-blueviolet.svg)](https://docs.anthropic.com/en/docs/claude-code)
[![AgentSkills](https://img.shields.io/badge/AgentSkills-standard-orange.svg)](https://github.com/anthropics/claude-code)

<br>

客户问你和解方案的净现值是多少。<br>
对方律师在歧视案中扔出一份回归分析。<br>
尽调中 CFO 的数字对不上，但你说不出哪里不对。<br>
合同条款看着没问题，但激励机制全是坑。<br>

**这些不是法律问题。这些才是律师真正面对的问题。**

**法外功夫** 将九大商业分析框架蒸馏成一个 AI 技能，赋予律师法学院从未教过的非法律超能力。

[知识域](#九大知识域) · [安装](#安装) · [使用](#使用方法) · [示例](#示例) · [为什么做这个](#为什么做这个)

[English](README.md)

</div>

---

## 它能做什么

法外功夫为 Claude 装备了 **9 大分析框架**，覆盖现代法律实务的核心非法律需求：

- **构建决策树** 用于和解谈判，包含期望值、敏感性分析和交叉点计算
- **运用博弈论** 识别谈判中的道德风险、逆向选择、可信威胁与空洞威胁
- **设计合同** 分析 6 种合同类型的激励对齐、风险分配和可验证性
- **解读财务报表** 在尽调中发现红旗信号（收入确认操纵、现金流与利润的背离）
- **计算现值、DCF 和 CAPM** 用于损害赔偿量化和企业估值
- **分析市场** 运用供需、弹性、剩余和垄断框架支持反垄断工作
- **运用法经济学** 评估违约救济、和解vs审判决策、最优制裁力度
- **评估统计证据** 包括假设检验、置信区间和 Daubert 标准
- **挑战回归分析** 在歧视案件中识别遗漏变量偏误、多重共线性和双向因果

## 九大知识域

| # | 域 | 参考文件 | 律师核心场景 |
|---|---|---------|------------|
| 1 | 决策分析 | `decision-analysis.md` | 诉讼策略、和解、风险规避、敏感性分析 |
| 2 | 博弈论与信息 | `game-theory.md` | 谈判策略、道德风险、逆向选择、囚徒困境 |
| 3 | 合同设计 | `contracting.md` | 合同结构、激励机制、风险分配、违约条款 |
| 4 | 会计 | `accounting.md` | 三大报表、尽调、财务舞弊识别 |
| 5 | 金融 | `finance.md` | 现值、DCF、CAPM、企业估值、损害赔偿 |
| 6 | 微观经济学 | `microeconomics.md` | 反垄断、市场失灵、外部性、科斯定理 |
| 7 | 法经济学 | `economic-analysis.md` | 违约赔偿、和解分析、刑罚经济学 |
| 8 | 统计分析 | `statistics.md` | 假设检验、Daubert 标准、置信区间 |
| 9 | 多元统计 | `multivariate-statistics.md` | 歧视诉讼回归分析、遗漏变量偏误 |

## 安装

### Claude Code（推荐）

```bash
git clone https://github.com/TracyWang95/AnythingButLaw.git ~/.claude/skills/AnythingButLaw
```

详见 [INSTALL.md](INSTALL.md)。

## 使用方法

安装后，当你向 Claude 提出涉及以下场景的问题时，技能会自动触发：

- 和解谈判与诉讼策略
- 合同起草与激励设计
- 财务报表分析与尽调
- 企业估值与损害赔偿计算
- 市场分析与反垄断
- 统计证据评估
- 歧视案件中的回归分析

### 示例提问

```
"客户收到110万和解要求。原告责任认定概率50%，可能赔偿100万，
但有10%概率判2500万惩罚性赔偿。该不该接受和解？"

"我们在谈一个服务合同——固定费用还是成本加成。各自的激励问题是什么？"

"对方提交了一份回归分析，控制学历和工龄后声称性别系数不显著。怎么挑战这个分析？"
```

## 示例

详见 [`examples/`](examples/) 目录中的完整分析案例。

## 为什么做这个

法学院培养出来的毕业生能解析法条、撰写案件摘要，但一看到 Excel 就慌。法律实务要求的决策分析、博弈论、会计、金融、经济学和统计学，法学院从来不教。

**法外功夫** 把这些律师必备的非法律技能蒸馏成一个 Claude Code 技能，让每个律师身边都有一个懂商业的分析师。

名字说明一切：**Anything But Law** — 律师能学到的最有价值的东西，恰恰是法律之外的一切。

## 评测结果

| 指标 | 有技能 | 基线 | 差异 |
|------|--------|------|------|
| **通过率** | **100%** | 73.3% | +26.7% |
| Tokens | 23,968 | 14,451 | +66% |
| 时间 | 117s | 79.8s | +47% |

## 致谢

- **灵感来源**：[colleague.skill](https://github.com/titanwings/colleague-skill) by @titanwings
- **驱动力**：Claude Code + AgentSkills standard

## 许可证

[MIT](LICENSE)
