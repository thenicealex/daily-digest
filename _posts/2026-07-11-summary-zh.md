---
layout: default
title: "Horizon Summary: 2026-07-11 (ZH)"
date: 2026-07-11
lang: zh
---

> 从 39 条内容中筛选出 9 条重要资讯。

---

1. [vLLM v0.25.0：默认使用 Model Runner V2，移除 PagedAttention](#item-1) ⭐️ 9.0/10
2. [人形机器人完成全球首例活猪胆囊手术](#item-2) ⭐️ 9.0/10
3. [ClickHouse 通过 SO_REUSEPORT 和 Peering 将 PgBouncer 吞吐量提升 4 倍](#item-3) ⭐️ 8.0/10
4. [优先选择 SQLite STRICT 表以确保类型安全](#item-4) ⭐️ 8.0/10
5. [中国实施临时氦气出口禁令，威胁全球供应链](#item-5) ⭐️ 8.0/10
6. [SK 海力士 CEO 警告 2027 年将出现最严重内存短缺](#item-6) ⭐️ 8.0/10
7. [苹果起诉 OpenAI，指控其窃取商业机密推动硬件业务](#item-7) ⭐️ 8.0/10
8. [U-Boot 引导程序曝 6 漏洞，可绕过验证执行恶意代码](#item-8) ⭐️ 8.0/10
9. [上海计划 2027 年前实现半侵入式脑机接口临床应用](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.25.0：默认使用 Model Runner V2，移除 PagedAttention](https://github.com/vllm-project/vllm/releases/tag/v0.25.0) ⭐️ 9.0/10

vLLM v0.25.0 将所有密集模型的默认执行路径切换到 Model Runner V2，移除了传统的 PagedAttention 实现，并使 Transformers 后端的性能与原生 vLLM 持平。 此版本标志着 vLLM 的重大架构转变，简化了代码库并提高了可维护性，同时确保用户不再需要在兼容性和性能之间做出选择。 该版本包含来自 232 位贡献者的 558 次提交，增加了对 LLaVA-OneVision-2 和 GLM-5 等新模型的支持，引入了统一的流式解析器引擎，并实现了异构词表的通用推测解码。

github · khluu · 7月11日 20:06

**背景**: vLLM 是一个开源的高吞吐量 LLM 推理引擎，它使用 PagedAttention 高效管理 KV 缓存内存。Model Runner V2 (MRv2) 是一个重新设计的执行核心，解决了原始 V1 架构的局限性，提供了更好的模块化和性能。移除 PagedAttention 标志着向 MRv2 和更新的注意力后端的迁移已完成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/PagedAttention">PagedAttention - Wikipedia</a></li>
<li><a href="https://vllm.ai/blog/2026-03-24-mrv2">Model Runner V2: A Modular and Faster Core for vLLM | vLLM Blog</a></li>
<li><a href="https://docs.vllm.ai/en/stable/features/speculative_decoding/dynamic_speculative_decoding/">Dynamic Speculative Decoding - vLLM</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#open source`, `#AI infrastructure`, `#performance`

---

<a id="item-2"></a>
## [人形机器人完成全球首例活猪胆囊手术](https://arstechnica.com/ai/2026/07/humanoid-robots-controlled-by-surgeons-did-world-first-operation-on-live-pigs/) ⭐️ 9.0/10

外科医生远程操控宇树 G1 人形机器人，在活猪身上完成了腹腔镜胆囊切除术，这是首次将通用人形机器人用于活体手术，成果发表在《自然》期刊。 这种低成本方案有望取代专用手术机器人，在农村、战场甚至太空等资源有限的场景中实现远程手术，大幅扩展手术护理的可及性。 宇树 G1 基础款售价 13500 美元，加配灵巧手后约 67000 美元，远低于达芬奇系统（50 万至数百万美元）。该机器人高 1.5 米，重 27 公斤，拥有 23 个以上自由度。

telegram · zaihuapd · 7月11日 02:29

**背景**: 人形机器人旨在模仿人类形态和运动。专用手术机器人如达芬奇价格昂贵且专用于手术。宇树 G1 是通用人形机器人，最初用于研究和工业任务。这项研究展示了其在医疗领域的适应性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Unitree_Robotics">Unitree Robotics</a></li>
<li><a href="https://www.unitree.com/g1/">Humanoid robot G1_Humanoid Robot Functions ... - Unitree G1</a></li>

</ul>
</details>

**标签**: `#humanoid robotics`, `#surgery`, `#medical robotics`, `#remote surgery`

---

<a id="item-3"></a>
## [ClickHouse 通过 SO_REUSEPORT 和 Peering 将 PgBouncer 吞吐量提升 4 倍](https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres) ⭐️ 8.0/10

ClickHouse 的工程师介绍了他们如何通过启用 SO_REUSEPORT 在同一端口上运行多个进程，并实现 peering 机制来正确处理连接取消，从而将 PgBouncer 的吞吐量提升了四倍。 这具有重要意义，因为 PgBouncer 是 PostgreSQL 广泛使用的连接池化工具；无需更改硬件即可将其吞吐量提升四倍，可以极大地惠及许多 PostgreSQL 部署，尤其是那些处理高并发或频繁查询取消的部署。 Peering 机制允许 PgBouncer 进程将取消请求转发给正确的拥有者进程，解决了取消请求落在不认识该查询的进程上的问题。SO_REUSEPORT 允许多个进程绑定到同一个 TCP 端口，从而将传入连接分布到这些进程上。

hackernews · saisrirampur · 7月11日 15:28 · [社区讨论](https://news.ycombinator.com/item?id=48872874)

**背景**: PgBouncer 是一个轻量级的 PostgreSQL 连接池化工具。每个 PostgreSQL 连接都会产生一个独立的 OS 进程，开销较大；连接池化通过复用连接来降低开销。SO_REUSEPORT 是 Linux 套接字选项（自内核 3.9 起可用），允许多个套接字绑定到同一端口以实现更好的负载分布。PgBouncer 中的 peering 机制使多个池化进程能够共享会话状态，从而将客户端的取消请求转发到正确的后端进程。

<details><summary>参考链接</summary>
<ul>
<li><a href="http://www.pgbouncer.org/usage.html">PgBouncer command-line usage</a></li>
<li><a href="https://www.linkedin.com/pulse/how-modern-kernels-handle-massive-traffic-use-jisan-ahmed-ghg1c">How Modern Kernels Handle Massive Traffic : the use of...</a></li>
<li><a href="https://www.pgbouncer.org/config.html">PgBouncer config</a></li>

</ul>
</details>

**社区讨论**: 评论者表现出浓厚兴趣，询问 peering 是否是 PgBouncer 内置功能以及如何设置。一些人建议使用 Odyssey 和 pgdog 等替代池化工具，另一些人则分享了在 Kubernetes 上运行多个 PgBouncer 进程的经验。总体而言，讨论是积极的，主要集中在实际部署细节上。

**标签**: `#pgbouncer`, `#postgresql`, `#scaling`, `#connection pooling`, `#performance`

---

<a id="item-4"></a>
## [优先选择 SQLite STRICT 表以确保类型安全](https://evanhahn.com/prefer-strict-tables-in-sqlite/) ⭐️ 8.0/10

Evan Hahn 的文章提倡使用 SQLite 的 STRICT 表来强制类型安全并防止数据损坏，强调了数据库完整性的一种最佳实践。 SQLite 默认的灵活类型可能导致微妙的数据损坏，因此采用 STRICT 表可提高数据完整性，尤其在多应用或关键数据场景中。 STRICT 表要求每列都有指定的类型（INT、INTEGER、REAL、TEXT、BLOB 或 ANY），并且如果数据无法无损转换则返回错误，这与默认的亲和性行为不同。

hackernews · ingve · 7月11日 17:33 · [社区讨论](https://news.ycombinator.com/item?id=48873940)

**背景**: SQLite 传统上使用灵活的类型系统，列具有类型亲和性而非严格类型，允许将任何值存储在任何列中。STRICT 表选项于 SQLite 3.37.0（2021 年 11 月）引入，通过强制严格类型来改变这一点，类似于其他 SQL 数据库。这解决了常见批评：SQLite 缺乏类型强制可能导致数据不一致。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sqlite.org/stricttables.html">STRICT Tables</a></li>
<li><a href="https://www.sqlitetutorial.net/sqlite-strict-tables/">SQLite Strict Tables</a></li>

</ul>
</details>

**社区讨论**: 社区评论强烈支持将 STRICT 设为默认，jll29 和 petilon 等用户认为它应该是默认值。然而，dfabulich 链接到官方理由，解释为什么 STRICT 不是默认值，引用了易于检测损坏的观点。讨论突显了嵌入式使用的灵活性与共享数据库的可靠性之间的张力。

**标签**: `#SQLite`, `#database`, `#type safety`, `#data integrity`

---

<a id="item-5"></a>
## [中国实施临时氦气出口禁令，威胁全球供应链](https://www.cls.cn/detail/2422943) ⭐️ 8.0/10

中国商务部与海关总署联合宣布对氦气实施临时禁止出口管理，这是首次针对这种关键气体采取此类措施。该禁令将扰乱全球半导体和医疗行业的氦气供应。 氦气在半导体制造（如冷却 EUV 光刻机）和医疗成像（如冷却 MRI 磁体）中不可替代。此禁令可能导致供应链中断、成本上升，并凸显中国对关键资源的管控力。 禁令的具体时长和范围尚未公开，但被描述为临时性。中国既生产也出口氦气，同时是主要进口国；禁令主要影响其出口量，足以对全球市场产生冲击。

telegram · FinanceNewsDaily · 7月11日 00:13

**背景**: 氦气是一种稀有惰性气体，主要通过天然气提取。它对于 MRI 机器的超导磁体冷却、半导体光刻中的冷却以及检漏至关重要。中国消耗全球约 30%的氦气，但国内产量仅满足一小部分需求，因此依赖从美国、卡塔尔等国进口。不过，中国也出口部分氦气，此次出口禁令可能使本就紧张的全球供应进一步承压。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.innovationnewsnetwork.com/why-helium-is-essential-to-the-future-of-semiconductor-manufacturing/64493/">Why helium is essential to semiconductor manufacturing</a></li>
<li><a href="https://yigasint.com/medical-helium-properties-uses-and-applications/">Medical Helium: Properties, Uses, and Applications</a></li>

</ul>
</details>

**标签**: `#helium`, `#export control`, `#semiconductor`, `#supply chain`, `#geopolitics`

---

<a id="item-6"></a>
## [SK 海力士 CEO 警告 2027 年将出现最严重内存短缺](https://www.reuters.com/world/asia-pacific/sk-hynix-ceo-sees-worst-ever-memory-supply-shortage-2027-says-demand-outstrip-2026-07-10/) ⭐️ 8.0/10

SK 海力士 CEO 郭鲁正预测，全球内存行业将在 2027 年面临史上最严重的供应短缺，即使积极扩产，客户需求在 2030 年后仍将超过供应能力。 作为顶级内存芯片 CEO 的预警，表明供需失衡将持续，可能导致内存价格上涨，并影响依赖半导体的行业，如人工智能和数据中心。 SK 海力士 2025 年营业利润达创纪录的 47 万亿韩元（约 310 亿美元），2026 年第二季度预计进一步增至 65.5 万亿韩元。海外晶圆厂候选地包括美国、日本和东南亚。

telegram · zaihuapd · 7月11日 00:45

**背景**: 内存芯片是电子设备、AI 加速器和云计算的关键组件。SK 海力士是全球最大的内存制造商之一，近期在纳斯达克上市后市值上升。这一预测突显了由人工智能驱动的结构性需求增长，AI 需要高带宽内存（HBM）芯片。

**标签**: `#memory industry`, `#supply shortage`, `#SK Hynix`, `#semiconductor`, `#AI`

---

<a id="item-7"></a>
## [苹果起诉 OpenAI，指控其窃取商业机密推动硬件业务](https://www.cnbc.com/2026/07/10/apple-openai-lawsuit-trade-secrets.html) ⭐️ 8.0/10

苹果于 7 月 10 日在美国加州北区联邦法院起诉 OpenAI、两名前员工及 io Products，指控其通过招聘苹果员工、接触供应商等方式，系统性窃取苹果的产品设计、制造工艺及供应链机密，以加快消费级硬件研发。 此次诉讼凸显了苹果与 OpenAI 之间日益加剧的紧张关系，后者正积极进军硬件领域，此举可能重塑 AI 消费设备的竞争格局，并为科技行业的商业机密保护树立法律先例。 苹果指控前员工 Chang Liu 离职后仍访问内部网络并下载数十份硬件文件；OpenAI 硬件负责人 Tang Yew Tan 在离职前将供应商资料发送至个人邮箱，并要求求职者携带苹果零部件参加面试。苹果还表示，目前有超过 400 名前苹果员工在 OpenAI 工作。

telegram · zaihuapd · 7月11日 03:14

**背景**: io Products 是一家 AI 硬件公司，由前苹果设计总监 Jony Ive、Scott Cannon、Evans Hankey 及硬件高管 Tang Tan 于 2024 年创立，并于 2025 年 5 月被 OpenAI 收购，以领导其硬件产品开发。OpenAI 一直在扩展消费硬件领域，包括与 Jony Ive 合作开发的 AI 原生设备（传闻无屏幕），以及面向开发者的宏键盘 Codex Micro。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Io_Products">Io Products</a></li>
<li><a href="https://builtin.com/articles/openai-device">OpenAI’s New Device: What We Know So Far | Built In</a></li>

</ul>
</details>

**标签**: `#Apple`, `#OpenAI`, `#lawsuit`, `#trade secrets`, `#hardware`

---

<a id="item-8"></a>
## [U-Boot 引导程序曝 6 漏洞，可绕过验证执行恶意代码](https://www.bleepingcomputer.com/news/security/new-u-boot-flaws-could-enable-stealthy-firmware-attacks/) ⭐️ 8.0/10

固件安全公司 Binarly 披露了 U-Boot 的 FIT 签名验证代码中的六个漏洞，其中两个可导致任意代码执行，四个可造成拒绝服务，影响自 U-Boot 2013.07 以来的版本。 这些漏洞使攻击者可在操作系统启动前执行恶意代码，可能禁用固件安全功能、修改启动流程或植入持久性固件恶意软件，影响大量嵌入式设备和物联网设备。 漏洞编号为 BRLY-2026-037 至 BRLY-2026-042，其中两个可实现代码执行，四个导致拒绝服务。对于支持远程固件更新的 BMC 系统，利用可能无需物理接触。

telegram · zaihuapd · 7月11日 08:32

**背景**: U-Boot 是一个广泛使用的开源引导程序，用于初始化硬件并加载操作系统。FIT（扁平化映像树）映像通过加密签名来保证启动时的真实性和完整性，由 U-Boot 进行验证。这些漏洞存在于签名验证逻辑中，允许精心构造的 FIT 映像绕过验证并在操作系统加载前执行任意代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cybersecuritynews.com/u-boot-fit-signature-verification/">Six U - Boot FIT Signature Verification Flaws Enable Code Execution...</a></li>
<li><a href="https://docs.u-boot-project.org/en/latest/usage/fit/signature.html">U - Boot FIT Signature Verification — Das U - Boot unknown version...</a></li>
<li><a href="https://proteanos.com/doc/secure-boot-uboot-fit-signatures-chain-of-trust/">Secure Boot with U - Boot FIT Signatures : A Practical Chain-of-Trust...</a></li>

</ul>
</details>

**标签**: `#security`, `#u-boot`, `#firmware`, `#vulnerabilities`, `#boot`

---

<a id="item-9"></a>
## [上海计划 2027 年前实现半侵入式脑机接口临床应用](https://t.me/zaihuapd/42501) ⭐️ 8.0/10

上海市科学技术委员会印发了《上海市脑机接口未来产业培育行动方案（2025-2030 年）》，提出到 2027 年实现高质量脑控、半侵入式脑机接口产品在国内率先临床应用、侵入式脑机接口研发取得突破。 该政策为中国的脑机接口发展提供了具体路线图和政府支持，有望加速瘫痪、失语等疾病的医疗康复，并使上海成为神经技术领域的全球中心。 方案明确到 2027 年推动 5 款以上侵入式或半侵入式脑机接口产品完成医疗器械型式检验和临床试验，面向失语、瘫痪等患者实现部分语言和运动功能恢复。

telegram · zaihuapd · 7月11日 15:49

**背景**: 脑机接口分为非侵入式（如头皮脑电）、半侵入式（如硬脑膜上的皮层脑电图）和侵入式（植入大脑皮层的电极）。半侵入式在信号质量和手术风险之间取得平衡。中国已将脑机接口纳入未来产业国家战略。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Brain–computer_interface">Brain–computer interface - Wikipedia</a></li>
<li><a href="https://www.sciencedirect.com/org/science/article/pii/S2817092X2400005X">Invasive Brain-Computer Interfaces: A Critical Assessment of ...</a></li>

</ul>
</details>

**标签**: `#brain-computer interface`, `#neurotechnology`, `#medical innovation`, `#government policy`, `#China`

---