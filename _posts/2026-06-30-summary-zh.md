---
layout: default
title: "Horizon Summary: 2026-06-30 (ZH)"
date: 2026-06-30
lang: zh
---

> 从 61 条内容中筛选出 13 条重要资讯。

---

1. [vLLM v0.24.0 发布：新增模型支持与重大优化](#item-1) ⭐️ 9.0/10
2. [最高法院要求地理围栏搜查需令状](#item-2) ⭐️ 9.0/10
3. [谷歌智能体 AI 审稿人处理 1 万篇论文](#item-3) ⭐️ 9.0/10
4. [长鑫存储与腾讯签近 30 亿美元 DRAM 供应协议](#item-4) ⭐️ 9.0/10
5. [火箭实验室收购铱星公司以保障发射基线和卫星制造](#item-5) ⭐️ 8.0/10
6. [WATaBoy：将 Game Boy 指令 JIT 编译到 WebAssembly，性能超越原生解释器](#item-6) ⭐️ 8.0/10
7. [CUDA 内核启动的幕后：门铃机制与 QMD](#item-7) ⭐️ 8.0/10
8. [欧洲 ISP 要求版权方对过度封锁承担责任](#item-8) ⭐️ 8.0/10
9. [Ornith-1.0：开源自脚手架 LLM 用于智能体编程](#item-9) ⭐️ 8.0/10
10. [Cerebras 与 OpenAI 交易导致初创企业推理容量被阻断](#item-10) ⭐️ 8.0/10
11. [EML 树被证明为通用近似器](#item-11) ⭐️ 8.0/10
12. [勒索软件集团泄露苹果印度供应商塔塔的 iPhone 18 Pro 数据](#item-12) ⭐️ 8.0/10
13. [三星与 SK 海力士公布大规模 AI 投资计划](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.24.0 发布：新增模型支持与重大优化](https://github.com/vllm-project/vllm/releases/tag/v0.24.0) ⭐️ 9.0/10

vLLM v0.24.0 正式发布，包含来自 256 位贡献者的 571 次提交。新版增加了对 MiniMax-M3 和 DiffusionGemma 模型的支持，并为 DeepSeek-V4 带来了重大优化，包括 FlashInfer 稀疏索引缓存和集群协同 topK 内核。 作为广泛使用的 LLM 推理引擎，此版本显著提升了 DeepSeek-V4 等大型 MoE 模型的性能，并扩展了模型支持，使高吞吐服务更加高效和易于使用。 值得注意的技术新增包括 MiniMax-M3 的 MXFP4 量化支持、可将首次令牌生成时间降低 2–4% 的 FlashInfer 稀疏索引缓存，以及统一各模型工具调用解析的新型流式解析器引擎。

github · khluu · 6月29日 19:41

**背景**: vLLM 是一个面向大型语言模型的高吞吐、内存高效的推理引擎，利用 PagedAttention 和连续批处理技术。MiniMax-M3 是一个新的稠密模型，而 DeepSeek-V4 是一个大型混合专家 (MoE) 模型，受益于 FlashInfer 等优化的内核库。MXFP4 是一种 4 位块浮点格式，可在最小精度损失下压缩模型权重。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/flashinfer-ai/flashinfer">GitHub - flashinfer-ai/flashinfer: FlashInfer: Kernel Library for LLM Serving · GitHub</a></li>
<li><a href="http://www.kapilsharma.dev/posts/mxfp4-visualizer/">Understanding MXFP4 Quantization | Kapil Sharma</a></li>
<li><a href="https://newreleases.io/project/github/vllm-project/vllm/release/v0.24.0">vllm-project/vllm v0.24.0 on GitHub - NewReleases.io</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#model serving`, `#AI infrastructure`

---

<a id="item-2"></a>
## [最高法院要求地理围栏搜查需令状](https://www.theguardian.com/us-news/2026/jun/29/supreme-court-geofence-warrants-case-decision) ⭐️ 9.0/10

美国最高法院裁定，地理围栏搜查令须受第四修正案保护，执法部门在获取特定区域内设备位置数据前，必须基于合理根据取得令状。 这项里程碑式裁决极大地限制了执法部门使用地理围栏搜查令，加强了数字隐私权，并影响存储位置数据的科技公司。 法院认为，政府在未取得令状的情况下获取某一地理区域的手机位置数据，构成第四修正案下的搜查，正如卡根大法官在意见书中引用 Riley v. California 案所述。

hackernews · cdrnsf · 6月29日 15:54 · [社区讨论](https://news.ycombinator.com/item?id=48720924)

**背景**: 地理围栏搜查令，又称反向位置令状，允许执法部门在特定时间段内搜索科技公司数据库中某一地理区域内的所有移动设备。此类令状已在调查中使用，但因范围广泛而引发隐私担忧，常波及无辜路人。第四修正案保护公民免受不合理搜查和扣押，要求令状具有特定性并基于合理根据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Geofence_warrant">Geofence warrant - Wikipedia</a></li>
<li><a href="https://www.nacdl.org/Content/Geofence-Warrants">NACDL - Geofence Warrants</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论了裁决的推理过程，有人指出法院援引事实来源并引用 Riley 案。另一人以 Paula Broadwell 案例说明位置数据可通过其他方式识别。还有人就 Flock 等产品是否现在需要令状展开争论。

**标签**: `#privacy`, `#supreme-court`, `#geofence-warrants`, `#fourth-amendment`, `#digital-rights`

---

<a id="item-3"></a>
## [谷歌智能体 AI 审稿人处理 1 万篇论文](https://www.reddit.com/r/MachineLearning/comments/1uio9rb/googles_agentic_peerreviewer_handled_10k_papers/) ⭐️ 9.0/10

谷歌在 ICML 和 STOC 会议上部署了一个智能体 AI 审稿系统，处理了约 1 万篇论文，每篇平均 30 分钟。正式研究论文显示，该系统比零样本提示多检测出 34%的数学错误。 这标志着 AI 辅助科学评审的一个重要里程碑，展示了大规模实际部署并取得了可衡量的改进。它可能加快同行评审过程，提高学术出版的质量控制。 该系统是智能体 AI，能够自主运行，具有目标驱动行为并适应任务。它平均在 30 分钟内处理完投稿，比零样本提示多检测出 34%的数学错误，该结果已记录在 arXiv 的正式论文中。

reddit · r/MachineLearning · /u/Justgototheeffinmoon · 6月29日 10:05

**背景**: 智能体 AI 指的是具有自主性、目标驱动行为和适应性的 AI 系统，不同于需要人工干预的传统模型。零样本提示是一种提示工程技术，模型在提示中没有任何示例的情况下执行任务，仅依赖其预训练。这则新闻将这两个概念结合起来，创建了一个在会议规模上运行的自动审稿人。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/agentic-ai">What is Agentic AI? | IBM</a></li>
<li><a href="https://www.promptingguide.ai/techniques/zeroshot">Zero-Shot Prompting | Prompt Engineering Guide</a></li>

</ul>
</details>

**标签**: `#AI`, `#peer review`, `#scientific publishing`, `#machine learning`, `#Google`

---

<a id="item-4"></a>
## [长鑫存储与腾讯签近 30 亿美元 DRAM 供应协议](https://www.reuters.com/world/china/chinas-cxmt-wins-3-billion-memory-supply-deal-with-tencent-sources-say-2026-06-29/) ⭐️ 9.0/10

据知情人士透露，长鑫存储（CXMT）已与腾讯签署一份长期 DRAM 供应协议，价值超过 200 亿元人民币（约 29.4 亿美元），涵盖数年内的服务器内存供应，协议期限为 3 至 5 年。 这笔交易标志着中国 DRAM 制造商长鑫存储在国内云和互联网市场取得重大突破，可能减少对三星、SK 海力士等外国内存供应商的依赖。同时，它也凸显了中国科技巨头在地缘政治紧张局势下加强供应链自主化的合作趋势。 据报，该交易价值约 30 亿美元，合同期限为 3 至 5 年不等。此外，长鑫存储据传还在与阿里云、字节跳动、小米等其他中国互联网公司进行类似供应协议的谈判。

telegram · zaihuapd · 6月29日 09:31

**背景**: DRAM（动态随机存取存储器）是一种广泛用于服务器、个人电脑和移动设备的半导体存储器。长鑫存储是中国领先的 DRAM 制造商之一，旨在与三星、SK 海力士、美光等全球巨头竞争。中国政府一直推动国内半导体生产，以减少对外国技术的依赖，尤其是在美国出口限制之后。

**标签**: `#semiconductors`, `#DRAM`, `#China`, `#Tencent`, `#supply chain`

---

<a id="item-5"></a>
## [火箭实验室收购铱星公司以保障发射基线和卫星制造](https://investors.rocketlabcorp.com/news-releases/news-release-details/rocket-lab-acquire-iridium-historic-deal-creating-fully) ⭐️ 8.0/10

火箭实验室宣布收购铱星通信公司，从而确保了稳定的发射基线，并将其卫星制造业务整合进来。 此举为火箭实验室提供了类似 SpaceX 星链的稳定发射需求，降低了规模化过程中的风险。同时，使火箭实验室成为一家完全整合的航天公司，可能重塑小型卫星发射市场。 此次收购包括铱星位于 780 公里近地轨道的卫星星座，Electron 火箭可以到达，以及下一代替换计划。火箭实验室即将推出的中子火箭将承担更大的载荷用于星座补充。

hackernews · everfrustrated · 6月29日 14:09 · [社区讨论](https://news.ycombinator.com/item?id=48719485)

**背景**: 火箭实验室是一家航空航天制造商和发射服务提供商，以其 Electron 火箭闻名，该火箭是全球最多产的小型运载火箭。铱星公司运营着由 66 颗卫星组成的近地轨道星座，用于全球通信。此次收购将发射和卫星制造整合到同一家公司旗下，这一模式由 SpaceX 首创。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Rocket_Lab">Rocket Lab - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Iridium_Communications">Iridium Communications - Wikipedia</a></li>
<li><a href="https://rocketlabcorp.com/about/about-us/">Rocket Lab | About Us | Rocket Lab</a></li>

</ul>
</details>

**社区讨论**: 一些评论者表达了对卫星数量增加导致太空垃圾的担忧，而另一些人则称赞这一战略举措，将其比作 SpaceX 利用星链保障发射的做法。少数人注意到火箭实验室的总部从新西兰迁至美国。

**标签**: `#space`, `#acquisition`, `#rocketlab`, `#iridium`, `#satellite`

---

<a id="item-6"></a>
## [WATaBoy：将 Game Boy 指令 JIT 编译到 WebAssembly，性能超越原生解释器](https://humphri.es/blog/WATaBoy/) ⭐️ 8.0/10

WATaBoy 是一款 Game Boy 模拟器，它在运行时将 SM83 CPU 指令动态重新编译为 WebAssembly（WASM），实现了比原生解释器更快的性能。 这种方法使得在限制原生 JIT 的平台（如 iOS）上实现 JIT 编译成为可能，有望在浏览器和移动应用中解锁高性能模拟，并展示了 WASM 作为 JIT 目标的可行性。 该模拟器针对 SM83（Game Boy 的类 Z80 CPU），利用 JavaScript 的 eval 类似机制（如 new Function()）在运行时生成优化的 WASM 代码。据报道，在此用例中 Firefox 比 Chrome/Safari 慢 25%。

hackernews · energeticbark · 6月29日 15:02 · [社区讨论](https://news.ycombinator.com/item?id=48720190)

**背景**: JIT（即时编译）在执行期间将代码转换为更快性能的机器码，但 iOS 禁止应用进行原生 JIT 编译。然而，Web 浏览器被允许对 JavaScript 和 WebAssembly 进行 JIT 编译。WATaBoy 利用了这一漏洞：通过编写一个输出 WASM 的 JIT，它借助浏览器已有的 WASM JIT 编译器，在遵守平台限制的同时获得速度提升。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://humphri.es/blog/WATaBoy/">WATaBoy: JIT-ing Game Boy Instructions to Wasm Beats a Native Interpreter</a></li>
<li><a href="https://github.com/torch2424/wasmboy">GitHub - torch2424/wasmboy: Game Boy / Game Boy Color Emulator Library, 🎮written for WebAssembly using AssemblyScript. 🚀Demos built with Preact and Svelte. ⚛️</a></li>
<li><a href="https://asktechnicians.com/the-browser-loophole-that-could-sneak-emulators-onto-iphone">JIT - to - Wasm : The Browser Loophole for iPhone Emulators · Ask...</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，使用 JavaScript 的 eval/new Function 是最简单的 JIT 方法，并有人讨论了 Apple 对浏览器 JIT 的例外使得 WATaBoy 在 iOS 上可行。还提到 WASM 开销（约 20%）远小于解释器开销（约 1000%），因此性能超越解释器在意料之中，但该项目作为本科生的作品仍然令人印象深刻。

**标签**: `#JIT compilation`, `#WebAssembly`, `#Game Boy emulation`, `#performance`, `#emulator`

---

<a id="item-7"></a>
## [CUDA 内核启动的幕后：门铃机制与 QMD](https://fergusfinn.com/blog/what-happens-when-you-run-a-gpu-kernel/) ⭐️ 8.0/10

一篇技术博客文章详细描述了 CUDA 内核从宿主代码到 GPU 执行的完整路径，解释了连接软件 API 调用与硬件提交的门铃机制和队列元数据描述符（QMD）。 这一解释填补了典型 CUDA 教程中的关键空白，帮助开发者理解 GPU 命令提交的开销，从而更明智地优化内核启动。 门铃是对内存映射寄存器的写入操作，用于通知 GPU 获取命令；而 QMD 是包含内核参数和指针的数据结构，由 GPU 的工作分发器读取。

hackernews · mezark · 6月29日 13:11 · [社区讨论](https://news.ycombinator.com/item?id=48718863)

**背景**: CUDA 是一个并行计算平台，允许开发者在 GPU 上运行代码。当内核启动时，CPU 驱动会构建命令缓冲区并写入门铃，触发 GPU 获取并执行命令。QMD 包含元数据，如网格维度、块大小和内核参数，GPU 利用这些信息在流多处理器上调度线程块。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2605.01352v1">VUDA: Breaking CUDA-Vulkan Isolation for Spatial Sharing of Compute and Graphics on the Same GPU</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞这篇文章澄清了 CPU 到 GPU 的路径，特别是门铃和 QMD 概念。有人指出 NVIDIA 提供了关于 QMD 格式的开放 GPU 文档，另有人欣赏 CUDA 语法与硬件提交之间的联系。还有人推测了内核优化工具的未来。

**标签**: `#CUDA`, `#GPU`, `#kernel execution`, `#HPC`, `#technical deep-dive`

---

<a id="item-8"></a>
## [欧洲 ISP 要求版权方对过度封锁承担责任](https://torrentfreak.com/european-isps-want-rightsholders-held-accountable-for-overblocking-damage/) ⭐️ 8.0/10

欧洲互联网服务提供商（ISP）要求，如果版权方过度执行版权封锁措施并导致合法内容受损，应当承担法律和财务责任。 这一诉求可能重塑在线版权执法的权力平衡，抑制版权方当前滥用广泛封锁令、干扰合法互联网流量的行为，同时不必承担任何后果。 这一诉求源于日益增长的不满情绪，尤其是在西班牙，法院应版权方要求在足球比赛期间实施的屏蔽措施频繁波及无关服务和合法用户。

hackernews · Brajeshwar · 6月29日 16:07 · [社区讨论](https://news.ycombinator.com/item?id=48721072)

**背景**: “过度封锁”指的是 ISP 因版权执法采用过于宽泛的过滤规则，无意中阻止了合法内容。目前，版权方通常无需为这种过度行为负责，ISP 和用户只能承担访问中断的损失。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://de.wikipedia.org/wiki/Overblocking">Overblocking – Wikipedia</a></li>
<li><a href="https://www.findlaw.com/smallbusiness/intellectual-property/isp-liability-for-the-acts-of-its-customers.html">ISP Liability for the Acts of Its Customers - FindLaw</a></li>

</ul>
</details>

**社区讨论**: 评论普遍支持 ISP 的立场，批评版权方在不经法院审查的情况下轻易实施内容审查，一些人提到西班牙的严重干扰现象，另一些人则将问题与关于网络审查和企业权力的更广泛辩论联系起来。

**标签**: `#internet governance`, `#copyright`, `#ISP liability`, `#censorship`, `#Spain`

---

<a id="item-9"></a>
## [Ornith-1.0：开源自脚手架 LLM 用于智能体编程](https://simonwillison.net/2026/Jun/29/ornith/#atom-everything) ⭐️ 8.0/10

DeepReinforce 发布了 Ornith-1.0，这是一个 MIT 许可的开源权重编码 LLM 系列，最大 397B 参数，基于 Gemma 4 和 Qwen 3.5 构建，在编码基准上实现了最先进性能。 这是 DeepReinforce 首次重大开源发布，展示了一种新的“自脚手架”训练范式，能够实现更自主的编码智能体，有望加速 AI 辅助软件开发。 该系列包括 9B 密集、31B 密集、35B MoE 和 397B MoE 变体；全部采用 MIT 许可，底层模型（Gemma 4 和 Qwen 3.5）采用 Apache 2.0 许可，确保兼容性。早期测试显示在多步工具调用和代码理解方面表现强劲。

rss · Simon Willison · 6月29日 16:17

**背景**: 自脚手架 LLM 是指在推理过程中自行生成推理或工具使用结构的模型，无需外部编排即可提高复杂任务的性能。智能体编程指的是自主执行多步软件开发任务的 AI 智能体。GGUF 格式允许通过 LM Studio 等工具进行高效本地推理，使这些模型对个人开发者可及。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/29/ornith/">Ornith-1.0: Self - Scaffolding LLMs for Agentic Coding</a></li>
<li><a href="https://deep-reinforce.com/ornith_1_0.html">Ornith-1.0: Self - Scaffolding LLMs ... | DeepReinforce Blog | Jun. 2026</a></li>
<li><a href="https://en.wikipedia.org/wiki/Agentic_coding">Agentic coding</a></li>

</ul>
</details>

**标签**: `#LLM`, `#open-source`, `#coding`, `#AI`, `#deep learning`

---

<a id="item-10"></a>
## [Cerebras 与 OpenAI 交易导致初创企业推理容量被阻断](https://www.reddit.com/r/MachineLearning/comments/1uiqhiv/cerebras_openai_deal_capacity_has_effectively/) ⭐️ 8.0/10

Cerebras 通过与 OpenAI 的数十亿美元交易，将其近期大部分推理容量分配给 OpenAI，实际上使其他初创企业的 API 等待名单变得无限期。 这种将计算资源集中到单一客户的做法威胁到小型 AI 初创企业和研究人员访问快速、基于 ASIC 的推理能力，可能抑制创新并巩固市场力量。 Cerebras 的晶圆级引擎（WSE）是一种专为高吞吐量 AI 工作负载设计的大型 ASIC，但生产能力似乎有限。发帖人需要约 1-2k tokens/秒的推理速度和低 p95 延迟，而 GPU 难以满足。

reddit · r/MachineLearning · /u/Kortopi-98 · 6月29日 12:00

**背景**: Cerebras 生产晶圆级引擎，这是世界上最大的 AI 处理器，面向训练和推理。推理 ASIC 为实时应用提供专门性能，但制造如此大的芯片复杂且容量受限。P95 延迟测量第 95 百分位的响应时间；对于实时编程代理，低 p95 延迟对响应能力至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cerebras">Cerebras - Wikipedia</a></li>
<li><a href="https://www.cerebras.ai/chip">Product - Chip - Cerebras</a></li>
<li><a href="https://redis.io/blog/p95-latency/">P95 Latency: What It Is & Why It Matters - Redis</a></li>

</ul>
</details>

**社区讨论**: Reddit 帖子表达了一位初创公司创始人因 Cerebras-OpenAI 交易需求未得到满足的强烈不满。评论（未在片段中提供）可能呼应了对资源垄断和小企业障碍的担忧。

**标签**: `#Cerebras`, `#OpenAI`, `#inference`, `#compute capacity`, `#AI startup`

---

<a id="item-11"></a>
## [EML 树被证明为通用近似器](https://www.reddit.com/r/MachineLearning/comments/1uipl1t/eml_trees_are_universal_approximators_r/) ⭐️ 8.0/10

作者通过构造多项式和双曲正切等函数的显式 EML 表示，证明了 EML 树是通用近似器，这些表示可作为逼近 Sobolev 空间中任意函数的构建模块。 这一结果扩展了已知通用近似器的模型类别，可能在符号回归和科学计算中带来新应用，因为 EML 树提供可解释且紧凑的表示。 证明采用“乐高积木”方法，构造二元运算和初等函数的 EML 表示，并通过符号分解和仿射映射处理对数定义域问题。论文通过添加可学习参数推广了原始 EML。

reddit · r/MachineLearning · /u/JoeGermany · 6月29日 11:16

**背景**: 通用逼近定理指出，某些模型（如神经网络）可以任意精度逼近任何连续函数。最近引入的 EML（初等数学库）函数通过组合能表示所有初等函数。本文证明树状结构的 EML 函数组合对 Sobolev 空间也具有通用逼近性质。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Universal_approximation_theorem">Universal approximation theorem - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2606.23179">[2606.23179] EML Trees Are Universal Approximators - arXiv.org</a></li>
<li><a href="https://arxiv.org/html/2606.23179v1">EML Trees Are Universal Approximators - arXiv.org</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#universal approximation`, `#theory`, `#EML trees`, `#function approximation`

---

<a id="item-12"></a>
## [勒索软件集团泄露苹果印度供应商塔塔的 iPhone 18 Pro 数据](https://t.me/FinanceNewsDaily/489740) ⭐️ 8.0/10

一个从塔塔电子窃取数据的勒索软件组织已在暗网发布即将推出的 iPhone 18 Pro 照片及敏感供应商信息。 此次泄露暴露了苹果严格控制供应链和未发布产品细节，可能影响苹果的安全声誉和供应商信任。 泄露文件不仅包含产品图片，还包括敏感零部件和供应商名单。塔塔既是零部件供应商，也是 iPhone 组装商。

telegram · FinanceNewsDaily · 6月29日 19:45

**背景**: 暗网是深网的一部分，无法被普通搜索引擎索引，常被用于数据泄露等非法活动。勒索软件是一种加密受害者数据并索要赎金以解锁的恶意软件，网络犯罪分子经常用它来攻击企业。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bbc.com/zhongwen/simp/world-69313893">Telegram... - BBC News 中文</a></li>
<li><a href="https://www.wangan.com/p/7fyg88b9e7ec1092">Akamai...</a></li>

</ul>
</details>

**标签**: `#supply chain`, `#security breach`, `#Apple`, `#iPhone`, `#ransomware`

---

<a id="item-13"></a>
## [三星与 SK 海力士公布大规模 AI 投资计划](https://t.me/zaihuapd/42235) ⭐️ 8.0/10

三星宣布了史上最大规模的 1000 万亿韩元（约 6480 亿美元）十年 AI 支出计划，SK 海力士则计划五年内将产能翻倍，并通过美国 IPO 筹资 290 亿美元。 这些投资标志着向 AI 驱动基础设施的关键转变，可能重塑全球半导体供应链并增强韩国的经济竞争力。 该公告计划于 6 月 29 日的国家简报会上发布，重点关注半导体、AI 数据中心和 Physical AI。同日，三星和 SK 海力士股价因苹果相关负面消息下跌超过 9%。

telegram · zaihuapd · 6月29日 07:00

**背景**: Physical AI 是 NVIDIA 定义的术语，指使机器人、自动驾驶汽车等自主系统能够在物理世界中感知、推理和行动的 AI 技术。此次投资热潮反映了全球为构建此类技术（包括 AI 数据中心和机器人）的硬件基础设施而展开的竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/glossary/generative-physical-ai/">What is Physical AI? | NVIDIA Glossary</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#AI investment`, `#Samsung`, `#SK Hynix`

---