---
layout: default
title: "Horizon Summary: 2026-08-09 (ZH)"
date: 2026-08-09
lang: zh
---

> 从 20 条内容中筛选出 9 条重要资讯。

---

1. [macOS 屏幕共享曝高危漏洞：无需密码即可登录任意账户](#item-1) ⭐️ 9.0/10
2. [把 Android 手机改造成家庭服务器](#item-2) ⭐️ 7.0/10
3. [Fastmail 推出欧盟数据区域，但未提供驻留保证](#item-3) ⭐️ 7.0/10
4. [拟议的“_for-sale”DNS 记录可标记域名出售](#item-4) ⭐️ 7.0/10
5. [英特尔终于在每瓦性能上超越 ARM 了吗？](#item-5) ⭐️ 7.0/10
6. [基于控制论的 Agent 安全防御体系：从失控到可控](#item-6) ⭐️ 7.0/10
7. [MiniMax H3 团队将开源 2K 视频模型，并开发图像模型](#item-7) ⭐️ 7.0/10
8. [115 网盘 API 开放平台宣布暂停服务](#item-8) ⭐️ 7.0/10
9. [Cloudflare 预测 AI 机器人流量将达人类千倍](#item-9) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [macOS 屏幕共享曝高危漏洞：无需密码即可登录任意账户](https://x.com/calif_io/status/2086022794840793454) ⭐️ 9.0/10

安全研究人员公开了 CVE-2026-65400 的概念验证（PoC），这是 macOS 屏幕共享功能中的一个关键漏洞，允许网络攻击者无需密码即可登录任意账户。苹果已在 macOS 26.6.1 中修复该问题，并为 macOS Sequoia 15.7.9 和 Sonoma 14.8.9 提供了反向移植补丁。 这是一个内置远程访问服务中的高危身份验证绕过漏洞：任何开启了屏幕共享的 Mac 都可能被本地网络中的攻击者免密接管。启用该功能的用户应立即安装安全更新，因为公开的 PoC 降低了利用门槛。 苹果通过改进屏幕共享身份验证流程中的状态管理解决了该身份验证问题。研究人员对官方补丁进行了逆向工程，以查明漏洞根因和利用路径，完整技术分析预计在公告次日发布。

telegram · zaihuapd · 8月8日 14:20

**背景**: 屏幕共享是 macOS 的内置功能，允许用户通过网络查看和控制另一台 Mac，通常使用用户名/密码或 VNC 凭据进行验证。开启该功能后，Mac 会监听传入连接，因此可能成为攻击面。CVE-2026-65400 是该功能中的一个身份验证绕过漏洞，而公开的 PoC 证明该漏洞可以被实际利用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.threads.com/@big0___/post/DbvWBWbjmwH/apple-details-the-security-flaw-patched-with-mac-os-mac-os-and-mac-os-apple-has/">Apple details the security flaw patched with macOS 26.6.1, macOS 15.7.9 and macOS 14.8.9. Apple has rolled out the macOS 26.6.1, 15.7.9, and 14.8.9 updates to fix a single critical security flaw. This vulnerability, referenced as CVE-2026-65400, allowed a network attacker to authenticate without valid credentials on the screen sharing function. The manufacturer resolved this authentication issue through improved state management. It is recommended to update your Mac via system settings.</a></li>
<li><a href="https://support.apple.com/guide/mac-help/turn-screen-sharing-on-or-off-mh11848/mac">Turn Mac screen sharing on or off - Apple Support</a></li>
<li><a href="https://www.cve.org/CVERecord?id=CVE-2026-65400">Cve</a></li>

</ul>
</details>

**标签**: `#macOS`, `#security`, `#vulnerability`, `#CVE`, `#screen sharing`

---

<a id="item-2"></a>
## [把 Android 手机改造成家庭服务器](https://seg6.space/posts/phone-server/) ⭐️ 7.0/10

作者详细介绍了如何把一台 Android 手机改造成自托管的家庭服务器，并强调 root 后性能有显著提升。文中还讲述了设置过程中遇到的困难及实用的解决办法。 这篇文章为自托管爱好者提供了一种利用旧手机的低成本改造方案，既能减少电子垃圾，也能节省硬件开销。同时，它也揭示了安全、bootloader 限制以及手机与旧台式机在典型家庭服务器场景中孰优孰劣等关键权衡。 作者指出 root 能提升速度并允许绑定低端口，而锁定的 bootloader 会阻止这类修改。评论者还提到，在低于 Android 8 的版本上 Termux 受限严重，并且长期保持手机电池充电若不妥善管理，会带来火灾隐患。

hackernews · seg6 · 8月8日 22:49 · [社区讨论](https://news.ycombinator.com/item?id=49226636)

**背景**: Termux 是一款免费开源的 Android 终端模拟器，能在 Android 设备上提供 Linux 环境，并带有基于 Debian 的包管理器。Root Android 可以允许用户修改系统设置、运行需要管理员权限的应用，并执行普通用户无法进行的操作。这些概念正是该手机服务器方案的核心。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Termux">Termux</a></li>
<li><a href="https://en.wikipedia.org/wiki/Rooting_(Android)">Rooting (Android) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者就安全性和实用性展开了讨论：有人提醒电池存在火灾隐患，建议将充电限制在 80%；也有人认为旧台式机仍然是大多数家庭服务器最具性价比的选择。还有人指出，锁定的 bootloader 无法复现作者的做法，未 root 时 Termux 会很慢，而 iPhone 因面向消费者的软件设计并不适合当服务器。

**标签**: `#self-hosting`, `#Android`, `#home server`, `#DIY`, `#Termux`

---

<a id="item-3"></a>
## [Fastmail 推出欧盟数据区域，但未提供驻留保证](https://www.fastmail.com/blog/fastmail-offers-eu-data-region/) ⭐️ 7.0/10

Fastmail 宣布推出新的欧盟数据区域选项，让欧盟用户可将数据托管在位于欧盟的基础设施上。但 Fastmail 明确表示，无法保证数据仅保留在欧盟境内。 这很重要，因为在 GDPR 下，数据驻留和主权是欧盟客户的主要关切，各大邮件服务商正竞相提供本地托管。然而，缺乏严格保证也表明非欧盟公司在法律和运营上仍存在局限。 Fastmail 的公司架构横跨澳大利亚和美国（通过收购 Pobox），因此涉及欧盟数据时形成了复杂的多司法管辖区风险面。该公司表示，欧盟区域在运营上让数据“明显更靠近用户”，但并不能提供防止美国或澳大利亚政府获取数据的严格法律保证。

hackernews · groomlake · 8月8日 16:04 · [社区讨论](https://news.ycombinator.com/item?id=49223082)

**背景**: 数据驻留（data residency）指的是组织的数据所存储的物理或地理位置；根据 GDPR 等法律，组织可能被要求将某些数据保存在其收集地所在区域内。欧盟数据主权则进一步要求，无论处理数据的组织位于何处，欧盟居民的个人数据都必须按照 GDPR 处理。由于美国法律及“五眼联盟”的情报访问仍可能触及托管在美国拥有或美国控制的设施上的数据，因此单纯选择地理位置本身并不意味着完全的主权。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/data-residency">What is data residency? - IBM</a></li>
<li><a href="https://visioncompliance.eu/en/blog/data-sovereignty-eu-guide">EU Data Sovereignty Guide</a></li>

</ul>
</details>

**社区讨论**: 评论者大多表示赞赏但保持谨慎：许多人指出，欧盟区域是一个好的开端，但并非隐私问题的万能药。一些人指出，美国拥有的基础设施和法律请求仍然可能触达数据，还有人建议改用 Tuta 等欧洲自有替代服务。

**标签**: `#email`, `#privacy`, `#data-residency`, `#fastmail`, `#EU`

---

<a id="item-4"></a>
## [拟议的“_for-sale”DNS 记录可标记域名出售](https://specification.website/spec/foundations/for-sale-dns/) ⭐️ 7.0/10

一项新提案（以及相关 RFC 10023）描述了“_for-sale”DNS TXT 记录，域名所有者可发布该记录来公开表示域名在售。该记录作为以下划线开头的叶子节点放在域名之下，遵循 RFC 8552 定义的模式。 如果被广泛采用，这将在 DNS 中创建一个明确且机器可读的市场信号，可能改变域名的买卖和发现方式。它同时带来法律风险：公开表示域名在售可能被用作 UDRP 仲裁中的证据，尤其涉及商标权人时。 技术上，该记录是域名下“_for-sale”标签处的 TXT 记录，域名不再出售时应删除该记录。然而，缺少该记录并不能可靠地表示“不出售”，因为如今大多数在售域名并未发布此记录。

hackernews · shaunpud · 8月8日 13:26 · [社区讨论](https://news.ycombinator.com/item?id=49221668)

**背景**: DNS 以多种记录类型（如 A、MX、TXT）存储域名信息；TXT 记录可包含任意文本，常被用于验证和策略标记。以下划线开头的 DNS 标签是特殊用途记录的公认约定，已在 RFC 8552 中说明。UDRP 是 ICANN 用于解决域名与商标争议的仲裁政策，因此公开的出售信号可能带来法律后果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.techtimes.com/articles/322752/20260803/dns-gets-first-standard-commercial-intent-rfc-10023-enables-sale-tags.htm">DNS Gets First Standard for Commercial Intent: RFC 10023 Enables...</a></li>
<li><a href="https://www.icann.org/en/contracted-parties/consensus-policies/uniform-domain-name-dispute-resolution-policy/uniform-domain-name-dispute-resolution-policy-01-01-2020-en">Uniform Domain - Name Dispute - Resolution Policy</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论了公开的“在售”标记是否会自动在商标仲裁中损害所有者利益，有人还讲述了自己与 Sony 的争议。另一些人拿 RFC 10023 开玩笑，提议对域名征收类似“乔治主义”的地价税，指出记录缺失并不代表不出售，并质疑在浏览器逐渐淡化 URL 的背景下域名是否仍然重要。

**标签**: `#DNS`, `#domains`, `#proposal`, `#trademark`, `#policy`

---

<a id="item-5"></a>
## [英特尔终于在每瓦性能上超越 ARM 了吗？](https://hackaday.com/2026/08/08/want-energy-efficiency-dude-youre-getting-a-dell/) ⭐️ 7.0/10

Hackaday 的一篇文章提出疑问：英特尔最新的笔记本电脑芯片能否终于在每瓦性能上匹敌或超越 ARM？文章引用了 2026 款戴尔 XPS 13 与苹果 MacBook Neo 的对比测试。实际测试由 Jeff Geerling 完成，其视频和博文提供了原始数据。 如果英特尔确实缩小了能效差距，可能会重塑笔记本电脑市场的竞争格局和电池续航预期，挑战 ARM 在移动端能效方面的传统主导地位。这一结果将影响消费者、云服务商以及 x86 与 ARM 之间的整体竞争态势。 评论者指出，该能效测试主要针对矩阵运算任务，可能无法反映日常综合负载；此外，苹果 Neo 搭载的是 iPhone 级别的 A18 Pro 芯片，而非 M 系列处理器。定价比较也因地区而异：在德国，戴尔 XPS 13 比 MacBook Neo 贵约 56%。

hackernews · gumby · 8月8日 16:04 · [社区讨论](https://news.ycombinator.com/item?id=49223079)

**背景**: 每瓦性能（performance per watt）衡量每消耗一瓦特电力所能提供的计算量，是笔记本电脑和数据中心的重要能效指标。苹果于 2026 年 3 月 4 日发布 MacBook Neo，这是首款使用 A 系列芯片的 Mac——该芯片此前仅用于 iPhone 和 iPad，而非其他 Apple Silicon Mac 所用的 M 系列。英特尔在能效方面历来落后于 ARM 架构，但最新的 x86 芯片设计正试图缩小这一差距。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Performance_per_watt">Performance per watt - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/MacBook_Neo">MacBook Neo - Wikipedia</a></li>
<li><a href="https://www.apple.com/macbook-neo/specs/">MacBook Neo - Tech Specs - Apple</a></li>

</ul>
</details>

**社区讨论**: 评论者总体持欣赏但怀疑的态度：有人指出应参考 Jeff Geerling 的原始视频和博文，也有人质疑测试仅覆盖矩阵运算以及不同地区的定价差异。一位评论者提到 Apple Neo 在图形性能上仍快 2 倍、单核 CPU 快约 1.4 倍，还有人抱怨取消了耳机插孔。整体上，人们对英特尔的能效提升持谨慎乐观，但对其在实际应用中的表现和全球性价比仍存保留意见。

**标签**: `#hardware`, `#performance-per-watt`, `#Intel`, `#ARM`, `#laptops`

---

<a id="item-6"></a>
## [基于控制论的 Agent 安全防御体系：从失控到可控](https://www.infoq.cn/article/MMh1pkuNSPDlUAtuRelk?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

本文介绍了一套基于系统控制论的 Agent 安全防御体系，旨在将 AI Agent 从失控状态转为可控。vivo 提出了覆盖感知、决策、执行、反馈全链路的安全架构，并在真实业务中验证了其可观测性与恢复能力。 随着 AI Agent 在生产环境中的广泛部署，其安全正从单点防护转向系统级可控。这一工程实践为构建动态闭环防御体系提供了参考，顺应了行业对 Agent 安全治理的迫切需求。 该体系以系统控制论为基础，强调闭环反馈机制，覆盖从感知、决策、执行到反馈的完整 Agent 链路，并重点验证可观测性与恢复能力。本文属于工程实践分享而非突破性研究，但其方法论对 Agent 安全设计具有通用参考价值。

rss · InfoQ 中文站 · 8月9日 10:00

**背景**: 系统控制论是一门研究如何通过反馈机制调节动态系统的学科。将其应用于 AI 安全，意味着把 Agent 视为受控系统，通过持续监测其行为并施加干预，使其始终处于安全边界内。近年已有研究从控制论和复杂系统视角探讨 AI 安全，尤其是生成模型与人类交互之间的反馈循环。这篇文章顺应了这一趋势，提供了系统级且经过实践验证的防御设计。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.infoq.cn/article/MMh1pkuNSPDlUAtuRelk">从失控到可控：基于系统控制论的 Agent 安全防御体系设计与实践｜AICo...</a></li>
<li><a href="https://hub.baai.ac.cn/paper/e5e95dbb-815f-4fc1-92e0-78d7dc1e95e7">Human-AI Safety: A Descendant of Generative AI and Control Systems Safety - 智源社区论文</a></li>
<li><a href="https://swarma.org/?p=47423">大模型安全与对齐：复杂系统视角下的AI安全 | 集智俱乐部</a></li>

</ul>
</details>

**标签**: `#AI安全`, `#Agent`, `#系统控制论`, `#防御体系`, `#实践`

---

<a id="item-7"></a>
## [MiniMax H3 团队将开源 2K 视频模型，并开发图像模型](https://www.infoq.cn/article/9C3eK9tJqDXbabbBy3aj?utm_source=rss&utm_medium=article) ⭐️ 7.0/10

MiniMax H3 团队在 Reddit 上宣布计划开源其 2K 视频模型，确认图像模型正在积极开发中，并表示正在考虑采用 Apache-2.0 许可证。 这标志着 MiniMax 强大的视频生成模型正朝着更开放的方向迈进，可能使社区能够更广泛地进行定制和本地部署。潜在的 Apache-2.0 许可证以及即将推出的图像模型，也可能增强 MiniMax 在竞争激烈的 AI 媒体生成领域的地位。 MiniMax H3（又称 Hailuo 3）的 2K 版本支持 768P 和 2K 输出、4-15 秒的视频时长、7000 字符的提示词上限以及最多九张参考图片。目前，开放权重版本可能仍有使用限制，因此转向 Apache-2.0 将是一个值得注意的许可变更。

rss · InfoQ 中文站 · 8月8日 08:00

**背景**: MiniMax H3 是一个多模态 AI 视频生成与编辑模型，能够在同一创作环境中处理文本、图像、视频和音频。它以生成带有原生立体声的视频而闻名，开放权重版本已经允许在高端 GPU 上本地部署，例如社区用户已在单块 RTX PRO 6000 上运行 FP8 版本。团队在 Reddit 上的公告为未来的开源版本和模型开发提供了路线图。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/MiniMaxAI/MiniMax-H3">MiniMaxAI/ MiniMax - H 3 · Hugging Face</a></li>
<li><a href="https://minimax3.com/">MiniMax H 3 — Hailuo 3 AI Video Generator, Text & Image to Video</a></li>
<li><a href="https://hailuoai.video/tools/minimax-h3">MiniMax H 3 Multimodal AI Video Model | Hailuo AI</a></li>

</ul>
</details>

**标签**: `#AI`, `#MiniMax`, `#open-source`, `#image generation`, `#licensing`

---

<a id="item-8"></a>
## [115 网盘 API 开放平台宣布暂停服务](https://q.115.com/115/T976421.html#) ⭐️ 7.0/10

115 网盘 API 开放平台于 8 月 8 日 23:56 发布公告，宣布自 2026 年 8 月 9 日 0:00 起暂停 API 服务。此前 115 已启动违规使用专项治理。 这次停服将直接影响依赖 115 官方 API 实现直链的 NAS 用户和第三方播放软件。在 2026 年截止日期前，依赖 115 云存储生态的开发者和用户需要寻找替代方案。 API 平台支持文件上传、下载、分享、重命名、移动、删除、文件信息查询及部分播放能力。恢复时间和后续安排将以官方公告为准。

telegram · zaihuapd · 8月8日 19:48

**背景**: NAS（网络附属存储）是连接到网络上的专用数据存储服务器，常用于备份照片和文件，以及在家中的电影、电视剧和音乐存储与播放。许多 NAS 和第三方播放器通过云盘官方 API 生成直链进行播放，因此 115 的 API 暂停会影响这些工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/651007267">NAS是什么？我们真的需要NAS吗？怎么选择NAS？NAS对家庭网络有什么要...</a></li>
<li><a href="https://www.cnblogs.com/rongba/articles/15589820.html">入门NAS？一篇就够了！真正给小白看的NAS科普篇——NAS是什么？你真的需...</a></li>

</ul>
</details>

**标签**: `#API`, `#云存储`, `#服务停止`, `#NAS`, `#115`

---

<a id="item-9"></a>
## [Cloudflare 预测 AI 机器人流量将达人类千倍](https://www.techspot.com/news/113410-cloudflare-humans-could-become-rounding-error-bots-generate.html) ⭐️ 7.0/10

Cloudflare 首席财务官 Thomas Seifert 在第二季度财报电话会议上表示，按当前趋势发展，五年内非人类流量将达到人类流量的 1000 倍。公司还指出，早前关于机器人流量将在 2027 年超过人类流量的预测已在今年提前实现。 这一预测凸显了互联网流量结构的根本性转变，其推动力是能以机器速度运行的智能体 AI 系统。它可能重塑网络基础设施的优先事项、机器人管理策略，以及发布商在日益自动化的网络环境中实现内容变现的方式。 驱动这一激增的是智能体 AI 系统，它们的行为类似于正常的人类浏览，却能够以规模化方式高速重复任务；一个简单提示就可能触发数千次请求。Cloudflare 首席执行官 Matthew Prince 此前曾预测机器人流量将在 2027 年底超过人类流量，但这一转折点已在今年到来。

telegram · zaihuapd · 8月9日 02:08

**背景**: 智能体 AI（Agentic AI）是指能自行感知、推理并采取行动的半自主或全自主 AI 系统，麻省理工斯隆管理学院对此有详细解释。思科的一项研究发现，智能体 AI 产生的网络流量比传统互联网使用多出 450%，形成持续不断的机器间通信模式。Cloudflare 作为主要互联网基础设施提供商，其流量数据和预测在行业讨论中具有重要分量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.techtimes.com/articles/317877/20260605/bot-traffic-passes-humans-online-cloudflare-says-agentic-ai-drove-575-share.htm">Bot Traffic Passes Humans Online: Cloudflare Says Agentic AI ...</a></li>
<li><a href="https://mitsloan.mit.edu/ideas-made-to-matter/agentic-ai-explained">Agentic AI, explained - MIT Sloan</a></li>
<li><a href="https://convergedigest.com/cisco-study-finds-agentic-ai-generates-450-more/">Cisco Study Finds Agentic AI Generates 450% More Traffic than ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#bots`, `#Cloudflare`, `#internet traffic`, `#prediction`

---