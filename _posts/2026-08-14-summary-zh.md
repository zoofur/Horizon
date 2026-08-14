---
layout: default
title: "Horizon Summary: 2026-08-14 (ZH)"
date: 2026-08-14
lang: zh
---

> 从 95 条内容中筛选出 10 条重要资讯。

---

1. [Azure Cosmos DB 曝严重漏洞：一条查询可攻破所有租户数据库](#item-1) ⭐️ 9.0/10
2. [OpenAI 发布 GPT-5.6 及帮助开发者打造高效 AI 智能体的构建指南](#item-2) ⭐️ 9.0/10
3. [谷歌推出 Gemini 3.7 Flash：更强大、更便宜的编码主力模型](#item-3) ⭐️ 8.0/10
4. [Cerebras 与 OpenAI 推出 GPT-5.6 Sol Ultrafast，推理速度宣称提升近 7 倍](#item-4) ⭐️ 8.0/10
5. [DeepSeek Harness 开发者预览版：一切皆插件、日志可追溯](#item-5) ⭐️ 8.0/10
6. [NP 被高估](#item-6) ⭐️ 8.0/10
7. [意面化 DRAM：逆向内存控制器攻击面](#item-7) ⭐️ 8.0/10
8. [白宫科学主管呼吁美国科学政策以 AI 为先、超越中国](#item-8) ⭐️ 8.0/10
9. [X 扩大开源排名算法并推出透明度工具](#item-9) ⭐️ 8.0/10
10. [苹果提交外部购买抽成方案，费率最高 15%](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Azure Cosmos DB 曝严重漏洞：一条查询可攻破所有租户数据库](https://www.infoq.cn/article/L9IqUuWzSB4zgP0PBqG2?utm_source=rss&utm_medium=article) ⭐️ 9.0/10

Azure Cosmos DB 被曝出严重漏洞 CosmosEscape，攻击者只需发送一条特制查询，就可能获取任意 Cosmos DB 账户的主密钥，从而跨租户访问数据库。该问题由安全研究人员披露，暴露出平台租户隔离机制存在缺陷。 Cosmos DB 是全球广泛使用的多租户云数据库服务，支撑着大量企业应用，因此跨租户漏洞是重大风险。一旦被利用，可能导致多个组织的敏感数据被未授权访问，动摇业界对托管云数据库隔离能力的信任。 漏洞根源在于 Cosmos DB 网关：该网关运行在多租户 Service Fabric 集群上，并使用账户主密钥访问客户数据库。网关可访问的凭据泄露了一个签名密钥，攻击者可用它请求任意 Cosmos DB 账户的主密钥，从而实现跨租户接管。

rss · InfoQ 中文站 · 8月13日 11:53

**背景**: Azure Cosmos DB 是微软提供的全球分布式、多模型数据库服务，旨在提供高可用、可扩展和低延迟的数据访问。多租户云服务中，各客户的数据在逻辑上相互隔离，但共享底层基础设施，因此隔离层的漏洞可能让一个租户的数据暴露给另一个租户。CosmosEscape 就是近期曝出的此类跨租户接管风险，出问题的是数据网关层。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://threat.wiki/ops/cosmosescape-azure-cosmos-db-cross-tenant-takeover/">CosmosEscape Azure Cosmos DB cross - tenant takeover - threat.wiki</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cosmos_DB">Cosmos DB - Wikipedia</a></li>

</ul>
</details>

**标签**: `#Azure`, `#Security`, `#Vulnerability`, `#Cloud Database`

---

<a id="item-2"></a>
## [OpenAI 发布 GPT-5.6 及帮助开发者打造高效 AI 智能体的构建指南](https://openai.com/index/builders-guide-to-gpt-5-6) ⭐️ 9.0/10

OpenAI 发布了 GPT-5.6，这是其 GPT 模型系列的最新重大版本，同时为初创企业提供了一份专门的构建指南。该指南重点介绍了新的 Responses API 功能和更智能的模型选择策略，以帮助开发者构建更快、更节省成本的 AI 智能体。 这一发布对开发者和 AI 从业者意义重大，因为它提供了一条利用更新、功能更强大的模型来控制成本的官方途径。强调模型选择和 Responses API，标志着行业持续向生产级智能体应用转型。 该构建指南重点介绍初创企业如何利用 GPT-5.6 更高效地创建 AI 智能体。它还详细说明了更新的 Responses API 功能，该 API 最初由 OpenAI 于 2025 年 3 月发布，旨在通过高级工具调用简化智能体应用的构建。

rss · OpenAI Blog · 8月13日 11:00

**背景**: GPT-5.6 是 OpenAI 大型语言模型系列的最新迭代。OpenAI 于 2025 年 3 月 11 日发布的 Responses API，将 Chat Completions API 的易用性与高级工具调用功能相结合。有效的模型选择正成为 AI 智能体的关键实践，因为不同模型在推理深度、响应质量和成本权衡方面各有差异。动态模型路由和选择策略可帮助开发者为每个任务优化性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/OpenAI_Responses_API">OpenAI Responses API</a></li>
<li><a href="https://learn.microsoft.com/en-us/microsoft-copilot-studio/authoring-select-agent-model">Select a primary AI model for your agent - Microsoft Copilot ...</a></li>
<li><a href="https://zylos.ai/research/2026-03-02-ai-agent-model-routing/">AI Agent Model Routing and Dynamic Model Selection Strategies</a></li>

</ul>
</details>

**标签**: `#GPT-5.6`, `#OpenAI`, `#AI agents`, `#Responses API`, `#model selection`

---

<a id="item-3"></a>
## [谷歌推出 Gemini 3.7 Flash：更强大、更便宜的编码主力模型](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/) ⭐️ 8.0/10

2026 年 8 月 13 日，谷歌发布了 Gemini 3.7 Flash，这是继 Gemini 3.6 Flash 发布仅三周后的又一次更新。新模型提升了编码和智能体（agent）性能，并引入了临时促销定价，该价格预计在 2026 年 12 月 31 日翻倍。 如此快速的发布节奏表明谷歌正在缩短 Flash 系列的迭代周期，让开发者更早用上更强的编码和视觉能力。此举也加剧了大模型 API 的价格战，在性价比上向 GPT-5.6 Luna 和 Claude Opus 等竞品发起挑战。 Gemini 3.7 Flash 支持可自定义的思考模式，让开发者权衡质量、成本和延迟。谷歌表示，此次发布直接响应开发者反馈，距 3.6 Flash 发布仅数周，其图像转 HTML 能力在与价格高得多的模型对比中表现不错。

hackernews · thisisauserid · 8月13日 17:23 · [社区讨论](https://news.ycombinator.com/item?id=49289112)

**背景**: Gemini Flash 系列是 Google DeepMind 旗下体积更小、效率更高的“主力”模型家族，专为高并发的生产场景设计，与更大的 Pro 或 Ultra 模型形成对比。Flash 模型支持多模态，常用于编码、智能体（agent）和视觉任务。3.7 Flash 的发布延续了 Gemini 高频、渐进式更新的节奏。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/">Gemini 3.7 Flash: our most intelligent workhorse model</a></li>
<li><a href="https://deepmind.google/models/model-cards/gemini-3-7-flash/">Gemini 3.7 Flash - Model Card — Google DeepMind</a></li>
<li><a href="https://ai.google.dev/gemini-api/docs/pricing">Gemini Developer API pricing - Google AI for Developers</a></li>

</ul>
</details>

**社区讨论**: 开发者们讨论热烈但看法不一。许多人称赞其图像转 HTML 的效果和具有竞争力的价格，也有人质疑谷歌为何如此快速地发布 Flash 模型（三周内从 3.6 到 3.7），并认为促销定价安排很奇怪；有评论者指出 Opus 5 在图像转 HTML 方面仍更强，但 Gemini 3.7 在其价位上性价比很高。

**标签**: `#Gemini`, `#Google AI`, `#LLM`, `#model release`, `#AI/ML`

---

<a id="item-4"></a>
## [Cerebras 与 OpenAI 推出 GPT-5.6 Sol Ultrafast，推理速度宣称提升近 7 倍](https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai) ⭐️ 8.0/10

Cerebras 与 OpenAI 宣布推出 GPT-5.6 Sol Ultrafast，一种新的推理模式，在前沿 AI 评估上的性能提升近 7 倍。测试中，它用 11 小时 11 分回答了全部 2500 道 HLE 问题，而 Claude Fable 5 完成同样任务并达到相近准确率耗时 78 小时 27 分钟。 这种加速之所以重要，是因为更快的推理能在实际时间预算内进行更多迭代式思考，从而显著提升复杂任务的回答质量。它也强化了 Cerebras 等专用晶圆级芯片在 AI 推理市场中的价值，影响依赖前沿大模型的研究人员和企业。 Cerebras 将速度提升归功于其晶圆级引擎（WSE-3）和 AI 推理云。目前尚未公布定价，部分观察者指出，Cerebras 和 OpenAI 都没有明确说明 Ultrafast 模式与标准 GPT-5.6 Sol 生成的结果完全一致，因此性能是否完全等同仍存在不确定性。

hackernews · pr337h4m · 8月13日 18:10 · [社区讨论](https://news.ycombinator.com/item?id=49289844)

**背景**: Cerebras Systems 设计晶圆级 AI 处理器，包括 WSE-3，它被宣传为全球最大的 AI 芯片，并为其 AI 推理云提供算力。前沿 AI 评估是用于衡量先进 AI 系统在困难任务上能力的标准化基准，例如这里提到的“人类最后一考”（HLE）。了解这些背景有助于理解为何在此类评估上的速度被视为一个重要里程碑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cerebras_Systems">Cerebras Systems - Wikipedia</a></li>
<li><a href="https://www.cerebras.ai/chip">Product - Chip - Cerebras</a></li>
<li><a href="https://www.aisi.gov.uk/frontier-ai-trends-report">Frontier AI Trends Report by The AI Security Institute (AISI)</a></li>

</ul>
</details>

**社区讨论**: Hacker News 评论区普遍欢迎速度提升，有人强调更快推理有助于迭代思考和更好的推理能力。不过也有多位评论者对 Ultrafast 是否真正达到标准 GPT-5.6 Sol 的准确率表示怀疑，并指出缺乏定价信息。还有评论者称所宣称的输出速度是‘了不起的工作’。

**标签**: `#AI`, `#LLM`, `#Inference`, `#Cerebras`, `#OpenAI`

---

<a id="item-5"></a>
## [DeepSeek Harness 开发者预览版：一切皆插件、日志可追溯](https://deepseek.com/harness/en/) ⭐️ 8.0/10

DeepSeek 发布了其 Harness 智能体框架的开发者预览版（v0.1，MIT 许可证），采用基于 Cordis v4 的“一切皆插件”架构，并提供仅追加的会话日志以实现全链路可追溯。该预览版已在 GitHub 开源，但官方警告会存在破坏性变更。 这一发布意义重大，因为它为开发者提供了可完全透明、可追溯的专有 AI 智能体框架替代方案，回应了对可观测性和审计性的需求。插件化一切的设计可能重塑智能体框架的组合与扩展方式。 所有能力——模型、工具、技能、会话、沙箱、存储、循环、调度和 UI——都是可替换、可重新组合的插件。会话日志会记录系统提示、推理过程、工具调用及结果、子智能体调度和每次上下文注入；预览版还警告可能存在破坏性 API 变更。

hackernews · bjin · 8月13日 12:58 · [社区讨论](https://news.ycombinator.com/item?id=49285244)

**背景**: Agent harness（智能体框架）是围绕大语言模型的软件基础设施，负责管理工具、记忆、状态和执行循环，从而将模型转变为智能体。DeepSeek Harness 基于 Cordis v4——一个无需重启进程即可热加载/卸载插件的元框架；其仅追加日志支持断点恢复、分支、搜索和回放。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.deepseek.com/harness/en/">DeepSeek Harness developer preview: Everything is a plugin</a></li>
<li><a href="https://github.com/deepseek-ai/deepseek-harness">GitHub - deepseek-ai/deepseek-harness: DeepSeek Harness ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Agent_harness">Agent harness - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 讨论很有实质性：一位作者承认这只是早期预览版，存在粗糙之处；有人称赞可追溯性是“杀手级功能”，认为美国模型因其加密、混淆的追踪机制无法提供；另一位评论者认为论文有用但并非突破性，还有人指出 Cordis 卸载插件时可回滚副作用；也有人因 README 过于简陋而质疑它到底是什么。

**标签**: `#AI`, `#DeepSeek`, `#developer-tools`, `#agent-harness`, `#open-source`

---

<a id="item-6"></a>
## [NP 被高估](https://gruhn.me/blog/2026-08-13/) ⭐️ 8.0/10

作者认为 NP 难度作为实际障碍被高估，引发了关于复杂性理论与现实世界问题解决作用的辩论。

hackernews · theanonymousone · 8月13日 20:14 · [社区讨论](https://news.ycombinator.com/item?id=49291268)

**标签**: `#complexity theory`, `#NP-hard`, `#algorithms`, `#software engineering`, `#practical computing`

---

<a id="item-7"></a>
## [意面化 DRAM：逆向内存控制器攻击面](https://github.com/xoreaxeaxeax/skitter-creek-bath-salts) ⭐️ 8.0/10

Christopher Domas 发布了一个新的硬件安全研究项目'skitter-creek-bath-salts'，对 DRAM 内部结构和现代内存控制器进行逆向工程，暴露了隐藏的攻击面。该研究显示，在 AMD Jaguar（AMD16h）系统上，ring-0 级 root 权限可以访问“负环”领域——即以前被认为无法访问的未记录的内存控制器寄存器和地址哈希逻辑。 这项研究意义重大，因为它揭示了 DRAM 和内存控制器的内部结构构成了一个在很大程度上未被记录的、甚至可从 ring-0 级别触及的攻击面。它可能使 Rowhammer 攻击、硬件级故障注入更加可靠，并加深对 CPU 厂商如何隐藏内存管理细节的理解，从而影响操作系统安全、游戏主机和云硬件。 README 指出受影响的平台是 AMD Jaguar（AMD16h）——一个 2013 年的老式低功耗架构——并提到 Zen 3 的内存控制器寄存器基地址不同。该攻击需要先获得 ring-0 代码执行权限，因此其主要效果是扩大影响范围：从内核级提升到固件/DRAM 级访问。预计还会有一场配套的 Black Hat 演讲。

hackernews · matt_d · 8月13日 14:17 · [社区讨论](https://news.ycombinator.com/item?id=49286341)

**背景**: DRAM 将数据存储在按行和列排列的电容单元中，而内存控制器是将 CPU 地址转换为精确的 DRAM 行、列、库（bank）和刷新命令的硬件。现代控制器采用复杂且往往未公开的地址哈希方案，将访问分布到不同的 bank 和通道以提高性能。Rowhammer 是一种已知漏洞，通过反复激活某一行导致相邻行位翻转，其可靠性依赖于获知精确的物理地址映射。这项工作继承了硬件逆向工程的传统，旨在揭示现代芯片内部专有逻辑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Row_hammer">Row hammer - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Memory_controller">Memory controller - Wikipedia</a></li>
<li><a href="https://www.systemverilog.io/design/understanding-ddr4-timing-parameters/">DDR 4 SDRAM - Understanding Timing Parameters - systemverilog.io</a></li>

</ul>
</details>

**社区讨论**: 评论者对配套的 Black Hat 演讲非常热情，称赞了 Christopher Domas 以往的逆向工程演示。一些人指出，DRAM 已变得如此复杂，存在巨大的未记录攻击面并不令人意外；另一些人则提出实际问题：除 AMD Jaguar 外，还有哪些 CPU 系列会受影响？鉴于内存控制器基地址不同，Zen 3 或更新的芯片是否也存在漏洞？

**标签**: `#security`, `#DRAM`, `#hardware`, `#reverse engineering`, `#exploitation`

---

<a id="item-8"></a>
## [白宫科学主管呼吁美国科学政策以 AI 为先、超越中国](https://www.economist.com/by-invitation/2026/08/13/the-case-for-overhauling-american-science) ⭐️ 8.0/10

白宫科学主管迈克尔·克拉齐奥斯在《经济学人》的“受邀评论”栏目撰文，主张美国科学政策应围绕人工智能展开全面改革，并致力于在同中国的竞争中占据优势。 这标志着美国科研政策和联邦研发投入方向可能出现重大转变，使联邦研发经费进一步向人工智能和对华地缘政治竞争倾斜。依赖联邦资助的科研人员、工程师和高校可能会看到资金方向发生显著变化。 这是一篇观点文章而非正式政策文件，其核心主张是将“用好人工智能”作为美国科学的组织原则。克拉齐奥斯明确将以与中国竞争作为此次改革提议的主要理由。

rss · The Economist · 8月13日 13:12

**背景**: 白宫科学主管一职由白宫科技政策办公室（OSTP）主任担任，负责为总统提供科技政策建议并协调联邦研发工作。过去十年来，美国科学政策越来越聚焦于与中国的战略竞争，尤其是在新兴技术领域。人工智能的迅速崛起进一步推动了重新调整联邦科研优先方向的呼声。这篇文章发表在《经济学人》的“受邀评论”栏目，该栏目主要刊登有影响力人物的观点文章，因此带有影响精英和全球舆论的意图。

**标签**: `#AI`, `#science policy`, `#US`, `#China`, `#innovation`

---

<a id="item-9"></a>
## [X 扩大开源排名算法并推出透明度工具](https://techcrunch.com/2026/08/13/x-open-sources-its-ranking-algorithm-letting-users-see-if-theyve-been-shadowbanned/) ⭐️ 8.0/10

X 已在 GitHub 上以 Apache 2.0 许可证开源其核心排名引擎和“为你推荐”时间线代码，代码规模约为此前版本的 10 至 15 倍。该公司还在设置中推出了一个透明度工具，符合条件的用户可下载 JSON 文件，查看其账号或帖子是否受到排名系统的影响。 这标志着大型社交媒体排名算法最大规模的开源行动之一，显著推进了算法问责制，并使得独立研究 X 如何对内容排名成为可能。该透明度工具还为用户提供了一种罕见的途径来检测可能的影子封禁或排名惩罚，这可能会促使其他平台效仿。 该透明度工具最初向账号注册满一年且近一个月发帖 10 次或以上的测试用户开放，允许他们以 JSON 文件形式下载聚合统计数据。值得注意的是，用于判断违规内容的 Grok 系统部分并未包含在此次开源发布中。

telegram · zaihuapd · 8月14日 01:03

**背景**: X（前身为 Twitter）于 2023 年 3 月首次以“The Algorithm”仓库名开源了其推荐算法。核心排名系统依靠 SimClusters 等机器学习模型和名为 Heavy Ranker 的神经网络来为“为你推荐”时间线中的帖子评分。此次扩展代表了一次规模大得多的代码发布，并增加了一项面向用户的透明度功能，这在大型社交平台中并不多见。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/08/13/x-open-sources-its-ranking-algorithm-letting-users-see-if-theyve-been-shadowbanned/">X open sources its ranking algorithm, letting users see if they've been 'shadowbanned' | TechCrunch</a></li>
<li><a href="https://adlibrary.com/guides/x-twitter-algorithm-explained">X (Twitter) Algorithm Explained 2026: How For You Ranks Posts</a></li>
<li><a href="https://www.firstpost.com/tech/x-open-sources-its-ranking-algorithm-lets-users-check-account-level-impacts-14038070.html">X open-sources its ranking algorithm, lets users check account-level impacts</a></li>

</ul>
</details>

**标签**: `#open source`, `#algorithm transparency`, `#ranking algorithm`, `#social media`, `#X`

---

<a id="item-10"></a>
## [苹果提交外部购买抽成方案，费率最高 15%](https://9to5mac.com/2026/08/13/apple-proposes-commissions-of-up-to-15-for-off-app-store-purchases-in-the-us/) ⭐️ 8.0/10

苹果已向法院提交美国 App Store 外部购买抽成方案：标准应用抽成 15%，视频、新闻等合作项目及订阅续费抽成 10%，小型企业计划应用抽成 5%。此前美国最高法院驳回了苹果暂停下级法院费率审理的请求。 这是 Epic Games 诉苹果反垄断案中的标志性进展，因为它为 App Store 之外完成购买提出了具体的费率层级。这将直接影响开发者的应用和订阅定价，并可能重塑 iOS 应用生态的经济模式。 费率因类别而异：标准应用抽成 15%，视频、新闻等合作项目及订阅续费抽成 10%，小型企业计划应用抽成 5%。Epic 将有回应机会，苹果预计于 9 月 14 日前向最高法院提交书面意见。

telegram · zaihuapd · 8月14日 02:33

**背景**: 该提案源于 Epic Games 诉苹果反垄断案，双方围绕 App Store 抽成和支付规则长期争讼。目前下级法院正在确定苹果可以对 App Store 之外的购买收取多少费用，苹果提交的方案列出了其拟议的费率结构。美国最高法院最近决定不暂停下级法院的审理，为继续推进费率确定程序扫清了道路。

**标签**: `#Apple`, `#App Store`, `#Epic Games`, `#Antitrust`, `#Commissions`

---