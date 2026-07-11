---
layout: default
title: "Horizon Summary: 2026-07-11 (EN)"
date: 2026-07-11
lang: en
---

> From 39 items, 9 important content pieces were selected

---

1. [vLLM v0.25.0: Model Runner V2 Default, PagedAttention Removed](#item-1) ⭐️ 9.0/10
2. [Humanoid robots perform world-first live pig gallbladder surgery](#item-2) ⭐️ 9.0/10
3. [ClickHouse Scales PgBouncer 4x with SO_REUSEPORT and Peering](#item-3) ⭐️ 8.0/10
4. [Prefer SQLite STRICT tables for type safety](#item-4) ⭐️ 8.0/10
5. [China Imposes Temporary Helium Export Ban, Threatens Global Supply Chains](#item-5) ⭐️ 8.0/10
6. [SK Hynix CEO Warns of Worst Memory Shortage by 2027](#item-6) ⭐️ 8.0/10
7. [Apple Sues OpenAI for Stealing Trade Secrets to Boost Hardware](#item-7) ⭐️ 8.0/10
8. [6 U-Boot Bootloader Flaws Allow Code Execution via FIT Validation Bypass](#item-8) ⭐️ 8.0/10
9. [Shanghai Aims for Clinical Semi-Invasive BCI by 2027](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.25.0: Model Runner V2 Default, PagedAttention Removed](https://github.com/vllm-project/vllm/releases/tag/v0.25.0) ⭐️ 9.0/10

vLLM v0.25.0 makes Model Runner V2 the default execution path for all dense models, removes the legacy PagedAttention implementation, and achieves performance parity between the Transformers backend and native vLLM. This release marks a major architecture shift for vLLM, simplifying the codebase and improving maintainability, while also ensuring that users no longer need to choose between compatibility and performance. The release includes 558 commits from 232 contributors, adds support for new models like LLaVA-OneVision-2 and GLM-5, introduces a unified streaming parser engine, and enables universal speculative decoding for heterogeneous vocabularies.

github · khluu · Jul 11, 20:06

**Background**: vLLM is an open-source high-throughput LLM inference engine that uses PagedAttention to manage KV-cache memory efficiently. Model Runner V2 (MRv2) is a redesigned execution core that addresses limitations of the original V1 architecture, offering better modularity and performance. The removal of PagedAttention signals the completion of the migration to MRv2 and newer attention backends.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/PagedAttention">PagedAttention - Wikipedia</a></li>
<li><a href="https://vllm.ai/blog/2026-03-24-mrv2">Model Runner V2: A Modular and Faster Core for vLLM | vLLM Blog</a></li>
<li><a href="https://docs.vllm.ai/en/stable/features/speculative_decoding/dynamic_speculative_decoding/">Dynamic Speculative Decoding - vLLM</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM inference`, `#open source`, `#AI infrastructure`, `#performance`

---

<a id="item-2"></a>
## [Humanoid robots perform world-first live pig gallbladder surgery](https://arstechnica.com/ai/2026/07/humanoid-robots-controlled-by-surgeons-did-world-first-operation-on-live-pigs/) ⭐️ 9.0/10

Surgeons remotely controlled Unitree G1 humanoid robots to perform laparoscopic cholecystectomy on live pigs, marking the first use of a general-purpose humanoid robot for live surgery, with results published in Nature. This low-cost alternative to dedicated surgical robots could enable remote surgery in resource-limited settings like rural areas, battlefields, or space, dramatically expanding access to surgical care. The Unitree G1 base model costs $13,500, and with dexterous hands it costs approximately $67,000, far cheaper than Da Vinci systems ($0.5M-$2.5M). The robot is 1.5 m tall, weighs 27 kg, and has 23+ degrees of freedom.

telegram · zaihuapd · Jul 11, 02:29

**Background**: Humanoid robots are designed to mimic human form and movement. Dedicated surgical robots like Da Vinci are expensive and specialized. Unitree G1 is a general-purpose humanoid, originally for research and industrial tasks. This research demonstrates its adaptability for medical procedures.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Unitree_Robotics">Unitree Robotics</a></li>
<li><a href="https://www.unitree.com/g1/">Humanoid robot G1_Humanoid Robot Functions ... - Unitree G1</a></li>

</ul>
</details>

**Tags**: `#humanoid robotics`, `#surgery`, `#medical robotics`, `#remote surgery`

---

<a id="item-3"></a>
## [ClickHouse Scales PgBouncer 4x with SO_REUSEPORT and Peering](https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres) ⭐️ 8.0/10

ClickHouse engineers describe how they achieved a fourfold throughput improvement for PgBouncer by enabling SO_REUSEPORT to run multiple processes on the same port and implementing peering to handle connection cancellation correctly. This is significant because PgBouncer is a widely-used connection pooler for PostgreSQL; scaling it by 4x without hardware changes can greatly benefit many PostgreSQL deployments, especially those handling high concurrency or frequent query cancellations. The peering mechanism allows PgBouncer processes to forward cancellation requests to the correct owner process, solving the issue where a cancel lands on a process unaware of the query. SO_REUSEPORT enables multiple processes to bind to the same TCP port, distributing incoming connections among them.

hackernews · saisrirampur · Jul 11, 15:28 · [Discussion](https://news.ycombinator.com/item?id=48872874)

**Background**: PgBouncer is a lightweight connection pooler for PostgreSQL. Each PostgreSQL connection spawns a separate OS process, which is expensive; connection pooling reuses connections to reduce overhead. SO_REUSEPORT is a Linux socket option (available since kernel 3.9) that allows multiple sockets to bind to the same port for better load distribution. Peering in PgBouncer enables multiple pooler processes to share session state, so that cancel requests from a client are forwarded to the correct backend process.

<details><summary>References</summary>
<ul>
<li><a href="http://www.pgbouncer.org/usage.html">PgBouncer command-line usage</a></li>
<li><a href="https://www.linkedin.com/pulse/how-modern-kernels-handle-massive-traffic-use-jisan-ahmed-ghg1c">How Modern Kernels Handle Massive Traffic : the use of...</a></li>
<li><a href="https://www.pgbouncer.org/config.html">PgBouncer config</a></li>

</ul>
</details>

**Discussion**: Commenters showed strong interest, asking whether peering is built into PgBouncer and how to set it up. Some suggested alternative poolers like Odyssey and pgdog, while others shared their experiences running multiple PgBouncer processes on Kubernetes. Overall, the discussion was positive and centered on practical deployment details.

**Tags**: `#pgbouncer`, `#postgresql`, `#scaling`, `#connection pooling`, `#performance`

---

<a id="item-4"></a>
## [Prefer SQLite STRICT tables for type safety](https://evanhahn.com/prefer-strict-tables-in-sqlite/) ⭐️ 8.0/10

Evan Hahn's article advocates using SQLite's STRICT tables to enforce type safety and prevent data corruption, highlighting a best practice for database integrity. SQLite's default flexible typing can lead to subtle data corruption, so adopting STRICT tables improves data integrity, especially in multi-application or critical data scenarios. STRICT tables require every column to have a specified type (INT, INTEGER, REAL, TEXT, BLOB, or ANY) and return an error if data cannot be losslessly converted, unlike default affinity behavior.

hackernews · ingve · Jul 11, 17:33 · [Discussion](https://news.ycombinator.com/item?id=48873940)

**Background**: SQLite traditionally uses a flexible type system where columns have type affinities rather than strict types, allowing any value to be stored in any column. The STRICT table option, introduced in SQLite 3.37.0 (November 2021), changes this by enforcing strict typing, similar to other SQL databases. This addresses the common criticism that SQLite's lack of type enforcement can lead to data inconsistency.

<details><summary>References</summary>
<ul>
<li><a href="https://sqlite.org/stricttables.html">STRICT Tables</a></li>
<li><a href="https://www.sqlitetutorial.net/sqlite-strict-tables/">SQLite Strict Tables</a></li>

</ul>
</details>

**Discussion**: Community comments express strong support for making STRICT the default, with users like jll29 and petilon arguing it should be default. However, dfabulich links to the official rationale explaining why STRICT is not default, citing ease of detecting corruption. The discussion highlights tension between flexibility for embedded use and reliability for shared databases.

**Tags**: `#SQLite`, `#database`, `#type safety`, `#data integrity`

---

<a id="item-5"></a>
## [China Imposes Temporary Helium Export Ban, Threatens Global Supply Chains](https://www.cls.cn/detail/2422943) ⭐️ 8.0/10

China's Ministry of Commerce and General Administration of Customs jointly announced a temporary export ban on helium, marking the first such measure targeting this critical gas. The ban is set to disrupt helium supplies to global semiconductor and medical industries. Helium is irreplaceable in semiconductor manufacturing (e.g., cooling EUV lithography machines) and medical imaging (e.g., cooling MRI magnets). This ban could cause supply chain disruptions, raise costs, and highlights China's growing leverage over essential resources. The exact duration and scope of the ban have not been disclosed, but it is described as temporary. China both produces and exports helium, though it is also a major importer; the ban will primarily affect its export volumes, which are significant enough to impact global markets.

telegram · FinanceNewsDaily · Jul 11, 00:13

**Background**: Helium is a rare, inert gas primarily extracted from natural gas. It is critical for cooling superconducting magnets in MRI machines, as a coolant in semiconductor lithography, and for leak detection. While China consumes about 30% of global helium, its domestic production meets only a fraction of demand, making it reliant on imports from the US, Qatar, and others. However, China also re-exports some helium, and any disruption from its export ban could strain an already tight global supply.

<details><summary>References</summary>
<ul>
<li><a href="https://www.innovationnewsnetwork.com/why-helium-is-essential-to-the-future-of-semiconductor-manufacturing/64493/">Why helium is essential to semiconductor manufacturing</a></li>
<li><a href="https://yigasint.com/medical-helium-properties-uses-and-applications/">Medical Helium: Properties, Uses, and Applications</a></li>

</ul>
</details>

**Tags**: `#helium`, `#export control`, `#semiconductor`, `#supply chain`, `#geopolitics`

---

<a id="item-6"></a>
## [SK Hynix CEO Warns of Worst Memory Shortage by 2027](https://www.reuters.com/world/asia-pacific/sk-hynix-ceo-sees-worst-ever-memory-supply-shortage-2027-says-demand-outstrip-2026-07-10/) ⭐️ 8.0/10

SK Hynix CEO Kwak Noh-Jung forecasted that the global memory industry will face its worst supply shortage by 2027, with demand outstripping supply even after 2030 despite expansion plans. This warning from a top memory chip CEO signals a prolonged imbalance that could drive up memory prices and impact industries reliant on semiconductors, such as AI and data centers. The company's operating profit for 2025 reached a record 47 trillion won (about $31 billion), with second-quarter 2026 expected to reach 65.5 trillion won. Overseas fab locations under consideration include the US, Japan, and Southeast Asia.

telegram · zaihuapd · Jul 11, 00:45

**Background**: Memory chips are critical components in electronics, AI accelerators, and cloud computing. SK Hynix is one of the world's largest memory manufacturers, and its market cap recently rose with its Nasdaq listing. The forecast highlights structural demand growth driven by AI, which requires high-bandwidth memory (HBM) chips.

**Tags**: `#memory industry`, `#supply shortage`, `#SK Hynix`, `#semiconductor`, `#AI`

---

<a id="item-7"></a>
## [Apple Sues OpenAI for Stealing Trade Secrets to Boost Hardware](https://www.cnbc.com/2026/07/10/apple-openai-lawsuit-trade-secrets.html) ⭐️ 8.0/10

Apple filed a lawsuit on July 10 in the U.S. District Court for the Northern District of California against OpenAI, two former employees, and io Products, accusing them of systematically stealing trade secrets related to product design, manufacturing processes, and supply chain information to accelerate OpenAI's consumer hardware development. This lawsuit highlights escalating tensions between Apple and OpenAI as the latter aggressively expands into hardware, potentially reshaping the competitive landscape of AI-powered consumer devices and setting a legal precedent for trade secret protection in the tech industry. Apple alleges that former employee Chang Liu accessed internal networks after leaving and downloaded dozens of hardware files, while OpenAI's hardware head Tang Yew Tan sent supplier information to his personal email before leaving and instructed job applicants to bring Apple parts to interviews. Apple also claims that over 400 former Apple employees now work at OpenAI.

telegram · zaihuapd · Jul 11, 03:14

**Background**: io Products, an AI hardware company founded in 2024 by former Apple design chief Jony Ive, Scott Cannon, Evans Hankey, and hardware executive Tang Tan, was acquired by OpenAI in May 2025 to lead its hardware product development. OpenAI has been expanding into consumer hardware, including a rumored AI-native device developed with Jony Ive and a developer-focused macro keyboard called Codex Micro.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Io_Products">Io Products</a></li>
<li><a href="https://builtin.com/articles/openai-device">OpenAI’s New Device: What We Know So Far | Built In</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#OpenAI`, `#lawsuit`, `#trade secrets`, `#hardware`

---

<a id="item-8"></a>
## [6 U-Boot Bootloader Flaws Allow Code Execution via FIT Validation Bypass](https://www.bleepingcomputer.com/news/security/new-u-boot-flaws-could-enable-stealthy-firmware-attacks/) ⭐️ 8.0/10

Binarly disclosed six vulnerabilities in U-Boot's FIT signature verification code, two enabling arbitrary code execution and four causing denial of service, affecting versions since U-Boot 2013.07. These flaws allow attackers to execute malicious code before the OS boots, potentially disabling firmware security, altering the boot flow, or implanting persistent firmware malware, impacting numerous embedded and IoT devices. The vulnerabilities are identified as BRLY-2026-037 through BRLY-2026-042; two allow code execution and four lead to DoS conditions. For BMC systems supporting remote firmware updates, exploitation may not require physical access.

telegram · zaihuapd · Jul 11, 08:32

**Background**: U-Boot is a popular open-source bootloader used in many embedded systems to initialize hardware and load the operating system. FIT (Flattened Image Tree) images are signed to ensure authenticity and integrity during boot, using cryptographic signatures verified by U-Boot. The vulnerabilities reside in the signature verification logic, allowing crafted FIT images to bypass validation and execute arbitrary code before the OS is loaded.

<details><summary>References</summary>
<ul>
<li><a href="https://cybersecuritynews.com/u-boot-fit-signature-verification/">Six U - Boot FIT Signature Verification Flaws Enable Code Execution...</a></li>
<li><a href="https://docs.u-boot-project.org/en/latest/usage/fit/signature.html">U - Boot FIT Signature Verification — Das U - Boot unknown version...</a></li>
<li><a href="https://proteanos.com/doc/secure-boot-uboot-fit-signatures-chain-of-trust/">Secure Boot with U - Boot FIT Signatures : A Practical Chain-of-Trust...</a></li>

</ul>
</details>

**Tags**: `#security`, `#u-boot`, `#firmware`, `#vulnerabilities`, `#boot`

---

<a id="item-9"></a>
## [Shanghai Aims for Clinical Semi-Invasive BCI by 2027](https://t.me/zaihuapd/42501) ⭐️ 8.0/10

Shanghai Municipal Science and Technology Commission issued the 'Shanghai Brain-Computer Interface Future Industry Cultivation Action Plan (2025-2030)', setting targets for 2027: high-quality brain control, semi-invasive BCI products achieving clinical application first in China, and breakthroughs in invasive BCI research. This policy provides a concrete roadmap and government backing for BCI development in China, potentially accelerating medical rehabilitation for conditions like paralysis and aphasia, and positioning Shanghai as a global hub for neurotechnology. The plan specifies that by 2027, at least five invasive or semi-invasive BCI products should pass medical device type testing and clinical trials, aiming to restore partial language and motor functions for patients with aphasia and paralysis.

telegram · zaihuapd · Jul 11, 15:49

**Background**: Brain-computer interfaces (BCIs) are classified into non-invasive (e.g., EEG on scalp), semi-invasive (e.g., ECoG on dura), and invasive (electrodes implanted in brain cortex). Semi-invasive BCIs offer a balance between signal quality and surgical risk. China has been investing in BCI technology as part of its national strategy for future industries.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Brain–computer_interface">Brain–computer interface - Wikipedia</a></li>
<li><a href="https://www.sciencedirect.com/org/science/article/pii/S2817092X2400005X">Invasive Brain-Computer Interfaces: A Critical Assessment of ...</a></li>

</ul>
</details>

**Tags**: `#brain-computer interface`, `#neurotechnology`, `#medical innovation`, `#government policy`, `#China`

---