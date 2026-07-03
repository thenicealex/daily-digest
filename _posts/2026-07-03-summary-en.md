---
layout: default
title: "Horizon Summary: 2026-07-03 (EN)"
date: 2026-07-03
lang: en
---

> From 74 items, 12 important content pieces were selected

---

1. [European Parliament Spy Probe Member Hacked with Pegasus](#item-1) ⭐️ 8.0/10
2. [Guide to Running SOTA LLMs Locally](#item-2) ⭐️ 8.0/10
3. [Wordgard: New Rich-Text Editor from ProseMirror Creator](#item-3) ⭐️ 8.0/10
4. [Tool cuts LLM costs 60% by sending code as images](#item-4) ⭐️ 8.0/10
5. [Critique of MVP Misuse and Founder Motivation](#item-5) ⭐️ 8.0/10
6. [CDD recovers verbatim finetuning data from logits alone](#item-6) ⭐️ 8.0/10
7. [China NFRA Takes Over Zhongbang Bank Over Credit Risk](#item-7) ⭐️ 8.0/10
8. [Anthropic Accuses Alibaba of Massive Distillation Attack on Claude](#item-8) ⭐️ 8.0/10
9. [Huawei Atlas 350 AI card claims 2.87x H20 performance](#item-9) ⭐️ 8.0/10
10. [Alibaba bans all employees from using Claude, Anthropic products](#item-10) ⭐️ 8.0/10
11. [NASA Launches Rescue Satellite to Save Falling Space Telescope](#item-11) ⭐️ 8.0/10
12. [Tencent's Atuin AI beats Mythos in CyberGym benchmark](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [European Parliament Spy Probe Member Hacked with Pegasus](https://citizenlab.ca/research/member-of-committee-investigating-spyware-hacked-with-pegasus/) ⭐️ 8.0/10

Citizen Lab discovered that Stelios Kouloglou, a member of the European Parliament's committee investigating spyware, had his iPhone infected with Pegasus spyware in October 2022 and again in March 2023. This case underscores the irony and danger of an investigator of spyware being targeted by the same technology, revealing persistent espionage threats against EU institutions and the need for heightened cybersecurity measures. The infections were confirmed with high confidence by Citizen Lab, and the compromised phone also contained confidential personal medical information and government documents, raising concerns about the lack of separation between work and personal devices.

hackernews · ledoge · Jul 3, 20:38 · [Discussion](https://news.ycombinator.com/item?id=48779683)

**Background**: Pegasus is a powerful commercial spyware developed by Israeli firm NSO Group, designed to remotely and covertly surveil mobile devices. Citizen Lab, based at the University of Toronto, is a leading research organization that investigates digital espionage and has exposed multiple abuses of Pegasus worldwide. Kouloglou was part of the European Parliament's committee investigating the use of spyware like Pegasus within the EU.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pegasus_(spyware)">Pegasus (spyware)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Citizen_Lab">Citizen Lab</a></li>

</ul>
</details>

**Discussion**: Community comments highlight the ongoing Greek spyware scandal, suggesting the attack may have been orchestrated by the Greek government rather than foreign actors. Some discuss device security, noting that using separate work and personal devices or enhanced privacy OS like GrapheneOS could have mitigated the risk. Others point out that EU member states have abused Pegasus, undermining trust within the union.

**Tags**: `#spyware`, `#Pegasus`, `#cybersecurity`, `#European Parliament`, `#Citizen Lab`

---

<a id="item-2"></a>
## [Guide to Running SOTA LLMs Locally](https://github.com/jamesob/local-llm) ⭐️ 8.0/10

A new GitHub guide by Jamesob provides a detailed breakdown of hardware setups for running state-of-the-art large language models locally, ranging from budget to high-end configurations costing up to $50,000. This guide addresses the growing interest in local AI inference, offering practical advice for enthusiasts and professionals who want privacy, offline access, or to avoid subscription costs, while also sparking debate on cost-effectiveness versus cloud services. The highest-end build uses four $12,000 GPUs, totaling around $50,000, and claims to approach Claude Opus-level performance; lower-cost options include dual RTX 3090s (48 GB VRAM) for around $3,000 or unified memory systems like the M5 MacBook Pro.

hackernews · livestyle · Jul 3, 15:03 · [Discussion](https://news.ycombinator.com/item?id=48775921)

**Background**: Running LLMs locally requires significant GPU memory (VRAM) for model weights, often leading to quantization to reduce memory usage. High-end setups can cost tens of thousands of dollars, while cloud subscriptions like Claude Opus ($200/month) offer cheaper alternatives. This guide helps users navigate hardware choices for different budgets.

**Discussion**: Commenters debate cost-effectiveness, with jacobgold noting that a $40K build equals 16.8 years of Claude subscription. Others suggest alternatives like 128 GB unified memory systems or cloud hosting, while Aurornis warns of hidden costs and reliance on quantization.

**Tags**: `#LLMs`, `#local inference`, `#hardware`, `#GPU`, `#AI`

---

<a id="item-3"></a>
## [Wordgard: New Rich-Text Editor from ProseMirror Creator](https://wordgard.net/) ⭐️ 8.0/10

Wordgard 0.1.0 has been released, a new in-browser rich-text editor created by Marijn Haverbeke, the same developer behind ProseMirror. It shares many concepts with ProseMirror but introduces a redesigned architecture and a custom document model. Wordgard represents a significant evolution in rich-text editing for the web, coming from a trusted author, but it requires substantial migration effort for existing ProseMirror users. This could fragment the ecosystem or drive innovation. There is no direct upgrade path from ProseMirror to Wordgard, as stated in its documentation. The editor is still in early development (version 0.1.0) and the creator has assured that ProseMirror will not be abandoned.

hackernews · indy · Jul 3, 08:50 · [Discussion](https://news.ycombinator.com/item?id=48772573)

**Background**: ProseMirror is a widely-used open-source library for building rich-text editors with a WYSIWYG interface, known for its extensible schema and collaborative editing support. It is the foundation for editors like Tiptap. Wordgard is a new system by the same author that rethinks some of ProseMirror's core decisions.

<details><summary>References</summary>
<ul>
<li><a href="https://discuss.prosemirror.net/t/wordgard-0-1-0/9035">Wordgard 0.1.0 - Announce - discuss.ProseMirror</a></li>
<li><a href="https://prosemirror.net/">ProseMirror</a></li>

</ul>
</details>

**Discussion**: The community discussion is generally positive but notes the lack of migration path. One user praised the design, while another expressed relief at seeing similarities to their own block-based approach. A commenter highlighted the need for a web standard for such editors.

**Tags**: `#rich-text editor`, `#ProseMirror`, `#web development`, `#WYSIWYG`

---

<a id="item-4"></a>
## [Tool cuts LLM costs 60% by sending code as images](https://github.com/teamchong/pxpipe) ⭐️ 8.0/10

A new tool called pxpipe converts code into images and sends them to an LLM, exploiting cheaper image token pricing to reduce API costs by up to 60%. This clever hack significantly cuts the cost of using LLMs for code-related tasks, making them more accessible, and highlights pricing inconsistencies in LLM APIs that may be exploited. The tool works by formatting code as an image and relying on the LLM's built-in OCR capabilities to read the text, with savings stemming from lower image token prices. However, this may be a temporary loophole if providers adjust their token accounting.

hackernews · dimitropoulos · Jul 3, 15:50 · [Discussion](https://news.ycombinator.com/item?id=48776464)

**Background**: LLMs typically charge per token for both text and images, with image tokens often priced lower. Some providers like Gemini handle PDFs by internally performing OCR without charging for text tokens, suggesting similar backend processes might exist. This tool exploits such pricing differences to reduce costs for code inputs.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.roboflow.com/image-token-cost-vlm/">What does it cost to process an image with a vision model?</a></li>
<li><a href="https://cloud.google.com/blog/products/ai-machine-learning/what-is-ocr">What is OCR | Google Cloud Blog</a></li>

</ul>
</details>

**Discussion**: Commenters noted that this might be a loophole in token accounting that could be closed, similar to past attempts with OpenAI models that led to higher overall costs due to increased completion tokens. Others compared it to tools like Oh-My-Pi that use images for context compression, and one joked about rediscovering compressed data representations.

**Tags**: `#LLM`, `#cost optimization`, `#hack`, `#OCR`, `#token pricing`

---

<a id="item-5"></a>
## [Critique of MVP Misuse and Founder Motivation](https://weli.dev/blog/half-baked-product/) ⭐️ 8.0/10

The blog post examines how misapplying the Minimum Viable Product (MVP) concept leads to half-baked products, illustrated by a founder whose primary motivation was wealth rather than domain expertise. It highlights a common pitfall in startup culture where the MVP is used as an excuse to ship incomplete products, and emphasizes the importance of genuine domain expertise over market-driven opportunism. The article notes that the founder had multiple failed startups in different sectors due to lack of domain expertise, and the MVP was misused to skip essential product development steps.

hackernews · weli · Jul 3, 08:23 · [Discussion](https://news.ycombinator.com/item?id=48772388)

**Background**: The Minimum Viable Product (MVP) is a concept popularized by Eric Ries in the Lean Startup methodology, defined as the version of a new product that allows a team to collect the maximum amount of validated learning with the least effort. However, in practice, it is often misinterpreted as a cheap, incomplete product rather than a learning tool. This critique argues that when founders prioritize wealth over understanding their domain, they misuse MVP to launch half-baked products.

**Discussion**: Commenters express frustration over MVP misuse, noting that founders often lack domain expertise and rely on market analysis. One commenter sarcastically remarks on a dishwasher startup prototype that breaks glasses, illustrating the half-baked problem. Another highlights the disconnect between different personas in a startup.

**Tags**: `#MVP`, `#startup`, `#product development`, `#founder motivation`

---

<a id="item-6"></a>
## [CDD recovers verbatim finetuning data from logits alone](https://www.reddit.com/r/MachineLearning/comments/1umn2dk/contrastive_decoding_diffing_cdd_recovering/) ⭐️ 8.0/10

Researchers introduce Contrastive Decoding Diffing (CDD), a method that recovers verbatim fine-tuning data by contrasting logits between base and finetuned models, requiring only logit access (no weights or activations). This technique significantly improves model auditing and interpretability, enabling detection of verbatim training data leakage and potential backdoors with minimal access compared to prior whitebox methods. CDD achieves a verbatim recovery score of 4+/5 on 19 out of 20 organism-model pairs across four model families (1B-32B parameters), surpassing the Activation Difference Lens (ADL) which never exceeds 3/5 despite requiring full weight access.

reddit · r/MachineLearning · /u/CebulkaZapiekana · Jul 3, 19:01

**Background**: Model diffing compares base and finetuned models to understand changes. Previous work (Activation Difference Lens) used activation differences but required whitebox access and only recovered vague descriptions. CDD is the output-level analog that contrasts logits.

<details><summary>References</summary>
<ul>
<li><a href="https://aiwiki.ai/wiki/contrastive_decoding">Contrastive decoding | AI Wiki</a></li>
<li><a href="https://transformer-circuits.pub/2024/model-diffing/index.html">Stage-Wise Model Diffing</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#model diffing`, `#LLM finetuning`, `#interpretability`, `#security`

---

<a id="item-7"></a>
## [China NFRA Takes Over Zhongbang Bank Over Credit Risk](https://t.me/FinanceNewsDaily/490005) ⭐️ 8.0/10

The National Financial Regulatory Administration (NFRA), together with Hubei Provincial People's Government, announced the takeover of Wuhan Zhongbang Bank Co., Ltd. due to severe credit risk. The decision was made on an unspecified date in 2026 to protect depositors and other clients according to China's banking laws. This takeover signals heightened regulatory scrutiny in China's banking sector and underscores systemic risks in smaller banks. The intervention aims to prevent contagion and maintain financial stability, affecting depositors and the broader banking ecosystem. Zhongbang Bank is a Wuhan-based commercial bank that faced severe credit risk, triggering the takeover. Under Chinese law, during the takeover period, the bank's shareholders' meeting and other governing bodies cease functions, replaced by a takeover team appointed by the regulator.

telegram · FinanceNewsDaily · Jul 3, 09:45

**Background**: The National Financial Regulatory Administration (NFRA) was established in March 2023 as a cabinet-level agency under the State Council, consolidating the former China Banking and Insurance Regulatory Commission (CBIRC) and some functions from the People's Bank of China and the China Securities Regulatory Commission. Bank takeover is a legal procedure used when a bank faces or is likely to face a credit crisis that severely impacts depositors' interests, allowing the regulator to reorganize the bank and restore its normal operations.

<details><summary>References</summary>
<ul>
<li><a href="https://zh.wikipedia.org/zh-cn/国家金融监督管理总局">国家金融监督管理总局 - 维基百科，自由的百科全书</a></li>
<li><a href="https://ailegal.baidu.com/legalarticle/qadetail?id=2d43012c49c25e250906">银行接管管理规定 - ailegal.baidu.com</a></li>
<li><a href="https://www.zhihu.com/question/387180588">商业银行接管的实质是什么？ - 知乎</a></li>

</ul>
</details>

**Tags**: `#finance`, `#regulation`, `#banking`, `#risk`

---

<a id="item-8"></a>
## [Anthropic Accuses Alibaba of Massive Distillation Attack on Claude](https://t.me/zaihuapd/42327) ⭐️ 8.0/10

Anthropic sent a letter to the U.S. Senate Banking Committee accusing Alibaba of orchestrating a massive distillation attack using nearly 25,000 fraudulent accounts to extract capabilities from the Claude AI model. This accusation, involving two major AI players, highlights the growing threat of model theft through distillation attacks and could escalate tensions in AI security and international tech competition. The attack occurred between April 22 and June 5, 2026, with over 28.8 million interactions with Claude, and Anthropic claims it is the largest known distillation attack against the company, involving Alibaba and its Qwen AI lab.

telegram · zaihuapd · Jul 3, 06:21

**Background**: Model distillation is a technique where a smaller model learns from the outputs of a larger, more powerful model to replicate its capabilities efficiently. While distillation is a legitimate method for model compression, it becomes a theft technique when used at scale without authorization to steal a proprietary model's functionality. Anthropic has been working on detecting and preventing such attacks, but notes that a coordinated industry response is needed.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/detecting-and-preventing-distillation-attacks">Detecting and preventing distillation attacks \ Anthropic</a></li>
<li><a href="https://www.linkedin.com/pulse/what-model-distillation-really-means-why-anthropic-example-mahajan-sf2bf">What model “ distillation ” really means and why the Anthropic example...</a></li>
<li><a href="https://www.mindstudio.ai/blog/ai-model-distillation-attacks-explained">AI Model Distillation Attacks : What They Are and Why... | MindStudio</a></li>

</ul>
</details>

**Tags**: `#AI security`, `#model distillation`, `#Anthropic`, `#Alibaba`, `#Claude`

---

<a id="item-9"></a>
## [Huawei Atlas 350 AI card claims 2.87x H20 performance](https://t.me/zaihuapd/42329) ⭐️ 8.0/10

Huawei announced and launched the Atlas 350 accelerator card at the 2026 China Partner Conference, featuring the new Ascend 950PR processor and claiming 2.87 times the compute performance of Nvidia's H20 GPU. This product marks Huawei's latest attempt to challenge Nvidia's dominance in the AI inference market, especially under ongoing export restrictions. With FP4 support and high memory capacity, it could significantly lower inference costs for large language models. The Atlas 350 delivers 1.56 PFLOPS at FP4 precision and includes 112 GB of Huawei's in-house HiBL 1.0 high-bandwidth memory. It supports single-card loading of 70B-parameter models without needing multiple GPUs.

telegram · zaihuapd · Jul 3, 08:35

**Background**: FP4 is a very low precision format (4-bit floating point) that speeds up AI inference by reducing memory and compute demands while maintaining acceptable accuracy. Nvidia's H20 is a reduced-spec GPU sold in China to comply with US export controls. Huawei's Ascend series are domestic alternatives that have been gaining traction in the Chinese market.

<details><summary>References</summary>
<ul>
<li><a href="https://www.huaweicentral.com/huawei-atlas-350-ai-card-debuts-outshining-nvidia-h20-chip/">Huawei Atlas 350 AI card debuts, outshining Nvidia H20 chip</a></li>
<li><a href="https://www.tomshardware.com/pc-components/gpus/huawei-unveils-new-atlas-350-ai-accelerator-with-1-56-pflops-of-fp4-compute-and-up-to-112gb-of-hbm-claims-2-8x-more-performance-than-nvidias-h20">Huawei unveils new Atlas 350 AI accelerator with 1.56 PFLOPS ...</a></li>
<li><a href="https://nerdleveltech.com/huawei-ascend-950pr-atlas-350-ai-chip-challenges-nvidia">Huawei Ascend 950PR Beats NVIDIA H20: 2.8× FP8, CUDA-Ready</a></li>

</ul>
</details>

**Tags**: `#Huawei`, `#AI accelerators`, `#hardware`, `#FP4`, `#Atlas 350`

---

<a id="item-10"></a>
## [Alibaba bans all employees from using Claude, Anthropic products](https://t.me/zaihuapd/42334) ⭐️ 8.0/10

Alibaba issued an internal order requiring all employees to uninstall Claude and all Anthropic-related products, including models like Sonnet, Opus, and Fable, as well as the agent product Claude Code, effective July 10. This ban signals escalating tensions between a major Chinese tech company and a leading Western AI firm, potentially reshaping corporate AI usage policies and impacting cross-border AI competition. The ban follows Anthropic's allegation that Alibaba used approximately 25,000 fake accounts to interact with Claude over 28 million times between April 22 and June 5, leading to tightened security measures. Previously, Alibaba had reimbursed employees for using external models like Claude, GPT, and Gemini.

telegram · zaihuapd · Jul 3, 13:00

**Background**: Claude is a series of large language models developed by Anthropic, an American AI safety company. Models include Haiku, Sonnet, Opus, and Fable, each optimized for different tasks. Claude Code is an agentic coding tool that reads codebases and executes commands. Alibaba's move reflects growing corporate restrictions on external AI tools amid security and competitive concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude ( AI ) - Wikipedia</a></li>
<li><a href="https://claude.com/resources/tutorials/choosing-the-right-claude-model">Choosing the right Claude model : Haiku, Sonnet , Opus , or Fable</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Claude`, `#Alibaba`, `#corporate policy`, `#Anthropic`

---

<a id="item-11"></a>
## [NASA Launches Rescue Satellite to Save Falling Space Telescope](https://apnews.com/article/swift-nasa-satellite-rescue-katalyst-a7ddd740ca099587c58865f583c7245a) ⭐️ 8.0/10

NASA launched the LINK spacecraft on a rescue mission to grapple the aging Swift space telescope and raise its orbit by about 240 km, preventing an atmospheric reentry that could occur as early as October. This mission marks the first attempt by a private spacecraft to capture an uncrewed U.S. government satellite, demonstrating a new capability for on-orbit servicing and debris mitigation that could extend the life of valuable assets like the Hubble Space Telescope in the future. The LINK spacecraft, developed by Katalyst Space Technologies under a $30 million NASA contract, will use a robotic arm to secure Swift and then fire thrusters to slowly raise the orbit; Swift is expected to resume science operations as soon as September if the rescue succeeds.

telegram · zaihuapd · Jul 3, 15:43

**Background**: Swift is a space observatory launched in 2004 to study gamma-ray bursts and other cosmic phenomena. Over 20 years, its orbit has decayed due to increased solar activity, and without intervention it would burn up in Earth's atmosphere. LINK is a dedicated in-orbit servicing vehicle designed to rendezvous with and capture aging satellites, raising their orbits to extend operational lifetimes.

<details><summary>References</summary>
<ul>
<li><a href="https://baike.baidu.com/item/Link/67531114">Link（美国航天器）_百度百科</a></li>
<li><a href="https://www.msn.com/zh-cn/news/other/link卫星27日升空赴约-3000万-救星-力挽5亿美元雨燕天文台轨道危机/ar-AA262rcJ">Link卫星27日升空赴约：3000万“救星”力挽5亿美元雨燕天文台轨道危机</a></li>
<li><a href="https://news.qq.com/rain/a/20260630A04WGY00">“雨燕”坠落，NASA紧急“太空营救”，成功的话下次救“哈勃”</a></li>

</ul>
</details>

**Tags**: `#航天`, `#太空望远镜`, `#轨道救援`, `#私人航天`, `#NASA`

---

<a id="item-12"></a>
## [Tencent's Atuin AI beats Mythos in CyberGym benchmark](https://mp.weixin.qq.com/s/BzU7g-2iG7d6h4ViwMhxyg) ⭐️ 8.0/10

Tencent Xuanwu Lab's Atuin AI, built on the open-source GLM-5.1 model, scored 84.0% on the CyberGym cybersecurity benchmark, surpassing Anthropic's Claude Mythos Preview while using less than 0.1% of Mythos's budget. This demonstrates that high-performing cybersecurity AI can be achieved with low-cost, open-source models, challenging the assumption that only massive proprietary models can excel in vulnerability detection. It could democratize access to advanced AI security tools at a fraction of the cost. Atuin AI also discovered multiple high-risk logic vulnerabilities in projects such as curl, gnark, OpenSSL, Python cryptography, and Java bc-java that Mythos missed, with a highest severity score of 9.3. On the Berkeley BVI real-world vulnerability list, Atuin AI ranked 1st in critical vulnerability count and 5th in total vulnerabilities.

telegram · zaihuapd · Jul 3, 16:12

**Background**: CyberGym is a benchmark for evaluating AI agents' cybersecurity capabilities, covering the full vulnerability lifecycle. GLM-5.1 is an open-weight large language model developed by Z.ai, released under the MIT License, allowing local deployment. Claude Mythos Preview is Anthropic's powerful model previously leading the CyberGym leaderboard.

<details><summary>References</summary>
<ul>
<li><a href="https://llm-stats.com/benchmarks/cybergym">CyberGym Benchmark Leaderboard | LLM Stats</a></li>
<li><a href="https://en.wikipedia.org/wiki/GLM-5.1">GLM-5.1</a></li>
<li><a href="https://www.cybergym.io/cybergym-e2e/">CyberGym -E2E: Scalable Real-World Benchmark for AI Agents...</a></li>

</ul>
</details>

**Tags**: `#AI安全`, `#网络安全`, `#腾讯`, `#GLM`, `#漏洞检测`

---