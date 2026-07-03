---
layout: default
title: "Horizon Summary: 2026-07-03 (EN)"
date: 2026-07-03
lang: en
---

> From 68 items, 14 important content pieces were selected

---

1. [crustc: Entire Rust compiler translated to C](#item-1) ⭐️ 9.0/10
2. [US Commerce Secretary Bans Differential Privacy in Census](#item-2) ⭐️ 9.0/10
3. [ECTC 2026: EMIB-T, Custom HBM, HBM4, Microfluidic Cooling, Photonics](#item-3) ⭐️ 9.0/10
4. [Satirical startup oven story highlights product development failures](#item-4) ⭐️ 8.0/10
5. [Right to Local Intelligence Movement Advocates for Local AI](#item-5) ⭐️ 8.0/10
6. [LUKS Suspend Security Regression in Linux 6.9](#item-6) ⭐️ 8.0/10
7. [Alibaba bans Claude Code over alleged backdoor risks](#item-7) ⭐️ 8.0/10
8. [Podman v6.0.0 Released with Quadlet Integration](#item-8) ⭐️ 8.0/10
9. [Immich 3.0 Major Release Launches](#item-9) ⭐️ 8.0/10
10. [Postgres transactions as a distributed systems superpower](#item-10) ⭐️ 8.0/10
11. [Meta Embraces Neocloud Model for AI Compute](#item-11) ⭐️ 8.0/10
12. [Google Gemini Omni Flash tops Video Arena leaderboard](#item-12) ⭐️ 8.0/10
13. [Anthropic accuses Alibaba of massive model distillation attack](#item-13) ⭐️ 8.0/10
14. [China drafts new internet rules: account inactivity, AI labeling, and more](#item-14) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [crustc: Entire Rust compiler translated to C](https://github.com/FractalFir/crustc) ⭐️ 9.0/10

A developer known as FractalFir has completed a 3-year project to translate the entire Rust compiler (rustc) into C, creating the crustc transpiler. This allows Rust code to be compiled on platforms that lack LLVM or GCC backends. This breakthrough could enable Rust to run on virtually any platform with a C compiler, including old and obscure hardware, significantly expanding Rust's reach. It also addresses bootstrapping concerns by potentially allowing Rust to be bootstrapped without requiring an existing Rust compiler. The crustc project is the 14th known attempt to transpile Rust to C, according to the author. It transpiles the entire rustc compiler itself, not just user programs, and outputs C code that can be compiled by GCC or other C compilers.

hackernews · Philpax · Jul 2, 22:57 · [Discussion](https://news.ycombinator.com/item?id=48768464)

**Background**: Transpilation (or source-to-source compilation) converts code from one high-level language to another, rather than to machine code. The Rust compiler (rustc) is a complex program that traditionally targets LLVM IR or GCC backend code generation. By translating rustc to C, crustc leverages the ubiquity of C compilers to enable Rust on platforms without native LLVM or GCC support.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/FractalFir/crustc">GitHub - FractalFir/crustc: Entirety of `rustc`, translated to C. · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Source-to-source_compiler">Source-to-source compiler - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community showed significant interest, with commenters noting the dedication required for this 'niche interest'. Some discussed using Diverse Double-Compiling to verify the Rust compiler's integrity, while others pointed out that LLVM once had a C backend but it was removed, and there are now efforts to revive it.

**Tags**: `#Rust`, `#compiler`, `#transpilation`, `#C`, `#systems programming`

---

<a id="item-2"></a>
## [US Commerce Secretary Bans Differential Privacy in Census](https://scottaaronson.blog/?p=9902) ⭐️ 9.0/10

On June 4, 2026, the U.S. Secretary of Commerce issued directive DAO-216-26, which bans differential privacy and noise infusion in census data, restricting disclosure avoidance to coarsening techniques only. This directive fundamentally changes how the Census Bureau protects privacy, sparking intense debate about the balance between individual privacy and data utility. It directly impacts researchers, policymakers, and anyone relying on accurate census statistics for resource allocation and redistricting. The directive explicitly forbids 'noise infusion,' defined as modifying data by adding random values, and eliminates techniques central to differential privacy. It mandates that coarsening (e.g., rounding or aggregation) be preferred, with suppression used only as a last resort.

hackernews · flowercalled · Jul 3, 00:01 · [Discussion](https://news.ycombinator.com/item?id=48768992)

**Background**: Differential privacy is a mathematical framework that adds carefully calibrated noise to statistical outputs to protect individual privacy while preserving aggregate accuracy. Noise infusion has been used by the Census Bureau and other agencies to prevent re-identification of respondents. This directive reverses a trend toward stronger mathematical privacy guarantees, favoring simpler methods that may offer less robust protection.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Differential_privacy">Differential privacy</a></li>
<li><a href="https://www.bea.gov/help/faq/1490">Why didn’t BEA use noise infusion as its statistical disclosure limitation method in its June 10, 2026, news release on “New Foreign Direct Investment in the United States, 2025’’? | U.S. Bureau of Economic Analysis (BEA)</a></li>
<li><a href="https://desfontain.es/blog/banning-noise.html">Banning noise will be a disaster for statistical data products - Ted is writing things</a></li>

</ul>
</details>

**Discussion**: Commenters expressed confusion about the political motivations behind the directive, with some speculating it aims to reduce the utility of census data for purposes like redistricting. Others noted the article lacks a detailed comparison of the banned and preferred methods, and called for more practical evidence of failures in noise infusion.

**Tags**: `#privacy`, `#differential privacy`, `#census`, `#data policy`, `#statistics`

---

<a id="item-3"></a>
## [ECTC 2026: EMIB-T, Custom HBM, HBM4, Microfluidic Cooling, Photonics](https://newsletter.semianalysis.com/p/ectc2026) ⭐️ 9.0/10

At ECTC 2026, Intel detailed its upcoming EMIB-T packaging technology with through-silicon vias for HBM4 and UCIe, while TSMC, SK Hynix, Samsung, Micron, Marvell, and Lightmatter presented advances in custom HBM, HBM4 packaging challenges, microfluidic cooling, and photonic interconnects. These advancements address critical bottlenecks in AI hardware performance and scalability, particularly for high-bandwidth memory and chip-to-chip interconnects, potentially accelerating next-generation AI accelerators. Intel's EMIB-T incorporates TSVs for improved power delivery and larger package sizes, targeting production rollout this year; Lightmatter demonstrated photonic interconnects for AI scaling, and HBM4 packaging remains a key challenge due to tighter bump pitches and thermal demands.

rss · Semianalysis · Jul 2, 17:25

**Background**: Semiconductor packaging connects chips together and to the outside world; advanced packaging like EMIB (Embedded Multi-die Interconnect Bridge) enables high-density interconnects. HBM (High Bandwidth Memory) stacks DRAM dies vertically, and HBM4 is the next generation with higher bandwidth. Photonic interconnects use light instead of electricity for faster, lower-power data transmission, critical for scaling AI systems.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/pc-components/cpus/intel-details-new-advanced-packaging-breakthroughs-emib-t-paves-the-way-for-hbm4-and-increased-ucie-bandwidth">Intel details new advanced packaging breakthroughs — EMIB-T paves the way for HBM4 and increased UCIe bandwidth | Tom's Hardware</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/semiconductors/intels-emib-t-heads-for-fab-rollout-this-year">Intel's EMIB-T packaging technology set for fab rollout this year — as TSMC CoWoS capacity remains limited, EMIB-T is preparing for advanced AI accelerator designs | Tom's Hardware</a></li>
<li><a href="https://spectrum.ieee.org/optical-interposers">Optical Interconnects: Lightmatter’s Optical Interposers ...</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#packaging`, `#HBM4`, `#photonics`, `#AI hardware`

---

<a id="item-4"></a>
## [Satirical startup oven story highlights product development failures](https://weli.dev/blog/half-baked-product/) ⭐️ 8.0/10

A satirical blog post titled 'Half-Baked Product' tells the story of a startup oven project that fails due to mismatched expectations, lack of domain expertise, and broken promises, resonating deeply with the tech community. The article offers a nuanced critique of common pitfalls in startup product development—such as founder motivation misaligned with realistic engineering—and serves as a cautionary tale for both founders and engineers. The founder, motivated by wealth rather than domain expertise, promised the engineer 20% equity and full creative freedom, but those promises were ultimately broken. The story also mentions a fictional competitor called OpenOven that offers a free oven with many non-functional buttons.

hackernews · weli · Jul 3, 08:23 · [Discussion](https://news.ycombinator.com/item?id=48772388)

**Background**: The blog post is a satirical allegory for common product development failures in the startup world, where founders often enter industries without deep knowledge, overpromise to engineers, and end up with a half-baked product. Many real-world startups face similar challenges, leading to wasted effort and disillusionment.

**Discussion**: Commenters found the story uncomfortably accurate, with one noting the part about the engineer's motivation being a 'complete lie.' Another shared a similar experience where their working oven was outcompeted by a free, feature-bloated competitor. The overall sentiment is a mix of dark humor and recognition of real startup dynamics.

**Tags**: `#startups`, `#product development`, `#engineering culture`, `#satire`

---

<a id="item-5"></a>
## [Right to Local Intelligence Movement Advocates for Local AI](https://righttointelligence.org/) ⭐️ 8.0/10

The 'Right to Local Intelligence' movement has launched to advocate for the legal right to run artificial intelligence locally on personal devices, opposing potential laws that could restrict local large language models (LLMs). This movement addresses concerns about regulatory capture by AI-as-a-service (AIaaS) companies and aims to protect user privacy, control, and innovation in the AI ecosystem. It could shape future policy debates around AI regulation and device rights. Major OEMs such as Asus, Dell, HP, Lenovo, Microsoft, and MSI are supporting local AI hardware through the upcoming Nvidia RTX Spark platform, indicating strong industry backing for local LLM usage. The movement is proactive, seeking to establish rights before restrictive laws are passed.

hackernews · thoughtpeddler · Jul 2, 23:54 · [Discussion](https://news.ycombinator.com/item?id=48768951)

**Background**: Local LLMs refer to large language models that run entirely on a user's own device, such as a PC or smartphone, without sending data to cloud servers. This contrasts with AI-as-a-service (AIaaS) models that process user data on remote servers. Potential regulations could require safety certifications or usage monitoring that may be infeasible for locally-run models, raising concerns about de facto bans on local AI.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/msb-msb/awesome-local-ai">GitHub - msb-msb/awesome-local-ai: A curated list of ...</a></li>
<li><a href="https://whatllm.org/best-local-llm">Best Local LLMs in 2026: Which Model Should You Run Locally ...</a></li>

</ul>
</details>

**Discussion**: Commenters had mixed reactions: some doubted that restrictive laws would pass given industry support for local AI hardware, while others emphasized the need for proactive advocacy to prevent regulatory capture. A few noted that making math illegal (like encryption) has failed historically, suggesting similar resistance would apply to local AI bans.

**Tags**: `#AI regulation`, `#local AI`, `#open-source AI`, `#digital rights`, `#LLM`

---

<a id="item-6"></a>
## [LUKS Suspend Security Regression in Linux 6.9](https://mathstodon.xyz/@iblech/116769502749142438) ⭐️ 8.0/10

Since Linux 6.9, the `cryptsetup luksSuspend` operation no longer wipes disk-encryption keys from memory, leaving them exposed during system suspend. This regression undermines a key security feature for full-disk encryption, as users relying on LUKS suspend to protect keys from cold boot attacks or device theft may have their data compromised. The bug originated from a kernel commit that accidentally removed a single line of C code responsible for clearing the encryption key, and it remained undetected for over two years in kernel versions 6.9 and later.

hackernews · IngoBlechschmid · Jul 2, 15:25 · [Discussion](https://news.ycombinator.com/item?id=48763035)

**Background**: LUKS (Linux Unified Key Setup) is a disk encryption specification. The `luksSuspend` command suspends a LUKS device and removes the decryption key from kernel memory, requiring re-entry of the passphrase on resume. This is designed to protect against cold boot attacks where an attacker with physical access could dump memory contents.

<details><summary>References</summary>
<ul>
<li><a href="https://www.man7.org/linux//man-pages/man8/cryptsetup-luksSuspend.8.html">cryptsetup-luksSuspend (8) - Linux manual page - man7.org</a></li>
<li><a href="https://news.ycombinator.com/item?id=48763035">Since Linux 6.9, LUKS suspend stopped wiping disk-encryption ...</a></li>
<li><a href="https://byteiota.com/luks-suspend-broken-since-kernel-6-9-two-year-gap/">LUKS Suspend Broken Since Kernel 6.9: Two-Year Gap</a></li>

</ul>
</details>

**Discussion**: Commenters debated the severity: some argued that suspend-to-RAM inherently retains keys, so the regression mainly affects specific use cases like border crossings; others highlighted that the bug was serious and that the lack of automated testing allowed it to persist.

**Tags**: `#security`, `#linux-kernel`, `#disk-encryption`, `#LUKS`

---

<a id="item-7"></a>
## [Alibaba bans Claude Code over alleged backdoor risks](https://www.reuters.com/world/china/alibaba-ban-claude-code-workplace-over-alleged-backdoor-risks-source-says-2026-07-03/) ⭐️ 8.0/10

Alibaba has ordered all employees to uninstall Claude Code and other Anthropic products, including Sonnet, Opus, and Fable, effective July 10, 2026, due to alleged backdoor risks. The ban follows Anthropic's accusation that Alibaba used approximately 25,000 fake accounts to interact with Claude over 28 million times between April 22 and June 5. This incident highlights escalating US-China tensions in AI security and the risks enterprises face when using cloud-based coding assistants that can access proprietary codebases. It may prompt other companies to reconsider reliance on foreign AI tools. Alibaba had previously reimbursed employees for using external AI models including Claude, GPT, and Gemini. Anthropic's accusation led to tightened risk controls, and the ban covers not only Claude Code but also the Sonnet, Opus, and Fable models.

hackernews · nsoonhui · Jul 3, 08:31 · [Discussion](https://news.ycombinator.com/item?id=48772443)

**Background**: Claude Code is an AI coding agent developed by Anthropic that reads codebases, edits files, and runs commands in the terminal. Anthropic's models are trained using 'constitutional AI' to improve ethical compliance. US federal agencies have also phased out Claude due to contractual disputes over surveillance and weapons use, highlighting broader geopolitical concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**Discussion**: Comments on Hacker News express mixed views: some recall previous incidents of Claude consuming usage or downgrading models, reinforcing distrust, while others argue that all remote AI pose security risks and that enterprises are becoming more cautious about tools accessing proprietary code. A leaked Chinese Telegram message details the ban order.

**Tags**: `#AI`, `#Security`, `#Enterprise`, `#Claude`, `#Geopolitics`

---

<a id="item-8"></a>
## [Podman v6.0.0 Released with Quadlet Integration](https://blog.podman.io/2026/07/introducing-podman-v6-0-0/) ⭐️ 8.0/10

Podman v6.0.0, a major version of the daemonless container engine, has been released with enhanced Quadlet support for declarative container management via systemd unit files. As a leading Docker alternative, Podman's v6.0.0 improves ease of use and systemd integration, potentially accelerating adoption in DevOps and production environments. The release centers on Quadlet, which allows users to define containers, pods, and networks in systemd unit files, simplifying deployment. Community feedback indicates seamless docker-compose compatibility but also notes minor incompatibilities and distribution support gaps.

hackernews · soheilpro · Jul 2, 14:23 · [Discussion](https://news.ycombinator.com/item?id=48762098)

**Background**: Podman is a daemonless, rootless container engine that aims to be a drop-in replacement for Docker. Quadlet is a tool that integrates with systemd to manage containers declaratively, enabling features like auto-updates and rollbacks. This release builds on that foundation to improve the developer and operator experience.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.podman.io/en/latest/markdown/podman-quadlet.1.html">podman-quadlet — Podman documentation</a></li>
<li><a href="https://www.redhat.com/en/blog/quadlet-podman">Make systemd better for Podman with Quadlet - Enable Sysadmin</a></li>

</ul>
</details>

**Discussion**: Community reaction is mixed: many praise Podman's ease of transition from Docker and the power of Quadlet, while others criticize the lack of official packages for popular distros like Ubuntu and minor Docker incompatibilities that may cause issues for projects relying on Docker-specific behavior.

**Tags**: `#podman`, `#containers`, `#docker-alternative`, `#devops`, `#release`

---

<a id="item-9"></a>
## [Immich 3.0 Major Release Launches](https://github.com/immich-app/immich/discussions/29439) ⭐️ 8.0/10

Immich 3.0 has been released, marking a major update to the popular open-source self-hosted photo management platform. The new version includes bug fixes and improvements contributed by the community. This release solidifies Immich as a leading self-hosted alternative to Google Photos, offering users full control over their data. Its growing feature set and active community make it a compelling choice for privacy-conscious individuals. The release does not introduce end-to-end encryption, a topic of much community discussion. Many users combine Immich with tools like Tailscale or full-disk encryption for additional security.

hackernews · hashier · Jul 2, 14:13 · [Discussion](https://news.ycombinator.com/item?id=48761944)

**Background**: Immich is a free, open-source self-hosted photo and video backup solution that serves as an alternative to cloud services like Google Photos. Users install the server on their own hardware and can access their media via web or mobile apps, ensuring privacy and data ownership. The project has gained significant traction in the self-hosting community.

<details><summary>References</summary>
<ul>
<li><a href="https://immich.app/">Immich</a></li>
<li><a href="https://grokipedia.com/page/Immich">Immich</a></li>

</ul>
</details>

**Discussion**: The community is highly engaged, with comments celebrating student contributions and debating encryption. Some users dismiss the need for end-to-end encryption, arguing physical security suffices, while others prefer alternatives like Ente that offer built-in encryption. Overall sentiment is positive, praising Immich's quality and value.

**Tags**: `#self-hosting`, `#photo management`, `#open source`, `#privacy`

---

<a id="item-10"></a>
## [Postgres transactions as a distributed systems superpower](https://www.dbos.dev/blog/co-locating-workflow-state-with-your-data) ⭐️ 8.0/10

A blog post proposes using Postgres transactions to manage workflow state, co-locating state with data in the same database to simplify distributed coordination. This approach eliminates the need for separate coordination mechanisms like message queues or two-phase commit, but it tightly couples the database to workflow logic, making architectural separation harder. Each workflow step becomes its own database commit unit, simplifying the outbox pattern; however, the database becomes tightly coupled to the workflow, which may be difficult to separate later.

hackernews · KraftyOne · Jul 2, 18:38 · [Discussion](https://news.ycombinator.com/item?id=48765639)

**Background**: Distributed workflows often require coordinating multiple services, traditionally using message queues or saga patterns. Postgres transactions provide atomicity and consistency, allowing workflow progress to be aligned with database commits, effectively using the database as a coordination point.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48765639">Postgres transactions are a distributed systems superpower ...</a></li>

</ul>
</details>

**Discussion**: Comments express mixed views: some appreciate the atomicity and simplicity (Crowberry), while others question whether it's truly distributed (cloudie78) and highlight tight coupling (jdw64). mrkeen recounts a job interview where he argued it's impossible to transactionally update both a database and a message queue.

**Tags**: `#Postgres`, `#distributed systems`, `#transactions`, `#workflow`, `#database architecture`

---

<a id="item-11"></a>
## [Meta Embraces Neocloud Model for AI Compute](https://newsletter.semianalysis.com/p/meta-compute-everyone-wants-to-be) ⭐️ 8.0/10

Meta is shifting its compute strategy toward a neocloud model, focusing on scaling recommendation systems by 10x, as analyzed in a SemiAnalysis newsletter that draws parallels to SpaceX and Bedrock strategies. This move signals a major trend where large tech companies build specialized AI infrastructure akin to neoclouds, potentially disrupting traditional hyperscaler dominance and redefining AI workload economics. The analysis mentions 'ClusterMAX ranking coming soon,' a GPU cloud rating system that scores providers on performance, networking, and pricing, and references scaling recommendation systems by 10x.

rss · Semianalysis · Jul 2, 22:18

**Background**: Neoclouds are specialized cloud providers dedicated to AI workloads, offering high-performance GPU clusters with transparent pricing and no long-term contracts, unlike traditional hyperscalers like AWS or Azure. Meta's shift reflects a broader industry trend where companies like SpaceX and Bedrock have also adopted similar bespoke infrastructure strategies.

<details><summary>References</summary>
<ul>
<li><a href="https://www.mckinsey.com/capabilities/tech-and-ai/our-insights/the-evolution-of-neoclouds-and-their-next-moves">Neoclouds’ challenges and next moves | McKinsey</a></li>
<li><a href="https://www.cisco.com/site/us/en/learn/topics/computing/what-is-neocloud.html">What is neocloud? - Cisco</a></li>
<li><a href="https://newsletter.semianalysis.com/p/clustermax-20-the-industry-standard">ClusterMAX™ 2.0: The Industry Standard GPU Cloud Rating System</a></li>

</ul>
</details>

**Tags**: `#Meta`, `#Cloud Computing`, `#AI Infrastructure`, `#Recommendation Systems`, `#Data Centers`

---

<a id="item-12"></a>
## [Google Gemini Omni Flash tops Video Arena leaderboard](https://x.com/Designarena/status/2072759122366509130) ⭐️ 8.0/10

Google DeepMind's Gemini Omni Flash video generation model has achieved the top spot on the Video Arena blind test leaderboard with a score of 1404, surpassing ByteDance's Seedance 2.0 Mini by 101 points. This marks a significant shift in the AI video generation landscape, as Google overtakes ByteDance's Seedance series which had long dominated the rankings, highlighting the rapid competition in multimodal generative AI. Gemini Omni Flash combines Gemini's intelligence with generative media models, supporting text-to-video, image-to-video, and conversational video editing. The model also improved Google's overall video model ranking by 7 positions compared to its Veo series.

telegram · zaihuapd · Jul 3, 05:51

**Background**: Video Arena is a crowdsourced blind test platform where users compare anonymous video outputs and vote, producing Elo-style rankings. ByteDance's Seedance 2.0 Mini is a cost-efficient tier of the Seedance 2 video family, capable of generating clips with synchronized audio in about two minutes. Google's previous Veo series had lower rankings.

<details><summary>References</summary>
<ul>
<li><a href="https://llm-stats.com/leaderboards/best-ai-for-video-generation">Best AI for Video Generation in 2026 — Ranked by Blind Human ...</a></li>
<li><a href="https://deepmind.google/models/model-cards/gemini-omni-flash/">Gemini Omni Flash - Model Card — Google DeepMind</a></li>
<li><a href="https://seedance2.ai/seedance-2-0-mini">Seedance 2.0 Mini - Lower-Cost Cinematic AI Video Generator ...</a></li>

</ul>
</details>

**Tags**: `#AI video generation`, `#Google`, `#Gemini Omni Flash`, `#ByteDance`, `#Video Arena`

---

<a id="item-13"></a>
## [Anthropic accuses Alibaba of massive model distillation attack](https://t.me/zaihuapd/42327) ⭐️ 8.0/10

Anthropic has accused Alibaba of conducting a massive 'distillation attack' using approximately 25,000 fraudulent accounts and over 28.8 million interactions with its Claude AI model from April 22 to June 5, 2026. If confirmed, this would be the largest known distillation attack against a leading AI company, raising significant concerns about intellectual property protection, AI security, and competitive intelligence in the industry. Anthropic specifically named Alibaba and its AI lab Qwen as participants, and reported the incident to the U.S. Senate Banking Committee. The attack exploited public API access to repeatedly query Claude and extract its capabilities.

telegram · zaihuapd · Jul 3, 06:21

**Background**: Model distillation is a technique where a smaller 'student' model learns to mimic the outputs of a larger 'teacher' model, often to reduce computational costs. A distillation attack applies this maliciously by repeatedly querying a proprietary AI model through its public interface to extract knowledge without authorization. Such attacks have been reported by multiple AI companies targeting Chinese labs.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation - Wikipedia</a></li>
<li><a href="https://www.anthropic.com/news/detecting-and-preventing-distillation-attacks">Detecting and preventing distillation attacks \ Anthropic</a></li>
<li><a href="https://www.mindstudio.ai/blog/ai-model-distillation-attacks-explained">AI Model Distillation Attacks: What They Are and Why They ...</a></li>

</ul>
</details>

**Tags**: `#AI Security`, `#Model Distillation`, `#Anthropic`, `#Alibaba`, `#Competitive Intelligence`

---

<a id="item-14"></a>
## [China drafts new internet rules: account inactivity, AI labeling, and more](https://mp.weixin.qq.com/s/TfYZaC8ULPvu9JeTqYGkKg) ⭐️ 8.0/10

China's Cyberspace Administration released a revised draft of the Internet Information Service Management Measures on July 3, 2026, proposing that platforms may deactivate accounts inactive for over six months, require AI-generated content labeling, allow users to opt out of personalized recommendations, and ban practices like click farming and comment manipulation. This regulation significantly impacts all internet platforms operating in China, affecting user account management, AI content transparency, and algorithmic recommendation systems. It marks a further step in China's efforts to regulate online content and protect user rights. The draft is open for public comment until August 2, 2026. It mandates that large platforms handle illegal information complaints within 24 hours and prohibits forced use of AI services. The AI labeling requirement is consistent with China's separate AI Content Labeling Measures effective September 1, 2025.

telegram · zaihuapd · Jul 3, 11:29

**Background**: China has been strengthening internet regulation through various laws, including the Cybersecurity Law and Personal Information Protection Law. The separate AI Content Labeling Measures, effective September 1, 2025, require explicit and implicit labeling of AI-generated content to prevent misinformation. The current draft expands these rules to platform account management and prohibits manipulative practices like click farming (刷量) and comment control (控评), which are common on social media to influence public opinion.

<details><summary>References</summary>
<ul>
<li><a href="http://english.scio.gov.cn/pressroom/2025-03/17/content_117769570.html">China requires labeling of AI-generated online content</a></li>
<li><a href="https://regulations.ai/regulations/RAI-CN-NA-CONTENT-2025">China AI-Generated Content Labeling Measures - Regulations.AI</a></li>
<li><a href="https://www.lexology.com/library/detail.aspx?g=3e0002f7-34f0-4df3-9879-b63a9350e085">The State Administration of Market Regulation Issues Typical ...</a></li>

</ul>
</details>

**Tags**: `#internet regulation`, `#AI content labeling`, `#privacy`, `#China`, `#platform compliance`

---