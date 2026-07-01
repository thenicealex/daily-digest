---
layout: default
title: "Horizon Summary: 2026-07-01 (ZH)"
date: 2026-07-01
lang: zh
---

> 从 62 条内容中筛选出 16 条重要资讯。

---

1. [首个从头合成的细胞实现生长与分裂](#item-1) ⭐️ 9.0/10
2. [Box3D：Erin Catto 发布的开源 3D 物理引擎](#item-2) ⭐️ 9.0/10
3. [Cloudflare 推出基于 HTTP 402 和稳定币的变现网关](#item-3) ⭐️ 9.0/10
4. [arXiv 将于 2026 年 7 月成为独立非营利组织](#item-4) ⭐️ 9.0/10
5. [FFmpeg 9.1 原生 AAC 编码器达到专有编码器质量](#item-5) ⭐️ 8.0/10
6. [索尼将于 2028 年 1 月停止生产实体游戏光盘](#item-6) ⭐️ 8.0/10
7. [内燃机互动深度解析](#item-7) ⭐️ 8.0/10
8. [Anthropic 的 Fable 5 引发安全和信任争议](#item-8) ⭐️ 8.0/10
9. [美国解除对 Anthropic 的 Claude Fable 5 和 Mythos 5 的出口管制](#item-9) ⭐️ 8.0/10
10. [MOTHRAG：无图多跳 RAG 性能超越基于图的系统](#item-10) ⭐️ 8.0/10
11. [Sentinel Gateway：系统级提示注入防御](#item-11) ⭐️ 8.0/10
12. [Claude Code 2.1.91 被指秘密遥测代理与时区信息](#item-12) ⭐️ 8.0/10
13. [英伟达将 DeepSeek V4 推理成本降至五分之一](#item-13) ⭐️ 8.0/10
14. [Visa、Mastercard 等 140 多家企业联合发起 Open Standard 稳定币网络](#item-14) ⭐️ 8.0/10
15. [ChatGPT 每周用户翻倍至 2 亿](#item-15) ⭐️ 8.0/10
16. [国巨 7 月 1 日起电容涨价五成](#item-16) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [首个从头合成的细胞实现生长与分裂](https://www.quantamagazine.org/for-the-first-time-a-cell-built-from-scratch-grows-and-divides-20260701/) ⭐️ 9.0/10

明尼苏达大学凯特·阿达马拉领导的研究团队创造了 SpudCell——一种完全由无生命化学物质构建的合成细胞，它能够生长、复制基因组并分裂，标志着首次实现完全合成细胞的自主生长与分裂。 这一突破克服了合成生物学中的重大障碍，证明缺乏细胞骨架的细胞仍然能够分裂，为设计最小生命形式和理解生命基本原理开辟了新可能。它还可能带来生物技术应用，如可编程药物递送或生物传感。 SpudCell 放弃了细胞骨架，转而依靠基于膜的分裂机制。该工作最初被《细胞》期刊拒绝，一名审稿人认为 SpudCells 不是真正的生物学。超过 190 页的手稿在发布到 bioRxiv 之前，已在禁运条件下与记者分享。

hackernews · defrost · 7月1日 14:20 · [社区讨论](https://news.ycombinator.com/item?id=48747304)

**背景**: 合成生物学旨在从头构建人工细胞，以更好地理解生命的基本组成部分。此前研究已在合成细胞中实现了喂食和 DNA 复制，但细胞分裂——通常涉及细胞骨架重组的复杂过程——仍是一个挑战。SpudCell 的设计完全绕过了细胞骨架，利用脂质膜的化学融合与分裂来进行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.science.org/content/article/lab-created-spudcell-marks-major-step-toward-building-life-scratch">Lab-created ‘SpudCell’ marks ‘stunning’ step toward building life from scratch | Science | AAAS</a></li>
<li><a href="https://www.nytimes.com/2026/07/01/science/spud-cell-what-to-know.html">SpudCell: Scientists Made a Cell With Most of the Hallmarks of Life. Here’s What to Know. - The New York Times</a></li>

</ul>
</details>

**社区讨论**: Hacker News 讨论区的评论褒贬不一。一些用户称赞这一成就是重大进展，而另一些则持怀疑态度，指出论文被《细胞》期刊拒绝以及手稿在同行评审前以禁运形式分发等争议。有用户指出，实际科学成果令人印象深刻，但宣传策略招致了批评。

**标签**: `#synthetic biology`, `#cell division`, `#biotechnology`, `#research`, `#breakthrough`

---

<a id="item-2"></a>
## [Box3D：Erin Catto 发布的开源 3D 物理引擎](https://box2d.org/posts/2026/06/announcing-box3d/) ⭐️ 9.0/10

Erin Catto 宣布发布 Box3D，这是一款新的开源 3D 物理引擎，基于其广泛使用的 Box2D 库的成功经验。 鉴于 Box2D 的遗产和社区的 enthusiasm，Box3D 可能成为独立游戏开发、强化学习环境和模拟的基础工具。 公告未明确是否支持确定性仿真（这是网络应用关注的话题），但预计引擎将根据社区反馈逐步发展。

hackernews · makepanic · 7月1日 12:12 · [社区讨论](https://news.ycombinator.com/item?id=48745445)

**背景**: Box2D 是由 Erin Catto 创建的自由开源 2D 刚体物理引擎，用于《愤怒的小鸟》等游戏以及 Gymnasium 等机器学习框架中的强化学习基准测试。Box3D 将类似的刚体动力学和碰撞检测原理扩展到三维空间，旨在为开发者提供快速准确的物理模拟。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Box2D">Box2D</a></li>
<li><a href="https://box2d.org/">Box2D</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了兴奋之情，回忆了 Box2D 对独立游戏和强化学习的影响。一些人提出了关于多玩家确定性仿真的问题，而机器学习研究人员则强调了 Box2D 在标准 RL 基准测试中的作用。

**标签**: `#physics engine`, `#open source`, `#game development`, `#simulation`, `#machine learning`

---

<a id="item-3"></a>
## [Cloudflare 推出基于 HTTP 402 和稳定币的变现网关](https://blog.cloudflare.com/monetization-gateway/) ⭐️ 9.0/10

Cloudflare 宣布推出一个变现网关，允许网站运营者通过 HTTP 402 状态码和 USDC 等稳定币，对 Cloudflare 网络后的任意资源进行收费。 这一功能实现了网页内容和 API 的无缝微交易，通过将加密货币支付直接集成到 HTTP 协议中，可能改变互联网的经济模式。 该网关实现了 x402 开放标准，重新启用了长期未使用的 HTTP 402“需要付款”状态码。Cloudflare 负责处理支付流程，运营者可以为每次请求设定价格，无需自行管理支付基础设施。

hackernews · soheilpro · 7月1日 13:59 · [社区讨论](https://news.ycombinator.com/item?id=48746914)

**背景**: HTTP 402 在最初的 HTTP 规范中已定义，但由于缺乏标准支付协议从未被广泛采用。x402 标准通过指定使用加密货币或法币的轻量级支付流程重新激活了它。Cloudflare 的网关基于该标准，为任何资源的变现提供了一站式解决方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/X402">X402</a></li>
<li><a href="https://www.x402.org/">x402 - Payment Required | Internet-Native Payments Standard</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Status/402">402 Payment Required - HTTP | MDN</a></li>

</ul>
</details>

**社区讨论**: 评论者对代理驱动的微交易潜力感到兴奋，但也提出了重大担忧：法律和监管障碍（发票、增值税、合规性）、区分机器人与人类的挑战，以及与新兴的网页机器人认证标准可能存在的冲突。

**标签**: `#monetization`, `#microtransactions`, `#cloudflare`, `#web payments`, `#api`

---

<a id="item-4"></a>
## [arXiv 将于 2026 年 7 月成为独立非营利组织](https://www.reddit.com/r/MachineLearning/comments/1ukjtlm/on_july_1_2026_arxiv_will_spin_out_from_cornell/) ⭐️ 9.0/10

arXiv 宣布将于 2026 年 7 月 1 日从康奈尔大学剥离，成为独立的非营利组织，并获得西蒙斯基金会和施密特科学基金会的主要资助。 这一结构变化确保了 arXiv 的长期可持续性和独立性，对于依赖其进行开放获取预印本分发的全球研究社区至关重要。 剥离包括网站重新设计（'抛弃红色'）和新的治理结构，而康奈尔大学将继续提供过渡期支持。

reddit · r/MachineLearning · /u/Nunki08 · 7月1日 12:07

**背景**: arXiv 是一个免费的预印本存储库，成立于 1991 年，自 2001 年起由康奈尔大学托管。它已成为物理学、数学、计算机科学及相关领域学术交流的基石，拥有超过两百万篇预印本。

**标签**: `#arXiv`, `#open access`, `#scholarly publishing`, `#research infrastructure`

---

<a id="item-5"></a>
## [FFmpeg 9.1 原生 AAC 编码器达到专有编码器质量](https://hydrogenaudio.org/index.php/topic,129691.0.html) ⭐️ 8.0/10

此次更新使 FFmpeg 成为无需依赖外部库即可进行 AAC 编码的一体化解决方案，惠及开源社区和需要高质量音频编码的用户。 该编码器针对 48 kHz 音频进行了优化，但支持其他采样率，质量可能较低；它避免了 AAC 解码器中与立体声感知噪声替换（PNS）相关的已知错误。

hackernews · ledoge · 7月1日 14:10 · [社区讨论](https://news.ycombinator.com/item?id=48747116)

**背景**: AAC（高级音频编码）是一种广泛使用的有损音频压缩标准。由 Rostislav Pehlivanov 和 Claudio Freire 开发的 FFmpeg 原生 AAC 编码器已成熟，可与 Apple 的 Core Audio 和 Fraunhofer FDK 等编码器竞争，为高质量编码提供了免费替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Advanced_Audio_Coding">Advanced Audio Coding - Wikipedia</a></li>
<li><a href="https://ffmpeg.org/ffmpeg-codecs.html">FFmpeg Codecs Documentation</a></li>
<li><a href="https://ffmpeg.org/index.html#aac_encoder_stable">FFmpeg</a></li>

</ul>
</details>

**社区讨论**: 社区评论指出，Opus 即使在 64 kbps 下也比所有 AAC 编码器表现更好，并提到编码器的主观调音基于开发者的耳朵。一些用户对修复恼人的啁啾伪影和采用 48 kHz 作为标准表示欣慰。

**标签**: `#FFmpeg`, `#AAC`, `#audio encoding`, `#open source`, `#codec`

---

<a id="item-6"></a>
## [索尼将于 2028 年 1 月停止生产实体游戏光盘](https://blog.playstation.com/2026/07/01/physical-disc-production-ending-in-january-2028-for-new-games-releasing-on-playstation-consoles/) ⭐️ 8.0/10

索尼宣布，PlayStation 实体游戏光盘的生产将于 2028 年 1 月停止，此后新游戏将仅通过数字下载形式在主机上提供。 这标志着游戏行业向完全数字化分发的重要转变，引发了关于游戏所有权、保存以及实体媒体未来的担忧。 该截止日期仅适用于新游戏发行；现有实体光盘仍可继续使用，某些特别版可能仍包含不含光盘的实体物品。索尼的决定紧随微软和任天堂近年来的类似举措。

hackernews · Tiberium · 7月1日 12:13 · [社区讨论](https://news.ycombinator.com/item?id=48745456)

**背景**: 实体游戏光盘数十年来一直是主机游戏的核心，允许玩家购买、出售和分享游戏。随着更快的互联网和更大存储的出现，数字化进程加速，但许多玩家仍看重所有权和转售潜力。游戏保护主义者担心，纯数字化的未来将导致服务器关闭后游戏丢失。

**社区讨论**: 社区评论普遍批评这一举措，提及索尼近期从客户库中删除已购电影的行为破坏了信任。许多人认为数字游戏只是租赁，实体媒体的终结威胁到游戏的长期保存和公平定价。

**标签**: `#gaming`, `#PlayStation`, `#digital rights`, `#physical media`, `#game preservation`

---

<a id="item-7"></a>
## [内燃机互动深度解析](https://ciechanow.ski/internal-combustion-engine/) ⭐️ 8.0/10

发布了一篇关于内燃机的详细互动教程，包含精美插图的机械与工程解释。 这一高质量教育资源使复杂的机械工程知识对大众更易理解，其互动设计增强了对发动机运行的理解。 文章涵盖四冲程循环、润滑和控制系统，同时讨论了现代电子燃油喷射与历史化油器。内容以其清晰性和深度受到好评。

hackernews · StefanBatory · 7月1日 13:04 · [社区讨论](https://news.ycombinator.com/item?id=48746076)

**背景**: 内燃机通过气缸内受控爆炸将燃料和空气转化为机械能。一个多世纪以来，它们为车辆提供动力，最近的进步集中在电子控制以提高效率和降低排放。

**社区讨论**: 评论者指出，尽管发动机机械结构几十年来保持相似，但现代控制系统如电子燃油喷射已大幅改进。一些人分享了关于发动机磨损和流体动力润滑效应的个人经验。

**标签**: `#internal combustion engine`, `#interactive tutorial`, `#engineering`, `#mechanical engineering`, `#educational content`

---

<a id="item-8"></a>
## [Anthropic 的 Fable 5 引发安全和信任争议](https://twitter.com/claudeai/status/2072402636813607381) ⭐️ 8.0/10

Anthropic 于 2026 年 6 月 9 日发布了 Claude Fable 5，但几天后美国政府将其列为危险军需品，限制外国公民访问。该模型因过度激进的安全限制导致无法用于合法任务而受到批评。 这场争议凸显了 AI 安全措施与实际可用性之间日益紧张的矛盾，并削弱了用户对实施过度限制的 AI 公司的信任。将商业 AI 模型列为军需品开创了先例，可能重塑全球 AI 治理格局。 Fable 5 是 Anthropic 声称在 FrontierBench 上得分最高的'Mythos 级'模型，但它会阻止进攻性网络安全查询并回退到 Opus 4.8，用户已发现通过重新措辞请求来绕过限制的方法。

hackernews · mfiguiere · 7月1日 19:35 · [社区讨论](https://news.ycombinator.com/item?id=48752030)

**背景**: Anthropic 开发了 Fable 5 作为一款高度能力强大的 AI 模型，内置了防止滥用的保护措施。美国政府迅速将其纳入出口管制分类，反映了国家安全担忧。批评者认为，这种限制使模型在许多合法应用中几乎无用，并引发了对 AI 公司无限制控制先进 AI 权力的质疑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://www.wired.com/story/anthropic-added-a-new-security-measure-to-get-back-into-the-trump-administrations-good-graces/">Anthropic Added a New Security Measure to Get Back Into... | WIRED</a></li>
<li><a href="https://www.schneier.com/blog/archives/2026/06/anthropics-fable-and-the-state-of-ai.html">Anthropic's Fable and the State of AI - Schneier on Security</a></li>

</ul>
</details>

**社区讨论**: 社区情绪普遍负面，用户 pkoird 称该模型‘糟糕得可笑’且‘被削弱到恶意程度’。其他人表达了对基于美国的 AI 模型的不信任，并预测信任侵蚀可能无法恢复。一些用户建议将该模型用于规划而非代码生成，以降低令牌成本。

**标签**: `#AI safety`, `#Anthropic`, `#model security`, `#trust`, `#community discussion`

---

<a id="item-9"></a>
## [美国解除对 Anthropic 的 Claude Fable 5 和 Mythos 5 的出口管制](https://simonwillison.net/2026/Jun/30/anthropic/#atom-everything) ⭐️ 8.0/10

Anthropic 宣布，美国商务部已解除对其先进 AI 模型 Claude Fable 5 和 Mythos 5 的出口管制，并将于明天开始恢复访问权限。 这一政策变化使得强大的 AI 模型能够在全球更广泛地使用，影响 AI 行业的竞争和监管。 Claude Fable 5 是一款专注于编码的模型，用于复杂的软件开发任务；而 Mythos 5 则设计用于网络安全漏洞的发现和利用。

rss · Simon Willison · 6月30日 23:58

**背景**: 美国政府对先进 AI 模型实施出口管制，以防止敏感技术落入对手手中。Anthropic 开发大型语言模型，注重安全性。出口管制的解除表明对这些特定模型的风险进行了重新评估。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bbc.com/news/articles/cdr42623e1do">Fable and Mythos : Anthropic says US lifts export ban on its advanced...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Fable_5">Claude Fable 5</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mythos_5">Mythos 5</a></li>

</ul>
</details>

**标签**: `#anthropic`, `#claude`, `#export-controls`, `#ai`, `#generative-ai`

---

<a id="item-10"></a>
## [MOTHRAG：无图多跳 RAG 性能超越基于图的系统](https://www.reddit.com/r/MachineLearning/comments/1ukotww/p_mothretrieval_graphfree_multihop_retrieval_via/) ⭐️ 8.0/10

研究者开源了 MOTHRAG，这是一个无图多跳检索增强生成框架，在 HotpotQA、2WikiMultiHopQA 和 MuSiQue 上的准确率优于 GraphRAG、HippoRAG 和 RAPTOR 等基于图的系统，同时无需重建即可实现低成本更新。 这种方法挑战了多跳 RAG 必须依赖知识图谱的普遍假设，为数据频繁变化的应用程序（如新闻或内部文档）提供了更便宜、更灵活的替代方案。 MOTHRAG 使用无图密集索引和查询时编排，在无需 GPU 的情况下通过商用 API 每次查询成本约 0.03 美元。它在大多数基准测试中与基于图的系统持平或更好，但由于检索召回瓶颈，在 MuSiQue 上表现落后。

reddit · r/MachineLearning · /u/Annual-Commercial563 · 7月1日 15:26

**背景**: 多跳检索增强生成（RAG）需要回答涉及连接多条信息的问题。传统方法离线构建知识图谱以捕捉实体关系，但更新图谱需要重新索引整个语料库，成本高昂。MOTHRAG 通过使用密集向量索引并在查询时编排检索步骤来避免这一问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/juliangeymonat-jpg/mothrag">GitHub - juliangeymonat-jpg/mothrag: Deterministic agentic ...</a></li>
<li><a href="https://arxiv.org/abs/2405.14831">[2405.14831] HippoRAG: Neurobiologically Inspired Long-Term ... GitHub - ianliuwd/HippoRAG2: [NeurIPS'24] HippoRAG is a novel ... HippoRAG: Neurobiologically Inspired Long-Term Memory for ... hipporag · PyPI HippoRAG | Proceedings of the 38th International Conference ... [2502.14802] From RAG to Memory: Non-Parametric Continual ...</a></li>
<li><a href="https://microsoft.github.io/graphrag/">Welcome - GraphRAG</a></li>

</ul>
</details>

**社区讨论**: 输入中没有提供社区评论；原始 Reddit 帖子邀请在频繁变化数据上运行 RAG 的用户提供反馈。

**标签**: `#multi-hop RAG`, `#retrieval-augmented generation`, `#knowledge graph`, `#open source`, `#NLP`

---

<a id="item-11"></a>
## [Sentinel Gateway：系统级提示注入防御](https://www.reddit.com/r/MachineLearning/comments/1ukgwk1/a_systemlevel_approach_to_prompt_injection/) ⭐️ 8.0/10

一种名为 Sentinel Gateway 的新型中间件层在 LLM 代理系统中强制执行指令与数据通道的严格分离，通过基于令牌的授权来防止提示注入攻击。 提示注入仍是 LLM 代理中的一个关键安全缺陷，这种系统级方法提供了结构性修复，而非依赖不完善的输入过滤，有望提高生产环境中代理工作流程的安全性。 该实现构建为 FastAPI 中间件，利用签名且有作用域的运行时授权令牌进行工具执行，并包含用于检查和审计日志记录的 Streamlit 界面。

reddit · r/MachineLearning · /u/vagobond45 · 7月1日 09:34

**背景**: 提示注入攻击发生在 LLM 处理包含恶意指令的不可信外部数据时，因为模型无法可靠地区分其原始指令与注入的数据。这从根本上来说很困难，因为在 LLM 中指令和数据共享相同的嵌入空间。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aihaberleri.org/en/news/breakthrough-ai-security-tool-blocks-prompt-injection-without-content-scanning">Breakthrough AI Security Tool Blocks Prompt Injection Without...</a></li>
<li><a href="https://sentinel-gateway.com/?ref=producthunt">Sentinel Gateway — Structural AI Agent Security</a></li>

</ul>
</details>

**标签**: `#prompt injection`, `#LLM security`, `#middleware`, `#agentic workflow`, `#systems design`

---

<a id="item-12"></a>
## [Claude Code 2.1.91 被指秘密遥测代理与时区信息](https://t.me/zaihuapd/42285) ⭐️ 8.0/10

一名逆向工程师发现，Claude Code 2.1.91 版本会静默检查系统时区和代理设置以检测中国用户，并将此信息编码进发送给 Anthropic API 的系统提示中。Anthropic 已承认问题并承诺修复。 这一发现引发了关于广泛使用的 AI 编程工具中秘密数据收集的严重隐私担忧，可能损害开发者的信任。同时也凸显了 AI 辅助软件开发中隐藏的地缘政治针对风险。 该工具检查时区是否设置为 Asia/Shanghai 或 Asia/Urumqi，以及代理 URL 是否指向中国域名或 AI 实验室，然后通过微妙改变系统提示日期格式中的 Unicode 字符来编码结果。这种数据外泄已持续至少三个月才被发现。

telegram · zaihuapd · 7月1日 04:42

**背景**: Claude Code 是 Anthropic 的智能编码工具，帮助开发者在终端中编辑文件和运行命令。系统提示是给 AI 模型的指令，用于设置响应上下文。检测中国用户可能与遵守出口管制或使用政策有关，但秘密遥测违反了用户对隐私的期望。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.techtimes.com/articles/319415/20260701/claude-code-hid-proxy-fingerprints-system-prompts-anthropic-promises-fix.htm">Claude Code Hid Proxy Fingerprints in System Prompts: Anthropic Promises Fix</a></li>
<li><a href="https://docs.anthropic.com/en/docs/claude-code/overview">Claude Code overview - Anthropic</a></li>

</ul>
</details>

**标签**: `#privacy`, `#AI`, `#Claude Code`, `#telemetry`, `#reverse engineering`

---

<a id="item-13"></a>
## [英伟达将 DeepSeek V4 推理成本降至五分之一](https://blogs.nvidia.com/blog/inference-software-lowest-token-cost/) ⭐️ 8.0/10

英伟达在 Blackwell 平台上的推理软件栈将 DeepSeek V4 模型的 Token 成本降至原来的五分之一，SGLang 引擎吞吐量从 2025 年 4 月的约 2200 Tokens/秒/GPU 提升至 6 月的约 11200 Tokens/秒/GPU。 这一显著的成本降低使大规模 AI 推理更具经济性，直接减少了企业部署大语言模型的运营开支，同时展示了英伟达在 AI 硬件和软件优化方面的持续领先地位。 优化涵盖内核融合、显存压缩、量化精度路径，以及改进的内存预算与可中断计算图支持。英伟达预计未来通过分解式服务和多 Token 预测等高级优化，系统级吞吐量最高可提升 20 倍。

telegram · zaihuapd · 7月1日 10:36

**背景**: 大语言模型推理成本常以每 GPU 每秒生成的 Token 数衡量，降低该指标直接影响部署经济性。SGLang 是一种流行的开源 LLM 推理引擎，广泛用于生产环境。分解式服务将预填充和解码阶段分离以优化资源利用率，而多 Token 预测则训练模型同时预测多个未来 Token，从而提高推理效率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/sgl-project/sglang">GitHub - sgl-project/ sglang : SGLang is a high-performance serving...</a></li>
<li><a href="https://docs.nvidia.com/dynamo/user-guides/disaggregated-serving">Disaggregated Serving | NVIDIA Dynamo Documentation</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#DeepSeek V4`, `#AI Inference`, `#Blackwell`, `#Performance Optimization`

---

<a id="item-14"></a>
## [Visa、Mastercard 等 140 多家企业联合发起 Open Standard 稳定币网络](https://www.reuters.com/business/consortium-including-visa-mastercard-jointly-launch-new-global-stablecoin-2026-06-30/) ⭐️ 8.0/10

2026 年 6 月 30 日，包括 Visa、Mastercard 和 Coinbase 在内的 140 多家企业联合宣布推出 Open Standard 稳定币网络。该网络计划于今年晚些时候发行 Open USD (OUSD)，企业可免费铸造和赎回代币，储备收益由合作伙伴共享。 这一举措标志着稳定币在加密交易之外获得重大机构采用，旨在为全球支付打造开放、低成本的基础设施。在支付巨头和收益共享模式的支持下，它可能加速稳定币在日常商业中的应用，并挑战现有的封闭系统。 Open Standard 定位为中立、共同治理的实体；Open USD 将通过受监管的合作伙伴网络发行，DBS 银行和 Tempo 被列为初始参与者。该联盟涵盖支付、科技和金融等多个领域的公司，显示出广泛的行业支持。

telegram · zaihuapd · 7月1日 11:06

**背景**: 稳定币是锚定美元等稳定资产的加密货币，常用于加密交易，但尚未成为支付主流。2025 年签署成为法律的《GENIUS 法案》为支付稳定币建立了联邦监管框架，为此类举措提供了法律明确性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.forbes.com/sites/christiancatalini/2026/06/30/why-an-open-standard-will-win-the-stablecoin-race/">Why An Open Standard Will Win The Stablecoin Race</a></li>
<li><a href="https://www.theblock.co/post/406736/visa-stripe-coinbase-join-open-usd-stablecoin-shares-reserve-revenue">Visa, Stripe, Coinbase and more join Open USD stablecoin that shares reserve revenue | The Block</a></li>
<li><a href="https://en.wikipedia.org/wiki/GENIUS_Act">GENIUS Act - Wikipedia</a></li>

</ul>
</details>

**标签**: `#stablecoins`, `#payments`, `#Visa`, `#Mastercard`, `#blockchain`

---

<a id="item-15"></a>
## [ChatGPT 每周用户翻倍至 2 亿](https://t.me/zaihuapd/42298) ⭐️ 8.0/10

OpenAI 宣布 ChatGPT 现在每周活跃用户超过 2 亿，是 2023 年 11 月报告的 1 亿用户的两倍。 这一里程碑凸显了 ChatGPT 在生成式 AI 市场中的快速主流采用和主导地位，92%的财富 500 强公司正在使用 OpenAI 的产品。 增长得益于 GPT-4o Mini 的发布，这款更便宜且更智能的模型使 API 使用量翻了一番。传言苹果和英伟达可能成为 OpenAI 下一轮融资的投资者。

telegram · zaihuapd · 7月1日 13:01

**背景**: ChatGPT 是 OpenAI 开发的对话式 AI 聊天机器人，于 2022 年 11 月推出，迅速走红，两个月内月活用户达到 1 亿。GPT-4o Mini 于 2024 年 7 月发布，是 GPT-4o 的较小版本，取代了 GPT-3.5 Turbo，以更低成本提供更优性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-4o_mini">GPT-4o mini</a></li>
<li><a href="https://www.linkedin.com/posts/harness-ai_say-hello-to-gpt-4o-mini-openai-has-activity-7219978703345192961-VYB6">Say hello to GPT - 4 o mini OpenAI has just launched their latest...</a></li>

</ul>
</details>

**标签**: `#AI`, `#ChatGPT`, `#OpenAI`, `#adoption`, `#enterprise`

---

<a id="item-16"></a>
## [国巨 7 月 1 日起电容涨价五成](https://www.trendforce.com/news/2026/07/01/news-passive-component-prices-rise-as-yageo-reportedly-begins-broadest-capacitor-hike-in-years-on-july-1/) ⭐️ 8.0/10

台湾被动元件厂商国巨宣布自 2026 年 7 月 1 日起，将全线电容产品（包括 MLCC、铝电解电容、钽电容）价格调涨约五成，为近年最大范围涨价。 此次涨价受地缘政治、能源与原材料成本上升推动，也反映了 AI 服务器和电动车对高端被动元件需求的增长。作为国巨首次对过半直接客户涨价，此举将显著提振公司营收与利润率，并可能引发全行业价格调整。 高端电容现货价近一个月内上涨近十倍，官方报价涨幅约五成。电容占国巨营收约一半，此次是国巨首次对占比过半的直接客户涨价。

telegram · zaihuapd · 7月1日 14:34

**背景**: 被动元件（如电容、电阻、电感）是电子电路的基本元件，不放大或产生能量，但对电路稳定性至关重要。MLCC（片式多层陶瓷电容器）是一种常见的电容类型，由多层陶瓷介质堆叠而成，广泛用于各类电子产品。国巨是全球主要的被动元件供应商之一，其 MLCC 产品与日韩厂商竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/349101940">MLCC是什么，其特点和作用是什么？ - 知乎</a></li>

</ul>
</details>

**标签**: `#capacitors`, `#price increase`, `#supply chain`, `#AI hardware`, `#passive components`

---