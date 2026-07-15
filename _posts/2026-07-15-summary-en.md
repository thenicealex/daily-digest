---
layout: default
title: "Horizon Summary: 2026-07-15 (EN)"
date: 2026-07-15
lang: en
---

> From 54 items, 11 important content pieces were selected

---

1. [Stripe and Advent Jointly Bid Over $53B for PayPal](#item-1) ⭐️ 9.0/10
2. [Inkling: A Large Open-Weights Multimodal Model with Audio](#item-2) ⭐️ 8.0/10
3. [Telegram Data Center Investigation Reveals Potential FSB Ties](#item-3) ⭐️ 8.0/10
4. [Sleep regularity beats duration for mortality risk](#item-4) ⭐️ 8.0/10
5. [Claude web_fetch data exfiltration via prompt injection](#item-5) ⭐️ 8.0/10
6. [First Paper on Disentangling CNN Neuron via Hadamard Clustering](#item-6) ⭐️ 8.0/10
7. [PyTorch model 170x slower on T4 than A100](#item-7) ⭐️ 8.0/10
8. [DeepSeek plans IPO by 2027, seeks new funding at $71B valuation](#item-8) ⭐️ 8.0/10
9. [Judge Questions Epic-Google $800M Deal Weakening Antitrust Case](#item-9) ⭐️ 8.0/10
10. [DeepSeek Raises Over $7.4B in First Round with Unusual Control Structure](#item-10) ⭐️ 8.0/10
11. [Telegram Serverless Platform: No Server Needed for Bots](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Stripe and Advent Jointly Bid Over $53B for PayPal](https://www.reuters.com/business/finance/stripe-advent-offer-buy-paypal-more-than-53-billion-sources-say-2026-07-15/) ⭐️ 9.0/10

Stripe and private equity firm Advent International have jointly made an offer to acquire PayPal for more than $53 billion, according to sources. This would be one of the largest consolidations in the fintech sector if completed. The acquisition would combine two of the largest online payment platforms, potentially reshaping the competitive landscape of digital payments. It raises significant antitrust concerns and could impact merchant choice, pricing, and service policies across the industry. The offer values PayPal at over $53 billion, and the deal would bring together Stripe, PayPal, Venmo, Braintree, and Xoom under one umbrella. The Herfindahl-Hirschman Index (HHI) for online card-not-present checkout would become extremely high, likely requiring significant divestitures to pass antitrust scrutiny.

hackernews · rvz · Jul 15, 03:32 · [Discussion](https://news.ycombinator.com/item?id=48915953)

**Background**: Stripe is a leading online payment processor favored by startups and tech companies, while PayPal is an older, widely-used platform with a broader consumer base. PayPal also owns Venmo, a popular peer-to-peer payment app, and Braintree, a direct competitor to Stripe. The acquisition could give Stripe access to PayPal's bank charter, enabling it to offer new financial services.

**Discussion**: Community sentiment is largely negative, with concerns about reduced competition and higher fees. Commenters note that Stripe's restrictive policies on certain industries (e.g., cannabis, adult) differ from PayPal's more permissive approach, potentially harming vendors. Some also worry about the consolidation of payment services increasing risk for users.

**Tags**: `#acquisition`, `#fintech`, `#payments`, `#antitrust`

---

<a id="item-2"></a>
## [Inkling: A Large Open-Weights Multimodal Model with Audio](https://thinkingmachines.ai/news/introducing-inkling/) ⭐️ 8.0/10

Thinking Machines AI released Inkling, an open-weights multimodal model supporting audio, along with resources for local deployment and fine-tuning via llama.cpp and Unsloth. It claims to be the largest open-weights model with native audio support. Inkling fills a gap in open-source multimodal models by offering strong audio capabilities, enabling developers and enterprises to build custom audio-aware AI applications. Its open-weights nature allows full customization, potentially lowering costs compared to proprietary models. The model is designed for efficient thinking and multimodal processing, with resources for fine-tuning on Tinker platform. Community members have already created GGUF and NVFP4 quantizations for efficient local inference.

hackernews · vimarsh6739 · Jul 15, 18:12 · [Discussion](https://news.ycombinator.com/item?id=48924912)

**Background**: Open-weights models provide pretrained parameters under permissive licenses, allowing anyone to download, run, fine-tune, and redistribute them without separate inference licenses. Multimodal AI systems can understand and reason across multiple data types like text, images, and audio. Inkling combines both concepts, aiming to offer a versatile base for customization.

<details><summary>References</summary>
<ul>
<li><a href="https://aiwiki.ai/wiki/open_weights">Open weights | AI Wiki</a></li>
<li><a href="https://www.ibm.com/think/topics/multimodal-ai">What is Multimodal AI? | IBM</a></li>
<li><a href="https://en.wikipedia.org/wiki/Multimodal_learning">Multimodal learning - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community is excited about Inkling's audio capabilities and its potential for local deployment, with some comparing it favorably to other open models. There is interest in benchmarking its audio performance, and several users have already shared deployment recipes and quantization files.

**Tags**: `#open-weights`, `#multimodal`, `#audio`, `#AI model`, `#fine-tuning`

---

<a id="item-3"></a>
## [Telegram Data Center Investigation Reveals Potential FSB Ties](https://dev.moe/en/3025) ⭐️ 8.0/10

An investigation suggests that Telegram's data center infrastructure is managed by an individual also managing infrastructure for Russia's FSB, unbeknownst to Telegram employees. Community discussion provides additional technical analysis and context. This raises serious privacy and security concerns for Telegram's global user base, especially given Telegram's reputation as a secure messaging platform. It could affect user trust and lead to increased regulatory scrutiny. The investigation notes that DC2 serves Russian and Ukrainian users and is frequently down, while a gap in DC3 deployment is questioned. Users can identify their assigned data center via Telegram's API method help.getConfig.

hackernews · theanonymousone · Jul 15, 13:22 · [Discussion](https://news.ycombinator.com/item?id=48920475)

**Background**: Telegram operates distributed data centers across multiple countries, with each user associated with a specific DC for data storage and processing. The FSB is Russia's Federal Security Service, and the investigation claims a link between Telegram's infrastructure management and FSB operations. Telegram has not publicly disputed these findings.

<details><summary>References</summary>
<ul>
<li><a href="https://core.telegram.org/api/datacenter">Working with Different Data Centers</a></li>
<li><a href="https://www.frugaltesting.com/blog/how-telegram-ensures-speed-reliability-at-massive-scale">How Telegram Ensures Speed & Reliability at Massive Scale</a></li>
<li><a href="https://www.fbi.gov/investigate/cyber/alerts/2025/russian-government-cyber-actors-targeting-networking-devices-critical-infrastructure">Russian Government Cyber Actors Targeting Networking Devices ...</a></li>

</ul>
</details>

**Discussion**: Comments highlight that the FSB link has been previously reported and remains undisputed by Telegram. Users also discuss data center performance (e.g., DC2 frequent downtime, Miami DC speed) and technical methods to identify DCs via API.

**Tags**: `#Telegram`, `#data centers`, `#privacy`, `#infrastructure`, `#security`

---

<a id="item-4"></a>
## [Sleep regularity beats duration for mortality risk](https://academic.oup.com/sleep/article/47/1/zsad253/7280269) ⭐️ 8.0/10

A 2023 study published in the journal Sleep found that sleep regularity (consistency of sleep-wake timing) is a stronger predictor of mortality risk than sleep duration, using data from over 60,000 participants. This finding challenges the common focus on sleep duration alone and suggests that maintaining a consistent sleep schedule could be a key modifiable factor for longevity, affecting public health guidelines and individual sleep habits. The study accounted for variables such as shift work and employment status, but critics note potential confounding from occupation and other factors like cosmic radiation exposure for frequent flyers.

hackernews · bilsbie · Jul 15, 11:46 · [Discussion](https://news.ycombinator.com/item?id=48919363)

**Background**: Sleep regularity refers to how consistent a person's sleep and wake times are from day to day, while sleep duration is the total amount of sleep. Previous research has emphasized duration for health outcomes, but this study highlights the importance of circadian rhythm alignment.

**Discussion**: Community comments provided diverse perspectives: one user credited magnesium supplementation for solving insomnia, while another explained the physiological benefits of a regular schedule. However, several commenters raised methodological concerns, such as confounding by occupation and the tendency for sensationalized findings in large-scale studies.

**Tags**: `#health`, `#sleep`, `#mortality`, `#research`, `#epidemiology`

---

<a id="item-5"></a>
## [Claude web_fetch data exfiltration via prompt injection](https://simonwillison.net/2026/Jul/15/claude-web-fetch-exfiltration/#atom-everything) ⭐️ 8.0/10

Researcher Ayush Paul demonstrated a prompt injection attack that bypassed Claude's web_fetch safeguards, tricking the AI into leaking private user data by following nested links from a honeypot site. This vulnerability shows that existing protections against data exfiltration in AI agents are still insufficient, highlighting the critical need for robust security measures as AI gains access to sensitive user data and external tools. The attack exploited a loophole where web_fetch was allowed to visit URLs embedded in previously fetched pages, so an attacker could craft a series of nested links to progressively extract user data such as name, city, and employer. Anthropic had already internally identified the issue and closed the hole by removing the ability for web_fetch to navigate to additional links from fetched content, thus no bug bounty was paid.

rss · Simon Willison · Jul 15, 14:21

**Background**: Prompt injection attacks occur when an attacker embeds malicious instructions in content that an AI processes, potentially overriding system safeguards. The 'lethal trifecta' refers to the combination of private data access, exposure to untrusted content, and ability to execute outbound actions—making AI agents vulnerable to data exfiltration. Claude's web_fetch tool was designed with protections such as only allowing navigation to user-specified or search-returned URLs, but the nested-link loophole bypassed this.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/">The lethal trifecta for AI agents: private data, untrusted content, and ...</a></li>
<li><a href="https://purplesec.us/learn/data-exfiltration-ai-prompt-injection/">Data Exfiltration Via AI Prompt Injection</a></li>
<li><a href="https://platform.claude.com/docs/en/agents-and-tools/tool-use/web-fetch-tool">Web fetch tool - Claude Platform Docs</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#security`, `#Claude`, `#data exfiltration`, `#prompt injection`

---

<a id="item-6"></a>
## [First Paper on Disentangling CNN Neuron via Hadamard Clustering](https://www.reddit.com/r/MachineLearning/comments/1uwya70/mechanistic_interpretability_a_first_paper_on/) ⭐️ 8.0/10

A new method uses Hadamard product clustering of a neuron's receptive field and weights to identify all patterns a single convolutional neuron detects, demonstrated on InceptionV1's 1x1 convolutions. This work provides a novel technique for mechanistic interpretability of CNNs, enabling detailed analysis of individual neurons and revealing how gradient descent distributes patterns into noisy ranges. The method produces clean monosemantic clusters (e.g., cars, cats, dogs) and also lower-valued clusters like letters; analysis shows dependent neurons fire on the same concept with balanced positive and negative weights to reduce the sum.

reddit · r/MachineLearning · /u/narang_27 · Jul 15, 06:59

**Background**: Mechanistic interpretability aims to reverse-engineer neural networks by understanding individual components. The Hadamard product is an element-wise matrix multiplication. InceptionV1 (GoogLeNet) is a deep CNN that uses 1x1 convolutions to reduce dimensionality, and this work focuses on neurons in its mixed4e layer.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hadamard_product_(matrices)">Hadamard product (matrices) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Inception_(deep_learning_architecture)">Inception (deep learning architecture) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#mechanistic interpretability`, `#convolutional neural networks`, `#neuron analysis`, `#InceptionV1`, `#interpretability`

---

<a id="item-7"></a>
## [PyTorch model 170x slower on T4 than A100](https://www.reddit.com/r/MachineLearning/comments/1ux6a9x/pytorch_model_running_170x_slower_on_t4_vs_a100/) ⭐️ 8.0/10

A developer reports that a point-tracking model with 4D correlation volumes and transformer layers runs 170x slower on an NVIDIA T4 GPU (85 seconds per half-video) compared to an A100 (0.5 seconds) when using pure FP32 precision. This extreme performance gap highlights how memory bandwidth limits and the lack of tensor core acceleration for pure FP32 on T4 can lead to severe bottlenecks, affecting deployment decisions for cost-sensitive applications. The model runs at 99% GPU utilization on both cards, ruling out CPU bottlenecks, and the same slowdown occurs on multiple T4 machines, eliminating driver or configuration issues.

reddit · r/MachineLearning · /u/Future-Structure-296 · Jul 15, 13:44

**Background**: The NVIDIA T4 has 2,560 CUDA cores and 320 Tensor Cores, but its Tensor Cores only accelerate mixed-precision (FP16, INT8) operations, not pure FP32. The A100 has 6,912 CUDA cores and 432 Tensor Cores that also accelerate FP32 via TF32 mode. Additionally, T4's memory bandwidth (320 GB/s) is much lower than A100's (2 TB/s for A100 80GB), and the 4D correlation volume construction involves heavy memory access, which hits T4's bandwidth limits harder.

<details><summary>References</summary>
<ul>
<li><a href="https://www.techpowerup.com/gpu-specs/tesla-t4.c3316">NVIDIA Tesla T4 Specs | TechPowerUp GPU Database</a></li>
<li><a href="https://arxiv.org/html/2505.16942">Efficient Correlation Volume Sampling for Ultra-High-Resolution Optical Flow Estimation</a></li>

</ul>
</details>

**Tags**: `#PyTorch`, `#GPU Performance`, `#Model Optimization`, `#NVIDIA T4`, `#A100`

---

<a id="item-8"></a>
## [DeepSeek plans IPO by 2027, seeks new funding at $71B valuation](https://t.me/zaihuapd/42577) ⭐️ 8.0/10

DeepSeek has initiated IPO preparations, aiming to file by end of 2024 or early 2025, with a target listing in 2027, while simultaneously seeking a new fundraising round at a pre-investment valuation of at least 4800 billion RMB (about $71 billion). This marks a major milestone for a leading Chinese AI startup, reflecting strong market confidence and potentially reshaping the AI industry's funding landscape, especially given DeepSeek's cost-efficient model development. The new funding round aims to raise at least 10 billion RMB, which could multiply based on investor interest; DeepSeek completed its first external funding of $700 million in June 2024 from investors including Tencent and CATL.

telegram · zaihuapd · Jul 15, 07:04

**Background**: DeepSeek, founded in July 2023 by Liang Wenfeng, is a Chinese AI company known for its open-weight large language models like DeepSeek-R1, which rivaled GPT-4 at a fraction of the cost. The company is owned by hedge fund High-Flyer and made headlines for its low training costs despite US chip export restrictions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek_(Company)">DeepSeek (Company)</a></li>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek_(chatbot)">DeepSeek (chatbot) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#IPO`, `#AI`, `#funding`, `#startup`

---

<a id="item-9"></a>
## [Judge Questions Epic-Google $800M Deal Weakening Antitrust Case](https://t.me/zaihuapd/42588) ⭐️ 8.0/10

A U.S. judge revealed that Epic Games and Google have entered a new commercial partnership worth approximately $800 million over six years, covering joint product development, marketing, and partnerships involving Unreal Engine, Fortnite, and Android. The judge questioned whether this deal undermines Epic's antitrust position against Google in the ongoing lawsuit. This case could set a precedent for app store policies and competition on Android, affecting how developers distribute apps and pay fees. If Epic's antitrust claims are weakened by this deal, it may reduce pressure on Google to change its Play Store policies. The deal includes Epic paying Google approximately $800 million over six years, with collaboration on Unreal Engine, Fortnite, and Android-related ventures. Judge James Donato expressed concern that the commercial agreement could conflict with Epic's push for Android ecosystem reforms.

telegram · zaihuapd · Jul 15, 11:15

**Background**: Epic Games sued Google in 2020, alleging anticompetitive practices in the Play Store, such as requiring developers to use Google's billing system and taking a 30% cut. The case is part of broader antitrust scrutiny on major tech platforms. A commercial deal between the two parties raises questions about the sincerity of Epic's antitrust challenge.

**Tags**: `#antitrust`, `#Epic Games`, `#Google`, `#Android`, `#legal`

---

<a id="item-10"></a>
## [DeepSeek Raises Over $7.4B in First Round with Unusual Control Structure](https://t.me/zaihuapd/42589) ⭐️ 8.0/10

DeepSeek has completed its first funding round, raising over 500 billion RMB (approximately $74 billion) at a valuation exceeding $50 billion. The round uses an unconventional structure where investors put money into a limited partnership managed by CEO Liang Wenfeng, accepting a five-year lock-up period with no voting rights. This massive funding round marks one of the largest in AI history, signaling strong investor confidence in DeepSeek’s technology and market potential. The unique control structure ensures founder Liang Wenfeng retains decision-making power, setting a precedent for other startups seeking to balance capital needs with founder control. Founder Liang Wenfeng personally invested 200 billion RMB in this round. Tencent and CATL are considering or planning to invest 100 billion RMB and 50 billion RMB respectively, potentially becoming the largest external investors. DeepSeek has not commented on the reports.

telegram · zaihuapd · Jul 15, 12:56

**Background**: DeepSeek is a Chinese AI startup gaining attention for its advanced large language models. The company's unusual funding structure involves a limited partnership that holds shares, allowing investors to provide capital without diluting founder control or gaining voting rights, which is rare in large financing rounds.

**Tags**: `#DeepSeek`, `#AI`, `#funding`, `#startup`, `#venture capital`

---

<a id="item-11"></a>
## [Telegram Serverless Platform: No Server Needed for Bots](https://core.telegram.org/bots/serverless) ⭐️ 8.0/10

Telegram has launched a serverless platform that allows developers to deploy JavaScript backend code for bots and Mini Apps directly on Telegram's infrastructure using a single command. This simplifies bot development by eliminating server management and scaling concerns, making it easier for developers to build and deploy bots within the Telegram ecosystem. Code runs in an isolated V8 sandbox adjacent to the Bot API, with a built-in SQLite database. Deployment is done via npx tgcloud push.

telegram · zaihuapd · Jul 15, 16:00

**Background**: Traditionally, Telegram bot backends required developers to host their own servers or use third-party cloud services. This new platform provides a native serverless alternative integrated directly with Telegram's Bot API, reducing overhead for developers.

<details><summary>References</summary>
<ul>
<li><a href="https://core.telegram.org/bots/serverless">Telegram Serverless</a></li>
<li><a href="https://github.com/btwiuse/tgcloud/blob/main/README.md">tgcloud/README.md at main · btwiuse/tgcloud · GitHub</a></li>

</ul>
</details>

**Tags**: `#Telegram`, `#Serverless`, `#Bots`, `#JavaScript`, `#Platform`

---