---
layout: default
title: "Horizon Summary: 2026-07-21 (ZH)"
date: 2026-07-21
lang: zh
---

> 从 48 条内容中筛选出 10 条重要资讯。

---

1. [AI 在寻找反例上超越人类数学家](#item-1) ⭐️ 9.0/10
2. [黑客清空罗马尼亚土地登记数据库](#item-2) ⭐️ 9.0/10
3. [OpenAI 分享长期 AI 模型的安全经验](#item-3) ⭐️ 9.0/10
4. [Fastjson 1.x 曝无依赖高危 RCE 漏洞](#item-4) ⭐️ 9.0/10
5. [中国开源 AI 模型威胁美国实验室溢价定价](#item-5) ⭐️ 8.0/10
6. [欧盟拟共享公民生物识别数据换取美国免签待遇](#item-6) ⭐️ 8.0/10
7. [智谱建成全国产芯片数据中心](#item-7) ⭐️ 8.0/10
8. [摩尔线程用国产 GPU 训练出世界模型，标志里程碑](#item-8) ⭐️ 7.0/10
9. [无问芯穹：智能基础设施对跨世界 AI 生产力至关重要](#item-9) ⭐️ 7.0/10
10. [AWS 详解客户将 Lambda 函数扩展至 100 万](#item-10) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [AI 在寻找反例上超越人类数学家](https://xenaproject.wordpress.com/2026/07/20/human-mathematicians-are-being-outcounterexampled/) ⭐️ 9.0/10

据 Xenaproject 博客文章讨论，AI 工具在生成数学猜想的反例方面比人类数学家更快更有效。 这标志着数学研究范式转变，可能通过快速证伪错误猜想节省数学家时间，将精力转向更有成效的领域。 博文提到一些研究生每月支付 200 美元使用 Sol 和 Fable 等 AI 模型，凸显数学领域对 AI 的依赖日益增加。

hackernews · artninja1988 · 7月20日 19:03 · [社区讨论](https://news.ycombinator.com/item?id=48983382)

**背景**: 反例是证伪数学猜想的特例，常对研究起指导作用。AI 近期在纽结理论和抽象代数等领域展现了发现反例的能力，挑战了传统由人类主导的发现过程。

**社区讨论**: 评论者反应不一：有人视 AI 为提高生产率的工具，可避免徒劳；有人担忧人类在数学中的角色，并提及如张益唐因错误推论而职业受挫的警示故事。

**标签**: `#AI`, `#mathematics`, `#machine learning`, `#research`, `#automation`

---

<a id="item-2"></a>
## [黑客清空罗马尼亚土地登记数据库](https://news.risky.biz/risky-bulletin-hacker-wipes-romanias-entire-land-registry-database/) ⭐️ 9.0/10

一名黑客入侵罗马尼亚土地登记机构，清空了整个数据库。官员们利用离线备份恢复了基本服务，并正在从头重建网络。 此次针对国家关键基础设施的攻击本可能导致土地所有权无法证明，造成大规模社会混乱。幸有离线备份避免长期危机，但事件凸显了政府 IT 安全漏洞。 黑客使用擦除恶意软件删除了主数据和备份数据，但机构另有一份离线物理备份。目前正在向罗马尼亚政府云迁移，由特种电信服务局（STS）协调。

hackernews · speckx · 7月20日 13:28 · [社区讨论](https://news.ycombinator.com/item?id=48978605)

**背景**: 擦除恶意软件是一种破坏性恶意软件，旨在从受感染系统中擦除数据，常被用于定向攻击。数据库备份恢复是一种标准灾难恢复实践，将数据副本分开存储，以便在数据丢失后恢复。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Wiper_(malware)">Wiper (malware) - Wikipedia</a></li>
<li><a href="https://learn.microsoft.com/en-us/sql/relational-databases/backup-restore/restore-a-database-backup-using-ssms?view=sql-server-ver17">Restore a Database Backup Using SSMS - SQL Server | Microsoft Learn</a></li>

</ul>
</details>

**社区讨论**: 评论指出离线备份的存在减轻了损害，并称赞恢复工作。一些罗马尼亚用户将此事件归咎于政府 IT 合同中的腐败，其他人则确认黑客是来自阿尔及利亚的 Zakaria Mahdjoub，并指出存在引渡条约。

**标签**: `#cybersecurity`, `#cyberattack`, `#land registry`, `#Romania`, `#data breach`

---

<a id="item-3"></a>
## [OpenAI 分享长期 AI 模型的安全经验](https://openai.com/index/safety-alignment-long-horizon-models) ⭐️ 9.0/10

OpenAI 发布了一篇博文，详细介绍了在部署长时间运行的 AI 模型时观察到的新安全风险和改进的保障措施，并强调了对齐面临的挑战。 长期模型在生产中使用日益广泛，这份指南有助于开发者预见故障并改进安全实践，从而影响更广泛的 AI 生态系统。 该博文涵盖了观察到的故障，如目标漂移和遗忘，并描述了改进的监控和干预技术，以在长时间任务中保持对齐。

rss · OpenAI Blog · 7月20日 10:00

**背景**: 长期模型是追求数天或数月复杂目标的 AI 系统，需要数千个中间步骤。由于它们长时间自主运行，传统的对齐方法效果较差，因此带来了独特的安全风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://jumpcloud.com/it-index/what-is-long-horizon-planning-in-ai">What Is Long-Horizon Planning in AI? - JumpCloud</a></li>
<li><a href="https://www.epam.com/insights/ai/blogs/how-to-use-long-horizon-agents-in-production">Long-horizon agents explained: Hype, reality, engineering lessons, and how to use AI agents in production</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#alignment`, `#long-horizon models`, `#deployment`

---

<a id="item-4"></a>
## [Fastjson 1.x 曝无依赖高危 RCE 漏洞](https://x.com/k_firsov/status/2078872293745570032) ⭐️ 9.0/10

安全研究人员 Kirill Firsov 披露，Fastjson 1.2.68 至 1.2.83 版本存在高危远程代码执行漏洞，该漏洞无需开启 autoType 支持，也无需依赖 classpath 中的任意 gadget，且可在 JDK 8、17 和 21 上利用。 该漏洞严重性极高，因为 Fastjson 1.x 已停止维护且官方大概率不会发布补丁，但它仍被广泛使用。由于利用无需特殊配置，大量现有应用面临风险，开发者必须立即升级到 Fastjson2 或启用 SafeMode。 该漏洞影响 Fastjson 1.x 的 1.2.68 至 1.2.83 版本，在 JDK 8、17 和 21 上均可成功利用，无需开启 autoType 或依赖任何外部 gadget 链。唯一的缓解措施是升级到 Fastjson2，或通过 JVM 启动参数或配置文件启用 SafeMode。

telegram · zaihuapd · 7月20日 14:32

**背景**: Fastjson 是阿里巴巴开发的 Java 流行 JSON 解析库。其 autoType 功能可自动反序列化 JSON 为指定 Java 类型，历史上曾通过 gadget 链被利用实现远程代码执行。SafeMode 自 1.2.68 版本引入，彻底禁用 autoType 以防止此类攻击。然而，此次披露的漏洞无需 autoType 和 gadget 即可利用，使其尤为危险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/alibaba/fastjson/wiki/fastjson_safemode">fastjson_safemode · alibaba/fastjson Wiki</a></li>
<li><a href="https://github.com/alibaba/fastjson/wiki/enable_autotype">enable_autotype · alibaba/fastjson Wiki · GitHub</a></li>
<li><a href="https://portswigger.net/web-security/deserialization/exploiting/lab-deserialization-developing-a-custom-gadget-chain-for-java-deserialization">Lab: Developing a custom gadget chain for Java deserialization | Web Security Academy</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#RCE`, `#fastjson`, `#remote-code-execution`

---

<a id="item-5"></a>
## [中国开源 AI 模型威胁美国实验室溢价定价](https://stratechery.com/2026/whos-afraid-of-chinese-models/) ⭐️ 8.0/10

阿里巴巴（通义千问）和深度求索等中国 AI 实验室免费发布高质量开源模型，直接挑战 OpenAI 和 Anthropic 等美国实验室的 API 溢价定价策略。 这威胁到美国 AI 实验室的巨额估值——Anthropic 估值 1.2 万亿美元、OpenAI 目标 8500 亿美元，这些估值建立在 API 高利润收入的预期之上。开源竞争可能迫使降价，重塑 AI 行业的经济格局。 DeepSeek-V3 是一个 6710 亿参数的混合专家模型，每个 token 激活 370 亿参数，采用多头潜在注意力等高效架构。Qwen 模型基于 Llama 架构，提供从 18 亿到 720 亿参数的不同尺寸。

hackernews · mfiguiere · 7月20日 11:05 · [社区讨论](https://news.ycombinator.com/item?id=48977128)

**背景**: 美国前沿 AI 实验室如 OpenAI 和 Anthropic 以天价估值融资数百亿美元，押注其专有模型能维持溢价定价。与此同时，中国 AI 实验室——由科技巨头或对冲基金支持——不断发布强大的开源模型，通常以极低的成本匹配或接近美国前沿性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>
<li><a href="https://github.com/deepseek-ai/deepseek-v3">GitHub - deepseek-ai/DeepSeek-V3 · GitHub</a></li>

</ul>
</details>

**社区讨论**: 社区评论指出 VC 担心中国开源模型导致估值崩溃，用户注意到编程助手之间的切换成本很低，并对中国数据中心表示担忧。有人主张美国立法明确允许模型蒸馏作为合理使用。

**标签**: `#Chinese AI`, `#open-source models`, `#AI industry`, `#valuation`, `#competition`

---

<a id="item-6"></a>
## [欧盟拟共享公民生物识别数据换取美国免签待遇](https://edri.org/our-work/the-eu-is-about-to-sell-our-most-sensitive-data-to-the-us-for-visa-free-travel/) ⭐️ 8.0/10

欧盟委员会正与美国特朗普政府谈判一项“增强边境安全伙伴关系”（EBSP）协议，该协议将要求欧盟成员国向美国当局传输公民的生物识别数据和风险指标，以换取美国公民的免签旅行。 该协议将为大规模监控和数据共享开创危险先例，可能压制政治异议和人权活动。它可能削弱欧盟的数据保护标准，并将敏感信息暴露给美国安全机构。 根据 EDRi 引用的泄露草案，欧盟基本接受了美方对生物识别数据库的无限制访问以及基于政治观点的“风险指标”自动交换的要求。该协议涵盖所有旅客，而不仅仅是签证申请人。

telegram · zaihuapd · 7月20日 15:08

**背景**: 增强边境安全伙伴关系（EBSP）是美国为扩大与伙伴国家的信息共享以加强边境安全而建立的框架，包括生物识别数据交换。美国的免签证计划（VWP）允许特定国家公民无需签证即可赴美旅行，但要求互惠安全协议。欧盟目前参与 VWP，但美国正寻求在 EBSP 下加强数据共享作为继续免签的条件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:52025PC0447">Enhanced Border Security Partnership - EUR-Lex</a></li>
<li><a href="https://edri.org/our-work/usa-border-plan-requires-continuous-and-systematic-transfers-of-biometric-data/">The new USA border plan - European Digital Rights (EDRi)</a></li>

</ul>
</details>

**标签**: `#privacy`, `#biometric data`, `#EU-US relations`, `#data protection`, `#surveillance`

---

<a id="item-7"></a>
## [智谱建成全国产芯片数据中心](https://www.bloomberg.com/news/articles/2026-07-20/z-ai-completes-giant-data-center-with-chinese-chips-to-train-ai) ⭐️ 8.0/10

智谱 AI 已完成一座功率达 1 吉瓦、全部采用国产芯片的数据中心，并已部分投入运营，用于支持其 GLM 平台的训练。 这一里程碑表明中国在 AI 芯片自给自足方面取得进展，在美国出口管制下减少了对受控硬件的依赖。同时，该中心能够支持中国领先的开源大模型家族 GLM 的大规模训练。 该数据中心功率容量达 1 吉瓦，足以为约 75 万户家庭供电，是中国 AI 实验室建造的最大规模设施之一。智谱 AI 运营着多个各拥有超万枚芯片的计算集群。

telegram · zaihuapd · 7月20日 15:43

**背景**: 大多数先进 AI 芯片，如 NVIDIA 的数据中心 GPU，受美国出口管制，无法合法销往中国。作为回应，中国企业加速开发国产替代芯片，这些芯片通常基于 14nm–28nm 工艺。智谱 AI 的 GLM（通用语言模型）是开源大语言模型家族，其中 GLM-5 是一个 7450 亿参数的尖端模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Z.ai">Z. ai - Wikipedia</a></li>
<li><a href="https://www.fobsourcify.com/what-companies-could-develop-ai-chips-in-china/">Sourcing What Companies Could Develop Ai Chips In China from...</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#domestic chips`, `#China`, `#GLM`, `#data center`

---

<a id="item-8"></a>
## [摩尔线程用国产 GPU 训练出世界模型，标志里程碑](https://www.infoq.cn/article/01aguG1Yrgxl0bpmfZps?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

摩尔线程声称已使用其国产 GPU 成功训练出一个世界模型，这是中国 GPU 公司的首次。 这一成就可能标志着国产 GPU 在 AI 负载方面迈出了重大一步，挑战英伟达在中国 AI 基础设施中的主导地位。 世界模型是一种 AI 系统，通过学习环境的内部表示来预测动态，比典型的分类或生成任务更复杂。

rss · InfoQ 中文站 · 7月20日 19:51

**背景**: AI 中的世界模型是一种机器学习系统，它从视频等数据中构建环境的内部表示，并预测其随时间的变化。这种能力对机器人、自动驾驶和视频生成的自主决策至关重要。摩尔线程是一家成立于 2020 年的中国 GPU 初创公司，定位为英伟达在 AI 训练和图形工作负载方面的国内替代品。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/World_model_(artificial_intelligence)">World model (artificial intelligence)</a></li>
<li><a href="https://en.mthreads.com/">Moore Threads | Accelerate Computing for the Future</a></li>
<li><a href="https://web3.bitget.cloud/en/academy/what-is-moore-threads-and-why-china-thinks-it-could-be-the-next-nvidia">What Is Moore Threads and Why China Thinks It Could Be the Next...</a></li>

</ul>
</details>

**标签**: `#GPU`, `#AI`, `#Chinese tech`, `#world model`

---

<a id="item-9"></a>
## [无问芯穹：智能基础设施对跨世界 AI 生产力至关重要](https://www.infoq.cn/article/AWhEVVgvNquuiKZdRQ0H?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

在 InfoQ 的一篇最新文章中，无问芯穹的夏立雪提出，智能基础设施（Agentic Infra）对于数字世界和物理世界中所有 AI 生产力都不可或缺，是自主 AI 代理安全高效运行的基础层。 随着 AI 代理变得越来越自主和普及，拥有用于权限、记忆、工作流和审计线索的强大基础设施对于确保实际部署中的安全性和可靠性至关重要。这一观点突出了 AI 栈中的一个关键新兴层，企业和开发者需要予以考虑。 智能基础设施的概念包括事件驱动执行、挂起/恢复能力以及按使用付费的成本模型，而非始终在线的服务器。这篇评论文章未提供技术实现细节，而是呼吁关注面向代理型 AI 工作负载的基础设施。

rss · InfoQ 中文站 · 7月20日 16:41

**背景**: 智能基础设施指的是使 AI 代理能在企业或环境中自主行动的基础系统层。它包括权限、记忆、工作流、审批和审计追踪，旨在通过事件驱动和成本高效的架构高效处理代理工作负载。随着 AI 代理从简单聊天机器人发展为自主行动者，专门的基础设施对于安全管理其行为变得必要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://human-beyond.ai/concepts/agentic-infrastructure">What Is Agentic Infrastructure ? — Human Beyond</a></li>
<li><a href="https://arcoventure.studio/lexicon/agentic-infrastructure">Agentic Infrastructure — Built for Agent Workloads | Arco</a></li>
<li><a href="https://www.vaditaslim.com/blog/ai/agentic-infrastructure">Agentic Infrastructure : When AI Actually Does the Work | Vadi Taslim</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#agentic AI`, `#digital world`, `#physical world`, `#productivity`

---

<a id="item-10"></a>
## [AWS 详解客户将 Lambda 函数扩展至 100 万](https://www.infoq.cn/article/bkhkOrQYPuIN672g20hi?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

AWS 发布了一篇案例研究，详细介绍了某客户如何成功将其 AWS Lambda 函数扩展至 100 万并发执行，展示了极端的无服务器可扩展性。 这展示了无服务器计算的实际极限，为考虑大规模 Lambda 部署的企业提供了参考。它验证了在适当的设计模式下，无服务器架构可以处理巨大的工作负载。 该客户实现了 100 万 Lambda 函数的并发，这需要仔细管理扩展行为和并发配额。AWS Lambda 通过创建新的执行环境自动扩展，但必须考虑突发并发限制和账户配额。

rss · InfoQ 中文站 · 7月20日 15:17

**背景**: AWS Lambda 是一种无服务器计算服务，它根据事件运行代码并自动管理底层基础设施。它通过按需添加新实例进行扩展，但存在限制：默认情况下，AWS 账户有 1000 的区域并发限制，并且可以请求增加。该服务每分钟最多只能以 1000 个并发执行的速度扩展。本案例研究展示了客户如何在这些限制内和超越这些限制，实现了 100 万并发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.aws.amazon.com/lambda/latest/dg/scaling-behavior.html">Lambda scaling behavior - AWS Lambda</a></li>
<li><a href="https://dashbird.io/knowledge-base/basic-concepts/scalability/">Serverless Scalability : Overview | Knowledge Base | Dashbird</a></li>

</ul>
</details>

**标签**: `#AWS Lambda`, `#serverless`, `#scaling`, `#cloud computing`

---