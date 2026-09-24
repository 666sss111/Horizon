---
layout: default
title: "Horizon Summary: 2026-09-24 (ZH)"
date: 2026-09-24
lang: zh
---

> 从 84 条内容中筛选出 7 条重要资讯。

---

**科技新闻**
1. [高通宣布骁龙 X2 系列将获得主线 Linux 驱动支持](#item-tech-news-1) ⭐️ 7.0/10
2. [Anthropic 宣称 Claude 发现类 CRISPR 新酶系统，社区称新颖性有限](#item-tech-news-2) ⭐️ 7.0/10
3. [谷歌发布 Gemini 3.8 文本转语音模型，支持 30 秒声音克隆](#item-tech-news-3) ⭐️ 7.0/10
4. [观点文章：模型调用成本或将低于 grep 等本地工具](#item-tech-news-4) ⭐️ 7.0/10
5. [小米开源 MiMo-V2.6：重点不在 1M 上下文，而在长轨迹强化学习](#item-tech-news-5) ⭐️ 7.0/10
6. [LeCun 于 ECCV 2026 演讲称「预测像素」是伪命题，主张以 JEPA 构建世界模型](#item-tech-news-6) ⭐️ 7.0/10
7. [AI 需求推动 HBM 单位面积价值首次超过先进制程逻辑芯片](#item-tech-news-7) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [高通宣布骁龙 X2 系列将获得主线 Linux 驱动支持](https://www.qualcomm.com/news/onq/2026/09/snapdragon-summit-agentic-ai-pcs-linux) ⭐️ 7.0/10

高通在骁龙峰会上宣布，将为骁龙 X2 系列 PC 芯片把核心 Linux 驱动上游化到主线内核，涵盖 Hexagon NPU 和 Adreno GPU，面向开发者与合作伙伴开放。这一承诺目前仍是厂商公告而非已全部落地的能力，但已有独立进展佐证：OpenBSD 开发者 Tobias Heider 提交了首批 OpenBSD/arm64 支持代码，使 HP EliteBook X G2q 在 ACPI 模式下的 USB、键盘和触控板可用；他还演示了 Ubuntu 并确认 ARM EL2 可用，即 KVM 虚拟化，这是前代骁龙 X 平台所不具备的能力。

hackernews · aaronday · 9月23日 22:38 · [社区讨论](https://news.ycombinator.com/item?id=49823582)

**「背景」** 高通上一代骁龙 X Elite 芯片同样曾承诺提供 Linux 支持，但主线上游进展缓慢且覆盖不完整，Linux 用户主要依赖社区自行移植，这也是本次官方支持消息受到关注的前提。与以往不同，高通此次表示将把 Hexagon NPU 和 Adreno GPU 等核心驱动直接上游进 Linux 主线内核，并计划在 2027 年上半年推出 Ubuntu 支持。骁龙 X2 的 Hexagon NPU 也已能通过早期开发者预览在 Linux 中访问，开发者可以直接利用板载硬件测试和运行 AI 工作负载。

**「影响」** 对希望在 Arm 笔记本上运行 Linux 的开发者和用户而言，主线驱动加上 EL2/KVM 支持意味着骁龙 X2 设备有望开箱运行主流发行版并进行虚拟化，而无需依赖厂商私有内核补丁。不过鉴于前代 X Elite 承诺的 Linux 支持进展缓慢且不完整，购买或迁移决策仍应等待驱动实际合入主线、整机适配得到验证之后再做。

**「社区讨论」** 评论者 brynet 提供的 OpenBSD/arm64 早期提交与 Ubuntu、EL2 演示信息，为高通的公告提供了厂商之外的独立佐证；modeless 和 nr378 援引 Geekbench 成绩认为骁龙 X2 性能已接近苹果 M 系列，希望买到预装 Linux 的机型。sharktheone 则回忆前代 X Elite 也曾承诺良好 Linux 支持却未能兑现，因此对此次公告持谨慎乐观而非全盘相信的态度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theverge.com/news/999664/qualcomm-snapdragon-x2-linux-support-arm">Qualcomm will finally support Linux on Snapdragon X2 chips.</a></li>
<li><a href="https://www.xda-developers.com/qualcomm-is-helping-linux-run-better-on-snapdragon-x2-laptops-with-an-early-developer-preview/">Qualcomm is helping Linux run better on Snapdragon X2 laptops with an ...</a></li>

</ul>
</details>

**标签**: `#linux-kernel`, `#qualcomm-snapdragon`, `#arm-laptops`, `#open-source-drivers`, `#npu`

---

<a id="item-tech-news-2"></a>
### [Anthropic 宣称 Claude 发现类 CRISPR 新酶系统，社区称新颖性有限](https://www.anthropic.com/news/claude-discovers-novel-enzyme-system) ⭐️ 7.0/10

Anthropic 于 2026 年 9 月 23 日发布公告，称其 Claude 智能体在梳理一段已知逆转录酶（RT）附近的原始 DNA 序列时，识别出一套此前未描述的类 CRISPR 串联重复阵列及酶系统。公告援引的智能体分析记录显示，它在 RT 旁&quot;肉眼&quot;发现了这一串联重复阵列，并判断其为类 CRISPR 重复结构。需要强调的是，这是 Anthropic 自行发布的厂商结果，目前没有独立验证或同行评审信息；参与讨论的研究者指出，该系统围绕一种已知的类 retron 逆转录酶，核心贡献更接近&quot;已知酶旁的新基因组排布&quot;，而非全新机制。

hackernews · raahelb · 9月23日 18:06 · [社区讨论](https://news.ycombinator.com/item?id=49820134)

**「背景：CRISPR 类系统与逆转录酶」** CRISPR 基因编辑技术源自细菌的免疫系统，其基因组中排列着一列等间距的 DNA 重复序列，用于储存入侵者的序列记录；本次报告的系统在结构上与之相似，但以逆转录酶（RT）为核心——这是一类能把 RNA 反转录拷贝为 DNA 的酶。据 Anthropic 描述，这类 ART 系统通常由三个要素组成：一个逆转录酶、一个配对基因和一列等间距的 DNA 重复序列。作为系统核心的这枚逆转录酶存在于一种巨型噬菌体中，此前的研究已识别过该酶本身，而本次结果的新意在于其旁侧成排的非编码 DNA 序列等此前未被描述的特征。

**「影响」** 对基因编辑和计算生物学领域而言，这一发现的近期实际影响可能有限：评论者指出当前工程化的 Cas9 变体在人类基因组靶向覆盖上已足够高效，基因治疗的主要瓶颈在于递送而非新核酸酶的来源。对关注 AI 智能体科研能力的读者，更可操作的结论是：将公告视为厂商陈述，待独立复现和论文评审后再评估其科学分量。

**「社区讨论」** 在 Hacker News 的 512 条评论中，最有分量的技术批评认为，冷静的表述应是&quot;Claude 在已知类 retron 逆转录酶附近识别出此前未描述的基因组排布&quot;，与&quot;发现新酶系统&quot;的标题存在落差。也有评论者乐于看到公告直接放出智能体原话带来的&quot;发现现场&quot;记录感，另一些人则质疑 Anthropic 刻意渲染&quot;只给高层提示、其余由智能体自行完成&quot;的自主性叙事，或对 LLM 能否真正推理生物化学表示困惑——这些均属个人观点而非已证实的事实。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-discovers-novel-enzyme-system">Claude discovers a novel enzyme system \ Anthropic</a></li>
<li><a href="https://www.econotimes.com/Anthropics-Claude-Discovers-CRISPR-Like-Enzyme-System-1752867">Anthropic’s Claude Discovers CRISPR-Like Enzyme System</a></li>

</ul>
</details>

**标签**: `#ai-agents`, `#machine-learning`, `#computational-biology`, `#genomics`, `#scientific-discovery`

---

<a id="item-tech-news-3"></a>
### [谷歌发布 Gemini 3.8 文本转语音模型，支持 30 秒声音克隆](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-8-text-to-speech/) ⭐️ 7.0/10

谷歌宣布推出 Gemini 3.8 文本转语音模型，主打声音复刻功能：据官方公告描述，仅需 30 秒音频样本即可重建一致的声线，并内置同意验证、SynthID 水印与 C2PA 凭证，官方称这些机制用于保护开发者及其配音演员。该模型面向开发者与服务集成方发布，其“3.8”的小数版本号显示这是 Gemini 系列的又一次增量更新。目前可核实的信息仅限于公告中被引用的片段，该模型在各平台的具体可用范围尚未完整披露。

hackernews · swolpers · 9月23日 15:29 · [社区讨论](https://news.ycombinator.com/item?id=49817615)

**「谷歌对语音克隆的立场转变」** 在此次发布之前，语音克隆能力已由多家其他供应商提供，而 Hacker News 上有评论者回忆，谷歌几年前曾因担心滥用而拒绝发布自家的语音合成模型；该回忆出自评论者个人、未经独立证实，但有人据此认为谷歌是因竞争环境变化而不再犹豫。作为对滥用风险的回应，谷歌此次表示复制声线需通过同意验证，生成的音频将附带 SynthID 水印与 C2PA 内容凭证。

**「对开发者与选型方的实际影响」** 对需要语音克隆能力的开发者而言，Gemini 3.8 并未填补能力空白——商业服务（如 ElevenLabs）早已提供语音克隆，而阿里 Qwen3-TTS 据第三方资料在 2026 年 1 月开源后可免费自托管——其真正的差异点在于内置的同意验证、SynthID 水印与 C2PA 凭证这一整套来源保护机制，对有合规或内容溯源要求的团队可能更具吸引力。实际采用前存在一个兼容性顾虑：有用户报告 Google 在消费级、专业级与云平台三个渠道之间的模型可用性和能力并不一致（例如 Omni Flash 的输出能力在消费/专业端与 GCP 上不同），若组织禁用了消费级与专业级入口，可能在云端拿不到同等功能，因此评估时应逐平台核对该模型的实际可用能力，再决定是否引入。

**「社区讨论」** 评论主要聚焦于政策转向与发布方式两点：simonw 认为声音克隆如今已被其他提供商普遍提供，谷歌因此不再对发布该功能犹豫；sharktheone 则回忆谷歌几年前曾因担心滥用而拒绝发布类似模型，并认为此次发布显得未多加考虑。rcr-anti 批评谷歌在消费级、专业级与云平台之间的发布范围和能力长期不一致（并以 Omni Flash 在消费端支持视频与文本输出、在 GCP 上仅支持视频输出为例），指出被禁用消费端产品的企业用户难以用上完整功能；另有开发者分享了本地托管的有声书生成工具 KeenLore，作为无需云端调用与按量付费的替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49817615">Gemini 3.8 text-to-speech | Hacker News</a></li>
<li><a href="https://www.ndtvprofit.com/business/google-launches-gemini-3-8-flash-tts-with-custom-voice-creation-in-100-languages-12088416">Google Launches Gemini 3.8 Flash TTS With Custom Voice Creation In ...</a></li>
<li><a href="https://qwen3-tts.app/blog/qwen3-tts-vs-elevenlabs-openai-comparison-2026">Qwen3- TTS vs ElevenLabs vs OpenAI TTS : Comprehensive 2026...</a></li>
<li><a href="https://apiscout.dev/guides/elevenlabs-vs-openai-tts-vs-deepgram-aura-2026">ElevenLabs vs OpenAI TTS vs Deepgram Aura 2026 | APIScout</a></li>

</ul>
</details>

**标签**: `#text-to-speech`, `#gemini`, `#google`, `#voice-cloning`, `#generative-ai`

---

<a id="item-tech-news-4"></a>
### [观点文章：模型调用成本或将低于 grep 等本地工具](https://jyn.dev/tokens-too-cheap-to-meter/) ⭐️ 7.0/10

一篇由 teoruiz 于 2026 年 9 月 23 日发表在 jyn.dev 的博文《Tokens too cheap to meter》提出：LLM token 价格下降速度极快，调用模型可能很快比 grep 这类传统本地工具调用还便宜。据评论区援引，文章观察到目前一次 GPT-5.6 Luna 调用的成本仅比 grep 高约 4-5 个数量级，并预测按当前改进速度这一差距将持续缩小直至反转。这是一篇观点/分析类文章而非实证研究，发布后在 Hacker News 上引发活跃讨论（227 分、179 条评论）。

hackernews · teoruiz · 9月23日 09:21 · [社区讨论](https://news.ycombinator.com/item?id=49813482)

**「背景」** 在当前的 AI 编程智能体实践中，模型调用通常与 grep 等传统命令行工具搭配使用：grep 是确定性的本地计算，需要逐字节扫描文件，成本几乎可以忽略，而 LLM 调用按 token 计价且属于近似输出，两者的成本结构截然不同。这篇文章的前提正是 LLM 推理价格的持续快速下滑——按原文的供给侧分析，约 1.5 个 token 即可表示一个单词，且更小模型的单 token 价格更低；据评论转述，一次前沿模型调用的价格目前仍比 grep 高出约 4 到 5 个数量级，而文章认为按现有降速推算，这一差距可能在未来消失。标题中的“便宜到无需计量”（too cheap to meter）化用了刘易斯·施特劳斯 1954 年关于核电“太便宜以致无需装电表”的著名预言，这一历史类比也被读者用来提醒对成本外推保持警惕。

**「对代理开发者的实际影响」** 对构建 AI 代理的开发者而言，这一论点的具体影响是：&quot;本地确定性工具（如 grep）是廉价选项、模型调用是昂贵选项&quot;的默认架构假设可能需要重新检验，任务在本地工具与模型调用之间的路由标准将随之改变。但证据并不支持均匀外推这一趋势——Epoch AI 的数据显示 LLM 推理价格虽在快速下降，但各任务之间的降幅差异很大，而实际部署经验也表明单位 token 降价可能被用量增长抵消，导致总预算不降反升。因此，受影响团队更稳妥的做法是按真实工作负载逐任务测量推理成本（推理经济学研究已将推理成本列为决定 LLM 商业可行性的关键变量），并据此调整代理架构与预算规划，而非假设降价曲线会无限延续。

**「社区讨论」** 评论者 jetrink 援引 Stein&\#x27;s Law（“若某事无法永远持续，它终将停止”）质疑将当前成本改进速度无限外推的做法，cs702 则认为文章对企业商业模式可行性的分析不足，指出各家正基于未来利润预期投入巨额基础设施资金。另有评论者以 1954 年 Lewis Strauss 关于核电“电便宜到无需计量”的承诺作历史类比，提醒这类预言的落空风险；以上均为社区观点，成本曲线能否按作者预测延续尚无独立测算证实。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49813482">Tokens too cheap to meter - Hacker News</a></li>
<li><a href="https://jyn.dev/tokens-too-cheap-to-meter/">tokens too cheap to meter - jyn.dev</a></li>
<li><a href="https://arxiv.org/html/2510.26136v1">Beyond Benchmarks: The Economics of AI Inference - arXiv.org</a></li>
<li><a href="https://epoch.ai/data-insights/llm-inference-price-trends">LLM inference prices have fallen rapidly but unequally across tasks</a></li>
<li><a href="https://www.ikangai.com/the-llm-cost-paradox-how-cheaper-ai-models-are-breaking-budgets/">The LLM Cost Paradox: How &quot;Cheaper&quot; AI Models Are Breaking Budgets</a></li>

</ul>
</details>

**标签**: `#llm-pricing`, `#ai-economics`, `#ai-agents`, `#inference-costs`, `#industry-analysis`

---

<a id="item-tech-news-5"></a>
### [小米开源 MiMo-V2.6：重点不在 1M 上下文，而在长轨迹强化学习](https://www.leiphone.com/category/ai/f8vJztYMmCQ3ENED.html) ⭐️ 7.0/10

小米正式发布并开源 MiMo-V2.6：Pro 版总参数 1.02T、每 token 激活约 42B，Flash 版总参数 309B、激活 15B，两款均支持 1M token 上下文，并接受文本、图像、视频与音频输入。雷锋网的拆解文章认为，这次更值得关注的是后训练而非上下文长度：代码、通用 Agent、视觉与网络安全任务被放进同一套强化学习系统，奖励机制也重新设计；单次 RL 更新使用 1568 个 prompt、每个 prompt 生成 16 条 rollout，约合 2.5 万条行为轨迹，训练对象是包含状态、决策和反馈的完整轨迹，而不只是最终答案。为支撑这类长轨迹负载，Pro 的 70 层 Transformer 中有 60 层采用窗口仅 128 token 的 Sliding Window Attention、只有 10 层使用全局注意力，MoE 每层 384 个 routed expert 中仅激活 8 个。需要说明的是，这些训练细节来自厂商口径下的媒体拆解，原文在异步训练与奖励设计的具体实现处被截断，独立效果数据在现有内容中无法核实。

rss · 雷锋网 · 9月23日 04:07

**「背景」** MiMo-V2.6 系列由小米于 2026 年 9 月 21 日正式开源，采用 MIT 协议，Pro 版为 1.02T 总参数、42B 激活参数的稀疏 MoE 架构，第三方报道称其在 AA 智能指数上取得 46 分。理解这篇拆解的前提是：当模型以 Agent 形态长期驻留环境、反复读取信息、调用工具并执行操作时，后训练强化学习的优化对象已从单个最终答案变为包含状态、决策与反馈的完整行为轨迹，长上下文计算开销和奖励判定（例如如何区分两条都能完成任务的路径）由此成为后训练阶段的新难点。小米官方文档还确认，其 RL 训练系统采用大 batch 加全异步架构，单次更新使用 1568 个样本，支持 1M 上下文长度的训练，每个训练步的 token 数达 35～37 亿。

**「对开发者与部署方的影响」** MiMo-V2.6 已于 9 月 22 日凌晨上线并开源，开发者可以自行部署长上下文 Agent 服务；由于 Pro 每个 token 仅激活约 42B 参数、Flash 仅 15B，且 Pro 的 70 层中有 60 层只使用 128 token 的滑动窗口注意力，长序列推理的实际计算开销明显低于总参数规模给人的印象。不过选型时不宜只看 1M 上下文标签：知乎上有跑过该模型 RL 实验的用户评价 Flash 表现平平、仅属开源第二梯队，建议团队在自己的代码与 Agent 工作负载上实测后再决定采用哪个版本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/XiaomiMiMo/MiMo-V2.6-Pro-RL">XiaomiMiMo/MiMo-V2.6-Pro-RL · Hugging Face</a></li>
<li><a href="https://cellcog.ai/blog/mimo-v2-6/">MiMo-V2.6: Xiaomi&#x27;s Open 1T Model Hits 46 on the AA Index | CellCog</a></li>
<li><a href="https://mimo.mi.com/docs/en-US/news/latest/v2-6">Xiaomi MiMo-V2.6 Series: 3 New Models Officially Released</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/2084784910288549156">mimo-v2.6 RL scaling实验观察 - 知乎</a></li>
<li><a href="https://www.zhihu.com/question/2085626643880613806">MiMo-V2.6已于9月22日凌晨上线并开源，全系支持多模态，包含Flash和Pro模型，效果如何？ - 知乎</a></li>

</ul>
</details>

**标签**: `#large language models`, `#reinforcement learning`, `#long context`, `#reward design`, `#AI industry news`

---

<a id="item-tech-news-6"></a>
### [LeCun 于 ECCV 2026 演讲称「预测像素」是伪命题，主张以 JEPA 构建世界模型](https://www.leiphone.com/category/academic/F8VUijJ4JY8kkXTG.html) ⭐️ 7.0/10

图灵奖得主 Yann LeCun 在 ECCV 2026 主题演讲《World Models: Enabling the next AI revolution》中主张，仅靠语言和 token 训练无法让 AI 达到人类水平智能，也跨不过物理世界的门槛；通往 AGI 需要让系统从视频、传感器与交互中学习世界模型。他的核心论点是「预测像素」本身是伪命题——下一帧拍到什么取决于当前帧中不存在的信息（如镜头外是否有人走入、光线是否变化）——因此 JEPA（联合嵌入预测架构）不生成未来，而是由编码器丢弃不可预测的细节，只在抽象表征空间中预测未来。演讲结尾他给出三条建议，其中可见的两条是「别再死磕生成式模型」和「别再去研究 LLM」，第三条在报道原文中被截断。需要说明的是，这些是 LeCun 的论点而非已验证的研究成果；报道同时指出，2026 年「世界模型」一词已被四条路线各自认领：Sora、Genie 代表的视频生成，World Labs 的三维几何，英伟达 Cosmos、Omniverse 的物理仿真，以及 JEPA 的抽象表征预测。

rss · 雷锋网 · 9月23日 01:49

**「背景」** JEPA（联合嵌入预测架构）的思路是不生成像素，而是让编码器丢弃无法预测的细节、只在抽象表征空间中预测未来，这是 LeCun 押注多年、用以替代生成式路线的方案。据 ECCV 官网讲者资料，LeCun 曾任 Meta 首席 AI 科学家（2018–2025）和 Facebook AI Research 创始负责人（2013–2017），现任 AMI Labs 执行主席。此外，网上可查到他 2026 年 4 月在一次应用数学网络研讨会上使用的同题幻灯片《World Models: Enabling the next AI revolution》，说明此次 ECCV 2026 受邀演讲是该论述在另一场合的延续，而非全新提出。

**「对研究者的影响」** 对于正在选择技术路线的 AI 研究者和团队，LeCun 给出的直接行动建议是停止投入生成式模型与 LLM 研究，转向从视频、传感器与交互中学习世界模型，并用 JEPA 进行后果预测与动作规划——但这属于演讲者的个人主张，报道未提供任何机构因此调整方向的证据。在选型层面，「世界模型」目前对应视频生成、三维几何、物理仿真和抽象表征预测四种彼此不同的技术定义，团队需先确认所指的具体路线，再评估相应方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://eccv.ecva.net/virtual/2026/invited-talk/6155">ECCV Invited Talk Yann LeCun — World Models: Enabling the ...</a></li>
<li><a href="https://eccv.ecva.net/virtual/2026/eventlistwithbios/keynotes-panels">ECCV 2026 Keynotes &amp; Panels</a></li>
<li><a href="https://lipn.fr/svn/tex/slides/lecun.pdf">World Models: Enabling the next AI revolution</a></li>

</ul>
</details>

**标签**: `#Yann LeCun`, `#JEPA`, `#world models`, `#self-supervised learning`, `#ECCV 2026`

---

<a id="item-tech-news-7"></a>
### [AI 需求推动 HBM 单位面积价值首次超过先进制程逻辑芯片](https://www.tomshardware.com/pc-components/dram/dram-is-now-more-expensive-than-compute-chips-on-per-area-basis-ai-demand-drives-memory-die-value-past-leading-edge-silicon) ⭐️ 7.0/10

据 Tom&\#x27;s Hardware 报道的行业分析，受 AI 加速器对内存带宽和容量需求持续增长的推动，高带宽内存（HBM）的单位面积价值已首次超过部分先进制程逻辑芯片。报告将这一变化归因于 HBM 更高的制造门槛：需要更复杂的堆叠工艺、先进封装以及更严格的良率控制，而在此之前，先进制程芯片长期被视为半导体产业中单位面积价值最高的产品。这一转变意味着内存厂商在 AI 芯片供应链中的话语权和重要性进一步上升。不过，该报道为简短转述，未提供具体的芯片型号、价格对比数据或计算方法，“部分”先进制程芯片的具体范围也不明确，读者应将其视为行业趋势信号而非精确的成本结论。

telegram · zaihuapd · 9月23日 11:39

**「背景」** 高带宽内存（HBM）是一种基于 3D 堆叠 DRAM 的内存接口技术，最初由三星、AMD 与 SK 海力士联合开发，常与面向高性能场景的图形及 AI 加速器搭配使用。其价值攀升与制造门槛直接相关：堆叠层数增加要求不断减薄 DRAM 裸片以控制在封装高度限制之内，而减薄工艺已接近极限，裸片在制造和封装环节的处理难度显著上升。行业通常以每 Gb 价格乘以位密度来折算单位面积价值，例如按 1.50 美元/Gb 的 DRAM 价格估算，密度为 0.273 Gb/mm² 的 1z 代 DRAM 单位面积价值约为 0.410 美元/mm²。

**「常规内存采购或面临供应与价格压力」** 对需要采购服务器、工作站或内存的组织而言，这一价值变化对应着实际的产能转移：据行业报道，三星、SK 海力士和美光正积极将产能转向 HBM，高端 AI 内存已售罄至 2026 年，缺货可能延续到 2027 年，常规 DRAM 的供应与价格因此面临上行压力。采购方可考虑提前锁定内存供货或在预算中预留涨价空间；同时三星已设定到 2026 年底将 HBM 产能提高约 50% 的目标，其扩产落地进度将影响后续供应紧张能否缓解。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://www.tomshardware.com/pc-components/dram/dram-is-now-more-expensive-than-compute-chips-on-per-area-basis-ai-demand-drives-memory-die-value-past-leading-edge-silicon">Memory chips are now more expensive than ... | Tom &#x27; s Hardware</a></li>
<li><a href="https://semiengineering.com/issues-stack-up-with-more-hbm-layers/">Issues Stack Up With More HBM Layers</a></li>
<li><a href="https://enkiai.com/ai-market-intelligence/memory-shortage-2026-how-ai-will-cause-a-supply-crisis/">Memory Shortage 2026: How AI Will Cause a Supply Crisis - Enki.AI</a></li>
<li><a href="https://www.facebook.com/ign/posts/a-new-report-suggests-that-all-three-memory-manufacturers-samsung-sk-hynix-and-m/1619899053125227/">A new report suggests that all three memory manufacturers - Facebook</a></li>
<li><a href="https://www.ersaelectronics.com/blog/skhynix-samsung?srsltid=AU7gw4V08ACZeR7uAv5Yj7ZZiNZEE5SBLjnUGQmloWH7UIQbgyCl3LE0">SK Hynix &amp; Samsung: The Unprecedented HBM Expansion ...</a></li>

</ul>
</details>

**标签**: `#HBM`, `#DRAM`, `#半导体行业`, `#AI基础设施`, `#先进封装`

---