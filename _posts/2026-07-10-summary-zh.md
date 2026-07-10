---
layout: default
title: "Horizon Summary: 2026-07-10 (ZH)"
date: 2026-07-10
lang: zh
---

> 从 58 条内容中筛选出 15 条重要资讯。

---

1. [SGLang v0.5.15 显著提升 Blackwell 上的 GLM-5.2 NVFP4 性能](#item-1) ⭐️ 8.0/10
2. [QuadRF：开源软件无线电可探测无人机和 WiFi 信号](#item-2) ⭐️ 8.0/10
3. [GPT-5.6 Sol Ultra 生成循环双覆盖猜想证明](#item-3) ⭐️ 8.0/10
4. [优秀工具应无形](#item-4) ⭐️ 8.0/10
5. [成功公司如何变得盲目](#item-5) ⭐️ 8.0/10
6. [SK 海力士 CEO：存储芯片短缺可能持续到 2030 年后](#item-6) ⭐️ 8.0/10
7. [SK 海力士 CEO 预测 2027 年将现史上最严重内存短缺](#item-7) ⭐️ 8.0/10
8. [苹果起诉 OpenAI 窃取商业机密](#item-8) ⭐️ 8.0/10
9. [中国法院裁定游戏账号可继承，平台禁止条款无效](#item-9) ⭐️ 8.0/10
10. [Anthropic 网页爬虫导流比达 2800:1](#item-10) ⭐️ 8.0/10
11. [长征十号乙实现全球首次网系火箭海上回收](#item-11) ⭐️ 8.0/10
12. [腾讯洽购 AI 公司 Manus，拟从 Meta 手中回购](#item-12) ⭐️ 8.0/10
13. [OpenAI 与 Google 被指通过新加坡向黑名单中国企业提供 AI](#item-13) ⭐️ 8.0/10
14. [中国对氦气实施临时出口禁令](#item-14) ⭐️ 8.0/10
15. [Meta 因成瘾设计面临欧盟 120 亿美元罚款](#item-15) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [SGLang v0.5.15 显著提升 Blackwell 上的 GLM-5.2 NVFP4 性能](https://github.com/sgl-project/sglang/releases/tag/v0.5.15) ⭐️ 8.0/10

SGLang v0.5.15 针对 Blackwell GPU 上的 GLM-5.2 模型，利用 NVFP4 精度优化了推理服务，在 8 块 B300 上达到每秒每用户超过 500 token，并引入了 Spec V2 和 IndexShare MTP 等推测解码改进。 此版本大幅提升了最前沿硬件上大语言模型的推理吞吐量，降低了生产部署的延迟和成本，同时展示了推测解码与低精度推理方面的实际进展。 关键优化包括可 CUDA 图的 DSA draft-extend 消除了同步开销（吞吐量提升 11%），IndexShare MTP 在草稿步骤间复用索引器 top-k（成本降低至 1.9 倍），以及将 12 个内核融合为 4 个（解码速度提升约 8%）。

github · Fridge003 · 7月10日 22:58

**背景**: NVFP4 是随 NVIDIA Blackwell 架构推出的 4 位浮点格式，可以实现高效的低精度推理。SGLang 是一个大语言模型推理引擎，利用推测解码每步生成多个 token，从而降低延迟。IndexShare 是一种跨层稀疏注意力复用技巧，可减少长上下文场景下的计算量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/introducing-nvfp4-for-efficient-and-accurate-low-precision-inference/">Introducing NVFP4 for Efficient and Accurate Low-Precision ...</a></li>
<li><a href="https://articles.phantom-byte.com/the-1m-context-mirage-what-indexshare-actually-delivers.html">1M Context Mirage: What IndexShare Delivers - PhantomByte</a></li>
<li><a href="https://sebastianraschka.com/blog/2026/glm-5-2-indexshare.html">GLM-5.2 IndexShare Architecture Note | Sebastian Raschka, PhD</a></li>

</ul>
</details>

**标签**: `#AI inference`, `#LLM serving`, `#GPU optimization`, `#speculative decoding`

---

<a id="item-2"></a>
## [QuadRF：开源软件无线电可探测无人机和 WiFi 信号](https://www.jeffgeerling.com/blog/2026/quadrf-can-spot-drones-and-see-wifi-through-my-wall/) ⭐️ 8.0/10

Jeff Geerling 的博文展示了 QuadRF，这是一款开源的 4x4 MIMO 软件无线电（SDR）模块，能够利用波束成形技术穿透墙壁探测无人机和 WiFi 信号。 该项目使相控阵波束成形技术变得价格亲民且易于获取，面向爱好者、安全研究人员和开源社区，可能催生新的射频探测应用，并提高人们对隐私的关注。 QuadRF 是一款 4 单元 SDR 模块，采用开放式天线架构，可通过 Crowd Supply 购买。它利用软件无线电分析射频信号，并根据用户反馈持续改进用户界面。

hackernews · speckx · 7月10日 15:59 · [社区讨论](https://news.ycombinator.com/item?id=48861717)

**背景**: 软件无线电（SDR）将无线电组件在软件而非硬件中实现，从而实现灵活的信号处理。相控阵波束成形利用多个天线以电子方式控制信号方向。QuadRF 结合了这两项技术，可探测并定位无人机和 WiFi 设备等射频源。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.crowdsupply.com/scale-rf/quadrf">QuadRF | Crowd Supply</a></li>
<li><a href="https://www.rtl-sdr.com/quadrf-4-element-beamforming-sdr-tile-coming-to-crowd-supply/">QuadRF: 4-Element Beamforming SDR Tile Coming to Crowd Supply</a></li>

</ul>
</details>

**社区讨论**: QuadRF 的创建者在评论区参与讨论，回答了有关校准和增益设置的问题。用户讨论了诸如声音探测等潜在应用，既对开源射频工具感到兴奋，也表达了对政府监控能力的担忧。

**标签**: `#hardware`, `#security`, `#RF`, `#open-source`, `#drones`

---

<a id="item-3"></a>
## [GPT-5.6 Sol Ultra 生成循环双覆盖猜想证明](https://cdn.openai.com/pdf/04d1d1e4-bc75-476a-97cf-49055cd98d31/cdc_proof.pdf) ⭐️ 8.0/10

据报道，OpenAI 的 GPT-5.6 Sol Ultra 模型生成了图论中长期未解决的循环双覆盖猜想的证明。该证明于 2026 年 7 月 10 日以预印本形式发布，同时附带了生成该证明所使用的提示词。 如果得到验证，这将是数学和人工智能领域的重大突破，表明大型语言模型能够解决开放的数学问题。这一成果可能会改变人们对 AI 在理论研究和自动定理证明中作用的看法。 该证明极为简洁，因此引发了专家们的质疑。根据 OpenAI 对 GPT-5.6 Sol 的预览，该模型使用了“最大推理努力”和“超模式”，通过子代理加速复杂工作。

hackernews · scrlk · 7月10日 18:29 · [社区讨论](https://news.ycombinator.com/item?id=48863490)

**背景**: 循环双覆盖猜想询问每个无桥无向图是否都有一个循环集合，使得每条边恰好出现两次。该猜想由 W. T. Tutte、Itai 和 Rodeh、George Szekeres 以及 Paul Seymour 提出。GPT-5.6 Sol Ultra 是 OpenAI 于 2026 年发布的最先进模型，分为 Luna、Terra 和 Sol 三个等级，其中 Sol 支持扩展推理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cycle_double_cover_conjecture">Cycle double cover conjecture</a></li>
<li><a href="https://openai.com/index/previewing-gpt-5-6-sol/">Previewing GPT - 5 . 6 Sol : a next-generation model | OpenAI</a></li>

</ul>
</details>

**社区讨论**: 社区评论既表达了兴奋也表达了怀疑。一些人指出该证明很简洁，可能利用了专家们忽略的巧妙技巧，而另一些人则质疑这是否真正构成了自主的“理论构建”证明。此外，还有人关注在开放问题上对前沿模型进行系统性测试。

**标签**: `#AI`, `#mathematics`, `#graph theory`, `#proof`, `#GPT-5.6`

---

<a id="item-4"></a>
## [优秀工具应无形](https://www.gingerbill.org/article/2026/07/10/good-tools-are-invisible/) ⭐️ 8.0/10

这篇文章主张，优秀的工具应减少摩擦、变得无形，让用户专注于任务本身而非工具。 这一理念挑战了常见的增加不必要复杂性的设计实践，影响开发者和设计师如何创造更好用户体验的工具。 文章讨论了“可自由选择的摩擦”这一概念，并指出工具变得无形不仅取决于初始设计，还与使用时间有关。

hackernews · theanonymousone · 7月10日 10:32 · [社区讨论](https://news.ycombinator.com/item?id=48858121)

**背景**: 工具应无形的理念在 UX 设计中很常见，常与“别让我思考”原则相关。好工具自然融入，用户不会注意它们。

**社区讨论**: 评论者普遍赞同但提出了细微差别。有人指出无形取决于用户体验，复杂任务中摩擦可能是必要的。还有人争论键盘与鼠标界面的价值。

**标签**: `#tool-design`, `#UX`, `#developer-experience`, `#philosophy`

---

<a id="item-5"></a>
## [成功公司如何变得盲目](https://ianreppel.org/how-successful-companies-go-blind/) ⭐️ 8.0/10

文章分析了成功公司如何对自身缺陷产生内部盲点，从而导致停滞和衰退。 这很重要，因为它揭示了组织衰退的常见模式，影响盈利能力和创新，对管理者和工程师都有参考价值。 文章引用了不同行业的实例，并讨论了官僚主义、风险规避以及缺乏新视角如何导致这种盲点。

hackernews · speckx · 7月10日 13:31 · [社区讨论](https://news.ycombinator.com/item?id=48859678)

**背景**: 组织盲点指的是公司因过去的成功而对自己的弱点视而不见，形成抗拒变革的文化。这一概念在商业管理文献中很常见。

**社区讨论**: 评论者分享了个人经历，其中一位指出在国防公司，惯性以及缺乏财务激励阻碍了创新。另一位指出，长期任职的管理者往往缺乏技能更新。第三位认为这更多是环境问题而非能力问题，因为官僚体制会阻碍有才华的人。

**标签**: `#organizational behavior`, `#company culture`, `#business strategy`, `#management`

---

<a id="item-6"></a>
## [SK 海力士 CEO：存储芯片短缺可能持续到 2030 年后](https://t.me/FinanceNewsDaily/490418) ⭐️ 8.0/10

SK 海力士 CEO 郭鲁正在彭博电视采访中表示，存储芯片供应短缺可能会持续到 2030 年之后。 来自顶级存储芯片制造商的长期预测表明，全球科技供应链将持续承压，影响从数据中心到消费电子等多个行业。 CEO 没有说明具体原因，但强调了半导体行业的结构性挑战，包括产能扩张延迟和需求上升。

telegram · FinanceNewsDaily · 7月10日 17:40

**背景**: 存储芯片包括 DRAM 和 NAND 闪存，是计算机、智能手机和服务器的关键组件。该行业经历了周期性的短缺，但近期地缘政治紧张和疫情驱动的需求加剧了供应限制。

**标签**: `#memory chips`, `#semiconductor supply chain`, `#SK Hynix`, `#hardware`, `#industry forecast`

---

<a id="item-7"></a>
## [SK 海力士 CEO 预测 2027 年将现史上最严重内存短缺](https://t.me/FinanceNewsDaily/490420) ⭐️ 8.0/10

SK 海力士首席执行官郭鲁正表示，全球内存行业正走向 2027 年史上最严重的供应短缺，预计未来十年内需求将持续超出公司的生产能力。 这家领先的内存制造商的预测预示着半导体市场可能面临重大干扰，可能影响从智能手机到数据中心等各种设备所用内存芯片的价格和供应。 郭鲁正指出，尽管积极扩充产能，未来十年需求仍将超过供应，并称 2027 年将是供应角度最糟糕的一年。该言论由路透社报道。

telegram · FinanceNewsDaily · 7月10日 19:50

**背景**: 内存芯片（包括 DRAM 和 NAND 闪存）是电子设备的关键部件。半导体行业历史上经历过因需求波动和新晶圆厂建设周期长而导致的短缺与过剩周期。长期短缺可能会限制消费电子和云基础设施的生产。

**标签**: `#memory`, `#semiconductor`, `#shortage`, `#SK Hynix`, `#industry forecast`

---

<a id="item-8"></a>
## [苹果起诉 OpenAI 窃取商业机密](https://t.me/FinanceNewsDaily/490421) ⭐️ 8.0/10

苹果对 OpenAI 提起重大诉讼，指控其窃取商业机密，并鼓励员工分享机密信息。 这起诉讼可能为人工智能行业的知识产权纠纷树立先例，影响公司如何保护商业机密以及与竞争对手合作。 苹果声称 OpenAI 鼓励其员工分享机密信息，可能泄露了苹果开发的专有技术。

telegram · FinanceNewsDaily · 7月10日 20:35

**背景**: 苹果和 OpenAI 是人工智能领域的主要参与者，苹果将人工智能集成到其产品中，而 OpenAI 开发了 GPT 等先进模型。商业机密诉讼虽不常见但意义重大，可能揭示内部做法并导致禁令或赔偿。

**标签**: `#Apple`, `#OpenAI`, `#lawsuit`, `#trade secrets`, `#AI`

---

<a id="item-9"></a>
## [中国法院裁定游戏账号可继承，平台禁止条款无效](https://www.tomshardware.com/tech-industry/big-tech/chinese-courts-allow-heirs-to-inherent-accounts-of-deceased-gamers-multiple-cases-spanning-years-establish-precedent-for-digital-ownership-of-games-in-game-items-and-microtransactions) ⭐️ 8.0/10

中国法院在多年来的多起判例中认定，游戏账号、游戏装备、加密货币及社交媒体运营权等虚拟资产具有财产属性，属于可继承的合法遗产，并判定平台用户协议中的“禁止继承”条款因违反法定权利而无效。 这为中国数字资产继承权确立了里程碑式的法律先例，可能影响数百万用户，并迫使平台调整政策。其影响可能波及全球关于数字财产权和虚拟资产用户所有权的讨论。 法院裁定，聊天记录等纯个人隐私内容不在继承范围内，由平台归档保存；平台可收取合理费用协助转移。这些判决依据《中华人民共和国民法典》，该法典将虚拟财产纳入遗产范围。

telegram · zaihuapd · 7月10日 02:56

**背景**: 数字遗产是指个人去世后遗留的数字资产，如网络账号、加密货币和虚拟物品等。中国自 2021 年起施行的《民法典》规定虚拟财产受法律保护，但继承细则此前存在争议。这些法院判例明确了具有经济价值的数字资产可以被继承，即使平台条款另有规定。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ailegal.baidu.com/legalarticle/qadetail?id=10903050849a99251031">网络虚拟财产继承经典法院案例 - ailegal.baidu.com</a></li>
<li><a href="https://www.lutongls.com/minshi/470.html">我国虚拟财产继承法律问题研究-上海陆同律师事务所</a></li>
<li><a href="https://china.cnr.cn/gdgg/20221002/t20221002_526026303.shtml">china.cnr.cn/gdgg/20221002/t20221002_526026303.shtml</a></li>

</ul>
</details>

**标签**: `#digital inheritance`, `#Chinese law`, `#virtual property`, `#gaming`, `#digital rights`

---

<a id="item-10"></a>
## [Anthropic 网页爬虫导流比达 2800:1](https://www.businessinsider.com/anthropic-web-bots-crawling-referrals-cloudflare-distillation-2026-7) ⭐️ 8.0/10

根据 Cloudflare 2026 年 7 月 1 日至 7 日的数据，Anthropic 的网页爬虫每抓取 2800 个页面仅带回一次导流访问，在主要 AI 公司中抓取与导流比例最高。 这种不平衡凸显了 AI 公司在训练时大量消耗网页内容，却几乎不给发布商回馈流量，引发了关于内容许可和开放网络资源可持续性的伦理与经济担忧。 该比例较 2026 年 4 月初的约 8800:1 有所下降，但在 5 月第一周曾高达 24700:1。Anthropic 质疑 Cloudflare 的统计方法，表示无法验证相关计算，并称其新搜索功能正在增加导流访问量。

telegram · zaihuapd · 7月10日 04:25

**背景**: Cloudflare Radar 追踪抓取与导流比，比较 AI 机器人抓取网站的频次与通过导流将用户带回网站的频次。据 Cloudflare 称，到 2025 年中，AI 训练驱动了近 80% 的 AI 爬虫活动，而给发布商的导流却在下降。OpenAI、Google 和 Anthropic 等主要 AI 公司因其爬取行为及其对网络生态的影响而受到审视。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.businessinsider.com/anthropic-web-bots-crawling-referrals-cloudflare-distillation-2026-7">Anthropic Treats the Web Like an All-You-Can-Eat... - Business Insider</a></li>
<li><a href="https://blog.cloudflare.com/ai-search-crawl-refer-ratio-on-radar/">The crawl before the fall… of referrals : understanding AI’s impact on...</a></li>
<li><a href="https://privacy.anthropic.com/en/articles/10023637-does-anthropic-crawl-data-from-the-web-and-how-can-site-owners-block-the-crawler">Does Anthropic crawl data from the web , and how can site owners...</a></li>

</ul>
</details>

**标签**: `#AI`, `#web scraping`, `#content licensing`, `#traffic analytics`, `#Anthropic`

---

<a id="item-11"></a>
## [长征十号乙实现全球首次网系火箭海上回收](https://weibo.com/7340734455/R814of1Ki) ⭐️ 8.0/10

2026 年 7 月 10 日，中国长征十号乙运载火箭从海南商业航天发射场升空，在级间分离约 6 分钟后，一子级通过网系捕获方式在海上回收平台成功回收，实现了全球首次运载火箭网系回收。 这一突破展示了一种新型可重复使用火箭技术，无需着陆支腿，有望降低未来太空任务的成本和复杂性，并使中国在火箭回收领域与 SpaceX 的推进式着陆方式并驾齐驱。 回收采用船上井字形阻拦索网系捕获火箭挂钩，实现无缓冲支腿的低冲击可重复使用着陆。长征十号乙成为中国首型成功实施一子级可控回收的运载火箭。

telegram · zaihuapd · 7月10日 04:36

**背景**: 火箭一子级回收是实现可重复使用的关键，可降低发射成本。SpaceX 率先实现了海上和陆地的推进式着陆。中国的网系回收方法提供了一种替代方案，避免了复杂的着陆支腿和精确的发动机反推，可能简化某些任务的回收流程。

<details><summary>参考链接</summary>
<ul>
<li><a href="http://www.ce.cn/xwzx/gnsz/gdxw/202607/t20260710_3080704.shtml">ce.cn/xwzx/gnsz/gdxw/202607/t20260710_3080704.shtml</a></li>
<li><a href="https://www.spacechina.com/n25/n2014789/n2414549/c4646874/content.html">长十乙火箭成功实现一子级可控回收_中国航天科技集团</a></li>
<li><a href="https://www.locpg.gov.cn/20260710/90f9157af72247dc9c5524ab8013da0a/c.html">长征十号乙运载火箭实现一子级可控回收</a></li>

</ul>
</details>

**标签**: `#aerospace`, `#rocket recovery`, `#China space`, `#engineering`

---

<a id="item-12"></a>
## [腾讯洽购 AI 公司 Manus，拟从 Meta 手中回购](https://www.reuters.com/technology/tencent-talks-become-ai-start-up-manus-largest-shareholder-ft-reports-2026-07-10/) ⭐️ 8.0/10

腾讯正在谈判收购 AI 初创公司 Manus，计划联合原投资者真格基金和 HSG 以至少 20 亿美元从 Meta 手中回购股份，成为其最大股东。 这笔交易反映了 AI 领域日益激烈的竞争和地缘政治紧张局势——北京此前要求 Meta 解除对 Manus 的收购。同时也标志着腾讯在 AI 代理技术上的战略布局。 交易金额不低于 20 亿美元，腾讯将与现有投资者真格基金和 HSG 联手买断 Meta 持有的股份。该消息由《金融时报》率先报道，腾讯、Manus、Meta 及两家投资方均未回应置评请求。

telegram · zaihuapd · 7月10日 06:45

**背景**: Manus 是一个 AI 代理平台，被称为“行动引擎”，超越了对话式 AI，能够规划并执行研究、分析、浏览和构建等多步骤任务。该初创公司此前被 Meta 收购，但北京出于监管考虑要求 Meta 剥离。腾讯作为中国科技巨头，正寻求在激烈竞争中扩展其 AI 能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/Manus_AI_company">Manus ( AI company ) — Grokipedia</a></li>
<li><a href="https://manus.im/">Manus : Hands On AI</a></li>
<li><a href="https://medium.com/@fahey_james/manus-ai-company-profile-352cf236db47">Manus AI company profile | by James Fahey | Medium</a></li>

</ul>
</details>

**标签**: `#Tencent`, `#Meta`, `#AI`, `#acquisition`, `#Manus`

---

<a id="item-13"></a>
## [OpenAI 与 Google 被指通过新加坡向黑名单中国企业提供 AI](https://www.ft.com/content/5d6aafa1-5d47-4585-aa95-6ec06a6cd20f) ⭐️ 8.0/10

OpenAI 和 Google 一直向阿里巴巴、百度和腾讯的新加坡子公司提供先进 AI 服务，而这些公司的母公司均被列在美国国防部 1260H 名单上，该名单指控相关实体与中国军方存在关联。 这引发了对美国 AI 技术出口管制有效性的新质疑，因为企业仍可通过海外子公司获取先进模型，可能削弱国家安全政策。 OpenAI 此前在发现疑似“模型蒸馏”行为后，暂停了阿里巴巴关联用户的 API 访问并上报美国政府；而 Anthropic 采取了更严格的政策，全面禁止中国实体及其海外关联方访问其前沿模型。

telegram · zaihuapd · 7月10日 09:59

**背景**: 美国国防部维护的 1260H 名单用于标识据称与中国人民解放军有联系的中国公司。模型蒸馏是一种将知识从大型 AI 模型转移到小型模型的技术，可用于规避 API 限制。当前的美国出口管制并未广泛禁止中国母公司在中国大陆以外获取先进 AI 模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.war.gov/News/Releases/Release/Article/4511232/dow-releases-list-of-chinese-military-companies-in-accordance-with-section-1260/">DOW Releases List of Chinese Military Companies in Accordance ...</a></li>
<li><a href="https://www.ibm.com/think/topics/knowledge-distillation">What is Knowledge distillation? | IBM</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#export controls`, `#OpenAI`, `#Google`, `#China`

---

<a id="item-14"></a>
## [中国对氦气实施临时出口禁令](https://wms.mofcom.gov.cn/zcfb/wmgl/art/2026/art_2a795a0d55df4cada91c9fbd2a2cc13a.html) ⭐️ 8.0/10

2026 年 7 月 10 日，中国商务部和海关总署联合发布公告，对氦气（海关商品编号 2804290010）实施临时禁止出口管理，自公布之日起执行。 该政策显著收紧了全球氦气供应，因为中国是主要生产国；这可能会扰乱依赖氦气的半导体制造、医疗成像和科研等领域。 该禁令适用于所列氦气产品的所有出口，未规定结束日期；后续调整将另行公告，该措施依据《中华人民共和国对外贸易法》制定。

telegram · zaihuapd · 7月10日 13:27

**背景**: 氦气是一种不可再生的惰性气体，对低温制冷、焊接以及作为 MRI 机器和半导体制造中的冷却剂至关重要。中国一直在扩大氦气产能，此类出口管制可用作技术竞争中的战略工具。

**标签**: `#helium`, `#trade policy`, `#supply chain`, `#semiconductors`, `#science`

---

<a id="item-15"></a>
## [Meta 因成瘾设计面临欧盟 120 亿美元罚款](https://www.theverge.com/policy/963872/meta-eu-addictive-design-200b-fine-risk-digital-services-act-dsa) ⭐️ 8.0/10

欧盟委员会初步裁定，Meta 旗下 Facebook 和 Instagram 因其无限滚动、自动播放和个性化推荐等成瘾性设计，违反了《数字服务法》。 如果最终裁定成立，Meta 可能面临高达 120 亿美元（占全球年营收 6%）的罚款，这将是《数字服务法》下用户安全监管的里程碑，迫使大型平台重新设计核心参与功能。 欧盟批评 Meta 现有的限时工具形同虚设，要求默认关闭成瘾功能、设置有效的屏幕休息时间，并弱化以参与度为导向的推荐算法。

telegram · zaihuapd · 7月10日 14:47

**背景**: 《数字服务法》（DSA）是 2022 年生效的欧盟法规，为数字服务问责制建立了全面的框架。它对 Facebook 和 Instagram 等月活跃用户超过 4500 万的超大型在线平台施加了最严格的义务，要求平台评估并减轻系统性风险，包括对用户心理健康的风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Digital_Services_Act">Digital Services Act</a></li>
<li><a href="https://grokipedia.com/page/Digital_Services_Act">Digital Services Act</a></li>

</ul>
</details>

**标签**: `#regulation`, `#Meta`, `#EU`, `#Digital Services Act`, `#addictive design`

---