---
layout: default
title: "Horizon Summary: 2026-07-26 (ZH)"
date: 2026-07-26
lang: zh
---

> 从 18 条内容中筛选出 6 条重要资讯。

---

1. [Anthropic 发布 Claude 5 的新上下文工程规则](#item-1) ⭐️ 8.0/10
2. [GitHub Issues 大改造：缓存与预取技术让页面提速数倍](#item-2) ⭐️ 8.0/10
3. [Fly.io 的 Sprites 困境引发身份危机反思](#item-3) ⭐️ 7.0/10
4. [通用汽车支持美国电网储能用钠离子电池](#item-4) ⭐️ 7.0/10
5. [清华与腾讯提出用 Rollout 降低 LLM 后训练成本](#item-5) ⭐️ 7.0/10
6. [微软用 TPM 芯片封堵盗版 Windows 激活](#item-6) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Anthropic 发布 Claude 5 的新上下文工程规则](https://claude.com/blog/the-new-rules-of-context-engineering-for-claude-5-generation-models) ⭐️ 8.0/10

Anthropic 宣布了其 Claude 5 系列模型的新上下文工程规则，改变了构建提示词和系统指令的最佳实践，旨在提升模型性能。 这些规则旨在提高可靠性和任务完成度，但社区讨论显示了对复杂度增加和可能锁定在 Anthropic 生态系统的担忧。 新规则强调结构化上下文管理，并依赖 Claude 的“自动记忆”功能，一些用户报告称与 Claude 4.8 相比，这导致了意外行为和更高的 token 使用量。

hackernews · mellosouls · 7月25日 20:42 · [社区讨论](https://news.ycombinator.com/item?id=49051361)

**背景**: 上下文工程涉及在推理过程中设计和优化大型语言模型（LLM）的指令和相关上下文，以提高其有效性。它包括从短期和长期记忆中挑选、检索和组织信息的策略。Anthropic 的新规则代表了这种实践专门为 Claude 5 量身定制的演进。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents">Effective context engineering for AI agents \ Anthropic</a></li>
<li><a href="https://www.promptingguide.ai/guides/context-engineering-guide">Context Engineering Guide | Prompt Engineering Guide</a></li>

</ul>
</details>

**社区讨论**: 社区意见不一：一些用户认为新规则不必要地复杂，更倾向于简单交互，而另一些人怀疑这些变更旨在增加供应商锁定。一位用户报告称 Claude 5 比之前版本出错更多且 token 使用量更高。

**标签**: `#Claude`, `#AI`, `#context engineering`, `#Anthropic`, `#LLM`

---

<a id="item-2"></a>
## [GitHub Issues 大改造：缓存与预取技术让页面提速数倍](https://www.infoq.cn/article/yDgq3fh4YxZM93u21Kr5?utm_source=rss&utm_medium=article) ⭐️ 8.0/10

GitHub Issues 通过实施缓存和预取技术，使页面加载速度提升了数倍。 这一改进显著提升了数百万开发者的用户体验，展示了可应用于其他大型 web 应用的前端优化策略。 优化包括客户端缓存 issue 数据和智能预取可能访问的页面，减少了网络请求和渲染时间。

rss · InfoQ 中文站 · 7月25日 09:00

**背景**: GitHub Issues 是 GitHub 平台中用于追踪 bug 和功能请求的关键部分。随着 issue 数量增长，页面加载性能可能下降。缓存将频繁访问的数据存储在本地以避免重复服务器请求，预取则预测用户行为并提前加载资源。这些技术是现代 Web 性能优化中的常见手段。

**标签**: `#GitHub`, `#performance`, `#caching`, `#prefetching`, `#frontend optimization`

---

<a id="item-3"></a>
## [Fly.io 的 Sprites 困境引发身份危机反思](https://fly.io/blog/kurt-scott-money-sprites/) ⭐️ 7.0/10

Fly.io 的博文《转身面对陌生》坦诚讨论了其产品 Sprites 的技术失败，以及 AI 时代公司面临的更广泛身份危机，同时宣布重新聚焦 Sprites 并更换 CEO。 这篇博文意义重大，因为它凸显了初创公司在核心产品存在可靠性问题、AI 革命威胁其整个商业模式时所面临的艰难抉择，为科技行业提供了警示。 Sprites 是用于任意代码的硬件隔离执行环境，类似于一次性 Linux 计算机，但经历了严重的数据丢失和僵尸状态。博文宣布 Scott Johnston 担任新 CEO，领导公司向 AI 沙盒转型。

hackernews · subarctic · 7月25日 20:43 · [社区讨论](https://news.ycombinator.com/item?id=49051369)

**背景**: Fly.io 是一个全球部署应用程序的平台。Sprites 作为代码运行沙盒环境推出，特别适用于 AI 代理，但正如用户所指出的，存在可靠性问题。该公司现在正将重心完全转向 Sprites 作为 AI 沙盒解决方案，而这是一个拥挤且商品化的领域。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sprites.dev/">Sprites — Stateful sandbox environments</a></li>
<li><a href="https://fly.io/blog/design-and-implementation/">The Design & Implementation of Sprites · The Fly Blog</a></li>
<li><a href="https://x.com/simonw/status/2009784546599055445?lang=en">Simon Willison on X: "Sprites is a very cool new thing: it solves two of my pet problems at once, developer sandbox environments for coding agents and a JSON API for executing untrusted code I wrote more here: https://t.co/5SlQAINELf" / X</a></li>

</ul>
</details>

**社区讨论**: 评论者对 Sprites 的可靠性表达了严重不满，一位用户称这是他们用过的最有问题的基础设施产品。其他人指出 Fly.io 长期以来在运营透明度和故障处理上存在问题。一些人认为这一转型是孤注一掷，可能会因来自成熟 AI 沙盒提供商的竞争而失败。

**标签**: `#Fly.io`, `#startups`, `#identity-crisis`, `#DevOps`, `#product-management`

---

<a id="item-4"></a>
## [通用汽车支持美国电网储能用钠离子电池](https://spectrum.ieee.org/sodium-ion-battery-peak-energy) ⭐️ 7.0/10

通用汽车宣布支持 Peak Energy 的钠离子电池技术，计划用于美国电网储能，这是企业对钠作为锂替代品的重大认可。 这一支持可能加速钠离子电池在电网储能领域的应用，减少对昂贵且地理集中的锂的依赖。尽管初期依赖中国供应商，但也显示出对国内生产的信心。 Peak Energy 目前从中国供应商采购商业电池，并计划最终在美国制造。此前一家美国钠离子初创公司因缺乏资金而失败，但通用汽车的支持提供了新动力。

hackernews · rbanffy · 7月25日 21:48 · [社区讨论](https://news.ycombinator.com/item?id=49051947)

**背景**: 钠离子电池是可充电电池，使用丰富的钠替代锂，成本更低且材料更易获得。其工作原理与锂离子电池相似，特别适合对能量密度要求不高的电网储能。中国的 CATL 和 HiNa 等公司已实现钠离子电池商业化，而美国生产则相对滞后。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sodium-ion_batteries">Sodium-ion batteries</a></li>
<li><a href="https://www.iea.org/commentaries/sodium-ion-battery-momentum-grows-but-challenges-remain">Sodium-ion battery momentum grows, but challenges remain – Analysis - IEA</a></li>

</ul>
</details>

**社区讨论**: 评论者指出了当前锂电池的高暖通空调功耗问题，若钠电池成本相近则可降低。一些人期待消费级钠离子家用电池，另一些人对早期美国钠离子初创公司的失败表示遗憾。少数人批评依赖中国电池，还有人更愿意等待固态电池。

**标签**: `#sodium-ion batteries`, `#grid storage`, `#energy storage`, `#GM`, `#battery technology`

---

<a id="item-5"></a>
## [清华与腾讯提出用 Rollout 降低 LLM 后训练成本](https://mp.weixin.qq.com/s?__biz=MzIzNjc1NzUzMw==&mid=2247907199&idx=3&sn=db62b221aeb50a9dfff1af69803b2787) ⭐️ 7.0/10

清华大学与腾讯提出一种方法，将智能体轨迹视为树，并利用 rollout 来降低大语言模型（LLM）后训练的成本。该方法优化了跨 prompt 的预算分配，而非平均分摊。 LLM 后训练成本高昂是公认的难题，该方法有望大幅降低微调及基于智能体交互的强化学习的门槛。它解决了一直困扰研究和工业界的一个关键痛点。 该方法借鉴了强化学习中的 rollout 概念，通过模拟多个可能的未来轨迹来更好地分配算力。将轨迹结构化为树后，系统能避免冗余计算，将资源集中在最有希望的分支上。

rss · 量子位 · 7月25日 04:40

**背景**: LLM 后训练通常包括监督微调（SFT）和基于人类反馈的强化学习（RLHF）等技术。在 on-policy RL 中，rollout 阶段需要从当前策略生成多个候选响应，计算开销极大。将智能体轨迹视为树，可以复用共享前缀并并行验证，从而降低总体生成成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2511.16193">Fast LLM Post - training via Decoupled and Fastest-of-N Speculation</a></li>
<li><a href="https://www.emergentmind.com/topics/specactor">SpecActor: Accelerating LLM Rollouts</a></li>
<li><a href="https://arxiv.org/html/2503.18455">SEAlign: Alignment Training for Software Engineering Agent</a></li>

</ul>
</details>

**标签**: `#LLM`, `#post-training`, `#cost reduction`, `#rollout`, `#agent trajectories`

---

<a id="item-6"></a>
## [微软用 TPM 芯片封堵盗版 Windows 激活](https://www.techspot.com/news/113232-microsoft-using-tpm-chips-crack-down-pirated-windows.html) ⭐️ 7.0/10

微软将在 KMS 激活流程中加入基于 TPM 芯片的硬件验证，即'TPM 证明'机制，要求 KMS 服务器先证明其硬件身份未被篡改，才能处理批量激活请求。该功能将从下一版 Windows Server 起成为强制要求，并自 2026 年 8 月起在 Windows Server 2025 中推送准备提示。 此举旨在打击盗版者长期利用的 KMS 伪造激活，可能使许多现有激活工具失效。然而，攻防战仍在继续，像 Massgrave 这样的组织已发布了更强大的绕过工具 TSforge。 微软已于 2025 年封堵了 KMS38 漏洞；TPM 证明专门针对需要每半年续期的 Online KMS 方法。与此同时，Massgrave 的 TSforge 方法号称可绕过整个 Windows DRM 激活架构，可能提供永久激活。

telegram · zaihuapd · 7月25日 15:55

**背景**: KMS（密钥管理服务）是企业用于批量激活 Windows 和 Office 的机制，无需直接联系微软。盗版激活工具常模拟 KMS 服务器来欺骗客户端激活。TPM（可信平台模块）是一种硬件安全芯片，可验证系统完整性。TPM 证明确保只有真实且未被篡改的 KMS 服务器才能授权激活。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/windows-server/get-started/kms-client-activation-keys">Key Management Services ( KMS ) client activation ... | Microsoft Learn</a></li>
<li><a href="https://massgrave.dev/">Microsoft Activation Scripts | MAS</a></li>
<li><a href="https://www.notebookcheck.net/Microsoft-Windows-and-Office-activation-cracked-again-TSforge-introduces-a-new-more-permanent-DRM-bypass.963349.0.html">Microsoft Windows and Office activation cracked again: TSforge introduces a new, more permanent DRM bypass - Notebookcheck News</a></li>

</ul>
</details>

**标签**: `#Windows`, `#TPM`, `#security`, `#piracy`, `#KMS`

---