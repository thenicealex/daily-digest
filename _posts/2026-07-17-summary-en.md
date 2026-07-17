---
layout: default
title: "Horizon Summary: 2026-07-17 (EN)"
date: 2026-07-17
lang: en
---

> From 52 items, 8 important content pieces were selected

---

1. [Firefox compiled to WebAssembly runs inside another browser](#item-1) ⭐️ 9.0/10
2. [Apple Sends Legal Letters to OpenAI Employees](#item-2) ⭐️ 8.0/10
3. [Kaggle Evaluation Flaws: AI Submissions and Judges Undermine Fairness](#item-3) ⭐️ 8.0/10
4. [Kimi K3: 2.8T Open-Weight Model Surpasses Many Frontier Models](#item-4) ⭐️ 8.0/10
5. [Codex bug may delete files in full-access mode](#item-5) ⭐️ 8.0/10
6. [Truth Social to sell real-time access to Trump's posts to Wall Street traders](#item-6) ⭐️ 8.0/10
7. [US lawmakers seek ban on Chinese memory chips in allied supply chains](#item-7) ⭐️ 8.0/10
8. [OpenAI CFO Proposes 'Useful Intelligence per Dollar' as AI ROI Metric](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Firefox compiled to WebAssembly runs inside another browser](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 9.0/10

Puter has successfully compiled Mozilla Firefox (Gecko engine) to WebAssembly, enabling the entire browser to run within another browser like Chrome. A live demo is available, showing a full Firefox instance rendering web pages inside a Chrome tab. This breakthrough demonstrates that WebAssembly has reached a level of performance and capability to run a full-featured desktop browser, opening possibilities for secure browser virtualization, cross-platform testing, and novel web applications. It also highlights the potential of AI-assisted programming, as the project leveraged Claude Opus and Fable tokens for development. The project used an estimated $25,000 worth of Claude Opus and Fable tokens, but actual cost was lower due to a Claude Max subscription. All network traffic is proxied through Puter's server using the Wisp protocol over WebSocket, because WebAssembly in browsers cannot open raw network connections. The demo supports end-to-end encryption for HTTPS traffic.

rss · Simon Willison · Jul 16, 23:34

**Background**: WebAssembly (Wasm) is a low-level binary instruction format that runs in modern web browsers near native speed. It allows developers to compile code from languages like C++ into a format that executes in the browser sandbox. Browser virtualization, running one browser inside another, has long been a goal but was extremely challenging due to the complexity and resource demands of full browsers like Firefox. Previous attempts like WebKitWasm are similar but less mature.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/ wisp - protocol : Wisp is a low-overhead...</a></li>
<li><a href="https://github.com/HeyPuter/puter">GitHub - HeyPuter/puter: 🌐 The Internet Computer! Free, Open-Source, and Self-Hostable.</a></li>
<li><a href="https://developer.puter.com/">Puter Developer - The Backend for AI-Generated Apps</a></li>

</ul>
</details>

**Tags**: `#webassembly`, `#firefox`, `#browser`, `#virtualization`, `#wasm`

---

<a id="item-2"></a>
## [Apple Sends Legal Letters to OpenAI Employees](https://www.ft.com/content/1b8c9d52-88a9-426b-ba47-f1811f859166) ⭐️ 8.0/10

Apple has sent legal letters to dozens of employees at OpenAI, signaling potential legal action over confidentiality or non-compete agreements. This move could escalate tensions between the two tech giants and set a precedent for how companies protect intellectual property in the AI industry. The letters are document retention notices, which are standard practice but can be aggressive if sent before a complaint is filed. Some observers note Apple may be late in sending these letters.

hackernews · merksittich · Jul 17, 12:02 · [Discussion](https://news.ycombinator.com/item?id=48946303)

**Background**: Apple and OpenAI are major players in the technology and AI sectors. Legal letters of this type are commonly used to preserve evidence and remind former employees of their contractual obligations.

**Discussion**: Comments are mixed: some view the letters as standard practice, while others see them as an aggressive escalation. One commenter suggests Apple must have strong evidence, and another criticizes OpenAI for allegedly using stolen content.

**Tags**: `#Apple`, `#OpenAI`, `#legal`, `#AI`, `#technology`

---

<a id="item-3"></a>
## [Kaggle Evaluation Flaws: AI Submissions and Judges Undermine Fairness](https://www.kaggle.com/competitions/kaggle-measuring-agi/discussion/724918#3498423) ⭐️ 8.0/10

A discussion on Kaggle reveals evidence of inconsistencies in competition evaluation, with community members raising concerns that AI-generated submissions and AI-powered judging are undermining fairness and human skill. This challenges the credibility of Kaggle competitions as a valid measure of human expertise, and highlights broader ethical issues about AI's dual role as both participant and judge in competitive machine learning. The discussion has high engagement with 401 points and 241 comments, including mentions of specific issues like prompt injection to manipulate AI judges and brute-force methods being used since the beginning of Kaggle.

hackernews · twerkmeister · Jul 17, 11:30 · [Discussion](https://news.ycombinator.com/item?id=48946010)

**Background**: Kaggle competitions are contests of skill where participants submit machine learning models or code, and winners are evaluated based on predefined metrics or by a panel of judges. The rise of AI-generated content has made it difficult to ensure original human work, and some competitions now rely on AI for judging, creating a cycle where AI both produces and evaluates submissions. This has led to concerns about fairness and the erosion of human skill as the core element of these competitions.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kaggle.com/docs/competitions">Kaggle Competition Documentation</a></li>
<li><a href="https://fitzyhistory.substack.com/p/what-student-writing-competitions">What Student Writing Competitions Reveal About Our AI Confusion</a></li>
<li><a href="https://www.schneier.com/blog/archives/2026/02/the-ai-generated-text-arms-race.html">AI-Generated Text and the Detection Arms Race - Schneier on Security</a></li>

</ul>
</details>

**Discussion**: Community members express frustration that AI has 'killed' hackathons, with one user noting that all code is AI-generated and judging is done by AI, allowing prompt injection to win. Others argue that brute-force methods have always existed in Kaggle, and that ML competitions inherently involve automation. A few users question Kaggle's overall reputation for original research.

**Tags**: `#Kaggle`, `#AI ethics`, `#competition integrity`, `#AI-generated content`, `#evaluation bias`

---

<a id="item-4"></a>
## [Kimi K3: 2.8T Open-Weight Model Surpasses Many Frontier Models](https://simonwillison.net/2026/Jul/16/kimi-k3/#atom-everything) ⭐️ 8.0/10

Moonshot AI announced Kimi K3, a 2.8 trillion parameter model that outperforms Claude Opus 4.8 and GPT-5.5 on many benchmarks, and promised open weights by July 27, 2026. This release signals that open-weight models are rapidly closing the gap with proprietary frontier models, potentially democratizing access to state-of-the-art AI capabilities. Kimi K3 uses 21% fewer output tokens than its predecessor K2.6, and its pricing ($3/$15 per million tokens) makes it the most expensive model from a Chinese lab yet, comparable to Claude Sonnet.

rss · Simon Willison · Jul 16, 20:19

**Background**: The 'pelican on a bicycle' benchmark is an informal test created by Simon Willison that asks LLMs to generate an SVG of a pelican riding a bicycle, evaluating code generation and spatial reasoning. Open-weight models provide access to model weights for fine-tuning and local deployment, unlike closed APIs.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jul/16/kimi-k3/">Kimi K3, and what we can still learn from the pelican benchmark</a></li>
<li><a href="https://grokipedia.com/page/Pelican_on_a_bicycle_AI_benchmark">Pelican on a bicycle (AI benchmark)</a></li>

</ul>
</details>

**Tags**: `#AI`, `#LLM`, `#Kimi K3`, `#Moonshot AI`, `#open model`

---

<a id="item-5"></a>
## [Codex bug may delete files in full-access mode](https://simonwillison.net/2026/Jul/16/bad-codex-bug/#atom-everything) ⭐️ 8.0/10

A bug in GPT-5.6 Codex can cause accidental deletion of user files when full-access mode is enabled and sandboxing protections are disabled. The model mistakenly deletes the $HOME directory while attempting to override the $HOME environment variable for a temporary directory. This bug highlights a critical safety risk for AI coding agents that have direct file system access. Developers relying on Codex without proper sandboxing could lose important data, underscoring the need for robust isolation and review mechanisms in agentic AI tools. The bug occurs specifically when full-access mode is enabled, codex is run without sandboxing, and auto review is disabled. The model's attempted override of $HOME fails, leading to the deletion of the entire home directory.

rss · Simon Willison · Jul 16, 17:45

**Background**: Codex is an AI coding agent from OpenAI that runs locally in the terminal (released as open-source CLI in April 2025). Full-access mode grants the agent unrestricted file system permissions, while sandboxing provides an isolated environment to limit potential damage. Auto review is a feature that requires user approval before executing file operations. This bug demonstrates the dangers of combining high privilege levels with insufficient safeguards.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Codex_(AI_agent)">OpenAI Codex (AI agent ) - Wikipedia</a></li>
<li><a href="https://www.fortinet.com/resources/cyberglossary/what-is-sandboxing">What is sandboxing? How AI sandboxing enhances threat detection | Fortinet</a></li>
<li><a href="https://developer.nvidia.com/blog/practical-security-guidance-for-sandboxing-agentic-workflows-and-managing-execution-risk/">Practical Security Guidance for Sandboxing Agentic Workflows and Managing Execution Risk | NVIDIA Technical Blog</a></li>

</ul>
</details>

**Tags**: `#codex`, `#coding-agents`, `#generative-ai`, `#ai-safety`

---

<a id="item-6"></a>
## [Truth Social to sell real-time access to Trump's posts to Wall Street traders](https://www.cnn.com/2026/07/16/business/truth-social-data-wall-street) ⭐️ 8.0/10

Trump Media & Technology Group announced that Truth Social will launch a paid API called Truth API on August 1, providing institutional clients with millisecond-speed access to real-time posts from the platform's top 10 accounts, including Donald Trump, for use in algorithmic trading strategies. This marks the first time a social media platform has directly monetized access to a political leader's posts for high-frequency trading, potentially amplifying market volatility and raising serious ethical questions about the intersection of presidential communication and profit. The API specifically targets algorithmic traders who seek information advantages, as Trump's posts on tariffs, Iran, and the Strait of Hormuz have previously caused sharp market moves in stocks and oil; TMTG has not disclosed pricing.

telegram · zaihuapd · Jul 17, 01:02

**Background**: High-frequency trading (HFT) uses computer algorithms to execute trades in microseconds, capitalizing on tiny price discrepancies. Social media feeds are increasingly used as data sources for trading signals. Truth Social has become Trump's primary communication channel, and its monetization through a paid API represents a new frontier in data selling, but also blurs the line between public service and private gain.

<details><summary>References</summary>
<ul>
<li><a href="https://www.hindustantimes.com/world-news/us-news/trump-media-launches-truth-api-to-give-banks-faster-access-to-truth-social-posts-101784225959242.html">Trump Media launches Truth API to give banks... | Hindustan Times</a></li>
<li><a href="https://en.wikipedia.org/wiki/High-frequency_trading">High-frequency trading</a></li>

</ul>
</details>

**Tags**: `#Truth Social`, `#API`, `#high-frequency trading`, `#data monetization`, `#Trump`

---

<a id="item-7"></a>
## [US lawmakers seek ban on Chinese memory chips in allied supply chains](https://www.tomshardware.com/pc-components/dram/lawmakers-want-us-government-to-ban-memory-chips-from-china-even-in-allied-supply-chains-citing-unacceptable-risk-to-national-economic-and-supply-chain-security) ⭐️ 8.0/10

US lawmakers John Moolenaar and George Whitesides sent a letter to Secretary of Commerce Howard Lutnick urging a ban on US purchases of Chinese memory chips and recommending adding CXMT to the Entity List while tightening restrictions on YMTC. They also called for coordination with allies to prevent Chinese memory chips from entering allied supply chains. This proposal could significantly reshape the global memory chip supply chain, potentially disrupting AI infrastructure and consumer electronics that rely on these components. It underscores escalating US-China tech rivalry and may force companies like Apple to find alternative suppliers. The letter specifically targets CXMT (DRAM) and YMTC (NAND flash), citing their ties to China's military and risks of funding dual-use technology. The lawmakers urge not only a US ban but also diplomatic pressure on Japan, South Korea, and the EU to block Chinese memory chips from allied supply chains.

telegram · zaihuapd · Jul 17, 14:00

**Background**: CXMT is a Chinese DRAM manufacturer founded in 2016, while YMTC produces NAND flash memory. The US Entity List is a trade blacklist that restricts exports to listed entities. These Chinese firms are already under some US restrictions, but the lawmakers propose expanding them to cover indirect purchases through allied supply chains.

<details><summary>References</summary>
<ul>
<li><a href="https://zh.wikipedia.org/wiki/长鑫存储">长鑫存储 - 维基百科，自由的百科全书</a></li>
<li><a href="https://developer.aliyun.com/article/1100149">长 江 存 储 YMTC Xtacking技术演进与芯片级解密-开发者社区-阿里云</a></li>
<li><a href="https://zh.wikipedia.org/zh-cn/實體清單">实 体 清 单 - 维基百科，自由的百科全书</a></li>

</ul>
</details>

**Tags**: `#US-China tech rivalry`, `#semiconductor supply chain`, `#memory chips`, `#national security`, `#policy`

---

<a id="item-8"></a>
## [OpenAI CFO Proposes 'Useful Intelligence per Dollar' as AI ROI Metric](https://openai.com/index/a-scorecard-for-the-ai-age) ⭐️ 8.0/10

OpenAI CFO Sarah Friar introduced a new framework for measuring AI ROI centered on 'useful intelligence per dollar,' replacing traditional metrics like user adoption or token cost. The framework was discussed alongside the release of GPT-5.6 Sol, which sets new records in coding tasks with 54% fewer output tokens than a leading model. This new metric provides enterprise decision-makers with a more business-aligned way to evaluate AI investments, focusing on task-level cost savings rather than raw token prices. It could become an industry standard for AI ROI reporting, influencing how companies purchase and deploy AI models. The framework has four dimensions: useful work completed, total cost per successful task, reliability of AI outputs, and whether each dollar yields more value as usage scales. Friar emphasized that the lowest token price does not equal the lowest task cost, as more powerful models can solve tasks in a single attempt, saving money overall.

telegram · zaihuapd · Jul 17, 15:00

**Background**: Traditionally, AI ROI has been measured by metrics like user count, subscription renewals, or token volume, which do not capture the actual business value generated. The new 'useful intelligence per dollar' metric aims to align AI spending with real outcomes such as time saved or tasks completed. The GPT-5.6 Sol model, with 105K tokens context and support for text and image inputs, demonstrates the performance improvements that make this metric relevant.

<details><summary>References</summary>
<ul>
<li><a href="https://xairouter.com/models/gpt-5.6-sol/">GPT - 5 . 6 Sol | XAI Router</a></li>

</ul>
</details>

**Tags**: `#AI ROI`, `#OpenAI`, `#performance metrics`, `#GPT-5.6`, `#enterprise AI`

---