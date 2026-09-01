---
layout: default
title: "Horizon Summary: 2026-09-01 (ZH)"
date: 2026-09-01
lang: zh
---

> 从 42 条内容中筛选出 10 条重要资讯。

---

**科技新闻**
1. [Bun 稳定版正式发布：延期六周，2900 个问题清零](#item-tech-news-1) ⭐️ 8.0/10
2. [OpenAI 将全面断供 Cursor：SpaceX 收购触发控制权条款](#item-tech-news-2) ⭐️ 7.0/10
3. [Kubeflow 扩展 AI 能力并接近 CNCF 毕业里程碑](#item-tech-news-3) ⭐️ 7.0/10
4. [Netflix 采用 Kueue 替代内部作业队列系统](#item-tech-news-4) ⭐️ 7.0/10
5. [LWiAI 播客第 255 期：Gemini 3.7、Qwen 3.8 与 AI 无人机](#item-tech-news-5) ⭐️ 7.0/10
6. [DLSS 5 视觉增强器：独立神经渲染工具](#item-tech-news-6) ⭐️ 7.0/10

**财经新闻**
1. [中国光伏装机首超煤电，成为第一大电源](#item-finance-news-1) ⭐️ 8.0/10
2. [高通上调芯片价格：9 月 1 日后出货产品涨幅两位数](#item-finance-news-2) ⭐️ 8.0/10
3. [迈阿密经济快速崛起，可持续性受关注](#item-finance-news-3) ⭐️ 6.0/10

**AI 创作者雷达**
1. [思科为 9 万员工部署个人 AI Agent，可跨系统代办事务](#item-ai-creator-1) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Bun 稳定版正式发布：延期六周，2900 个问题清零](https://www.infoq.cn/article/olsG3w9zkyKRqbQesB1g?utm_source=rss&amp;utm_medium=article) ⭐️ 8.0/10

JavaScript 运行时 Bun 的稳定版在跳票约六周后正式发布，开发团队表示此前积累的 2900 个问题已全部解决。此次发布意味着 Bun 从长期被戏称“烂代码”的开发阶段走向生产可用，为开发者提供更快速的脚本运行、打包与工具链能力。由于原始资料仅提供标题和概要，具体版本号、发布时间及兼容性细节尚未披露。对依赖 JavaScript 生态的开发者而言，这是一个值得关注的里程碑，但仍需结合官方文档进一步验证。

rss · InfoQ 中文站 · 8月31日 15:14

**「背景」** Bun 是由 Oven 团队开发的 JavaScript 运行时与工具链，使用 Zig 语言编写，旨在替代 Node.js，并内置打包器、测试运行器、包管理器等功能。该项目在稳定版发布之前多次跳票，最终在解决约 2900 个问题后正式落地；后续迭代中，1.3.1 版本曾被用户报告安装速度下降，而随后的更新又修复了 95 个问题，显示出项目仍处于持续修复阶段。

**「影响」** Bun 1.0 稳定版正式发布，使 JavaScript/TypeScript 开发者可以在生产环境中使用这一集运行时、打包器、测试运行器和 npm 兼容包管理器于一体的工具，从而减少对多个独立开发工具的依赖；该版本跳票约六周，团队在解决约 2900 个问题后才宣布稳定可用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bun.com/blog">Blog | Bun</a></li>
<li><a href="https://github.com/oven-sh/bun/issues/23969">Bun install slower than before · Issue #23969 · oven-sh/bun</a></li>
<li><a href="https://bun.sh/">Bun — A fast all-in-one JavaScript runtime</a></li>
<li><a href="https://dev.to/ervidaslaven/bun-10-the-swift-newcomer-in-the-javascript-ecosystem-3ol9">Bun 1.0: The Swift Newcomer in the JavaScript Ecosystem</a></li>
<li><a href="https://bun.com/blog/bun-v1.0">Bun 1.0 | Bun Blog</a></li>

</ul>
</details>

**标签**: `#bun`, `#javascript`, `#runtime`, `#release`, `#tooling`

---

<a id="item-tech-news-2"></a>
### [OpenAI 将全面断供 Cursor：SpaceX 收购触发控制权条款](https://www.infoq.cn/article/YiHrlKLX6I6IP92BgV7K?utm_source=rss&amp;utm_medium=article) ⭐️ 7.0/10

据 InfoQ 报道，OpenAI 将全面停止向 AI 代码编辑器 Cursor 提供服务，原因是 SpaceX 完成收购后触发了相关控制权条款。这一决定可能对依赖 Cursor 的开发者及 AI 编程工具生态产生重大影响，但由于原始报道缺少正文，具体断供时间、适用版本或替代方案等细节尚不明确。目前该消息仍属于初步报道，有待官方进一步确认。

rss · InfoQ 中文站 · 8月31日 14:16

**「背景」** Cursor 是一款 AI 代码编辑器，长期通过定制合同接入 OpenAI 的模型。SpaceX 于 2026 年 8 月 14 日以全股票交易完成对 Cursor 的收购，触发了 OpenAI 合同中的控制权变更条款。OpenAI 已通知 SpaceX 打算终止供货合同，拟议的断供日期为 2026 年 11 月 12 日；OpenAI 表示无法确信 SpaceX 会遵守其条款，并提及与马斯克旗下公司的过往纠纷。

**「影响」** Cursor 用户将从 2026 年 11 月 12 日起失去对 OpenAI 编码模型的访问，必须在到期前决定改用其他模型或更换编码平台；这一变化由 SpaceX 以 600 亿美元收购 Anysphere 触发，而非 Cursor 自身行为所致。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/our-decision-on-cursor-following-its-acquisition-by-spacex/">Our decision on Cursor following its acquisition by SpaceX | OpenAI</a></li>
<li><a href="https://www.cnbc.com/2026/08/29/openai-cursor-spacex-model-access.html">OpenAI to end model access to Cursor after acquisition by Elon Musk&#x27;s SpaceX</a></li>
<li><a href="https://cellcog.ai/blog/openai-pulls-models-from-cursor/">OpenAI Is Pulling Its Models From Cursor: What Actually Changes | CellCog</a></li>
<li><a href="https://dev.to/jamilxt/openai-is-cutting-off-cursor-the-ai-coding-lock-in-lesson-every-developer-needs-2617">OpenAI Is Cutting Off Cursor: The AI Coding Lock-In Lesson ...</a></li>
<li><a href="https://ai-herald.com/openai-cuts-cursor-off-after-spacex-acquisition/">OpenAI Cuts Cursor Off After SpaceX Acquisition – AI Herald</a></li>
<li><a href="https://www.cio.com/article/4216508/cursor-customers-will-lose-access-to-openai-coding-models-in-november-2.html">Cursor customers will lose access to OpenAI coding ... - CIO</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#Cursor`, `#AI code editor`, `#acquisition`, `#industry news`

---

<a id="item-tech-news-3"></a>
### [Kubeflow 扩展 AI 能力并接近 CNCF 毕业里程碑](https://www.infoq.cn/article/grb2X7v7fr6kUNuuRkvt?utm_source=rss&amp;utm_medium=article) ⭐️ 7.0/10

据 InfoQ 中文站报道，Kubeflow 宣布扩展了其 AI 功能，同时该项目正接近云原生计算基金会（CNCF）的毕业状态。作为运行在 Kubernetes 上的主流 MLOps 平台，这一进展对机器学习工作流的编排具有重要意义。不过，目前仅能依据标题确认这些消息，文章正文尚未提供具体的技术细节、版本信息或时间表。因此，关于新增 AI 功能的具体范围和 CNCF 毕业的正式时间仍有待原文进一步披露。

rss · InfoQ 中文站 · 8月31日 13:31

**「背景」** Kubeflow 是一个在 Kubernetes 上运行机器学习工作负载的开源 MLOps 平台，涵盖数据处理、模型训练、微调和推理等环节。CNCF 毕业（graduation）标志着项目在技术成熟度、治理和生态采用上达到了较高水平。Kubeflow 近期宣布了一系列技术更新，包括现代化的 SDK Kale 2.0、Notebooks v2，以及通过 CRD、OCI 和 OpenAI 兼容接口减少平台组件间定制集成的工作。不过，毕业并不代表所有能力都已完全成熟，Kale 和 Notebooks v2 仍需在不同组织的工作流中验证。

**「主要影响」** Kubeflow 获得 CNCF 毕业认证，标志着它成为 Kubernetes 上云原生 AI/机器学习运维的成熟生产级标准；同时，新推出的 Kale 2.0 SDK、原生 Spark 支持以及 Kubeflow Trainer 的扩展能力，将帮助用户在 Kubernetes 上更高效地运行分布式 AI 和高性能计算工作负载。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.infoq.com/news/2026/08/kubeflow/">Kubeflow Expands AI Capabilities as CNCF Graduation Nears</a></li>
<li><a href="https://www.cncf.io/announcements/2026/08/17/cncf-announces-kubeflows-graduation-solidifying-the-standard-for-cloud-native-ai-operations/">CNCF Announces Kubeflow’s Graduation, Solidifying a Standard ...</a></li>
<li><a href="https://cctest.ai/en/articles/kubeflow-broadens-cloud-native-ai-capabilities-as-cncf-graduation-nears">Kubeflow Expands Cloud-Native AI as CNCF Graduation Nears ...</a></li>
<li><a href="https://www.cncf.io/announcements/2026/08/17/cncf-announces-kubeflows-graduation-solidifying-the-standard-for-cloud-native-ai-operations/">CNCF Announces Kubeflow ’s Graduation , Solidifying... | CNCF</a></li>
<li><a href="https://www.infoq.com/news/2026/08/kubeflow/">Kubeflow Expands AI Capabilities as CNCF Graduation Nears - InfoQ</a></li>

</ul>
</details>

**标签**: `#Kubeflow`, `#CNCF`, `#MLOps`, `#Kubernetes`, `#AI`

---

<a id="item-tech-news-4"></a>
### [Netflix 采用 Kueue 替代内部作业队列系统](https://www.infoq.cn/article/d1qT2acYJodVCcKaBe4u?utm_source=rss&amp;utm_medium=article) ⭐️ 7.0/10

Netflix 正在采用云原生作业队列系统 Kueue 来替代其内部解决方案。Kueue 是 Kubernetes 原生的作业队列系统，提供配额管理与作业排队能力。Netflix 的采用表明其希望在统一作业调度方面提升资源利用率和可移植性。来源中未提供具体的迁移时间表、Kueue 版本或性能数据。这一采用对云原生和开源生态系统具有重要标志性意义。

rss · InfoQ 中文站 · 8月31日 12:00

**「背景信息」** Kueue 是一个开源的 Kubernetes 原生作业排队系统，用于管理批处理作业和配额。Netflix 此前使用的是 2018 年基于 Titus 构建的内部系统 Compute Managed Batch（CMB），随着业务发展，该内部方案已逐渐无法满足需求。此次迁移中，Netflix 将 CMB 的租户层级映射为 Kueue 的 Cohort、ClusterQueue 和 LocalQueue 资源，并保持 API 兼容，以降低对用户的影响。

**「影响」** 对于 Kubernetes 用户和云原生社区而言，Netflix 的采用验证了 Kueue 在生产环境中的可行性，可能推动更多企业评估和采用该开源系统。不过，由于来源缺乏详细证据，实际性能和迁移效果仍需进一步观察。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.infoq.com/news/2026/08/netflix-kueue-kubernetes-batch/">Netflix Adopts Cloud-Native Job Queueing System Kueue to ...</a></li>
<li><a href="https://daily.dev/posts/netflix-adopts-cloud-native-job-queueing-system-kueue-to-replace-an-in-house-solution-7gbkjcg1w">Netflix Adopts Cloud-Native Job Queueing System Kueue to...</a></li>

</ul>
</details>

**标签**: `#cloud-native`, `#Kubernetes`, `#job queue`, `#Netflix`, `#open source`

---

<a id="item-tech-news-5"></a>
### [LWiAI 播客第 255 期：Gemini 3.7、Qwen 3.8 与 AI 无人机](https://lastweekin.ai/p/lwiai-podcast-255-gemini-37-jalapeno) ⭐️ 7.0/10

《Last Week in AI》播客第 255 期集中讨论了多项重要 AI 进展：Google 发布了 Gemini 3.7 Flash，Jalapeño 的初步结果显示其速度处于行业领先水平，同时涉及 Qwen 3.8 的发布，以及一起完全由 AI 引导的无人机袭击造成三名乌克兰人死亡的事件。这期节目为听众梳理了最新模型发布与 AI 军事应用的现实案例，突出了生成式 AI 模型快速迭代及其在自主武器系统中的直接使用。节目名称与报道标题共同确认了这些话题，但具体版本细节和性能数据仍需以原始发布为准。

rss · Last Week in AI · 8月31日 08:20

**「背景信息」** Gemini 是 Google DeepMind 开发的多模态大语言模型家族，包括 Pro、Flash、Flash Lite 等版本，其中 Gemini 3.7 Flash 基于 Gemini 3.6 Flash，支持文本、图片、音频和视频输入，上下文窗口可达 100 万 tokens，并已用于 Google AI Pro 和 Ultra 订阅用户的 Gemini Spark 服务。Qwen 3.8-Max 是阿里巴巴在 2026 年 7 月预告、8 月 3 日发布的多模态基础模型，拥有 2.4 万亿总参数和 950 亿激活参数，支持 100 万上下文，按$2/$6 每百万 tokens 计费，并在开放权重版本发布前先行扩大使用范围。关于 Jalapeño，外部资料说法不一：有介绍称它是 OpenAI 与 Broadcom 合作的首款定制推理芯片，也有营销材料将其描述为 Solana 上的 AI 芯片代币，播客所称的“行业领先速度”应指其推理性能测试的初步结果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Google_Gemini_2.5_Flash_Image">Google Gemini 2.5 Flash Image</a></li>
<li><a href="https://deepmind.google/models/model-cards/gemini-3-7-flash/">Gemini 3 . 7 Flash - Model Card — Google DeepMind</a></li>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/">Gemini 3 . 7 Flash : our most intelligent workhorse model</a></li>
<li><a href="https://www.mindstudio.ai/blog/qwen-3-8-max-benchmarks-features">Qwen 3.8 Max Explained: Alibaba&#x27;s 2.4 Trillion Parameter Model | MindStudio</a></li>
<li><a href="https://www.yottalabs.ai/post/qwen-3-8-max-release-date-specs-how-to-access-2026">Qwen 3.8-Max: Specs, Pricing, Benchmark Status, and How to Access It (2026) | Yotta Labs</a></li>
<li><a href="https://www.scmp.com/tech/article/3362738/alibabas-ai-model-qwen38-max-made-widely-accessible-ahead-open-weights-release">Alibaba’s AI model Qwen3.8-Max made widely accessible ahead of open-weights release | South China Morning Post</a></li>
<li><a href="https://www.jalapenosol.com/">JALAPEÑO , The World&#x27;s First Spicy AI Chip</a></li>
<li><a href="https://www.linkedin.com/posts/entrepolish_openai-artificialintelligence-semiconductors-activity-7476191276149932032-M7Dd">OpenAI Unveils Jalapeño AI Chip for Efficient Inference | LinkedIn</a></li>

</ul>
</details>

**标签**: `#AI`, `#Gemini`, `#Qwen`, `#autonomous drones`, `#podcast`

---

<a id="item-tech-news-6"></a>
### [DLSS 5 视觉增强器：独立神经渲染工具](https://www.reddit.com/r/StableDiffusion/comments/1w3wuqu/dlss_5_visual_enhancer_standalone_neural/) ⭐️ 7.0/10

开发者 Merserk13 发布了独立 Windows 应用 DLSS 5 Visual Enhancer，将 DLSS 5 神经渲染的 feature-18 管线用于任意图片和视频，而不是仅限于游戏。它支持 DLAA/原始、1.5x、约 1.724x、2x 和 3x 模式，输出最高 8K，并提供神经预设及自然/电影风格，以及强度、局部色调、结构和皮肤结构控制。该工具支持批量图片处理和带前后对比预览，视频输出支持 H.264、HEVC、AV1 和 ProRes，并使用光流进行时间输入和场景切换重置。GPU 支持以 RTX 40/50 系列为主要目标，RTX 30 系列为较慢的测试路径；仓库包含应用/管线源码，但不重新分发所需的专有和第三方运行时二进制文件。这是一个独立的社区项目，与 NVIDIA、ReShade 或 RenoDX 无关联。

reddit · r/StableDiffusion · /u/Merserk13 · 9月1日 00:52

**「背景」** DLSS 5 是 NVIDIA 的神经渲染技术，通常需要借助 ReShade 与 RenoDX 插件在游戏内启用，通过神经网络对画面进行增强与超分辨率处理。社区也开发了类似 DLSS5-Feeder 的工具，将 DLSS 5 神经渲染引入未原生支持该功能的 DirectX 11/12 或 Vulkan 游戏。该项目则把这一通常用于游戏的渲染管线独立出来，用于处理任意图像和视频，因此需要依赖 ReShade/RenoDX 路径以及 RTX 40/50 系列 GPU 的神经渲染支持。

**「影响」** 对于拥有 RTX 40/50 系列显卡的 Windows 用户，现在可以将 DLSS 5 神经渲染应用于通用图片和视频的增强与超分；RTX 30 系列用户也可尝试，但性能较慢且处于测试阶段。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nexusmods.com/site/mods/2224">Applying RR and DLSS 5 RenoDX for the games at Modding Tools - Nexus Mods</a></li>
<li><a href="https://wccftech.com/nvidia-dlss-5-neural-rendering-in-10-modern-games-the-best-unofficial-dlss-5-on-vs-off-comparisons-so-far/">NVIDIA DLSS 5 Neural Rendering In 10 Modern Games – The Best Unofficial DLSS 5 ON vs OFF Comparisons So Far</a></li>
<li><a href="https://github.com/jlrouzies-fr/DLSS5-Feeder">GitHub - jlrouzies-fr/DLSS5-Feeder: DLSS 5 neural rendering in D3D11/D12/Vulkan games that ship without any DLSS — feeds a synthetic DLAA contract (ReShade depth + motion vectors) to the DLSS 5 add-on via a private D3D12 device.</a></li>

</ul>
</details>

**标签**: `#DLSS`, `#neural rendering`, `#video enhancement`, `#image upscaling`, `#Windows`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [中国光伏装机首超煤电，成为第一大电源](https://content-static.cctvnews.cctv.com/) ⭐️ 8.0/10

截至 2026 年 7 月底，全国光伏发电装机达 12.86 亿千瓦，首次超越煤电，成为我国第一大电源，占总装机的 31.5%。今年 1 至 7 月，全国光伏发电量突破 8024 亿千瓦时，同比增长 15.5%，相当于每 8 度电就有 1 度来自光伏。

telegram · zaihuapd · 9月1日 02:42

**「背景」** 煤电此前长期是中国第一大电源；“装机”指的是发电设备的总规模，光伏装机首次超过煤电，反映能源结构正在转换。

**「影响」** 全球每 10 块光伏组件有 8 块为中国制造，未来五年产业投资预计超过 2 万亿元，意味着光伏制造和投资将继续是能源领域的重点。

**标签**: `#光伏`, `#能源转型`, `#电力结构`, `#中国经济`, `#制造业`

---

<a id="item-finance-news-2"></a>
### [高通上调芯片价格：9 月 1 日后出货产品涨幅两位数](https://www.macrumors.com/2026/08/31/qualcomm-chip-price-increase/) ⭐️ 8.0/10

据 MacRumors 报道，高通宣布自 2026 年 9 月 1 日后出货的全系列芯片价格将上涨，涨幅达两位数，具体幅度将与客户逐一协商。高通 CEO 克里斯蒂亚诺·阿蒙表示，公司无法继续自行承担不断上升的供应商成本；苹果仍为 iPhone 17 系列采购高通的调制解调器芯片。

telegram · zaihuapd · 9月1日 04:10

**「背景」** 高通是向手机厂商供应处理器和调制解调器芯片的主要供应商；此次涨价发生在供应商成本上升的背景下。

**「影响」** 苹果因继续为 iPhone 17 系列采购高通调制解调器芯片，将直接面对这部分采购成本上升。

**标签**: `#semiconductors`, `#pricing`, `#Qualcomm`, `#Apple`, `#supply-chain`

---

<a id="item-finance-news-3"></a>
### [迈阿密经济快速崛起，可持续性受关注](https://www.economist.com/finance-and-economics/2026/08/31/the-extraordinary-rise-of-miamis-economy) ⭐️ 6.0/10

《经济学人》刊文称，在资本流入与政治因素共同推动下，迈阿密经济正在迅速繁荣，但文章对增长能否持续提出疑问。

rss · The Economist · 8月31日 17:01

**「背景」** 这篇报道关注迈阿密经济近期因资本流入和政治因素而快速扩张的现象，并质疑这种繁荣能否持续。相关分析指出，当地财富增长部分来自人们对未来人口涌入、新建项目和资产升值的预期。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://phenomenalworld.org/analysis/miami-syndrome/">Miami Syndrome - Phenomenal World</a></li>

</ul>
</details>

**标签**: `#Miami economy`, `#economic growth`, `#capital flows`, `#urban policy`, `#regional development`

---

## AI 创作者雷达

<a id="item-ai-creator-1"></a>
### [思科为 9 万员工部署个人 AI Agent，可跨系统代办事务](https://www.infoq.cn/article/HQXDr69U4tUQUDzEiidW?utm_source=rss&amp;utm_medium=article) ⭐️ 7.0/10

据 InfoQ 报道，思科（Cisco）为其约 9 万名员工部署了个人 AI Agent。该 Agent 据称能够记忆员工的相关信息，并代表员工跨系统完成事务性操作。目前材料仅确认了这一部署动向，关于该 Agent 的具体功能细节、落地时间及实际效果均未在原文中提供。

rss · InfoQ 中文站 · 8月31日 14:20

**「为什么现在值得关注」** 这一消息值得注意，是因为它不是实验室演示或小范围试点，而是大型企业面向全员规模部署 Agent 的实际案例；不过材料未提供该部署的成效数据，实际影响仍待验证。

**「可做内容角度」** 可做角度：从“记住你的一切”到“替你跨系统办事”，企业给全员配 Agent 后，员工工作流与数据边界可能发生哪些变化；材料只确认了部署动作，具体能力边界仍应谨慎核实，并关注后续官方公布细节。

**标签**: `#Cisco`, `#AI Agent`, `#企业AI`, `#AI助手`, `#企业应用`

---