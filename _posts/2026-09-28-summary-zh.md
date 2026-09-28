---
layout: default
title: "Horizon Summary: 2026-09-28 (ZH)"
date: 2026-09-28
lang: zh
---

> 从 62 条内容中筛选出 3 条重要资讯。

---

**科技新闻**
1. [Simon Willison 主题演讲：2026 年大模型进展盘点](#item-tech-news-1) ⭐️ 8.0/10
2. [Fireworks AI 发布 Ember-1，首次公开自研模型](#item-tech-news-2) ⭐️ 7.0/10
3. [SemiAnalysis 测算：中国数据中心容量达 24GW，三大巨头现金流转负](#item-tech-news-3) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Simon Willison 主题演讲：2026 年大模型进展盘点](https://simonwillison.net/2026/Sep/27/2026-in-llms-so-far/) ⭐️ 8.0/10

Simon Willison 于 2026 年 9 月 25 日在圣何塞举办的 WeAreDevelopers World Congress North America 上发表闭幕主题演讲，按时间线梳理了 2026 年至今大模型领域的关键进展；演讲视频已发布在 YouTube，其博客提供了带注释的幻灯片和配套笔记。他把 2026 年的叙事起点设在 2025 年 11 月：Claude Opus 4.5 与 GPT-5.1 发布后，这两款模型与各自的编程代理框架（Claude Code 与 Codex）搭配使用，表现从“经常出错”跨入了“可靠到可以日常使用”的阶段。演讲还提到 2025 年 11 月 24 日首次提交的 GitHub 仓库 Warelay，并介绍了作者自己 2026 年的新年计划——从往年的“少接新项目、保持专注”反转为“更大胆、想接多少新项目就接多少”。他此前在 Oxide and Friends 播客中给出的年度预测包括“LLM 能写好代码将变得无可争议”“沙箱问题将最终得到解决”以及“编程代理安全可能出现挑战者号式的灾难”。

rss · Simon Willison · 9月27日 23:54

**「背景」** 编程代理本身并不新鲜：Claude Code 早在 2025 年 2 月就已推出，Codex 稍晚一些，但在 2025 年 11 月之前，这类工具&quot;经常出错&quot;。转折点出现在 2025 年 11 月 Claude Opus 4.5 与 GPT-5.1 发布之后——新模型与各自编程代理配合时，从&quot;经常出错&quot;提升到&quot;可靠到可日常使用&quot;，这也是演讲者把 2026 年的起点定在 2025 年 11 月的原因。至于演讲中埋下伏笔的 GitHub 仓库 steipete/Warelay（2025 年 11 月 24 日首次提交），检索到的 steipete/clawdis 仓库页面与发布说明显示，这是开发者 steipete 的一个个人 AI 助手项目，可通过 WhatsApp、Telegram 或网页进行对话，其代理运行时支持 Claude、Pi、Codex、Opencode 等可插拔后端切换，发布说明中也直接以 warelay 指代代理运行流程。

**「对开发者的影响」** 已将 Claude Code、Codex 等编码代理纳入日常工作的开发者，可借助这份免费公开的 YouTube 视频与注释幻灯片核对自己工具链所处的阶段：资料把 2025 年 11 月发布的 Claude Opus 4.5 与 GPT-5.1 定位为编码代理从“经常出错”变为“可靠到可日常使用”的转折点。幻灯片中列出的 2026 年预测还包括“最终解决沙箱问题”以及编码代理安全可能出现“挑战者号灾难”式事故，提示团队在扩大代理使用范围时应把沙箱与安全隔离当作前提条件；不过源内容在预测部分被截断，各项预测是否应验无法据此确认。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/steipete/clawdis/releases">Releases · steipete/clawdis</a></li>
<li><a href="https://github.com/steipete/clawdis">GitHub - steipete/clawdis: Your own personal AI assistant. Talk via WhatsApp, Telegram or Web.</a></li>
<li><a href="https://simonwillison.net/2026/Sep/27/2026-in-llms-so-far/">2026 in LLMs (so far)</a></li>
<li><a href="https://simonwillison.net/2026/Sep/27/">Archive for Sunday, 27th September 2026 | Simon Willison ’s Weblog</a></li>

</ul>
</details>

**标签**: `#llms`, `#artificial-intelligence`, `#keynote`, `#ai-trends`, `#generative-ai`

---

<a id="item-tech-news-2"></a>
### [Fireworks AI 发布 Ember-1，首次公开自研模型](https://fireworks.ai/blog/ember-1) ⭐️ 7.0/10

推理服务商 Fireworks AI 在其官方博客（fireworks.ai/blog/ember-1）发布了 Ember-1；据 Hacker News 评论区反映，这是这家长期以托管第三方开放权重模型为主的公司首次公开涉足自研模型研发。本次提供的材料不含博客正文，因此 Ember-1 的参数规模、基准成绩、许可证条款与开放程度均无法核实，评论者对其“是否算开放模型”也存在分歧。该消息在 Hacker News 上引发了大量讨论，获得 348 点与 179 条评论。

hackernews · gmays · 9月27日 17:31 · [社区讨论](https://news.ycombinator.com/item?id=49868830)

**「背景」** Fireworks AI 此前主要以推理服务商的身份为人所知，其核心业务是托管并提供第三方开源权重模型的 API 服务，而非训练自己的模型，这也是 Ember-1 被视为该公司首次公开已知的模型研发尝试的背景。理解这次发布的另一个前提是其技术底座：Ember-1 并非从零训练的模型，而是对开放权重模型 Kimi K3 进行后训练的产物，K3 此前以 3/15 美元的按 token 计费 API 费率对外提供，而 Ember-1 沿用了完全相同的定价。

**「对 Fireworks 托管客户的影响」** 对把 Fireworks 当作中立推理服务商的用户而言，Ember-1 带来的是具体的信任与选型影响：有用户在讨论中表示，这是他首次得知 Fireworks 拥有自有模型研究团队，因而对继续通过其 API 使用 DeepSeek v4 flash 等第三方开源模型产生了利益冲突方面的担忧，即推理服务商可能同时与自己所托管的开源模型形成竞争。受影响的团队可向 Fireworks 求证自有模型与第三方托管模型之间在资源调度和数据隔离上的保障措施，或在必要时把部分流量分散到 Together AI、Baseten 等同样争夺企业推理业务的竞争平台。

**「社区讨论」** 评论者 tukHelix 表示心情复杂：一方面欢迎开放模型在智能与成本效率上的进步，另一方面担心 Fireworks 在托管 DeepSeek 等第三方模型的同时推出自研模型会带来利益冲突，并称自己此前正通过 Fireworks 使用 DeepSeek v4 flash；tangled 也质疑，一家以跨云调度和批量采购议价为核心价值的推理聚合商转做自研模型意味着什么。另有 jamienk 以 Linux 与 Wikipedia 为例提出开放模型可能借此快速追赶专有模型（属个人观点），netvarun 则在题外话中比较定价，称内部测试中 Sol 质量更好且更便宜（报价为 2/10，而 Kimi K3 为 3/15）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.explainx.ai/blog/fireworks-ember-1-kimi-k3-reasoning-tokens-2026">Ember-1: 71% Fewer Reasoning Tokens at K3 Price (2026 ...</a></li>
<li><a href="https://fireworks.ai/models/fireworks/ember-1">Ember-1 API &amp; Playground | Fireworks AI</a></li>
<li><a href="https://beckmann.ai/en/ai-economy/2026-07/fireworks-ai-series-d-valuation">Fireworks AI reaches a valuation of 17.5 billion dollars · Beckmann</a></li>

</ul>
</details>

**标签**: `#AI models`, `#open source`, `#LLM inference`, `#Fireworks AI`, `#machine learning`

---

<a id="item-tech-news-3"></a>
### [SemiAnalysis 测算：中国数据中心容量达 24GW，三大巨头现金流转负](https://newsletter.semianalysis.com/p/the-chinese-ai-infrastructure-boom) ⭐️ 7.0/10

SemiAnalysis 最新模型测算称，中国已交付数据中心容量达 24GW，覆盖 60 余家运营商、1000 多个设施，规模已超过 EMEA 与亚太其他地区总和；该数字经 Telegram 频道转述，属研究机构估算结果，尚无独立核实。据其测算，字节跳动独家锁定全国近 20% 的交付容量，并在核心节点创下“12 个月落地 100MW”的交付纪录。报告还称，阿里、腾讯、百度在 2026 年第二季度合计资本开支升至 200 亿美元、同比翻倍，三家首次同时录得负自由现金流。容量增长的底座来自此前被市场低估的存量零售型机房，这些设施正借助高密度供电与液冷升级被改造为 AI 集群，形成仅次于北美的物理算力池。

telegram · zaihuapd · 9月27日 08:36

**「背景：以 GW 计量的容量与数据来源」** 数据中心行业通常以电力容量（GW）而非机房数量来衡量算力底座规模，因为 AI 集群的主要瓶颈在于供电与散热，而非机架数量。这批数字并非官方统计，而是来自 SemiAnalysis 首次发布的“中国数据中心模型”；其原文同时确认，2026 年第二季度阿里、腾讯、百度合计资本开支达 200 亿美元、同比翻倍，且三家公司有记录以来首次同时录得负自由现金流。

**「算力供给趋紧与巨头现金流承压」** 对需要在中国境内采购算力与托管资源的企业而言，字节跳动锁定约五分之一的全国交付容量意味着可租机房供给趋紧，核心节点的租金与交付周期可能进一步上行，采购方宜提前锁定电力与机柜资源——SemiAnalysis 记录到字节在核心节点实现了 12 个月落地 100MW 的交付速度。这一资本开支激增有外部数据佐证：国家统计局数据显示 2026 年 1-7 月互联网企业设备支出同比增长 81.8%（同期整体固定资产投资下降 6.7%），高盛 2025 年 11 月的报告亦预计中国 AI 数据中心投资将达 700 亿美元量级。对投资者而言，据 SemiAnalysis 测算，阿里、腾讯、百度首次同时录得负自由现金流，表明扩张已超出经营性现金流的承载能力，其后续债券或股权融资动向值得跟踪。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/the-chinese-ai-infrastructure-boom">The Chinese AI Infrastructure Boom: Introducing the SemiAnalysis China Datacenter Model</a></li>
<li><a href="https://newsletter.semianalysis.com/p/the-chinese-ai-infrastructure-boom">The Chinese AI Infrastructure Boom: Introducing the ...</a></li>
<li><a href="https://www.goldmansachs.com/insights/articles/chinas-ai-providers-expected-to-invest-70-billion-dollars-in-data-centers-amid-overseas-expansion">China’s AI Providers Expected to Invest $70 Billion in Data ...</a></li>
<li><a href="https://www.techtimes.com/articles/324735/20260817/china-bought-it-nbs-confirms-818-ai-equipment-surge-broader-investment-falls.htm">China Bought It: NBS Confirms 81.8% AI Equipment Surge as ...</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#data centers`, `#compute capacity`, `#China tech industry`, `#hyperscaler capex`

---