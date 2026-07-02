---
layout: default
title: "Horizon Summary: 2026-07-02 (EN)"
date: 2026-07-02
lang: en
---

> From 57 items, 10 important content pieces were selected

---

1. [ECTC 2026 Roundup: EMIB-T, HBM4, Photonic Interconnects, and Cooling](#item-1) ⭐️ 9.0/10
2. [Virginia Bans Sale of Geolocation Data](#item-2) ⭐️ 8.0/10
3. [Linux 6.9 Bug: LUKS Suspend Fails to Wipe Encryption Keys](#item-3) ⭐️ 8.0/10
4. [Podman v6.0.0 Release Boosts Networking](#item-4) ⭐️ 8.0/10
5. [Using DSPy to Optimize Datasette Agent's SQL Prompts](#item-5) ⭐️ 8.0/10
6. [Understand to Participate: Avoiding Cognitive Debt with AI Coding Agents](#item-6) ⭐️ 8.0/10
7. [Cloudflare to Block Mixed-Purpose AI Crawlers from September](#item-7) ⭐️ 8.0/10
8. [OpenAI Proposes U.S. Government Stake in AI Companies](#item-8) ⭐️ 8.0/10
9. [Companies Restrict AI Tools as Costs Soar](#item-9) ⭐️ 8.0/10
10. [PS3 Store Shutdown in 2027 Spurs Archival Effort](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [ECTC 2026 Roundup: EMIB-T, HBM4, Photonic Interconnects, and Cooling](https://newsletter.semianalysis.com/p/ectc2026) ⭐️ 9.0/10

A roundup from ECTC 2026 covers Intel's EMIB-T advanced packaging for HBM4, challenges in HBM4 integration, microfluidic cooling, and photonic interconnects from companies like Lightmatter. These technologies address critical bottlenecks in AI and HPC computing, such as memory bandwidth, thermal management, and interconnect efficiency, shaping the future of chip design. Intel's EMIB-T scales to large form factors with reduced defect vulnerability, while HBM4 raises I/O density and power delivery demands. Microfluidic cooling and photonic interconnects offer novel solutions for heat dissipation and data transmission.

rss · Semianalysis · Jul 2, 17:25

**Background**: EMIB (Embedded Multi-die Interconnect Bridge) is Intel's technology for connecting multiple dies in a package. HBM (High Bandwidth Memory) stacks DRAM vertically for high bandwidth. Photonic interconnects use light instead of electrons for faster, lower-power data transfer. Advanced packaging integrates these components to overcome performance limits of traditional chips.

<details><summary>References</summary>
<ul>
<li><a href="https://abit.ee/en/hard/intel-introduces-emib-t-revolutionary-multi-die-packaging-technology-with-hbm4-support">Intel Introduces EMIB - T — Revolutionary Multi-Die Packaging...</a></li>
<li><a href="https://blogs.sw.siemens.com/semiconductor-packaging/2026/04/24/hbm3e-hbm4-ic-design-guide/">HBM3e and HBM4: IC design guide for next-generation high bandwidth memory</a></li>
<li><a href="https://www.sciencedirect.com/topics/engineering/photonic-interconnects">Photonic Interconnects - an overview | ScienceDirect Topics</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#advanced packaging`, `#HBM`, `#photonic interconnects`, `#cooling`

---

<a id="item-2"></a>
## [Virginia Bans Sale of Geolocation Data](https://www.hunton.com/privacy-and-cybersecurity-law-blog/virginia-bans-sale-of-geolocation-data) ⭐️ 8.0/10

Virginia has banned the sale of geolocation data, effective July 1, 2024, through a new state privacy law. This legislation sets an important precedent for state-level privacy protections, potentially influencing other states to adopt similar measures and giving consumers more control over their sensitive location data. The ban applies to the sale of geolocation data collected from individuals within Virginia, but enforcement challenges remain regarding out-of-state companies and data processed in Virginia data centers.

hackernews · toomuchtodo · Jul 2, 21:03 · [Discussion](https://news.ycombinator.com/item?id=48767347)

**Background**: Geolocation data reveals a person's precise whereabouts and is increasingly collected by apps and devices. Concerns about misuse, such as tracking visits to sensitive locations like abortion clinics or use by insurance companies, have driven calls for regulation. Virginia's law is part of a broader trend of U.S. states enacting privacy protections in the absence of a comprehensive federal law.

**Discussion**: Comments generally support the ban but highlight enforcement difficulties and loopholes, such as out-of-state companies selling data collected in Virginia. Specific concerns include use of location data for anti-abortion ads (citing a Politico investigation) and car insurance tracking. The discussion also notes that the ban was effective July 1, 2024.

**Tags**: `#privacy`, `#geolocation data`, `#legislation`, `#Virginia`, `#data protection`

---

<a id="item-3"></a>
## [Linux 6.9 Bug: LUKS Suspend Fails to Wipe Encryption Keys](https://mathstodon.xyz/@iblech/116769502749142438) ⭐️ 8.0/10

A regression in Linux kernel 6.9 causes the `cryptsetup luksSuspend` command to no longer wipe disk-encryption keys from kernel memory, potentially exposing them during system suspend. This security regression undermines protection against cold boot attacks that rely on removing encryption keys from memory during suspend. It affects users who rely on LUKS encryption and suspend-to-RAM, particularly on Debian where the feature is integrated. The bug was introduced in Linux 6.9, and the `luksSuspend` command normally wipes the encryption key from kernel memory before suspending I/O. The community discovered it via NixOS tests, which now include a test to prevent recurrence.

hackernews · IngoBlechschmid · Jul 2, 15:25 · [Discussion](https://news.ycombinator.com/item?id=48763035)

**Background**: LUKS (Linux Unified Key Setup) is a disk encryption specification. When a system suspends to RAM, the encryption master key remains in kernel memory to allow quick resume. To mitigate cold boot attacks, `cryptsetup luksSuspend` can evict the key before suspend and require re-entry on resume. This regression broke that key eviction.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/systemd/systemd/issues/17887">Wipe LUKS Disk Encryption Key for Root Disk from RAM during Shutdown to defeat Cold Boot Attacks · Issue #17887 · systemd/systemd</a></li>
<li><a href="https://blog.freesources.org/posts/2020/08/cryptsetup-suspend/">cryptsetup- suspend</a></li>
<li><a href="https://wiki.archlinux.org/title/Power_management/Suspend_and_hibernate">Power management/ Suspend and hibernate - ArchWiki</a></li>

</ul>
</details>

**Discussion**: Comments noted that the bug might only affect Debian since `luksSuspend` is not officially supported upstream. Some argued the title was clickbait, while others appreciated the NixOS test. A commenter pointed out that security regressions like this are easy to miss because everything still appears to work.

**Tags**: `#Linux`, `#security`, `#encryption`, `#kernel`, `#LUKS`

---

<a id="item-4"></a>
## [Podman v6.0.0 Release Boosts Networking](https://blog.podman.io/2026/07/introducing-podman-v6-0-0/) ⭐️ 8.0/10

Podman v6.0.0 has been released with significant networking improvements, further strengthening its position as a Docker alternative. The update includes enhanced network stack performance and continued support for rootless containers and Quadlet. This release underscores Podman's growing maturity and adoption as a secure, daemonless container engine. With high community engagement on Hacker News, it signals increasing trust in Podman for production workloads. Podman v6.0.0 introduces new networking features that improve performance and ease of use, while maintaining compatibility with Docker CLI and docker-compose. However, some users report minor incompatibilities that can cause issues in complex setups.

hackernews · soheilpro · Jul 2, 14:23 · [Discussion](https://news.ycombinator.com/item?id=48762098)

**Background**: Podman is an open-source, OCI-compliant container engine developed by Red Hat. Unlike Docker, it is daemonless and supports rootless containers by default, enhancing security. It integrates well with systemd and can be used as a drop-in replacement for Docker in many scenarios.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Podman">Podman - Wikipedia</a></li>
<li><a href="https://podman.io/">Podman</a></li>
<li><a href="https://www.redhat.com/en/topics/containers/what-is-podman">What is Podman?</a></li>

</ul>
</details>

**Discussion**: Community sentiment is largely positive, with users praising Podman's ease of migration and performance. Some users express frustration over minor Docker incompatibilities, while others highlight the benefits of rootless operation and systemd integration.

**Tags**: `#Podman`, `#containerization`, `#Docker alternative`, `#open source`, `#release`

---

<a id="item-5"></a>
## [Using DSPy to Optimize Datasette Agent's SQL Prompts](https://simonwillison.net/2026/Jul/2/dspy-datasette-agent-prompts/#atom-everything) ⭐️ 8.0/10

Simon Willison used the DSPy framework to automatically evaluate and improve the system prompts for Datasette Agent's SQL query generation feature, identifying and fixing issues like column-name guessing due to incomplete schema information. This demonstrates a practical, automated approach to prompt engineering that can enhance the reliability and accuracy of AI agents that generate SQL. It shows how frameworks like DSPy can be leveraged to systematically improve agent behavior without manual trial and error. The experiment used Claude Code (with the Fable 5 model) to set up the evaluation pipeline, and tested with GPT-4.1 mini and nano models. One key finding was that the original prompt's advice to avoid unnecessary schema lookups caused the agent to guess column names, leading to errors.

rss · Simon Willison · Jul 2, 18:25

**Background**: DSPy is a Python framework for algorithmically optimizing prompts and weights of language models, treating prompt engineering as a programming task. Datasette Agent is an open-source AI assistant plugin for Datasette that allows users to query SQLite databases using natural language. Claude Code is an AI coding agent developed by Anthropic that can read codebases, edit files, and run commands.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/stanfordnlp/dspy">GitHub - stanfordnlp/dspy: DSPy: The framework for programming—not prompting—language models</a></li>
<li><a href="https://datasette.io/blog/2026/datasette-agent/">Datasette Agent, an extensible AI assistant for Datasette - Datasette Blog</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>

</ul>
</details>

**Tags**: `#DSPy`, `#prompt engineering`, `#AI agents`, `#SQL generation`, `#Datasette`

---

<a id="item-6"></a>
## [Understand to Participate: Avoiding Cognitive Debt with AI Coding Agents](https://simonwillison.net/2026/Jul/2/understand-to-participate/#atom-everything) ⭐️ 8.0/10

Geoffrey Litt introduced the 'understand to participate' framing during his talk at AIE 2026, emphasizing that developers must deeply understand code produced by AI agents to remain active participants and avoid cognitive debt. This concept helps developers maintain code quality and accurate mental models when using AI coding agents, preventing the buildup of cognitive debt that can hinder long-term project health and evolution. The talk was part of AIE 2026, which had over 300 recorded sessions; Geoffrey also published a Twitter thread summarizing his talk, and the full video will be released on YouTube over the following three weeks.

rss · Simon Willison · Jul 2, 17:07

**Background**: Cognitive debt is an emerging term describing the erosion of shared understanding in a software team, especially when AI agents generate code that developers do not fully comprehend. Unlike technical debt, which is about code quality, cognitive debt affects developers' ability to reason about and safely change the system, leading to increased uncertainty and slowed progress.

<details><summary>References</summary>
<ul>
<li><a href="https://margaretstorey.com/blog/2026/02/09/cognitive-debt/">How Generative and Agentic AI Shift Concern from Technical Debt to Cognitive Debt</a></li>
<li><a href="https://getdx.com/blog/cognitive-debt-the-hidden-risk-in-ai-driven-software-development/">Cognitive debt: The hidden risk in AI-driven software development</a></li>
<li><a href="https://www.faros.ai/blog/best-ai-coding-agents-2026">Best AI Coding Agents for 2026: Real-World Developer Reviews</a></li>

</ul>
</details>

**Tags**: `#AI-assisted coding`, `#cognitive debt`, `#collaboration`, `#software engineering`, `#developer tools`

---

<a id="item-7"></a>
## [Cloudflare to Block Mixed-Purpose AI Crawlers from September](https://techcrunch.com/2026/07/01/cloudflares-new-policy-pushes-ai-companies-to-pay-for-publishers-content/) ⭐️ 8.0/10

Cloudflare announced that starting September 15, it will by default block 'mixed-purpose' crawlers that are used for both search indexing and AI training from accessing ad-supported pages. The company specifically called out Google for exploiting the gap between allowing search indexing and blocking AI training. This policy shift could force AI companies to negotiate payment for using publisher content, potentially reshaping the economics of web scraping and AI training. It highlights growing tensions between content creators and AI firms over data usage rights. The new rule applies to crawlers that serve both search indexing and AI training purposes, such as Google's crawler which may index for search while also training its AI models. Cloudflare's move comes amid broader industry debates over fair compensation for content used in AI systems.

telegram · zaihuapd · Jul 2, 05:37

**Background**: Web crawlers are automated programs that scan websites to index content for search engines or collect data for AI training. While search crawlers are generally welcomed by sites to improve visibility, AI training crawlers are often blocked because they extract content without compensation. Mixed-purpose crawlers blur this line, making it hard for websites to differentiate between allowed indexing and unwanted AI training. Cloudflare's new policy attempts to address this by default blocking such crawlers on ad-supported pages.

<details><summary>References</summary>
<ul>
<li><a href="https://www.zhihu.com/question/24098641">通俗的讲，网络爬虫到底是什么？</a></li>
<li><a href="https://www.clickfrom.ai/zh/blog/inside-the-ai-mind-how-chatgpt-and-ai-crawlers-see-your-website">进入 AI 的思维：ChatGPT和 AI 爬 虫 如何看待你的网站 — ClickFrom. AI</a></li>

</ul>
</details>

**Discussion**: A comment on the TechCrunch article summarized the issue: many websites block AI crawlers but not Google's search crawler, and Google exploits this loophole to train its AI. This sentiment reflects widespread frustration with AI companies' data practices.

**Tags**: `#Cloudflare`, `#AI crawlers`, `#Google`, `#web scraping`, `#AI training`

---

<a id="item-8"></a>
## [OpenAI Proposes U.S. Government Stake in AI Companies](https://www.bloomberg.com/news/articles/2026-07-02/openai-proposes-giving-the-us-government-a-5-stake-ft-says) ⭐️ 8.0/10

OpenAI has proposed that the U.S. government take a 5% equity stake in the company and potentially in other leading AI firms such as Google, Meta, and Anthropic, according to a Financial Times report. The proposal is intended to address political backlash and allow the public to benefit from AI's economic gains. This proposal could reshape AI governance by creating a formal mechanism for public profit-sharing from AI technologies, potentially setting a precedent for government involvement in the tech industry. If adopted, it would give the government a financial stake and possibly influence over major AI companies, raising questions about control and conflicts of interest. The stake would be held by a government carrier, and at OpenAI's current valuation, a 5% stake would be worth approximately $42.6 billion. It remains unclear whether the other companies mentioned have agreed to the proposal, and the plan could face significant regulatory and antitrust scrutiny.

telegram · zaihuapd · Jul 2, 06:02

**Background**: The proposal comes amid growing political pressure on AI companies to address concerns about job displacement, safety, and the concentration of wealth. OpenAI recently became a Public Benefit Corporation (PBC), which legally requires it to consider public interests alongside profits. Other lawmakers, such as Senator Bernie Sanders, have proposed more extensive public ownership models for AI.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/07/02/openai-proposes-us-government-own-5percent-stake-to-address-political-blowback.html">OpenAI proposes U.S. government own 5% stake to address ...</a></li>
<li><a href="https://www.forbes.com/sites/siladityaray/2026/07/02/openai-reportedly-pitches-granting-us-government-5-stake/">OpenAI Reportedly Pitches Granting U.S. Government 5% Stake</a></li>
<li><a href="https://apnews.com/article/bernie-sanders-ai-public-ownership-57b9f20d96490083e2749adba0f13977">Bernie Sanders unveils plan for public ownership of AI ...</a></li>

</ul>
</details>

**Tags**: `#政策影响`, `#AI治理`, `#大型科技公司`, `#政府持股`

---

<a id="item-9"></a>
## [Companies Restrict AI Tools as Costs Soar](https://www.404media.co/companies-are-throttling-employees-ai-use-because-its-too-expensive/) ⭐️ 8.0/10

Citi banned GPT-5.5 and Claude Opus 4.6/4.7 on June 24, 2026, deeming them too expensive. Atlassian's monthly AI spend skyrocketed from $5M to $15M between August 2025 and May 2026, prompting usage caps and cost dashboards. Adobe also ended its unlimited Claude contract. This trend reveals that enterprise AI adoption faces serious cost sustainability issues under usage-based pricing. It may slow AI integration and prompt a shift in pricing models or internal usage policies across industries. Internal data from 404 Media shows that advanced models like GPT-5.5 and Claude Opus 4.6 consume AI credits much faster than standard models. Atlassian's cost dashboard revealed that 20% of employees were using AI excessively, driving the spending surge.

telegram · zaihuapd · Jul 2, 13:59

**Background**: GPT-5.5, released by OpenAI on April 23, 2026, is its most capable model but comes with higher token pricing—prompts over 272K tokens cost double the input rate. Claude Opus 4.6, released by Anthropic on February 5, 2026, is similarly expensive. Many enterprises now use AI credits or tokens for billing, where each interaction consumes credits based on model and token count.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.5">GPT-5.5 - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Opus_4.6">Claude Opus 4.6</a></li>

</ul>
</details>

**Tags**: `#AI`, `#cost management`, `#enterprise`, `#OpenAI`, `#Claude`

---

<a id="item-10"></a>
## [PS3 Store Shutdown in 2027 Spurs Archival Effort](http://no-intro.org/) ⭐️ 8.0/10

Sony announced the permanent closure of the PS3 and PS Vita PlayStation Stores in July 2027, prompting digital archivists and the RPCS3 emulator team to urgently backup game data to prevent permanent loss of digital-only titles. This closure threatens the preservation of hundreds of digital-only PS3 and PS Vita games, highlighting the fragility of digital game ownership and the need for community-led preservation efforts. RPCS3 recommends using the no-intro.org database, which catalogs metadata like cryptographic hashes and file sizes, to coordinate backup efforts and track which games have been preserved.

telegram · zaihuapd · Jul 2, 15:04

**Background**: The PlayStation 3 and PS Vita stores are digital marketplaces for downloading games. With the store closure, users will no longer be able to purchase or re-download digital content. RPCS3 is an open-source PS3 emulator that allows playing PS3 games on PC, and no-intro.org is a community-driven database for game preservation.

<details><summary>References</summary>
<ul>
<li><a href="https://rpcs3.net/">RPCS3</a></li>
<li><a href="https://no-intro.org/">No - Intro . org</a></li>
<li><a href="https://www.tomshardware.com/video-games/playstation/digital-archivists-rush-to-save-ps3-game-data-before-sony-shuts-down-the-store-forever-in-2027-rpcs3-emulator-urges-users-to-preserve-all-content">Digital archivists rush to save PS3 game data before... | Tom's Hardware</a></li>

</ul>
</details>

**Tags**: `#digital preservation`, `#PlayStation`, `#game emulation`, `#digital rights`

---