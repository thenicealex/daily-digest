---
layout: default
title: "Horizon Summary: 2026-07-08 (EN)"
date: 2026-07-08
lang: en
---

> From 59 items, 14 important content pieces were selected

---

1. [OpenAI Launches GPT-Live Voice Mode with Hour-Long Conversations](#item-1) ⭐️ 9.0/10
2. [TypeScript 7.0 Announced with Up to 11.9x Speedup](#item-2) ⭐️ 9.0/10
3. [Agentic safety triggers fail against tool-call attacks](#item-3) ⭐️ 9.0/10
4. [Android Remote Root Exploit Chain Disclosed via Firefox and Kernel Bugs](#item-4) ⭐️ 9.0/10
5. [Grok 4.5 Release with Competitive Pricing and Reasoning Improvements](#item-5) ⭐️ 8.0/10
6. [Mistral Unveils Robostral Navigate: Map-Less Navigation Model](#item-6) ⭐️ 8.0/10
7. [OpenBSD use-after-free leads to local root privilege escalation](#item-7) ⭐️ 8.0/10
8. [EU Advances Legislation Mandating Private Message Scanning](#item-8) ⭐️ 8.0/10
9. [Cloudflare Meerkat: Leaderless Consensus at Global Scale](#item-9) ⭐️ 8.0/10
10. [Fable's Overly Zealous Safety Classifiers Hinder Legitimate Use](#item-10) ⭐️ 8.0/10
11. [SigLIP drastically outperforms DINOv2 in k-NN for fine-grained car classification](#item-11) ⭐️ 8.0/10
12. [LingBot-Video: Open-source 13B sparse MoE video diffusion world model](#item-12) ⭐️ 8.0/10
13. [DeepSeek Develops Its Own AI Chip to Reduce Reliance on Nvidia and Huawei](#item-13) ⭐️ 8.0/10
14. [Smartphone apps identified via leaked radio signals with ~99% accuracy](#item-14) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI Launches GPT-Live Voice Mode with Hour-Long Conversations](https://openai.com/index/introducing-gpt-live/) ⭐️ 9.0/10

OpenAI introduced GPT-Live, a new voice mode for ChatGPT that enables natural, hour-long conversations and can delegate complex tasks to GPT-5.5 in the background. This marks a significant leap in conversational AI, moving beyond short, simplistic voice interactions to sustained, productive dialogues, and bridging the gap between voice models and frontier text models. GPT-Live allows users to have conversations lasting up to an hour, and it can delegate questions to GPT-5.5, a more advanced model, for deeper reasoning. A bug was reported where it would interrupt and laugh at unintended moments.

hackernews · logickkk1 · Jul 8, 17:03 · [Discussion](https://news.ycombinator.com/item?id=48834405)

**Background**: GPT-Live is a new voice mode from OpenAI that powers ChatGPT Voice, designed for more natural human-AI interaction. GPT-5.5, released in April 2026, is a large language model that excels at coding, research, and analysis, running in the background to handle complex queries. Previous voice modes were limited to simpler models, but GPT-Live breaks that restriction.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/introducing-gpt-live/">Introducing GPT-Live | OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.5">GPT-5.5</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some praise the improvement and longer conversations (simonw), while others express concerns about replacing human relationships (jonstaab, overgard). Artdigital notes the lack of tool integration in voice mode, and a bug about interrupting was reported.

**Tags**: `#AI`, `#OpenAI`, `#voice assistant`, `#GPT-5.5`, `#conversational AI`

---

<a id="item-2"></a>
## [TypeScript 7.0 Announced with Up to 11.9x Speedup](https://devblogs.microsoft.com/typescript/announcing-typescript-7-0/) ⭐️ 9.0/10

Microsoft announced TypeScript 7.0, a major release that achieves up to 11.9x faster compilation on large codebases like VS Code, with improvements ranging from 7.7x to 11.9x in internal benchmarks. This release significantly reduces build times for large TypeScript projects, improving developer productivity and addressing a long-standing pain point for the community, while further solidifying TypeScript's position as a leading typed superset of JavaScript. The speed improvements were measured on codebases including VS Code (125.7s to 10.6s), Sentry (139.8s to 15.7s), and Playwright (12.8s to 1.47s). However, community feedback indicates that TypeScript 7 may not work out of the box with common tools like ts-jest, requiring workarounds.

hackernews · DanRosenwasser · Jul 8, 16:06 · [Discussion](https://news.ycombinator.com/item?id=48833715)

**Background**: TypeScript is a typed superset of JavaScript developed by Microsoft that compiles to plain JavaScript, providing static type checking and modern language features. Large codebases often suffer from long compilation times, which has been a major area of optimization. Version 6 was the previous stable release, and version 7 introduces a new architecture or optimizations yielding dramatic speedups.

**Discussion**: The community praised the performance improvements, with one comment highlighting the 11.9x speedup on VS Code and congratulating the team. However, concerns were raised about compatibility with ts-jest and the complexity of tsconfig scoping for mixed environments, alongside excitement for a potential future Rust rewrite.

**Tags**: `#TypeScript`, `#performance`, `#programming languages`, `#Microsoft`

---

<a id="item-3"></a>
## [Agentic safety triggers fail against tool-call attacks](https://www.reddit.com/r/MachineLearning/comments/1ur1fnz/agentic_safety_triggers_arent_textual_safety/) ⭐️ 9.0/10

A new study shows that current safety guardrails for LLM agents fail against attacks where the exploit is encoded in tool-call sequences (e.g., via Model Context Protocol) rather than in the text prompt, with SOTA safety-tuning methods like DPO and SafeDPO refusing only up to 48% of attacks. This finding challenges the assumption that safety alignment can rely solely on textual trigger detection, as agents with real tool access introduce a new attack surface. It signals a paradigm shift needed for AI safety research and development. The attacks leverage a known CVE and rewrite the exploitation steps as ordinary-sounding requests that lead to malicious tool-call sequences. Training-free methods achieved roughly 3× the baseline refusal rate without any fine-tuning.

reddit · r/MachineLearning · /u/mlsandwich · Jul 8, 18:36

**Background**: Model Context Protocol (MCP) is an open standard by Anthropic that standardizes how AI models integrate with external tools and data sources. Direct Preference Optimization (DPO) and SafeDPO are common alignment methods that fine-tune models to reject harmful outputs based on human preferences. This study shows that these textual-based alignment methods are insufficient for agentic tasks involving tool use.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol</a></li>
<li><a href="https://en.wikipedia.org/wiki/Direct_preference_optimization">Direct preference optimization</a></li>
<li><a href="https://arxiv.org/abs/2505.20065">[2505.20065] SafeDPO: A Simple Approach to Direct Preference Optimization with Enhanced Safety</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#LLM agents`, `#adversarial attacks`, `#tool use`, `#MCP`

---

<a id="item-4"></a>
## [Android Remote Root Exploit Chain Disclosed via Firefox and Kernel Bugs](https://www.coolapk.com/feed/72700258?s=ZGQ2MTVlZjYxMDYyNTM3ZzZhNGUzOThjega1640) ⭐️ 9.0/10

Security firm Nebula disclosed a remote root exploit chain affecting Android 17 and all earlier versions, combining a Firefox browser vulnerability (Firefox 151.0.2 and earlier) with a 15-year-old Linux kernel bug. Proof-of-concept code has been published on GitHub. This exploit allows attackers to gain persistent root access by simply having a user click a malicious link, affecting millions of devices. The public availability of proof-of-concept code increases the risk of widespread exploitation before patches are deployed. The exploit chain uses a memory safety bug in Firefox 151.0.2 and earlier for initial code execution, then leverages a ancient Linux kernel vulnerability to escalate privileges to root. Google Pixel devices have been tested and confirmed compromised, and a complete Android 17 device can be rooted within one minute.

telegram · zaihuapd · Jul 8, 13:01

**Background**: A remote root exploit chain combines multiple vulnerabilities to gain full system control over a device without physical access. The Firefox vulnerability is a memory safety bug fixed in version 151, while the Linux kernel bug has existed for 15 years and was recently patched by the kernel maintainers. Proof-of-concept code demonstrates the attack and helps vendors develop fixes, but also enables malicious actors.

<details><summary>References</summary>
<ul>
<li><a href="https://www.mozilla.org/en-US/security/known-vulnerabilities/firefox/">Security Advisories for Firefox — Mozilla</a></li>
<li><a href="https://github.com/secmob/TiYunZong-An-Exploit-Chain-to-Remotely-Root-Modern-Android-Devices">GitHub - secmob/TiYunZong-An-Exploit-Chain-to-Remotely-Root-Modern-Android-Devices</a></li>
<li><a href="https://www.mozilla.org/en-US/security/advisories/mfsa2026-46/">Security Vulnerabilities fixed in Firefox 151 — Mozilla</a></li>

</ul>
</details>

**Tags**: `#Android`, `#vulnerability`, `#remote root`, `#Linux kernel`, `#cybersecurity`

---

<a id="item-5"></a>
## [Grok 4.5 Release with Competitive Pricing and Reasoning Improvements](https://x.ai/news/grok-4-5) ⭐️ 8.0/10

xAI released Grok 4.5, claiming improved reasoning efficiency and competitive pricing at $2/$6 per million tokens, trained on trillions of tokens of Cursor data. This release challenges other AI models on cost while leveraging unique real-world coding data from Cursor, potentially influencing developer tools and agent interactions. However, trust concerns may limit enterprise adoption. Grok 4.5 is priced at $2/$6 per million tokens, offering 4x better reasoning efficiency than Opus, and benchmarks suggest it performs at Opus 4.7 level. The model was trained on Cursor data capturing real-world developer-agent interactions.

hackernews · BoumTAC · Jul 8, 18:00 · [Discussion](https://news.ycombinator.com/item?id=48835111)

**Background**: Grok is a large language model developed by xAI, Elon Musk's AI company. The model uses data from Cursor, an AI-powered code editor, which provides real-world coding interactions. This approach aims to improve the model's understanding of developer workflows.

**Discussion**: Many commenters express distrust, citing political bias and ethical concerns such as xAI's perceived tolerance of CSAM. Some acknowledge the model's cost efficiency and performance, but question the economic sense of massive AI spending.

**Tags**: `#AI`, `#Grok`, `#xAI`, `#Model Release`, `#Benchmark`

---

<a id="item-6"></a>
## [Mistral Unveils Robostral Navigate: Map-Less Navigation Model](https://mistral.ai/news/robostral-navigate/) ⭐️ 8.0/10

Mistral AI has released Robostral Navigate, an 8-billion-parameter robotics navigation model that achieves map-less navigation using a single RGB camera, trained entirely in simulation. This model advances embodied AI by enabling robots to navigate unknown environments without pre-built maps, reducing deployment time and cost for industrial automation and hobbyist robotics. Robostral Navigate sets a state-of-the-art on the R2R-CE benchmark and combines pointing-based navigation with reinforcement learning for continuous improvement. It is not openly available, but Mistral may offer access through partnerships.

hackernews · ottomengis · Jul 8, 14:09 · [Discussion](https://news.ycombinator.com/item?id=48832212)

**Background**: Traditional robot navigation relies on pre-built maps of the environment, which must be created beforehand and updated when the environment changes. Map-less navigation instead uses sensor data (e.g., camera images) and learned policies to move through unfamiliar spaces. Simulation training allows the model to learn robust behaviors without physical hardware risks.

<details><summary>References</summary>
<ul>
<li><a href="https://mistral.ai/news/robostral-navigate/">Robostral Navigate: single-camera AI navigation | Mistral AI</a></li>
<li><a href="https://cryptobriefing.com/mistral-robostral-navigate-robotics-model/">Mistral AI unveils Robostral Navigate, an 8B robotics model that could reshape industrial automation investing</a></li>
<li><a href="https://x.com/MistralAI/status/2074856309438980145">Mistral AI on X: "Announcing Robostral Navigate, our first model for embodied navigation: an 8B robotics navigation model that guides robots to autonomously perform tasks specified with natural language. Single RGB camera. State-of-the-art on R2R-CE. https://t.co/UlmUsXNxhX" / X</a></li>

</ul>
</details>

**Discussion**: The Hacker News community expressed excitement about map-less navigation, with users noting its potential for hobbyist projects like farm robots. Some highlighted that indoor map-less navigation is a newer challenge than outdoor, and compared it to Stanford's PIGEON model. Others lamented the lack of open availability, hoping for future release.

**Tags**: `#robotics`, `#navigation`, `#AI`, `#Mistral`, `#deep learning`

---

<a id="item-7"></a>
## [OpenBSD use-after-free leads to local root privilege escalation](https://nvd.nist.gov/vuln/detail/cve-2026-57589) ⭐️ 8.0/10

A use-after-free vulnerability (CVE-2026-57589) in OpenBSD has been disclosed, allowing a local attacker to escalate privileges to root. The bug was discovered by Trail of Bits as part of OpenAI's Patch The Planet initiative, which uses AI models to find vulnerabilities in open-source software. This finding is significant because OpenBSD is widely regarded as one of the most security-focused operating systems. It also highlights the growing role of AI-assisted bug hunting in improving open-source security. The vulnerability is a use-after-free issue that can be exploited for local privilege escalation to root. The discovery was made under the Patch The Planet project, which provides AI model access to security firms for vulnerability research.

hackernews · linggen · Jul 8, 13:24 · [Discussion](https://news.ycombinator.com/item?id=48831658)

**Background**: OpenBSD is a free, Unix-like operating system focused on security, featuring proactive measures and integrated cryptography. A use-after-free vulnerability occurs when a program continues to use a pointer after the memory it points to has been freed, often leading to crashes or arbitrary code execution. Local privilege escalation means an attacker with limited access can gain full root control.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenBSD">OpenBSD</a></li>

</ul>
</details>

**Discussion**: Community members noted the discovery was part of Patch The Planet, and some praised OpenBSD's security culture despite this finding. Others wondered why the vulnerability was not yet listed on OpenBSD's security page and expressed curiosity about how many vulnerabilities might be found as AI-assisted hunting expands.

**Tags**: `#OpenBSD`, `#security`, `#vulnerability`, `#privilege escalation`, `#use-after-free`

---

<a id="item-8"></a>
## [EU Advances Legislation Mandating Private Message Scanning](https://cyberinsider.com/eu-now-one-step-away-from-reviving-private-message-scanning-rules/) ⭐️ 8.0/10

The European Parliament has voted to fast-track the return of Chat Control 1.0, allowing voluntary scanning of private messages by providers like Meta, and a binding vote on mandatory scanning (Chat Control 2.0) is scheduled for July 9, 2025. This legislation threatens end-to-end encryption and user privacy, potentially forcing messaging platforms to scan all private communications for child sexual abuse material, which could set a global precedent for surveillance. Chat Control 1.0 allows voluntary scanning, while Chat Control 2.0 mandates scanning and bans end-to-end encryption; an absolute majority of 361 MEPs is needed to stop the latter in the upcoming vote.

hackernews · ggirelli · Jul 8, 16:53 · [Discussion](https://news.ycombinator.com/item?id=48834296)

**Background**: Chat Control is a proposed EU regulation to combat child sexual abuse by scanning messages, but critics argue it undermines encryption and privacy. The legislation is divided into two versions: Chat Control 1.0 permits voluntary scanning under an ePrivacy derogation, while Chat Control 2.0 mandates scanning and effectively bans end-to-end encryption. The Internet Watch Foundation, funded by big tech, supports client-side scanning.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control">Chat Control - Wikipedia</a></li>
<li><a href="https://fightchatcontrol.eu/">Fight Chat Control - Protect Digital Privacy in the EU</a></li>
<li><a href="https://www.patrick-breyer.de/en/posts/chat-control/">Chat Control: The EU's CSAM scanner proposal</a></li>

</ul>
</details>

**Discussion**: Comments express skepticism, with one user noting the Internet Watch Foundation pushes for client-side scanning. Another clarifies that Chat Control 1.0 is less concerning than 2.0, which mandates scanning and bans encryption. Some view it as 'Terminator legislation' that will keep returning.

**Tags**: `#privacy`, `#EU legislation`, `#encryption`, `#surveillance`

---

<a id="item-9"></a>
## [Cloudflare Meerkat: Leaderless Consensus at Global Scale](https://blog.cloudflare.com/meerkat-introduction/) ⭐️ 8.0/10

Cloudflare announced Meerkat, a globally distributed consensus algorithm that is leaderless and based on asynchronous consensus (QuePaxa). This marks the first production implementation of an asynchronous consensus protocol, which does not rely on timeouts. Meerkat's leaderless design eliminates issues like leader flapping and election storms common in leader-based protocols (e.g., Raft), improving resilience under variable network conditions. It enables Cloudflare to maintain strong consistency across its global edge network without a single point of failure. Unlike Paxos or Raft, which are partially synchronous and rely on timeouts, QuePaxa (the core of Meerkat) makes progress even with wild fluctuations in message delay. However, it requires global consensus for every read operation, which may introduce higher latency compared to systems that use local reads.

hackernews · bobnamob · Jul 8, 13:18 · [Discussion](https://news.ycombinator.com/item?id=48831565)

**Background**: Distributed consensus algorithms allow multiple nodes to agree on a single value despite failures. Traditional protocols like Paxos and Raft are partially synchronous: they assume bounds on message delays and use timeouts to detect failures, which can cause issues on unreliable networks. Asynchronous consensus removes these timing assumptions, guaranteeing progress regardless of network latency, but has historically been considered too expensive for practical use. Meerkat aims to make this practical at global scale.

**Discussion**: The community acknowledged the novelty of a production asynchronous consensus implementation, but some questioned the trade-offs: requiring consensus for reads limits use cases, and comparisons to leaderless Paxos-class algorithms would have been more appropriate than to Raft. Others noted that for messy networks, Meerkat's approach could be beneficial, though it is not yet in production.

**Tags**: `#distributed consensus`, `#cloudflare`, `#leaderless`, `#asynchronous`, `#systems research`

---

<a id="item-10"></a>
## [Fable's Overly Zealous Safety Classifiers Hinder Legitimate Use](https://combine-lab.github.io/blog/2026/07/07/fable-is-not-a-useful-model.html) ⭐️ 8.0/10

A blog post and community discussion reveal that Anthropic's Fable model frequently and incorrectly downgrades legitimate user requests to the less capable Opus 4.8 model, due to overly sensitive safety classifiers. This issue undermines the usability of Fable for many legitimate tasks, especially in scientific and technical fields, and raises concerns about the tradeoff between safety and functionality in AI systems. The classifier is designed to downgrade requests related to cybersecurity, biology, or jailbreak attempts, but it triggers on benign queries such as statistical analysis for clinical trials or code optimization for GPUs.

hackernews · karrot-kake · Jul 8, 20:41 · [Discussion](https://news.ycombinator.com/item?id=48837162)

**Background**: Anthropic's Fable is a powerful AI model built on their constitutional AI approach, which includes safety classifiers to prevent misuse. However, the classifier's high false-positive rate causes it to route many harmless requests to Opus 4.8, a less capable model, frustrating users with legitimate needs.

**Discussion**: Commenters share numerous examples, including a medical physicist unable to get any work-related question answered, and a developer whose requests for vLLM patching were constantly downgraded. They express frustration and note that such over-filtering makes the model nearly useless for serious work.

**Tags**: `#Anthropic`, `#Fable`, `#safety classifiers`, `#AI usability`, `#model limitations`

---

<a id="item-11"></a>
## [SigLIP drastically outperforms DINOv2 in k-NN for fine-grained car classification](https://www.reddit.com/r/MachineLearning/comments/1uqtamz/dinov2_way_worse_than_siglip_in_knn_is_this/) ⭐️ 8.0/10

A user reports that SigLIP2 SO400M achieves ~92% accuracy with weighted k-NN on a fine-grained car classification dataset, while DINOv2 Giant only reaches ~41%, despite both models having similar scale and frozen encoders. This huge performance gap challenges the assumption that state-of-the-art self-supervised vision models like DINOv2 are universally suitable for retrieval tasks, highlighting the importance of contrastive pretraining objectives for k-NN based fine-grained classification. The user used L2-normalized embeddings and tried both cosine and Euclidean distance with no change. They note that DINOv2 is self-supervised and likely requires a trained linear probe to perform well, while SigLIP's contrastive training naturally structures the embedding space for similarity search.

reddit · r/MachineLearning · /u/psy_com · Jul 8, 13:51

**Background**: Self-supervised learning (SSL) methods like DINOv2 learn visual representations without explicit labels, focusing on semantic features, while contrastive methods like SigLIP explicitly pull similar image-text pairs together in embedding space. k-NN classification uses nearest neighbors in the embedding space to classify images, so models that structure embeddings for similarity naturally perform better. Fine-grained car classification requires distinguishing subtle differences between closely related models like VW Golf generations.

**Tags**: `#DINOv2`, `#SigLIP`, `#k-NN`, `#fine-grained classification`, `#self-supervised learning`

---

<a id="item-12"></a>
## [LingBot-Video: Open-source 13B sparse MoE video diffusion world model](https://www.reddit.com/r/MachineLearning/comments/1ur0bxq/lingbotvideo_sparsemoe_video_diffusion/) ⭐️ 8.0/10

LingBot-Video, a 13B-parameter sparse mixture-of-experts video diffusion transformer with only 1.4B active parameters, has been released as open source with reinforcement learning post-training and action-conditioned video prediction for robot world modeling. This model advances open-source video generation by combining efficient sparse MoE architecture with RL-based physical plausibility reward, pushing toward practical world models for robotics. Its release invites community scrutiny on the boundary between video generators and action-conditional world models. The model uses a DeepSeek-V3-style sparse MoE with 128 experts and top-8 routing, and is post-trained with six rewards including a VLM-graded physical-plausibility loss. It features an action-to-video mode that predicts robot rollout frames from action and hand-pose inputs.

reddit · r/MachineLearning · /u/Savings-Display5123 · Jul 8, 17:58

**Background**: Video diffusion models generate temporally coherent video frames from noise via iterative denoising. Sparse mixture-of-experts (MoE) architectures selectively activate only a subset of parameters per token, enabling larger total model capacity with lower computational cost. World models in robotics aim to simulate future states from actions, bridging generative video and embodied AI.

**Discussion**: The community raised two main concerns: (1) whether a VLM judging physical plausibility from sampled frames is reliable or prone to Goodhart's law, and (2) whether the model truly functions as a world model given it only outputs video-quality frames without closed-loop robot experiments. The author acknowledged these points and invited further critique.

**Tags**: `#video diffusion`, `#world model`, `#sparse MoE`, `#reinforcement learning`, `#open-source`

---

<a id="item-13"></a>
## [DeepSeek Develops Its Own AI Chip to Reduce Reliance on Nvidia and Huawei](https://t.me/zaihuapd/42423) ⭐️ 8.0/10

DeepSeek, a Chinese AI company, is developing its own AI chip focused on inference to reduce dependence on Nvidia and Huawei chips. The project started about a year ago and is still in early stages, with the company recruiting chip design engineers. This move could reduce DeepSeek's vulnerability to US export controls and geopolitical risks associated with relying on foreign chip suppliers. If successful, it may also lower costs and enable custom optimizations for their specific AI workloads. The chip is designed for inference, the phase where a trained model generates responses, rather than training. DeepSeek has contacted chip design, foundry, and memory companies, and has been privately recruiting chip design engineers in recent months.

telegram · zaihuapd · Jul 8, 05:20

**Background**: DeepSeek is a Chinese AI startup known for its large language models, which previously relied on Nvidia H800 and Huawei Ascend chips. US export restrictions have limited Chinese access to advanced AI chips, prompting domestic companies to develop their own hardware. Inference chips are typically less complex than training chips but still critical for AI deployment.

**Tags**: `#AI chips`, `#DeepSeek`, `#hardware`, `#inference`, `#semiconductors`

---

<a id="item-14"></a>
## [Smartphone apps identified via leaked radio signals with ~99% accuracy](https://www.scmp.com/news/china/science/article/3359688/chinese-researchers-find-peephole-any-smartphone-its-leaked-radio-signal) ⭐️ 8.0/10

Chinese researchers developed a non-contact forensic technique that analyzes low-frequency electromagnetic signals leaked from smartphones to identify running apps with up to 99.07% accuracy, even when devices are offline, encrypted, or in airplane mode. This research highlights a serious privacy and security vulnerability, as electromagnetic side-channel attacks can bypass common protections like encryption and flight mode, potentially enabling surveillance or forensic analysis without physical access. The experiments were conducted on iPhone 15 Pro, Xiaomi 15 Pro, and OPPO Reno 13, successfully identifying apps including Douyin, WeChat video calls, Baidu Maps, messaging, browser, camera, and cloud storage applications.

telegram · zaihuapd · Jul 8, 16:05

**Background**: Electromagnetic side-channel attacks exploit unintentional radio frequency emissions from electronic devices to infer internal operations. Unlike software-based exploits, this approach does not require access to the device's operating system or stored data, making it effective even on locked or encrypted phones.

**Tags**: `#security`, `#privacy`, `#mobile forensics`, `#electromagnetic signals`, `#research`

---