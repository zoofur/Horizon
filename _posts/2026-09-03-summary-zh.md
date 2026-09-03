---
layout: default
title: "Horizon Summary: 2026-09-03 (ZH)"
date: 2026-09-03
lang: zh
---

> 从 47 条内容中筛选出 10 条重要资讯。

---

**科技新闻**
1. [Gemini 3.8 Flash 与 Flash Cyber 发布：低成本 Flash 模型基准表现亮眼](#item-tech-news-1) ⭐️ 8.0/10
2. [三网站炮制 21.5 万条“最佳软件”页面，Perplexity 等 AI 工具频繁引用](#item-tech-news-2) ⭐️ 7.0/10
3. [BMC 漏洞或让数千台服务器面临硬件级入侵风险](#item-tech-news-3) ⭐️ 7.0/10
4. [Cursor 推出面向智能体的 GitHub 替代方案 Origin](#item-tech-news-4) ⭐️ 7.0/10

**财经新闻**
1. [谷歌胜诉，免于被强制拆分广告技术业务](#item-finance-news-1) ⭐️ 8.0/10
2. [数据中心为何成为美国中期选举的政治热点](#item-finance-news-2) ⭐️ 7.0/10
3. [科技助力，厄瓜多尔成为养虾大国](#item-finance-news-3) ⭐️ 7.0/10
4. [报道：月之暗面秘密递交港股 IPO 申请，新一轮融资投前估值 500 亿美元](#item-finance-news-4) ⭐️ 7.0/10

**科技博客**
1. [1967 版蜘蛛侠片头真人化：MiniMax H3 工作流解析](#item-tech-blog-1) ⭐️ 8.0/10

**AI 创作者雷达**
1. [Meta 发布 Muse Spark 1.3，带来 anti-slop 过滤等 UI/SVG 生成改进](#item-ai-creator-1) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Gemini 3.8 Flash 与 Flash Cyber 发布：低成本 Flash 模型基准表现亮眼](https://blog.google/innovation-and-ai/models-and-research/gemini-models/3-8-flash-and-3-8-flash-cyber/) ⭐️ 8.0/10

谷歌 DeepMind 在官方博客发布 Gemini 3.8 Flash 与 Gemini 3.8 Flash Cyber 模型，对应的模型卡已在 DeepMind 网站公开。作为低成本 Flash 系列的新一代，该模型以较低成本和较快速度为主打，社区初步测试显示它在 HTML/JavaScript 生成和若干编码或智能体基准上表现抢眼；评论者引用 Artificial Analysis 数据称其智能分为 59，与 Opus 5 medium 持平，并在 Deepswe 排行榜上超过 Opus 5。目前 Gemini Web 仍使用 3.6 Flash，尚不清楚 3.8 Flash 何时进入面向普通用户的 Gemini 界面。开发者 Simon Willison 展示了约 13 秒、约 1.8 美分即可根据“make me a cool thing in html”提示生成一个可运行的 HTML 原型，发布后 Hacker News 上的讨论相当热烈。

hackernews · bratao · 9月2日 15:12 · [社区讨论](https://news.ycombinator.com/item?id=49537553)

**「背景」** Gemini 3.8 Flash 是 Google DeepMind 发布的 Flash 系列轻量模型之一，该系列面向对速度和成本敏感的推理、智能体与开发任务，与前代 3.7 Flash 同类定位。3.8 Flash Cyber 是专门面向网络安全场景的变体，主打自主发现漏洞并生成可用补丁，Google 将其称为“最强大的网络安全模型”，并通过 Fairwind 计划向受信任的防御者提供。定价方面，3.8 Flash 保持与 3.7 Flash 相同的介绍价：每百万输入 token 0.75 美元、每百万输出 token 3.75 美元。

**「影响」** 对需要低成本完成前端原型、编码辅助或浏览器相关任务的开发者，3.8 Flash 提供了一个基准实力接近高端模型的低价选项，但实际使用表现仍需在各自工作流中进一步验证。

**「社区讨论」** 社区整体看好该模型的速度和 HTML/JavaScript 生成能力，Simon Willison 的实测展示了低至 1.8 美分、13 秒生成 HTML 作品的效果；同时也有评论者指出 Gemini Web 尚未切换到 3.8 Flash，并认为 3.8 在低思考档位的表现相比 3.7 可能有回退。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/3-8-flash-and-3-8-flash-cyber/">Introducing Gemini 3.8 Flash and 3.8 Flash Cyber - The Keyword</a></li>
<li><a href="https://cybersecuritynews.com/gemini-3-8-flash-cyber/">Google Launches Gemini 3.8 Flash Cyber to Identify and Auto ...</a></li>
<li><a href="https://arstechnica.com/ai/2026/09/google-releases-gemini-3-8-flash-its-third-flash-model-in-six-weeks/">Google releases Gemini 3.8 Flash, its third Flash model in ...</a></li>

</ul>
</details>

**标签**: `#Gemini`, `#AI models`, `#Google`, `#machine learning`, `#developer tools`

---

<a id="item-tech-news-2"></a>
### [三网站炮制 21.5 万条“最佳软件”页面，Perplexity 等 AI 工具频繁引用](https://trellner.com/reports/manufactured-sources-behind-ai-recommendations/) ⭐️ 7.0/10

一项调查发现，wifitalents.com、worldmetrics.org 和 gitnux.org 三个内容农场网站共制造了 215,128 个“最佳软件”页面，并被 Perplexity 等 AI 搜索工具当作可靠来源引用。这些页面依赖 SEO 批量生成，构成低质量的 AI 训练与检索语料，威胁 AI 回答的可信度。Semrush 估算显示，三个域名分别在 7 月 15 日、7 月 27 日和 8 月 20 日达到 18000、8000、8000 次自然搜索访问峰值，随后均呈下降趋势。调查还表明，AI 工具引用这类自动生成内容时，用户可能难以分辨哪些推荐真正来自人工评测，加剧 AI 搜索结果被内容农场的“制造权威”污染的问题。

hackernews · jakobgreenfeld · 9月2日 13:59 · [社区讨论](https://news.ycombinator.com/item?id=49536375)

**「背景」** Perplexity 等 AI 搜索引擎在回答“最佳软件”类问题时，会引用大量网页作为依据。近期一项调查发现，WorldMetrics、WifiTalents、Gitnux 等三个疑似关联的网站生成了超过 21.5 万个“最佳软件”推荐页面，这些页面并非面向人类读者，而是专门针对 AI 模型抓取与引用而构建。调查还显示，在 380 个软件类别中，Perplexity 的 Sonar 模型所引用的来源有 59.8% 来自流量排名 10 万名之外的网站，其中不少就是这类自动生成的内容农场页面，这引发了对 AI 搜索与训练数据可靠性的担忧。

**「影响」** 使用 Perplexity 等 AI 搜索工具的用户，在查询“最佳软件”类问题时可能收到由 SEO 内容农场批量生成、缺乏真实评测依据的推荐页面；这种影响还会扩散到依赖 AI 输出进行决策或二次创作的开发者、记者和研究者的工作流程中。

**「社区讨论」** Hacker News 评论普遍认可调查揭示的问题，并补充了更多佐证：有用户指出 LLM 倾向于偏爱自己生成的答案，甚至会把不存在的“Foobar 广场”当作当地街头美食地标并添加生动细节；另一用户表示 Perplexity 为追求响应速度牺牲结果质量，返回的链接和参考资料越来越差。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://trellner.com/reports/manufactured-sources-behind-ai-recommendations/">Three sites made 215,128 &quot;best software&quot; pages for AI ...</a></li>
<li><a href="https://www.explainx.ai/blog/ai-recommendation-sources-manufactured-geo-farms-trellner-2026">215K Fake &quot;Best Software&quot; Pages Feed AI Answers (2026 ...</a></li>

</ul>
</details>

**标签**: `#AI search reliability`, `#SEO spam`, `#content farms`, `#LLM hallucinations`, `#Perplexity`

---

<a id="item-tech-news-3"></a>
### [BMC 漏洞或让数千台服务器面临硬件级入侵风险](https://www.infoq.cn/article/PfVEf7xZJBSkrYib9R8z?utm_source=rss&amp;utm_medium=article) ⭐️ 7.0/10

相关报道标题指出，BMC（基板管理控制器）漏洞可能使数千台服务器面临硬件级入侵风险。不过目前可获取的内容仅有标题和原文链接，缺乏具体漏洞编号、受影响厂商或型号、利用条件及修复状态等信息，也无法核实该风险的严重程度。建议关注原始报告或后续更新，以获取可验证的技术细节。

rss · InfoQ 中文站 · 9月3日 10:40

**「背景知识」** BMC（基板管理控制器）是服务器主板上内置的专用管理处理器，提供带外管理能力，即使操作系统未运行也可远程监控和控制服务器硬件。安全厂商发布的研究显示，BMC 固件存在多类严重漏洞，例如 Supermicro BMC 中的 CVE-2025-7937 等，攻击者若利用这些漏洞可篡改 BMC 固件，从而在低于操作系统和常规安全软件的层次获得持久控制权；另有报告指出一个存在 22 年之久的 BMC 漏洞可能导致大量数据中心面临入侵风险。本次报道中提到的“数千台服务器面临硬件级入侵风险”，指的正是 BMC 这类管理处理器所存在的安全薄弱点。

**「影响」** 安全厂商 Lava 的扫描显示，超过 24,000 台可互联网访问的服务器管理界面存在 BMC 漏洞，攻击者可在登录前获取认证哈希，且已出现野外利用迹象；受影响范围覆盖现代 Supermicro、HPE 服务器及 GPU 服务商设备，甚至包括仍使用出厂密码的系统，使服务器面临硬件级入侵风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.networkworld.com/article/4063464/new-supermicro-bmc-vulnerabilities-open-servers-to-malicious-attacks-on-firmware.html">New Supermicro BMC vulnerabilities open servers to malicious attacks on firmware | Network World</a></li>
<li><a href="https://www.infoq.com/news/2026/08/bmc-vulnerabilities/">BMC Vulnerabilities Put Thousands of Servers at Risk of Hardware-Level Compromise - InfoQ</a></li>
<li><a href="https://www.securityweek.com/decades-old-bmc-vulnerability-exposes-thousands-of-data-centers-to-attacks/amp/">Decades-Old BMC Vulnerability Exposes Thousands of Data Centers to Attacks - SecurityWeek</a></li>
<li><a href="https://www.infoq.com/news/2026/08/bmc-vulnerabilities/">BMC Vulnerabilities Put Thousands of Servers at Risk of ...</a></li>
<li><a href="https://www.securityweek.com/decades-old-bmc-vulnerability-exposes-thousands-of-data-centers-to-attacks/">Decades-Old BMC Vulnerability Exposes Thousands of Data ...</a></li>
<li><a href="https://lavahq.io/research/bmc-exposure-alert">How We Hacked Thousands of Data Centers in Minutes Using a 20 ...</a></li>

</ul>
</details>

**标签**: `#security`, `#BMC`, `#server hardware`, `#vulnerabilities`, `#infrastructure`

---

<a id="item-tech-news-4"></a>
### [Cursor 推出面向智能体的 GitHub 替代方案 Origin](https://www.infoq.cn/article/labxcNbT15HapoWw69lq?utm_source=rss&amp;utm_medium=article) ⭐️ 7.0/10

Cursor 宣布推出 Origin，定位为面向 AI 智能体的 GitHub 替代方案。该产品尝试将版本控制与协作流程设计为优先服务自主智能体，而不仅是人类开发者，可能推动 AI 辅助软件工程从人工审查协作转向更自动化的代理协作模式。目前官方披露的技术细节有限，具体功能、与既有 Git 工作流的兼容性以及正式上线时间仍需后续说明。此消息由 InfoQ 报道，原作者为 Matt Saunders。

rss · InfoQ 中文站 · 9月3日 09:09

**「背景」** Cursor 是一款基于 VS Code 的 AI 编程编辑器，Origin 是其在 2026 年 6 月 17 日发布的、面向 AI 智能体的 Git 代码托管平台，被定位为 GitHub 的替代方案；它于 2026 年 8 月 17-18 日向付费用户开放测试，内置于 Cursor 编辑器中，支持 GitHub 同步、堆叠式 PR 与智能体协同等能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.explainx.ai/blog/cursor-origin-git-hosting-github-alternative-ai-agents-2026">Cursor Origin: agent-first git hosting and GitHub alternative (2026) | explainx.ai Blog | explainx.ai</a></li>
<li><a href="https://www.infoq.com/news/2026/08/cursor-origin-alternative-github/">Cursor Releases Origin as an Agent-Native Alternative to GitHub - InfoQ</a></li>
<li><a href="https://tbreak.com/cursor-origin-launch/">Cursor Origin: Cursor&#x27;s GitHub Rival for the AI-Agent Era</a></li>

</ul>
</details>

**标签**: `#Cursor`, `#AI agents`, `#developer tools`, `#version control`, `#software engineering`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [谷歌胜诉，免于被强制拆分广告技术业务](https://www.nytimes.com/2026/09/02/technology/google-ad-tech-remedies.html) ⭐️ 8.0/10

谷歌在美国反垄断诉讼中获胜，法院未支持美国司法部寻求的强制出售其广告技术业务的拆分要求。这一结果意味着 Alphabet 可以继续保有这项业务，避免了大规模资产剥离。

hackernews · donohoe · 9月2日 14:46 · [社区讨论](https://news.ycombinator.com/item?id=49537131)

**「背景」** 此前，美国司法部在弗吉尼亚州亚历山德里亚联邦法院起诉谷歌，指控其在开放网络数字广告技术市场非法垄断，并寻求强制谷歌出售其广告技术业务。法院认定谷歌构成垄断，但拒绝了拆分要求，倾向于行为救济，即要求谷歌改变商业行为而非剥离资产。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://easternherald.com/2026/09/02/google-adx-antitrust-ruling-behavioral-remedies/">US Judge Rejects Google Ad Tech Breakup</a></li>
<li><a href="https://dnyuz.com/2026/09/02/google-avoids-breakup-of-ad-tech-business-in-antitrust-ruling/">Google Avoids Breakup of Ad Tech Business in Antitrust Ruling</a></li>

</ul>
</details>

**标签**: `#antitrust`, `#Google`, `#Alphabet`, `#digital advertising`, `#regulation`

---

<a id="item-finance-news-2"></a>
### [数据中心为何成为美国中期选举的政治热点](https://www.economist.com/united-states/2026/09/02/how-data-centres-became-one-of-americas-hottest-political-issues) ⭐️ 7.0/10

据《经济学人》报道，数据中心已成为美国政治议题中的热点，地方反对情绪高涨正在重塑中期选举的选情。报道认为，这一政治反弹可能带来监管与经济层面的后续影响。

rss · The Economist · 9月2日 19:35

**「背景」** 近年人工智能热潮推动大型数据中心在美国各地快速扩张，但这些无窗设施带来的噪音、用电和供水等问题引发当地居民反感。据美国媒体报道，这种反对情绪正成为跨越党派界限的政治议题，并影响 2026 年中期选举选情。

**「影响」** 数据中心已成为 2026 年美国中期选举的新争论点，地方反对情绪可能影响关键选区的选情；例如威斯康星州民调显示，78%的选民认为数据中心的成本超过收益，较去年 10 月的 55%大幅上升，这可能促使两党候选人承诺加强监管，进而给数据中心开发商和投资者带来政策不确定性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://political.org/2026/08/21/rising-data-center-backlash-reshapes-2026-midterm-races-across-the-country/">Rising Data Center Backlash Reshapes 2026 Midterm Races ...</a></li>
<li><a href="https://www.usatoday.com/story/news/politics/elections/2026/08/24/data-centers-trump-midterm-elections/91442283007/">Data center backlash is overtaking 2026 midterm elections</a></li>
<li><a href="https://www.financialexpress.com/world-news/us-news/us-mid-terms-get-an-ai-twist-how-data-centres-power-bills-could-decide-key-races/4328250/?ref=world_hp">US mid - terms get an AI twist: How data centres , power bills could...</a></li>
<li><a href="https://www.jsonline.com/story/news/politics/elections/2026/08/26/7-takeaways-from-the-first-marquette-poll-of-the-midterm-election/91439589007/">7 takeaways from the first Marquette poll of the midterm election</a></li>

</ul>
</details>

**标签**: `#data centers`, `#politics`, `#elections`, `#regulation`, `#infrastructure`

---

<a id="item-finance-news-3"></a>
### [科技助力，厄瓜多尔成为养虾大国](https://www.economist.com/the-americas/2026/09/02/a-prawn-superpower-rises) ⭐️ 7.0/10

《经济学人》报道称，厄瓜多尔养殖户借助技术，使该国成为全球重要的虾类生产国。

rss · The Economist · 9月2日 15:35

**「背景」** 厄瓜多尔是世界主要养虾国之一。其沿海养殖场正普遍采用物联网传感器与自动监测系统等精准水产养殖技术，即用数据精细管理养殖环境，以提高产量并满足可持续要求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.marketsandmarkets.com/Market-Reports/geography/precision-aquaculture-market/ecuador">Ecuador Precision Aquaculture Market Size, Share,Trends ...</a></li>

</ul>
</details>

**标签**: `#Ecuador`, `#aquaculture`, `#technology adoption`, `#shrimp farming`, `#exports`

---

<a id="item-finance-news-4"></a>
### [报道：月之暗面秘密递交港股 IPO 申请，新一轮融资投前估值 500 亿美元](https://x.com/latepostnews/status/2095142540660093315) ⭐️ 7.0/10

据晚点 LatePost 报道，月之暗面（Kimi）已以保密形式向港交所递交 A1 上市文件，启动港股 IPO；公司回应称暂无信息可披露。报道同时称，公司正以 500 亿美元投前估值推进新一轮融资，可能为 IPO 前最后一轮。

telegram · zaihuapd · 9月3日 03:15

**「背景」** 月之暗面是大模型创业公司，旗下产品为 Kimi。报道称，公司保持约三个月迭代一次模型，估值在约半年内从约 43 亿美元升至今年 7 月投后 350 亿美元。

**标签**: `#IPO`, `#Artificial Intelligence`, `#Moonshot AI`, `#Hong Kong`, `#Valuation`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [1967 版蜘蛛侠片头真人化：MiniMax H3 工作流解析](https://www.reddit.com/r/StableDiffusion/comments/1w59dvs/the_1967_spiderman_tv_show_intro_updated_to_live/) ⭐️ 8.0/10

reddit · r/StableDiffusion · /u/seeker\_ktf · 9月2日 12:48

**「背景」** 作者用 MiniMax H3 尝试将 1967 年《蜘蛛侠》动画开场片头重制为真人影像。难点在于原片约 60 秒内含约 31 处场景切换，动画动作和物理也常不合常理，同时还要让人物形象一致、时间点尽可能对上。

**「方案」** 作者的核心做法是不求一次性生成，而是把 60 秒拆成 14 个片段，每个片段最多包含 3 次剪辑。他先将参考视频用 Handbrake 转成 24fps，并以帧为单位记录所有起止点，利用 VHS 加载器逐帧读入；先用 0.2/0.3MP 低分辨率加速度 LoRA 测试节奏，再以 0.9MP、20 次迭代和 dpmpp\_2m 做最终生成。Prompt 方面，他严格按官方指南使用 subject 占位符，不写角色本名，连建筑物等景物也定义为 subject，并尽量描述“想要什么”而非“不要什么”。他还发现，用低分辨率生成的帧截图或此前片段作为参考帧/风格参考，可以给模型有效“推一把”；存在无法逐帧对齐动画剪辑、参考图开头后消失等局限，因此他保留了一些动画式“错误”，并用 Krea2 补充把日景改成夜景等细节。

**「启示」** 作者认为，只要把长视频合理分镜、精确记录时间线并用结构化提示词，AI 视频模型可以把经典动画转成连贯的真人短片；但帧级匹配仍不可靠，最终成果仍需人为剪辑与风格取舍。

**标签**: `#AI video generation`, `#MiniMax H3`, `#ComfyUI`, `#prompt engineering`, `#reference video workflow`

---

## AI 创作者雷达

<a id="item-ai-creator-1"></a>
### [Meta 发布 Muse Spark 1.3，带来 anti-slop 过滤等 UI/SVG 生成改进](https://developer.meta.com/ai/models/muse-spark/) ⭐️ 7.0/10

Meta 推出了模型更新 Muse Spark 1.3，官方博客称这次版本包含 anti-slop 过滤等改进。开发者 Simon Willison 实际用命令行生成了 SVG 示例，成本约为 4.2266 美分、耗时 38 秒，并对比 1.2 后认为 1.3 在自行车车架、翅膀和帽子等细节上更好。整体看，这更像是一次针对低成本 SVG、UI 和代码生成场景的模型更新，而非前沿基础模型的大版本跃迁。

hackernews · bvaldivielso · 9月2日 19:35 · [社区讨论](https://news.ycombinator.com/item?id=49541256)

**「为什么现在」** 在开发者社区已经开始关注 Muse Spark 1.2 的低成本开发用途，并讨论其生成质量是否够用时，1.3 的出现把同一性价比档位上的重点从“便宜”转向“减少机器感”。不过目前能确认的只有发布信息和个别的生成对比体验，尚不能据此判断它会改变编程或 UI 工具链的广泛使用方式。

**「内容角度」** 可做角度：用同一个 SVG 生成提示词对比 Muse Spark 1.2 与 1.3 的实际输出，结合 4.2266 美分和 38 秒的成本数据，观察 anti-slop 过滤是否真的让生成 UI 少一点“机器味”。只呈现已发生的对比结果，不延伸成对开发者工具链或市场格局的结论。

**「社区讨论」** 开发者讨论比较集中在性价比和适用场景：有评论者说 Muse Spark 1.2 在允许 Meta 使用数据进行训练时非常便宜，适合非前沿任务，但也有评论认为它在 C/C++ 内部基准上不如 DeepSeek 的预览版本，显得过拟合。另有评论引用 75.4 分和“当天短暂登顶”等说法来讨论价格竞争，但这些只是个人观点，材料里没有给出可核验的榜单上下文。

**标签**: `#Meta`, `#Muse Spark`, `#AI 编程`, `#UI 生成`, `#模型更新`

---