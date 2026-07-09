---
layout: default
title: "Horizon Summary: 2026-07-09 (EN)"
date: 2026-07-09
lang: en
---

> From 63 items, 12 important content pieces were selected

---

1. [OpenAI Releases GPT-5.6 with Three Sizes, New SOTA on ARC-AGI-3](#item-1) ⭐️ 9.0/10
2. [EU Parliament Passes Chat Control 1.0 Mass Scanning](#item-2) ⭐️ 9.0/10
3. [Postgres rewritten in Rust passes all regression tests](#item-3) ⭐️ 9.0/10
4. [Meta's Superintelligence Update Reveals Stealth RL Startup](#item-4) ⭐️ 9.0/10
5. [TypeScript 7.0 Released with Go Rewrite, Up to 12x Faster Builds](#item-5) ⭐️ 9.0/10
6. [Ant Group Open-Sources LingBot-Video: First MoE Embodied Video Foundation Model](#item-6) ⭐️ 9.0/10
7. [Meta Releases Muse Spark 1.1 Agentic AI Model](#item-7) ⭐️ 8.0/10
8. [Bun Rewritten from Zig to Rust Using AI Agents](#item-8) ⭐️ 8.0/10
9. [OpenAI Launches GPT-Live for ChatGPT Voice Mode](#item-9) ⭐️ 8.0/10
10. [Former Fed Chair Bernanke Joins Anthropic's AI Oversight Trust](#item-10) ⭐️ 8.0/10
11. [DJI EV50 Drone Flies to 8,861m on Everest](#item-11) ⭐️ 8.0/10
12. [National Supercomputing Internet Core Node Goes Live in Zhengzhou](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI Releases GPT-5.6 with Three Sizes, New SOTA on ARC-AGI-3](https://openai.com/index/gpt-5-6/) ⭐️ 9.0/10

OpenAI has released GPT-5.6, its latest frontier model, available in three sizes: Luna, Terra, and Sol. The model achieves a new state-of-the-art score on the ARC-AGI-3 benchmark, with improved intent understanding and image detail preservation. This release marks a significant leap in AI reasoning and agentic capabilities, as GPT-5.6 is the first frontier model verified to beat an ARC-AGI-3 game. The tiered pricing and improved understanding could reshape competitive dynamics in the AI assistant market, particularly against models like Claude Opus and Fable 5. Pricing per 1M tokens is: Luna $1/$6, Terra $2.50/$15, Sol $5/$30. The knowledge cutoff is February 16, 2026. GPT-5.6 can better infer user intent without explicit step-by-step instructions and preserves original image dimensions for improved visual processing.

hackernews · logickkk1 · Jul 9, 17:04 · [Discussion](https://news.ycombinator.com/item?id=48849066)

**Background**: ARC-AGI-3 is an interactive reasoning benchmark that challenges AI agents to explore novel environments, infer goals, and plan actions, measuring human-like intelligence. Frontier models are large-scale, general-purpose AI systems that push the boundaries of capabilities in reasoning, coding, and multimodal tasks. GPT-5.6 is OpenAI's response to increasingly competitive models from Anthropic and other labs.

<details><summary>References</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>
<li><a href="https://arxiv.org/abs/2603.24621">[2603.24621] ARC-AGI-3: A New Challenge for Frontier Agentic Intelligence</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/frontier-models/">What Are Frontier AI Models and How They Work | NVIDIA Glossary</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion shows mixed sentiment: some users praise the new SOTA on ARC-AGI-3 and practical improvements, while others critique OpenAI's lack of openness compared to competitors. Comments also compare GPT-5.6's pricing and capabilities with Claude models, with some users hesitant to switch from established tools like Claude Code.

**Tags**: `#GPT-5.6`, `#OpenAI`, `#large language model`, `#frontier model`, `#ARC-AGI`

---

<a id="item-2"></a>
## [EU Parliament Passes Chat Control 1.0 Mass Scanning](https://www.patrick-breyer.de/en/eu-parliament-greenlights-chat-control-1-0-breyer-our-children-lose-out/) ⭐️ 9.0/10

The European Parliament passed Chat Control 1.0, allowing US tech companies to scan private messages without a warrant until 2028. This was approved despite a majority of MEPs voting against (314 against, 276 in favor, 17 abstentions) because the rejection failed to achieve the required absolute majority of 361 votes. This decision undermines digital privacy and end-to-end encryption, affecting millions of users on platforms like Instagram, Discord, Gmail, and iCloud. It sets a dangerous precedent for mass surveillance and could erode trust in digital communications. The regulation, originally proposed in 2022, had been rejected twice in March 2026 but was revived and fast-tracked in July 2026. The procedural vote required an absolute majority (361 of 720 MEPs) to reject, which failed despite a simple majority opposing it.

hackernews · rapnie · Jul 9, 11:03 · [Discussion](https://news.ycombinator.com/item?id=48843923)

**Background**: Chat Control refers to EU regulations aimed at combating child sexual abuse online by requiring digital platforms to scan private communications. Civil society groups argue this effectively mandates mass surveillance, undermining encryption and privacy. The first version, Chat Control 1.0, was a temporary measure that was set to expire in 2026 but was revived.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control_1.0">Chat Control 1.0</a></li>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control">Chat Control - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community comments strongly criticize the parliamentary procedure as undemocratic, with many accusing the EU of becoming totalitarian. Users highlight that a majority voted against but the law passed due to an absolute majority rule, with 113 MEPs absent on the day before summer break.

**Tags**: `#privacy`, `#EU`, `#surveillance`, `#regulation`, `#messaging`

---

<a id="item-3"></a>
## [Postgres rewritten in Rust passes all regression tests](https://github.com/malisper/pgrust) ⭐️ 9.0/10

A project called pgrust has rewritten PostgreSQL entirely in Rust using LLMs, passing 100% of the official PostgreSQL regression tests. The author, malisper, is now working on a new unpublished version incorporating additional techniques. This demonstrates the feasibility of using LLMs to produce production-quality rewrites of complex systems, potentially accelerating database innovation. However, it also raises important questions about licensing and the trustworthiness of AI-generated code. The project changed the license from the PostgreSQL license to the AGPL, which has sparked debate about compatibility with the original license. The codebase was generated with over 7,100 commits in less than a month via LLMs, making traditional code review impractical.

hackernews · SweetSoftPillow · Jul 9, 06:18 · [Discussion](https://news.ycombinator.com/item?id=48841676)

**Background**: PostgreSQL is a 30-year-old open-source relational database with a permissive license. pgrust is an experimental Rust rewrite using large language models (LLMs) to generate the code, aiming to modernize the database architecture. The change to AGPL means derivative works must also be open-sourced under copyleft terms, which contrasts with the original PostgreSQL license.

<details><summary>References</summary>
<ul>
<li><a href="https://www.techtarget.com/searchenterpriseai/tip/Examining-the-future-of-AI-and-open-source-software">Does AI-generated code violate open source licenses? | TechTarget</a></li>
<li><a href="https://selleo.com/blog/using-ai-to-code-here-s-what-you-must-know-about-copyright-laws">Who Owns AI Generated Code? Copyright, Law & Ownership</a></li>
<li><a href="https://www.redhat.com/en/blog/when-bots-commit-ai-generated-code-open-source-projects">When bots commit: AI-generated code in open source projects</a></li>

</ul>
</details>

**Discussion**: Community comments show skepticism about trusting AI-generated code, with some stating they would never trust it. Others raise concerns about the license change from the PostgreSQL license to AGPL, questioning compatibility. Suggestions include mirroring queries to compare output and performance under real load as a testing method.

**Tags**: `#Postgres`, `#Rust`, `#LLM`, `#database`, `#AI-generated code`

---

<a id="item-4"></a>
## [Meta's Superintelligence Update Reveals Stealth RL Startup](https://newsletter.semianalysis.com/p/the-future-of-meta-superintelligence) ⭐️ 9.0/10

Semianalysis reports that Meta's superintelligence progress update reveals a new top-tier reinforcement learning (RL) environment startup emerging from stealth, an unprecedented compute ramp, and a 2000km+ scale-across infrastructure. This signals a paradigm shift in AI scale, as Meta aggressively invests in both large-scale infrastructure and novel RL environments, potentially accelerating progress toward superintelligence and reshaping competition with Google DeepMind. The RL environment startup emerged from stealth, building simulation platforms for training agents; the compute ramp is described as the most aggressive ever seen; scale-across infrastructure spans over 2000 km linking multiple data centers.

rss · Semianalysis · Jul 9, 19:16

**Background**: Reinforcement learning environments are simulated worlds where AI agents learn through trial and error, crucial for developing general intelligence. Scale-across refers to networking infrastructure that connects compute clusters across geographically distant data centers, enabling massive distributed training.

<details><summary>References</summary>
<ul>
<li><a href="https://www.primeintellect.ai/blog/environments">Environments Hub: A Community Hub To Scale RL To Open AGI</a></li>
<li><a href="https://techcrunch.com/2025/09/21/silicon-valley-bets-big-on-environments-to-train-ai-agents/">Silicon Valley bets big on 'environments' to train AI agents | TechCrunch</a></li>
<li><a href="https://drivenets.com/blog/hybrid-scaling-scale-up-scale-out-and-scale-across-gain-new-meaning/">Scale-Up, Scale-Out, and Scale-Across Gain New Meaning</a></li>

</ul>
</details>

**Tags**: `#AI`, `#superintelligence`, `#Meta`, `#reinforcement learning`, `#infrastructure`

---

<a id="item-5"></a>
## [TypeScript 7.0 Released with Go Rewrite, Up to 12x Faster Builds](https://devblogs.microsoft.com/typescript/announcing-typescript-7-0/) ⭐️ 9.0/10

Microsoft has officially released TypeScript 7.0, a native version rewritten in Go that achieves 8 to 12 times faster full builds and supports shared-memory multithreading. This major performance boost significantly improves developer productivity, especially for large codebases, and demonstrates a trend of rewriting performance-critical tools in lower-level languages like Go. Users can install TypeScript 7.0 via npm, and mainstream editors support the new language server through LSP, but embedded language toolchains for Vue and Svelte still require the previous version due to unready APIs.

telegram · zaihuapd · Jul 9, 04:01

**Background**: TypeScript is a typed superset of JavaScript that compiles to plain JavaScript, widely used for large-scale applications. The Language Server Protocol (LSP) is a standard that enables editors and IDEs to provide language features like code completion and error checking via a language server.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Language_Server_Protocol">Language Server Protocol</a></li>
<li><a href="https://microsoft.github.io/language-server-protocol/">Official page for Language Server Protocol</a></li>

</ul>
</details>

**Tags**: `#TypeScript`, `#Go`, `#性能`, `#编程语言`

---

<a id="item-6"></a>
## [Ant Group Open-Sources LingBot-Video: First MoE Embodied Video Foundation Model](https://www.qbitai.com/2026/07/446458.html) ⭐️ 9.0/10

Ant Group has open-sourced LingBot-Video, the world's first MoE-based embodied video foundation model with 30B total parameters and 3B active parameters, achieving state-of-the-art results on the RBench benchmark. This is significant because it combines Mixture-of-Experts (MoE) with Diffusion Transformer (DiT) for embodied video generation, achieving 3x inference efficiency over dense models, and is released under Apache 2.0, potentially accelerating research in robotics and video generation. The model incorporates a portrait engine with 70,000 hours of embodied data covering dexterous manipulation, robot movement, and first-person interaction, and uses a multi-dimensional reinforcement learning reward system focusing on physical plausibility and task completion.

telegram · zaihuapd · Jul 9, 04:30

**Background**: Mixture-of-Experts (MoE) is an architecture that uses conditional computation, activating only a subset of parameters per input, enabling larger models with similar compute cost. Embodied video foundation models aim to generate videos that understand physical interactions and robot actions, useful for training robotics systems. LingBot-Video is the first such model to apply MoE in this domain.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/mixture-of-experts">What is mixture of experts? | IBM</a></li>

</ul>
</details>

**Tags**: `#MoE`, `#embodied AI`, `#video generation`, `#robotics`, `#open-source`

---

<a id="item-7"></a>
## [Meta Releases Muse Spark 1.1 Agentic AI Model](https://ai.meta.com/blog/introducing-muse-spark-meta-model-api/) ⭐️ 8.0/10

Meta announced the release of Muse Spark 1.1, an agentic AI model with improved coding performance on real-world tasks, and introduced pricing at $1.25/$4.5 per 1M tokens. Muse Spark 1.1 enters the competitive AI coding market, offering a lower-cost alternative to models from OpenAI and Anthropic, which could commoditize coding assistants and pressure other providers. The evaluation methodology has been criticized for overriding default resource caps (6 CPU cores, 8GB RAM) in Terminal-Bench 2.1 tasks, which some argue disqualifies the results. A community member created an LLM plugin for easy terminal access.

hackernews · ot · Jul 9, 14:10 · [Discussion](https://news.ycombinator.com/item?id=48846184)

**Background**: Agentic AI models are AI systems that can autonomously pursue goals, use tools, and execute multi-step tasks, often driven by large language models. Meta previously released Muse Spark in April 2026, and Muse Spark 1.1 is an updated version focused on coding and agentic capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://ai.meta.com/blog/introducing-muse-spark-meta-model-api/">Introducing Muse Spark 1.1</a></li>
<li><a href="https://techcrunch.com/2026/07/09/meta-enters-the-crowded-ai-coding-battle-with-muse-spark-1-1/">Meta enters the crowded AI coding battle with Muse Spark 1.1 | TechCrunch</a></li>
<li><a href="https://ai.meta.com/static-resource/muse-spark-1-1-evaluation-report">Muse Spark 1.1 Evaluation Report</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some praise the practical utility via the LLM plugin and competitive pricing, while others question the fairness of the evaluation benchmarks, particularly the resource cap override. One commenter suggests Meta should focus on open-weight releases to commoditize the market.

**Tags**: `#AI`, `#Meta`, `#Muse Spark`, `#agentic models`, `#evaluation`

---

<a id="item-8"></a>
## [Bun Rewritten from Zig to Rust Using AI Agents](https://simonwillison.net/2026/Jul/8/rewriting-bun-in-rust/#atom-everything) ⭐️ 8.0/10

Jarred Sumner has rewritten the Bun JavaScript runtime from Zig to Rust, leveraging AI agents to automate much of the porting process and using the existing TypeScript test suite as a conformance suite. This rewrite demonstrates that large-scale software rewrites previously considered impractical are now feasible with AI coding agents, and it directly addresses memory safety issues that plagued Bun's Zig implementation. The rewrite cost approximately $165,000 in API tokens (5.9 billion input and 690 million output tokens) and involved adversarial code review. The Rust port has been live in Claude Code since June 17, yielding 10% faster startup on Linux.

rss · Simon Willison · Jul 8, 23:57

**Background**: Bun is a popular JavaScript runtime initially written in Zig, a systems programming language that provides manual memory management. Rust is another systems language that offers memory safety through its ownership system, making it attractive for reducing crashes. The rewrite was enabled by AI agents from Anthropic, which automated the conversion of Zig code to Rust while using Bun's extensive TypeScript test suite to validate correctness.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>

</ul>
</details>

**Tags**: `#bun`, `#rust`, `#zig`, `#javascript-runtime`, `#rewrite`

---

<a id="item-9"></a>
## [OpenAI Launches GPT-Live for ChatGPT Voice Mode](https://simonwillison.net/2026/Jul/8/introducing-gptlive/#atom-everything) ⭐️ 8.0/10

OpenAI has introduced GPT-Live, a new voice model for ChatGPT that can delegate complex tasks to GPT-5.5 in the background while maintaining a fluid conversation. This upgrade significantly improves the voice interaction experience, making ChatGPT a more capable brainstorming partner by leveraging a much more powerful model for reasoning and web search. GPT-Live is built on a full-duplex architecture, allowing it to listen and speak simultaneously, and it will be continuously updated with future frontier models. The previous voice mode was based on an older GPT-4o era model with a 2024 knowledge cut-off.

rss · Simon Willison · Jul 8, 23:20

**Background**: ChatGPT's voice mode allows users to have spoken conversations with the AI. GPT-Live replaces an older model, bringing real-time delegation to GPT-5.5 for tasks requiring deeper reasoning or web access, while the model can continue speaking. Full-duplex means both parties can talk at once, enabling more natural interaction.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/introducing-gpt-live/">Introducing GPT-Live - OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.5">GPT-5.5</a></li>
<li><a href="https://openai.com/index/introducing-gpt-5-5/">Introducing GPT-5.5 - OpenAI</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#GPT-Live`, `#ChatGPT`, `#voice mode`, `#AI`

---

<a id="item-10"></a>
## [Former Fed Chair Bernanke Joins Anthropic's AI Oversight Trust](https://t.me/FinanceNewsDaily/490344) ⭐️ 8.0/10

Former Federal Reserve Chair Ben Bernanke has been appointed as a member of Anthropic's Long-Term Benefit Trust, a body tasked with ensuring the AI company remains accountable to its public mission. This appointment signals increasing attention on AI governance and societal risks, such as job displacement and financial bubbles, from high-profile figures outside the tech industry, potentially influencing policy and public discourse. Bernanke will have the authority to appoint and remove members of Anthropic's board of directors and advise on key decisions related to AI risk and societal impact, including concerns about AI replacing white-collar jobs and fueling financial bubbles.

telegram · FinanceNewsDaily · Jul 9, 16:35

**Background**: Anthropic is an AI safety company known for developing large language models with a focus on responsible AI. The Long-Term Benefit Trust is an oversight mechanism designed to ensure the company prioritizes long-term societal benefit over short-term profits, reflecting growing efforts to institutionalize AI governance.

**Tags**: `#AI governance`, `#Anthropic`, `#societal impact`, `#Ben Bernanke`, `#AI risk`

---

<a id="item-11"></a>
## [DJI EV50 Drone Flies to 8,861m on Everest](https://www.163.com/dy/article/L1CUCV940514R9OJ.html) ⭐️ 8.0/10

DJI's unreleased EV50 vertical takeoff and landing drone set a record by flying to 8,861 meters on Mount Everest during a scientific expedition, becoming the highest-flying VTOL drone in public tests. This achievement demonstrates the potential of drones for high-altitude logistics and scientific data collection, pushing the boundaries of drone capabilities in extreme environments and opening new applications for cargo transport at altitude. The EV50 is a hybrid-wing drone that takes off and lands vertically, then transitions to fixed-wing cruising. During the 12-day mission, it completed 32 sorties, climbed 3,730 meters continuously, and returned with 30% battery remaining.

telegram · zaihuapd · Jul 9, 06:00

**Background**: High-altitude environments like Everest pose extreme challenges for drones, including thin air reducing lift and battery efficiency. DJI's EV50 is designed for vertical takeoff and landing and aims at cargo delivery over 100 km. The 'Peak Mission' scientific expedition collected atmospheric profile data above 8,000 meters.

**Tags**: `#drone`, `#DJI`, `#aviation`, `#Everest`, `#logistics`

---

<a id="item-12"></a>
## [National Supercomputing Internet Core Node Goes Live in Zhengzhou](https://36kr.com/newsflashes/3887797387344387) ⭐️ 8.0/10

On July 9, 2026, the national supercomputing internet core node was launched in Zhengzhou, providing over 100,000 domestic AI computing cards. This is the largest single domestic AI computing power resource pool connected to the national supercomputing internet platform since its launch. This milestone significantly boosts China's domestic AI computing capabilities and advances the national strategy for a unified computing resource network. It enables large-scale AI model training and inference using domestic hardware, reducing reliance on foreign technologies. The core node serves as the central hub for operation management and resource scheduling across the national supercomputing internet, while also integrating supply-demand matching and industry incubation services. The 100,000+ cards represent a massive pool of domestic AI accelerators.

telegram · zaihuapd · Jul 9, 07:00

**Background**: The national supercomputing internet is a Chinese initiative to build a nationwide network connecting major supercomputing centers, enabling efficient allocation of high-performance computing resources. The Zhengzhou node is a key component of this network, aggregating domestic AI computing power for researchers and enterprises. This launch follows the earlier debut of the overall national supercomputing internet platform.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/agentscope-ai/QwenPaw/issues/2312">[Bug]: 无法使用国家超算互联网的api #2312 - QwenPaw - GitHub</a></li>

</ul>
</details>

**Tags**: `#supercomputing`, `#AI infrastructure`, `#China`, `#national computing network`

---