---
layout: default
title: "Horizon Summary: 2026-07-25 (ZH)"
date: 2026-07-25
lang: zh
---

> 从 37 条内容中筛选出 10 条重要资讯。

---

1. [Claude Opus 5 发布，无数据保留要求](#item-1) ⭐️ 9.0/10
2. [安防摄像头登录页泄露 GitHub 管理员令牌](#item-2) ⭐️ 8.0/10
3. [科技巨头警告不要过度监管开放权重 AI 模型](#item-3) ⭐️ 8.0/10
4. [菲尔兹奖得主加盟 OpenAI，称 AI 改变数学研究](#item-4) ⭐️ 8.0/10
5. [Claude Opus 5 登陆 GitHub Copilot](#item-5) ⭐️ 8.0/10
6. [英伟达通知 AIC 合作伙伴 GPU 涨价，出货暂停](#item-6) ⭐️ 8.0/10
7. [中国对离岸信托收益征收 20%税，堵住避税漏洞](#item-7) ⭐️ 8.0/10
8. [Postgres 的 LISTEN/NOTIFY 实际上扩展性很好](#item-8) ⭐️ 7.0/10
9. [Opus 5 登顶 AI 排行榜，成本与审查引发争议](#item-9) ⭐️ 7.0/10
10. [WeLM 617B MoE 隐式缩放](#item-10) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Claude Opus 5 发布，无数据保留要求](https://www.anthropic.com/news/claude-opus-5) ⭐️ 9.0/10

Anthropic 发布了其最新前沿 AI 模型 Claude Opus 5，该模型引入了通用访问无数据保留要求的政策，并在图像转 HTML 等任务上表现更佳。 取消数据保留要求使得 Opus 5 适用于具有严格数据隐私政策的企业部署，其性能提升可能改变领先 AI 模型间的竞争格局。 与 Anthropic 之前有 30 天数据保留政策的 Fable 模型不同，Opus 5 对通用访问没有此类要求。早期测试表明，Opus 5 在图像转 HTML 任务上优于 Fable，同时在写作风格上保留了一些典型的“Claude 风格”。

hackernews · alvis · 7月24日 16:57 · [社区讨论](https://news.ycombinator.com/item?id=49038433)

**背景**: 模型路由是一种系统，它根据成本、延迟和质量等因素动态选择最适合每个请求的 AI 模型。系统卡是一份文档，详细说明模型的能力、安全评估和局限性。这些概念之所以相关，是因为 Opus 5 的发布引发了关于模型之间路由的讨论，企业希望平衡性能、成本和数据政策。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www-cdn.anthropic.com/c5fbac3f0b1280a933ebd26d3cb8bb9f5bdeaf48/Claude+Opus+5+System+Card.pdf">Claude Opus 5 System Card</a></li>
<li><a href="https://dapto.ai/blog/how-ai-model-routing-works/">How AI Model Routing Works: Why One Model Isn't Enough Anymore | Dapto Blog</a></li>

</ul>
</details>

**社区讨论**: 评论者强调了无数据保留政策对企业采用的重要性，一位用户指出 Opus 5 的图像转 HTML 转换似乎比之前的最佳模型 Fable 更准确。另一条评论指出，具有不同选项的模型激增正在推动模型路由服务的快速增长。

**标签**: `#AI`, `#LLM`, `#Claude`, `#Anthropic`, `#model release`

---

<a id="item-2"></a>
## [安防摄像头登录页泄露 GitHub 管理员令牌](https://hhh.hn/hanwha-github-token/) ⭐️ 8.0/10

发现一款安防摄像头的登录页面硬编码了 GitHub 管理员令牌，该令牌可能允许未经授权访问厂商的 GitHub 仓库。 这起事件凸显了物联网固件中严重的安全疏忽，此类硬编码凭据可能导致供应链攻击、数据泄露或代码完整性受损。 该令牌直接嵌入在摄像头的登录页面中，任何检查页面源代码的人都能获取。具有管理员权限的 GitHub 令牌可以控制仓库访问、工作流和组织设置。

hackernews · hhh · 7月24日 11:54 · [社区讨论](https://news.ycombinator.com/item?id=49034292)

**背景**: GitHub 管理员令牌是拥有高级权限的个人访问令牌，可执行推送到受保护分支或管理团队等操作。硬编码凭据是嵌入源代码或配置文件中的认证密钥，属于生产系统中绝对不应使用的安全反模式。在物联网设备中，由于成本削减和安全关注不足，这种做法不幸地很常见。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens">Managing your personal access tokens - GitHub Docs</a></li>
<li><a href="https://cwe.mitre.org/data/definitions/798.html">CWE - CWE-798: Use of Hard - coded Credentials (4.20)</a></li>

</ul>
</details>

**社区讨论**: 评论者批评厂商出货硬编码凭据，有人建议将摄像头置于无互联网访问的隔离 VLAN 中。一位用户指出固件中还嵌入了美国战争部的 IP 地址，称这是更大的问题。

**标签**: `#security`, `#IoT`, `#vulnerability`, `#GitHub token`, `#hardcoded credentials`

---

<a id="item-3"></a>
## [科技巨头警告不要过度监管开放权重 AI 模型](https://www.cnbc.com/2026/07/24/nvidia-microsoft-meta-open-weight-ai-models.html) ⭐️ 8.0/10

英伟达（Nvidia）、微软（Microsoft）和 Meta 联合致信美国政府，警告过度监管开放权重 AI 模型可能会损害美国在人工智能领域的领导地位。 这表明业界对开放权重模型的潜在监管进行了重大反击，可能影响全球 AI 竞争以及开源创新与安全考量之间的平衡。 该信强调，开放权重模型（发布训练参数但不包含完整训练数据）对美国 AI 进步至关重要。支持者认为限制措施将使中国等国的闭源竞争对手受益。

hackernews · louiereederson · 7月24日 13:32 · [社区讨论](https://news.ycombinator.com/item?id=49035303)

**背景**: 开放权重 AI 模型仅发布训练后的参数权重，而开源模型则提供完整代码、数据和训练方法。这使得开放权重模型透明度较低但更易分发。关于其监管的辩论日益激烈，Anthropic 和 OpenAI 等公司主张更严格控制，而另一些公司则警告称这可能扼杀创新并让外国竞争对手乘虚而入。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://neysa.ai/blog/open-weights-open-source/">Open Weights vs Open Source: What's the Real Difference? - neysa.ai</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you've been told - Open Source Initiative</a></li>

</ul>
</details>

**社区讨论**: Hacker News 评论者大多支持开放权重模型，并批评 Anthropic 和 OpenAI 为保护利润而推动监管。一些人将这种情况比作 SOPA 抗议，指出对限制开放访问的广泛反对。

**标签**: `#AI Regulation`, `#Open-Source AI`, `#Open-Weight Models`, `#Technology Policy`, `#Industry Lobbying`

---

<a id="item-4"></a>
## [菲尔兹奖得主加盟 OpenAI，称 AI 改变数学研究](https://www.infoq.cn/article/7rHl2bfzSq4kNVPQ9219?utm_source=rss&utm_medium=article) ⭐️ 8.0/10

一位菲尔兹奖得主离开学术界加入 OpenAI，声称 AI 的进步使数学家这份工作难以为继，并且不再招收研究生。 此举标志着范式转变：顶尖数学人才流向工业界 AI，可能加速 AI 驱动的数学发现，但也引发对学术数学未来和职业可持续性的担忧。 这位数学家特别提到，由于 AI 的快速进步，招收研究生不再可行。OpenAI 专注于通用人工智能，此次招募可能旨在利用数学专长进行 AI 对齐或推理研究。

rss · InfoQ 中文站 · 7月24日 19:30

**背景**: 菲尔兹奖是数学界最高荣誉，每四年颁发给 40 岁以下的数学家。OpenAI 是领先的 AI 研究机构，开发了 GPT-4 等模型。这一决定反映了顶尖研究者从学术界向私营 AI 公司流动的趋势，原因是更好的资源和影响力。

**社区讨论**: 社区观点不一：一些人赞赏对 AI 潜力的认可，而另一些人则为学术界人才流失感到惋惜，并担心纯数学价值被贬低。有人担忧没有这些杰出人物，数学研究的长期健康将受影响。

**标签**: `#AI`, `#mathematics`, `#OpenAI`, `#academia`, `#job displacement`

---

<a id="item-5"></a>
## [Claude Opus 5 登陆 GitHub Copilot](https://github.blog/changelog/2026-07-24-claude-opus-5-is-now-available-in-github-copilot) ⭐️ 8.0/10

这一集成使开发者能够直接在 IDE 中使用最先进的推理模型，有望提高需要仔细思考和工具编排的任务的生产力。 Claude Opus 5 专为需要多步推理和可靠工具使用的复杂编码工作流而设计，基于 Anthropic 的宪法 AI 方法构建。

rss · GitHub Changelog · 7月24日 16:40

**背景**: Claude 是 Anthropic 开发的一系列大型语言模型，使用宪法 AI 进行训练以增强伦理对齐。自 Claude 3 起，每一代都包含三个级别：Haiku、Sonnet 和 Opus，其中 Opus 能力最强。GitHub Copilot 是一个 AI 驱动的代码补全工具，将大型语言模型集成到开发环境中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-opus-5">Introducing Claude Opus 5 \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Opus">Claude Opus</a></li>

</ul>
</details>

**标签**: `#AI`, `#GitHub Copilot`, `#Claude`, `#coding`, `#LLM`

---

<a id="item-6"></a>
## [英伟达通知 AIC 合作伙伴 GPU 涨价，出货暂停](https://finance.sina.com.cn/tech/discovery/2026-07-24/doc-iniiwvke9215911.shtml) ⭐️ 8.0/10

英伟达已通知所有 AIC 合作伙伴 GPU 涨价，具体政策将于 8 月确定。各大显卡厂商已暂停出货并收紧 RTX 50 系列供应，从 7 月下旬开始。 此次涨价覆盖基于 GDDR7 的 Blackwell 旗舰产品线和基于 GDDR6 的 GeForce 消费级产品线，可能推高 AI/ML 硬件和消费者的成本。供应收紧可能加剧市场上的 GPU 短缺。 显存成本涨幅显著：8GB、12GB 和 16GB 显卡的显存成本分别增加约 76 美元、114 美元和 152 美元。此外，RTX 50 SUPER 系列因 GDDR7 采购价过高而暂缓发售。

telegram · zaihuapd · 7月24日 14:21

**背景**: AIC 是指'Add-in-Card'合作伙伴，即生产基于 NVIDIA 显卡的板卡制造商，如华硕、微星和技嘉。GDDR7 是最新的图形内存技术，提供更快的速度，而 Blackwell 是 NVIDIA 当前的 GPU 架构，用于消费级和数据中心产品。涨价源于内存芯片成本上升，部分原因是 AI 相关的内存需求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.guru3d.com/story/nvidia-raises-gddr7-and-gddr6-memory-pricing-for-geforce-rtx-gpus/">NVIDIA Raises GDDR 7 and GDDR6 Memory Pricing for GeForce RTX...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Blackwell_(microarchitecture)">Blackwell (microarchitecture) - Wikipedia</a></li>
<li><a href="https://www.tomshardware.com/pc-components/ram/ai-memory-shortage-is-now-increasing-the-price-of-cars-gm-warns-of-vast-cost-increases-byd-hikes-driver-assistance-prices-20-percent">AI memory shortage is now increasing the price of... | Tom's Hardware</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#GPU`, `#price increase`, `#hardware`, `#AI/ML`

---

<a id="item-7"></a>
## [中国对离岸信托收益征收 20%税，堵住避税漏洞](https://liaoning.chinatax.gov.cn/art/2026/7/24/art_5869_7823.html) ⭐️ 8.0/10

2026 年 7 月 24 日，中国财政部和税务总局联合发布第 21 号公告，要求居民个人对装入离岸信托的财产以及信托存续期间产生的全部收益申报缴纳个人所得税，无论是否分配，统一按增值额的 20%征税。 该法规关闭了离岸信托收益被无限期递延纳税的长期漏洞，直接影响使用此类结构进行税收筹划的中国高净值居民。这标志着中国在加强离岸资产申报和税务合规方面的更广泛努力。 该规则采用穿透式做法：所有信托收益每年归集到居民委托人名下，设立环节按‘财产转让所得’适用 20%税率，终止环节按‘利息、股息、红利所得’计税。设有 90 天宽限期，纳税人对 2026 年前装入和 2026 年前的信托收益进行自愿申报补缴，不加收滞纳金。

telegram · zaihuapd · 7月25日 00:31

**背景**: 离岸信托通常被富裕个人用于在税收或隐私法律优惠的司法管辖区持有资产。此前，中国税法对未分配的信托收益征税不明确，居民可通过将收益留存于信托内来递延或逃避纳税。新规明确对所有信托收益（无论是否分配）实行按年征税，有效消除了递延利益。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.news.cn/politics/20260724/206e5905c9204c62a0fdb918dfd1bc5a/c.html">两部门明确离岸信托个税事项-新华网</a></li>
<li><a href="https://www.peopleapp.com/column/30052749094-500007615389">离岸信托需缴纳个人所得税，官方解读→_人民日报</a></li>
<li><a href="https://www.yicai.com/news/103291247.html">两部门就 离 岸 信 托 个人所得 税 有关事项答记者问</a></li>

</ul>
</details>

**标签**: `#tax regulation`, `#offshore trust`, `#China`, `#personal finance`, `#compliance`

---

<a id="item-8"></a>
## [Postgres 的 LISTEN/NOTIFY 实际上扩展性很好](https://www.dbos.dev/blog/postgres-listen-notify-scalability) ⭐️ 7.0/10

一项详细的性能分析表明，PostgreSQL 的 LISTEN/NOTIFY 每秒可处理超过 60,000 条通知，推翻了它无法扩展的普遍看法。 这一发现让考虑使用 LISTEN/NOTIFY 实现实时功能和轻量消息传递的开发者放心，表明在正确使用时它适用于许多应用。 该基准测试在 100 个并发连接下达到了约每秒 60,000 条通知，作者指出仅在极端负载（如 10,000 个连接）下性能才会下降。

hackernews · KraftyOne · 7月24日 19:05 · [社区讨论](https://news.ycombinator.com/item?id=49040296)

**背景**: PostgreSQL 的 LISTEN 和 NOTIFY 命令允许数据库客户端之间的异步通知。一个普遍误解（部分源于早期版本的锁定问题）认为该机制无法扩展。这篇文章提供了更新的基准来反驳这一说法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/sql-notify.html">PostgreSQL: Documentation: 18: NOTIFY</a></li>
<li><a href="https://www.postgresql.org/docs/current/sql-listen.html">PostgreSQL: Documentation: 18: LISTEN</a></li>
<li><a href="https://www.cybertec-postgresql.com/en/listen-notify-automatic-client-notification-in-postgresql/">LISTEN / NOTIFY : Automatic client notification in PostgreSQL</a></li>

</ul>
</details>

**社区讨论**: 评论者一致认为“扩展”是一个连续体，而非二元概念，并对真实数据表示赞赏。一位评论者分享了一个使用 LISTEN/NOTIFY 构建可扩展队列的成功案例。另一位则链接了声称它无法扩展的相反观点文章，引发了关于正确使用和配置的讨论。

**标签**: `#postgresql`, `#database`, `#notifications`, `#scalability`, `#performance`

---

<a id="item-9"></a>
## [Opus 5 登顶 AI 排行榜，成本与审查引发争议](https://artificialanalysis.ai/models) ⭐️ 7.0/10

Anthropic 的 Claude Opus 5 在 Artificial Analysis Intelligence 排行榜上夺得榜首，以 61 分的智力指数超越其他模型。然而，该模型因高昂的成本以及因激进的审查机制导致的可靠性问题而受到批评。 此次排行榜更新为比较顶尖 AI 模型提供了关键基准，但社区讨论中凸显的智力、成本与可靠性之间的权衡，对于开发者和企业选择模型至关重要。这强调了原始性能分数并不能反映全貌，尤其是在审查机制和定价可能限制实际用途的情况下。 该排行榜采用 AA Intelligence Index v4.1，包含九项评估指标，包括 GDPval-AA、GPQA Diamond 和 AA-Omniscience。Opus 5 的 61 分仅略高于 GPT-5.6 Sol Max 的 59 分，但 GPT-5.6 每任务成本大约只有 Opus 5 的一半。

hackernews · aarondong · 7月24日 19:45 · [社区讨论](https://news.ycombinator.com/item?id=49040741)

**背景**: Artificial Analysis Intelligence 排行榜根据综合智力指数对大型语言模型进行排名，该指数衡量推理、知识和可靠性。Anthropic 的 Claude Opus 5 于 2026 年 7 月发布，是比更大的 Fable 5 模型更具成本效益且限制更少的替代品，但其价格仍然很高。社区指出，Claude 模型通常包含严格的安全措施，可能拒绝或降级响应，从而影响可靠性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/leaderboards/models">LLM Leaderboard - Comparison of AI models from OpenAI, Anthropic...</a></li>
<li><a href="https://techcrunch.com/2026/07/24/anthropic-launches-opus-5/">Anthropic launches Opus 5 | TechCrunch</a></li>
<li><a href="https://www.cnbc.com/2026/07/24/anthropic-claude-opus-5-ai-fable-5-cost.html">Anthropic's Claude Opus 5 AI model rivals Fable 5 and is cheaper</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了复杂的感受：一些人批评 Opus 5 的审查机制使其不可靠，而另一些人则指出 GPT-5.6 以一半的成本提供了可比的性能。一位用户指出，Opus 5 在不同努力级别下仍优于最大努力的 GPT-5.6，但成本仍然是一个重大缺点。

**标签**: `#AI`, `#leaderboard`, `#Claude`, `#models`, `#benchmarking`

---

<a id="item-10"></a>
## [WeLM 617B MoE 隐式缩放](https://mp.weixin.qq.com/s?__biz=MzI3MTA0MTk1MA==&mid=2652714734&idx=1&sn=7e98659aa2ab44778c0d5587a1aa8a84) ⭐️ 7.0/10

微信团队提出了一种新的 AI 缩放定律，即隐式缩放，并通过一个 617B 参数的混合专家模型 WeLM 进行了验证。 这一发现挑战了仅依赖增加参数和数据量的传统缩放定律，可能为构建大型语言模型提供更高效的路径。通过降低计算成本的同时保持或提升性能，它将对 AI 研究产生重大影响。 WeLM 617B MoE 模型采用稀疏激活，以适度资源实现高性能；隐式缩放定律描述了通过架构优化而非单纯规模带来的性能提升。该团队声称这是 AI 的“第三条缩放定律”，区别于传统的基于算力和数据的缩放定律。

rss · 新智元 · 7月24日 04:33

**背景**: 神经缩放定律描述了模型性能随参数、数据或算力增加而提升的规律。混合专家架构是一种每个词元仅激活部分参数的结构，能够以较低计算成本实现大模型容量。WeLM 是微信团队开发的一系列预训练语言模型，专注于中文理解与生成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2209.10372">WeLM: A Well-Read Pre-trained Language Model for Chinese WeLM Blog WeLM: A Well-Read Pre-trained Language Model for Chinese WeLM Blog SoftVein-WELM: A Weighted Extreme Learning Machine Model for ... A human breast cancer-derived xenograft and organoid platform ... WeChat launches Xiao Wei AI assistant powered by WeLM and ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Neural_scaling_law">Neural scaling law - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained - Hugging Face</a></li>

</ul>
</details>

**标签**: `#scaling laws`, `#large language models`, `#MoE`, `#WeChat`, `#AI research`

---