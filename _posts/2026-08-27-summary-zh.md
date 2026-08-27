---
layout: default
title: "Horizon Summary: 2026-08-27 (ZH)"
date: 2026-08-27
lang: zh
---

> 从 62 条内容中筛选出 10 条重要资讯。

---

**AI 创作者雷达**
1. [Claude 桌面端 Cowork 内置浏览器开始推送](#item-ai-creator-1) ⭐️ 9.0/10
2. [535B 大模型直播训练三个月并开源，吴恩达公开力挺](#item-ai-creator-2) ⭐️ 7.0/10

**科技新闻**
1. [亚马逊 Mechanical Turk 9 月 30 日关停](#item-tech-news-1) ⭐️ 8.0/10
2. [GLM-5.3-Flash 开源模型发布](#item-tech-news-2) ⭐️ 8.0/10
3. [Asahi Linux 为 M3 系列带来 USB 3.0 和雷电支持](#item-tech-news-3) ⭐️ 7.0/10
4. [Tailcat：在 Tailscale 加密数据面上重制 netcat](#item-tech-news-4) ⭐️ 7.0/10
5. [美国暂停移民签证申请引发科技人才担忧](#item-tech-news-5) ⭐️ 7.0/10

**财经新闻**
1. [Meta 就重磅诉讼达成和解，最高支付 170 亿美元并调整青少年平台规则](#item-finance-news-1) ⭐️ 8.0/10
2. [俄罗斯为何故意让卢布贬值](#item-finance-news-2) ⭐️ 8.0/10
3. [英伟达季度营收 962 亿美元，首次提前一年给出 70%增长指引](#item-finance-news-3) ⭐️ 8.0/10

---

## AI 创作者雷达

<a id="item-ai-creator-1"></a>
### [Claude 桌面端 Cowork 内置浏览器开始推送](https://claude.com/blog/cowork-built-in-browser) ⭐️ 9.0/10

Anthropic 在 Claude Cowork 桌面应用中新增内置浏览器：当任务涉及网站时，侧边栏会自动打开浏览器，Claude 可自行导航、阅读、点击和输入，并填写表单或操作无连接器的门户，无需安装扩展。该浏览器与用户常用浏览器隔离，无法看到用户的标签页、书签和密码。官方称本周起向 Pro、Max、Team 计划推送并默认开启，Enterprise 管理员今天起可启用。

telegram · zaihuapd · 8月27日 03:06

**「为什么现在值得注意」** 此次更新把浏览器操作能力直接嵌入 Claude 桌面端，并以默认开启方式推送给付费计划，属于产品层面的实质变化。目前仍处于推送早期，官方尚未给出复杂网页场景下的稳定性或效果验证数据。

**「内容角度」** 可做角度：从“桌面端内置浏览器 vs 浏览器扩展/本地自动化”的差异切入，梳理 Claude Cowork 对普通用户与企业的实际可用场景和限制（隔离、默认开启、无扩展），并提示目前仍是推送早期，效果有待验证。

**标签**: `#Claude`, `#桌面应用`, `#内置浏览器`, `#AI代理`, `#产品更新`

---

<a id="item-ai-creator-2"></a>
### [535B 大模型直播训练三个月并开源，吴恩达公开力挺](https://www.infoq.cn/article/y7KTOS9YbBz0OcoyiweQ?utm_source=rss&amp;utm_medium=article) ⭐️ 7.0/10

据 InfoQ 报道，一个规模为 535B 参数的大模型以直播形式公开了三个月的训练全过程，并开源了相关代码、数据与 Loss 曲线。这一做法获得了吴恩达的公开支持。目前报道仅有标题和摘要，缺少训练主体、项目名称、开源地址等可核验细节，因此无法确认更多具体信息。

rss · InfoQ 中文站 · 8月26日 14:51

**「为何现在值得关注」** 在开源大模型持续升温的当下，公开直播训练过程并同步开源代码和数据，是一种罕见的透明度尝试；但值得注意的是，这种“公开”的影响尚未得到验证，不应视为行业趋势或必然成功。

**「内容角度」** 可做角度：以“训练过程全程公开”这件事本身为切入点，讨论大模型开发从“黑盒”走向“透明直播”可能带来的技术监督、社区参与和商业风险，而不是直接评价模型性能或推荐使用。

**标签**: `#大模型`, `#开源`, `#直播训练`, `#吴恩达`, `#535B`

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [亚马逊 Mechanical Turk 9 月 30 日关停](https://www.mturk.com/) ⭐️ 8.0/10

亚马逊的众包微任务平台 Mechanical Turk 宣布于 9 月 30 日正式关闭。该平台长期用于 AI 数据标注、内容审核和零工式在线工作，其关停将直接影响依赖人类智能任务（HIT）的机器学习工作流和众包研究。社区评论指出，随着 AI 足以完成大量非技能型任务，平台作为“横向通用”模式的竞争力下降；另有内部知情者表示，AWS 负责该项目的资深高管约两三年前已转向 Bedrock 和 SageMaker 模型评测，项目迁移至 AWS 原生计费后团队几乎无人维护。对仍依赖人工验证 AI 输出的领域，客户将需要转向需要领域专家的“信任但验证”模式。

hackernews · tmp10423288442 · 8月26日 23:55 · [社区讨论](https://news.ycombinator.com/item?id=49457545)

**「背景」** Mechanical Turk（MTurk）是亚马逊于 2005 年推出的众包平台，让企业把大型人工项目拆分成大量在线“微任务”，分发给全球劳动力完成，曾被杰夫·贝索斯称为“人工人工智慧”。该平台长期支撑 AI 数据标注、内容审核等零工式工作，在人工智能模型训练数据生产中扮演重要角色。然而随着 AI 能力提升重塑众包工作，亚马逊已通知用户将于 2026 年 9 月 30 日正式关闭该服务，结束其 21 年的运营。

**「影响」** 此次关停最直接的影响是，依赖 Mechanical Turk 完成数据标注和微任务的众包工人与请求方将失去该平台，且亚马逊已停止新客户接入，AI 行业正转向具有质量控制和审计追踪的托管标注服务，这使得匿名开放众包模式被进一步边缘化。

**「社区讨论」** 评论区整体认为关停并不意外：多数开发者和用户感到平台长期低调，而 AI 已能胜任许多非技能型微任务，使通用众包模式难以为继。一位自称 Amazon Mechanical Turk 十年最大请求者的用户补充说，AWS 的项目负责人早已调往 Bedrock/SageMaker，团队几近空缺；另有用户分享了 2005 年依靠该平台赚钱的怀旧故事。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techstartups.com/2026/08/26/amazon-is-shutting-down-mechanical-turk-after-21-years-as-ai-reshapes-crowdsourced-work/">Amazon is shutting down Mechanical Turk after 21 years as AI reshapes crowdsourced work - Tech Startups</a></li>
<li><a href="https://www.technotime.net/16283">Amazon to Shut Down Mechanical Turk on September 30, 2026, Ending 21-Year Crowdsourcing Era Amid AI Rise | Techno Time</a></li>
<li><a href="https://aiweekly.co/alerts/amazon-sets-sept-30-shutdown-for-bezos-era-mechanical-turk">Amazon Sets Sept. 30 Shutdown for Bezos-Era Mechanical Turk | AI Weekly</a></li>
<li><a href="https://www.businessinsider.com/amazon-mechanical-turk-shuttered-amid-rise-of-ai-driven-tasks-2026-8">Amazon Shutters Mechanical Turk Amid Rise of AI-Driven Tasks - Business Insider</a></li>
<li><a href="https://www.techtimes.com/articles/319933/20260708/amazon-mechanical-turk-closes-ai-consumed-platform-it-was-built-fake.htm">Amazon Mechanical Turk Closes: AI Consumed the Platform It Was Built to Fake</a></li>
<li><a href="https://best-ai.org/ai-news/amazon-mechanical-turk-to-cease-new-customer-onboarding-by-july-2026-amid-ai-advancements-qdsnjc">Amazon Mechanical Turk to Cease New Customer Onboarding by July 2026 Amid AI Advancements | Best-AI.org | Best-AI.org</a></li>

</ul>
</details>

**标签**: `#Mechanical Turk`, `#crowdsourcing`, `#AI data labeling`, `#gig economy`, `#AWS`

---

<a id="item-tech-news-2"></a>
### [GLM-5.3-Flash 开源模型发布](https://z.ai/blog/glm-5.3-flash) ⭐️ 8.0/10

Z.ai 发布了 GLM-5.3-Flash，这是一个开放权重的语言模型，参数量减半，价格降至 GLM-5.3 的五分之一，同时性能接近 GLM-5.3。模型权重已在 Hugging Face 上提供，并运行在国内芯片上。社区独立基准显示，该模型在成本远低于竞争对手的情况下，性能可与更昂贵的模型相媲美，甚至超越部分模型。该发布延续了中国开源模型快速迭代的势头，为开发者提供了更高效、更低成本的选项。

hackernews · Philpax · 8月26日 14:08 · [社区讨论](https://news.ycombinator.com/item?id=49449507)

**「背景」** GLM-5.3-Flash 是 Z.ai 于 2026 年 8 月 26 日发布的开源权重模型，属于 GLM 系列，此前曾以“Ox Alpha”名义在 OpenRouter 上匿名预览。它是一款 320B-A18B 的原生多模态混合专家（MoE）模型，支持 100 万 token 上下文，采用 MIT 许可证，输入定价为每百万 token 0.15 美元。该模型延续 GLM 系列在开源大语言模型中的布局，并以更低成本接近 GLM-5.3 的性能。

**「影响」** 对于使用开源大模型的开发者和企业，GLM-5.3-Flash 提供了接近旗舰性能但成本大幅降低的替代方案，可显著降低推理和部署开销，并可能推动更多应用采用开放权重模型。

**「社区讨论」** 社区对模型的性价比和发布速度表示赞赏，尤其认可其独立基准表现和成本优势；但也有用户指出 Z.ai 的服务条款存在对输入输出及用户信息的广泛永久授权，以及对“国家利益”等模糊禁止条款的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GLM_%28AI%29">GLM (AI) - Wikipedia</a></li>
<li><a href="https://www.marktechpost.com/2026/08/26/z-ai-releases-glm-5-3-flash-a-320b-a18b-natively-multimodal-moe-with-a-1m-token-context/amp/">Z.ai Releases GLM-5.3-Flash: A 320B-A18B Natively Multimodal MoE With a 1M-Token Context - MarkTechPost</a></li>
<li><a href="https://www.intelligentliving.co/zai-built-ox-alpha-glm-5-3-flash/">Z.ai Built Ox Alpha: GLM-5.3-Flash Now Open-Source</a></li>

</ul>
</details>

**标签**: `#AI`, `#LLM`, `#open-source`, `#GLM`, `#machine-learning`

---

<a id="item-tech-news-3"></a>
### [Asahi Linux 为 M3 系列带来 USB 3.0 和雷电支持](https://asahilinux.org/2026/08/progress-report-7-2/) ⭐️ 7.0/10

Asahi Linux 发布 7.2 版进度报告，宣布已为所有 M3 系列设备启用 USB 3.0 与 Thunderbolt 支持。团队通过逆向工程发现 ACE3 控制器与 CD3217 寄存器集基本相同，但使用 SPMI 接口而非 I2C。目前 SPMI 接口与 ACE3 控制器均已在 Asahi Linux 中正常工作。这项工作为 Linux 在 Apple Silicon 上的硬件兼容性提供了重要进展。

hackernews · pizzaiolo · 8月26日 22:35 · [社区讨论](https://news.ycombinator.com/item?id=49456851)

**「背景」** Asahi Linux 是一个致力于在苹果 Apple Silicon 芯片的 Mac 上原生运行 Linux 的开源项目，通过逆向工程和自研引导加载程序（如 m1n1）逐步实现对 M 系列芯片的支持。该项目曾在开发组织调整中遇到一些障碍，M3 芯片的支持也经历了从仅能启动到逐步完善的过程，早期 M3 Mac 甚至无法使用 GPU 加速。本次进展报告中提到的 USB 3.0 和 Thunderbolt 支持，是在此前完成基础启动和硬件适配的基础上，进一步扩展 M3 系列设备外设兼容性的重要一步。

**「影响」** 这一里程碑意味着 M3 系列 Mac 用户现在可以在 Linux 上使用 USB 3.0 和 Thunderbolt 外设，填补了此前缺失的高速 I/O 支持；值得注意的是，Asahi Linux 在 Apple Silicon 上的运行仍受制于苹果特有的引导和固件机制，官方已提醒用户暂缓升级 macOS 27 Golden Gate 以避免兼容问题。

**「社区讨论」** 评论者普遍赞赏 Asahi Linux 团队的逆向工程成果，但也有人质疑在 Intel 和 AMD 功耗效率不断追赶的情况下，是否仍有必要在 M 系列笔记本上运行 Linux；还有用户希望尽快支持 M4，并期待电源管理优化以改善电池续航。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.howtogeek.com/asahi-linux-reorganization-m3-m4-mac-support/">Asahi Linux Gets a Reboot, Still Working On M 3 &amp; M4 Mac Support</a></li>
<li><a href="https://appleinsider.com/articles/26/01/27/its-not-usable-yet-but-asahi-linux-runs-on-m3-macs-now">M 3 Macs can now run Asahi Linux , albeit with no GPU support</a></li>
<li><a href="https://www.linuxencaja.net/en/asahi-linux-continues-apple-m3-support-m1n1-bootloader-evolves-to-rust/">Asahi Linux Boosted: m1n1 Switches to Rust for the Apple M 3</a></li>
<li><a href="https://linuxiac.com/asahi-linux-users-told-to-avoid-macos-27-golden-gate-for-now/">Asahi Linux Users Told to Avoid macOS 27 Golden Gate for Now</a></li>

</ul>
</details>

**标签**: `#asahi linux`, `#apple silicon`, `#open source`, `#linux`, `#hardware support`

---

<a id="item-tech-news-4"></a>
### [Tailcat：在 Tailscale 加密数据面上重制 netcat](https://github.com/tailscale/tailcat) ⭐️ 7.0/10

Tailscale 推出了官方工具 Tailcat，一个类似于 netcat 的命令行工具，但把数据传输放在 Tailscale 的加密数据平面上，从而实现安全的点对点传输。它让用户可以在已接入同一 Tailnet 的设备之间直接发送数据，利用 Tailscale 的加密和身份体系，而不必像传统 netcat 那样手动处理加密或暴露端口。Tailcat 是专门为 Tailscale 生态设计的实用工具，并提供了 Nix 安装/开发环境。官方团队用 Tailcat 做了一个 Minecraft 模组演示作为趣味用例，说明它可作为自定义应用的安全传输层。

hackernews · nderjung · 8月26日 17:42 · [社区讨论](https://news.ycombinator.com/item?id=49452990)

**「背景」** netcat 是一个传统的网络调试工具，可以在两个端点之间传输原始数据。Tailscale 通常通过控制平面协调设备并建立加密的网状网络，其数据平面负责实际的加密流量转发。Tailcat 将 netcat 的功能移植到 Tailscale 的数据平面上，但不需要 Tailscale 的控制平面或账户，从而在设备间建立安全的点对点隧道。

**「影响」** Tailscale 用户可立即用 Tailcat 在 Tailnet 内设备间进行加密点对点数据传输，无需手动配置端口转发或公网 IP；社区已用它实现 Minecraft 模组的传输层原型。

**「社区讨论」** 评论者将其与 Iroh、Tor 的 .onion 服务等既有 p2p/匿名方案对比，认为在 IPv6 尚未普及且存在 CGNAT 的网络环境中，这类工具是有价值的补充。还有人询问 Nix 是否已是 Tailscale 的标准开发环境，并指出 Minecraft 模组更像趣味演示而非正式产品。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/tailscale/tailcat">GitHub - tailscale / tailcat : like netcat , but over Tailscale &#x27;s data plane...</a></li>
<li><a href="https://www.pradha.id/read/tailscale-releases-tailcat-secure-point-to-point-tunnels-without-a-control-plane">Tailcat : Secure P2P Tunnels Without a Tailscale Account | Pradha</a></li>

</ul>
</details>

**标签**: `#Tailscale`, `#networking`, `#netcat`, `#secure tunneling`, `#peer-to-peer`

---

<a id="item-tech-news-5"></a>
### [美国暂停移民签证申请引发科技人才担忧](https://www.wsj.com/politics/policy/u-s-state-department-pauses-immigrant-visa-applications-25b31b23) ⭐️ 7.0/10

美国国务院已暂停处理移民签证申请，直接影响依赖 H-1B 等技术移民的科技行业。有评论者报告，一名 H-1B 员工返回印度后因无法预约美国使馆面签而无法返美，下一次可预约日期已排到明年。此次暂停没有给出新的预约日期，导致签证续签和入境安排陷入停滞，增加员工与雇主的不确定性。在 AI 等领域对人才需求旺盛的背景下，该政策可能进一步削弱美国对全球技术人才的吸引力。

hackernews · sss111 · 8月26日 17:22 · [社区讨论](https://news.ycombinator.com/item?id=49452709)

**「背景」** 美国国务院已暂停全球范围内的移民签证申请受理，以便对领事官员进行“深入培训”，这是特朗普政府收紧移民政策的一部分。《金融时报》援引国务院发言人的消息报道，英国《卫报》也确认此举旨在限制可能依赖美国公共福利的申请者。移民签证（包括家庭团聚和部分职业移民）与 H-1B 等工作签证不同，但暂停受理会进一步加剧签证预约积压，影响依赖海外雇员续签或入境的企业与家庭。

**「影响」** 最直接受影响的是需要离境续签或申请移民签证的 H-1B 等技术工人及其雇主；评论中的案例显示，员工可能因无法预约面签而长期滞留海外，企业也面临关键人才缺位。由于暂停未给出恢复日期，影响持续时间尚不确定。

**「社区讨论」** 评论者普遍认为政策执行方式显得“故意残酷”且缺乏合理性；有人指出合法签证持有者在美国有房产和家庭却被困在国外，也有人认为这会在 AI 人才竞争激烈时赶走顶尖人才。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://english.news.cn/20260826/c49f3caafc5b407d950d226295674fbe/c.html">U . S . State Department pauses immigrant visa applications ...</a></li>
<li><a href="https://www.theguardian.com/us-news/2026/aug/25/us-immigrant-visa-application-trump-crackdwon">US halts all immigrant visa applications amid... | The Guardian</a></li>

</ul>
</details>

**标签**: `#immigration`, `#visa`, `#tech-industry`, `#talent`, `#policy`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [Meta 就重磅诉讼达成和解，最高支付 170 亿美元并调整青少年平台规则](https://www.economist.com/business/2026/08/26/meta-settles-its-blockbuster-trial-for-up-to-17bn) ⭐️ 8.0/10

据《经济学人》报道，Meta 已就一场重磅诉讼达成和解，将支付最高 170 亿美元，并调整青少年使用其平台的方式。

rss · The Economist · 8月26日 22:58

**「背景」** 这起诉讼由 47 个州的总检察长提起，指控 Meta 旗下 Instagram 和 Facebook 助长青少年社交媒体成瘾；作为和解，Meta 同意支付最高 170 亿美元，并调整青少年使用平台的规则。

**「影响」** 受此和解影响，美国 18 岁以下的青少年在 Facebook 和 Instagram 上将被设置每日两小时的使用上限和夜间禁用时段，且这些限制只能由家长移除。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.npr.org/2026/08/26/nx-s1-5944781/meta-settlement-child-safety-lawsuit">Meta, states agree to $17 billion settlement in child safety trial : NPR</a></li>
<li><a href="https://www.latimes.com/business/story/2026-08-26/meta-reaches-17-billion-settlement-with-states-in-landmark-trial-over-teen-social-media-addiction">Meta trial leads to $17 billion payment and overhaul of Facebook and Instagram - Los Angeles Times</a></li>
<li><a href="https://www.kron4.com/news/technology-ai/meta-reaches-17b-settlement-in-landmark-trial-over-teen-social-media-addiction/">Meta reaches $17B settlement in landmark trial over teen social media addiction | KRON4</a></li>
<li><a href="https://www.aljazeera.com/economy/2026/8/26/meta-agrees-to-settlement-platform-changes-in-youth-addiction-case">Meta agrees to settlement, platform changes in youth... | Al Jazeera</a></li>

</ul>
</details>

**标签**: `#Meta`, `#settlement`, `#regulation`, `#social media`, `#teen safety`

---

<a id="item-finance-news-2"></a>
### [俄罗斯为何故意让卢布贬值](https://www.economist.com/finance-and-economics/2026/08/26/why-is-russia-deliberately-weakening-its-currency) ⭐️ 8.0/10

据《经济学人》报道，俄罗斯正在故意让卢布贬值，原因是强势卢布不利于国家预算。

rss · The Economist · 8月26日 18:28

**「背景」** 俄罗斯财政预算依赖出口收入，而卢布汇率偏强会使以美元等外币计价的出口收入换成卢布后缩水。为此，俄财政部 8 月 5 日宣布将每日购买外汇和黄金的规模提高约 20%，由 7 月的 54 亿卢布增至 65 亿卢布，以推动卢布走弱。

**「影响」** 卢布贬值将直接缓解俄罗斯联邦预算压力：以欧元计价的出口税和自然资源税折算成卢布后的收入增加，而养老金等支出随通胀上升的幅度小于收入增幅，有助于避免财政赤字扩大。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.economist.com/finance-and-economics/2026/08/26/why-is-russia-deliberately-weakening-its-currency">Why is Russia deliberately weakening its currency?</a></li>
<li><a href="https://www.newsweek.com/what-does-rubles-sharp-fall-mean-russias-economy-1992933">What Ruble to USD Fall Means for Russia&#x27;s Economy - Newsweek</a></li>
<li><a href="https://janiskluge.substack.com/p/the-ruble-is-too-strong-really">The ruble is too strong - really - by Janis Kluge - Russianomics</a></li>

</ul>
</details>

**标签**: `#Russia`, `#rouble`, `#monetary policy`, `#budget`, `#currency`

---

<a id="item-finance-news-3"></a>
### [英伟达季度营收 962 亿美元，首次提前一年给出 70%增长指引](https://mp.weixin.qq.com/s/JTZ_ZJ_pn5vgrI_1QUyWNw) ⭐️ 8.0/10

英伟达发布 2027 财年第二季度财报：营收 962.21 亿美元，同比增长 106%，其中数据中心收入 890 亿美元，同比增长 117%。首席财务官首次提前一年给出 2028 财年营收同比增长约 70%的指引，并表示该增速受供给限制；新一代 Vera Rubin 平台本月起量产出货，预计第三季度贡献约 20%的数据中心收入。

telegram · zaihuapd · 8月27日 08:51

**「背景」** 英伟达 2027 财年第二季度指截至 2026 年 7 月的季度，营收为 962.2 亿美元，其中数据中心收入 890 亿美元、同比增长 117%。财报还显示，下一代平台 Vera Rubin 已在合作伙伴处进入量产爬坡，预计三季度占数据中心收入约 20%。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nvidianews.nvidia.com/news/nvidia-announces-financial-results-for-second-quarter-fiscal-2027">NVIDIA Announces Financial Results for Second Quarter Fiscal 2027 | NVIDIA Newsroom</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/nvidia-q2-earnings-call-highlights-230417656.html">NVIDIA Q2 Earnings Call Highlights</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#earnings`, `#AI infrastructure`, `#data center`, `#semiconductor industry`

---