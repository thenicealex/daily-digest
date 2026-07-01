---
layout: default
title: "Horizon Summary: 2026-07-01 (EN)"
date: 2026-07-01
lang: en
---

> From 62 items, 16 important content pieces were selected

---

1. [First Synthetic Cell Built from Scratch Grows and Divides](#item-1) ⭐️ 9.0/10
2. [Box3D: Open Source 3D Physics Engine by Erin Catto](#item-2) ⭐️ 9.0/10
3. [Cloudflare launches monetization gateway with HTTP 402 and stablecoins](#item-3) ⭐️ 9.0/10
4. [arXiv to Become Independent Nonprofit in July 2026](#item-4) ⭐️ 9.0/10
5. [FFmpeg 9.1 Native AAC Encoder Matches Proprietary Quality](#item-5) ⭐️ 8.0/10
6. [Sony to end physical game disc production by January 2028](#item-6) ⭐️ 8.0/10
7. [Interactive Deep Dive into Internal Combustion Engines](#item-7) ⭐️ 8.0/10
8. [Anthropic's Fable 5 Sparks Security and Trust Controversy](#item-8) ⭐️ 8.0/10
9. [US Lifts Export Controls on Anthropic's Claude Fable 5 and Mythos 5](#item-9) ⭐️ 8.0/10
10. [MOTHRAG: Graph-Free Multi-Hop RAG Outperforms Graph-Based Systems](#item-10) ⭐️ 8.0/10
11. [Sentinel Gateway: System-Level Prompt Injection Defense](#item-11) ⭐️ 8.0/10
12. [Claude Code 2.1.91 Secretly Telemetries Proxy and Timezone Data](#item-12) ⭐️ 8.0/10
13. [NVIDIA Slashes DeepSeek V4 Inference Cost to One-Fifth](#item-13) ⭐️ 8.0/10
14. [Visa, Mastercard Lead 140+ Firms in Open Standard Stablecoin Network](#item-14) ⭐️ 8.0/10
15. [ChatGPT weekly users double to 200 million in under a year](#item-15) ⭐️ 8.0/10
16. [Yageo to Hike Capacitor Prices 50% Starting July 1](#item-16) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [First Synthetic Cell Built from Scratch Grows and Divides](https://www.quantamagazine.org/for-the-first-time-a-cell-built-from-scratch-grows-and-divides-20260701/) ⭐️ 9.0/10

Researchers led by Kate Adamala at the University of Minnesota have created SpudCell, a synthetic cell built entirely from non-living chemicals that can grow, replicate its genome, and divide, marking the first time a fully synthetic cell has achieved autonomous growth and division. This breakthrough overcomes a major hurdle in synthetic biology by demonstrating that a cell lacking a cytoskeleton can still divide, opening new possibilities for designing minimal life forms and understanding the fundamental principles of life. It could also lead to applications in biotechnology, such as programmable drug delivery or biosensing. SpudCell forgoes a cytoskeleton, relying instead on a membrane-based mechanism for division. The work was initially rejected by the journal Cell, with one reviewer claiming SpudCells were "not real biology." The manuscript, over 190 pages, was shared with journalists under embargo before being posted on bioRxiv.

hackernews · defrost · Jul 1, 14:20 · [Discussion](https://news.ycombinator.com/item?id=48747304)

**Background**: Synthetic biology aims to build artificial cells from scratch to better understand life's essential components. Previous research had achieved feeding and DNA replication in synthetic cells, but cell division—a complex process typically involving cytoskeletal reorganization—remained a challenge. SpudCell's design bypasses the cytoskeleton entirely, using chemical fusion and division of its lipid membrane.

<details><summary>References</summary>
<ul>
<li><a href="https://www.science.org/content/article/lab-created-spudcell-marks-major-step-toward-building-life-scratch">Lab-created ‘SpudCell’ marks ‘stunning’ step toward building life from scratch | Science | AAAS</a></li>
<li><a href="https://www.nytimes.com/2026/07/01/science/spud-cell-what-to-know.html">SpudCell: Scientists Made a Cell With Most of the Hallmarks of Life. Here’s What to Know. - The New York Times</a></li>

</ul>
</details>

**Discussion**: Comments in the Hacker News thread are mixed. Some users praise the achievement as a major step, while others are skeptical, noting the controversy over the paper's rejection by Cell and the unusual distribution of the manuscript under embargo before peer review. A user points out that the actual science is impressive but the publicity tactics have drawn criticism.

**Tags**: `#synthetic biology`, `#cell division`, `#biotechnology`, `#research`, `#breakthrough`

---

<a id="item-2"></a>
## [Box3D: Open Source 3D Physics Engine by Erin Catto](https://box2d.org/posts/2026/06/announcing-box3d/) ⭐️ 9.0/10

Erin Catto announced Box3D, a new open-source 3D physics engine, building on the success of his widely-used Box2D library. Box3D could become a foundational tool for indie game development, reinforcement learning environments, and simulation, given Box2D's legacy and the community's enthusiasm. The announcement did not specify determinism support, a topic of interest for networked applications, but the engine is expected to evolve with community input.

hackernews · makepanic · Jul 1, 12:12 · [Discussion](https://news.ycombinator.com/item?id=48745445)

**Background**: Box2D is a free and open-source 2D rigid body physics engine created by Erin Catto, used in games like Angry Birds and in ML frameworks like Gymnasium for reinforcement learning benchmarks. Box3D extends similar rigid body dynamics and collision detection principles into three dimensions, aiming to provide fast and accurate physics simulation for developers.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Box2D">Box2D</a></li>
<li><a href="https://box2d.org/">Box2D</a></li>

</ul>
</details>

**Discussion**: Commenters expressed excitement, recalling Box2D's impact on indie games and RL. Some raised questions about determinism for multiplayer, while ML researchers highlighted Box2D's role in standard RL benchmarks.

**Tags**: `#physics engine`, `#open source`, `#game development`, `#simulation`, `#machine learning`

---

<a id="item-3"></a>
## [Cloudflare launches monetization gateway with HTTP 402 and stablecoins](https://blog.cloudflare.com/monetization-gateway/) ⭐️ 9.0/10

Cloudflare announced a monetization gateway that allows website operators to charge for any resource behind their Cloudflare network using the HTTP 402 status code and stablecoins like USDC. This feature enables seamless microtransactions for web content and APIs, potentially transforming the economics of the internet by integrating cryptocurrency payments directly into the HTTP protocol. The gateway implements the x402 open standard, which repurposes the long-unused HTTP 402 'Payment Required' status code. Cloudflare handles the payment processing, allowing operators to set prices per request without managing their own payment infrastructure.

hackernews · soheilpro · Jul 1, 13:59 · [Discussion](https://news.ycombinator.com/item?id=48746914)

**Background**: HTTP 402 was defined in the original HTTP specification but never widely adopted due to the lack of a standard payment protocol. The x402 standard revives it by specifying a lightweight payment flow using cryptocurrencies or fiat. Cloudflare’s gateway builds on this standard, providing a turnkey solution for monetizing any resource.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/X402">X402</a></li>
<li><a href="https://www.x402.org/">x402 - Payment Required | Internet-Native Payments Standard</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Status/402">402 Payment Required - HTTP | MDN</a></li>

</ul>
</details>

**Discussion**: Commenters are excited about the potential for agent-driven microtransactions, but also raise significant concerns: legal and regulatory hurdles (invoicing, VAT, compliance), the challenge of distinguishing bots from humans, and potential conflicts with emerging web bot authentication standards.

**Tags**: `#monetization`, `#microtransactions`, `#cloudflare`, `#web payments`, `#api`

---

<a id="item-4"></a>
## [arXiv to Become Independent Nonprofit in July 2026](https://www.reddit.com/r/MachineLearning/comments/1ukjtlm/on_july_1_2026_arxiv_will_spin_out_from_cornell/) ⭐️ 9.0/10

arXiv announced it will spin out from Cornell University on July 1, 2026, becoming an independent nonprofit organization with major funding from the Simons Foundation and Schmidt Sciences. This structural change ensures arXiv's long-term sustainability and independence, which is crucial for the global research community that relies on it for open-access preprint distribution. The spin-out includes a website redesign ('ditching the red') and new governance structure, while Cornell will continue to provide transitional support.

reddit · r/MachineLearning · /u/Nunki08 · Jul 1, 12:07

**Background**: arXiv is a free preprint repository founded in 1991, hosted at Cornell University since 2001. It has become a cornerstone of academic communication in physics, mathematics, computer science, and related fields, with over two million preprints.

**Tags**: `#arXiv`, `#open access`, `#scholarly publishing`, `#research infrastructure`

---

<a id="item-5"></a>
## [FFmpeg 9.1 Native AAC Encoder Matches Proprietary Quality](https://hydrogenaudio.org/index.php/topic,129691.0.html) ⭐️ 8.0/10

FFmpeg 9.1 introduces a major update to its native AAC encoder, achieving competitive audio quality with proprietary encoders and fixing long-standing bugs like stereo PNS artifacts. This update makes FFmpeg a viable all-in-one solution for AAC encoding without relying on external libraries, benefiting the open-source community and users who need high-quality audio encoding. The encoder is optimized for 48 kHz audio, though other sample rates are supported with potentially lower quality; it avoids a known bug in AAC decoders related to stereo Perceptual Noise Substitution (PNS).

hackernews · ledoge · Jul 1, 14:10 · [Discussion](https://news.ycombinator.com/item?id=48747116)

**Background**: AAC (Advanced Audio Coding) is a widely used lossy audio compression standard. FFmpeg's native AAC encoder, developed by Rostislav Pehlivanov and Claudio Freire, has matured to compete with encoders like Apple's Core Audio and Fraunhofer FDK, providing a free alternative for high-quality encoding.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Advanced_Audio_Coding">Advanced Audio Coding - Wikipedia</a></li>
<li><a href="https://ffmpeg.org/ffmpeg-codecs.html">FFmpeg Codecs Documentation</a></li>
<li><a href="https://ffmpeg.org/index.html#aac_encoder_stable">FFmpeg</a></li>

</ul>
</details>

**Discussion**: Community comments highlight that Opus outperforms all AAC encoders even at 64 kbps, and note the encoder's subjective tuning based on the developer's ears. Some users express relief over fixing the annoying chirping artifacts and adoption of 48 kHz as standard.

**Tags**: `#FFmpeg`, `#AAC`, `#audio encoding`, `#open source`, `#codec`

---

<a id="item-6"></a>
## [Sony to end physical game disc production by January 2028](https://blog.playstation.com/2026/07/01/physical-disc-production-ending-in-january-2028-for-new-games-releasing-on-playstation-consoles/) ⭐️ 8.0/10

Sony announced that production of physical game discs for PlayStation will cease by January 2028, making new games available only through digital download on its consoles. This marks a major industry shift towards all-digital distribution, raising concerns about game ownership, preservation, and the future of physical media in gaming. The cut-off applies only to new game releases; existing physical discs will remain playable and some special editions may still include physical items without discs. Sony's decision follows similar moves by Microsoft and Nintendo in recent years.

hackernews · Tiberium · Jul 1, 12:13 · [Discussion](https://news.ycombinator.com/item?id=48745456)

**Background**: Physical game discs have been a cornerstone of console gaming for decades, allowing players to buy, sell, and share games. The shift to digital has accelerated with faster internet and larger storage, but many gamers value ownership and resale potential. Game preservationists worry that digital-only futures will lead to lost titles when servers shut down.

**Discussion**: Community comments strongly criticize the move, citing Sony's recent removal of purchased movies from customer libraries as a breach of trust. Many argue digital games are merely rentals, and the end of physical media threatens long-term game preservation and fair pricing.

**Tags**: `#gaming`, `#PlayStation`, `#digital rights`, `#physical media`, `#game preservation`

---

<a id="item-7"></a>
## [Interactive Deep Dive into Internal Combustion Engines](https://ciechanow.ski/internal-combustion-engine/) ⭐️ 8.0/10

A detailed interactive tutorial on internal combustion engines was published, featuring beautifully illustrated mechanics and engineering explanations. This high-quality educational resource makes complex mechanical engineering accessible to a broad audience, and its interactive design enhances understanding of engine operations. The article covers the four-stroke cycle, lubrication, and control systems, with modern electronic fuel injection discussed alongside historical carburetors. The content is praised for its clarity and depth.

hackernews · StefanBatory · Jul 1, 13:04 · [Discussion](https://news.ycombinator.com/item?id=48746076)

**Background**: Internal combustion engines convert fuel and air into mechanical energy through controlled explosions in cylinders. They have powered vehicles for over a century, with recent advances focusing on electronic control for efficiency and emissions.

**Discussion**: Commenters noted that while engine mechanics have remained similar for decades, modern control systems like electronic fuel injection have drastically improved. Some shared personal experiences with engine wear and hydrodynamic lubrication effects.

**Tags**: `#internal combustion engine`, `#interactive tutorial`, `#engineering`, `#mechanical engineering`, `#educational content`

---

<a id="item-8"></a>
## [Anthropic's Fable 5 Sparks Security and Trust Controversy](https://twitter.com/claudeai/status/2072402636813607381) ⭐️ 8.0/10

Anthropic launched Claude Fable 5 on June 9, 2026, but days later the US government classified it as a dangerous munition, restricting access for foreign nationals. The model has faced criticism for overly aggressive safety restrictions that render it unusable for legitimate tasks. This controversy highlights the growing tension between AI safety measures and practical usability, and erodes trust in AI companies that implement heavy-handed restrictions. The classification of a commercial AI model as a munition sets a precedent that could reshape global AI governance. Fable 5 is a 'Mythos-class' model that Anthropic claims is the highest-scoring on FrontierBench. However, it blocks offensive-cyber queries and falls back to Opus 4.8, and users have found ways to bypass restrictions by rephrasing requests.

hackernews · mfiguiere · Jul 1, 19:35 · [Discussion](https://news.ycombinator.com/item?id=48752030)

**Background**: Anthropic developed Fable 5 as a highly capable AI model with built-in safeguards to prevent misuse. The US government's swift classification under export control laws reflects national security concerns. Critics argue that such restrictions make the model practically useless for many legitimate applications, and raise questions about the unchecked power of AI companies to gatekeep advanced AI.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://www.wired.com/story/anthropic-added-a-new-security-measure-to-get-back-into-the-trump-administrations-good-graces/">Anthropic Added a New Security Measure to Get Back Into... | WIRED</a></li>
<li><a href="https://www.schneier.com/blog/archives/2026/06/anthropics-fable-and-the-state-of-ai.html">Anthropic's Fable and the State of AI - Schneier on Security</a></li>

</ul>
</details>

**Discussion**: Community sentiment is largely negative, with users like pkoird calling the model 'hilariously bad' and 'defanged to malice.' Others express distrust in US-based AI models and predict an erosion of trust that may not recover. Some users suggest using the model for planning rather than code generation to minimize token costs.

**Tags**: `#AI safety`, `#Anthropic`, `#model security`, `#trust`, `#community discussion`

---

<a id="item-9"></a>
## [US Lifts Export Controls on Anthropic's Claude Fable 5 and Mythos 5](https://simonwillison.net/2026/Jun/30/anthropic/#atom-everything) ⭐️ 8.0/10

Anthropic announced that the U.S. Department of Commerce has lifted export controls on its advanced AI models Claude Fable 5 and Mythos 5, and will begin restoring access tomorrow. This policy change enables broader global availability of powerful AI models, impacting competition and regulation in the AI industry. Claude Fable 5 is a coding-focused model for complex software development tasks, while Mythos 5 is designed for cybersecurity vulnerability discovery and exploitation.

rss · Simon Willison · Jun 30, 23:58

**Background**: Export controls on advanced AI models are imposed by the U.S. government to prevent sensitive technology from reaching adversaries. Anthropic develops large language models with a focus on safety. The lifting of controls indicates a reassessment of risks associated with these specific models.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bbc.com/news/articles/cdr42623e1do">Fable and Mythos : Anthropic says US lifts export ban on its advanced...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Fable_5">Claude Fable 5</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mythos_5">Mythos 5</a></li>

</ul>
</details>

**Tags**: `#anthropic`, `#claude`, `#export-controls`, `#ai`, `#generative-ai`

---

<a id="item-10"></a>
## [MOTHRAG: Graph-Free Multi-Hop RAG Outperforms Graph-Based Systems](https://www.reddit.com/r/MachineLearning/comments/1ukotww/p_mothretrieval_graphfree_multihop_retrieval_via/) ⭐️ 8.0/10

Researchers have open-sourced MOTHRAG, a graph-free multi-hop retrieval-augmented generation framework that achieves superior accuracy on HotpotQA, 2WikiMultiHopQA, and MuSiQue compared to graph-based systems like GraphRAG, HippoRAG, and RAPTOR, while enabling low-cost updates without rebuilding. This approach challenges the prevailing assumption that knowledge graphs are necessary for multi-hop RAG, offering a cheaper and more flexible alternative for applications with frequently changing data, such as news or internal documents. MOTHRAG uses a graph-free dense index with query-time orchestration, costing approximately $0.03 per query on commodity APIs without needing a GPU. It matches or beats graph-based systems on most benchmarks but lags on MuSiQue due to retrieval recall bottlenecks.

reddit · r/MachineLearning · /u/Annual-Commercial563 · Jul 1, 15:26

**Background**: Multi-hop retrieval-augmented generation (RAG) requires answering questions that need connecting multiple pieces of information. Traditional approaches build a knowledge graph offline to capture entity relationships, but updating the graph requires re-indexing the entire corpus, which is expensive. MOTHRAG avoids this by using a dense vector index and orchestrating retrieval steps at query time.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/juliangeymonat-jpg/mothrag">GitHub - juliangeymonat-jpg/mothrag: Deterministic agentic ...</a></li>
<li><a href="https://arxiv.org/abs/2405.14831">[2405.14831] HippoRAG: Neurobiologically Inspired Long-Term ... GitHub - ianliuwd/HippoRAG2: [NeurIPS'24] HippoRAG is a novel ... HippoRAG: Neurobiologically Inspired Long-Term Memory for ... hipporag · PyPI HippoRAG | Proceedings of the 38th International Conference ... [2502.14802] From RAG to Memory: Non-Parametric Continual ...</a></li>
<li><a href="https://microsoft.github.io/graphrag/">Welcome - GraphRAG</a></li>

</ul>
</details>

**Discussion**: No community comments were provided in the input; the original Reddit post invites feedback from users running RAG on frequently changing data.

**Tags**: `#multi-hop RAG`, `#retrieval-augmented generation`, `#knowledge graph`, `#open source`, `#NLP`

---

<a id="item-11"></a>
## [Sentinel Gateway: System-Level Prompt Injection Defense](https://www.reddit.com/r/MachineLearning/comments/1ukgwk1/a_systemlevel_approach_to_prompt_injection/) ⭐️ 8.0/10

A new middleware layer called Sentinel Gateway enforces strict separation between instruction and data channels in LLM agent systems, using token-based authorization to prevent prompt injection attacks. Prompt injection remains a critical security flaw in LLM agents, and this system-level approach offers a structural fix rather than relying on imperfect input filtering, potentially improving safety in production agentic workflows. The implementation is built as FastAPI middleware, utilizes signed and scoped runtime authorization tokens for tool execution, and includes a Streamlit interface for inspection and audit logging.

reddit · r/MachineLearning · /u/vagobond45 · Jul 1, 09:34

**Background**: Prompt injection attacks occur when an LLM processes untrusted external data that contains malicious instructions, because the model cannot reliably separate its original instructions from the injected data. This is fundamentally difficult because instructions and data share the same embedding space in LLMs.

<details><summary>References</summary>
<ul>
<li><a href="https://aihaberleri.org/en/news/breakthrough-ai-security-tool-blocks-prompt-injection-without-content-scanning">Breakthrough AI Security Tool Blocks Prompt Injection Without...</a></li>
<li><a href="https://sentinel-gateway.com/?ref=producthunt">Sentinel Gateway — Structural AI Agent Security</a></li>

</ul>
</details>

**Tags**: `#prompt injection`, `#LLM security`, `#middleware`, `#agentic workflow`, `#systems design`

---

<a id="item-12"></a>
## [Claude Code 2.1.91 Secretly Telemetries Proxy and Timezone Data](https://t.me/zaihuapd/42285) ⭐️ 8.0/10

A reverse engineer discovered that Claude Code version 2.1.91 silently checks the system timezone and proxy settings to detect Chinese users, encoding this information into the system prompt sent to Anthropic's API. Anthropic acknowledged the issue and promised a fix. This revelation raises significant privacy concerns about covert data collection in widely-used AI coding tools, potentially eroding trust among developers. It also highlights the risk of hidden geopolitical targeting in AI-assisted software development. The tool checks if the timezone is set to Asia/Shanghai or Asia/Urumqi and if the proxy URL points to Chinese domains or AI labs, then encodes the result by subtly altering Unicode characters in the system prompt's date format. This data exfiltration occurred for at least three months before discovery.

telegram · zaihuapd · Jul 1, 04:42

**Background**: Claude Code is Anthropic's agentic coding tool that helps developers edit files and run commands in the terminal. System prompts are instructions given to the AI model to set context for its responses. Detecting Chinese users may relate to compliance with export controls or usage policies, but secret telemetry violates user privacy expectations.

<details><summary>References</summary>
<ul>
<li><a href="https://www.techtimes.com/articles/319415/20260701/claude-code-hid-proxy-fingerprints-system-prompts-anthropic-promises-fix.htm">Claude Code Hid Proxy Fingerprints in System Prompts: Anthropic Promises Fix</a></li>
<li><a href="https://docs.anthropic.com/en/docs/claude-code/overview">Claude Code overview - Anthropic</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#AI`, `#Claude Code`, `#telemetry`, `#reverse engineering`

---

<a id="item-13"></a>
## [NVIDIA Slashes DeepSeek V4 Inference Cost to One-Fifth](https://blogs.nvidia.com/blog/inference-software-lowest-token-cost/) ⭐️ 8.0/10

NVIDIA's inference software stack on the Blackwell platform achieved a 5x reduction in token cost for DeepSeek V4, with SGLang engine throughput increasing from about 2,200 to 11,200 tokens/second/GPU between April and June 2025. This significant cost reduction makes large-scale AI inference more economical, directly lowering operational expenses for enterprises deploying LLMs. It also demonstrates NVIDIA's continued dominance in optimizing both hardware and software for AI workloads. The optimization involves kernel fusion, memory compression, quantization precision paths, and improved memory budgeting with interruptible computation graphs. NVIDIA projects up to 20x system-level throughput gains with future advanced optimizations like disaggregated serving and multi-token prediction.

telegram · zaihuapd · Jul 1, 10:36

**Background**: Large language model inference cost is often measured in tokens per second per GPU; reducing this directly impacts deployment economics. SGLang is a popular open-source LLM inference engine used in production. Disaggregated serving separates prefill and decode phases for better resource utilization, while multi-token prediction trains models to predict multiple future tokens simultaneously, improving inference efficiency.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/sgl-project/sglang">GitHub - sgl-project/ sglang : SGLang is a high-performance serving...</a></li>
<li><a href="https://docs.nvidia.com/dynamo/user-guides/disaggregated-serving">Disaggregated Serving | NVIDIA Dynamo Documentation</a></li>

</ul>
</details>

**Tags**: `#NVIDIA`, `#DeepSeek V4`, `#AI Inference`, `#Blackwell`, `#Performance Optimization`

---

<a id="item-14"></a>
## [Visa, Mastercard Lead 140+ Firms in Open Standard Stablecoin Network](https://www.reuters.com/business/consortium-including-visa-mastercard-jointly-launch-new-global-stablecoin-2026-06-30/) ⭐️ 8.0/10

On June 30, 2026, a consortium of over 140 companies including Visa, Mastercard, and Coinbase announced the launch of Open Standard, a new stablecoin network. They plan to release Open USD (OUSD) later this year, which will allow businesses to mint and redeem tokens for free, with reserve income shared among partners. This initiative signals major institutional adoption of stablecoins beyond crypto trading, aiming to create an open, low-cost infrastructure for global payments. With backing from payment giants and a shared revenue model, it could accelerate stablecoin use in everyday commerce and challenge existing closed-loop systems. Open Standard is positioned as a neutral, collectively governed entity; Open USD will be issued on a network of regulated partners, with DBS Bank and Tempo mentioned as initial participants. The consortium includes a diverse set of firms from payments, tech, and finance, indicating broad industry support.

telegram · zaihuapd · Jul 1, 11:06

**Background**: Stablecoins are cryptocurrencies pegged to stable assets like the US dollar, commonly used for crypto trading but not yet mainstream in payments. The GENIUS Act, signed into US law in 2025, established a federal regulatory framework for payment stablecoins, providing legal clarity for such initiatives.

<details><summary>References</summary>
<ul>
<li><a href="https://www.forbes.com/sites/christiancatalini/2026/06/30/why-an-open-standard-will-win-the-stablecoin-race/">Why An Open Standard Will Win The Stablecoin Race</a></li>
<li><a href="https://www.theblock.co/post/406736/visa-stripe-coinbase-join-open-usd-stablecoin-shares-reserve-revenue">Visa, Stripe, Coinbase and more join Open USD stablecoin that shares reserve revenue | The Block</a></li>
<li><a href="https://en.wikipedia.org/wiki/GENIUS_Act">GENIUS Act - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#stablecoins`, `#payments`, `#Visa`, `#Mastercard`, `#blockchain`

---

<a id="item-15"></a>
## [ChatGPT weekly users double to 200 million in under a year](https://t.me/zaihuapd/42298) ⭐️ 8.0/10

OpenAI announced that ChatGPT now has over 200 million weekly active users, doubling the 100 million reported in November 2023. This milestone highlights ChatGPT's rapid mainstream adoption and its dominance in the generative AI market, with 92% of Fortune 500 companies using OpenAI products. The growth is fueled by the release of GPT-4o Mini, a cheaper and more intelligent model, which doubled API usage. Companies like Apple and Nvidia are rumored to be potential investors in OpenAI's next funding round.

telegram · zaihuapd · Jul 1, 13:01

**Background**: ChatGPT is a conversational AI chatbot developed by OpenAI, launched in November 2022. It gained rapid popularity, reaching 100 million monthly users within two months. GPT-4o Mini, released in July 2024, is a smaller version of GPT-4o that replaced GPT-3.5 Turbo, offering improved performance at lower cost.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-4o_mini">GPT-4o mini</a></li>
<li><a href="https://www.linkedin.com/posts/harness-ai_say-hello-to-gpt-4o-mini-openai-has-activity-7219978703345192961-VYB6">Say hello to GPT - 4 o mini OpenAI has just launched their latest...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#ChatGPT`, `#OpenAI`, `#adoption`, `#enterprise`

---

<a id="item-16"></a>
## [Yageo to Hike Capacitor Prices 50% Starting July 1](https://www.trendforce.com/news/2026/07/01/news-passive-component-prices-rise-as-yageo-reportedly-begins-broadest-capacitor-hike-in-years-on-july-1/) ⭐️ 8.0/10

Taiwan-based passive component maker Yageo announced a broad price increase of approximately 50% across its entire capacitor product line, including MLCC, aluminum electrolytic, and tantalum capacitors, effective July 1, 2026. This price hike, driven by rising geopolitical, energy, and raw material costs, reflects intensifying demand from AI servers and electric vehicles, which are consuming more high-end passive components. As Yageo's first price increase directly for over half of its customers, it could significantly boost the company's revenue and profit margins while potentially triggering industry-wide adjustments. Spot market prices for high-end capacitors have surged nearly tenfold in the past month, while official quotes see a ~50% rise. Capacitors account for about half of Yageo's revenue, and this is the first time Yageo has raised prices directly for more than half of its customers.

telegram · zaihuapd · Jul 1, 14:34

**Background**: Passive components, such as capacitors, resistors, and inductors, are essential electronic parts that do not amplify or generate energy but are critical for circuit stability. MLCC (Multi-layer Ceramic Capacitor) is a common capacitor type made of stacked ceramic layers, widely used in electronics. Yageo is a major global supplier of passive components, and its MLCC products compete with Japanese and Korean manufacturers.

<details><summary>References</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/349101940">MLCC是什么，其特点和作用是什么？ - 知乎</a></li>

</ul>
</details>

**Tags**: `#capacitors`, `#price increase`, `#supply chain`, `#AI hardware`, `#passive components`

---