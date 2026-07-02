---
layout: default
title: "Horizon Summary: 2026-07-02 (ZH)"
date: 2026-07-02
lang: zh
---

> 从 57 条内容中筛选出 10 条重要资讯。

---

1. [ECTC 2026 综述：EMIB-T、HBM4、光子互连与冷却技术](#item-1) ⭐️ 9.0/10
2. [弗吉尼亚州禁止出售地理位置数据](#item-2) ⭐️ 8.0/10
3. [Linux 6.9 漏洞：LUKS 暂停时未清除加密密钥](#item-3) ⭐️ 8.0/10
4. [Podman v6.0.0 发布，网络功能增强](#item-4) ⭐️ 8.0/10
5. [使用 DSPy 优化 Datasette Agent 的 SQL 提示](#item-5) ⭐️ 8.0/10
6. [理解才能参与：与 AI 编码代理协作避免认知债务](#item-6) ⭐️ 8.0/10
7. [Cloudflare 9 月起默认拦截混合用途 AI 爬虫](#item-7) ⭐️ 8.0/10
8. [OpenAI 提议美国政府入股多家 AI 公司](#item-8) ⭐️ 8.0/10
9. [多家公司因 AI 成本飙升限制工具使用](#item-9) ⭐️ 8.0/10
10. [2027 年 PS3 商店关闭引发存档抢救](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [ECTC 2026 综述：EMIB-T、HBM4、光子互连与冷却技术](https://newsletter.semianalysis.com/p/ectc2026) ⭐️ 9.0/10

ECTC 2026 的综述涵盖了英特尔针对 HBM4 的 EMIB-T 先进封装技术、HBM4 集成挑战、微流体冷却以及 Lightmatter 等公司的光子互连技术。 这些技术解决了 AI 和高性能计算中的关键瓶颈，如内存带宽、热管理和互连效率，将塑造芯片设计的未来。 英特尔的 EMIB-T 可扩展到大尺寸且缺陷率更低，而 HBM4 提高了 I/O 密度和供电需求。微流体冷却和光子互连为散热和数据传输提供了新颖的解决方案。

rss · Semianalysis · 7月2日 17:25

**背景**: EMIB（嵌入式多芯片互连桥接）是英特尔用于封装内连接多个芯片的技术。HBM（高带宽内存）垂直堆叠 DRAM 以提供高带宽。光子互连使用光而非电子实现更快、更低功耗的数据传输。先进封装将这些组件集成，以克服传统芯片的性能限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://abit.ee/en/hard/intel-introduces-emib-t-revolutionary-multi-die-packaging-technology-with-hbm4-support">Intel Introduces EMIB - T — Revolutionary Multi-Die Packaging...</a></li>
<li><a href="https://blogs.sw.siemens.com/semiconductor-packaging/2026/04/24/hbm3e-hbm4-ic-design-guide/">HBM3e and HBM4: IC design guide for next-generation high bandwidth memory</a></li>
<li><a href="https://www.sciencedirect.com/topics/engineering/photonic-interconnects">Photonic Interconnects - an overview | ScienceDirect Topics</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#advanced packaging`, `#HBM`, `#photonic interconnects`, `#cooling`

---

<a id="item-2"></a>
## [弗吉尼亚州禁止出售地理位置数据](https://www.hunton.com/privacy-and-cybersecurity-law-blog/virginia-bans-sale-of-geolocation-data) ⭐️ 8.0/10

弗吉尼亚州通过一项新的隐私法，自 2024 年 7 月 1 日起禁止出售地理位置数据。 这项立法为州级隐私保护树立了重要先例，可能促使其他州采取类似措施，让消费者对自己的敏感位置数据拥有更多控制权。 该禁令适用于从弗吉尼亚州境内个人收集的地理位置数据的出售，但对外州公司和在弗吉尼亚数据中心处理的数据存在执行挑战。

hackernews · toomuchtodo · 7月2日 21:03 · [社区讨论](https://news.ycombinator.com/item?id=48767347)

**背景**: 地理位置数据能揭示个人的精确行踪，正越来越多地被应用程序和设备收集。人们对滥用该数据的担忧日益加剧，例如跟踪前往堕胎诊所等敏感地点或保险公司利用该数据，从而推动了监管呼声。在没有全面联邦法律的情况下，弗吉尼亚州的这项法律是美国各州制定隐私保护措施更广泛趋势的一部分。

**社区讨论**: 评论普遍支持该禁令，但强调了执行困难和漏洞，例如外州公司出售在弗吉尼亚收集的数据。具体担忧包括将位置数据用于反堕胎广告（引用了 Politico 的调查）以及车险追踪。讨论还指出该禁令于 2024 年 7 月 1 日生效。

**标签**: `#privacy`, `#geolocation data`, `#legislation`, `#Virginia`, `#data protection`

---

<a id="item-3"></a>
## [Linux 6.9 漏洞：LUKS 暂停时未清除加密密钥](https://mathstodon.xyz/@iblech/116769502749142438) ⭐️ 8.0/10

Linux 内核 6.9 版本中的一个回归导致`cryptsetup luksSuspend`命令不再从内核内存中清除磁盘加密密钥，可能在系统暂停期间暴露密钥。 这一安全回归削弱了针对冷启动攻击的保护，该攻击依赖于在暂停期间从内存中移除加密密钥。它影响了依赖 LUKS 加密和待机（suspend-to-RAM）的用户，特别是在集成了该功能的 Debian 系统上。 该漏洞在 Linux 6.9 中被引入，`luksSuspend`命令通常会在暂停 I/O 前从内核内存中清除加密密钥。社区通过 NixOS 测试发现了该问题，现在这些测试包含了防止再次发生此类问题的测试用例。

hackernews · IngoBlechschmid · 7月2日 15:25 · [社区讨论](https://news.ycombinator.com/item?id=48763035)

**背景**: LUKS（Linux 统一密钥设置）是一种磁盘加密规范。当系统待机（suspend to RAM）时，加密主密钥保留在内核内存中以允许快速恢复。为了缓解冷启动攻击，`cryptsetup luksSuspend`可以在暂停前移除密钥，并在恢复时要求重新输入。这一回归破坏了密钥移除功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/systemd/systemd/issues/17887">Wipe LUKS Disk Encryption Key for Root Disk from RAM during Shutdown to defeat Cold Boot Attacks · Issue #17887 · systemd/systemd</a></li>
<li><a href="https://blog.freesources.org/posts/2020/08/cryptsetup-suspend/">cryptsetup- suspend</a></li>
<li><a href="https://wiki.archlinux.org/title/Power_management/Suspend_and_hibernate">Power management/ Suspend and hibernate - ArchWiki</a></li>

</ul>
</details>

**社区讨论**: 评论指出该漏洞可能只影响 Debian，因为`luksSuspend`并非上游官方支持。有人认为标题有标题党之嫌，但其他人则赞赏 NixOS 测试。一位评论者指出，像这样的安全回归很容易被忽略，因为一切看起来仍然正常工作。

**标签**: `#Linux`, `#security`, `#encryption`, `#kernel`, `#LUKS`

---

<a id="item-4"></a>
## [Podman v6.0.0 发布，网络功能增强](https://blog.podman.io/2026/07/introducing-podman-v6-0-0/) ⭐️ 8.0/10

Podman v6.0.0 已发布，带来了显著的网络改进，进一步巩固了其作为 Docker 替代品的地位。此次更新包括增强的网络栈性能，并继续支持无根容器和 Quadlet。 此次发布凸显了 Podman 作为安全、无守护进程容器引擎的日益成熟和被采用。在 Hacker News 上的高社区参与度表明，人们越来越信任 Podman 用于生产工作负载。 Podman v6.0.0 引入了新的网络功能，提高了性能和易用性，同时保持与 Docker CLI 和 docker-compose 的兼容性。但一些用户报告存在细微的不兼容性，可能在复杂设置中引发问题。

hackernews · soheilpro · 7月2日 14:23 · [社区讨论](https://news.ycombinator.com/item?id=48762098)

**背景**: Podman 是由 Red Hat 开发的开源、符合 OCI 标准的容器引擎。与 Docker 不同，它是无守护进程的，并默认支持无根容器，增强了安全性。它与 systemd 集成良好，在许多场景下可作为 Docker 的即插即用替代品。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Podman">Podman - Wikipedia</a></li>
<li><a href="https://podman.io/">Podman</a></li>
<li><a href="https://www.redhat.com/en/topics/containers/what-is-podman">What is Podman?</a></li>

</ul>
</details>

**社区讨论**: 社区情绪总体积极，用户称赞 Podman 的迁移简便性和性能。一些用户对细微的 Docker 不兼容性表示沮丧，而另一些用户则强调无根操作和 systemd 集成的优势。

**标签**: `#Podman`, `#containerization`, `#Docker alternative`, `#open source`, `#release`

---

<a id="item-5"></a>
## [使用 DSPy 优化 Datasette Agent 的 SQL 提示](https://simonwillison.net/2026/Jul/2/dspy-datasette-agent-prompts/#atom-everything) ⭐️ 8.0/10

Simon Willison 使用 DSPy 框架自动评估并改进了 Datasette Agent 的 SQL 查询生成功能的系统提示，识别并修复了因模式信息不完整导致的列名猜测等问题。 这展示了一种实用的自动化提示工程方法，能够提高生成 SQL 的 AI 代理的可靠性和准确性。它表明像 DSPy 这样的框架可以系统地改进代理行为，而无需手动反复试验。 该实验使用了 Claude Code（Fable 5 模型）来搭建评估管道，并测试了 GPT-4.1 mini 和 nano 模型。一个重要发现是，原始提示中关于避免不必要的模式查找的建议导致代理猜测列名，从而引发错误。

rss · Simon Willison · 7月2日 18:25

**背景**: DSPy 是一个 Python 框架，它通过算法优化语言模型的提示和权重，将提示工程视为编程任务。Datasette Agent 是 Datasette 的一个开源 AI 助手插件，允许用户使用自然语言查询 SQLite 数据库。Claude Code 是 Anthropic 开发的 AI 编码代理，能够读取代码库、编辑文件并运行命令。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/stanfordnlp/dspy">GitHub - stanfordnlp/dspy: DSPy: The framework for programming—not prompting—language models</a></li>
<li><a href="https://datasette.io/blog/2026/datasette-agent/">Datasette Agent, an extensible AI assistant for Datasette - Datasette Blog</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>

</ul>
</details>

**标签**: `#DSPy`, `#prompt engineering`, `#AI agents`, `#SQL generation`, `#Datasette`

---

<a id="item-6"></a>
## [理解才能参与：与 AI 编码代理协作避免认知债务](https://simonwillison.net/2026/Jul/2/understand-to-participate/#atom-everything) ⭐️ 8.0/10

Geoffrey Litt 在 AIE 2026 的演讲中提出了“理解才能参与”的框架，强调开发者必须深入理解 AI 代理生成的代码，才能保持主动参与并避免认知债务。 这一概念帮助开发者在利用 AI 编码代理时保持代码质量和准确的思维模型，防止认知债务的积累，从而避免阻碍项目的长期健康发展。 该演讲是 AIE 2026 的一部分，大会有超过 300 场录播；Geoffrey 还在 Twitter 上发布了演讲摘要，完整视频将在随后三周内于 YouTube 上逐步发布。

rss · Simon Willison · 7月2日 17:07

**背景**: 认知债务是一个新兴术语，描述软件团队中共享理解的侵蚀，尤其是当 AI 代理生成开发者未能完全理解的代码时。与技术债务关注代码质量不同，认知债务影响开发者推理和安全修改系统的能力，导致不确定性增加和进展放缓。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://margaretstorey.com/blog/2026/02/09/cognitive-debt/">How Generative and Agentic AI Shift Concern from Technical Debt to Cognitive Debt</a></li>
<li><a href="https://getdx.com/blog/cognitive-debt-the-hidden-risk-in-ai-driven-software-development/">Cognitive debt: The hidden risk in AI-driven software development</a></li>
<li><a href="https://www.faros.ai/blog/best-ai-coding-agents-2026">Best AI Coding Agents for 2026: Real-World Developer Reviews</a></li>

</ul>
</details>

**标签**: `#AI-assisted coding`, `#cognitive debt`, `#collaboration`, `#software engineering`, `#developer tools`

---

<a id="item-7"></a>
## [Cloudflare 9 月起默认拦截混合用途 AI 爬虫](https://techcrunch.com/2026/07/01/cloudflares-new-policy-pushes-ai-companies-to-pay-for-publishers-content/) ⭐️ 8.0/10

Cloudflare 宣布自 9 月 15 日起，默认阻止那些同时用于搜索索引和 AI 训练的“混合用途”爬虫抓取带广告的页面，并特别点名谷歌利用搜索收录和 AI 训练之间的漏洞。 这一政策变化可能迫使 AI 公司为使用发布者内容付费，重塑网络爬取和 AI 训练的经济模式，突显了内容创作者与 AI 公司之间关于数据使用权的紧张关系。 新规则适用于同时服务搜索索引和 AI 训练的爬虫，例如谷歌爬虫既用于搜索收录又用于 AI 模型训练。此举正值行业就 AI 系统使用内容的公平补偿问题展开广泛讨论之际。

telegram · zaihuapd · 7月2日 05:37

**背景**: 网络爬虫是自动扫描网站的程序，用于为搜索引擎建立索引或收集数据进行 AI 训练。搜索爬虫通常受到欢迎，因为它们能提高网站可见性，而 AI 训练爬虫则常被屏蔽，因为它们未经补偿就提取内容。混合用途爬虫模糊了这一界限，使网站难以区分允许的索引和不允许的 AI 训练。Cloudflare 的新政策试图通过在带广告的页面上默认阻止此类爬虫来解决这一问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.zhihu.com/question/24098641">通俗的讲，网络爬虫到底是什么？</a></li>
<li><a href="https://www.clickfrom.ai/zh/blog/inside-the-ai-mind-how-chatgpt-and-ai-crawlers-see-your-website">进入 AI 的思维：ChatGPT和 AI 爬 虫 如何看待你的网站 — ClickFrom. AI</a></li>

</ul>
</details>

**社区讨论**: TechCrunch 文章下的评论总结道：许多网站屏蔽了 AI 爬虫但没有屏蔽谷歌搜索爬虫，谷歌利用了这个漏洞训练其 AI。这种观点反映了对 AI 公司数据实践的普遍不满。

**标签**: `#Cloudflare`, `#AI crawlers`, `#Google`, `#web scraping`, `#AI training`

---

<a id="item-8"></a>
## [OpenAI 提议美国政府入股多家 AI 公司](https://www.bloomberg.com/news/articles/2026-07-02/openai-proposes-giving-the-us-government-a-5-stake-ft-says) ⭐️ 8.0/10

据《金融时报》报道，OpenAI 提议美国政府持有该公司 5%的股份，并可能扩展到 Google、Meta 和 Anthropic 等主要 AI 公司。该提议旨在应对政治反弹，并让公众从 AI 的经济收益中获益。 这一提议可能通过建立 AI 技术收益的公共分享机制，重塑 AI 治理格局，并为政府参与科技行业开创先例。若被采纳，政府将持有主要 AI 公司的财务股份，并可能获得一定影响力，引发关于控制权和利益冲突的讨论。 该股份将由一个政府载体持有，按 OpenAI 当前估值，5%的股份价值约 426 亿美元。被提及的其他公司是否同意该提议尚不明确，该计划可能面临重大的监管和反垄断审查。

telegram · zaihuapd · 7月2日 06:02

**背景**: 该提议是在 AI 公司面临日益增长的政治压力背景下提出的，这些压力涉及就业替代、安全以及财富集中等问题。OpenAI 最近转型为公益公司（PBC），在法律上要求其在追求利润的同时考虑公共利益。其他立法者，如参议员伯尼·桑德斯，提出了更广泛的 AI 公共所有权模式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/07/02/openai-proposes-us-government-own-5percent-stake-to-address-political-blowback.html">OpenAI proposes U.S. government own 5% stake to address ...</a></li>
<li><a href="https://www.forbes.com/sites/siladityaray/2026/07/02/openai-reportedly-pitches-granting-us-government-5-stake/">OpenAI Reportedly Pitches Granting U.S. Government 5% Stake</a></li>
<li><a href="https://apnews.com/article/bernie-sanders-ai-public-ownership-57b9f20d96490083e2749adba0f13977">Bernie Sanders unveils plan for public ownership of AI ...</a></li>

</ul>
</details>

**标签**: `#政策影响`, `#AI治理`, `#大型科技公司`, `#政府持股`

---

<a id="item-9"></a>
## [多家公司因 AI 成本飙升限制工具使用](https://www.404media.co/companies-are-throttling-employees-ai-use-because-its-too-expensive/) ⭐️ 8.0/10

花旗银行于 2026 年 6 月 24 日禁用 GPT-5.5 和 Claude Opus 4.6/4.7，认为这些模型消耗的 AI 积分过高。Atlassian 的 AI 月支出从 2025 年 8 月的 500 万美元飙升至 2026 年 5 月的 1500 万美元，因此终止了无限使用并推出成本追踪面板。Adobe 也终止了其无限使用 Claude 的合同。 这一趋势表明，在按用量计费模式下，企业 AI 应用面临严重的成本可持续性问题。这可能会减缓 AI 整合速度，并促使各行业重新考虑定价模式或内部使用政策。 404 Media 获取的内部数据显示，GPT-5.5 和 Claude Opus 4.6 等高级模型消耗 AI 积分的速度远快于普通模型。Atlassian 的成本追踪面板显示，20%的员工过度使用 AI，导致支出激增。

telegram · zaihuapd · 7月2日 13:59

**背景**: GPT-5.5 由 OpenAI 于 2026 年 4 月 23 日发布，是其最强模型，但 token 定价更高——超过 272K 输入 token 的提示词按输入价格的两倍计费。Claude Opus 4.6 由 Anthropic 于 2026 年 2 月 5 日发布，同样昂贵。许多企业现在使用 AI 积分或 token 计费，每次交互根据模型和 token 数量消耗积分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.5">GPT-5.5 - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Opus_4.6">Claude Opus 4.6</a></li>

</ul>
</details>

**标签**: `#AI`, `#cost management`, `#enterprise`, `#OpenAI`, `#Claude`

---

<a id="item-10"></a>
## [2027 年 PS3 商店关闭引发存档抢救](http://no-intro.org/) ⭐️ 8.0/10

索尼宣布将于 2027 年 7 月永久关闭 PS3 和 PS Vita 的 PlayStation 商店，数字档案管理员与 RPCS3 模拟器团队正紧急备份游戏数据，以防止纯数字版游戏永久丢失。 此次关闭威胁到数百款纯数字版 PS3 和 PS Vita 游戏的保存，凸显了数字游戏所有权的脆弱性以及社区主导的保存工作的必要性。 RPCS3 推荐使用 no-intro.org 数据库，该数据库记录加密哈希值、文件大小等元数据，以协调备份工作并追踪哪些游戏已得到保存。

telegram · zaihuapd · 7月2日 15:04

**背景**: PlayStation 3 和 PS Vita 商店是购买和下载游戏的数字平台。商店关闭后，用户将无法再购买或重新下载数字内容。RPCS3 是一个开源的 PS3 模拟器，可在 PC 上运行 PS3 游戏；no-intro.org 是一个由社区驱动的游戏存档数据库。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rpcs3.net/">RPCS3</a></li>
<li><a href="https://no-intro.org/">No - Intro . org</a></li>
<li><a href="https://www.tomshardware.com/video-games/playstation/digital-archivists-rush-to-save-ps3-game-data-before-sony-shuts-down-the-store-forever-in-2027-rpcs3-emulator-urges-users-to-preserve-all-content">Digital archivists rush to save PS3 game data before... | Tom's Hardware</a></li>

</ul>
</details>

**标签**: `#digital preservation`, `#PlayStation`, `#game emulation`, `#digital rights`

---