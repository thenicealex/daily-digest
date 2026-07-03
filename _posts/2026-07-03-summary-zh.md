---
layout: default
title: "Horizon Summary: 2026-07-03 (ZH)"
date: 2026-07-03
lang: zh
---

> 从 74 条内容中筛选出 12 条重要资讯。

---

1. [欧洲议会间谍调查员遭飞马间谍软件攻击](#item-1) ⭐️ 8.0/10
2. [本地运行顶级大型语言模型指南](#item-2) ⭐️ 8.0/10
3. [Wordgard：ProseMirror 创建者推出的新富文本编辑器](#item-3) ⭐️ 8.0/10
4. [将代码转为图片降低 LLM 成本 60%的新工具](#item-4) ⭐️ 8.0/10
5. [对 MVP 误用和创始人动机的批判](#item-5) ⭐️ 8.0/10
6. [CDD 仅从 logits 恢复微调逐字数据](#item-6) ⭐️ 8.0/10
7. [国家金融监管总局接管众邦银行因信用风险](#item-7) ⭐️ 8.0/10
8. [Anthropic 指控阿里巴巴对 Claude 发动大规模蒸馏攻击](#item-8) ⭐️ 8.0/10
9. [华为 Atlas 350 加速卡算力达 H20 近三倍](#item-9) ⭐️ 8.0/10
10. [阿里巴巴禁止员工使用 Claude 及 Anthropic 产品](#item-10) ⭐️ 8.0/10
11. [NASA 发射救援卫星，抢救即将坠落的太空望远镜](#item-11) ⭐️ 8.0/10
12. [腾讯阿图因 AI 在 CyberGym 测试中击败 Mythos](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [欧洲议会间谍调查员遭飞马间谍软件攻击](https://citizenlab.ca/research/member-of-committee-investigating-spyware-hacked-with-pegasus/) ⭐️ 8.0/10

公民实验室发现，欧洲议会间谍软件调查委员会成员斯特利奥斯·库洛格卢的 iPhone 在 2022 年 10 月和 2023 年 3 月两次被飞马间谍软件感染。 此案突显了调查间谍软件的人员反被同一技术盯上的讽刺与危险，揭示了欧盟机构面临的持续间谍威胁，以及加强网络安全措施的必要性。 公民实验室高度确信地确认了感染事件，且被入侵的手机中还包含机密个人医疗信息和政府文件，引发了对工作与个人设备未分离的担忧。

hackernews · ledoge · 7月3日 20:38 · [社区讨论](https://news.ycombinator.com/item?id=48779683)

**背景**: 飞马（Pegasus）是以色列 NSO 集团开发的强大商业间谍软件，能够远程、隐蔽地监控移动设备。公民实验室位于多伦多大学，是研究数字间谍活动的领先机构，曾曝光全球多起飞马滥用事件。库洛格卢是欧洲议会调查欧盟内部飞马等间谍软件使用情况的委员会成员。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pegasus_(spyware)">Pegasus (spyware)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Citizen_Lab">Citizen Lab</a></li>

</ul>
</details>

**社区讨论**: 社区评论强调了希腊持续的间谍软件丑闻，认为此次攻击可能由希腊政府而非外国势力策划。部分讨论涉及设备安全，指出使用独立的工作和个人设备或增强隐私的操作系统（如 GrapheneOS）本可降低风险。还有人指出欧盟成员国曾滥用飞马，破坏了联盟内部的信任。

**标签**: `#spyware`, `#Pegasus`, `#cybersecurity`, `#European Parliament`, `#Citizen Lab`

---

<a id="item-2"></a>
## [本地运行顶级大型语言模型指南](https://github.com/jamesob/local-llm) ⭐️ 8.0/10

Jamesob 在 GitHub 发布了一份新指南，详细介绍了本地运行最先进大语言模型的硬件配置，从经济型到高达 5 万美元的高端方案。 该指南回应了日益增长的本地 AI 推理兴趣，为希望保护隐私、离线使用或避免订阅费用的爱好者和专业人士提供了实用建议，同时也引发了关于其与云服务成本效益的讨论。 最高端配置使用四块单价 1.2 万美元的 GPU，总花费约 5 万美元，号称能接近 Claude Opus 的性能；低成本方案包括双 RTX 3090（48 GB 显存）约 3000 美元，或采用统一内存架构的 M5 MacBook Pro。

hackernews · livestyle · 7月3日 15:03 · [社区讨论](https://news.ycombinator.com/item?id=48775921)

**背景**: 本地运行大语言模型需要大量 GPU 显存来存储模型权重，通常需要采用量化技术来减少内存占用。高端配置可能花费数万美元，而云订阅服务如 Claude Opus（每月 200 美元）提供了更便宜的替代方案。本指南帮助用户根据预算选择合适的硬件。

**社区讨论**: 评论者就成本效益展开辩论，jacobgold 指出 4 万美元的硬件相当于 16.8 年的 Claude 订阅费用。其他人建议使用 128 GB 统一内存系统或云托管等替代方案，而 Aurornis 警告存在隐藏成本和对量化技术的依赖。

**标签**: `#LLMs`, `#local inference`, `#hardware`, `#GPU`, `#AI`

---

<a id="item-3"></a>
## [Wordgard：ProseMirror 创建者推出的新富文本编辑器](https://wordgard.net/) ⭐️ 8.0/10

Wordgard 0.1.0 已发布，这是一款由 ProseMirror 的创建者 Marijn Haverbeke 开发的新款浏览器内富文本编辑器。它与 ProseMirror 共享许多概念，但引入了重新设计的架构和自定义文档模型。 Wordgard 代表了 Web 富文本编辑领域的一次重要演进，它来自受信任的作者，但现有 ProseMirror 用户需要付出大量的迁移工作。这可能会分裂生态系统，或者推动创新。 根据文档，从 ProseMirror 到 Wordgard 没有直接的升级路径。该编辑器仍处于早期开发阶段（版本 0.1.0），创建者已保证 ProseMirror 不会被弃用。

hackernews · indy · 7月3日 08:50 · [社区讨论](https://news.ycombinator.com/item?id=48772573)

**背景**: ProseMirror 是一个广泛使用的开源库，用于构建具有所见即所得界面的富文本编辑器，以其可扩展的 schema 和协作编辑支持而闻名。它是 Tiptap 等编辑器的基础。Wordgard 是同一作者的新系统，重新思考了 ProseMirror 的一些核心设计决策。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://discuss.prosemirror.net/t/wordgard-0-1-0/9035">Wordgard 0.1.0 - Announce - discuss.ProseMirror</a></li>
<li><a href="https://prosemirror.net/">ProseMirror</a></li>

</ul>
</details>

**社区讨论**: 社区讨论总体积极，但注意到缺乏迁移路径。一位用户称赞了设计，另一位用户对看到与自己基于块的实现相似之处表示欣慰。还有评论者强调了为此类编辑器制定 Web 标准的必要性。

**标签**: `#rich-text editor`, `#ProseMirror`, `#web development`, `#WYSIWYG`

---

<a id="item-4"></a>
## [将代码转为图片降低 LLM 成本 60%的新工具](https://github.com/teamchong/pxpipe) ⭐️ 8.0/10

一款名为 pxpipe 的新工具将代码转换为图片，利用更便宜的图像 token 定价，将 LLM API 成本降低高达 60%。 这一巧妙技巧大幅降低了使用 LLM 处理代码相关任务的成本，使其更易获取，同时揭示了 LLM API 中可能被利用的定价不一致问题。 该工具将代码格式化为图片，并依赖 LLM 内置的 OCR 功能读取文本，节省来自较低的图像 token 定价。但若提供商调整 token 计费，这可能只是临时漏洞。

hackernews · dimitropoulos · 7月3日 15:50 · [社区讨论](https://news.ycombinator.com/item?id=48776464)

**背景**: LLM 通常对文本和图像按 token 收费，图像 token 定价往往更低。一些提供商如 Gemini 在处理 PDF 时内部执行 OCR 而不收文本 token 费用，暗示可能存在类似后端处理。该工具利用这种定价差异来降低代码输入的成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.roboflow.com/image-token-cost-vlm/">What does it cost to process an image with a vision model?</a></li>
<li><a href="https://cloud.google.com/blog/products/ai-machine-learning/what-is-ocr">What is OCR | Google Cloud Blog</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，这可能是 token 计费中的漏洞，可能会被修复，类似于过去使用 OpenAI 模型的尝试，因增加完成 token 而导致总成本更高。还有人将其与使用图像进行上下文压缩的 Oh-My-Pi 等工具比较，有人调侃这是重新发现压缩数据表示。

**标签**: `#LLM`, `#cost optimization`, `#hack`, `#OCR`, `#token pricing`

---

<a id="item-5"></a>
## [对 MVP 误用和创始人动机的批判](https://weli.dev/blog/half-baked-product/) ⭐️ 8.0/10

这篇博客文章探讨了如何误用最小可行产品（MVP）概念导致产品半成品，并以一个创始人主要动机是财富而非领域专业知识为例进行说明。 它揭示了创业文化中的一个常见陷阱：将 MVP 用作发布不完整产品的借口，并强调了真正的领域专业知识胜过市场驱动的机会主义。 文章指出，该创始人在不同行业有多个失败的创业项目，原因是缺乏领域专业知识，并且 MVP 被误用来跳过关键的产品开发步骤。

hackernews · weli · 7月3日 08:23 · [社区讨论](https://news.ycombinator.com/item?id=48772388)

**背景**: 最小可行产品（MVP）是 Eric Ries 在精益创业方法论中推广的概念，被定义为允许团队以最小努力收集最多关于客户的验证学习的版本。然而在实践中，它常被误解为廉价、不完整的产品，而非学习工具。这种批判认为，当创始人优先考虑财富而非理解其领域时，他们会滥用 MVP 来推出半成品。

**社区讨论**: 评论者对 MVP 的误用表示沮丧，指出创始人往往缺乏领域专业知识而依赖市场分析。一位评论者讽刺地提到一个洗碗机初创公司的原型会打碎玻璃，说明了半成品问题。另一位评论者强调了初创公司中不同角色之间的脱节。

**标签**: `#MVP`, `#startup`, `#product development`, `#founder motivation`

---

<a id="item-6"></a>
## [CDD 仅从 logits 恢复微调逐字数据](https://www.reddit.com/r/MachineLearning/comments/1umn2dk/contrastive_decoding_diffing_cdd_recovering/) ⭐️ 8.0/10

研究人员提出对比解码差分（CDD）方法，通过对比基础模型和微调模型的 logits 来恢复逐字微调数据，仅需 logit 访问权限（无需权重或激活值）。 该技术极大提升了模型审计和可解释性，与之前的白盒方法相比，能以最小访问权限检测逐字训练数据泄露和潜在后门。 CDD 在四个模型系列（1B-32B 参数）的 20 个有机体-模型对中的 19 对上取得了 4+/5 的逐字恢复分数，超越了需要完全权重访问但从未超过 3/5 的激活差分透镜（ADL）。

reddit · r/MachineLearning · /u/CebulkaZapiekana · 7月3日 19:01

**背景**: 模型差分是比较基础模型和微调模型以理解变化的方法。先前的工作（激活差分透镜）使用激活差异但需要白盒访问，且只能恢复模糊描述。CDD 是对比 logits 的输出级类比。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aiwiki.ai/wiki/contrastive_decoding">Contrastive decoding | AI Wiki</a></li>
<li><a href="https://transformer-circuits.pub/2024/model-diffing/index.html">Stage-Wise Model Diffing</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#model diffing`, `#LLM finetuning`, `#interpretability`, `#security`

---

<a id="item-7"></a>
## [国家金融监管总局接管众邦银行因信用风险](https://t.me/FinanceNewsDaily/490005) ⭐️ 8.0/10

国家金融监督管理总局联合湖北省人民政府宣布对武汉众邦银行股份有限公司实施接管，原因是该行出现严重信用风险。此举依据《银行业监督管理法》和《商业银行法》，旨在保护存款人和其他客户的合法权益。 此次接管表明中国银行业监管力度加大，凸显了中小银行面临的系统性风险。干预旨在防止风险蔓延、维护金融稳定，对存款人和整个银行业生态具有重要影响。 众邦银行是一家总部位于武汉的商业银行，因出现严重信用风险而被接管。根据中国法律，接管期间该银行股东会等权力机构停止履行职责，相关职能由监管机构指定的接管组行使。

telegram · FinanceNewsDaily · 7月3日 09:45

**背景**: 国家金融监督管理总局（金融监管总局）于 2023 年 3 月设立，是国务院直属机构，在原中国银行保险监督管理委员会基础上组建，并整合了中国人民银行的部分监管职责及中国证券投资者保护职责。银行接管是针对已经或可能发生信用危机、严重影响存款人利益的银行所采取的法律程序，监管机构可借此进行机构重组，帮助银行恢复正常经营。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zh.wikipedia.org/zh-cn/国家金融监督管理总局">国家金融监督管理总局 - 维基百科，自由的百科全书</a></li>
<li><a href="https://ailegal.baidu.com/legalarticle/qadetail?id=2d43012c49c25e250906">银行接管管理规定 - ailegal.baidu.com</a></li>
<li><a href="https://www.zhihu.com/question/387180588">商业银行接管的实质是什么？ - 知乎</a></li>

</ul>
</details>

**标签**: `#finance`, `#regulation`, `#banking`, `#risk`

---

<a id="item-8"></a>
## [Anthropic 指控阿里巴巴对 Claude 发动大规模蒸馏攻击](https://t.me/zaihuapd/42327) ⭐️ 8.0/10

Anthropic 致信美国参议院银行委员会，指控阿里巴巴通过近 2.5 万个欺诈账户对 Claude AI 模型发动大规模蒸馏攻击，以窃取其能力。 这一涉及两大 AI 巨头的指控凸显了通过蒸馏攻击窃取模型能力的日益严重威胁，可能加剧 AI 安全和国际科技竞争中的紧张局势。 攻击发生在 2026 年 4 月 22 日至 6 月 5 日期间，与 Claude 进行了超过 2880 万次交互，Anthropic 称这是针对该公司迄今已知最大规模的蒸馏攻击，涉及阿里巴巴及其 Qwen AI 实验室。

telegram · zaihuapd · 7月3日 06:21

**背景**: 模型蒸馏是一种技术，通过让较小的模型从较大、更强大的模型输出中学习，以高效复制其能力。虽然蒸馏是用于模型压缩的合法方法，但当大规模未经授权使用时，就变成了窃取专有模型功能的盗窃技术。Anthropic 一直在研究检测和防范此类攻击，但指出需要行业协同应对。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/detecting-and-preventing-distillation-attacks">Detecting and preventing distillation attacks \ Anthropic</a></li>
<li><a href="https://www.linkedin.com/pulse/what-model-distillation-really-means-why-anthropic-example-mahajan-sf2bf">What model “ distillation ” really means and why the Anthropic example...</a></li>
<li><a href="https://www.mindstudio.ai/blog/ai-model-distillation-attacks-explained">AI Model Distillation Attacks : What They Are and Why... | MindStudio</a></li>

</ul>
</details>

**标签**: `#AI security`, `#model distillation`, `#Anthropic`, `#Alibaba`, `#Claude`

---

<a id="item-9"></a>
## [华为 Atlas 350 加速卡算力达 H20 近三倍](https://t.me/zaihuapd/42329) ⭐️ 8.0/10

华为在 2026 年中国合作伙伴大会上正式发布并上市 Atlas 350 加速卡，搭载全新昇腾 950PR 处理器，声称其算力达到英伟达 H20 的 2.87 倍。 该产品标志着华为在 AI 推理市场挑战英伟达主导地位的最新尝试，特别是在出口限制持续背景下。支持 FP4 和高内存容量，有望大幅降低大语言模型的推理成本。 Atlas 350 在 FP4 精度下提供 1.56 PFLOPS 算力，并配备 112 GB 华为自研 HiBL 1.0 高带宽内存。它支持单卡加载 70B 参数模型，无需多卡组合。

telegram · zaihuapd · 7月3日 08:35

**背景**: FP4 是一种极低精度格式（4 位浮点），通过降低内存和计算需求来加速 AI 推理，同时保持可接受的精度。英伟达 H20 是为符合美国出口管制而在中国销售的降规 GPU。华为昇腾系列是国产替代品，在中国市场逐渐获得认可。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.huaweicentral.com/huawei-atlas-350-ai-card-debuts-outshining-nvidia-h20-chip/">Huawei Atlas 350 AI card debuts, outshining Nvidia H20 chip</a></li>
<li><a href="https://www.tomshardware.com/pc-components/gpus/huawei-unveils-new-atlas-350-ai-accelerator-with-1-56-pflops-of-fp4-compute-and-up-to-112gb-of-hbm-claims-2-8x-more-performance-than-nvidias-h20">Huawei unveils new Atlas 350 AI accelerator with 1.56 PFLOPS ...</a></li>
<li><a href="https://nerdleveltech.com/huawei-ascend-950pr-atlas-350-ai-chip-challenges-nvidia">Huawei Ascend 950PR Beats NVIDIA H20: 2.8× FP8, CUDA-Ready</a></li>

</ul>
</details>

**标签**: `#Huawei`, `#AI accelerators`, `#hardware`, `#FP4`, `#Atlas 350`

---

<a id="item-10"></a>
## [阿里巴巴禁止员工使用 Claude 及 Anthropic 产品](https://t.me/zaihuapd/42334) ⭐️ 8.0/10

阿里巴巴发布内部指令，要求所有员工卸载 Claude 及所有 Anthropic 相关产品，包括 Sonnet、Opus、Fable 等模型以及 Agent 产品 Claude Code，禁令于 7 月 10 日生效。 这一禁令标志着中国大型科技公司与西方领先 AI 公司之间紧张关系升级，可能重塑企业 AI 使用政策，并影响跨境 AI 竞争格局。 此次禁令前，Anthropic 指控阿里巴巴在 4 月 22 日至 6 月 5 日期间使用约 2.5 万个虚假账户与 Claude 交互超过 2800 万次，导致 Anthropic 收紧风控策略。此前，阿里巴巴曾报销员工使用 Claude、GPT、Gemini 等外部模型的费用。

telegram · zaihuapd · 7月3日 13:00

**背景**: Claude 是由美国 AI 安全公司 Anthropic 开发的一系列大型语言模型，包括 Haiku、Sonnet、Opus 和 Fable 等针对不同任务的优化版本。Claude Code 是一种智能编码工具，可以读取代码库并执行命令。阿里巴巴此举反映了企业在安全和竞争考虑下对外部 AI 工具日益严格的限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude ( AI ) - Wikipedia</a></li>
<li><a href="https://claude.com/resources/tutorials/choosing-the-right-claude-model">Choosing the right Claude model : Haiku, Sonnet , Opus , or Fable</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**标签**: `#AI`, `#Claude`, `#Alibaba`, `#corporate policy`, `#Anthropic`

---

<a id="item-11"></a>
## [NASA 发射救援卫星，抢救即将坠落的太空望远镜](https://apnews.com/article/swift-nasa-satellite-rescue-katalyst-a7ddd740ca099587c58865f583c7245a) ⭐️ 8.0/10

NASA 于 2026 年 6 月发射了 LINK 航天器，执行救援任务，计划抓住老化的雨燕太空望远镜并将其轨道抬升约 240 公里，以防止其最早在今年 10 月坠入大气层。 这次任务标志着私人航天器首次尝试抓取美国政府的无人卫星，展示了在轨服务和碎片减缓的新能力，未来可能延长哈勃太空望远镜等宝贵资产的寿命。 LINK 航天器由 Katalyst Space Technologies 根据 NASA 3000 万美元的合同开发，将使用机械臂固定雨燕，然后通过推进器缓慢抬升轨道；如果救援成功，雨燕最快可在 9 月恢复科学观测。

telegram · zaihuapd · 7月3日 15:43

**背景**: 雨燕是一台于 2004 年发射升空的空间天文台，用于研究伽马射线暴等宇宙现象。20 多年来，其轨道因太阳活动加剧而持续衰减，若不干预将坠入地球大气层烧毁。LINK 是一种专用的在轨服务飞行器，旨在交会并抓取老化卫星，抬升其轨道以延长运行寿命。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://baike.baidu.com/item/Link/67531114">Link（美国航天器）_百度百科</a></li>
<li><a href="https://www.msn.com/zh-cn/news/other/link卫星27日升空赴约-3000万-救星-力挽5亿美元雨燕天文台轨道危机/ar-AA262rcJ">Link卫星27日升空赴约：3000万“救星”力挽5亿美元雨燕天文台轨道危机</a></li>
<li><a href="https://news.qq.com/rain/a/20260630A04WGY00">“雨燕”坠落，NASA紧急“太空营救”，成功的话下次救“哈勃”</a></li>

</ul>
</details>

**标签**: `#航天`, `#太空望远镜`, `#轨道救援`, `#私人航天`, `#NASA`

---

<a id="item-12"></a>
## [腾讯阿图因 AI 在 CyberGym 测试中击败 Mythos](https://mp.weixin.qq.com/s/BzU7g-2iG7d6h4ViwMhxyg) ⭐️ 8.0/10

腾讯玄武实验室的阿图因 AI 基于开源模型 GLM-5.1 构建，在 CyberGym 网络安全基准测试中获得 84.0%的得分，超越 Anthropic 的 Claude Mythos Preview，且预算不到 Mythos 的 0.1%。 这表明高性能的网络安全 AI 可以通过低成本的开源模型实现，挑战了只有大规模专有模型才能胜任漏洞检测的假设。它可能以极低的成本使先进的 AI 安全工具更加普及。 阿图因 AI 还在 curl、gnark、OpenSSL、Python cryptography 和 Java bc-java 等项目中发现多个 Mythos 未检出的高危逻辑漏洞，最高严重性评分达 9.3。在伯克利 BVI 真实世界漏洞榜单中，阿图因 AI 的严重漏洞数量排名第一，总数排名第五。

telegram · zaihuapd · 7月3日 16:12

**背景**: CyberGym 是一个评估 AI 代理网络安全能力的基准测试，涵盖漏洞的完整生命周期。GLM-5.1 是由智谱 AI（Z.ai）开发的开源大语言模型，采用 MIT 许可证发布，支持本地部署。Claude Mythos Preview 是 Anthropic 的强大模型，此前在 CyberGym 排行榜上领先。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://llm-stats.com/benchmarks/cybergym">CyberGym Benchmark Leaderboard | LLM Stats</a></li>
<li><a href="https://en.wikipedia.org/wiki/GLM-5.1">GLM-5.1</a></li>
<li><a href="https://www.cybergym.io/cybergym-e2e/">CyberGym -E2E: Scalable Real-World Benchmark for AI Agents...</a></li>

</ul>
</details>

**标签**: `#AI安全`, `#网络安全`, `#腾讯`, `#GLM`, `#漏洞检测`

---