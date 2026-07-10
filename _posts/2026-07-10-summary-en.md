---
layout: default
title: "Horizon Summary: 2026-07-10 (EN)"
date: 2026-07-10
lang: en
---

> From 58 items, 15 important content pieces were selected

---

1. [SGLang v0.5.15 Boosts GLM-5.2 NVFP4 on Blackwell](#item-1) ⭐️ 8.0/10
2. [QuadRF: Open-Source SDR Detects Drones and WiFi](#item-2) ⭐️ 8.0/10
3. [GPT-5.6 Sol Ultra Generates Proof of Cycle Double Cover Conjecture](#item-3) ⭐️ 8.0/10
4. [Good Tools Are Invisible](#item-4) ⭐️ 8.0/10
5. [How Successful Companies Go Blind](#item-5) ⭐️ 8.0/10
6. [SK Hynix CEO: Memory Chip Shortage May Last Beyond 2030](#item-6) ⭐️ 8.0/10
7. [SK Hynix CEO Predicts Worst Memory Shortage by 2027](#item-7) ⭐️ 8.0/10
8. [Apple Sues OpenAI for Trade Secret Theft](#item-8) ⭐️ 8.0/10
9. [Chinese Courts Rule Game Accounts Inheritable, Invalidating Platform Bans](#item-9) ⭐️ 8.0/10
10. [Anthropic Web Crawler Referral Ratio Hits 2800:1](#item-10) ⭐️ 8.0/10
11. [Long March 10B achieves world's first net-based rocket recovery at sea](#item-11) ⭐️ 8.0/10
12. [Tencent in Talks to Acquire AI Startup Manus from Meta](#item-12) ⭐️ 8.0/10
13. [OpenAI, Google reportedly serve AI to blacklisted Chinese firms via Singapore](#item-13) ⭐️ 8.0/10
14. [China Imposes Temporary Ban on Helium Exports](#item-14) ⭐️ 8.0/10
15. [Meta faces $120B EU fine over addictive design](#item-15) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [SGLang v0.5.15 Boosts GLM-5.2 NVFP4 on Blackwell](https://github.com/sgl-project/sglang/releases/tag/v0.5.15) ⭐️ 8.0/10

SGLang v0.5.15 delivers optimized serving for GLM-5.2 using NVFP4 precision on Blackwell GPUs, achieving over 500 tokens/second/user on 8x B300 with speculative decoding improvements including Spec V2 and IndexShare MTP. This release significantly improves inference throughput for large language models on cutting-edge hardware, reducing latency and cost for production deployments, and demonstrates practical advances in speculative decoding and low-precision inference. Key optimizations include CUDA-graphable DSA draft-extend eliminating synchronization overhead (+11% TPS), IndexShare MTP reusing indexer top-k across draft steps (up to 1.9x lower cost), and fusion of 12 kernels into 4 (~8% faster decode).

github · Fridge003 · Jul 10, 22:58

**Background**: NVFP4 is a 4-bit floating point format introduced with NVIDIA's Blackwell architecture, enabling efficient low-precision inference. SGLang is an inference engine for large language models that leverages speculative decoding to generate multiple tokens per step, reducing latency. IndexShare is a cross-layer reuse trick for sparse attention, reducing computation in long-context scenarios.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/introducing-nvfp4-for-efficient-and-accurate-low-precision-inference/">Introducing NVFP4 for Efficient and Accurate Low-Precision ...</a></li>
<li><a href="https://articles.phantom-byte.com/the-1m-context-mirage-what-indexshare-actually-delivers.html">1M Context Mirage: What IndexShare Delivers - PhantomByte</a></li>
<li><a href="https://sebastianraschka.com/blog/2026/glm-5-2-indexshare.html">GLM-5.2 IndexShare Architecture Note | Sebastian Raschka, PhD</a></li>

</ul>
</details>

**Tags**: `#AI inference`, `#LLM serving`, `#GPU optimization`, `#speculative decoding`

---

<a id="item-2"></a>
## [QuadRF: Open-Source SDR Detects Drones and WiFi](https://www.jeffgeerling.com/blog/2026/quadrf-can-spot-drones-and-see-wifi-through-my-wall/) ⭐️ 8.0/10

Jeff Geerling's blog post demonstrates the QuadRF, an open-source 4x4 MIMO software-defined radio (SDR) tile that can detect drones and WiFi signals through walls using beamforming. This project makes phased-array beamforming technology affordable and accessible to hobbyists, security researchers, and the open-source community, potentially enabling new RF detection applications and raising privacy awareness. QuadRF is a 4-element SDR tile with an open antenna architecture, available via Crowd Supply. It uses software-defined radio to analyze RF signals, with ongoing UI improvements based on user feedback.

hackernews · speckx · Jul 10, 15:59 · [Discussion](https://news.ycombinator.com/item?id=48861717)

**Background**: Software-defined radio (SDR) implements radio components in software rather than hardware, allowing flexible signal processing. Phased-array beamforming uses multiple antennas to steer signal direction electronically. QuadRF combines these to detect and locate RF sources like drones and WiFi devices.

<details><summary>References</summary>
<ul>
<li><a href="https://www.crowdsupply.com/scale-rf/quadrf">QuadRF | Crowd Supply</a></li>
<li><a href="https://www.rtl-sdr.com/quadrf-4-element-beamforming-sdr-tile-coming-to-crowd-supply/">QuadRF: 4-Element Beamforming SDR Tile Coming to Crowd Supply</a></li>

</ul>
</details>

**Discussion**: The QuadRF creator engaged in the comments, answering questions about calibration and gain settings. Users discussed potential applications like sound detection and expressed both excitement about open-source RF tools and concerns about government surveillance capabilities.

**Tags**: `#hardware`, `#security`, `#RF`, `#open-source`, `#drones`

---

<a id="item-3"></a>
## [GPT-5.6 Sol Ultra Generates Proof of Cycle Double Cover Conjecture](https://cdn.openai.com/pdf/04d1d1e4-bc75-476a-97cf-49055cd98d31/cdc_proof.pdf) ⭐️ 8.0/10

OpenAI's GPT-5.6 Sol Ultra model has reportedly produced a proof of the Cycle Double Cover Conjecture, a long-standing open problem in graph theory. The proof was released as a preprint on July 10, 2026, along with the prompt used to generate it. If verified, this would mark a major breakthrough in both mathematics and AI, demonstrating that large language models can solve open mathematical problems. The result could shift perceptions of AI's role in theoretical research and automated theorem proving. The proof is extremely concise, which has sparked skepticism among experts. The model used a 'max reasoning effort' and 'ultra mode' with subagents to accelerate complex work, as described in OpenAI's preview of GPT-5.6 Sol.

hackernews · scrlk · Jul 10, 18:29 · [Discussion](https://news.ycombinator.com/item?id=48863490)

**Background**: The Cycle Double Cover Conjecture asks whether every bridgeless undirected graph has a collection of cycles such that each edge appears exactly twice. It was posed by W. T. Tutte, Itai and Rodeh, George Szekeres, and Paul Seymour. GPT-5.6 Sol Ultra is OpenAI's most advanced model, released in 2026, with tiers Luna, Terra, and Sol, where Sol supports extended reasoning.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cycle_double_cover_conjecture">Cycle double cover conjecture</a></li>
<li><a href="https://openai.com/index/previewing-gpt-5-6-sol/">Previewing GPT - 5 . 6 Sol : a next-generation model | OpenAI</a></li>

</ul>
</details>

**Discussion**: Community comments express both excitement and skepticism. Some note that the proof is concise and might exploit a clever trick experts missed, while others question whether this truly constitutes an autonomous 'theory-building' proof. There is also interest in the systematic testing of frontier models on open problems.

**Tags**: `#AI`, `#mathematics`, `#graph theory`, `#proof`, `#GPT-5.6`

---

<a id="item-4"></a>
## [Good Tools Are Invisible](https://www.gingerbill.org/article/2026/07/10/good-tools-are-invisible/) ⭐️ 8.0/10

The article argues that good tools minimize friction and become invisible, allowing users to focus on their tasks rather than the tool itself. This philosophy challenges common design practices that add unnecessary complexity, impacting how developers and designers approach tool creation for better user experience. The article discusses the concept of 'discretionary friction' and notes that making tools invisible is a function of time spent using them, not just initial design.

hackernews · theanonymousone · Jul 10, 10:32 · [Discussion](https://news.ycombinator.com/item?id=48858121)

**Background**: The idea that tools should be invisible is common in UX design, often associated with the principle of 'don't make me think.' Good tools fit so naturally that users don't notice them.

**Discussion**: Commenters generally agree but offer nuance. Some note that invisibility depends on user experience, and that friction can be necessary for complex tasks. Others debate the value of keyboard vs. mouse interfaces.

**Tags**: `#tool-design`, `#UX`, `#developer-experience`, `#philosophy`

---

<a id="item-5"></a>
## [How Successful Companies Go Blind](https://ianreppel.org/how-successful-companies-go-blind/) ⭐️ 8.0/10

The article analyzes how successful companies develop internal blindness to their own flaws, leading to stagnation and decline. This matters because it highlights a common pattern in organizational decline that affects profitability and innovation, relevant to managers and engineers. The article uses examples from various industries and discusses how bureaucracy, risk aversion, and lack of fresh perspectives contribute to this blindness.

hackernews · speckx · Jul 10, 13:31 · [Discussion](https://news.ycombinator.com/item?id=48859678)

**Background**: Organizational blindness refers to a situation where a company becomes unaware of its own weaknesses due to past success, creating a culture resistant to change. This concept is common in business management literature.

**Discussion**: Commenters shared personal experiences, with one noting that in defense companies, momentum and lack of financial incentives stifle innovation. Another pointed out that long-tenured managers often lack upskilling. A third argued it's more about context than competence, as talented people can be hindered by bureaucracy.

**Tags**: `#organizational behavior`, `#company culture`, `#business strategy`, `#management`

---

<a id="item-6"></a>
## [SK Hynix CEO: Memory Chip Shortage May Last Beyond 2030](https://t.me/FinanceNewsDaily/490418) ⭐️ 8.0/10

SK Hynix CEO Kwak Noh-Jung stated in a Bloomberg TV interview that the memory chip supply shortage could persist beyond 2030. This long-term forecast from a top memory chip maker signals sustained pressure on global tech supply chains, affecting industries from data centers to consumer electronics. The CEO did not specify exact reasons but highlighted structural challenges in the semiconductor industry, including capacity expansion delays and rising demand.

telegram · FinanceNewsDaily · Jul 10, 17:40

**Background**: Memory chips, including DRAM and NAND flash, are essential components in computers, smartphones, and servers. The industry has experienced cyclical shortages, but recent geopolitical tensions and pandemic-driven demand have exacerbated supply constraints.

**Tags**: `#memory chips`, `#semiconductor supply chain`, `#SK Hynix`, `#hardware`, `#industry forecast`

---

<a id="item-7"></a>
## [SK Hynix CEO Predicts Worst Memory Shortage by 2027](https://t.me/FinanceNewsDaily/490420) ⭐️ 8.0/10

SK Hynix CEO Kwak Noh-jung stated that the global memory industry is heading towards the most severe supply shortage in history by 2027, with demand expected to outpace the company's production capacity for the next decade. This prediction from a leading memory manufacturer signals a potential major disruption in the semiconductor market, which could impact prices and availability of memory chips used in everything from smartphones to data centers. Kwak noted that despite aggressive capacity expansion, demand will exceed supply for the next ten years, and he described 2027 as the worst year from a supply perspective. The statement was reported by Reuters.

telegram · FinanceNewsDaily · Jul 10, 19:50

**Background**: Memory chips, including DRAM and NAND flash, are critical components in electronic devices. The semiconductor industry has historically experienced cycles of shortages and gluts, driven by fluctuating demand and long lead times for new fabrication plants. A prolonged shortage could constrain production of consumer electronics and cloud infrastructure.

**Tags**: `#memory`, `#semiconductor`, `#shortage`, `#SK Hynix`, `#industry forecast`

---

<a id="item-8"></a>
## [Apple Sues OpenAI for Trade Secret Theft](https://t.me/FinanceNewsDaily/490421) ⭐️ 8.0/10

Apple filed a major lawsuit against OpenAI, alleging the company stole trade secrets and encouraged employees to share confidential information. This lawsuit could set a precedent for intellectual property disputes in the AI industry, affecting how companies protect trade secrets and collaborate with competitors. Apple claims that OpenAI encouraged its employees to share confidential information, potentially exposing proprietary technologies developed by Apple.

telegram · FinanceNewsDaily · Jul 10, 20:35

**Background**: Apple and OpenAI are major players in the AI sector, with Apple integrating AI into its products while OpenAI develops advanced models like GPT. Trade secret lawsuits are rare but significant, as they can reveal internal practices and lead to injunctions or damages.

**Tags**: `#Apple`, `#OpenAI`, `#lawsuit`, `#trade secrets`, `#AI`

---

<a id="item-9"></a>
## [Chinese Courts Rule Game Accounts Inheritable, Invalidating Platform Bans](https://www.tomshardware.com/tech-industry/big-tech/chinese-courts-allow-heirs-to-inherent-accounts-of-deceased-gamers-multiple-cases-spanning-years-establish-precedent-for-digital-ownership-of-games-in-game-items-and-microtransactions) ⭐️ 8.0/10

Chinese courts have issued multiple rulings across several years that digital game accounts, in-game items, cryptocurrencies, and social media operation rights constitute inheritable property. These decisions invalidate platform terms of service that prohibit inheritance of such accounts. This establishes a landmark legal precedent for digital asset inheritance rights in China, potentially affecting millions of users and forcing platform policies to change. It could influence global discussions on digital property rights and user ownership of virtual assets. The courts ruled that chat records and other purely private content are not inheritable, and platforms may charge reasonable fees for transferring accounts to heirs. The rulings are based on the Civil Code of the People's Republic of China, which includes virtual property as part of estate.

telegram · zaihuapd · Jul 10, 02:56

**Background**: The concept of digital inheritance involves the transfer of digital assets—such as online accounts, cryptocurrencies, and virtual items—after a person's death. In China, the Civil Code, effective since 2021, notes that virtual property is protected by law, but its inheritance specifics have been debated. These court cases clarify that digital assets with economic value can be inherited, even if platform terms say otherwise.

<details><summary>References</summary>
<ul>
<li><a href="https://ailegal.baidu.com/legalarticle/qadetail?id=10903050849a99251031">网络虚拟财产继承经典法院案例 - ailegal.baidu.com</a></li>
<li><a href="https://www.lutongls.com/minshi/470.html">我国虚拟财产继承法律问题研究-上海陆同律师事务所</a></li>
<li><a href="https://china.cnr.cn/gdgg/20221002/t20221002_526026303.shtml">china.cnr.cn/gdgg/20221002/t20221002_526026303.shtml</a></li>

</ul>
</details>

**Tags**: `#digital inheritance`, `#Chinese law`, `#virtual property`, `#gaming`, `#digital rights`

---

<a id="item-10"></a>
## [Anthropic Web Crawler Referral Ratio Hits 2800:1](https://www.businessinsider.com/anthropic-web-bots-crawling-referrals-cloudflare-distillation-2026-7) ⭐️ 8.0/10

According to Cloudflare data from July 1-7, 2026, Anthropic's web crawler brings back only one referral visit for every 2800 pages scraped, the highest crawl-to-refer ratio among major AI companies. This imbalance highlights how AI companies consume vast amounts of web content for training while providing minimal traffic back to publishers, raising ethical and economic concerns about content licensing and the sustainability of open web resources. The ratio has improved from about 8800:1 in early April 2026 but spiked to 24700:1 in the first week of May. Anthropic has questioned Cloudflare's methodology, stating they cannot verify the calculations and that their new search feature is increasing referral traffic.

telegram · zaihuapd · Jul 10, 04:25

**Background**: Cloudflare Radar tracks the crawl-to-refer ratio, comparing how often AI bots crawl a site versus how often they send users back to that site via referrals. This metric has become important as AI training drives nearly 80% of AI crawling by mid-2025, according to Cloudflare, while referrals to publishers decline. Major AI companies like OpenAI, Google, and Anthropic face scrutiny over their scraping practices and their impact on the web ecosystem.

<details><summary>References</summary>
<ul>
<li><a href="https://www.businessinsider.com/anthropic-web-bots-crawling-referrals-cloudflare-distillation-2026-7">Anthropic Treats the Web Like an All-You-Can-Eat... - Business Insider</a></li>
<li><a href="https://blog.cloudflare.com/ai-search-crawl-refer-ratio-on-radar/">The crawl before the fall… of referrals : understanding AI’s impact on...</a></li>
<li><a href="https://privacy.anthropic.com/en/articles/10023637-does-anthropic-crawl-data-from-the-web-and-how-can-site-owners-block-the-crawler">Does Anthropic crawl data from the web , and how can site owners...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#web scraping`, `#content licensing`, `#traffic analytics`, `#Anthropic`

---

<a id="item-11"></a>
## [Long March 10B achieves world's first net-based rocket recovery at sea](https://weibo.com/7340734455/R814of1Ki) ⭐️ 8.0/10

On July 10, 2026, China's Long March 10B rocket launched from Hainan Commercial Space Launch Site and successfully recovered its first stage via net-based capture at sea about 6 minutes after stage separation, marking the world's first net-based recovery of a rocket first stage. This breakthrough demonstrates a novel reusable rocket technology that eliminates the need for landing legs, potentially reducing costs and complexity for future space missions, and positions China as a leader in rocket recovery alongside SpaceX's propulsive landing approach. The recovery uses a shipboard net system with arresting cables that catch the rocket's hook, enabling a low-shock, reusable touchdown without landing gear. The Long March 10B is the first Chinese launcher to achieve controlled recovery of its first stage.

telegram · zaihuapd · Jul 10, 04:36

**Background**: Rocket first-stage recovery is key to reusability, reducing launch costs. SpaceX pioneered propulsive landings on drone ships and ground pads. China's net-based method offers an alternative that avoids complex landing gear and precise engine burns, potentially simplifying the recovery process for certain missions.

<details><summary>References</summary>
<ul>
<li><a href="http://www.ce.cn/xwzx/gnsz/gdxw/202607/t20260710_3080704.shtml">ce.cn/xwzx/gnsz/gdxw/202607/t20260710_3080704.shtml</a></li>
<li><a href="https://www.spacechina.com/n25/n2014789/n2414549/c4646874/content.html">长十乙火箭成功实现一子级可控回收_中国航天科技集团</a></li>
<li><a href="https://www.locpg.gov.cn/20260710/90f9157af72247dc9c5524ab8013da0a/c.html">长征十号乙运载火箭实现一子级可控回收</a></li>

</ul>
</details>

**Tags**: `#aerospace`, `#rocket recovery`, `#China space`, `#engineering`

---

<a id="item-12"></a>
## [Tencent in Talks to Acquire AI Startup Manus from Meta](https://www.reuters.com/technology/tencent-talks-become-ai-start-up-manus-largest-shareholder-ft-reports-2026-07-10/) ⭐️ 8.0/10

Tencent is negotiating to acquire AI startup Manus and become its largest shareholder by repurchasing shares from Meta for at least $2 billion, alongside original investors ZhenFund and HSG. This deal reflects the intensifying competition in the AI sector and geopolitical tensions, as Beijing previously required Meta to unwind its acquisition of Manus. It also marks Tencent's strategic push into AI agent technology. The transaction is valued at no less than $2 billion, with Tencent joining forces with existing investors ZhenFund and HSG to buy out Meta's stake. The news was first reported by the Financial Times; Tencent, Manus, Meta, and the investors declined to comment.

telegram · zaihuapd · Jul 10, 06:45

**Background**: Manus is an AI agent platform described as an 'action engine' that goes beyond conversational AI to plan and execute multi-step tasks such as research, analysis, browsing, and building. The startup was previously acquired by Meta, but Beijing ordered Meta to divest due to regulatory concerns. Tencent, a Chinese tech giant, is seeking to expand its AI capabilities amid fierce competition in the sector.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/Manus_AI_company">Manus ( AI company ) — Grokipedia</a></li>
<li><a href="https://manus.im/">Manus : Hands On AI</a></li>
<li><a href="https://medium.com/@fahey_james/manus-ai-company-profile-352cf236db47">Manus AI company profile | by James Fahey | Medium</a></li>

</ul>
</details>

**Tags**: `#Tencent`, `#Meta`, `#AI`, `#acquisition`, `#Manus`

---

<a id="item-13"></a>
## [OpenAI, Google reportedly serve AI to blacklisted Chinese firms via Singapore](https://www.ft.com/content/5d6aafa1-5d47-4585-aa95-6ec06a6cd20f) ⭐️ 8.0/10

OpenAI and Google have been providing advanced AI services to Singapore subsidiaries of Alibaba, Baidu, and Tencent, whose parent companies are on the US Department of Defense's Section 1260H list of alleged Chinese military companies. This raises fresh questions about the effectiveness of US export controls on AI technology, as companies can still access advanced models through overseas subsidiaries, potentially undermining national security policies. OpenAI previously suspended API access for an Alibaba-affiliated user after detecting suspected 'model distillation' and reported it to US authorities, while Anthropic has adopted a stricter policy barring all Chinese entities including overseas affiliates.

telegram · zaihuapd · Jul 10, 09:59

**Background**: The Section 1260H list, maintained by the US Department of Defense, identifies Chinese companies alleged to have ties to the People's Liberation Army. Model distillation is a technique that transfers knowledge from a large AI model to a smaller one, which can be used to evade API restrictions. Current US export controls do not broadly prohibit Chinese parent companies from accessing advanced AI models outside mainland China.

<details><summary>References</summary>
<ul>
<li><a href="https://www.war.gov/News/Releases/Release/Article/4511232/dow-releases-list-of-chinese-military-companies-in-accordance-with-section-1260/">DOW Releases List of Chinese Military Companies in Accordance ...</a></li>
<li><a href="https://www.ibm.com/think/topics/knowledge-distillation">What is Knowledge distillation? | IBM</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#export controls`, `#OpenAI`, `#Google`, `#China`

---

<a id="item-14"></a>
## [China Imposes Temporary Ban on Helium Exports](https://wms.mofcom.gov.cn/zcfb/wmgl/art/2026/art_2a795a0d55df4cada91c9fbd2a2cc13a.html) ⭐️ 8.0/10

On July 10, 2026, China's Ministry of Commerce and General Administration of Customs jointly issued a notice imposing a temporary export ban on helium (HS code 2804290010), effective immediately. This policy significantly tightens global helium supply, as China is a major producer; it will likely disrupt semiconductor manufacturing, medical imaging, and scientific research that rely on helium. The ban applies to all exports of the listed helium product, with no specified end date; future adjustments will be announced separately, and the measure is based on China's Foreign Trade Law.

telegram · zaihuapd · Jul 10, 13:27

**Background**: Helium is a non-renewable noble gas critical for cryogenics, welding, and as a cooling agent in MRI machines and semiconductor fabrication. China has been increasing its helium production capacity, and such export controls can be used as a strategic tool in technology competition.

**Tags**: `#helium`, `#trade policy`, `#supply chain`, `#semiconductors`, `#science`

---

<a id="item-15"></a>
## [Meta faces $120B EU fine over addictive design](https://www.theverge.com/policy/963872/meta-eu-addictive-design-200b-fine-risk-digital-services-act-dsa) ⭐️ 8.0/10

The European Commission preliminarily found that Meta's Facebook and Instagram violate the Digital Services Act (DSA) through addictive design features such as infinite scroll, autoplay, and personalized recommendations. If finalized, Meta could face a fine of up to $12 billion (6% of annual global revenue), setting a landmark precedent for enforcing user safety regulations under the DSA and forcing major platforms to redesign core engagement features. The EU criticized Meta's existing time-limiting tools as ineffective and demanded default deactivation of addictive features, effective screen-time breaks, and de-emphasis of engagement-driven algorithms.

telegram · zaihuapd · Jul 10, 14:47

**Background**: The Digital Services Act (DSA) is an EU regulation that took effect in 2022, establishing comprehensive rules for digital services accountability. It imposes the strictest obligations on Very Large Online Platforms (VLOPs) like Facebook and Instagram, which have over 45 million monthly active users in the EU. The DSA requires platforms to assess and mitigate systemic risks, including those to users' mental health.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Digital_Services_Act">Digital Services Act</a></li>
<li><a href="https://grokipedia.com/page/Digital_Services_Act">Digital Services Act</a></li>

</ul>
</details>

**Tags**: `#regulation`, `#Meta`, `#EU`, `#Digital Services Act`, `#addictive design`

---