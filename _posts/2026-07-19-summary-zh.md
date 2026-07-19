---
layout: default
title: "Horizon Summary: 2026-07-19 (ZH)"
date: 2026-07-19
lang: zh
---

> 从 27 条内容中筛选出 10 条重要资讯。

---

1. [自进化 Agent Harness 性能提升 104%](#item-1) ⭐️ 8.0/10
2. [腾讯发布三大具身基座模型](#item-2) ⭐️ 8.0/10
3. [香港宏福苑火灾调查：承包商违规与监管全面失效](#item-3) ⭐️ 8.0/10
4. [文章：社区需要积极参与而非被动消费](#item-4) ⭐️ 7.0/10
5. [纽约市长禁止租房广告秘密使用 AI 图片](#item-5) ⭐️ 7.0/10
6. [Kimi K3 发布即登顶 Arena 排行榜](#item-6) ⭐️ 7.0/10
7. [中国 AI 产业出海白皮书发布](#item-7) ⭐️ 7.0/10
8. [可观测对象图语义层赋能 AI Agent 推理](#item-8) ⭐️ 7.0/10
9. [AI 智能体算力消耗过快，传统账单风控难以匹敌](#item-9) ⭐️ 7.0/10
10. [火山引擎重构多模态传输底座支持 Agent 时代视频通话](#item-10) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [自进化 Agent Harness 性能提升 104%](https://mp.weixin.qq.com/s?__biz=MzIzNjc1NzUzMw==&mid=2247904823&idx=3&sn=af8b10819641ba1f59492acb8aa9ebd4) ⭐️ 8.0/10

上海 AI 实验室提出了一种方法，让 AI 代理自我进化其运行规则（Harness），而无需更换模型，实现了高达 104%的性能提升。 这一突破大幅减少了人工调优 Agent Harness 的需求，有望在不进行昂贵模型重训练的情况下，使 AI 代理在各种应用中更具适应性和效率。 该框架称为 Self-Harness，将变更提议与验证分离：语言模型诊断失败并提出补丁，而确定性代码处理所有采样和显著性测试以确保可靠性。

rss · 量子位 · 7月18日 07:45

**背景**: Agent Harness 是将大型语言模型（LLM）转化为代理的软件基础设施，管理工具使用、记忆和执行循环。没有 Harness，LLM 本身是无状态的，仅限于文本生成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2607.13683">[2607.13683] Self-Evolving Agent Harnesses via Gated Semantic Quality-Diversity</a></li>
<li><a href="https://venturebeat.com/orchestration/researchers-introduce-self-harness-a-framework-that-lets-ai-agents-rewrite-their-own-rules-boosting-performance-up-to-60">Researchers introduce Self-Harness, a framework that lets AI agents rewrite their own rules, boosting performance up to 60% | VentureBeat</a></li>
<li><a href="https://en.wikipedia.org/wiki/Agent_harness">Agent harness</a></li>

</ul>
</details>

**标签**: `#AI Agent`, `#自进化`, `#Harness`, `#Shanghai AI Lab`

---

<a id="item-2"></a>
## [腾讯发布三大具身基座模型](https://www.infoq.cn/article/uD0p2FcQE2JKSwYY1wXK?utm_source=rss&utm_medium=article) ⭐️ 8.0/10

腾讯发布了三个具身 AI 基座模型，通过在工业任务中紧密耦合感知与行动，实现了超过 95%的成功率。 这意义重大，因为它展示了具身 AI 从研究到实际工业应用的重大进展，具有高可靠性，可能加速制造业自动化。 这三个模型旨在闭环感知-行动循环，使机器人能够感知环境并自主行动。超过 95%的成功率是在真实的工业环境中测得的。

rss · InfoQ 中文站 · 7月19日 07:55

**背景**: 具身 AI 指的是集成到物理实体中的 AI 系统，通过传感器和驱动器与世界交互。基座模型是大型预训练模型，可适应多种任务。感知-行动循环是机器人学的核心概念，感知指导行动，行动改变感知。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/glossary/embodied-ai/">Embodied AI: What Is It and How to Build It?</a></li>
<li><a href="https://lifestyle.sustainability-directory.com/term/perception-action-loop/">Perception-Action Loop → Term</a></li>

</ul>
</details>

**标签**: `#Tencent`, `#embodied AI`, `#foundation models`, `#robotics`, `#industrial AI`

---

<a id="item-3"></a>
## [香港宏福苑火灾调查：承包商违规与监管全面失效](https://china.caixin.com/2026-07-17/102465415.html) ⭐️ 8.0/10

一份 627 页的调查报告揭露，2025 年香港宏福苑大火中，承包商蓄意使用非阻燃材料并提交虚假防火证书，而政府部门监管全面失效，导致 168 人遇难。 调查结果暴露了香港建筑安全监管的系统性缺陷，引发对加强执法、实地检查及问责改革的迫切呼吁，可能重塑公共安全政策。 大火通过天井垂直蔓延，非阻燃安全网和发泡胶板助长火势；消防栓和警报系统被关闭，41 起居民投诉被忽视。

telegram · zaihuapd · 7月18日 10:01

**背景**: 中国标准 GB 5725 要求建筑安全网具备阻燃性能以防火灾蔓延。发泡胶板用于保温，但未经阻燃处理极易燃烧。高层建筑中，火灾可通过天井垂直蔓延（烟囱效应），浓烟灌满楼梯间堵塞逃生通道。香港政府过度依赖行业自我监管，缺乏现场核查，是酿成灾祸的原因之一。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ailegal.baidu.com/legalarticle/qadetail?id=6d63fa2572c985260130">用非阻燃安全网处罚 - ailegal.baidu.com</a></li>
<li><a href="https://www.sohu.com/a/965777079_121895465">大浦大火暴露出的安全网易燃隐患，安全网阻燃性能是否经得起 GB 5725...</a></li>
<li><a href="https://www.tfcaijing.com/touch/article/page/67672b4f367044633632596a365a59396658715058413d3d">tfcaijing.com/touch/article/page/67672b4f367044633632596a365...</a></li>

</ul>
</details>

**标签**: `#fire safety`, `#regulatory failure`, `#Hong Kong`, `#disaster investigation`, `#construction safety`

---

<a id="item-4"></a>
## [文章：社区需要积极参与而非被动消费](https://www.benlandautaylor.com/p/if-you-build-it-they-will-come) ⭐️ 7.0/10

Ben Landau Taylor 发表了一篇论文，认为社区需要成员的积极参与而不是被动消费，在 Hacker News 上引发了广泛讨论。 这一观点挑战了线上和线下社区中常见的消费者心态，为社区建设者和成员提供了促进更健康社交动态的可行见解。 该文用野生蓝莓丛的隐喻来说明人们往往将社区视为自动出现的特征，而非需要努力维护的事物。Hacker News 的讨论获得了 258 个点赞和 91 条评论，表明其引起了强烈共鸣。

hackernews · barry-cotter · 7月18日 15:37 · [社区讨论](https://news.ycombinator.com/item?id=48959090)

**社区讨论**: 评论者分享了个人经历，许多人同意对社区的消费者态度普遍存在。一些人强调了作为社交纽带的风险和倦怠的可能性，另一些人则反思了美国基层社会机构的衰落和代际鸿沟。

**标签**: `#community`, `#social dynamics`, `#essay`, `#hackernews`, `#building`

---

<a id="item-5"></a>
## [纽约市长禁止租房广告秘密使用 AI 图片](https://petapixel.com/2026/07/16/mayor-mamdani-says-landlords-cant-secretly-use-ai-images-to-advertise-properties/) ⭐️ 7.0/10

纽约市长 Mamdani 发布规定，要求房东在租房广告中披露任何使用 AI 生成的图片，实际上禁止了秘密使用此类欺骗性视觉内容。 这项规定回应了人们对 AI 生成的‘装修’照片扭曲公寓大小和特征、误导租房者的日益担忧。它为房地产广告中的 AI 问责制树立了先例，并可能推动其他城市出台类似规则。 该规则要求任何使用 AI 生成图片的房源必须明确标注，但并未完全禁止。要求适用于 StreetEasy 等平台，这些平台已被 AI 装修的房源充斥。

hackernews · gnabgib · 7月18日 22:13 · [社区讨论](https://news.ycombinator.com/item?id=48962983)

**背景**: AI 生成的图片通常使用生成对抗网络（GANs）创建，可以令人信服地改变房间尺寸并添加家具，使空间看起来更大。FTC 最近加强了对广告中 AI 披露的执法，但美国没有联邦 AI 法规；纽约等州正在制定自己的规则。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://humanadsai.com/blog/ftc-ai-generated-content-disclosure">FTC AI Content Disclosure Rules: What Brands Must Know in 2026</a></li>
<li><a href="https://billo.app/blog/us-ai-regulations/">The US AI Regulations: What Brands Need to Know Before June 2026</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍支持披露规则，但一些人主张全面禁止房地产中的 AI 图片。另一些人质疑这是否已被现有的欺骗性广告法涵盖，以及市长能否在没有立法支持的情况下单方面实施此类规则。

**标签**: `#AI regulation`, `#deceptive advertising`, `#real estate`, `#NYC`, `#AI ethics`

---

<a id="item-6"></a>
## [Kimi K3 发布即登顶 Arena 排行榜](https://www.infoq.cn/article/NtfFE25blBHubhNNTmkJ?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

Moonshot AI 的最新模型 Kimi K3 发布后立即在 Arena 排行榜上占据首位，并迅速上线“模型广场”平台。 这表明 Kimi K3 在与领先模型的竞争中表现出色，可能会增加在长周期编码和知识工作任务中的采用，也反映了 AI 模型发布的快速节奏。 Kimi K3 是一个拥有 2.8 万亿参数的混合专家模型，支持 100 万 token 的上下文窗口和原生视觉能力，被称为首个开放的 3T 级模型，可通过 Kimi API 平台获取。

rss · InfoQ 中文站 · 7月18日 17:14

**背景**: Arena 是一个公开排行榜，根据文本、图像和代码任务的真实评估对 AI 模型进行排名。“模型广场”是一个列出 200 多个 AI 模型供比较和定价的平台。Kimi K3 是 Kimi K2 系列的继任者，专为长周期编码和智能体工作负载设计。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://platform.kimi.ai/docs/guide/kimi-k3-quickstart">Kimi K3 - Kimi API Platform</a></li>
<li><a href="https://openlm.ai/kimi-k3/">Kimi K3 - openlm.ai</a></li>
<li><a href="https://arena.ai/leaderboard">Arena Leaderboard | Compare & Benchmark the Best Frontier AI ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#language models`, `#benchmark`, `#Kimi`

---

<a id="item-7"></a>
## [中国 AI 产业出海白皮书发布](https://www.infoq.cn/minibook/GSbtyU9968lerf5gwPpU?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

InfoQ 发布了一份白皮书，分析中国 AI 产业出海的核心要素与战略。 该白皮书为中国 AI 企业出海提供战略参考，揭示了全球扩张中的机遇与挑战。 白皮书涵盖技术、人才、合规及商业模式等关键领域，为成功出海提供指导。

rss · InfoQ 中文站 · 7月18日 12:02

**背景**: 白皮书是权威报告，用于介绍复杂议题。中国 AI 产业日趋成熟，众多企业开始寻求海外市场以提升竞争力。该白皮书为理解出海战略考量提供了参考。

**标签**: `#AI`, `#China`, `#industry report`, `#globalization`, `#strategy`

---

<a id="item-8"></a>
## [可观测对象图语义层赋能 AI Agent 推理](https://www.infoq.cn/article/KPd6YwU0Y1iCMGMakSmE?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

阿里云技术专家张鑫在 AICon 深圳大会提出并开源了一种可观测对象图语义层设计，旨在解决 AI Agent 处理企业数据时的推理瓶颈。 该工作直接解决了 AI Agent 拿到数据却无法有效推理的常见问题，提升了其理解业务规则和做出准确决策的能力。它为可广泛采用的企业 AI 部署提供了一种实用的工程方法。 可观测对象图语义层结合了可观测性（如 OpenTelemetry）和语义层概念，创建了基于规则而非原始概率帮助 Agent 进行推理的结构化表示。该设计已开源，但公告中未提供具体仓库细节。

rss · InfoQ 中文站 · 7月18日 10:00

**背景**: AI Agent 经常因缺乏结构化业务上下文而难以推理企业数据。常见的 RAG（检索增强生成）或把数据塞进上下文窗口等方法存在局限。语义层作为一种“规则系统”抽象业务逻辑，使智能体从概率生成转向基于规则的推理。提出的可观测对象图为此层增加了监控和可追溯性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.infoq.cn/article/KPd6YwU0Y1iCMGMakSmE">为什么 AI Agent 拿到数据却不会推理？可观测对象图语义层的设计与开...</a></li>
<li><a href="https://aloudata.com/resources/guides/ai-data-intelligence/ai-agent-semantic-layer-governance">别让 AI Agent 胡说八道：如何用统一语义层为智能体“立规矩” | Alouda...</a></li>

</ul>
</details>

**标签**: `#AI Agent`, `#知识图谱`, `#语义层`, `#推理`, `#开源`

---

<a id="item-9"></a>
## [AI 智能体算力消耗过快，传统账单风控难以匹敌](https://www.infoq.cn/article/secM60Za0CNxIYvQO47m?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

文章指出一个日益突出的运营挑战：AI 智能体的算力消耗速度远超传统云账单和风控系统的处理能力，可能导致成本超支和治理漏洞。 这一问题对规模化部署 AI 智能体的企业至关重要，因为高效的账单与风险管理是可持续 AI 基础设施的基础。若未更新控制措施，企业将面临不可预测的成本和安全风险。 InfoQ 的文章指出，当前账单系统并非为 AI 智能体突发且不可预测的算力使用模式而设计，这可能在风险监控中引发级联故障。传统的账单周期和阈值反应过慢，无法应对分钟级的资源峰值。

rss · InfoQ 中文站 · 7月18日 09:00

**背景**: AI 智能体是利用大语言模型或其他 AI 技术执行任务的自主软件程序，通常同时运行多个操作。云账单通常采用订阅或按量付费模式并设有固定阈值，但 AI 智能体可能导致资源突然飙升，超出预设限制，使得实时成本控制变得困难。适当的账单风控措施（如每小时上限和自动告警）对于管理这类动态变化至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://amnic.com/blogs/cloud-billing-cycle">Cloud Billing Cycle Explained: Models and Optimization - Amnic</a></li>
<li><a href="https://agentxcloud.com/engineering/cloud-billing-risk">Cloud Billing Risk Controls for VPS and Managed Hosting</a></li>
<li><a href="https://nordcloud.com/blog/follow-the-money-what-cloud-billing-reveals-about-security-risk-operations/">Follow the money: what cloud billing reveals about security ...</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#billing`, `#infrastructure`, `#risk management`

---

<a id="item-10"></a>
## [火山引擎重构多模态传输底座支持 Agent 时代视频通话](https://www.infoq.cn/article/GICIrEsTJwEgGsDYFvCM?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

字节跳动旗下云服务平台火山引擎重构了其多模态传输基础设施，为 AI Agent 提供视频通话能力，使其能够在 Agent 驱动的应用中实现实时语音和视频交互。 这一升级至关重要，因为 AI Agent 越来越需要多模态通信（语音、视频、文本）来与人类自然交互。它为 Agent 时代的云基础设施树立了新标准，将影响构建对话式 AI 产品的开发者和企业。 此次重构专注于低延迟传输和高效多模态数据处理，支持与 Agent 编排集成的高质量视频通话。虽然未披露具体技术细节，但此举使火山引擎在 Agent 基础设施领域与华为云等竞争对手展开竞争。

rss · InfoQ 中文站 · 7月18日 08:54

**背景**: 火山引擎是字节跳动于 2020 年推出的云服务平台，提供企业数字化服务。随着 AI Agent 成为主流，云服务商正在构建 Agent 基础设施来处理多模态工作负载，包括实时通信。火山引擎的更新解决了 Agent 进行视频通话的需求，这是一项需要协调音频、视频和 AI 处理的复杂任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://baike.baidu.com/en/item/Volcano+Engine/1423148">Volcano Engine（ByteDance's cloud service platform）_Baiduwiki</a></li>
<li><a href="https://www.besthub.dev/articles/a-new-data-lake-paradigm-volcano-engine-s-multi-modal-data-lake-built-on-lance-3a6eae3d580a">A New Data Lake Paradigm: Volcano Engine’s Multi‑Modal Data ...</a></li>
<li><a href="https://devblogs.microsoft.com/all-things-azure/platform-engineering-for-the-agentic-ai-era/">Platform Engineering for the Agentic AI era | All things Azure</a></li>

</ul>
</details>

**标签**: `#video calls`, `#multimodal AI`, `#cloud infrastructure`, `#AI agents`, `#Volcano Engine`

---