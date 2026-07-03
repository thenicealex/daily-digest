---
layout: default
title: "Horizon Summary: 2026-07-03 (ZH)"
date: 2026-07-03
lang: zh
---

> 从 68 条内容中筛选出 14 条重要资讯。

---

1. [crustc：将整个 Rust 编译器翻译成 C](#item-1) ⭐️ 9.0/10
2. [美国商务部长禁止人口普查中的差分隐私](#item-2) ⭐️ 9.0/10
3. [ECTC 2026：EMIB-T、定制 HBM、HBM4、微流冷却与光子互连](#item-3) ⭐️ 9.0/10
4. [讽刺创业烤箱故事揭示产品开发失败教训](#item-4) ⭐️ 8.0/10
5. [本地智能权利运动倡导本地 AI 运行权](#item-5) ⭐️ 8.0/10
6. [Linux 6.9 中 LUKS 挂起操作的安全回归](#item-6) ⭐️ 8.0/10
7. [阿里巴巴因后门风险禁止 Claude Code](#item-7) ⭐️ 8.0/10
8. [Podman v6.0.0 发布，集成 Quadlet](#item-8) ⭐️ 8.0/10
9. [Immich 3.0 重大版本发布](#item-9) ⭐️ 8.0/10
10. [Postgres 事务：分布式系统超能力](#item-10) ⭐️ 8.0/10
11. [Meta 拥抱面向 AI 计算的 Neocloud 模式](#item-11) ⭐️ 8.0/10
12. [Google Gemini Omni Flash 登顶 Video Arena 排行榜](#item-12) ⭐️ 8.0/10
13. [Anthropic 指控阿里巴巴发动大规模模型蒸馏攻击](#item-13) ⭐️ 8.0/10
14. [中国新规草案：账号休眠注销、AI 标识与个性化推荐关闭](#item-14) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [crustc：将整个 Rust 编译器翻译成 C](https://github.com/FractalFir/crustc) ⭐️ 9.0/10

名为 FractalFir 的开发者完成了一项为期三年的工程，将整个 Rust 编译器（rustc）翻译成 C 语言，创建了 crustc 转译器。这使得 Rust 代码可以在缺乏 LLVM 或 GCC 后端的平台上编译。 这一突破可能使 Rust 能够在任何拥有 C 编译器的平台上运行，包括老旧和冷门硬件，大幅拓展 Rust 的适用范围。同时，它也有可能解决自举问题，允许无需现有 Rust 编译器即可从源码构建 Rust。 据作者称，crustc 项目是已知的第 14 次将 Rust 转译为 C 的尝试。它不仅转译用户程序，还转译了整个 rustc 编译器本身，输出可由 GCC 或其他 C 编译器编译的 C 代码。

hackernews · Philpax · 7月2日 22:57 · [社区讨论](https://news.ycombinator.com/item?id=48768464)

**背景**: 转译（或称源到源编译）是将代码从一种高级语言转换为另一种高级语言，而非转换为机器码。Rust 编译器（rustc）是一个复杂的程序，传统上它生成 LLVM IR 或 GCC 后端代码。通过将 rustc 翻译成 C，crustc 利用了 C 编译器的普遍性，使 Rust 能在没有原生 LLVM 或 GCC 支持的平台上运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/FractalFir/crustc">GitHub - FractalFir/crustc: Entirety of `rustc`, translated to C. · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Source-to-source_compiler">Source-to-source compiler - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区表现出浓厚兴趣，评论者注意到这一‘小众兴趣’所需的奉献精神。有些人讨论了使用双重编译（Diverse Double-Compiling）来验证 Rust 编译器的完整性，另一些人指出 LLVM 曾有过 C 后端但已被移除，现在有复兴它的努力。

**标签**: `#Rust`, `#compiler`, `#transpilation`, `#C`, `#systems programming`

---

<a id="item-2"></a>
## [美国商务部长禁止人口普查中的差分隐私](https://scottaaronson.blog/?p=9902) ⭐️ 9.0/10

2026 年 6 月 4 日，美国商务部长发布了第 DAO-216-26 号指令，禁止在人口普查数据中使用差分隐私和噪声注入技术，将披露避免限制为仅使用粗化技术。 该指令从根本上改变了人口普查局保护隐私的方式，引发了关于个人隐私与数据效用之间平衡的激烈辩论。它直接影响研究人员、政策制定者以及任何依赖准确人口普查数据来进行资源分配和选区重划的人。 该指令明确禁止“噪声注入”（即通过添加随机值来修改数据），并消除了差分隐私的核心技术。它强制要求优先使用粗化（例如四舍五入或聚合），仅将抑制作为最后手段。

hackernews · flowercalled · 7月3日 00:01 · [社区讨论](https://news.ycombinator.com/item?id=48768992)

**背景**: 差分隐私是一种数学框架，通过向统计输出中添加精心校准的噪声来保护个人隐私，同时保持聚合数据的准确性。人口普查局和其他机构一直使用噪声注入来防止受访者被重新识别。该指令逆转了向更强数学隐私保障发展的趋势，转而青睐可能提供较弱保护的简单方法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Differential_privacy">Differential privacy</a></li>
<li><a href="https://www.bea.gov/help/faq/1490">Why didn’t BEA use noise infusion as its statistical disclosure limitation method in its June 10, 2026, news release on “New Foreign Direct Investment in the United States, 2025’’? | U.S. Bureau of Economic Analysis (BEA)</a></li>
<li><a href="https://desfontain.es/blog/banning-noise.html">Banning noise will be a disaster for statistical data products - Ted is writing things</a></li>

</ul>
</details>

**社区讨论**: 评论者对指令背后的政治动机表示困惑，一些人推测其目的是削弱人口普查数据在选区重划等方面的效用。其他人指出，文章缺乏对被禁方法和首选方法的详细比较，并呼吁提供更多关于噪声注入失败的实践证据。

**标签**: `#privacy`, `#differential privacy`, `#census`, `#data policy`, `#statistics`

---

<a id="item-3"></a>
## [ECTC 2026：EMIB-T、定制 HBM、HBM4、微流冷却与光子互连](https://newsletter.semianalysis.com/p/ectc2026) ⭐️ 9.0/10

在 ECTC 2026 上，英特尔详细介绍了其即将推出的带有硅通孔的 EMIB-T 封装技术，用于 HBM4 和 UCIe；而台积电、SK 海力士、三星、美光、Marvell 和 Lightmatter 展示了定制 HBM、HBM4 封装挑战、微流冷却和光子互连方面的进展。 这些进展解决了 AI 硬件性能和扩展性方面的关键瓶颈，特别是高带宽内存和芯片间互连，可能加速下一代 AI 加速器的发展。 英特尔的 EMIB-T 集成了硅通孔以改善供电和更大的封装尺寸，计划今年投入生产；Lightmatter 展示了用于 AI 扩展的光子互连，而 HBM4 封装由于更紧密的凸点间距和散热需求仍是一个关键挑战。

rss · Semianalysis · 7月2日 17:25

**背景**: 半导体封装将芯片连接在一起并连接到外部世界；像 EMIB（嵌入式多芯片互连桥）这样的先进封装实现了高密度互连。HBM（高带宽内存）垂直堆叠 DRAM 芯片，HBM4 是下一代更高带宽的产品。光子互连使用光而非电进行更快、更低功耗的数据传输，对于扩展 AI 系统至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tomshardware.com/pc-components/cpus/intel-details-new-advanced-packaging-breakthroughs-emib-t-paves-the-way-for-hbm4-and-increased-ucie-bandwidth">Intel details new advanced packaging breakthroughs — EMIB-T paves the way for HBM4 and increased UCIe bandwidth | Tom's Hardware</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/semiconductors/intels-emib-t-heads-for-fab-rollout-this-year">Intel's EMIB-T packaging technology set for fab rollout this year — as TSMC CoWoS capacity remains limited, EMIB-T is preparing for advanced AI accelerator designs | Tom's Hardware</a></li>
<li><a href="https://spectrum.ieee.org/optical-interposers">Optical Interconnects: Lightmatter’s Optical Interposers ...</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#packaging`, `#HBM4`, `#photonics`, `#AI hardware`

---

<a id="item-4"></a>
## [讽刺创业烤箱故事揭示产品开发失败教训](https://weli.dev/blog/half-baked-product/) ⭐️ 8.0/10

一篇题为《半生不熟的产品》的讽刺博文讲述了一个创业烤箱项目因期望错位、缺乏领域专长以及承诺落空而失败的故事，在科技社区引起强烈共鸣。 这篇文章对创业产品开发中的常见陷阱（如创始人动机与工程现实的脱节）进行了细腻的批评，为创始人和工程师提供了警示。 创始人受财富驱动而非领域专长，向工程师承诺 20%股权和完全创作自由，但最终这些承诺未能兑现。故事中还提到一个名为 OpenOven 的虚构竞争对手，提供免费烤箱但有许多功能异常的按钮。

hackernews · weli · 7月3日 08:23 · [社区讨论](https://news.ycombinator.com/item?id=48772388)

**背景**: 这篇博文是一个讽刺性寓言，影射创业世界中常见的产品开发失败：创始人常在没有深厚知识的情况下进入行业，对工程师过度承诺，最终得到半生不熟的产品。许多现实中的初创公司面临类似挑战，导致努力白费、期望破灭。

**社区讨论**: 评论者认为这个故事真实得令人不安，有人指出关于工程师动机的部分是“彻头彻尾的谎言”。另一位分享了类似经历：他们功能正常的烤箱被一个免费且功能臃肿的竞争对手击败。整体情绪混合了黑色幽默和对真实创业动态的认同。

**标签**: `#startups`, `#product development`, `#engineering culture`, `#satire`

---

<a id="item-5"></a>
## [本地智能权利运动倡导本地 AI 运行权](https://righttointelligence.org/) ⭐️ 8.0/10

该运动回应了对 AI 即服务（AIaaS）公司监管俘获的担忧，旨在保护 AI 生态系统中的用户隐私、控制权和创新。它可能影响未来围绕 AI 监管和设备权利的政 华硕、戴尔、惠普、联想、微软和微星等主要 OEM 厂商正通过即将推出的 Nvidia RTX Spark 平台支持本地 AI 硬件，表明行业对本地 LLM 使用的大力支持。该运动具有前瞻性，旨在限制性法律通过之前确立权利。

hackernews · thoughtpeddler · 7月2日 23:54 · [社区讨论](https://news.ycombinator.com/item?id=48768951)

**背景**: 本地 LLM 是指在用户自有设备（如 PC 或智能手机）上完全运行的大型语言模型，无需将数据发送到云服务器。这与 AI 即服务（AIaaS）模式形成对比，后者在远程服务器上处理用户数据。潜在法规可能要求安全认证或使用监控，而这对于本地运行的模型可能不可行，从而引发对本地 AI 事实禁令的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/msb-msb/awesome-local-ai">GitHub - msb-msb/awesome-local-ai: A curated list of ...</a></li>
<li><a href="https://whatllm.org/best-local-llm">Best Local LLMs in 2026: Which Model Should You Run Locally ...</a></li>

</ul>
</details>

**社区讨论**: 评论者反应不一：一些人认为鉴于行业对本地 AI 硬件的支持，限制性法律不太可能通过；而另一些人则强调需要积极倡导以防止监管俘获。还有人指出，历史上将数学（如加密）定为非法的做法已经失败，暗示对本地 AI 禁令也会出现类似的抵制。

**标签**: `#AI regulation`, `#local AI`, `#open-source AI`, `#digital rights`, `#LLM`

---

<a id="item-6"></a>
## [Linux 6.9 中 LUKS 挂起操作的安全回归](https://mathstodon.xyz/@iblech/116769502749142438) ⭐️ 8.0/10

自 Linux 6.9 起，`cryptsetup luksSuspend` 操作不再从内存中清除磁盘加密密钥，导致系统挂起时密钥暴露。 这一回归破坏了全盘加密的关键安全功能，依赖 LUKS 挂起操作来保护密钥免受冷启动攻击或设备盗窃的用户可能会面临数据泄露风险。 该错误源于内核提交中意外删除了负责清除加密密钥的一行 C 代码，并且在 Linux 6.9 及更高版本中未被发现超过两年。

hackernews · IngoBlechschmid · 7月2日 15:25 · [社区讨论](https://news.ycombinator.com/item?id=48763035)

**背景**: LUKS（Linux 统一密钥设置）是一种磁盘加密规范。`luksSuspend` 命令会挂起 LUKS 设备并从内核内存中移除解密密钥，恢复时需要重新输入密码。该设计旨在防止冷启动攻击——攻击者通过物理访问可以转储内存内容。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.man7.org/linux//man-pages/man8/cryptsetup-luksSuspend.8.html">cryptsetup-luksSuspend (8) - Linux manual page - man7.org</a></li>
<li><a href="https://news.ycombinator.com/item?id=48763035">Since Linux 6.9, LUKS suspend stopped wiping disk-encryption ...</a></li>
<li><a href="https://byteiota.com/luks-suspend-broken-since-kernel-6-9-two-year-gap/">LUKS Suspend Broken Since Kernel 6.9: Two-Year Gap</a></li>

</ul>
</details>

**社区讨论**: 评论者就严重性展开辩论：有人认为挂起至 RAM 本身就保留了密钥，因此该回归主要影响边境检查等特定场景；另一些人则指出该错误很严重，缺乏自动化测试使其持续存在。

**标签**: `#security`, `#linux-kernel`, `#disk-encryption`, `#LUKS`

---

<a id="item-7"></a>
## [阿里巴巴因后门风险禁止 Claude Code](https://www.reuters.com/world/china/alibaba-ban-claude-code-workplace-over-alleged-backdoor-risks-source-says-2026-07-03/) ⭐️ 8.0/10

阿里巴巴已下令所有员工卸载 Claude Code 及其他 Anthropic 产品，包括 Sonnet、Opus 和 Fable，禁令将于 2026 年 7 月 10 日生效。此前，Anthropic 指控阿里巴巴在 4 月 22 日至 6 月 5 日间使用了约 2.5 万个虚假账号与 Claude 交互超过 2800 万次。 此事件凸显了中美在 AI 安全领域日益紧张的局势，以及企业使用能访问专有代码库的云端编码助手所面临的风险。这可能促使其他公司重新考虑对外部 AI 工具的依赖。 阿里巴巴此前曾报销员工使用 Claude、GPT 和 Gemini 等外部模型的费用。Anthropic 的指控导致其收紧风控，此次禁令不仅涵盖 Claude Code，还包括 Sonnet、Opus 和 Fable 模型。

hackernews · nsoonhui · 7月3日 08:31 · [社区讨论](https://news.ycombinator.com/item?id=48772443)

**背景**: Claude Code 是 Anthropic 开发的 AI 编码代理，可读取代码库、编辑文件并在终端中运行命令。Anthropic 的模型采用“宪法 AI”技术训练以提升伦理合规性。美国联邦机构也曾因合同纠纷逐步淘汰 Claude，这凸显了更广泛的地缘政治关切。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论观点不一：有人回忆之前 Claude 消耗用量或降级模型的事件，加剧了不信任；也有人认为所有远程 AI 都存在安全风险，企业对访问专有代码的工具变得更加谨慎。一份泄露的中文 Telegram 消息详细说明了禁令指令。

**标签**: `#AI`, `#Security`, `#Enterprise`, `#Claude`, `#Geopolitics`

---

<a id="item-8"></a>
## [Podman v6.0.0 发布，集成 Quadlet](https://blog.podman.io/2026/07/introducing-podman-v6-0-0/) ⭐️ 8.0/10

Podman v6.0.0 这个无守护进程容器引擎的主要版本已发布，增强了 Quadlet 支持，可通过 systemd 单元文件声明式管理容器。 作为 Docker 的主要替代品，Podman v6.0.0 提升了易用性和 systemd 集成，有望加速在 DevOps 及生产环境中的采用。 此版本核心是 Quadlet，用户可在 systemd 单元文件中定义容器、Pod 和网络，简化部署。社区反馈表明 docker-compose 兼容性良好，但也存在细微不兼容和发行版支持不足的问题。

hackernews · soheilpro · 7月2日 14:23 · [社区讨论](https://news.ycombinator.com/item?id=48762098)

**背景**: Podman 是一个无守护进程、支持 rootless 的容器引擎，旨在作为 Docker 的即插即用替代品。Quadlet 是一个与 systemd 集成、声明式管理容器的工具，可实现自动更新和回滚等功能。此版本在此基础上改进，提升了开发者和运维人员的使用体验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.podman.io/en/latest/markdown/podman-quadlet.1.html">podman-quadlet — Podman documentation</a></li>
<li><a href="https://www.redhat.com/en/blog/quadlet-podman">Make systemd better for Podman with Quadlet - Enable Sysadmin</a></li>

</ul>
</details>

**社区讨论**: 社区反应褒贬不一：许多人称赞 Podman 从 Docker 迁移的便利性和 Quadlet 的威力，但也有人批评缺乏对 Ubuntu 等流行发行版的官方包支持，以及细微的 Docker 不兼容问题，可能给依赖 Docker 特定行为的项目带来麻烦。

**标签**: `#podman`, `#containers`, `#docker-alternative`, `#devops`, `#release`

---

<a id="item-9"></a>
## [Immich 3.0 重大版本发布](https://github.com/immich-app/immich/discussions/29439) ⭐️ 8.0/10

Immich 3.0 已发布，这是广受欢迎的开源自托管照片管理平台的一次重大更新。新版本包含了社区贡献的错误修复和改进。 此次发布巩固了 Immich 作为 Google Photos 领先的自托管替代品的地位，让用户完全掌控自己的数据。其不断增强的功能集和活跃的社区使其成为注重隐私的用户的不二之选。 该版本未引入端到端加密，这是社区讨论的热点。许多用户将 Immich 与 Tailscale 或全盘加密等工具结合使用以增强安全性。

hackernews · hashier · 7月2日 14:13 · [社区讨论](https://news.ycombinator.com/item?id=48761944)

**背景**: Immich 是一款免费的开源自托管照片和视频备份解决方案，可作为 Google Photos 等云服务的替代品。用户在自己的硬件上安装服务器，并通过网页或移动应用访问媒体，从而确保隐私和数据所有权。该项目在自托管社区中获得了显著关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://immich.app/">Immich</a></li>
<li><a href="https://grokipedia.com/page/Immich">Immich</a></li>

</ul>
</details>

**社区讨论**: 社区参与度很高，评论中既有庆祝学生贡献的，也有关于加密的辩论。一些用户认为不需要端到端加密，物理安全就足够了，而另一些用户则更喜欢像 Ente 这样提供内置加密的替代方案。总体情绪积极，用户称赞 Immich 的品质和价值。

**标签**: `#self-hosting`, `#photo management`, `#open source`, `#privacy`

---

<a id="item-10"></a>
## [Postgres 事务：分布式系统超能力](https://www.dbos.dev/blog/co-locating-workflow-state-with-your-data) ⭐️ 8.0/10

一篇博文提出利用 Postgres 事务来管理工作流状态，将状态与数据放在同一数据库中，从而简化分布式协调。 这种方法消除了对消息队列或两阶段提交等独立协调机制的需求，但将数据库与工作流逻辑紧密耦合，使得后续架构分离更加困难。 每个工作流步骤成为一个独立的数据库提交单元，简化了发件箱模式；但数据库与工作流紧密耦合，后续可能难以分离。

hackernews · KraftyOne · 7月2日 18:38 · [社区讨论](https://news.ycombinator.com/item?id=48765639)

**背景**: 分布式工作流通常需要协调多个服务，传统上使用消息队列或 Saga 模式。Postgres 事务提供原子性和一致性，使工作流进度与数据库提交对齐，从而将数据库用作协调点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48765639">Postgres transactions are a distributed systems superpower ...</a></li>

</ul>
</details>

**社区讨论**: 评论观点不一：有人欣赏其原子性和简洁性（Crowberry），而另一些人质疑它是否真正分布式（cloudie78），并指出紧密耦合问题（jdw64）。mrkeen 回忆了一次面试经历，他认为无法原子性地同时更新数据库和消息队列。

**标签**: `#Postgres`, `#distributed systems`, `#transactions`, `#workflow`, `#database architecture`

---

<a id="item-11"></a>
## [Meta 拥抱面向 AI 计算的 Neocloud 模式](https://newsletter.semianalysis.com/p/meta-compute-everyone-wants-to-be) ⭐️ 8.0/10

此举标志着大型科技公司构建类似 neocloud 的专用 AI 基础设施的重要趋势，可能颠覆传统超大规模云服务商的主导地位，并重新定义 AI 工作负载的经济性。 该分析提到即将推出的“ClusterMAX 排名”，这是一个对 GPU 云提供商的性能、网络和定价进行评分的系统，并提及将推荐系统扩展 10 倍。

rss · Semianalysis · 7月2日 22:18

**背景**: Neocloud 是专门针对 AI 工作负载的云服务商，提供高性能 GPU 集群、透明定价且无需长期合同，不同于 AWS 或 Azure 等传统超大规模云服务商。Meta 的转变反映了更广泛的行业趋势，SpaceX 和 Bedrock 等公司也采用了类似的定制基础设施策略。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.mckinsey.com/capabilities/tech-and-ai/our-insights/the-evolution-of-neoclouds-and-their-next-moves">Neoclouds’ challenges and next moves | McKinsey</a></li>
<li><a href="https://www.cisco.com/site/us/en/learn/topics/computing/what-is-neocloud.html">What is neocloud? - Cisco</a></li>
<li><a href="https://newsletter.semianalysis.com/p/clustermax-20-the-industry-standard">ClusterMAX™ 2.0: The Industry Standard GPU Cloud Rating System</a></li>

</ul>
</details>

**标签**: `#Meta`, `#Cloud Computing`, `#AI Infrastructure`, `#Recommendation Systems`, `#Data Centers`

---

<a id="item-12"></a>
## [Google Gemini Omni Flash 登顶 Video Arena 排行榜](https://x.com/Designarena/status/2072759122366509130) ⭐️ 8.0/10

Google DeepMind 的视频生成模型 Gemini Omni Flash 以 1404 分在 Video Arena 盲测排行榜上登顶，领先字节跳动的 Seedance 2.0 Mini 达 101 分。 这标志着 AI 视频生成领域的重大变化，Google 超越了长期占据榜首的字节跳动 Seedance 系列，凸显了多模态生成式 AI 的激烈竞争。 Gemini Omni Flash 结合了 Gemini 的智能与生成式媒体模型，支持文本生成视频、图像生成视频以及对话式视频编辑。该模型还使 Google 的总体视频模型排名相比 Veo 系列提升了 7 位。

telegram · zaihuapd · 7月3日 05:51

**背景**: Video Arena 是一个众包盲测平台，用户通过比较匿名视频输出并进行投票，产生类似 Elo 的排名。字节跳动的 Seedance 2.0 Mini 是 Seedance 2 视频系列中的经济高效版本，能在大约两分钟内生成带有同步音频的视频片段。Google 之前的 Veo 系列排名较低。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://llm-stats.com/leaderboards/best-ai-for-video-generation">Best AI for Video Generation in 2026 — Ranked by Blind Human ...</a></li>
<li><a href="https://deepmind.google/models/model-cards/gemini-omni-flash/">Gemini Omni Flash - Model Card — Google DeepMind</a></li>
<li><a href="https://seedance2.ai/seedance-2-0-mini">Seedance 2.0 Mini - Lower-Cost Cinematic AI Video Generator ...</a></li>

</ul>
</details>

**标签**: `#AI video generation`, `#Google`, `#Gemini Omni Flash`, `#ByteDance`, `#Video Arena`

---

<a id="item-13"></a>
## [Anthropic 指控阿里巴巴发动大规模模型蒸馏攻击](https://t.me/zaihuapd/42327) ⭐️ 8.0/10

Anthropic 指控阿里巴巴通过约 2.5 万个欺诈账户，在 2026 年 4 月 22 日至 6 月 5 日期间与 Claude 进行了超过 2880 万次交互，发动了大规模“蒸馏攻击”以窃取其 AI 模型能力。 如果证实，这将是针对领先 AI 公司迄今已知最大规模的蒸馏攻击，引发对知识产权保护、AI 安全以及行业竞争情报的重大担忧。 Anthropic 明确点名阿里巴巴及其 AI 实验室 Qwen 参与其中，并向美国参议院银行委员会报告了此事。攻击利用公共 API 访问，反复查询 Claude 以提取其能力。

telegram · zaihuapd · 7月3日 06:21

**背景**: 模型蒸馏是一种让较小的“学生”模型学习模仿较大“教师”模型输出的技术，通常用于降低计算成本。蒸馏攻击则恶意利用这一原理，通过公共接口反复查询专有 AI 模型，未经授权窃取其知识。多家 AI 公司曾报告过针对中国实验室的此类攻击。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation - Wikipedia</a></li>
<li><a href="https://www.anthropic.com/news/detecting-and-preventing-distillation-attacks">Detecting and preventing distillation attacks \ Anthropic</a></li>
<li><a href="https://www.mindstudio.ai/blog/ai-model-distillation-attacks-explained">AI Model Distillation Attacks: What They Are and Why They ...</a></li>

</ul>
</details>

**标签**: `#AI Security`, `#Model Distillation`, `#Anthropic`, `#Alibaba`, `#Competitive Intelligence`

---

<a id="item-14"></a>
## [中国新规草案：账号休眠注销、AI 标识与个性化推荐关闭](https://mp.weixin.qq.com/s/TfYZaC8ULPvu9JeTqYGkKg) ⭐️ 8.0/10

国家网信办于 2026 年 7 月 3 日发布了《互联网信息服务管理办法（修订草案征求意见稿）》，提出平台可对超过 6 个月未登录的账号进行限制或注销，要求对 AI 生成内容进行标识，允许用户关闭个性化推荐，并禁止刷量、控评等行为。 该法规将对中国所有互联网平台产生重大影响，涉及用户账号管理、AI 内容透明度和算法推荐系统。这标志着中国在规范网络内容和保护用户权益方面又迈出了一步。 草案公开征求意见截止至 2026 年 8 月 2 日。要求大型平台在 24 小时内处理违法信息投诉，并禁止强制使用 AI 服务。AI 标识要求与 2025 年 9 月 1 日生效的《人工智能生成内容标识管理办法》一致。

telegram · zaihuapd · 7月3日 11:29

**背景**: 中国近年来通过《网络安全法》《个人信息保护法》等不断强化互联网监管。2025 年 9 月 1 日生效的《人工智能生成内容标识管理办法》要求对 AI 生成内容进行显式和隐式标识以防止虚假信息。本次草案将规则扩展到平台账号管理，并禁止刷量、控评等操纵社交媒体的行为。

<details><summary>参考链接</summary>
<ul>
<li><a href="http://english.scio.gov.cn/pressroom/2025-03/17/content_117769570.html">China requires labeling of AI-generated online content</a></li>
<li><a href="https://regulations.ai/regulations/RAI-CN-NA-CONTENT-2025">China AI-Generated Content Labeling Measures - Regulations.AI</a></li>
<li><a href="https://www.lexology.com/library/detail.aspx?g=3e0002f7-34f0-4df3-9879-b63a9350e085">The State Administration of Market Regulation Issues Typical ...</a></li>

</ul>
</details>

**标签**: `#internet regulation`, `#AI content labeling`, `#privacy`, `#China`, `#platform compliance`

---