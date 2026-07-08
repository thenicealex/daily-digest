---
layout: default
title: "Horizon Summary: 2026-07-08 (ZH)"
date: 2026-07-08
lang: zh
---

> 从 59 条内容中筛选出 14 条重要资讯。

---

1. [OpenAI 发布 GPT-Live 语音模式，支持长达一小时的对话](#item-1) ⭐️ 9.0/10
2. [TypeScript 7.0 发布，速度提升高达 11.9 倍](#item-2) ⭐️ 9.0/10
3. [智能体安全防线在工具调用攻击下失效](#item-3) ⭐️ 9.0/10
4. [通过 Firefox 和内核漏洞披露的安卓远程 Root 漏洞链](#item-4) ⭐️ 9.0/10
5. [Grok 4.5 发布：竞争性定价与推理改进](#item-5) ⭐️ 8.0/10
6. [Mistral 发布 Robostral Navigate：无地图导航模型](#item-6) ⭐️ 8.0/10
7. [OpenBSD 释放后使用漏洞可本地提权至 root](#item-7) ⭐️ 8.0/10
8. [欧盟推进强制扫描私人信息的立法](#item-8) ⭐️ 8.0/10
9. [Cloudflare Meerkat：无领导者的全球共识算法](#item-9) ⭐️ 8.0/10
10. [Fable 模型安全分类器过于严格，阻碍合法使用](#item-10) ⭐️ 8.0/10
11. [SigLIP 在细粒度汽车分类的 k-NN 任务中大幅超越 DINOv2](#item-11) ⭐️ 8.0/10
12. [LingBot-Video：开源 13B 稀疏专家混合视频扩散世界模型](#item-12) ⭐️ 8.0/10
13. [DeepSeek 自研 AI 芯片以减少对英伟达和华为的依赖](#item-13) ⭐️ 8.0/10
14. [通过泄漏电磁信号识别手机应用，准确率达 99%](#item-14) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI 发布 GPT-Live 语音模式，支持长达一小时的对话](https://openai.com/index/introducing-gpt-live/) ⭐️ 9.0/10

OpenAI 推出了 GPT-Live，这是一种新的 ChatGPT 语音模式，支持长达一小时的自然对话，并能在后台将复杂任务委托给 GPT-5.5。 这标志着对话式 AI 的重大飞跃，超越了简短、简单的语音交互，转向持续、高效的对话，并弥合了语音模型与前沿文本模型之间的差距。 GPT-Live 允许用户进行长达一小时的对话，并可将问题委托给更先进的 GPT-5.5 模型进行深度推理。有用户报告了一个错误，它会在不适当的时刻打断并发出笑声。

hackernews · logickkk1 · 7月8日 17:03 · [社区讨论](https://news.ycombinator.com/item?id=48834405)

**背景**: GPT-Live 是 OpenAI 推出的新语音模式，为 ChatGPT 语音提供支持，旨在实现更自然的人机交互。GPT-5.5 于 2026 年 4 月发布，是一款大型语言模型，擅长编程、研究和分析，可在后台处理复杂查询。以往的语音模式仅限于较简单的模型，而 GPT-Live 打破了这一限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/introducing-gpt-live/">Introducing GPT-Live | OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.5">GPT-5.5</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：有人称赞改进和更长的对话（simonw），也有人担心取代人际关系（jonstaab, overgard）。artdigital 指出语音模式缺乏工具集成，同时有用户报告了打断对话的错误。

**标签**: `#AI`, `#OpenAI`, `#voice assistant`, `#GPT-5.5`, `#conversational AI`

---

<a id="item-2"></a>
## [TypeScript 7.0 发布，速度提升高达 11.9 倍](https://devblogs.microsoft.com/typescript/announcing-typescript-7-0/) ⭐️ 9.0/10

微软发布了 TypeScript 7.0，这是一个重大版本，在 VS Code 等大型代码库上实现了高达 11.9 倍的编译速度提升，内部基准测试显示加速范围从 7.7 倍到 11.9 倍。 此版本大幅减少了大型 TypeScript 项目的构建时间，提高了开发者的生产力，解决了社区长期以来的痛点，同时进一步巩固了 TypeScript 作为领先的类型化 JavaScript 超集地位。 速度改进在包括 VS Code（125.7 秒降至 10.6 秒）、Sentry（139.8 秒降至 15.7 秒）和 Playwright（12.8 秒降至 1.47 秒）等代码库上进行了测量。但社区反馈表明，TypeScript 7 可能无法与 ts-jest 等常用工具直接兼容，需要采用变通方案。

hackernews · DanRosenwasser · 7月8日 16:06 · [社区讨论](https://news.ycombinator.com/item?id=48833715)

**背景**: TypeScript 是由微软开发的一种类型化的 JavaScript 超集，编译为纯 JavaScript，提供静态类型检查和现代语言特性。大型代码库通常存在编译时间过长的问题，这已成为优化的主要方向。版本 6 是之前的稳定版本，而版本 7 引入了新的架构或优化，实现了显著的加速。

**社区讨论**: 社区对性能改进表示赞扬，有评论特别提到 VS Code 上 11.9 倍的加速并祝贺团队。但同时也有对与 ts-jest 兼容性以及混合环境下 tsconfig 作用域复杂性的担忧，此外还有人对未来可能用 Rust 重写表示期待。

**标签**: `#TypeScript`, `#performance`, `#programming languages`, `#Microsoft`

---

<a id="item-3"></a>
## [智能体安全防线在工具调用攻击下失效](https://www.reddit.com/r/MachineLearning/comments/1ur1fnz/agentic_safety_triggers_arent_textual_safety/) ⭐️ 9.0/10

一项新研究表明，当前针对大语言模型智能体的安全护栏在面对将攻击嵌入工具调用序列（例如通过模型上下文协议 MCP）而非文本提示的攻击时失效，诸如 DPO 和 SafeDPO 等最先进的安全微调方法仅能拒绝最多 48%的攻击。 这一发现挑战了安全对齐仅依赖文本触发检测的假设，因为具备真实工具访问权限的智能体引入了新的攻击面。它标志着 AI 安全研究和开发需要范式转变。 攻击利用已知的 CVE 漏洞，将利用步骤重写为看似普通的请求，最终导向恶意的工具调用序列。无需训练的方法在不进行任何微调的情况下达到了约 3 倍基线的拒绝率。

reddit · r/MachineLearning · /u/mlsandwich · 7月8日 18:36

**背景**: 模型上下文协议（MCP）是 Anthropic 提出的开放标准，用于规范 AI 模型与外部工具和数据源的集成。直接偏好优化（DPO）和 SafeDPO 是常见的对齐方法，通过人类偏好微调模型以拒绝有害输出。这项研究表明这些基于文本的对齐方法不足以应对涉及工具使用的智能体任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol</a></li>
<li><a href="https://en.wikipedia.org/wiki/Direct_preference_optimization">Direct preference optimization</a></li>
<li><a href="https://arxiv.org/abs/2505.20065">[2505.20065] SafeDPO: A Simple Approach to Direct Preference Optimization with Enhanced Safety</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#LLM agents`, `#adversarial attacks`, `#tool use`, `#MCP`

---

<a id="item-4"></a>
## [通过 Firefox 和内核漏洞披露的安卓远程 Root 漏洞链](https://www.coolapk.com/feed/72700258?s=ZGQ2MTVlZjYxMDYyNTM3ZzZhNGUzOThjega1640) ⭐️ 9.0/10

安全公司 Nebula 披露了一个影响 Android 17 及所有更早版本的远程 Root 漏洞链，该链结合了 Firefox 浏览器漏洞（Firefox 151.0.2 及更早版本）和一个 15 年前的 Linux 内核漏洞。概念验证代码已在 GitHub 上发布。 该漏洞利用链允许攻击者仅通过诱使用户点击恶意链接即可获得持久 Root 权限，影响数百万台设备。概念验证代码的公开增加了在补丁部署前被大规模利用的风险。 该漏洞链利用 Firefox 151.0.2 及更早版本中的内存安全漏洞实现初始代码执行，然后利用一个古老的 Linux 内核漏洞提权至 Root。Google Pixel 设备已实测可被攻破，整个 Android 17 设备可在 1 分钟内被 Root。

telegram · zaihuapd · 7月8日 13:01

**背景**: 远程 Root 漏洞链结合多个漏洞，无需物理接触即可获得设备的完全系统控制。Firefox 漏洞是一个在 151 版本中修复的内存安全缺陷，而内核漏洞已存在 15 年，最近被内核维护者修补。概念验证代码展示了攻击过程并帮助厂商开发修复，但也可能被恶意行为者利用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.mozilla.org/en-US/security/known-vulnerabilities/firefox/">Security Advisories for Firefox — Mozilla</a></li>
<li><a href="https://github.com/secmob/TiYunZong-An-Exploit-Chain-to-Remotely-Root-Modern-Android-Devices">GitHub - secmob/TiYunZong-An-Exploit-Chain-to-Remotely-Root-Modern-Android-Devices</a></li>
<li><a href="https://www.mozilla.org/en-US/security/advisories/mfsa2026-46/">Security Vulnerabilities fixed in Firefox 151 — Mozilla</a></li>

</ul>
</details>

**标签**: `#Android`, `#vulnerability`, `#remote root`, `#Linux kernel`, `#cybersecurity`

---

<a id="item-5"></a>
## [Grok 4.5 发布：竞争性定价与推理改进](https://x.ai/news/grok-4-5) ⭐️ 8.0/10

xAI 发布了 Grok 4.5，声称改进了推理效率，定价为每百万 tokens $2/$6，并使用了数万亿 tokens 的 Cursor 数据进行训练。 此次发布在成本上挑战其他 AI 模型，同时利用来自 Cursor 的独特真实世界编码数据，可能影响开发者工具和智能体交互。然而，信任问题可能限制企业采用。 Grok 4.5 定价为每百万 tokens $2/$6，推理效率比 Opus 高 4 倍，基准测试表明其性能达到 Opus 4.7 水平。该模型使用捕捉真实世界开发者-智能体交互的 Cursor 数据进行训练。

hackernews · BoumTAC · 7月8日 18:00 · [社区讨论](https://news.ycombinator.com/item?id=48835111)

**背景**: Grok 是 xAI（Elon Musk 的 AI 公司）开发的大型语言模型。该模型使用了 AI 代码编辑器 Cursor 的数据，这些数据提供了真实的编码交互，旨在提升模型对开发者工作流的理解。

**社区讨论**: 许多评论者表达了不信任，提及政治偏见和伦理问题，如 xAI 被认为对 CSAM（儿童性虐待材料）的容忍。部分人认可模型的成本效益和性能，但质疑大规模 AI 投入的经济合理性。

**标签**: `#AI`, `#Grok`, `#xAI`, `#Model Release`, `#Benchmark`

---

<a id="item-6"></a>
## [Mistral 发布 Robostral Navigate：无地图导航模型](https://mistral.ai/news/robostral-navigate/) ⭐️ 8.0/10

Mistral AI 发布了 Robostral Navigate，这是一个 80 亿参数的机器人导航模型，通过单个 RGB 摄像头实现无地图导航，且完全在模拟环境中训练而成。 该模型推动了具身 AI 的发展，使机器人无需预先构建地图即可在未知环境中导航，从而降低了工业自动化和爱好者机器人的部署时间和成本。 Robostral Navigate 在 R2R-CE 基准测试上达到了最先进水平，并结合了基于指向的导航与强化学习以实现持续改进。该模型目前未公开开放，但 Mistral 可能通过合作提供访问权限。

hackernews · ottomengis · 7月8日 14:09 · [社区讨论](https://news.ycombinator.com/item?id=48832212)

**背景**: 传统的机器人导航依赖于预先构建的环境地图，地图需要提前创建并在环境变化时更新。无地图导航则利用传感器数据（如摄像头图像）和学习策略在陌生空间中移动。模拟训练使模型能够在没有物理硬件风险的情况下学习鲁棒的行为。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mistral.ai/news/robostral-navigate/">Robostral Navigate: single-camera AI navigation | Mistral AI</a></li>
<li><a href="https://cryptobriefing.com/mistral-robostral-navigate-robotics-model/">Mistral AI unveils Robostral Navigate, an 8B robotics model that could reshape industrial automation investing</a></li>
<li><a href="https://x.com/MistralAI/status/2074856309438980145">Mistral AI on X: "Announcing Robostral Navigate, our first model for embodied navigation: an 8B robotics navigation model that guides robots to autonomously perform tasks specified with natural language. Single RGB camera. State-of-the-art on R2R-CE. https://t.co/UlmUsXNxhX" / X</a></li>

</ul>
</details>

**社区讨论**: Hacker News 社区对无地图导航表示兴奋，用户指出其在农场机器人等爱好者项目中的潜力。一些人强调室内无地图导航是比室外更新的挑战，并与斯坦福大学的 PIGEON 模型进行了比较。其他人则对模型未开放访问感到遗憾，希望未来能发布。

**标签**: `#robotics`, `#navigation`, `#AI`, `#Mistral`, `#deep learning`

---

<a id="item-7"></a>
## [OpenBSD 释放后使用漏洞可本地提权至 root](https://nvd.nist.gov/vuln/detail/cve-2026-57589) ⭐️ 8.0/10

OpenBSD 中发现了一个释放后使用漏洞（CVE-2026-57589），本地攻击者可利用该漏洞将权限提升至 root。此漏洞由 Trail of Bits 在 OpenAI 的“Patch The Planet”项目中通过 AI 模型发现。 该发现具有重要意义，因为 OpenBSD 被广泛认为是最注重安全的操作系统之一。同时，它也凸显了 AI 辅助漏洞挖掘在提升开源软件安全性方面日益重要的作用。 该漏洞是一个释放后使用问题，可被利用进行本地提权至 root。该发现是“Patch The Planet”项目的一部分，该项目为安全公司提供 AI 模型访问权限以进行漏洞研究。

hackernews · linggen · 7月8日 13:24 · [社区讨论](https://news.ycombinator.com/item?id=48831658)

**背景**: OpenBSD 是一个专注于安全的自由类 Unix 操作系统，具有主动安全措施和集成密码学。释放后使用漏洞是指程序在指向的内存被释放后仍继续使用该指针，常导致崩溃或任意代码执行。本地提权意味着拥有有限权限的攻击者可以获得完整的 root 控制权。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenBSD">OpenBSD</a></li>

</ul>
</details>

**社区讨论**: 社区成员指出该发现是 Patch The Planet 项目的一部分，一些人称赞 OpenBSD 的安全文化。其他人则质疑为什么该漏洞尚未出现在 OpenBSD 的安全页面上，并对随着 AI 辅助漏洞挖掘的扩展可能发现多少漏洞表示好奇。

**标签**: `#OpenBSD`, `#security`, `#vulnerability`, `#privilege escalation`, `#use-after-free`

---

<a id="item-8"></a>
## [欧盟推进强制扫描私人信息的立法](https://cyberinsider.com/eu-now-one-step-away-from-reviving-private-message-scanning-rules/) ⭐️ 8.0/10

欧洲议会投票决定快速恢复“聊天控制 1.0”，允许 Meta 等提供商自愿扫描私人信息；同时，关于强制扫描的“聊天控制 2.0”有约束力的投票定于 2025 年 7 月 9 日举行。 该立法威胁端到端加密和用户隐私，可能迫使消息平台扫描所有私人通信以查找儿童性虐待材料，这可能会为全球监控树立先例。 “聊天控制 1.0”允许自愿扫描，而“聊天控制 2.0”强制扫描并禁止端到端加密；在即将到来的投票中，需要 361 名欧洲议会议员的绝对多数才能阻止后者。

hackernews · ggirelli · 7月8日 16:53 · [社区讨论](https://news.ycombinator.com/item?id=48834296)

**背景**: “聊天控制”是一项拟议的欧盟法规，旨在通过扫描消息来打击儿童性虐待，但批评者认为它破坏了加密和隐私。该立法分为两个版本：“聊天控制 1.0”允许在电子隐私减损条款下进行自愿扫描，而“聊天控制 2.0”强制扫描并实际上禁止端到端加密。由大型科技公司资助的互联网观察基金会支持客户端扫描。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control">Chat Control - Wikipedia</a></li>
<li><a href="https://fightchatcontrol.eu/">Fight Chat Control - Protect Digital Privacy in the EU</a></li>
<li><a href="https://www.patrick-breyer.de/en/posts/chat-control/">Chat Control: The EU's CSAM scanner proposal</a></li>

</ul>
</details>

**社区讨论**: 评论表达了怀疑态度，一位用户指出互联网观察基金会正在推动客户端扫描。另一位澄清说“聊天控制 1.0”不如“聊天控制 2.0”令人担忧，后者强制扫描并禁止加密。一些人将其视为“终结者立法”，会不断卷土重来。

**标签**: `#privacy`, `#EU legislation`, `#encryption`, `#surveillance`

---

<a id="item-9"></a>
## [Cloudflare Meerkat：无领导者的全球共识算法](https://blog.cloudflare.com/meerkat-introduction/) ⭐️ 8.0/10

Cloudflare 宣布了 Meerkat，一个基于异步共识（QuePaxa）的无领导者全球分布式共识算法。这标志着异步共识协议的首次生产实现，该协议不依赖超时机制。 Meerkat 的无领导者设计消除了基于领导者的协议（如 Raft）中常见的领导者抖动和选举风暴问题，提高了在变化网络条件下的韧性。它使 Cloudflare 能够在其全球边缘网络上保持强一致性，且没有单点故障。 与依赖超时的部分同步协议（如 Paxos 或 Raft）不同，QuePaxa（Meerkat 的核心）即使在消息延迟剧烈波动时也能推进。但每次读取操作都需要全局共识，相比使用本地读取的系统可能会引入更高延迟。

hackernews · bobnamob · 7月8日 13:18 · [社区讨论](https://news.ycombinator.com/item?id=48831565)

**背景**: 分布式共识算法允许多个节点在出现故障时对一个值达成一致。传统协议如 Paxos 和 Raft 是部分同步的：它们假设消息延迟有界，并使用超时检测故障，这在不稳定的网络上可能引发问题。异步共识消除了这些时间假设，保证无论网络延迟如何都能推进，但历史上被认为成本过高而不实用。Meerkat 旨在使其在全局规模上变得实用。

**社区讨论**: 社区认同了生产环境中异步共识实现的创新性，但一些人质疑其权衡：读取操作需要共识限制了用例，且与无领导者的 Paxos 类算法比较比与 Raft 比较更合适。其他人指出，对于不稳定的网络，Meerkat 的方法可能有益，尽管它尚未投入生产。

**标签**: `#distributed consensus`, `#cloudflare`, `#leaderless`, `#asynchronous`, `#systems research`

---

<a id="item-10"></a>
## [Fable 模型安全分类器过于严格，阻碍合法使用](https://combine-lab.github.io/blog/2026/07/07/fable-is-not-a-useful-model.html) ⭐️ 8.0/10

一篇博文和社区讨论揭示，Anthropic 的 Fable 模型由于过于敏感的安全分类器，频繁错误地将合法用户请求降级到功能较弱的 Opus 4.8 模型。 该问题削弱了 Fable 在诸多合法任务中的可用性，尤其是在科学和技术领域，并引发了对 AI 系统安全性与功能性之间权衡的担忧。 该分类器旨在降级涉及网络安全、生物学或越狱尝试的请求，但它对良性查询也触发，例如临床试验的统计分析或 GPU 的代码优化。

hackernews · karrot-kake · 7月8日 20:41 · [社区讨论](https://news.ycombinator.com/item?id=48837162)

**背景**: Anthropic 的 Fable 是一个强大的 AI 模型，基于其宪法 AI 方法构建，其中包括防止滥用的安全分类器。然而，分类器的高误报率导致它将许多无害请求路由到功能较弱的 Opus 4.8 模型，使有合法需求的用户感到沮丧。

**社区讨论**: 评论者分享了众多例子，包括一位医学物理学家无法获得任何工作相关问题的回答，以及一位开发者请求修补 vLLM 时被不断降级。他们表达了沮丧，并指出这种过度过滤使得该模型对严肃工作几乎毫无用处。

**标签**: `#Anthropic`, `#Fable`, `#safety classifiers`, `#AI usability`, `#model limitations`

---

<a id="item-11"></a>
## [SigLIP 在细粒度汽车分类的 k-NN 任务中大幅超越 DINOv2](https://www.reddit.com/r/MachineLearning/comments/1uqtamz/dinov2_way_worse_than_siglip_in_knn_is_this/) ⭐️ 8.0/10

一位用户报告称，在细粒度汽车分类数据集上，SigLIP2 SO400M 使用加权 k-NN 达到了约 92% 的准确率，而 DINOv2 Giant 仅约为 41%，尽管两个模型规模相近且编码器都保持冻结。 这一巨大的性能差距挑战了假设认为像 DINOv2 这样的最先进自监督视觉模型普遍适用于检索任务，凸显了对比性预训练目标对于基于 k-NN 的细粒度分类的重要性。 用户使用了 L2 归一化的嵌入向量，并尝试了余弦距离和欧氏距离，结果没有变化。他们指出 DINOv2 是自监督的，可能需要训练一个线性探针才能表现良好，而 SigLIP 的对比训练自然形成了适用于相似度搜索的嵌入空间。

reddit · r/MachineLearning · /u/psy_com · 7月8日 13:51

**背景**: 自监督学习（SSL）方法如 DINOv2 在没有显式标签的情况下学习视觉表示，专注于语义特征，而对比方法如 SigLIP 则明确地将相似的图像-文本对在嵌入空间中拉近。k-NN 分类利用嵌入空间中的最近邻来对图像进行分类，因此那些为相似度结构化的嵌入的模型自然表现更好。细粒度汽车分类需要区分非常相似的车型如大众高尔夫各代之间的细微差别。

**标签**: `#DINOv2`, `#SigLIP`, `#k-NN`, `#fine-grained classification`, `#self-supervised learning`

---

<a id="item-12"></a>
## [LingBot-Video：开源 13B 稀疏专家混合视频扩散世界模型](https://www.reddit.com/r/MachineLearning/comments/1ur0bxq/lingbotvideo_sparsemoe_video_diffusion/) ⭐️ 8.0/10

该模型通过结合高效的稀疏专家混合架构与基于强化学习的物理合理性奖励，推动了开源视频生成的发展，向机器人实际世界模型迈进。它的发布引发了社区对视频生成器与动作条件世界模型边界的讨论。 该模型采用 DeepSeek-V3 风格的稀疏专家混合架构，包含 128 个专家和 top-8 路由，并使用包括 VLM 评分的物理合理性损失在内的六项奖励进行后训练。它具备动作到视频模式，可根据动作和手部姿态输入预测机器人展开帧。

reddit · r/MachineLearning · /u/Savings-Display5123 · 7月8日 17:58

**背景**: 视频扩散模型通过迭代去噪从噪声中生成时间连贯的视频帧。稀疏专家混合架构每次只激活部分参数，从而以更低计算成本实现更大模型容量。机器人世界模型旨在从动作模拟未来状态，连接生成视频与具身人工智能。

**社区讨论**: 社区提出了两个主要担忧：（1）由 VLM 从采样帧判断物理合理性是否可靠，是否容易受到古德哈特定律的影响；（2）该模型仅输出视频质量帧而没有闭环机器人实验，是否真正作为世界模型。作者承认了这些观点，并邀请进一步批评。

**标签**: `#video diffusion`, `#world model`, `#sparse MoE`, `#reinforcement learning`, `#open-source`

---

<a id="item-13"></a>
## [DeepSeek 自研 AI 芯片以减少对英伟达和华为的依赖](https://t.me/zaihuapd/42423) ⭐️ 8.0/10

中国 AI 公司 DeepSeek 正在开发自己的 AI 芯片，专注于推理阶段，以减少对英伟达和华为芯片的依赖。该项目始于大约一年前，目前仍处于早期阶段，公司正在招募芯片设计工程师。 此举可降低 DeepSeek 因依赖外国芯片供应商而面临的美国出口管制和地缘政治风险。如果成功，还有望降低成本并为其特定 AI 工作负载实现定制优化。 该芯片专为推理阶段（即已训练模型生成回答的环节）设计，而非训练阶段。DeepSeek 已与芯片设计、代工和存储公司接洽，并在近几个月私下招募芯片设计工程师。

telegram · zaihuapd · 7月8日 05:20

**背景**: DeepSeek 是一家中国 AI 初创公司，以其大型语言模型闻名，此前依赖英伟达 H800 和华为昇腾芯片。美国的出口管制限制了中国获取先进 AI 芯片的渠道，促使国内公司自主开发硬件。推理芯片通常比训练芯片复杂度低，但对 AI 部署仍然至关重要。

**标签**: `#AI chips`, `#DeepSeek`, `#hardware`, `#inference`, `#semiconductors`

---

<a id="item-14"></a>
## [通过泄漏电磁信号识别手机应用，准确率达 99%](https://www.scmp.com/news/china/science/article/3359688/chinese-researchers-find-peephole-any-smartphone-its-leaked-radio-signal) ⭐️ 8.0/10

中国研究人员开发出一种非接触式取证技术，通过分析智能手机运行时泄漏的低频电磁信号，识别正在运行的应用，准确率高达 99.07%，即使设备处于离线、加密或飞行模式也能工作。 这项研究凸显了严重的隐私和安全漏洞，因为电磁侧信道攻击可以绕过加密和飞行模式等常见保护，可能在没有物理接触的情况下实现监视或取证分析。 实验在 iPhone 15 Pro、小米 15 Pro 和 OPPO Reno 13 上进行，成功识别了抖音、微信视频通话、百度地图、短信、浏览器、相机和云存储等应用。

telegram · zaihuapd · 7月8日 16:05

**背景**: 电磁侧信道攻击利用电子设备无意中发射的射频信号来推断内部操作。与基于软件的漏洞利用不同，这种方法不需要访问设备的操作系统或存储数据，因此即使在锁定或加密的手机上也能有效。

**标签**: `#security`, `#privacy`, `#mobile forensics`, `#electromagnetic signals`, `#research`

---