---
layout: default
title: "Horizon Summary: 2026-07-07 (ZH)"
date: 2026-07-07
lang: zh
---

> 从 65 条内容中筛选出 16 条重要资讯。

---

1. [Januscape：潜伏 16 年的 KVM 虚拟机逃逸漏洞影响 Intel 和 AMD](#item-1) ⭐️ 9.0/10
2. [Kokoro：本地、CPU 友好的高音质文本转语音](#item-2) ⭐️ 8.0/10
3. [欧盟聊天控制 1.0 与 2.0：监控与隐私之战](#item-3) ⭐️ 8.0/10
4. [欧盟强制新车配备驾驶员监测摄像头](#item-4) ⭐️ 8.0/10
5. [欧盟聊天控制提案在议会首轮投票通过](#item-5) ⭐️ 8.0/10
6. [在关键场景中，98%的成功率远远不够](#item-6) ⭐️ 8.0/10
7. [Astro 7.0 发布基于 Rust 的编译器和 Markdown 管道](#item-7) ⭐️ 8.0/10
8. [sqlite-utils 4.0 发布，新增数据库迁移功能](#item-8) ⭐️ 8.0/10
9. [腾讯发布 Hy3：295B MoE 模型，21B 活跃参数，Apache 2.0 许可](#item-9) ⭐️ 8.0/10
10. [MIRA：一个 5B 参数交互世界模型，用于《火箭联盟》](#item-10) ⭐️ 8.0/10
11. [将神经网络约束在可信 LoRA 子空间以阻止恶意微调](#item-11) ⭐️ 8.0/10
12. [马斯克解散 xAI，更名为 SpaceXAI 并入 SpaceX](#item-12) ⭐️ 8.0/10
13. [中国拟投 2 万亿元建设全国算力网络](#item-13) ⭐️ 8.0/10
14. [Anthropic 发布 Claude Sonnet 5，增强代理能力](#item-14) ⭐️ 8.0/10
15. [DeepSeek 自研 AI 推理芯片](#item-15) ⭐️ 8.0/10
16. [商务部拟限制顶尖 AI 模型出口](#item-16) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Januscape：潜伏 16 年的 KVM 虚拟机逃逸漏洞影响 Intel 和 AMD](https://github.com/V4bel/Januscape) ⭐️ 9.0/10

研究人员公开了 Januscape（CVE-2026-53359），这是 KVM shadow MMU 中的一个严重释放后使用漏洞，允许客户机在 Intel 和 AMD x86 系统上逃逸到宿主机。该漏洞在 Linux 内核中潜伏了约 16 年，已发布的概念验证利用可导致宿主机内核崩溃。 这是首个同时影响 Intel 和 AMD KVM 的虚拟机逃逸漏洞，对依赖虚拟机隔离的多租户云环境构成直接威胁。成功利用可让攻击者突破虚拟机并破坏宿主机，进而可能访问其他虚拟机。 该漏洞位于 KVM 的 shadow MMU 模拟中，涉及一个释放后使用缺陷，可破坏宿主内核的 shadow 页表。概念验证利用已发布在 GitHub 上，在 Red Hat Enterprise Linux 等发行版中，本地普通用户还可利用该缺陷提权至 root。

telegram · zaihuapd · 7月7日 10:14

**背景**: KVM（基于内核的虚拟机）是一个 Linux 内核模块，使内核能够充当 hypervisor。Shadow MMU 用于在硬件嵌套页表（NPT）或扩展页表（EPT）未完全利用时管理客户虚拟内存。释放后使用漏洞是指程序在内存被释放后继续使用该内存，可能使攻击者执行任意代码。虚拟机逃逸是一种安全利用，虚拟机内运行的代码突破隔离与宿主机操作系统交互。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/16-year-old-linux-kvm-flaw-lets-guest.html">16-Year-Old Linux KVM Flaw Lets Guest VMs Escape to Host on Intel and AMD x86 Systems</a></li>
<li><a href="https://docs.kernel.org/virt/kvm/x86/mmu.html">The x86 kvm shadow mmu — The Linux Kernel documentation</a></li>
<li><a href="https://en.wikipedia.org/wiki/VM_escape">VM escape</a></li>

</ul>
</details>

**标签**: `#security`, `#virtualization`, `#KVM`, `#vulnerability`, `#VM escape`

---

<a id="item-2"></a>
## [Kokoro：本地、CPU 友好的高音质文本转语音](https://ariya.io/2026/03/local-cpu-friendly-high-quality-tts-text-to-speech-with-kokoro/) ⭐️ 8.0/10

Kokoro 是一个拥有 8200 万个参数的开源文本转语音模型，能够在 CPU 上高效运行，无需 GPU 即可实现本地高质量语音合成。 这很重要，因为它使高质量语音合成更容易获得，特别是对于没有强大 GPU 的用户，并促进用于无障碍和内容消费的社区项目。 该模型通过 mlx-audio 库在苹果芯片上表现出高效性能，并支持手动 IPA 发音指南以提高准确性。

hackernews · speckx · 7月7日 18:24 · [社区讨论](https://news.ycombinator.com/item?id=48821576)

**背景**: 文本转语音（TTS）将书面文字转换为语音。许多高质量的 TTS 模型需要强大的 GPU，限制了本地使用。Kokoro 是为 CPU 推理设计的轻量级模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/Kokoro_TTS">Kokoro TTS</a></li>
<li><a href="https://kokorottsai.com/">Kokoro TTS: Advanced AI Text-to-Speech Model with 82M parameters</a></li>

</ul>
</details>

**社区讨论**: 用户报告在无障碍产品和文章阅读器中使用 Kokoro 的积极体验，其中一位用户开发了 Chrome 扩展程序实现同步阅读和高亮。部分用户指出在单个词语发音上的局限性，但赞赏手动发音调整功能。

**标签**: `#TTS`, `#Text-to-Speech`, `#Kokoro`, `#AI`, `#Accessibility`

---

<a id="item-3"></a>
## [欧盟聊天控制 1.0 与 2.0：监控与隐私之战](https://fightchatcontrol.eu/chat-control-overview) ⭐️ 8.0/10

欧盟提出了两项名为“聊天控制”（1.0 和 2.0）的立法提案，旨在打击儿童性虐待材料，其中聊天控制 2.0 要求对加密通信进行强制扫描，引发了关于加密和隐私的争论。 这项立法可能为削弱整个欧盟的端到端加密开创先例，影响数百万用户并威胁数字隐私权，同时也引发了对大规模监控的担忧。 聊天控制 1.0 是对 ePrivacy 指令的临时豁免，允许自愿扫描未加密消息，已于 2026 年 4 月到期；而聊天控制 2.0 则提出对加密内容进行强制扫描，包括所有私人聊天和电子邮件。

hackernews · gasull · 7月7日 14:23 · [社区讨论](https://news.ycombinator.com/item?id=48818311)

**背景**: 端到端加密（E2EE）确保只有发送者和接收者能阅读消息，甚至服务提供商也无法访问内容。欧盟的聊天控制提案旨在检测儿童性虐待材料（CSAM），但批评者认为这将破坏加密并导致大规模监控。这场辩论将儿童保护与基本隐私权对立起来。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control">Chat Control - Wikipedia</a></li>
<li><a href="https://www.patrick-breyer.de/en/posts/chat-control/">Chat Control: The EU's CSAM scanner proposal</a></li>
<li><a href="https://thecybersecguru.com/news/eu-chat-control-2026-guide/">EU Chat Control Is Back - And This Time It Might Actually Pass | The CyberSec Guru</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了强烈反对，认为聊天控制是'赋予我独裁权力'的伎俩，并批评其广泛的监控范围。一些人质疑在不破坏端到端加密的情况下扫描加密消息的技术可行性，提及苹果的设备端 CSAM 扫描仪作为替代方案。总体情绪对这项立法持压倒性负面态度。

**标签**: `#encryption`, `#privacy`, `#EU legislation`, `#surveillance`, `#policy`

---

<a id="item-4"></a>
## [欧盟强制新车配备驾驶员监测摄像头](https://allaboutcookies.org/eu-mandatory-distracted-driver-system) ⭐️ 8.0/10

自 2024 年 7 月 7 日起，所有在欧盟销售的新车必须配备驾驶员瞌睡和注意力警告系统，该系统通过车内摄像头监测驾驶员行为。 该法规旨在减少因分心和瞌睡造成的事故，可能挽救生命，但也引发了驾驶员和汽车制造商对隐私和用户体验的重大担忧。 该系统使用红外摄像头追踪眼球运动和头部位置，在检测到分心或瞌睡时发出警报。适用于乘用车（M 类）和轻型商用车（N 类）。

hackernews · nickslaughter02 · 7月7日 20:50 · [社区讨论](https://news.ycombinator.com/item?id=48823557)

**背景**: 驾驶员监测系统（DMS）是检测疲劳或注意力不集中迹象的高级安全功能。此前仅在部分豪华车型中可选，但欧盟《通用安全法规》（GSR）现要求所有新车必须配备，以提升道路安全。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Driver_monitoring_system">Driver monitoring system - Wikipedia</a></li>
<li><a href="https://www.aptiv.com/en/insights/article/what-is-a-driver-monitoring-system">What Is a Driver-Monitoring System?</a></li>
<li><a href="https://jungo.com/driving-safety-in-the-age-of-gsr-2024-how-driver-monitoring-systems-can-help/">Driving Safety in the Age of GSR 2024: How Driver Monitoring Systems Can Help - Jungo</a></li>

</ul>
</details>

**社区讨论**: 评论显示观点分歧：一些用户赞扬安全性提升，并引用福特 Blue Cruise 的积极体验；另一些人则批评侵入式监测和现代汽车糟糕的用户体验，担心误报和隐私侵蚀。

**标签**: `#regulation`, `#automotive`, `#privacy`, `#safety`, `#ux`

---

<a id="item-5"></a>
## [欧盟聊天控制提案在议会首轮投票通过](https://www.heise.de/en/news/Showdown-in-Strasbourg-The-unexpected-return-of-Chat-Control-1-0-11356680.html) ⭐️ 8.0/10

欧洲议会投票通过了颇具争议的《聊天控制》法规（CSAR）的首轮审议，并将在周四进行最终表决。该提案要求对私人消息进行自动扫描，以查找儿童性虐待内容。 若该法通过，将要求对所有私人通信（包括加密消息）进行扫描，引发严重的隐私和安全担忧。立法程序为支持者提供了战术优势，使否决变得更加困难。 周四，修改或否决提案需要绝对多数（361 票），而通过只需出席议员的简单多数。许多议员可能已因夏休离开，导致法定人数减少。

hackernews · miroljub · 7月7日 15:16 · [社区讨论](https://news.ycombinator.com/item?id=48819008)

**背景**: 《聊天控制》正式名称为《预防和打击儿童性虐待法规》（CSAR），由欧盟委员会于 2022 年 5 月提出。其目的是遏制儿童性虐待材料（CSAM）的传播，但批评者认为它将破坏端到端加密并导致大规模监控。此前该立法的数次尝试均被否决。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Regulation_to_Prevent_and_Combat_Child_Sexual_Abuse">Chat Control - Wikipedia</a></li>
<li><a href="https://www.eff.org/deeplinks/2026/04/eu-parliament-blocks-mass-scanning-our-chats-whats-next">EU Parliament Blocks Mass-Scanning of Our Chats—What's Next? | Electronic Frontier Foundation</a></li>
<li><a href="https://www.patrick-breyer.de/en/posts/chat-control/">Chat Control: The EU's CSAM scanner proposal</a></li>

</ul>
</details>

**社区讨论**: 评论者对立法的策略表示失望，指出支持者反复推动不受欢迎的法律直至通过。有人引用了让-克洛德·容克关于无视反对声的言论。多数评论反对该提案，认为它威胁民主和隐私。

**标签**: `#EU legislation`, `#privacy`, `#surveillance`, `#encryption`, `#technology policy`

---

<a id="item-6"></a>
## [在关键场景中，98%的成功率远远不够](https://whynothugo.nl/journal/2026/07/03/98-isnt-very-much/) ⭐️ 8.0/10

文章指出，在需要近乎完美的场景中，98%的成功率远远不够，并通过清洁和票务等例子加以说明，强调了高百分比声称的统计陷阱。 这很重要，因为它挑战了软件工程和可靠性中关于可接受故障率的常见假设，促使开发者考虑边缘情况和实际影响，而不是依赖误导性的百分比。 文章使用清洁例子：去除 98%的针叶仍然留下可见的杂乱，以及票务例子：2%的失败率可能意味着显著的收入损失或客户沮丧。作者强调，接近 100%的百分比可能掩盖大量的绝对失败数量。

hackernews · speckx · 7月7日 12:45 · [社区讨论](https://news.ycombinator.com/item?id=48816959)

**背景**: 在软件工程中，“边缘情况”是指在极端操作参数下才会出现的问题，这些情况在开发过程中常被忽视。文章基于这样的概念：虽然 98%的成功率听起来令人印象深刻，但对于支付处理或安全关键系统等任务，即使很小的故障率也可能产生严重后果。讨论涉及统计显著性与实际影响之间的差异。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Edge_case">Edge case - Wikipedia</a></li>
<li><a href="https://www.coursera.org/articles/edge-case">What Is an Edge Case? | Coursera</a></li>

</ul>
</details>

**社区讨论**: 社区评论反映了微妙的辩论。一位评论者指出，98%可能足够，具体取决于业务背景，比如浏览器支持中关注 98%的用户是务实的。另一位分享了个人清洁轶事，说明即使 99%的去除率在视觉要求高的任务中也不可接受。第三位指出，真正的问题往往是利润驱动的决策，例如 Ticketmaster 的电话验证失败。总体而言，讨论同意上下文很重要，百分比可能具有误导性。

**标签**: `#reliability`, `#software engineering`, `#statistics`, `#edge cases`

---

<a id="item-7"></a>
## [Astro 7.0 发布基于 Rust 的编译器和 Markdown 管道](https://astro.build/blog/astro-7/) ⭐️ 8.0/10

Astro 7.0 是 Astro 网页框架的一个主要版本，引入了基于 Rust 的编译器和 Markdown 管道，将依赖项从 247 个减少到 190 个，并提升了构建性能。 此版本标志着 JavaScript 生态系统向性能和简化迈出了重要一步，Rust 编译器缩短了构建时间，依赖项减少使项目更易于维护。它使构建内容驱动型网站的开发者受益，提供了更快、更精简的构建。 根据 node-modules.dev 的验证，依赖项数量从 v6 的 247 个降到了 v7 的 190 个。基于 Rust 的编译器和 Markdown 管道由名为 Princesseuh 的开发者贡献。

hackernews · saikatsg · 7月7日 18:30 · [社区讨论](https://news.ycombinator.com/item?id=48821653)

**背景**: Astro 是一个现代网页框架，专为博客、营销网站和文档等内容导向型网站设计。它采用“孤岛”架构，通过仅发送最少的 JavaScript 来实现快速初始加载。与基于 JavaScript 的工具相比，Rust 编译器可以显著加快解析和打包速度，使构建更快、更高效。

**社区讨论**: Rust 相关贡献的开发者 Princesseuh 回答了关于实现的问题。用户对依赖项减少以及高效构建静态网站的能力表示赞赏，但也有一些人表示困惑，认为在众多框架中 Astro 的角色不明确，并担心七个大版本意味着频繁的破坏性更改。

**标签**: `#astro`, `#web-framework`, `#rust`, `#dependency-reduction`, `#frontend`

---

<a id="item-8"></a>
## [sqlite-utils 4.0 发布，新增数据库迁移功能](https://simonwillison.net/2026/Jul/7/sqlite-utils-4/#atom-everything) ⭐️ 8.0/10

sqlite-utils 4.0 引入了三大主要功能：数据库迁移、通过新的 db.atomic() 方法实现的嵌套事务，以及对复合外键的支持。这是自 2020 年 11 月 3.0 版本以来的首个重大版本更新。 数据库迁移是长期期待的功能，使 sqlite-utils 更适合在生产或协作项目中管理不断演进的数据库。此版本巩固了该工具作为 Python 开发者全面 SQLite 工具包的地位。 迁移使用 sqlite-utils 库以 Python 文件定义，利用强大的 table.transform() 方法来实现超出 SQLite 的 ALTER TABLE 语句范围的复杂模式更改。该工具会跟踪已应用的迁移，并自动应用待处理的迁移。

rss · Simon Willison · 7月7日 19:32

**背景**: sqlite-utils 是一个用于创建、操作和查询 SQLite 数据库的 Python 库及命令行工具。数据库迁移允许开发者对数据库模式进行版本控制并逐步应用更改，这是应用程序开发中的一个关键功能，而 SQLite 本身并不内置此支持。

**标签**: `#sqlite`, `#python`, `#database`, `#migrations`, `#open-source`

---

<a id="item-9"></a>
## [腾讯发布 Hy3：295B MoE 模型，21B 活跃参数，Apache 2.0 许可](https://simonwillison.net/2026/Jul/6/hy3/#atom-everything) ⭐️ 8.0/10

腾讯 Hy 团队发布了 Hy3，这是一个 295B 参数的混合专家（MoE）模型，具有 21B 活跃参数和 3.8B MTP 层参数，采用 Apache 2.0 许可。该模型在性能上超越同尺寸模型，可与参数规模大 2-5 倍的旗舰开源模型匹敌。 此次发布展示了中国在开源大语言模型领域日益增长的能力，提供了一个可与更大模型竞争的高效 MoE 模型。这可能降低开发者和企业部署强大 AI 的门槛，尤其是通过 OpenRouter 提供的免费试用（截至 7 月 21 日）。 完整模型在 Hugging Face 上为 598GB，FP8 量化版本为 300GB，支持 256K token 的上下文长度。该模型在 OpenRouter 上免费提供至 2026 年 7 月 21 日。

rss · Simon Willison · 7月6日 23:57

**背景**: 混合专家（MoE）是一种神经网络架构，使用多个专门的子网络（专家）和一个门控机制，每个输入只激活一部分专家，从而在总参数更大的情况下降低计算成本。Hy3 模型在 295B 总参数中仅有 21B 活跃参数，这意味着它在高效运行的同时实现了高性能。

**标签**: `#AI`, `#machine learning`, `#open source`, `#MoE`, `#Tencent`

---

<a id="item-10"></a>
## [MIRA：一个 5B 参数交互世界模型，用于《火箭联盟》](https://www.reddit.com/r/MachineLearning/comments/1upofuw/mira_multiplayer_interactive_world_models_trained/) ⭐️ 8.0/10

MIRA 是一个 50 亿参数的交互式世界模型，专为《火箭联盟》多人游戏设计，基于 1 万小时的合成数据训练，可在单块 B200 GPU 上以 20fps 实时模拟四名玩家。开发者已发布可玩演示、技术报告、代码以及 1000 小时的四人游戏数据集。 此次发布推动了多智能体交互环境中的世界模型研究，证明了大模型能够实时模拟复杂的多人游戏。它将加速强化学习、游戏 AI 和交互式模拟器的研究，开源发布降低了社区参与门槛。 该模型有 50 亿参数，可在单块 NVIDIA B200 GPU 上为 4 名玩家提供 20fps 的实时模拟。训练数据包含 1 万小时合成《火箭联盟》游戏录像，其中 1000 小时的四人游戏数据作为数据集发布。

reddit · r/MachineLearning · /u/MasterScrat · 7月7日 07:59

**背景**: 世界模型是学习环境内部表征的人工智能系统，能够模拟可能的未来状态。它们在强化学习和规划中至关重要，因为智能体无需真实交互即可想象结果。MIRA 将该概念扩展到多人场景，并实现了实时性能。

**标签**: `#world models`, `#reinforcement learning`, `#game AI`, `#interactive AI`, `#Rocket League`

---

<a id="item-11"></a>
## [将神经网络约束在可信 LoRA 子空间以阻止恶意微调](https://www.reddit.com/r/MachineLearning/comments/1uq68li/what_if_a_model_could_only_learn_what_trusted/) ⭐️ 8.0/10

一篇新论文提出了一种防御微调投毒的方法，将权重更新约束在可信 LoRA 适配器张成的子空间中，使恶意更新在几何上不可达。 该方法通过从根本上限制模型能学习的内容，解决了微调大型模型中的一个关键安全漏洞——即恶意数据可能引入隐藏后门。 该方法在 196 个公开 LoRA 适配器上进行了测试，包括自适应攻击，结果显示攻击成功率大幅下降，同时在适配器池覆盖的任务上保留了有用的适应能力。

reddit · r/MachineLearning · /u/Bright_Warning_8406 · 7月7日 20:00

**背景**: 使用 LoRA（低秩适应）微调大型语言模型是一种常见的效率方法。然而，恶意行为者可以注入有毒数据来创建后门。传统防御检测或缓解有毒数据，但这项工作从几何上限制了模型的更新空间。

**标签**: `#AI Safety`, `#Fine-tuning`, `#LoRA`, `#Adversarial Defense`, `#Machine Learning`

---

<a id="item-12"></a>
## [马斯克解散 xAI，更名为 SpaceXAI 并入 SpaceX](https://x.com/i/status/2074214064746832060) ⭐️ 8.0/10

埃隆·马斯克宣布解散 xAI，将其更名为 SpaceXAI 并整合到 SpaceX 中。该公司已开始使用 SpaceXAI 这一名称，首次出现在与 Anthropic 的计算合作公告中。 这代表了 AI 行业的重大战略转变，一个最著名的 AI 实验室被并入一家太空技术公司。这可能加速 AI 在太空探索和卫星通信中的应用。 xAI 已在与 Anthropic 的合作公告中采用了 SpaceXAI 品牌，埃隆·马斯克在社交媒体上确认：“xAI 将作为独立公司解散，以后就是 SpaceXAI，即 SpaceX 的 AI 产品。”xAI 的品牌和实体都将消失。

telegram · zaihuapd · 7月7日 02:30

**背景**: xAI 由埃隆·马斯克于 2023 年创立，旨在与 OpenAI 等 AI 实验室竞争。SpaceX 是马斯克的航天制造商和太空运输公司。xAI 并入 SpaceX 表明 AI 开发将直接与 SpaceX 的目标对齐，例如增强星舰和星链的自主系统。

**标签**: `#AI`, `#SpaceX`, `#xAI`, `#Elon Musk`, `#business`

---

<a id="item-13"></a>
## [中国拟投 2 万亿元建设全国算力网络](https://t.me/zaihuapd/42399) ⭐️ 8.0/10

中国计划未来五年投入约 2 万亿元（2950 亿美元），建设全国互联数据中心网络，由国有电信企业运营主要设施。该计划优先采用华为等本土供应商的 AI 芯片，目标本地化率至少 80%，以减少对英伟达、AMD 等美企的依赖。 这一举措具有重要战略意义，旨在将分散的区域算力资源整合为统一网络，让企业和公共部门更易获得高性能计算。同时也凸显了中国在 AI 基础设施和半导体领域推动技术自主的决心，可能对全球供应链产生地缘政治影响。 该计划是北京“六网”基础设施战略的关键一环，目前中国电信、联通等已推出“token 套餐”，把算力像移动数据一样打包销售，为大规模 AI 应用铺路。

telegram · zaihuapd · 7月7日 04:45

**背景**: 中国于 2022 年启动的“东数西算”工程，旨在将数据处理从沿海地区转移到能源丰富、气候凉爽的西部地区。新的全国算力网络在此基础上扩展，打造一个完全集成的中心辐射式系统。“Token 套餐”指的是一种计费模式，将计算资源像移动数据一样计量并销售，使用户能够按需访问云计算。

**标签**: `#China`, `#AI infrastructure`, `#computing network`, `#semiconductors`, `#policy`

---

<a id="item-14"></a>
## [Anthropic 发布 Claude Sonnet 5，增强代理能力](https://t.me/zaihuapd/42404) ⭐️ 8.0/10

Anthropic 发布了 Claude Sonnet 5，称其是迄今代理能力最强的 Sonnet 模型，可以规划、使用浏览器和终端等工具并自主运行。 相比 Sonnet 4.6，此版本在推理、工具使用、编码和知识工作上大幅提升，性能接近 Opus 4.8 但价格更低，使先进 AI 更加普惠。 Claude Sonnet 5 即日起面向所有套餐开放，并成为 Free 和 Pro 的默认模型；定价为每百万输入 token 2 美元、输出 token 同样价格（限时价格截止至 2026 年 8 月 31 日）。

telegram · zaihuapd · 7月7日 09:02

**背景**: Claude 是 Anthropic 开发的大语言模型系列，以安全和对齐著称。Sonnet 系列是一个平衡型产品线，以较低成本提供强劲性能，而 Opus 是旗舰模型。本次发布凸显了 Anthropic 对代理能力的重视，即模型可以独立规划并使用外部工具执行任务。

**标签**: `#Anthropic`, `#Claude`, `#LLM`, `#AI`, `#agentic`

---

<a id="item-15"></a>
## [DeepSeek 自研 AI 推理芯片](https://www.reuters.com/world/china/chinas-deepseek-developing-its-own-ai-chip-sources-say-2026-07-07/) ⭐️ 8.0/10

中国 AI 公司 DeepSeek 正在开发自己的 AI 芯片，专注于推理阶段，以减少对英伟达和华为芯片的依赖。该项目始于约一年前，目前仍处于早期阶段，DeepSeek 已开始招募芯片设计工程师并与供应链伙伴接洽。 此举可能显著改变 AI 硬件格局，减少对美国的英伟达和中国竞争对手华为的依赖，尤其是在美国出口管制背景下。这也标志着 DeepSeek 向垂直整合的战略转变，可能降低成本并确保供应链安全。 该芯片专门设计用于推理阶段，即已训练模型为用户生成回答的环节，而非模型训练。DeepSeek 近几个月私下大量招募芯片设计工程师，并与芯片设计、代工和存储公司接洽。

telegram · zaihuapd · 7月7日 11:08

**背景**: DeepSeek 是一家以开发大型语言模型闻名的中国 AI 公司。其模型此前依赖英伟达 H800 和华为昇腾芯片，但美国出口管制限制了中国获取先进半导体的渠道。这促使多家中国 AI 公司探索自研芯片，以对冲地缘政治风险。

**标签**: `#AI chips`, `#DeepSeek`, `#semiconductor`, `#hardware`, `#China`

---

<a id="item-16"></a>
## [商务部拟限制顶尖 AI 模型出口](https://www.reuters.com/world/beijing-is-looking-curbing-overseas-access-chinas-top-ai-models-sources-say-2026-07-07/) ⭐️ 8.0/10

中国商务部近日召集阿里巴巴、字节跳动及智谱等企业开会，讨论限制最先进的国产 AI 模型向海外提供访问，包括尚未发布的模型。 该政策可能重塑全球 AI 技术的获取和贸易格局——中国是 AI 领域的重要参与者。这也表明 AI 技术带来的国家安全担忧正在升级。 讨论内容包括将 AI 核心技术泄露或窃取纳入国家安全法治罪，并考虑限制境外资本投资国内 AI 初创企业。限制范围可能仅适用于未来发布的新模型。

telegram · zaihuapd · 7月7日 11:42

**背景**: 中国 AI 产业快速发展，已产出可与美国同行媲美的模型。对 AI 模型实施出口管制是技术监管的新领域，类似于半导体限制。商务部负责技术出口管制，此举与更广泛的国家安全保护努力一致。

**标签**: `#AI政策`, `#出口管制`, `#国家安全`, `#中国AI`

---