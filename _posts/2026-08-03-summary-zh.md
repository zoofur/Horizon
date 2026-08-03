---
layout: default
title: "Horizon Summary: 2026-08-03 (ZH)"
date: 2026-08-03
lang: zh
---

> 从 19 条内容中筛选出 6 条重要资讯。

---

1. [Kakehashi：实验性用户空间在 Linux ARM 上运行 macOS 二进制程序](#item-1) ⭐️ 8.0/10
2. [阿里开源 22B 模型，实现实时稳定数字人生成](#item-2) ⭐️ 8.0/10
3. [Remix 3.0 彻底重写：不再基于 React](#item-3) ⭐️ 8.0/10
4. [卡帕西的 AI 鹈鹕引发 3D 场景基准测试之争](#item-4) ⭐️ 7.0/10
5. [美国能否在 AI 取代工人前完成再培训？](#item-5) ⭐️ 7.0/10
6. [美国多州拟取消数据中心税收优惠，AI 基建成本上升](#item-6) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Kakehashi：实验性用户空间在 Linux ARM 上运行 macOS 二进制程序](https://github.com/wie-project/kakehashi) ⭐️ 8.0/10

Kakehashi 是一个实验性的用户空间翻译层，能够让 macOS 命令行二进制文件原生运行在 Linux ARM（aarch64）上。目前它已经具备 7-Zip、curl 和 Xcode Tools Git 的可运行原型。 该项目可能让 macOS 命令行工具无需完整虚拟化即可运行在 Linux ARM 机器上，类似于 Wine/Proton 对 Windows 应用所做的那样。尽管处于早期阶段，它对系统研究和扩大跨平台兼容性具有潜力。 Kakehashi 以命令行优先，不使用 JIT；它加载 Darwin 的 Mach-O 二进制文件，映射独立的 libSystem，并将 BSD 系统调用转换为 Linux 等价调用。7-Zip 原型目前比原生执行慢约 5.2 倍，而 curl 在自动化测试中通过了 200 多个命令。

hackernews · vlad_kalinkin · 8月2日 16:26 · [社区讨论](https://news.ycombinator.com/item?id=49145937)

**背景**: macOS 二进制文件使用 Mach-O 可执行格式，并依赖 Darwin 内核系统调用，这与 Linux 的 ELF 格式和系统调用接口不同。要在 Linux 上运行它们，翻译层必须重新解释 Mach-O 头，将 Darwin 系统调用重定向到 Linux 等价调用，并提供兼容的库桩。Kakehashi 采用纯用户空间方案（无内核模块），在概念上类似于 Wine 将 Windows API 调用翻译为原生系统服务的方式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/wie-project/kakehashi">wie- project / kakehashi : Userspace macOS translation layer for Linux ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mach-O">Mach-O - Wikipedia</a></li>
<li><a href="https://github.com/apple/darwin-xnu/blob/main/bsd/kern/syscalls.master">darwin-xnu/bsd/kern/syscalls.master at main · apple/darwin-xnu</a></li>

</ul>
</details>

**社区讨论**: 评论者非常热情，并看到了与 Darling 项目的相似之处，询问作者是否会与 Darling 的 ARM64 支持工作合作。还有人希望未来能支持 macOS GUI 应用，包括通过类似 yabridge 的桥接在 Linux 上运行 Audio Unit 插件。

**标签**: `#macOS`, `#Linux`, `#ARM`, `#emulation`, `#userspace`

---

<a id="item-2"></a>
## [阿里开源 22B 模型，实现实时稳定数字人生成](https://mp.weixin.qq.com/s?__biz=MzIzNjc1NzUzMw==&mid=2247908954&idx=3&sn=1f4f3bf12d5fa00e2c37a4dcb7f71de9) ⭐️ 8.0/10

阿里巴巴开源了一款 220 亿参数的模型，能够实现实时、分钟级稳定的数字人生成，并支持自定义角色的流式交互。此次发布直接解决了长期困扰 AI 生成虚拟人的长视频漂移问题。 这一发布意义重大，因为实时稳定、支持自定义角色的数字人生成可以改变 AI 驱动的内容创作、虚拟助手和交互应用。开源 22B 模型降低了开发者和研究人员构建逼真虚拟人的门槛，避免随时间推移出现的质量退化。 该模型旨在保留早期帧的记忆并防止误差累积，这是长视频生成面临的两大核心挑战。它支持流式交互，使数字人能够实时响应，同时在数分钟生成的视频中保持视觉一致性。

rss · 量子位 · 8月2日 02:00

**背景**: 视频生成模型常常面临两个相关问题：遗忘问题，即模型丢失早期内容的记忆；以及漂移问题，即随着视频变长，小误差逐渐累积导致视觉质量下降。这些问题在生成“数字人”——即需要长时间交互中保持视觉一致的 AI 虚拟人物——时尤为突出。流式交互指模型能够持续处理并响应用户输入，而不是等待全部输入完成。这一背景有助于理解为什么阿里宣称的实时、无漂移、自定义角色生成是一个重要的技术里程碑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.qq.com/rain/a/20250715A04D7H00">斯坦福大学突破性视频生成技术：让AI记住更多画面还不“跑偏”的FramePack方法_腾讯新闻</a></li>
<li><a href="https://blog.csdn.net/weixin_44292902/article/details/147398498">FramePack：让视频生成更高效、更实用-CSDN博客</a></li>
<li><a href="https://juejin.cn/post/7337989768637120539">juejin.cn/post/7337989768637120539</a></li>

</ul>
</details>

**标签**: `#AI`, `#数字人`, `#开源模型`, `#视频生成`, `#阿里`

---

<a id="item-3"></a>
## [Remix 3.0 彻底重写：不再基于 React](https://www.infoq.cn/article/s8IA8KgdrizgCEsQAOXr?utm_source=rss&utm_medium=article) ⭐️ 8.0/10

Remix 3.0 不是一次增量升级，而是一次彻底重写：它弃用了 React，改用 Preact 分支，并采用以 this.update() 为核心的命令式模型。该框架还移除了对 Node 特有 API 的依赖，可部署到 serverless、边缘或 Node 运行时。 这次重写标志着从以 React 为中心的声明式开发向新范式的重大转变，开发者需要重新审视自己的心智模型。同时，它使 Remix 在不同部署平台间更加可移植，可能影响全栈框架的演进方向。 Remix 3 基于 Preact 分支而不是 React；状态管理改为调用 this.update() 方法通知框架发生变化，而不是像 React 那样跟踪状态。由于框架避免了 Node 特有 API，开发者可将同一份代码部署到 serverless 函数、边缘 Worker 或长期运行的 Node 进程。

rss · InfoQ 中文站 · 8月2日 09:11

**背景**: Remix 是一个全栈 React 框架，以服务端渲染和基于文件的路由著称，常被视为 Next.js 的替代品。原版 Remix 与 React 的声明式组件模型深度绑定，因此 3.0 的重写意味着与这一传统的根本性决裂。有社区评论指出，这不是一次迁移，而是相当于选择了一个全新框架，这引发了关于 React 生态走向的激烈讨论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.logrocket.com/remix-3-ditched-react/">Remix 3 ditched React: Should you stick with it? - LogRocket Blog</a></li>
<li><a href="https://appwrite.io/blog/post/remix-3-whats-changing-and-why-it-matters">Remix 3: what's changing and why it matters - Appwrite</a></li>
<li><a href="https://frantic.im/remix-3/">Thoughts on Remix 3 / frantic.im - Alex Kotliarskyi</a></li>

</ul>
</details>

**标签**: `#React`, `#Remix`, `#Framework`, `#Frontend`, `#Release`

---

<a id="item-4"></a>
## [卡帕西的 AI 鹈鹕引发 3D 场景基准测试之争](https://twitter.com/karpathy/status/2083749667410727319) ⭐️ 7.0/10

安德烈·卡帕西在推特上分享了一段 AI 生成的 3D 鹈鹕动画，很可能是通过 LLM 编写 three.js 代码完成的。这条推文在 Hacker News 引发讨论：是否应将此类 LLM 生成的 3D 场景用作评估物理世界理解能力和模型能力的新基准。 这场讨论标志着从静态图像生成转向动态 3D 场景，作为更深入检验 AI 对物理现实理解的方式。同时引出了关于基准可复现性的关键问题，以及主流 AI 模型是否隐式地针对 three.js 等特定代码库进行了专门优化。 评论者指出，原图提示词未被公开，导致结果无法直接复现。也有人认为 Anthropic 模型可能专门针对 three.js 代码生成进行过训练，因此这类演示未必反映通用的 3D 推理能力。即便是创建可玩的弹球游戏这类简单任务仍难倒前沿 LLM，说明这些基准仍具挑战性。

hackernews · delichon · 8月2日 04:05 · [社区讨论](https://news.ycombinator.com/item?id=49140998)

**背景**: three.js 是一个广泛使用的 JavaScript 库，通过 WebGL 在浏览器中实现 GPU 加速的 3D 图形，无需专有插件。LLM 可以根据自然语言提示生成 three.js 代码，从而制作出像卡帕西所展示的鹈鹕动画。这促使研究者考虑将 LLM 生成的 3D 场景作为一种评估物理世界推理的基准方法，不过这类基准常面临复现性问题，并可能将针对特定库的训练与真正的理解能力相混淆。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Three.js">Three.js - Wikipedia</a></li>
<li><a href="https://arxiv.org/html/2502.08503v1">Revisiting 3D LLM Benchmarks: Are We Really Testing 3D Capabilities?</a></li>
<li><a href="https://ai4europe-benchmark-guide.readthedocs.io/en/latest/reproducibility.html">Reproducibility in Benchmarking : Challenges and Opportunities...</a></li>

</ul>
</details>

**社区讨论**: 评论者观点不一：consumer451 质疑结果的可复现性，因为提示词未公开；jmugan 则为该演示辩护，认为即使视觉输出不完美，仍是有用的定性基准。HarHarVeryFunny 认为 Anthropic 模型似乎专门针对 three.js 进行了调整，因此结果并不能代表通用智能；bredren 则分享了用 LLM 根据电影场景构建 3D 动画的实际经验，并指出其中所需的大量调优工作。

**标签**: `#AI`, `#LLMs`, `#3D animation`, `#benchmarks`, `#three.js`

---

<a id="item-5"></a>
## [美国能否在 AI 取代工人前完成再培训？](https://www.economist.com/united-states/2026/08/02/can-america-retrain-workers-before-ai-leaves-them-behind) ⭐️ 7.0/10

《经济学人》认为，除非美国像投资半导体那样认真投资劳动力，否则无法成功再培训被 AI 替代的工人。文章将劳动力再培训定位为与《芯片与科学法案》制造业投入同等重要的政策挑战。 这篇文章指出 AI 应用与美国竞争力之间的关键交汇点，若再培训失败，可能加剧经济不平等并削弱公众对 AI 的支持。它将劳动力政策与产业战略联系起来，影响全国员工、雇主和决策者。 《芯片与科学法案》为国内芯片生产提供 390 亿美元资金，为研发和劳动力工作提供 130 亿美元，但其中仅 2 亿美元拨给“美国芯片劳动力与教育基金”。《经济学人》认为，劳动力再培训需要同等规模且持续的投入，才能跟上 AI 导致的岗位替代速度。

rss · The Economist · 8月2日 17:51

**背景**: 《芯片与科学法案》于 2022 年 8 月签署，设立了 25%的税收抵免、390 亿美元的国内生产激励基金，以及 130 亿美元用于研发和劳动力工作。半导体行业组织长期以来敦促加强联邦、州和地方劳动力发展项目的协作，认为政府投资在行业主导时效果最佳。《经济学人》将这一经验应用于 AI 领域，认为再培训项目应被视为核心产业政策，而非事后弥补措施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/CHIPS_and_Science_Act">CHIPS and Science Act — Grokipedia</a></li>
<li><a href="https://www.brookings.edu/articles/an-emerging-partnership-between-economic-development-and-a-community-foundation-in-syracuse-new-york/">An emerging partnership between economic development ... | Brookings</a></li>
<li><a href="https://www.semiconductors.org/wp-content/uploads/2018/06/Roundtable_Summary_Report_-_FINAL.pdf">SIA Workforce Roundtable</a></li>

</ul>
</details>

**标签**: `#AI`, `#workforce`, `#policy`, `#retraining`, `#economics`

---

<a id="item-6"></a>
## [美国多州拟取消数据中心税收优惠，AI 基建成本上升](https://theinformation.com/articles/exclusive-data-center-costs-set-rise-u-s-states-move-repeal-tax-breaks) ⭐️ 7.0/10

据 The Information 报道，美国多个州正考虑取消或收紧此前用于吸引数据中心投资的税收减免政策，原因是电力需求、基础设施投入和财政减收压力上升。此举可能推高美国数据中心建设成本，并影响未来 AI 基础设施布局。 此事意义重大，因为税收优惠一直是数据中心选址的关键因素之一，取消优惠将直接提高云服务商和 AI 企业的成本。这一变化可能减缓 AI 基础设施建设进度，促使投资转向其他地区，并最终推高云服务和 AI 服务的价格。 这些税收优惠通常免除数据中心在服务器、电力及其他设备上的销售税。随着 AI 计算需求激增，地方政府开始要求企业承担更多电网升级和公共基础设施成本，因此新增费用可能会转嫁给云计算客户。

telegram · zaihuapd · 8月3日 00:42

**背景**: 数据中心是容纳服务器并支撑云计算和 AI 工作负载的大型设施。为了吸引这些资本密集型项目，美国许多州历来对硬件和电力提供税收豁免，但 AI 时代数据中心的爆发式增长给当地电网和市政财政带来压力，促使政策转向。

**标签**: `#AI infrastructure`, `#data centers`, `#tax policy`, `#cloud computing`, `#cost analysis`

---