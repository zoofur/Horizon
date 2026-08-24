---
layout: default
title: "Horizon Summary: 2026-08-24 (ZH)"
date: 2026-08-24
lang: zh
---

> 从 33 条内容中筛选出 10 条重要资讯。

---

1. [1998 年经典文章：复杂系统如何失效与根本原因分析的徒劳](#item-1) ⭐️ 9.0/10
2. [拥有你的设备：深入固件逆向工程](#item-2) ⭐️ 8.0/10
3. [Staff Engineer 寻找高影响力问题的系统方法](#item-3) ⭐️ 8.0/10
4. [Anthropic 旗舰模型用户增长乏力，廉价竞品趁势发展](#item-4) ⭐️ 8.0/10
5. [DynamoDB 原生支持向量搜索，挑战专用向量数据库](#item-5) ⭐️ 8.0/10
6. [开发者公开 AGENTS.md 规则以提升 LLM 代码质量](#item-6) ⭐️ 7.0/10
7. [什么是 Harness？重新思考 AI 智能体的接口层](#item-7) ⭐️ 7.0/10
8. [中国安卓车载中控遭 OTA 更新植入恶意软件](#item-8) ⭐️ 7.0/10
9. [Cloudflare WriteGuard 为 MCP 服务器提供精细化安全控制](#item-9) ⭐️ 7.0/10
10. [亚马逊云科技开源 Dogwood，为 AI 智能体工具调用立规矩](#item-10) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [1998 年经典文章：复杂系统如何失效与根本原因分析的徒劳](https://how.complexsystems.fail/) ⭐️ 9.0/10

理查德·库克 1998 年的文章《复杂系统如何失效》在 Hacker News 上被重新讨论，被视为关于系统失效、弹性工程和根本原因分析局限性的关键文本。 这篇文章被广泛视为弹性工程和混沌工程的奠基之作，其论点直接影响现代软件团队针对失效进行设计的方式。它挑战了寻找单一根本原因的传统思路，转而主张构建能够承受并从意外事件中恢复的系统。 该文章由医学博士理查德·库克于 1998 年撰写，可在 how.complexsystems.fail 免费获取。虽然最初聚焦于患者安全，但其原则已被航空、医疗和软件运维等行业广泛采纳。

hackernews · shortcrct · 8月23日 15:13 · [社区讨论](https://news.ycombinator.com/item?id=49409473)

**背景**: 复杂系统本质上是危险的，因为其包含许多相互作用的组件，任何人都无法完全理解。弹性工程是安全科学的一个子领域，研究系统如何在复杂性和时间压力下应对意外并保持安全运行。受这些思想启发的混沌工程会故意在生产系统中引入故障，以暴露弱点并建立系统承受动荡条件的信心。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Resilience_engineering">Resilience engineering</a></li>
<li><a href="https://how.complexsystems.fail/">How Complex Systems Fail</a></li>
<li><a href="https://en.wikipedia.org/wiki/Chaos_engineering">Chaos engineering</a></li>

</ul>
</details>

**社区讨论**: 评论者高度赞扬这篇文章，tptacek 称其'直到你亲眼目睹复杂系统真正失效才会体会到其重要性'，并指出常见的解读是根本原因分析徒劳无功。jedberg 认为文章的主题启发了混沌工程，另一位评论者推荐了约翰·高尔的《Systemantics》作为相关读物。

**标签**: `#systems engineering`, `#complexity`, `#failure analysis`, `#resilience engineering`, `#chaos engineering`

---

<a id="item-2"></a>
## [拥有你的设备：深入固件逆向工程](https://schlarp.com/posts/everything-i-own-owned/) ⭐️ 8.0/10

博客文章《Everything I own, owned》记录了作者通过逆向工程和修补固件，全面掌控自己设备的经历。文章重点介绍了修改设备固件的实用方法，以去除不需要的功能并实现真正的所有权。 随着越来越多的日常设备运行专有固件，用户往往无法真正掌控自己的硬件。这篇文章意义重大，因为它展示了个人可以重新夺回主动权，并且在人工智能辅助逆向工程的帮助下，这一过程对爱好者和安全研究人员来说正变得越来越容易。 作者从一台华硕 ROG Swift PG42UQ 显示器入手，目的是移除不断出现的像素清理弹出提示，并计划为其修补固件。社区中的例子既有成功案例（如通过 Claude 给 Wi-Fi 插座继电器刷写固件），也有风险教训（如在修改固件时把路由器变砖）。

hackernews · schlarpc · 8月23日 22:41 · [社区讨论](https://news.ycombinator.com/item?id=49413320)

**背景**: 固件是嵌入在硬件中的底层软件，控制设备功能，通常是专有的，且被制造商锁定。逆向工程固件包括提取固件、分析代码，有时还需打补丁来改变其行为。在这种背景下，“拥有”设备意味着能够修改和控制其所有软件层面。像 Binary Ninja 的 Firmware Ninja 这样的工具以及逐步指南能帮助研究人员完成这一复杂流程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://binary.ninja/2025/04/02/firmware-ninja.html">Binary Ninja - Embedded Reverse Engineering with Firmware Ninja</a></li>
<li><a href="https://www.infosecinstitute.com/resources/iot-security/iot-security-fundamentals-reverse-engineering-firmware/">Firmware reverse engineering: A step-by-step guide | Infosec</a></li>
<li><a href="https://tcm-sec.com/hardware-hacking-part-3-analyzing-firmware/">Analyzing Firmware : Hardware Hacking Part 3 - TCM Security</a></li>

</ul>
</details>

**社区讨论**: 评论对使用 AI 代理大幅加速逆向工程感到兴奋，但也提醒人们注意将昂贵设备变砖的风险。成功案例包括在没有事先研究的情况下控制一个 Wi-Fi 插座，以及用几小时逆向出小众设备的文件格式；而一次失败的路由器修补则凸显了更安全的迭代修补方法的必要性。

**标签**: `#reverse engineering`, `#firmware`, `#IoT`, `#security`, `#hacking`

---

<a id="item-3"></a>
## [Staff Engineer 寻找高影响力问题的系统方法](https://lalitm.com/post/find-problems-staff-engineer/) ⭐️ 8.0/10

这篇文章提出了一种方法：Staff Engineer 会等待同一模式在多个问题领域重复出现，再投入精力构建通用解决方案，而不是针对孤立问题立即行动。作者也承认这种方法有前提条件，比如在大公司中需要自下而上的自主权。 这很重要，因为 Staff Engineer 的职责是解决高杠杆问题，但关于如何识别这些问题，具体的框架很少。这种方法能帮助工程师避免浪费精力，并使工作与组织需求保持一致，但其适用性取决于公司文化。 一个关键前提是，作者的经验来自大公司的基础设施和开发者工具团队，这些团队拥有较充分的自下而上自主权。在自上而下的环境或初创公司中，这套方法可能并不直接适用，因为优先级变化快、资源限制也更紧。

hackernews · vanpra · 8月23日 19:23 · [社区讨论](https://news.ycombinator.com/item?id=49411643)

**背景**: Staff Engineer 是一种高级技术人员（individual contributor），负责跨团队解决全局性的技术问题，常常在工程团队与管理层之间起到桥梁作用。与管理者的区别在于，他们没有直接的管理权力，因此需要通过专业能力影响技术路线。这篇文章的思路是：跨领域反复出现的相同模式，正是通用解决方案能创造最大价值的信号。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://leaddev.com/leadership/what-staff-engineer-technical-leaders-arent-managers">What is a staff engineer? Technical leaders who aren't managers - LeadDev</a></li>
<li><a href="https://www.reddit.com/r/programming/comments/10wxp5i/what_is_a_staff_engineer/">r/programming on Reddit: What is a Staff Engineer?</a></li>

</ul>
</details>

**社区讨论**: 评论区对该方法的实用性提出了质疑。有评论者认为，团队往往缺乏耐心，如果没有现成解决方案，他们会自己绕过去，形成“先有鸡还是先有蛋”的问题。另有人质疑整个行业是否正在减少自下而上的自主权；而一位创业公司的工程师表示，更大的挑战是排定优先级而不是找问题。还有产品方向的评论补充说，用户常直接要某个方案而不说根本原因，因此更需要深入分析。

**标签**: `#career`, `#engineering-management`, `#problem-solving`, `#staff-engineer`

---

<a id="item-4"></a>
## [Anthropic 旗舰模型用户增长乏力，廉价竞品趁势发展](https://www.ft.com/content/5ee49718-c258-4f01-aa32-7e5b76ae5245) ⭐️ 8.0/10

《金融时报》报道称，Anthropic 最先进的 AI 模型在吸引用户方面遇到困难，而更便宜的替代方案正在获得市场青睐。读者评论指出，定价和访问限制是采用缓慢的关键原因。 此事意义重大，因为 Anthropic 是领先的 AI 实验室，如果其最佳模型无法将质量转化为用户量，就可能在竞争中输给 OpenAI 和成本更低的提供商。该公司的定价策略还可能影响整个 AI 市场如何在能力、成本与可及性之间取得平衡。 社区评论者描述了令人困惑的变现举措，例如高级功能只在限定时间内可用、使用量上限低于 50%，以及将顶级能力在不同订阅等级之间来回调整。部分用户还怀疑旧模型被降智，或新旗舰被刻意削弱以拉大付费等级之间的差距。

hackernews · naves · 8月23日 18:16 · [社区讨论](https://news.ycombinator.com/item?id=49411102)

**背景**: Anthropic 是一家以 Claude 系列大语言模型闻名的 AI 安全公司。AI 实验室通常通过订阅计划或按 token 计费来将前沿模型商业化，而高级模型的推理成本很高，因此服务商常用分级访问来控制成本。《金融时报》的报道似乎正是聚焦于这种定价压力如何影响 Anthropic 在消费者端的采用率。

**社区讨论**: 评论者普遍对 Anthropic 的变现和访问政策感到不满，认为相比之下 OpenAI 更可靠、更大方。不少用户怀疑新旗舰模型是被人为削弱了，实力不如前代；还有人抱怨 token 费用和严格的使用限制让产品难以真正使用。

**标签**: `#AI`, `#Anthropic`, `#Pricing`, `#Generative AI`, `#Business Strategy`

---

<a id="item-5"></a>
## [DynamoDB 原生支持向量搜索，挑战专用向量数据库](https://www.infoq.cn/article/9YicfQysexJdmx11xG4m?utm_source=rss&utm_medium=article) ⭐️ 8.0/10

2026 年 8 月 5 日，AWS 宣布 Amazon DynamoDB 现在原生支持实时向量搜索，具备个位数毫秒延迟和 99% 以上的召回率，可扩展到万亿级向量。这消除了基于 DynamoDB 的应用为相似性搜索单独运行向量数据库的需要。 这一举措可能颠覆独立的向量数据库市场，让开发者将业务数据与向量搜索放在同一处，从而简化 AI 应用架构。它直接影响到在 AWS 上构建语义搜索、推荐引擎和检索增强生成（RAG）系统的团队。 原生向量搜索能力不需要管理任何基础设施，并且面向任意规模设计，最高可支持万亿级向量。AWS 还演示了使用 Amazon Bedrock 嵌入构建语义搜索应用，并详细说明了向量搜索的计量方式，同时支持元数据过滤和混合检索工作流。

rss · InfoQ 中文站 · 8月23日 14:09

**背景**: 向量数据库存储和检索高维向量嵌入，支持语义相似性搜索，而不是精确匹配查找。这些嵌入常用于语义搜索、多模态搜索和 RAG。以前，需要向量相似性搜索的 DynamoDB 用户必须单独运行一个向量数据库，增加了运维复杂性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aws.amazon.com/blogs/aws/amazon-dynamodb-now-supports-real-time-vector-search-at-any-scale/">Amazon DynamoDB now supports real-time vector search at any ...</a></li>
<li><a href="https://aws.amazon.com/blogs/database/build-semantic-search-with-native-vector-support-in-amazon-dynamodb/">Build semantic search with native vector support in Amazon ...</a></li>
<li><a href="https://www.infoq.com/news/2026/08/aws-dynamodb-vector-search/">AWS Introduces Native Vector Search for DynamoDB - InfoQ</a></li>

</ul>
</details>

**标签**: `#DynamoDB`, `#Vector Search`, `#AI`, `#Database`, `#AWS`

---

<a id="item-6"></a>
## [开发者公开 AGENTS.md 规则以提升 LLM 代码质量](https://fabiensanglard.net/agent.md/index.html) ⭐️ 7.0/10

开发者 Fabien Sanglard 公开了他个人使用的 AGENTS.md 文件，其中包含一套旨在引导 LLM 编码 Agent 产出更高质量代码的规则与指令。这篇文章迅速获得关注，并引发了有关这些规则应写入 Agent 提示词还是交由 linter 强制执行的社区讨论。 随着 AI 辅助开发成为许多工作流中的标准环节，AGENTS.md 正成为向编码 Agent 提供持久项目上下文的事实标准。这场讨论折射出行业内一个更广泛的问题：代码质量防线应当放在哪里，它影响着每一位依赖 LLM 生成代码的开发者。 这份共享文件包含约十几条规则，例如单行 if 语句也必须使用花括号、函数名长度不超过 30 个字符，同时还有提交信息规范。评论者指出部分规则与 linter 已检查的内容重复；还有用户举例说，LLM 曾生成了 web-sys 中那种长达 80 多个字符的真实 API 名，例如 draw_image_with_html_image_element_and_sw_and_sh_and_dx_and_dy_and_dw_and_dh。

hackernews · ibobev · 8月23日 17:59 · [社区讨论](https://news.ycombinator.com/item?id=49410932)

**背景**: AGENTS.md 是一种开放格式，相当于 AI 编码 Agent 的 README——一个纯文本文件，记录项目的约定、架构和约束，让助手在多个会话中保持行为一致。它在 Cursor、Claude Code 等 Agent 化编码环境中日益流行。随着 LLM 生成的代码能力增强但仍容易出现结构性问题，开发者越来越依赖此类指令文件来保证质量，有时还会与传统的 lint 和风格检查搭配使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://agents.md/">AGENTS.md</a></li>
<li><a href="https://cobusgreyling.medium.com/what-is-agents-md-2846b586b116">What is AGENTS.md?. AGENTS.md has become the most practical… | by Cobus Greyling | Medium</a></li>

</ul>
</details>

**社区讨论**: 评论区总体氛围是建设性的，但在必要性上存在分歧：有人主张大多数规则应由 linter 强制执行，让手工编写的代码也遵守同样的标准；也有人觉得不少规则只是在重复 Agent 本已理解的基础 CS 原则。一个有趣的例子是，LLM 原样使用了一个 80 多字符的真实 API 名，说明“函数名要短”这类规则无法纠正上游库的命名选择。还有几位用户分享了自己更为精简的 AGENTS.md 版本——例如三态“收敛规则”——可见并没有放之四海而皆准的方案。

**标签**: `#LLM`, `#code-quality`, `#AGENTS.md`, `#developer-tools`, `#best-practices`

---

<a id="item-7"></a>
## [什么是 Harness？重新思考 AI 智能体的接口层](https://earendil.com/posts/what-is-a-harness/) ⭐️ 7.0/10

文章《What Is a Harness?》提出了 AI 智能体中“harness”的概念框架，将其比作汽车底盘，并在 Hacker News 上获得了 309 分和 135 条评论。该文将 harness 定义为连接 LLM 与工具、状态和执行环境的接口层，引发了实践者的广泛讨论。 随着 AI 智能体在 LLM 应用中日益重要，harness 正成为决定智能体实际能力的关键架构层。这篇文章为理解智能体基础设施提供了通用词汇和心理模型，同时社区讨论突出了交接（handoff）、可扩展性和工具设计等实际需求。 作者 ni10c 指出这篇文章面向非黑客读者，并考虑了“harness = 底盘、model = 引擎、fuel = 燃料、agent = 汽车”的类比是否更具解释力。评论者分享了实际经验，比如为会计智能体构建内部 CLI，并提出了支持跨模态、跨团队、跨模型和跨提供方交接（handoff）的 harness 问题。

hackernews · tosh · 8月23日 14:24 · [社区讨论](https://news.ycombinator.com/item?id=49409092)

**背景**: Agent harness，又称 agent scaffolding（智能体外架/脚手架），是围绕 LLM 的软件基础设施，使其能够作为 AI 智能体运行，负责管理工具调用、内存、状态持久化、执行环境和反馈循环。由于 LLM 是无状态的且只能生成文本，harness 正是支持多步骤、使用工具和长期运行任务的关键，常用公式表示为 Agent = Model + Harness。Microsoft Agent Framework 和 LangChain 等主流框架正在积极文档化和构建 harness 架构，显示出行业关注度日益提升。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Agent_harness">Agent harness - Wikipedia</a></li>
<li><a href="https://www.langchain.com/blog/the-anatomy-of-an-agent-harness">The Anatomy of an Agent Harness - langchain.com</a></li>
<li><a href="https://learn.microsoft.com/en-us/agent-framework/concepts/harness">Agent Harness | Microsoft Learn</a></li>

</ul>
</details>

**社区讨论**: 实践者的反馈总体积极，有评论者分享了为会计智能体构建内部 CLI harness 的成功经验，也有人称赞 Pi 的扩展系统是最佳 harness。其他人提出了关于跨界面和跨提供方、支持交接的 harness 的开放问题，作者本人也邀请大家对底盘类比提出意见。有评论者预测“harness”将成为 2026 年的 AI 热词。

**标签**: `#AI agents`, `#LLM tooling`, `#agent infrastructure`, `#interface design`

---

<a id="item-8"></a>
## [中国安卓车载中控遭 OTA 更新植入恶意软件](https://securelist.com/android-head-unit-malware/121106/) ⭐️ 7.0/10

卡巴斯基 Securelist 的研究人员报告称，恶意软件正通过第一方 OTA（空中下载）更新，被植入到廉价的中国安卓车载中控固件中。该恶意软件不具备自我传播能力，也不影响仅作为屏幕镜像协议的 Android Auto。 车载中控常与手机配对，并可能连接到车辆的 CAN 总线，这意味着此类恶意软件可能被利用来向手机横向渗透，甚至在极端情况下直接触发刹车和发动机等关键车辆系统的动作。这凸显了廉价后装汽车零部件日益增长的安全风险。 感染途径是廉价中国后装安卓车载中控的官方第一方 OTA 更新，而非在生态系统中自我传播。由于车载中控通常不存有高价值数据，该恶意软件的一个可能用途是将设备招募进僵尸网络。

hackernews · campuscodi · 8月23日 13:05 · [社区讨论](https://news.ycombinator.com/item?id=49408550)

**背景**: CAN 总线（控制器局域网）是一种车辆总线标准，使电子控制单元（ECU）无需主机即可通信，常被比作汽车的神经系统。安卓车载中控是运行完整安卓操作系统的后装信息娱乐系统，可以安装 APK，这与 Android Auto 或 CarPlay 不同，后两者是透传协议，主要计算在手机上完成，仅将手机屏幕镜像到中控。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/CAN_bus">CAN bus - Wikipedia</a></li>
<li><a href="https://www.csselectronics.com/pages/can-bus-simple-intro-tutorial">CAN Bus Explained - A Simple Intro [2026] – CSS Electronics CAN bus - Wikipedia CAN Bus in Cars: Everything You Need to Know - Auto Veteran Introduction to CAN bus for automotive: a practical guide for ... CAN Bus in Automotive: A Comprehensive Guide What Is a CAN Bus on a Car and How Does It Work? CAN Bus Explained (2025): Frames, Arbitration & Tools - AutoPi.io</a></li>
<li><a href="https://www.autoveteran.tech/blog/details/442/can-bus-in-cars:-everything-you-need-to-know/">CAN Bus in Cars: Everything You Need to Know - Auto Veteran</a></li>

</ul>
</details>

**社区讨论**: 评论者澄清该恶意软件不会自我传播，且只影响廉价后装中控，不涉及 Android Auto。有人担心车载中控可能连接 CAN 总线，从而被远程控制门锁、车窗甚至驾驶功能，未来的版本还可能横向渗透到已配对的手机。整体情绪既有不安，也有对汽车行业安全实践缺失的批评。

**标签**: `#security`, `#malware`, `#android`, `#automotive`, `#IoT`

---

<a id="item-9"></a>
## [Cloudflare WriteGuard 为 MCP 服务器提供精细化安全控制](https://www.infoq.cn/article/1pa8asW4xOs6y2GYfl8T?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

Cloudflare 推出了 WriteGuard，为 Model Context Protocol（MCP）服务器提供精细化的安全控制，旨在增强 AI 上下文交互中的安全性。 随着 MCP 成为连接 AI 应用与外部工具和数据的关键标准，MCP 服务器的安全性日益重要。来自 Cloudflare 这样的大型基础设施厂商的 WriteGuard，有望推动企业在生产环境中更安全地采用 AI 智能体。 新闻报道未说明 WriteGuard 的版本号或具体配置细节。该服务似乎侧重于对 MCP 服务器进行细粒度的权限和策略管理，以应对未授权工具调用、数据泄露等威胁。

rss · InfoQ 中文站 · 8月24日 09:03

**背景**: Model Context Protocol（MCP）是由 Anthropic 于 2024 年 11 月推出的开放标准，旨在规范 AI 系统（如大语言模型）与外部工具和数据源的集成方式。MCP 服务器充当中间层，为 AI 应用提供上下文，而随着 AI 智能体能力增强，这些交互的安全问题日益凸显。Cloudflare 一直致力于构建 AI 和边缘基础设施，MCP 安全是其产品组合的自然延伸。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>
<li><a href="https://modelcontextprotocol.io/docs/2026-07-28/getting-started/intro">What is the Model Context Protocol (MCP)?</a></li>
<li><a href="https://modelcontextprotocol.io/docs/2026-07-28/learn/architecture">Architecture overview - Model Context Protocol</a></li>

</ul>
</details>

**标签**: `#Cloudflare`, `#MCP`, `#Security`, `#AI Infrastructure`

---

<a id="item-10"></a>
## [亚马逊云科技开源 Dogwood，为 AI 智能体工具调用立规矩](https://www.infoq.cn/article/cwj5Ikvhqu5mKH22zKsO?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

亚马逊云科技已开源 Dogwood，这是一种扩展 Cedar 的策略语言，通过引入时间条件来管理 AI 智能体的工具调用。该项目采用 Apache 2.0 许可证发布。 Dogwood 解决了 AI 智能体工具调用中日益突出的问题——调用在技术上合法但语义上错误，例如未经事先授权就执行退款。它为开发者提供了一种可编程的方式，在整个智能体工作流中强制执行规则、审批和约束，这在 AI 智能体越来越多地连接企业 API 和外部工具的背景下至关重要。 Dogwood 基于 Cedar 构建，Cedar 是亚马逊云科技于 2025 年底捐赠给 CNCF 的一个开源授权语言沙箱项目。其关键创新是加入时间条件，使策略能够基于智能体此前的工具调用历史进行推理，而不是孤立地评估每个请求。

rss · InfoQ 中文站 · 8月23日 17:00

**背景**: AI 智能体依靠工具调用与外部系统交互，但随着它们连接越来越多的 API 和 schema，权限管理变得越来越复杂。传统的授权检查通常独立处理每个请求，无法捕捉多步骤滥用或依赖上下文的错误。Dogwood 旨在通过提供一种理解工具调用序列和意图的策略语言来填补这一空白，让开发者对智能体行为拥有更细粒度的控制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.infoq.com/news/2026/08/aws-dogwood-agent-policy/">AWS Open - Sources Dogwood , Extending Cedar to Govern... - InfoQ</a></li>
<li><a href="https://thenewstack.io/aws-dogwood-agent-policies/">Your AI agent’s next tool call may be valid but wrong. AWS 's Dogwood ...</a></li>
<li><a href="https://techstrong.ai/articles/aws-open-sources-dogwood-language-for-programmatically-governing-ai-agents/">AWS Open Sources Dogwood Language for... - Techstrong.ai</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#Tool calling`, `#Open source`, `#AWS`, `#Software engineering`

---