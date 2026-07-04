---
layout: default
title: "Horizon Summary: 2026-07-04 (EN)"
date: 2026-07-04
lang: en
---

> From 46 items, 9 important content pieces were selected

---

1. [Google Books $200k Bounty for All Scans](#item-1) ⭐️ 9.0/10
2. [YouTube private video leak via crafted link](#item-2) ⭐️ 8.0/10
3. [Claude Code session leakage report sparks security debate](#item-3) ⭐️ 8.0/10
4. [Newer Claude Models Invent Extra Fields in Tool Calls, Causing Rejection](#item-4) ⭐️ 8.0/10
5. [USAF: Sparse Fine-Tuning for MoE Models on Consumer GPUs](#item-5) ⭐️ 8.0/10
6. [BaryGraph: Knowledge Graph with Embedded Relationships as Documents](#item-6) ⭐️ 8.0/10
7. [Huawei Updates 'Tao's Law' Paper with Engineering Details and Data](#item-7) ⭐️ 8.0/10
8. [iOS 27 introduces Trust Insights anti-fraud feature](#item-8) ⭐️ 8.0/10
9. [South Korea Plans $518B Semiconductor Cluster, Double DRAM Output](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Google Books $200k Bounty for All Scans](https://software.annas-archive.gl/AnnaArchivist/annas-archive/-/work_items/234) ⭐️ 9.0/10

A $200,000 bounty has been offered on Anna's Archive for the complete collection of Google Books digitized scans, aiming to make them freely accessible. This bounty underscores the ongoing tension between copyright restrictions and open access to knowledge, potentially impacting digital libraries, researchers, and readers worldwide. The bounty is posted on Anna's Archive, a shadow library project, and targets the complete Google Books corpus, which includes millions of digitized books.

hackernews · Cider9986 · Jul 4, 16:51 · [Discussion](https://news.ycombinator.com/item?id=48786838)

**Background**: Google Books is a service that scans and indexes books from libraries and publishers, but full access is often restricted by copyright. Anna's Archive and similar projects like Z-Library operate in legal gray areas to provide free access to digitized books.

**Discussion**: Commenters expressed gratitude for Anna's Archive and Z-Library, with one user highlighting how it enabled access to books in a country with limited English selections. Another shared info about their rare book translation project. Discussion also touched on bounties for internet scrapes due to Cloudflare restrictions.

**Tags**: `#digital libraries`, `#open access`, `#data archiving`, `#Google Books`, `#piracy`

---

<a id="item-2"></a>
## [YouTube private video leak via crafted link](https://javoriuski.com/post/youtube) ⭐️ 8.0/10

A security researcher discovered a vulnerability that leaks YouTube creators' private video titles when they click a specially crafted link, such as a comment containing a malicious URL. This vulnerability affects all YouTube creators with private videos, potentially exposing sensitive content to attackers. It highlights ongoing privacy risks on major platforms and the challenge of prompt injection attacks. The researcher demonstrated the attack by posting a comment with a crafted link; when the creator clicked it in YouTube Studio, the attacker received the private video's title in the response. The exploit leverages YouTube's own suggested AI prompts in the comment moderation interface.

hackernews · javxfps · Jul 4, 16:45 · [Discussion](https://news.ycombinator.com/item?id=48786781)

**Background**: YouTube offers three visibility settings: public, unlisted, and private. Private videos can only be viewed by the creator and specific users. The leaked vulnerability bypasses this restriction by tricking creators into interacting with a malicious link within the official YouTube Studio interface. This type of attack is known as prompt injection, where attacker-controlled input is processed by an AI system.

<details><summary>References</summary>
<ul>
<li><a href="https://apisecurity.io/issue-265-youtube-api-privacy-bug-medical-records-leaked-openapi-news-spring-boot-api-impacts-volkswagen/">Issue 265: YouTube API privacy bug, Medical records leaked ...</a></li>
<li><a href="https://news.inventrium.net/researcher-exposes-youtube-email-leak-vulnerability/">Researcher Exposes YouTube Email Leak Vulnerability - Inventrium...</a></li>

</ul>
</details>

**Discussion**: The community praised the article for its clear and concise reporting. A former Google engineer provided insight into why YouTube may handle the bug slowly, explaining that it likely went to the original feature engineer who has already moved on. Other commenters criticized YouTube for not treating prompt injection as a security bug.

**Tags**: `#security`, `#vulnerability`, `#youtube`, `#privacy`

---

<a id="item-3"></a>
## [Claude Code session leakage report sparks security debate](https://github.com/anthropics/claude-code/issues/74066) ⭐️ 8.0/10

A GitHub issue on the Claude Code repository reports a potential session or cache leakage between workspace instances, where a user claims to have seen responses from other users' contexts. If confirmed, this could represent a serious data privacy breach affecting all Claude Code users, but the debate over whether it's a hallucination highlights challenges in diagnosing LLM behavior. The reporter used a throwaway account and described seeing a pathname containing 'minecraft.py' from another session; the Claude Code team responded that they believe it is a hallucination and are investigating.

hackernews · chatmasta · Jul 4, 14:03 · [Discussion](https://news.ycombinator.com/item?id=48785485)

**Background**: Claude Code is Anthropic's AI-powered coding assistant that operates within workspace instances, each isolated for different projects or users. Large language models like Claude can occasionally 'hallucinate' — produce plausible but factually incorrect outputs — especially with large context windows. The reported incident involves claims of cross-tenant data leakage, which if real would be a security flaw, but the similarity to known hallucination patterns suggests it may not be a genuine leak.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://docs.secureauth.com/iam/capability-workspace-isolation">Workspace isolation | SecureAuth Connect Product Docs</a></li>

</ul>
</details>

**Discussion**: Community comments are divided: some users report similar experiences across different LLM providers (e.g., Gemini), while others argue it is likely a hallucination due to large context or cache collisions. An official response from the Claude Code team states they are confident it is a hallucination and are looking into it.

**Tags**: `#security`, `#data leakage`, `#LLM`, `#hallucination`, `#Claude Code`

---

<a id="item-4"></a>
## [Newer Claude Models Invent Extra Fields in Tool Calls, Causing Rejection](https://simonwillison.net/2026/Jul/4/better-models-worse-tools/#atom-everything) ⭐️ 8.0/10

Newer Claude models (Opus 4.8, Sonnet 5) sometimes invent extra fields in the nested `edits[]` array when calling Pi's edit tool, causing Pi to reject the tool call. This regression is not observed in older Claude models. This regression degrades the reliability of third-party coding harnesses that rely on precise tool call schemas, highlighting a trade-off where model improvements for first-party tools can harm compatibility with custom tools. Developers building AI-powered tools need to account for model-specific quirks. The issue specifically affects the nested `edits[]` array in tool call arguments, where the model invents keys not present in the schema. Armin Ronacher theorizes that Anthropic's reinforcement learning optimized the models for Claude Code's built-in edit tool, inadvertently causing incorrect usage of Pi's custom edit tool.

rss · Simon Willison · Jul 4, 22:53

**Background**: Large language models can be augmented with tools by defining a schema that specifies the function's parameters. When the model calls a tool, it must generate arguments that exactly match that schema. Claude has a built-in text editor tool using search-and-replace, while OpenAI Codex uses an apply_patch mechanism. Third-party harnesses like Pi define their own custom edit tools, which may not align with the model's fine-tuning.

<details><summary>References</summary>
<ul>
<li><a href="https://platform.claude.com/docs/en/agents-and-tools/tool-use/implement-tool-use">How to implement tool use - Claude API Docs</a></li>
<li><a href="https://sunpeak.ai/blogs/claude-connector-tool-design/">Designing Claude Connector Tools: Schemas, Descriptions, and Patterns for Reliable Tool Calls (May 2026) - sunpeak</a></li>

</ul>
</details>

**Tags**: `#AI`, `#LLM`, `#tool-use`, `#reliability`, `#model regression`

---

<a id="item-5"></a>
## [USAF: Sparse Fine-Tuning for MoE Models on Consumer GPUs](https://www.reddit.com/r/MachineLearning/comments/1unl62q/if_your_gpu_can_run_inference_it_should_be_able/) ⭐️ 8.0/10

The author introduces USAF, a novel sparse fine-tuning method that enables fine-tuning of Mixture-of-Experts (MoE) models on GPUs with limited VRAM that previously could only run inference. For instance, a Qwen3-30B-A3B model can be fine-tuned on an AMD RX 6750 XT with 12 GB VRAM by training sparse expert weights and the router instead of using adapters like LoRA. This democratizes fine-tuning of large MoE models, which are typically resource-intensive, by making it accessible to users with consumer-grade GPUs. It could spur more experimentation and customization of state-of-the-art models like Mixtral or GPT-4-like architectures in resource-constrained settings. USAF fine-tunes only sparse expert weights and the router, significantly reducing memory usage compared to full fine-tuning or adapter-based methods. The project is fully open-source under Apache 2.0, with no commercial intent, and is available on GitHub at https://github.com/tsuyu122/usaf.

reddit · r/MachineLearning · /u/tsuyu122 · Jul 4, 21:56

**Background**: Mixture-of-Experts (MoE) models activate only a subset of parameters per input, making them efficient for inference but challenging to fine-tune due to memory constraints. Traditional fine-tuning methods like LoRA add trainable adapters, but still require significant VRAM. USAF leverages the sparse structure of MoE to update only a fraction of parameters, enabling fine-tuning on GPUs that previously could only handle inference.

<details><summary>References</summary>
<ul>
<li><a href="https://ai.plainenglish.io/how-mixture-of-experts-moe-language-models-work-342b0db571c8">How Mixture of Experts ( MoE ) Language Models Work?</a></li>
<li><a href="https://aplicar.ai/ai-glossary/mixture-of-experts-moe/">Mixture of Experts ( MoE ) - Learn & Apply AI</a></li>

</ul>
</details>

**Tags**: `#fine-tuning`, `#MoE`, `#sparse training`, `#GPU`, `#open-source`

---

<a id="item-6"></a>
## [BaryGraph: Knowledge Graph with Embedded Relationships as Documents](https://www.reddit.com/r/MachineLearning/comments/1un3lsf/barygraph_knowledge_graph_where_every/) ⭐️ 8.0/10

BaryGraph introduces BaryEdges, where each relationship in a knowledge graph is a first-class embedded document rather than a simple edge, enabling structural bridging across unrelated concepts. It has been demonstrated on the full English Wiktionary with 6.6M documents. This approach addresses a fundamental limitation of traditional vector search and RAG systems, which fail to capture cross-domain structural connections. If validated, it could significantly improve knowledge retrieval and reasoning in AI systems. BaryGraph uses a recursive triad hierarchy (MetaBary) built from algebraic combinations of BaryEdge vectors, with zero additional embedding calls beyond base level. It runs locally on MongoDB Community + mongot + nomic-embed-text, and takes 8–14 hours to build the full graph on a single workstation.

reddit · r/MachineLearning · /u/adseipsum · Jul 4, 08:24

**Background**: Traditional knowledge graphs represent relationships as edges between nodes, and vector search retrieves information based on proximity of embeddings, but this discards structural information. Reification is a technique that makes relationships first-class entities, allowing metadata and complex semantics to be captured. The Model Context Protocol (MCP) is a standard for connecting AI systems with external tools and data sources, which BaryGraph uses for its interface.

<details><summary>References</summary>
<ul>
<li><a href="https://link.springer.com/chapter/10.1007/978-3-031-59468-7_2">Knowledge Graph Multilevel Abstraction: A Property Graph ...</a></li>
<li><a href="https://trustgraph.ai/guides/key-concepts/graph-reification/">Graph Reification | TrustGraph</a></li>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#knowledge-graph`, `#graph-embeddings`, `#RAG`, `#vector-search`, `#structured-knowledge`

---

<a id="item-7"></a>
## [Huawei Updates 'Tao's Law' Paper with Engineering Details and Data](https://t.me/FinanceNewsDaily/490027) ⭐️ 8.0/10

He Tingbo, head of Huawei's semiconductor division, released version 2 of the 'Tao's Law' paper on July 3, 2026, adding engineering implementation details, quantitative measurement data, and product roadmaps. This paper provides a concrete path forward for post-Moore scaling, potentially reducing reliance on advanced lithography and enabling continued chip performance improvements despite US restrictions. The V2 paper refines the 'τ scaling' framework centered on the time constant τ, and cites 381 chips already designed and mass-produced based on this principle over the past six years.

telegram · FinanceNewsDaily · Jul 4, 05:10

**Background**: Moore's Law, which predicts transistor density doubling every two years, is approaching physical limits. 'Tao's Law' or 'τ scaling' proposes using time constant τ as the scaling metric instead of geometric dimensions, optimizing across device, circuit, chip, and system levels. This approach was first presented in May 2026 and has led to Huawei's LogicFolding architecture for upcoming Kirin chips.

<details><summary>References</summary>
<ul>
<li><a href="https://siliconsemiconductor.net/article/124601/Huawei_outlines_“τ_Scaling”_vision_for_the_post-Moore_semiconductor_era">Huawei outlines “τ Scaling” vision for the post-Moore ...</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/2042360536688498595">多层电子系统的时间缩微理论（韬定律/τ 定律 ）何庭波 原论文论文中文...</a></li>
<li><a href="https://www.huaweicentral.com/huawei-logicfolding-architecture-everything-you-need-to-know/">Huawei LogicFolding Architecture: Everything you need to know</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#scaling`, `#post-Moore`, `#Huawei`, `#engineering`

---

<a id="item-8"></a>
## [iOS 27 introduces Trust Insights anti-fraud feature](https://www.cultofmac.com/news/ios-27-trust-insights-feature) ⭐️ 8.0/10

Apple's iOS 27 introduces a new on-device anti-fraud framework called Trust Insights, which analyzes user behavior patterns and sensor data in real time to detect scam-induced activities such as fraudulent money transfers. The feature was announced at WWDC 2026 and is available to developers starting with the iOS 27 beta. Trust Insights addresses the hardest type of fraud to stop: social engineering scams where users are manipulated into performing actions themselves. By providing real-time warnings and optional transaction delays, it could significantly reduce financial losses from phone scams while preserving user privacy through on-device processing. Trust Insights does not read messages, emails, or photos; raw data is deleted immediately and only a single output value is sent to Apple servers. The feature can be turned off, but there is a cooling-off period before changes take effect to prevent scammers from disabling it during a call. Its effectiveness depends on third-party app adoption.

telegram · zaihuapd · Jul 4, 14:30

**Background**: Social engineering scams are fraudulent schemes that manipulate people into divulging confidential information or transferring money. They often involve fake phone calls from scammers posing as bank officials or tech support, instructing victims to perform actions on their devices. Traditional anti-fraud measures rely on detecting suspicious messages or calls, but Trust Insights takes a novel approach by monitoring user behavior patterns on the device itself. Apple emphasizes privacy by processing all data locally and not accessing personal content.

<details><summary>References</summary>
<ul>
<li><a href="https://techmymoney.com/2026/07/04/ios-27-trust-insights-will-warn-iphone-owners-mid-scam-before-money-moves/">iOS 27 Trust Insights: iPhone Scam Warnings Explained</a></li>
<li><a href="https://9to5mac.com/2026/07/02/ios-27-helps-apps-detect-when-a-user-may-be-getting-scammed-in-real-time/">iOS 27 helps apps detect when a user may be getting scammed ...</a></li>
<li><a href="https://applemagazine.com/ios-27-trust-insights/">iOS 27 Trust Insights Helps Apps Detect Scam Coaching</a></li>

</ul>
</details>

**Tags**: `#iOS`, `#security`, `#anti-fraud`, `#privacy`, `#mobile security`

---

<a id="item-9"></a>
## [South Korea Plans $518B Semiconductor Cluster, Double DRAM Output](https://t.me/zaihuapd/42357) ⭐️ 8.0/10

South Korea announced a plan to invest 800 trillion won (about $518 billion) to build a semiconductor mega-cluster in the southwestern region, aiming to double DRAM production within five years and construct four memory fabs. This massive government-led investment signals South Korea's determination to maintain its global leadership in memory semiconductors, especially DRAM, and could reshape the global supply chain by increasing production capacity and decentralizing manufacturing away from the Seoul area. The total investment is expected to exceed 1,000 trillion won by 2035, expanding capacity to 18.4 GW. The government also pledged to ensure adequate electricity and water supply and strengthen power infrastructure around existing clusters.

telegram · zaihuapd · Jul 4, 15:15

**Background**: DRAM (Dynamic Random Access Memory) is a type of volatile memory commonly used as main memory in personal computers, servers, and workstations. South Korea's semiconductor industry is currently heavily concentrated around Seoul, with companies like Samsung and SK Hynix dominating the global DRAM market. This new cluster aims to decentralize production and solidify national competitiveness.

<details><summary>References</summary>
<ul>
<li><a href="https://en.yna.co.kr/view/AEN20260629006252320">(2nd LD) S. Korea to build semiconductor cluster in southwest ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Random-access_memory">Random - access memory - Wikipedia</a></li>
<li><a href="https://www.techtarget.com/searchstorage/definition/DRAM">What is DRAM ( Dynamic Random Access Memory )? How Does it...</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#DRAM`, `#South Korea`, `#investment`, `#manufacturing`

---