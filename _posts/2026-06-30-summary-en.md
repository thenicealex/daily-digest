---
layout: default
title: "Horizon Summary: 2026-06-30 (EN)"
date: 2026-06-30
lang: en
---

> From 61 items, 13 important content pieces were selected

---

1. [vLLM v0.24.0 Released with New Models and Major Optimizations](#item-1) ⭐️ 9.0/10
2. [Supreme Court mandates warrants for geofence searches](#item-2) ⭐️ 9.0/10
3. [Google's Agentic AI Peer Reviewer Handles 10K Papers](#item-3) ⭐️ 9.0/10
4. [CXMT signs ~$3B DRAM supply deal with Tencent](#item-4) ⭐️ 9.0/10
5. [Rocket Lab acquires Iridium for launch baseline and satellite manufacturing](#item-5) ⭐️ 8.0/10
6. [WATaBoy: JIT-ing Game Boy Instructions to WASM Outperforms Native Interpreter](#item-6) ⭐️ 8.0/10
7. [Under the Hood of a CUDA Kernel Launch: Doorbell and QMD](#item-7) ⭐️ 8.0/10
8. [European ISPs Seek Liability for Rightsholders Over Overblocking](#item-8) ⭐️ 8.0/10
9. [Ornith-1.0: Open-Source Self-Scaffolding LLMs for Agentic Coding](#item-9) ⭐️ 8.0/10
10. [Cerebras-OpenAI Deal Blocks Startups from Inference Capacity](#item-10) ⭐️ 8.0/10
11. [EML Trees Proven as Universal Approximators](#item-11) ⭐️ 8.0/10
12. [Ransomware group leaks iPhone 18 Pro data from Apple's India supplier Tata](#item-12) ⭐️ 8.0/10
13. [Samsung and SK Hynix Unveil Massive AI Investment Plans](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.24.0 Released with New Models and Major Optimizations](https://github.com/vllm-project/vllm/releases/tag/v0.24.0) ⭐️ 9.0/10

vLLM v0.24.0 has been released with 571 commits from 256 contributors, adding support for MiniMax-M3 and DiffusionGemma models, and delivering major optimizations for DeepSeek-V4 including a FlashInfer sparse index cache and cluster-cooperative topK kernel. As a widely used LLM inference engine, this release significantly improves performance for large MoE models like DeepSeek-V4 and expands model support, making high-throughput serving more efficient and accessible. Notable technical additions include MXFP4 quantization for MiniMax-M3, a FlashInfer sparse index cache that reduces time-to-first-token by 2–4%, and a new streaming parser engine unifying tool-call parsing across models.

github · khluu · Jun 29, 19:41

**Background**: vLLM is a high-throughput, memory-efficient inference engine for large language models, leveraging PagedAttention and continuous batching. MiniMax-M3 is a new dense model, while DeepSeek-V4 is a large Mixture-of-Experts (MoE) model that benefits from optimized kernel libraries like FlashInfer. MXFP4 is a 4-bit block floating-point format that compresses model weights with minimal accuracy loss.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/flashinfer-ai/flashinfer">GitHub - flashinfer-ai/flashinfer: FlashInfer: Kernel Library for LLM Serving · GitHub</a></li>
<li><a href="http://www.kapilsharma.dev/posts/mxfp4-visualizer/">Understanding MXFP4 Quantization | Kapil Sharma</a></li>
<li><a href="https://newreleases.io/project/github/vllm-project/vllm/release/v0.24.0">vllm-project/vllm v0.24.0 on GitHub - NewReleases.io</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM inference`, `#model serving`, `#AI infrastructure`

---

<a id="item-2"></a>
## [Supreme Court mandates warrants for geofence searches](https://www.theguardian.com/us-news/2026/jun/29/supreme-court-geofence-warrants-case-decision) ⭐️ 9.0/10

The US Supreme Court ruled that geofence warrants are subject to Fourth Amendment protections, requiring law enforcement to obtain a warrant based on probable cause before accessing location data of devices within a defined area. This landmark decision significantly limits the use of geofence warrants by law enforcement, strengthening digital privacy rights and affecting tech companies that store location data. The Court held that the government's warrantless acquisition of cell phone location data for a geographic area constitutes a search under the Fourth Amendment, as highlighted by Justice Kagan's opinion citing Riley v. California.

hackernews · cdrnsf · Jun 29, 15:54 · [Discussion](https://news.ycombinator.com/item?id=48720924)

**Background**: A geofence warrant, also known as a reverse location warrant, allows law enforcement to search a tech company's database for all mobile devices within a specific geographic area during a certain time period. These warrants have been used in investigations but have raised privacy concerns due to their sweeping nature, often implicating innocent bystanders. The Fourth Amendment protects against unreasonable searches and seizures, requiring warrants to be particular and based on probable cause.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Geofence_warrant">Geofence warrant - Wikipedia</a></li>
<li><a href="https://www.nacdl.org/Content/Geofence-Warrants">NACDL - Geofence Warrants</a></li>

</ul>
</details>

**Discussion**: Commenters discussed the decision's reasoning, with one noting the Court's factual sourcing and reference to Riley. Another highlighted the Paula Broadwell example to illustrate that location data can be identified through other means. There was also debate about whether products like Flock would now require warrants.

**Tags**: `#privacy`, `#supreme-court`, `#geofence-warrants`, `#fourth-amendment`, `#digital-rights`

---

<a id="item-3"></a>
## [Google's Agentic AI Peer Reviewer Handles 10K Papers](https://www.reddit.com/r/MachineLearning/comments/1uio9rb/googles_agentic_peerreviewer_handled_10k_papers/) ⭐️ 9.0/10

Google deployed an agentic AI peer-review system at the ICML and STOC conferences, processing approximately 10,000 papers with a 30-minute turnaround. The formal research paper reveals that this system detects 34% more mathematical errors compared to zero-shot prompting. This marks a major milestone in AI-assisted scientific review, demonstrating practical large-scale deployment with measurable improvements. It could accelerate peer review processes and improve quality control in academic publishing. The system is an agentic AI, meaning it operates autonomously with goal-driven behavior and adapts to tasks. It processed submissions with a 30-minute average turnaround, catching 34% more mathematical errors than zero-shot prompting, as documented in the formal paper on arXiv.

reddit · r/MachineLearning · /u/Justgototheeffinmoon · Jun 29, 10:05

**Background**: Agentic AI refers to AI systems that exhibit autonomy, goal-driven behavior, and adaptability, unlike traditional models that require human intervention. Zero-shot prompting is a technique where a model performs a task without any examples in the prompt, relying solely on its pre-training. This news combines both concepts to create an automated peer reviewer that operates at conference scale.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/agentic-ai">What is Agentic AI? | IBM</a></li>
<li><a href="https://www.promptingguide.ai/techniques/zeroshot">Zero-Shot Prompting | Prompt Engineering Guide</a></li>

</ul>
</details>

**Tags**: `#AI`, `#peer review`, `#scientific publishing`, `#machine learning`, `#Google`

---

<a id="item-4"></a>
## [CXMT signs ~$3B DRAM supply deal with Tencent](https://www.reuters.com/world/china/chinas-cxmt-wins-3-billion-memory-supply-deal-with-tencent-sources-say-2026-06-29/) ⭐️ 9.0/10

ChangXin Memory Technologies (CXMT) has signed a long-term DRAM supply deal worth over 200 billion RMB (about $2.94 billion) with Tencent, covering server memory for a period of 3 to 5 years, according to sources. This deal marks a major step for Chinese DRAM maker CXMT in penetrating the domestic cloud and internet market, potentially reducing reliance on foreign memory suppliers like Samsung and SK Hynix. It also underscores growing collaboration between Chinese tech giants to strengthen supply chain self-sufficiency amid geopolitical tensions. The deal value is reported to be approximately $3 billion, with contract durations varying between 3 and 5 years. CXMT is also reportedly in talks with other Chinese internet companies including Alibaba Cloud, ByteDance, and Xiaomi for similar supply agreements.

telegram · zaihuapd · Jun 29, 09:31

**Background**: DRAM (Dynamic Random Access Memory) is a type of semiconductor memory widely used in servers, PCs, and mobile devices. CXMT is one of China's leading DRAM manufacturers, aiming to compete with global giants like Samsung, SK Hynix, and Micron. The Chinese government has been promoting domestic semiconductor production to reduce dependence on foreign technology, especially in the wake of US export restrictions.

**Tags**: `#semiconductors`, `#DRAM`, `#China`, `#Tencent`, `#supply chain`

---

<a id="item-5"></a>
## [Rocket Lab acquires Iridium for launch baseline and satellite manufacturing](https://investors.rocketlabcorp.com/news-releases/news-release-details/rocket-lab-acquire-iridium-historic-deal-creating-fully) ⭐️ 8.0/10

Rocket Lab announced the acquisition of Iridium Communications, securing a steady baseline of launches and integrating satellite manufacturing into its operations. This move gives Rocket Lab a guaranteed launch demand similar to SpaceX's Starlink, reducing risk as it scales up. It also positions Rocket Lab as a fully integrated space company, potentially reshaping the small satellite launch market. The acquisition includes Iridium's LEO satellite constellation at 780 km orbit, which Electron can reach, and plans for next-generation replacements. Rocket Lab's upcoming Neutron rocket will handle larger payloads for constellation replenishment.

hackernews · everfrustrated · Jun 29, 14:09 · [Discussion](https://news.ycombinator.com/item?id=48719485)

**Background**: Rocket Lab is an aerospace manufacturer and launch service provider known for its Electron rocket, the most prolific small-lift launch vehicle globally. Iridium operates a 66-satellite LEO constellation for global communications. This acquisition merges launch and satellite manufacturing under one roof, a model pioneered by SpaceX.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Rocket_Lab">Rocket Lab - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Iridium_Communications">Iridium Communications - Wikipedia</a></li>
<li><a href="https://rocketlabcorp.com/about/about-us/">Rocket Lab | About Us | Rocket Lab</a></li>

</ul>
</details>

**Discussion**: Some commenters expressed concerns about space junk from increasing satellite numbers, while others praised the strategic move, comparing it to SpaceX's use of Starlink to guarantee launches. A few noted Rocket Lab's shift from New Zealand to US headquarters.

**Tags**: `#space`, `#acquisition`, `#rocketlab`, `#iridium`, `#satellite`

---

<a id="item-6"></a>
## [WATaBoy: JIT-ing Game Boy Instructions to WASM Outperforms Native Interpreter](https://humphri.es/blog/WATaBoy/) ⭐️ 8.0/10

WATaBoy is a Game Boy emulator that dynamically recompiles SM83 CPU instructions to WebAssembly (WASM) at runtime, achieving faster performance than a native interpreter. This approach enables JIT compilation on platforms like iOS that restrict native JIT, potentially unlocking high-performance emulation in browsers and mobile apps, and demonstrates WASM's viability as a JIT target. The emulator targets the SM83 (Game Boy's Z80-like CPU) and uses JavaScript's eval-like mechanisms like new Function() to generate optimized WASM code at runtime. Firefox is reported to be 25% slower than Chrome/Safari in this use case.

hackernews · energeticbark · Jun 29, 15:02 · [Discussion](https://news.ycombinator.com/item?id=48720190)

**Background**: JIT (Just-In-Time) compilation converts code during execution for faster performance, but iOS bans native JIT for apps. Web browsers, however, are allowed to JIT-compile JavaScript and WebAssembly. WATaBoy leverages this loophole: by writing a JIT that emits WASM, it piggybacks on the browser's existing WASM JIT compiler, achieving speed gains while complying with platform restrictions.

<details><summary>References</summary>
<ul>
<li><a href="https://humphri.es/blog/WATaBoy/">WATaBoy: JIT-ing Game Boy Instructions to Wasm Beats a Native Interpreter</a></li>
<li><a href="https://github.com/torch2424/wasmboy">GitHub - torch2424/wasmboy: Game Boy / Game Boy Color Emulator Library, 🎮written for WebAssembly using AssemblyScript. 🚀Demos built with Preact and Svelte. ⚛️</a></li>
<li><a href="https://asktechnicians.com/the-browser-loophole-that-could-sneak-emulators-onto-iphone">JIT - to - Wasm : The Browser Loophole for iPhone Emulators · Ask...</a></li>

</ul>
</details>

**Discussion**: Commenters noted that using JavaScript eval/new Function is the simplest JIT approach, and one discussed how Apple's exception for browser JIT makes WATaBoy viable on iOS. There was also a mention that WASM overhead (~20%) is far less than interpreter overhead (~1000%), so outperforming an interpreter is expected but the project is still impressive for an undergraduate.

**Tags**: `#JIT compilation`, `#WebAssembly`, `#Game Boy emulation`, `#performance`, `#emulator`

---

<a id="item-7"></a>
## [Under the Hood of a CUDA Kernel Launch: Doorbell and QMD](https://fergusfinn.com/blog/what-happens-when-you-run-a-gpu-kernel/) ⭐️ 8.0/10

A technical blog post details the entire path of a CUDA kernel from host code to GPU execution, explaining the doorbell mechanism and Queue Metadata Descriptor (QMD) that connect software API calls to hardware submission. This explanation fills a critical gap in typical CUDA tutorials, helping developers understand GPU command submission overhead and enabling more informed optimization of kernel launches. The doorbell is a write to a memory-mapped register that signals the GPU to fetch commands, while the QMD is a data structure containing kernel parameters and pointers that the GPU's work distributor reads.

hackernews · mezark · Jun 29, 13:11 · [Discussion](https://news.ycombinator.com/item?id=48718863)

**Background**: CUDA is a parallel computing platform that allows developers to run code on GPUs. When a kernel is launched, the CPU driver builds a command buffer and writes a doorbell, triggering the GPU to fetch and execute the commands. The QMD holds metadata such as grid dimensions, block size, and kernel arguments, which the GPU uses to schedule thread blocks on streaming multiprocessors.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2605.01352v1">VUDA: Breaking CUDA-Vulkan Isolation for Spatial Sharing of Compute and Graphics on the Same GPU</a></li>

</ul>
</details>

**Discussion**: Commenters praised the article for clarifying the CPU-to-GPU path, especially the doorbell and QMD concepts. One noted that NVIDIA provides open GPU documentation for QMD formats, while another appreciated the connection between CUDA syntax and hardware submission. A third speculated about the future of kernel optimization tools.

**Tags**: `#CUDA`, `#GPU`, `#kernel execution`, `#HPC`, `#technical deep-dive`

---

<a id="item-8"></a>
## [European ISPs Seek Liability for Rightsholders Over Overblocking](https://torrentfreak.com/european-isps-want-rightsholders-held-accountable-for-overblocking-damage/) ⭐️ 8.0/10

European Internet Service Providers (ISPs) are demanding that rightsholders be held legally and financially accountable for damages caused by overzealous copyright blocking measures that affect legitimate content. This push could rebalance the power dynamics in online copyright enforcement, discouraging overly broad blocking orders that currently disrupt legitimate internet traffic without consequence for rightsholders. The demand comes amid growing frustration, particularly in Spain, where court-ordered blockades during soccer matches frequently ensnare unrelated services and legitimate users.

hackernews · Brajeshwar · Jun 29, 16:07 · [Discussion](https://news.ycombinator.com/item?id=48721072)

**Background**: Overblocking occurs when ISPs inadvertently block legitimate content due to overly broad filtering rules aimed at copyright infringement. Currently, rightsholders often face no liability for such overreach, leaving ISPs and users to bear the costs of disrupted access.

<details><summary>References</summary>
<ul>
<li><a href="https://de.wikipedia.org/wiki/Overblocking">Overblocking – Wikipedia</a></li>
<li><a href="https://www.findlaw.com/smallbusiness/intellectual-property/isp-liability-for-the-acts-of-its-customers.html">ISP Liability for the Acts of Its Customers - FindLaw</a></li>

</ul>
</details>

**Discussion**: Comments largely support the ISPs' stance, criticizing the ease with which rightsholders can censor content without court oversight, with some noting the extreme disruption in Spain and others linking the issue to broader debates about internet censorship and corporate power.

**Tags**: `#internet governance`, `#copyright`, `#ISP liability`, `#censorship`, `#Spain`

---

<a id="item-9"></a>
## [Ornith-1.0: Open-Source Self-Scaffolding LLMs for Agentic Coding](https://simonwillison.net/2026/Jun/29/ornith/#atom-everything) ⭐️ 8.0/10

DeepReinforce releases Ornith-1.0, an MIT-licensed family of open-weight coding LLMs with up to 397B parameters, built on Gemma 4 and Qwen 3.5, achieving state-of-the-art performance on coding benchmarks. This marks the first major open-source release from DeepReinforce and demonstrates a new 'self-scaffolding' training paradigm that could enable more autonomous coding agents, potentially accelerating AI-assisted software development. The family includes 9B Dense, 31B Dense, 35B MoE, and 397B MoE variants; all are MIT licensed, and the underlying models (Gemma 4 and Qwen 3.5) are Apache 2.0 licensed, ensuring compatibility. Early tests show strong performance in multi-step tool calling and code understanding.

rss · Simon Willison · Jun 29, 16:17

**Background**: Self-scaffolding LLMs are models that generate their own reasoning or tool-use structures during inference, improving performance on complex tasks without external orchestration. Agentic coding refers to AI agents that autonomously perform multi-step software development tasks. The GGUF format enables efficient local inference via tools like LM Studio, making these models accessible to individual developers.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/29/ornith/">Ornith-1.0: Self - Scaffolding LLMs for Agentic Coding</a></li>
<li><a href="https://deep-reinforce.com/ornith_1_0.html">Ornith-1.0: Self - Scaffolding LLMs ... | DeepReinforce Blog | Jun. 2026</a></li>
<li><a href="https://en.wikipedia.org/wiki/Agentic_coding">Agentic coding</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#open-source`, `#coding`, `#AI`, `#deep learning`

---

<a id="item-10"></a>
## [Cerebras-OpenAI Deal Blocks Startups from Inference Capacity](https://www.reddit.com/r/MachineLearning/comments/1uiqhiv/cerebras_openai_deal_capacity_has_effectively/) ⭐️ 8.0/10

Cerebras has allocated most of its near-term inference capacity to OpenAI through a multi-billion dollar deal, effectively making its API waitlist indefinite for other startups. This concentration of compute resources to a single customer threatens the ability of smaller AI startups and researchers to access fast, ASIC-based inference, potentially stifling innovation and consolidating market power. Cerebras' Wafer-Scale Engine (WSE) is a large ASIC designed for high-throughput AI workloads, but production capacity appears limited. The poster requires ~1-2k tokens/second inference with low p95 latency, which GPUs cannot easily provide.

reddit · r/MachineLearning · /u/Kortopi-98 · Jun 29, 12:00

**Background**: Cerebras produces the Wafer-Scale Engine, the world's largest AI processor, targeting both training and inference. Inference ASICs offer specialized performance for real-time applications, but manufacturing such large chips is complex and capacity is constrained. P95 latency measures the 95th percentile response time; for a real-time coding agent, low p95 latency is critical for responsiveness.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cerebras">Cerebras - Wikipedia</a></li>
<li><a href="https://www.cerebras.ai/chip">Product - Chip - Cerebras</a></li>
<li><a href="https://redis.io/blog/p95-latency/">P95 Latency: What It Is & Why It Matters - Redis</a></li>

</ul>
</details>

**Discussion**: The Reddit post expresses strong frustration from a startup founder whose needs are unmet due to the Cerebras-OpenAI deal. Comments (not provided in the snippet) likely echo concerns about resource monopolization and barriers for small players.

**Tags**: `#Cerebras`, `#OpenAI`, `#inference`, `#compute capacity`, `#AI startup`

---

<a id="item-11"></a>
## [EML Trees Proven as Universal Approximators](https://www.reddit.com/r/MachineLearning/comments/1uipl1t/eml_trees_are_universal_approximators_r/) ⭐️ 8.0/10

The author proves that EML trees are universal approximators by constructing explicit EML representations of polynomials, hyperbolic tangent, and partitions of unity, which serve as building blocks for approximating any function in Sobolev spaces. This result expands the class of models known to be universal approximators, potentially enabling new applications in symbolic regression and scientific computing where EML trees offer interpretable and compact representations. The proof uses a 'LEGO block' approach, constructing EML representations for binary operations and elementary functions, and addresses the logarithm's domain issues via sign-based decompositions and affine maps. The paper generalizes the original EML by adding learnable parameters.

reddit · r/MachineLearning · /u/JoeGermany · Jun 29, 11:16

**Background**: The universal approximation theorem states that certain models, like neural networks, can approximate any continuous function to arbitrary accuracy. The EML (Elementary Math Library) function, introduced recently, can represent all elementary functions through composition. This paper proves that tree-structured compositions of EML functions also possess universal approximation properties for Sobolev spaces.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Universal_approximation_theorem">Universal approximation theorem - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2606.23179">[2606.23179] EML Trees Are Universal Approximators - arXiv.org</a></li>
<li><a href="https://arxiv.org/html/2606.23179v1">EML Trees Are Universal Approximators - arXiv.org</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#universal approximation`, `#theory`, `#EML trees`, `#function approximation`

---

<a id="item-12"></a>
## [Ransomware group leaks iPhone 18 Pro data from Apple's India supplier Tata](https://t.me/FinanceNewsDaily/489740) ⭐️ 8.0/10

A ransomware group that stole data from Tata Electronics has published photos of the upcoming iPhone 18 Pro and sensitive supplier information on the dark web. This breach exposes Apple's tightly controlled supply chain and unreleased product details, potentially impacting Apple's security reputation and supplier trust. The leaked files include not only product images but also lists of sensitive components and supplier names. Tata Electronics is both a parts supplier and an iPhone assembler.

telegram · FinanceNewsDaily · Jun 29, 19:45

**Background**: The dark web is a part of the deep web not indexed by standard search engines, often used for illegal activities like data leaks. Ransomware is a type of malware that encrypts a victim's data and demands payment for its release, frequently used by cybercriminals to target corporations.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bbc.com/zhongwen/simp/world-69313893">Telegram... - BBC News 中文</a></li>
<li><a href="https://www.wangan.com/p/7fyg88b9e7ec1092">Akamai...</a></li>

</ul>
</details>

**Tags**: `#supply chain`, `#security breach`, `#Apple`, `#iPhone`, `#ransomware`

---

<a id="item-13"></a>
## [Samsung and SK Hynix Unveil Massive AI Investment Plans](https://t.me/zaihuapd/42235) ⭐️ 8.0/10

Samsung announced a record 1000 trillion won ($648 billion) ten-year spending plan for AI, while SK Hynix plans to double its capacity in five years and raise $29 billion through a US IPO. These investments mark a pivotal shift toward AI-driven infrastructure, potentially transforming the global semiconductor supply chain and bolstering South Korea's economic competitiveness. The announcement is scheduled for a national briefing on June 29, with a focus on semiconductors, AI data centers, and Physical AI. On the same day, Samsung and SK Hynix stocks dropped over 9% due to negative Apple-related news.

telegram · zaihuapd · Jun 29, 07:00

**Background**: Physical AI, as defined by NVIDIA, enables autonomous systems like robots and self-driving cars to perceive, reason, and act in the physical world. The investment surge reflects a global race to build the hardware backbone for such technologies, including AI data centers and robotics.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/glossary/generative-physical-ai/">What is Physical AI? | NVIDIA Glossary</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#AI investment`, `#Samsung`, `#SK Hynix`

---