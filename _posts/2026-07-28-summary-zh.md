---
layout: default
title: "Horizon Summary: 2026-07-28 (ZH)"
date: 2026-07-28
lang: zh
---

> 从 45 条内容中筛选出 10 条重要资讯。

---

1. [月之暗面开源 Kimi K3：2.8 万亿参数](#item-1) ⭐️ 9.0/10
2. [Anthropic 阐明对开源权重模型的立场](#item-2) ⭐️ 8.0/10
3. [快手大规模从 ClickHouse 迁移至 Apache Doris](#item-3) ⭐️ 8.0/10
4. [RSPack 2.0 发布：ESM 核心与性能提升](#item-4) ⭐️ 8.0/10
5. [Cursor AI 智能体仅凭手册重建 SQLite](#item-5) ⭐️ 8.0/10
6. [AWS 发布 Loom：面向企业级 AI 代理的开源平台](#item-6) ⭐️ 8.0/10
7. [中国启动国产 DUV 光刻机量产](#item-7) ⭐️ 8.0/10
8. [Agentic AI 将基础设施焦点从 Token 转向任务](#item-8) ⭐️ 7.0/10
9. [版本控制 SQL 数据库 Dolt 发布 2.0 版](#item-9) ⭐️ 7.0/10
10. [AMD 发布全球首款 2nm GPU，获巨头力挺](#item-10) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [月之暗面开源 Kimi K3：2.8 万亿参数](https://huggingface.co/moonshotai/Kimi-K3) ⭐️ 9.0/10

月之暗面开源了 Kimi K3，这是首个公开的 2.8 万亿总参数模型，激活参数为 1040 亿，采用了新颖的 Kimi Delta Attention（KDA）和 Attention Residuals（AttnRes）架构。 此次发布是开源 AI 的一个重要里程碑，它提供了一个超过 2 万亿参数的模型，此前这仅能从专有系统中获得，并且它在性能上与 GPT-5.6 和 Claude Fable 5 等前沿模型不相上下。 Kimi K3 采用混合专家（MoE）架构，包含 896 个专家，每个 token 激活 16 个，支持多模态输入（文本、图像、视频），上下文窗口达 100 万 token。它在微调阶段就采用 MXFP4 量化感知训练以实现高效推理。

telegram · zaihuapd · 7月27日 15:15

**背景**: 拥有万亿参数的大型语言模型通常需要巨大的计算资源，且很少开源。Kimi K3 的 KDA 是一种线性注意力机制，能够高效扩展至长上下文；而 AttnRes 用自适应的基于注意力的跳跃连接取代了传统的残差连接，改善了深层网络中的信息流动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2603.15031">Attention Residuals</a></li>
<li><a href="https://www.emergentmind.com/topics/kimi-delta-attention-kda">Kimi Delta Attention: Efficient Long-Context Models</a></li>

</ul>
</details>

**标签**: `#AI`, `#open-source`, `#large language model`, `#Moonshot AI`, `#Kimi K3`

---

<a id="item-2"></a>
## [Anthropic 阐明对开源权重模型的立场](https://www.anthropic.com/news/position-open-weights-models) ⭐️ 8.0/10

Anthropic 发布政策声明，澄清其不主张禁止开源权重模型，而是支持对所有足够强大的模型（无论是开源还是闭源）进行强制安全测试。 这一声明涉及 AI 监管的关键辩论，因为开源权重模型可提供广泛访问但也带来滥用风险。Anthropic 的立场可能影响未来的政策和行业实践。 Anthropic 明确表示从未呼吁禁止开源权重模型，但批评者认为，如果测试成本高昂或受限，强制测试要求可能实际上等同于禁令。该公司还支持对华芯片销售禁令等措施，有些人认为这与其立场矛盾。

hackernews · surprisetalk · 7月27日 22:03 · [社区讨论](https://news.ycombinator.com/item?id=49076057)

**背景**: 开源权重模型是指公开发布训练后参数（权重）的 AI 模型，使任何人都可以运行、微调或在此基础上构建。这与包括训练代码和数据的完全开源模型不同。争论焦点在于如何平衡创新所需的开放性和安全风险（如被用于有害目的）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.analyticsvidhya.com/blog/2025/04/open-weight-models/">What are Open Source and Open Weight Models ? | Analytics Vidhya</a></li>

</ul>
</details>

**社区讨论**: 评论者强烈批评 Anthropic 的立场，认为强制安全测试实际上等同于对开源权重模型的禁令，因为可能存在成本和访问障碍。有人指出其矛盾之处，例如 Anthropic 支持芯片禁令却声称不支持禁令。还有人指责该公司是为了保护自身商业利益而进行作秀。

**标签**: `#AI Safety`, `#Open Source`, `#Regulation`, `#Anthropic`, `#AI Policy`

---

<a id="item-3"></a>
## [快手大规模从 ClickHouse 迁移至 Apache Doris](https://www.infoq.cn/article/1YYoykV4gk0eRGE5HpTO?utm_source=rss&utm_medium=article) ⭐️ 8.0/10

快手完成从 ClickHouse 到 Apache Doris 的大规模迁移，涉及数百 PB 数据和超过 200 个集群。 这一案例展示了 Apache Doris 处理海量数据和复杂工作负载的能力，为大规模实时分析提供了 ClickHouse 之外的可行选择，可能影响业界对 Apache Doris 作为下一代 OLAP 引擎的采用。 迁移涉及数百 PB 数据和超过 200 个集群，体现了此次迁移的规模和复杂性。文章详细介绍了迁移过程中的技术挑战和解决方案。

rss · InfoQ 中文站 · 7月27日 16:55

**背景**: ClickHouse 和 Apache Doris 都是流行的开源列式存储数据库，常用于实时分析。ClickHouse 以单表查询的高性能著称，而 Apache Doris 在多表连接和数据更新操作方面表现更优。快手作为中国主要的短视频平台，之前依赖 ClickHouse 进行数据分析，但面临可扩展性和维护方面的挑战。

**标签**: `#ClickHouse`, `#Apache Doris`, `#Big Data`, `#Migration`, `#Data Engineering`

---

<a id="item-4"></a>
## [RSPack 2.0 发布：ESM 核心与性能提升](https://www.infoq.cn/article/Pl99PqDrDO6abAIlm1jp?utm_source=rss&utm_medium=article) ⭐️ 8.0/10

RSPack 2.0 正式发布，引入了新的 ESM 核心、更精简的依赖项以及更快的构建性能。这一重大版本更新标志着这个基于 Rust 的 JavaScript 打包工具迈出了重要一步。 作为一款用 Rust 编写且兼容 webpack 的打包工具，RSPack 2.0 的性能提升和 ESM 核心使其成为大型 JavaScript 项目的有力替代方案，有望大幅缩短构建时间。这一版本可能会加速开发者在寻找更快速、更现代的打包解决方案时的采用。 ESM（ES 模块）核心原生支持现代 JavaScript 模块语法，而更精简的依赖项则减少了包体积和安装开销。公告中未提供具体的基准测试数据或迁移指南。

rss · InfoQ 中文站 · 7月27日 15:56

**背景**: Rspack 是一款用 Rust 编写的高性能 JavaScript 打包工具，旨在作为 webpack 的即插即用替代品，提供兼容的 API。它的目标是在保持熟悉的 webpack 生态系统的同时，显著缩短构建时间。像 webpack 和 Rspack 这样的打包工具将多个 JavaScript 文件及依赖项合并成优化后的浏览器可运行包。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rspack.rs/">Rspack</a></li>
<li><a href="https://blog.appsignal.com/2025/04/16/an-introduction-to-javascript-bundler-rspack.html">An Introduction to JavaScript Bundler Rspack | AppSignal Blog</a></li>
<li><a href="https://betterstack.com/community/guides/scaling-nodejs/rspack-explained/">Getting Started with Rspack | Better Stack Community</a></li>

</ul>
</details>

**标签**: `#RSPack`, `#bundler`, `#JavaScript`, `#performance`, `#ESM`

---

<a id="item-5"></a>
## [Cursor AI 智能体仅凭手册重建 SQLite](https://www.infoq.cn/article/5qw8Qe37kGVDq9Yy57XC?utm_source=rss&utm_medium=article) ⭐️ 8.0/10

Cursor 的 AI 智能体系统仅凭 SQLite 的 835 页技术手册，在无源码、无测试集、无网络的情况下成功重建了该数据库引擎。 这一成就表明 AI 智能体能够仅靠文档自主复现复杂软件，可能将彻底改变软件维护、迁移和恢复工作。 该多智能体系统自主规划并编写代码，重建的 SQLite 通过了官方测试套件，证明了与原始版本的功能等价性。

rss · InfoQ 中文站 · 7月27日 09:34

**背景**: SQLite 是一个广泛使用的嵌入式数据库引擎。Cursor 是一个支持自主编码智能体的 AI 代码编辑器。该实验展示了 AI 仅凭规格文档理解并复现软件的能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cursor.com/product">Cursor — Build Software with AI Agents</a></li>
<li><a href="https://cursor.com/agents">Agents | Cursor - The AI Code Editor</a></li>
<li><a href="https://medium.com/@dave-patten/the-state-of-ai-coding-agents-2026-from-pair-programming-to-autonomous-ai-teams-b11f2b39232a">The State of AI Coding Agents (2026): From Pair Programming to Autonomous AI Teams | by Dave Patten | Medium</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#SQLite`, `#software engineering`, `#automated development`, `#Cursor`

---

<a id="item-6"></a>
## [AWS 发布 Loom：面向企业级 AI 代理的开源平台](https://www.infoq.cn/article/JDgONrm19ROF1qHzfOQO?utm_source=rss&utm_medium=article) ⭐️ 8.0/10

亚马逊云科技宣布推出 Loom，这是一个开源参考平台，用于在企业级规模上构建、部署和管理 AI 代理。该平台基于 Strands Agents SDK 构建，并利用 Amazon Bedrock 和 AgentCore 等 AWS 托管服务。 Loom 回应了企业安全、大规模管理 AI 代理的日益增长的需求，提供了内置的治理、身份验证和生命周期管理。随着 AI 代理日益普及，像 Loom 这样的平台可以通过简化运维复杂性来加速其采用。 Loom 包含一个统一的管理 UI，支持基于 Cognito 的身份验证、基于作用域的授权，以及代理记忆、MCP 服务器、A2A 集成和 AWS Agent Registry。它是一个有主见的平台，意味着它提供了一种预设的代理构建方式，同时隐藏了底层实现细节。

rss · InfoQ 中文站 · 7月27日 09:24

**背景**: AI 代理是能够自主执行任务、做出决策并代表用户与系统交互的软件实体。在企业规模上管理它们需要强大的安全、治理和基础设施编排能力。Loom 是一个开源参考实现，展示了如何在 AWS 上利用最佳实践来实现这一目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aws.amazon.com/blogs/opensource/building-secure-ai-agents-at-scale-introducing-loom-for-aws/">Building secure AI agents at scale: Introducing Loom for AWS</a></li>
<li><a href="https://github.com/awslabs/loom/">GitHub - awslabs/loom: Loom for AWS is an enterprise-grade platform for ...</a></li>
<li><a href="https://www.infoq.com/news/2026/07/loom-aws-agent-platform/">AWS Releases Loom, an Open-Source Reference Platform for ... - InfoQ</a></li>

</ul>
</details>

**标签**: `#AWS`, `#AI agents`, `#open-source`, `#enterprise`, `#AI management`

---

<a id="item-7"></a>
## [中国启动国产 DUV 光刻机量产](https://www.theinformation.com/articles/china-starts-mass-producing-homegrown-duv-chipmaking-tools-advance-local-chip-industry) ⭐️ 8.0/10

中国已开始大规模生产自主研发的浸没式深紫外（DUV）光刻机，计划今年生产约 5 台，2027 年约 20 台，将交付给中芯国际、华虹半导体等国内芯片制造商。 这标志着中国推动半导体自给自足的重要里程碑，可能减少对 ASML 的依赖并重塑全球光刻市场，但该设备目前在性能和可靠性上仍落后于 ASML。 国产 DUV 光刻机主要使用国产零部件，但部分关键部件仍来自日本，今年本地供应链延误已影响进度；芯片制造商需数月时间测试精度和兼容性才能投入量产。

telegram · zaihuapd · 7月27日 14:10

**背景**: 深紫外（DUV）光刻使用波长为 365、248 或 193 纳米的光在晶圆上刻印电路。浸没式光刻通过在镜头和晶圆之间放置液体来提高分辨率。ASML 目前主导 DUV 和 EUV 光刻市场。中国在出口限制背景下一直致力于开发国产替代品。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Extreme_ultraviolet_lithography">Extreme ultraviolet lithography</a></li>
<li><a href="https://www.asml.com/en/products/duv-lithography-systems">See ASML's DUV lithography systems</a></li>
<li><a href="https://en.wikipedia.org/wiki/Immersion_lithography">Immersion lithography - Wikipedia</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#lithography`, `#ASML`, `#China`, `#chip manufacturing`

---

<a id="item-8"></a>
## [Agentic AI 将基础设施焦点从 Token 转向任务](https://www.infoq.cn/article/vhx0VYNXpieSIuq0YIR6?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

InfoQ 的这篇文章探讨了 Agentic AI 的兴起如何改变基础设施的优先事项，从优化 Token 吞吐量转向关注任务执行与编排。 随着 AI 代理变得更加自主和面向任务，基础设施必须适应支持长期运行的多步骤工作流，而非简单的请求-响应模式，这将影响云架构、资源分配和系统设计。 文章认为，像每秒 Token 数这样的传统基础设施指标变得不那么重要，取而代之的是任务完成时间、可靠性和每任务成本。它强调需要新的可观测性和编排工具。

rss · InfoQ 中文站 · 7月27日 16:51

**背景**: Agentic AI 是指能够在多个步骤中自主追求目标，无需每步人工批准的 AI 系统。与响应单一提示的传统聊天机器人不同，Agentic AI 可以独立规划、推理和执行任务。这种转变要求基础设施处理持久状态、调度和跨长期运行的代理交互的错误恢复。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lilys.ai/en/notes/agentic-ai-20251022/agentic-ai-explained-simply">Agentic AI explained in a way anyone can understand!</a></li>
<li><a href="https://remolda.com/en/glossary/agentic-ai">Agentic AI — definition | Remolda</a></li>

</ul>
</details>

**标签**: `#Agentic AI`, `#infrastructure`, `#AI agents`, `#technology trends`

---

<a id="item-9"></a>
## [版本控制 SQL 数据库 Dolt 发布 2.0 版](https://www.infoq.cn/article/NiKzwp2aEJFJvJqR5ybt?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

版本控制 SQL 数据库 Dolt 2.0 发布，新增自动存储清理和压缩功能，提高了数据管理效率。 此次发布减少了依赖 Dolt 进行版本控制数据的用户的手动维护工作，使存储增长管理更轻松，并提升了数据密集型应用的性能。 自动存储清理功能可能包括对未引用数据的垃圾回收，而压缩则减少磁盘占用。这些改进提升了 Dolt 部署的可扩展性和成本效益。

rss · InfoQ 中文站 · 7月27日 11:08

**背景**: Dolt 是一个版本控制 SQL 数据库，像 Git 管理代码一样管理数据，支持分支、合并和历史追踪。它兼容 MySQL 查询，用于可复现的数据分析和协作式数据管理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.dolthub.com/docs/introduction/what-is-dolt/">What is Dolt ? | Dolt Docs</a></li>
<li><a href="https://github.com/dolthub/dolt">GitHub - dolthub/ dolt : Dolt – Git for Data · GitHub</a></li>
<li><a href="https://medium.com/@adai_9636/dolt-a-version-controlled-sql-database-tool-2ea49d73a0b8">Dolt : A version - controlled SQL database tool | by Athena | Medium</a></li>

</ul>
</details>

**标签**: `#Dolt`, `#SQL`, `#version control`, `#database`, `#open source`

---

<a id="item-10"></a>
## [AMD 发布全球首款 2nm GPU，获巨头力挺](https://www.infoq.cn/article/SJj23gRv7ZXBHyaCi8Eq?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

AMD 发布了基于台积电 2nm 工艺、采用 CDNA 5 架构的 Instinct MI455X GPU，拥有 3200 亿个晶体管和 432 GB 的 HBM4 内存。 这标志着 AI 硬件的重大飞跃，直接挑战 NVIDIA 在数据中心 GPU 市场的主导地位，并获得了 OpenAI、Meta 和微软的支持。 该 GPU 采用多芯片封装，结合了 2nm 和 3nm 工艺节点，其 3200 亿个晶体管接近 NVIDIA 即将推出的 Rubin 芯片（3360 亿个）。

rss · InfoQ 中文站 · 7月27日 09:57

**背景**: 2nm 工艺节点是继 3nm 之后的新一代制程，提供更高的密度和能效。AMD 的 CDNA 架构专为 AI 和高性能计算设计，而 NVIDIA 目前凭借其 Hopper 和 Blackwell GPU 在市场上领先。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/2_nm_process">2 nm process - Wikipedia</a></li>
<li><a href="https://www.techpowerup.com/351006/amd-instinct-mi400-series-and-helios-rack-debut-cdna-5-goes-2-nm-plus-rocm-ai-and-gorgon-halo">AMD Instinct MI400 Series and Helios Rack Debut... | TechPowerUp</a></li>
<li><a href="https://wccftech.com/amd-instinct-mi455x-gpu-320b-behemoth-tackle-nvidia-rubin-with-432gb-hbm4-40-pflops-ai/">AMD Unleashes Instinct MI455X GPU , A 320 Billion Transistor...</a></li>

</ul>
</details>

**标签**: `#AMD`, `#2nm GPU`, `#NVIDIA`, `#芯片`, `#AI硬件`

---