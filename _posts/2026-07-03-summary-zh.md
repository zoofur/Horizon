---
layout: default
title: "Horizon Summary: 2026-07-03 (ZH)"
date: 2026-07-03
lang: zh
---

> 从 29 条内容中筛选出 9 条重要资讯。

---

1. [腾讯阿图因 AI 在 CyberGym 基准测试中超越 Mythos](#item-1) ⭐️ 9.0/10
2. [Jamesob 的本地运行 SOTA LLM 实用指南](#item-2) ⭐️ 8.0/10
3. [PostgreSQL 与 OOM Killer：为何使用严格内存超发](#item-3) ⭐️ 8.0/10
4. [HAT-4D：单目视频直接生成 4D 交互场景](#item-4) ⭐️ 8.0/10
5. [OpenAI 与 Anthropic 自研芯片，剑指英伟达护城河](#item-5) ⭐️ 8.0/10
6. [Costco：亚马逊的反面模式](#item-6) ⭐️ 7.0/10
7. [工厂不过是房间](#item-7) ⭐️ 7.0/10
8. [阿里巴巴下令全员卸载 Claude，7 月 10 日生效](#item-8) ⭐️ 7.0/10
9. [极客湾评测：华为 Mate 80 Pro 游戏能效超骁龙 8 Gen3](#item-9) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [腾讯阿图因 AI 在 CyberGym 基准测试中超越 Mythos](https://mp.weixin.qq.com/s/BzU7g-2iG7d6h4ViwMhxyg) ⭐️ 9.0/10

腾讯玄武实验室宣布，其基于开源模型 GLM-5.1 构建的阿图因 AI 在 CyberGym 网络安全基准测试中获得 84.0%的分数，超过了 Anthropic 的 Claude Mythos Preview。该工具消耗的预算不足 Mythos“玻璃翼计划”的 0.1%，并在 curl、OpenSSL 等多个关键开源项目中发现了 Mythos 未检测到的高危漏洞。 这标志着 AI 驱动漏洞检测的重大进步，以极低成本实现了顶级性能。它有望使高级网络安全测试更普及，并加速关键软件漏洞的修复。 阿图因 AI 基于可本地部署的 GLM-5.1 模型，发现了 curl、gnark、OpenSSL 等项目中评分高达 9.3 的逻辑漏洞。在 BVI 真实世界漏洞榜单中，其漏洞严重程度排名第一，总数排名第五。

telegram · zaihuapd · 7月3日 16:12

**背景**: CyberGym 是加州大学伯克利分校主导的评估框架，包含来自 188 个开源项目的 1507 个真实漏洞，用于测试 AI 智能体的漏洞复现能力。GLM-5.1 是智谱 AI 推出的开源旗舰模型，专为智能体工程任务设计，编码能力更强。Mythos 是 Anthropic 针对网络安全优化的 AI 模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cybergym.io/cybergym/">CyberGym: Evaluating AI Agents' Real-World Cybersecurity ...</a></li>
<li><a href="https://z.ai/blog/glm-5.1">GLM-5.1: Towards Long-Horizon Tasks - z.ai</a></li>

</ul>
</details>

**标签**: `#AI`, `#Cybersecurity`, `#Vulnerability Detection`, `#Benchmark`, `#Tencent`

---

<a id="item-2"></a>
## [Jamesob 的本地运行 SOTA LLM 实用指南](https://github.com/jamesob/local-llm) ⭐️ 8.0/10

Jamesob 在 GitHub 上发布了一份新指南，提供了在本地硬件上设置和运行最先进大语言模型的实用说明，涵盖硬件选择、量化和优化技术。 该指南满足了人们对本地部署大语言模型日益增长的兴趣，以实现隐私保护、成本节约和低延迟使用场景，并帮助爱好者和开发者了解硬件需求和权衡。 重点包括顶级设置的高成本（超过 4 万美元，包含多个 1.2 万美元的 GPU），以及更便宜的替代方案（如 32GB Intel Arc B70）的可行性，并利用量化模型将大语言模型装入有限内存。指南还强调了 GPU 卸载等技术，以及统一内存架构（如 Apple Silicon）的新兴选择，可以以合理速度运行 DeepSeek 等大型模型。

hackernews · livestyle · 7月3日 15:03 · [社区讨论](https://news.ycombinator.com/item?id=48775921)

**背景**: 由于包含数十亿个参数，在本地运行大语言模型需要大量的计算资源。量化是一种通过降低模型权重的数值精度（通常从 16 位降至 4 位或 5 位）来减少内存和计算需求的技术，评估表明其精度损失极小。本地设置通常使用 llama.cpp 等软件运行 GGUF 格式的量化模型，这些模型可以扩展到从消费级 GPU 到多 GPU 服务器的范围。硬件选择涉及 GPU 内存容量、内存带宽（如 GDDR5 与 DDR4）和计算能力之间的权衡，现代模型即使经过量化后也通常需要数十 GB 的显存。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.reddit.com/r/StableDiffusion/comments/1kup6v2/could_someone_explain_which_quantized_model/">r/StableDiffusion on Reddit: Could someone explain which quantized model versions are generally best to download? What's the differences?</a></li>
<li><a href="https://developers.redhat.com/articles/2024/10/17/we-ran-over-half-million-evaluations-quantized-llms">We ran over half a million evaluations on quantized LLMs—here's what we found | Red Hat Developer</a></li>

</ul>
</details>

**社区讨论**: 社区评论揭示了热情与谨慎并存的态度。用户分享了像 Intel Arc B70 这样的替代硬件选择以节省成本，警告追逐最先进模型的高成本和收益递减，并强调较小的量化模型可能足以满足许多任务。一些人表示对硬件环境感到困惑，并希望为非开发者提供更简单的指导，而另一些人则指出像 Apple Silicon 这样的统一内存系统是实用的折衷方案。

**标签**: `#local-llm`, `#hardware`, `#guide`, `#quantized-models`, `#home-lab`

---

<a id="item-3"></a>
## [PostgreSQL 与 OOM Killer：为何使用严格内存超发](https://www.ubicloud.com/blog/postgresql-and-the-oom-killer-why-we-use-strict-memory-overcommit) ⭐️ 8.0/10

云服务商 Ubicloud 发布一篇技术文章，解释他们在托管 PostgreSQL 服务中采用严格内存超发（vm.overcommit_memory=2）的原因，以避免 Linux 的 OOM killer 意外终止进程。 这揭示了数据库运维中的一个关键权衡：Linux 默认超发策略可能在内存紧张时不可预测地杀死 PostgreSQL 进程，导致宕机和数据丢失，而严格超发牺牲部分内存利用率以换取稳定性。 严格模式根据 overcommit_kbytes 或 overcommit_ratio 设定 CommitLimit，超额分配即返回 ENOMEM 失败；若限制过紧，可能破坏依赖写时复制 fork 语义的程序，需仔细调优和测试。

hackernews · furkansahin · 7月3日 13:00 · [社区讨论](https://news.ycombinator.com/item?id=48774509)

**背景**: Linux 内核的内存超发允许进程请求超过物理内存的虚拟内存，假设进程不会同时全部使用。当物理内存耗尽时，OOM killer 根据评分选择进程杀死。系统通过 overcommit_memory 参数控制：0（启发式默认），1（始终超发），2（严格模式，受交换空间和超发比例限制）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ubicloud.com/blog/postgresql-and-the-oom-killer-why-we-use-strict-memory-overcommit">PostgreSQL and the OOM Killer: Why We Use Strict Memory Overcommit</a></li>
<li><a href="https://www.baeldung.com/linux/memory-overcommitment-oom-killer">Linux Memory Overcommitment and the OOM Killer - Baeldung Understanding and Utilizing the Linux OOM Killer How to Configure the Linux Out-of-Memory Killer - Oracle How to Prevent Out of Memory (OOM) Freezes on Linux: Fixing ... Out Of Memory Management - The Linux Kernel Archives How to interpret an OOM killer message - Red Hat Customer Portal</a></li>
<li><a href="https://www.kernel.org/doc/html/v6.13/mm/overcommit-accounting.html">Overcommit Accounting — The Linux Kernel documentation</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：许多人批评 Linux 默认设置“疯狂”，另有人警告严格超发会浪费内存或破坏不检查 malloc 返回值的程序。Ubicloud 的 Ozgun 承认标题语气过强，但坚称该策略适合托管服务，且所有人强调上线前必须充分测试。

**标签**: `#postgresql`, `#linux`, `#overcommit`, `#memory-management`, `#oom-killer`

---

<a id="item-4"></a>
## [HAT-4D：单目视频直接生成 4D 交互场景](https://mp.weixin.qq.com/s?__biz=MzIzNjc1NzUzMw==&mid=2247901356&idx=3&sn=54ee94026f76691a380cd3ea214e0def) ⭐️ 8.0/10

上海交通大学等机构的研究人员提出了 HAT-4D，这是首个基于智能体的框架，能从单一单目视频中重建多个物体的三维几何、时序动态和物理交互，无需昂贵的运动捕捉设备。 该突破大幅降低了运动捕捉的成本门槛，使机器人、AR/VR、自动驾驶和内容创作等领域更容易获取 4D 交互场景生成技术，并可能加速具身 AI 的研究。 HAT-4D 采用人机协作范式，很可能利用视觉-语言模型从有限视角推断物体交互和遮挡关系，并重建实例级几何，而不仅仅是照片级渲染。

rss · 量子位 · 7月3日 03:43

**背景**: 4D 重建在三维基础上增加时间维度，捕捉形状和外观的动态变化，是理解动态场景的关键。传统方法通常依赖多视角相机阵列或运动捕捉系统，成本高昂且局限于专用棚。单目视频仅提供单一视角，信息严重不足，使 4D 重建极具挑战。HAT-4D 通过显式建模物体交互的智能体框架解决了上述难题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2606.28215v1">[2606.28215v1] HAT-4D: Lifting Monocular Video for 4D Multi-Object Interactions via Human-Agent Collaboration</a></li>
<li><a href="https://arxiv.org/html/2606.28215v1">HAT-4D: Lifting Monocular Video for 4D Multi-Object Interactions via Human-Agent Collaboration</a></li>

</ul>
</details>

**标签**: `#AI`, `#computer vision`, `#4D reconstruction`, `#monocular video`, `#motion capture`

---

<a id="item-5"></a>
## [OpenAI 与 Anthropic 自研芯片，剑指英伟达护城河](https://www.infoq.cn/article/MOqFJbvWYlJ9PXcfdfCC?utm_source=rss&utm_medium=article) ⭐️ 8.0/10

据报道，OpenAI 和 Anthropic 正在各自设计定制 AI 芯片，可能为 ASIC，以减少对英伟达昂贵 GPU 的依赖，并降低训练和推理成本。 此举可能打破英伟达在 AI 加速器领域的近乎垄断地位，促进竞争，从而降低硬件成本，加速 AI 技术的更广泛采用。 定制 ASIC 针对特定 AI 工作负载可能提供更高的能效比，但开发需要巨额投资，且需克服英伟达根深蒂固的 CUDA 软件生态。

rss · InfoQ 中文站 · 7月3日 18:00

**背景**: 目前，英伟达的 GPU 在训练和运行 AI 模型的市场中占主导地位，但它们通用且昂贵。专用集成电路（ASIC）是为单一用途定制的芯片，效率更高。英伟达的 CUDA 平台提供了使其 GPU 高度可编程的软件层，形成了强大的开发者生态锁定。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Application-specific_integrated_circuit">Application-specific integrated circuit - Wikipedia</a></li>
<li><a href="https://www.arm.com/glossary/asic">What is ASIC? - ASIC Cost – Arm®</a></li>
<li><a href="https://en.wikipedia.org/wiki/Nvidia_CUDA_platform">Nvidia CUDA platform</a></li>

</ul>
</details>

**标签**: `#AI chips`, `#OpenAI`, `#Anthropic`, `#NVIDIA`, `#hardware`

---

<a id="item-6"></a>
## [Costco：亚马逊的反面模式](https://phenomenalworld.org/analysis/the-anti-amazon/) ⭐️ 7.0/10

一项新分析认为，Costco 基于托盘、顾客自提的模式避免了亚马逊高昂的最后一英里配送，创造了更大的社会价值。 这挑战了亚马逊便利性总是更优的传统观念，突显了最后一英里配送的潜在社会和环境成本。 Costco 的模式依赖批量运送到面向消费者的仓储，减少了包装和配送开支，而亚马逊的最后一英里物流涉及个性化处理。

hackernews · bookofjoe · 7月3日 15:14 · [社区讨论](https://news.ycombinator.com/item?id=48776044)

**背景**: Costco 采用会员制模式，在大型仓储式商店批量销售，由顾客自行取货。亚马逊则以庞大的配送网络将商品直接送到消费者家中，承担高昂的最后一英里成本。

**社区讨论**: 评论者讨论了 Costco 模式的社会价值，一些人赞扬它避免了最后一英里复杂性，另一些人指出它仍通过 Instacart 提供配送，并批评过度消费。

**标签**: `#business-models`, `#logistics`, `#e-commerce`, `#costco`, `#amazon`

---

<a id="item-7"></a>
## [工厂不过是房间](https://interconnected.org/home/2026/07/03/factories) ⭐️ 7.0/10

马特·韦伯的文章提出，工厂本质上只是制造物品的房间，这一观点揭开了制造业的神秘面纱，鼓励人们自己动手。 这种思维转变可以帮助个人开始小规模生产，降低创业门槛，与创客运动相呼应，振兴本地经济。 社区评论强调，实际制造过程涉及流程设计、库存管理和劳动分工等复杂挑战，远非一个房间那么简单。

hackernews · arbesman · 7月3日 15:13 · [社区讨论](https://news.ycombinator.com/item?id=48776035)

**背景**: 创客运动普及了个人利用可及工具制造产品的理念。历史上工厂集中了生产，但分布式制造正变得可行。然而，从原型扩展到运转良好的工厂需要供应链、质量控制和商业运营方面的专业知识。

**社区讨论**: 总体上，评论者赞赏这种鼓舞人心的信息，但也警告经营工厂需要专业分工和市场头脑。有关小规模制造中欢乐与挣扎的故事，凸显了从“我可以”到可持续经营之间的差距。

**标签**: `#manufacturing`, `#maker-movement`, `#mindset`, `#diy`, `#technology`

---

<a id="item-8"></a>
## [阿里巴巴下令全员卸载 Claude，7 月 10 日生效](https://t.me/zaihuapd/42334) ⭐️ 7.0/10

阿里巴巴内部要求所有员工卸载 Anthropic 产品，包括 Claude 模型 Sonnet、Opus、Fable 以及代理产品 Claude Code，禁令于 7 月 10 日生效。此前，Anthropic 指控阿里巴巴在 4 月至 6 月间使用约 2.5 万个虚假账号与 Claude 交互超过 2800 万次。 此举凸显了企业 AI 安全紧张局势的升级，以及中国科技巨头与美国 AI 公司之间的直接争端。这可能会影响内部 AI 工具政策、供应商关系以及全球 AI 行业的竞争格局。 禁令涵盖所有 Claude 模型（Sonnet、Opus、Fable）以及 Claude Code。Anthropic 声称阿里巴巴使用 2.5 万个虚假账号与 Claude 进行超 2800 万次交互，导致 Anthropic 收紧风控策略。

telegram · zaihuapd · 7月3日 13:00

**背景**: Claude 是 Anthropic 开发的大语言模型系列，该公司由前 OpenAI 成员创立，专注于 AI 安全。模型包括 Haiku、Sonnet、Opus 和 Fable，针对不同任务进行了优化。Claude Code 是 AI 辅助软件开发工具。阿里巴巴此前曾报销员工使用外部 AI 模型的费用，但在滥用指控下逆转了政策。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anthropic_Claude">Anthropic Claude</a></li>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>

</ul>
</details>

**标签**: `#Alibaba`, `#Claude`, `#AI policy`, `#corporate security`, `#Anthropic`

---

<a id="item-9"></a>
## [极客湾评测：华为 Mate 80 Pro 游戏能效超骁龙 8 Gen3](https://www.bilibili.com/video/BV1F7T46wEyT) ⭐️ 7.0/10

极客湾的评测显示，华为 Mate 80 Pro 系列搭载麒麟 9030/9030 Pro，并在原生鸿蒙优化下，游戏能效超越骁龙 8 Gen3，其中 Mate 80 Pro Max 运行《原神》60 帧时整机功耗仅 4.9W。 这表明软硬件深度协同能够有效弥补芯片的理论性能差距，对华为在制裁下的生态竞争力意义重大，也可能推动行业更重视系统优化。 麒麟 9030 Pro 采用 9 核 14 线程 CPU 和 ALU 单元翻倍的马良 935 GPU；评测中《王者荣耀》120 帧极致画质功耗约 3W，且得益于更智能的调度和应用优化，系统流畅度与续航均有提升。

telegram · zaihuapd · 7月3日 13:27

**背景**: 由于美国制裁，华为海思麒麟芯片在制程工艺上受限，因此转向架构和软硬协同优化。鸿蒙 OS 是华为自研的微内核操作系统，原生应用支持可实现更高效的调度。骁龙 8 Gen3 是高通当前旗舰平台，性能强劲但游戏功耗通常较高。极客湾是国内知名科技评测团队，以深度性能分析见长。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ithome.com/0/972/456.htm">华 为 Mate 80 Pro 性能解禁：麒麟 9030 Pro GPU 相比 9020 提升 76...</a></li>
<li><a href="https://www.notebookcheck.net/HiSilicon-Maleoon-935-Benchmarks-and-Specs.1249609.0.html">Specifications and benchmarks of the HiSilicon Maleoon 935 GPU .</a></li>
<li><a href="https://m.zol.com.cn/article/11359173.html">华为Mate 80 Pro 现货开放， 麒 麟 9030 系列供货趋稳但 Pro Max...</a></li>

</ul>
</details>

**标签**: `#mobile processors`, `#performance optimization`, `#HarmonyOS`, `#gaming`, `#energy efficiency`

---