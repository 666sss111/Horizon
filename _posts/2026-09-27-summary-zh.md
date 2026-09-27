---
layout: default
title: "Horizon Summary: 2026-09-27 (ZH)"
date: 2026-09-27
lang: zh
---

> 从 58 条内容中筛选出 2 条重要资讯。

---

**科技新闻**
1. [美国上诉法院维持五角大楼将 Anthropic 列入黑名单](#item-tech-news-1) ⭐️ 7.0/10
2. [Excel 预览版首次支持一个单元格存放多个值](#item-tech-news-2) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [美国上诉法院维持五角大楼将 Anthropic 列入黑名单](https://www.reuters.com/world/us-appeals-court-declines-block-pentagons-blacklisting-anthropic-2026-09-25/) ⭐️ 7.0/10

9 月 25 日，美国华盛顿特区联邦上诉法院以 2 比 1 的表决，维持五角大楼将 Anthropic 列为国家安全供应链风险、禁止其参与军事合同的决定，多数法官认为 Anthropic 拒绝允许其产品用于自主武器和大规模监控，五角大楼的担忧具有合理性。Anthropic 表示不认同该裁决，正考虑请求全体上诉法院法官复审。此前旧金山一名联邦法官曾依据另一部法律推翻相关列名，并阻止政府对 Anthropic 实施更广泛的禁令，因此两级法院目前结论对立，诉讼尚未结束，列名的法律效力仍存争议。

telegram · zaihuapd · 9月26日 05:19

**「争议缘起」** 争端源于五角大楼 2026 年 3 月将 Anthropic 列为国家安全供应链风险的决定：该列名取消了这家 AI 公司当时持有的军事合同，并禁止其他五角大楼承包商使用其技术。列名针对的正是 Anthropic 拒绝允许其 AI 用于自主武器和大规模监控的使用限制；据媒体报道，这一政府行动由特朗普政府和国防部长皮特·赫格塞斯方面推动，被视作联邦政府与坚持为其技术设置安全护栏的 AI 创业公司之间的对抗。

**「Claude 持续被排除在军事合同之外，收入与采购承压」** 随着上诉法院以 2 比 1 维持列名，Claude 模型将继续被排除在美军合同和系统之外（tool-3-2）；据 Reuters 报道，Anthropic 高管此前曾估计该列名可能使公司 2026 年收入减少数十亿美元，这一风险现在因禁令得以维持而更可能成为现实（tool-3-3）。依赖 Claude 参与国防项目的承包商和政府用户需转向其他 AI 供应商或调整采购安排；Anthropic 表示不同意裁决，正考虑请求全体上诉法院复审，后续诉讼结果仍可能改变禁令状态。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.straitstimes.com/world/united-states/us-appeals-court-upholds-pentagons-blacklisting-of-ai-startup-anthropic">US appeals court upholds Pentagon blacklist of AI startup Anthropic</a></li>
<li><a href="https://ijr.com/discover/tech-2026-09-25-appeals-court-backs-pentagon-anthropic-blacklist-735e00e0">Appeals Court Upholds Pentagon Exclusion of Anthropic From...</a></li>
<li><a href="https://www.linkedin.com/news/story/anthropic-loses-blacklisting-battle-with-federal-government-7626044/">Anthropic loses blacklisting battle with federal government | LinkedIn</a></li>
<li><a href="https://www.facebook.com/AriseTVNews/posts/a-us-appeals-court-rules-the-pentagon-can-blacklist-anthropic-keeping-its-claude/1691070589691473/">A US appeals court rules the Pentagon can blacklist Anthropic ...</a></li>
<li><a href="https://www.reuters.com/world/how-anthropic-pentagon-dispute-over-ai-safeguards-escalated-2026-09-25/">Anthropic&#x27;s Pentagon blacklist upheld in US appeals court - Reuters</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#AI safety`, `#military AI`, `#defense procurement`, `#Anthropic`

---

<a id="item-tech-news-2"></a>
### [Excel 预览版首次支持一个单元格存放多个值](https://techcommunity.microsoft.com/blog/microsoft365insiderblog/put-multiple-values-in-one-cell-with-lists-and-arrays-in-excel/4559395) ⭐️ 7.0/10

微软正在 Excel 中以预览形式推出列表与单元格内数组，首次允许在一个单元格中存放多个值，目前已面向 Windows 和 Mac 的 Beta 通道用户开放。用户可通过 Ctrl+J 快捷键或「插入 &gt; 列表」入口写入以逗号或分号分隔的多个项目，并能针对其中的单个项目进行筛选与计算。配套新增的 FLATTEN、HAS、HASANY、HASALL 四个函数用于处理这类数组数据。微软强调这些均为预览功能，正式发布前行为可能调整，建议暂不用于重要工作簿。

telegram · zaihuapd · 9月26日 16:26

**「背景：Excel 长期以来的“一单元格一值”模型」** 在此次更新之前，Excel 数十年来一直遵循“一个单元格只存放一个值”的基本数据模型：即便用户把多个项目用逗号写进同一单元格，Excel 也只会将其视为一段普通文本，无法按其中的单个项目进行筛选或计算。此前引入的动态数组功能虽然让公式能够一次返回多个结果，但这些结果仍必须“溢出”到相邻的多个单元格中逐一显示，每个单元格本身依旧各自只持有一个值。

**「使用建议」** 该功能目前仅面向 Windows 和 Mac 的 Beta 通道，且属于行为可能随时调整的预览特性，微软明确建议不要在重要工作簿中使用；依赖 Excel 处理关键数据的团队应等待功能正式发布后再评估采用，届时按单项筛选与计算的写法可能需要配合 FLATTEN、HAS 等新函数。

**标签**: `#Excel`, `#Microsoft 365`, `#spreadsheets`, `#arrays`, `#preview features`

---