---
layout: default
title: "Horizon Summary: 2026-07-05 (ZH)"
date: 2026-07-05
lang: zh
---

> 从 42 条内容中筛选出 6 条重要资讯。

---

1. [数字游戏购买应保障完整所有权](#item-1) ⭐️ 8.0/10
2. [Claude Fable AI 协助发布 sqlite-utils 4.0rc2](#item-2) ⭐️ 8.0/10
3. [能力门：基于内部置信度调控工具使用](#item-3) ⭐️ 8.0/10
4. [F-Droid 称 Google ADV 为预装在 40 亿设备上的恶意软件](#item-4) ⭐️ 8.0/10
5. [卫报揭露 OpenAI 从未实地考察星际之门英国关键选址](#item-5) ⭐️ 8.0/10
6. [SpaceX 向投资者展示原型手机](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [数字游戏购买应保障完整所有权](https://popcar.bearblog.dev/its-about-ownership/) ⭐️ 8.0/10

一篇文章主张数字游戏购买应赋予完整所有权，包括可转让性和离线访问权，批评当前将购买视为可撤销许可的授权模式。 这场辩论影响消费者权益和数字游戏库的长期可用性，推动监管变革，可能重塑游戏行业和软件许可实践。 文章认为，即使像 Steam 这样 DRM 限制较少的平台也未提供真正所有权，并批评行业向订阅模式转变进一步削弱消费者权益。

hackernews · popcar2 · 7月5日 14:56 · [社区讨论](https://news.ycombinator.com/item?id=48794750)

**背景**: 数字游戏通常根据最终用户许可协议（EULA）获得许可而非购买，该协议限制复制、转售和离线使用。数字版权管理（DRM）强制执行这些限制。消费者权益倡导者主张数字购买应赋予与实物商品类似的所有权，包括转售或出借游戏的能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Digital_rights_management">Digital rights management - Wikipedia</a></li>
<li><a href="https://www.digitaltrends.com/gaming/what-is-drm-in-video-games/">What is DRM in video games and how does it work? - Digital Trends</a></li>
<li><a href="https://en.wikipedia.org/wiki/End-user_license_agreement">End - user license agreement - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍支持有监管的所有权，有人指出像《魔兽世界》这样的订阅模式已影响行业。其他人分享了失去已购买游戏访问权限的个人经历，还有人提到使用破解作为应对 DRM 限制的变通方法。

**标签**: `#digital ownership`, `#gaming`, `#consumer rights`, `#regulation`, `#licensing`

---

<a id="item-2"></a>
## [Claude Fable AI 协助发布 sqlite-utils 4.0rc2](https://simonwillison.net/2026/Jul/5/sqlite-utils-fable/#atom-everything) ⭐️ 8.0/10

Simon Willison 发布了 sqlite-utils 4.0rc2，该候选版本主要由 Claude Fable AI 生成，此前 AI 在 rc1 版本中发现了多个严重错误，包括 delete_where() 中的数据丢失错误。 这展示了 AI 在软件维护和发布管理中的实用且经济高效的应用，表明 AI 可以在稳定版本发布前发现重大错误并提高代码质量。 AI 审查了 4.0rc1 并发现了 5 个发布阻塞问题，其中包括一个导致数据丢失的事务错误。通过 37 次提示和 34 次提交，AI 在 30 个文件中生成了 +1,321 行代码更改，总成本约为 149.25 美元。

rss · Simon Willison · 7月5日 01:00

**背景**: sqlite-utils 是一个用于操作 SQLite 数据库的 Python 库和 CLI 工具，在 sqlite3 包之上提供更高级的操作。Claude Fable 是 Anthropic 开发的先进 AI 模型，以其编码能力著称。Simon Willison 是 sqlite-utils 和 Datasette 的创建者。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sqlite-utils.datasette.io/">sqlite-utils</a></li>
<li><a href="https://github.com/simonw/sqlite-utils">GitHub - simonw/sqlite-utils: Python CLI utility and library for manipulating SQLite databases · GitHub</a></li>
<li><a href="https://simonwillison.net/2026/Jun/21/sqlite-utils-40rc1/">sqlite-utils 4.0rc1 adds migrations and nested transactions</a></li>

</ul>
</details>

**标签**: `#sqlite-utils`, `#AI-assisted development`, `#software release`, `#open source`, `#Claude`

---

<a id="item-3"></a>
## [能力门：基于内部置信度调控工具使用](https://www.reddit.com/r/MachineLearning/comments/1unw5un/competence_gate_gating_tooluse_on_a_small_models/) ⭐️ 8.0/10

发布了一个基于 Qwen3.5-4B 的 10MB LoRA 适配器，它根据内部激活置信度而非口头表达的置信度来调控工具使用，改进了错误检测并减少了私人数据泄露。该适配器针对每个查询决定是直接回答、搜索网络还是从本地文档检索。 小型语言模型通常过度自信，无法准确口头表达其不确定性；该方法利用内部信号调控工具使用，使小模型更加可靠。通过减少幻觉和意外数据泄露，它可能有助于在隐私敏感或高风险应用中实现更安全的部署。 该门控在捕捉自身错误方面实现了 0.46 的 d′提升（95%置信区间[0.01, 0.89]），并且被门控标记而基础模型未标记的案例中，87%确实是错误答案。一个双信号版本将发送到公共搜索的私人问题比例从 22%降至 10%（降低 0.12，95%置信区间[0.02, 0.22]）。

reddit · r/MachineLearning · /u/Synthium- · 7月5日 07:49

**背景**: LoRA（低秩适应）是一种参数高效的微调方法，它冻结预训练权重并注入可训练矩阵，从而实现轻量级适配。d′（d-prime）是衡量信号检测敏感度的指标，考虑了反应偏向。GGUF 是一种二进制文件格式，针对模型的快速加载和推理进行了优化，常用于 llama.cpp 和 Ollama。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.geeksforgeeks.org/deep-learning/low-rank-adaptation-lora/">Low Rank Adaptation (LoRA) - GeeksforGeeks</a></li>
<li><a href="https://dictionary.apa.org/d-prime">d prime - APA Dictionary of Psychology</a></li>
<li><a href="https://en.wikipedia.org/wiki/GGUF">GGUF - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI/ML`, `#language models`, `#tool use`, `#model confidence`, `#open source`

---

<a id="item-4"></a>
## [F-Droid 称 Google ADV 为预装在 40 亿设备上的恶意软件](https://f-droid.org/2026/07/01/adv-malware.html) ⭐️ 8.0/10

F-Droid（一个自由开源的安卓应用商店）宣布 Google 的 Android Developer Verifier (ADV) 为恶意软件，该程序将阻止未经 Google 批准的应用程序，并计划于 2026 年 9 月 30 日在巴西、印尼、新加坡和泰国首批激活，2027 年起全球推广。 这一声明突显了对安卓开放性和用户选择的潜在威胁，ADV 可能允许 Google 屏蔽 F-Droid 等替代应用商店，限制软件自由。这将影响数十亿依赖侧载的用户和应用开发者。 F-Droid 称 ADV 作为系统服务在 Android 8 及以上设备上以 root 权限运行，无法移除，并预装在约 40 亿台设备上。Google 据称在服务条款中刻意不定义'恶意软件'，从而可任意将广告拦截器等不喜欢的软件归类为恶意软件。

telegram · zaihuapd · 7月5日 00:41

**背景**: Android Developer Verifier (ADV) 是 Google 通过 Play Protect 引入的系统进程，旨在验证开发者身份并保护用户免受恶意软件侵害。F-Droid 是一个自由开源安卓应用仓库，常被用作 Google Play Store 的替代。争议源于 ADV 能够阻止未经 Google 批准的应用程序，批评者认为这削弱了用户控制和软件自由。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://f-droid.org/2026/07/01/adv-malware.html">What We Talk About When We Talk About Malware | F-Droid - Free and Open Source Android App Repository</a></li>
<li><a href="https://techplanet.today/post/android-developer-verification-googles-controversial-security-initiative-and-its-impact-on-app-ecosystem-freedom">Android Developer Verification: Google's Controversial Security Initiative and Its Impact on App Ecosystem Freedom | TechPlanet</a></li>
<li><a href="https://en.wikipedia.org/wiki/F-Droid">F-Droid</a></li>

</ul>
</details>

**标签**: `#Android`, `#F-Droid`, `#Google`, `#malware`, `#privacy`

---

<a id="item-5"></a>
## [卫报揭露 OpenAI 从未实地考察星际之门英国关键选址](https://www.theguardian.com/technology/2026/jul/04/openai-apparent-failure-visit-key-site-questions-stargate-uk-project) ⭐️ 8.0/10

《卫报》报道称，OpenAI 从未实地造访其星际之门英国项目位于北泰恩赛德的核心选址，当地官员也从未与 OpenAI 或合作方 Nscale 会面，这使得 300 亿美元的投资承诺被质疑为公关噱头。 这项调查削弱了对 OpenAI 重大基础设施承诺的信任，并对政府与技术公司在人工智能发展方面合作的真伪提出质疑，可能影响未来的投资和政策决策。 星际之门英国项目于去年特朗普访英期间作为英美 AI 合作旗舰工程高调宣布，但于 2026 年 4 月以监管和能源成本过高为由暂停；当地官员表示该项目'极不可能'落地。

telegram · zaihuapd · 7月5日 05:09

**背景**: 星际之门英国项目由 OpenAI 于 2025 年 9 月宣布，旨在英国建设使用本地计算能力的 AI 基础设施。这代表了大型 AI 公司承诺大规模数据中心投资的广泛趋势。《卫报》的调查显示，尽管有高调宣布，OpenAI 并未对所提议选址进行基本尽职调查，该项目似乎被用于政治目的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/introducing-stargate-uk/">Introducing Stargate UK - OpenAI</a></li>
<li><a href="https://datacentremagazine.com/news/stargate-uk-why-is-openai-halting-ai-data-centre-project">Stargate UK: Why is OpenAI Halting its AI Data Centre Deal?</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#Stargate`, `#UK`, `#AI infrastructure`, `#controversy`

---

<a id="item-6"></a>
## [SpaceX 向投资者展示原型手机](https://www.wsj.com/tech/spacexs-telecom-dreams-d461e568) ⭐️ 8.0/10

据《华尔街日报》报道，SpaceX 已经开发了一款比 iPhone 更薄、运行自有操作系统的原型智能手机。该设备旨在利用 Starlink 卫星提供移动通信服务。 SpaceX 进军手机制造可能通过将卫星连接直接集成到消费设备中，颠覆移动行业。此举挑战传统电信运营商，并可能加速基于卫星的移动服务的普及。 据悉，原型机比当前 iPhone 更薄，并运行定制操作系统。SpaceX 总裁 Gwynne Shotwell 还讨论了建设移动服务地面网络以及与蜂窝运营商合作的事宜，尽管 Elon Musk 此前否认了制造手机的计划。

telegram · zaihuapd · 7月5日 14:10

**背景**: SpaceX 运营 Starlink 卫星互联网星座，并一直在发射可直接连接标准智能手机的“手机直连”（DTC）卫星。DTC 卫星使用激光星间链路连接到宽带星座，并采用先进调制解调器作为太空中的基站，支持短信、彩信，并最终支持语音和视频。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.txrjy.com/thread-1331558-1-1.html">星链（Starlink）手机直连卫星互联网计划详细介绍及未来展望 - 5G终端 - 通信人家园 - Powered by C114</a></li>
<li><a href="https://www.sohu.com/a/787591589_466840">Starlink手机直连卫星即将突破百颗，通过LISL技术链接宽带星座实现数据回传_SpaceX_商业_网络</a></li>
<li><a href="https://news.mydrivers.com/1/1133/1133547.htm">传 SpaceX 原 型 机 比iPhone还薄！马斯克再辟谣造 手 机 ：完全失实 | 快科技</a></li>

</ul>
</details>

**标签**: `#SpaceX`, `#Starlink`, `#手机`, `#卫星通信`, `#移动通信`

---