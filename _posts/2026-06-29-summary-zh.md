---
layout: default
title: "Horizon Summary: 2026-06-29 (ZH)"
date: 2026-06-29
lang: zh
---

> 从 49 条内容中筛选出 4 条重要资讯。

---

1. [1960 年至 2026 年内存价格历史图表](#item-1) ⭐️ 8.0/10
2. [使用 Claude Code 获取 MRI 第二意见引发热议](#item-2) ⭐️ 8.0/10
3. [交互式 Transformer：可实时编辑权重](#item-3) ⭐️ 8.0/10
4. [谷歌因算力短缺限制 Meta 使用 Gemini](#item-4) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [1960 年至 2026 年内存价格历史图表](https://dam.stanford.edu/memory-prices.html) ⭐️ 8.0/10

斯坦福大学 DAM 实验室发布了一张详尽图表及讨论，展示了从 1960 年到预计 2026 年的内存（RAM）价格，呈现了长期大幅下降及周期性波动。 这一长期数据集有助于分析半导体行业的价格趋势、通胀影响和市场周期，从而理解内存成本的历史和未来走向。 该图表未根据通胀调整，否则早期价格会显得更高。1990 年之前每 GB 的价格不切实际，因为当时的系统没有 GB 级内存。

hackernews · vga1 · 6月28日 18:32 · [社区讨论](https://news.ycombinator.com/item?id=48710092)

**背景**: 内存价格长期呈指数下降，并因供需周期和技术节点转换而出现周期性繁荣与萧条。该数据集是此前由 jcmit.com 维护的数据集的延续，现由斯坦福大学托管。

**社区讨论**: 评论者指出了数据未经通胀调整，分享了 20 世纪 80 至 90 年代内存价格高昂的个人记忆，并质疑 AI 驱动的价格上涨对未来硬件升级的影响。他们还讨论了重复的价格周期以及数据集的长期保存问题。

**标签**: `#memory`, `#hardware`, `#history`, `#pricing`, `#semiconductor`

---

<a id="item-2"></a>
## [使用 Claude Code 获取 MRI 第二意见引发热议](https://antoine.fi/mri-analysis-using-claude-code-opus) ⭐️ 8.0/10

一名用户将其肩部 MRI 图像上传至 Anthropic 的 AI 模型 Claude Code，以获取第二诊断意见，并在博客文章中记录了这一过程。 这一实验凸显了 AI 辅助医疗诊断的潜力，同时也引发了关于信任、准确性以及 AI 在医疗中合理角色的关键讨论。 用户使用了 Claude Opus（Claude 系列中最强大的变体）分析肩部 MRI 扫描结果，并与放射科医生的报告进行对比。社区讨论中一位放射科医生指出，超声波检查在检测钙化方面不可靠，而这正是用户案例中的关键点。

hackernews · engmarketer · 6月28日 16:35 · [社区讨论](https://news.ycombinator.com/item?id=48708941)

**背景**: Claude 是 Anthropic 公司开发的一系列大型语言模型，以其“宪法 AI”对齐方法而闻名。Claude Code 是一款 AI 编程代理，也能处理文本和图像，因此可适用于分析医学图像等任务，但并非为医疗用途专门设计或认证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**社区讨论**: 来自放射科医生和患者的评论揭示了人们对 AI 可靠性的深切担忧，以及对专业诊断产生怀疑的心理影响。一些用户分享了个人误诊经历，而一位放射科医生强调，在没有看到完整 3D MRI 数据集的情况下，很难评估 AI 的准确性。

**标签**: `#AI`, `#healthcare`, `#radiology`, `#second opinion`, `#Claude Code`

---

<a id="item-3"></a>
## [交互式 Transformer：可实时编辑权重](https://www.reddit.com/r/MachineLearning/comments/1uhw7fu/i_shrank_a_transformer_until_every_number_fitted/) ⭐️ 8.0/10

一位软件工程师制作了一个自包含的 HTML 页面，将完整 Transformer 缩小到 6 个词表和 3 维嵌入，权重可编辑且整个前向传播会实时重新计算。 该工具让 Transformer 的内部机制（从词向量到注意力分数再到 logits）变得直观可操作，极大降低了自学者理解 LLM 原理的门槛。 该页面使用单注意力头、单 Transformer 块、6 个词表以及 3 维嵌入。所有权重都可编辑，下游数值即时更新，但故意省略了反向传播。

reddit · r/MachineLearning · /u/DanielMoGo · 6月28日 12:35

**背景**: Transformer 是现代 LLM（如 GPT）的核心架构。它使用自注意力机制，包含 Query、Key、Value 投影以及因果掩码，以防止模型看到未来 token。该交互页面逐步可视化了整个前向传播过程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://poloclub.github.io/transformer-explainer/">Transformer Explainer: LLM Transformer Model Visually Explained</a></li>
<li><a href="https://machinelearningmastery.com/a-gentle-introduction-to-attention-masking-in-transformer-models/">A Gentle Introduction to Attention Masking in Transformer ...</a></li>
<li><a href="https://www.codecademy.com/article/transformer-architecture-self-attention-mechanism">Transformer Architecture Explained With Self-Attention Mechanism | Codecademy</a></li>

</ul>
</details>

**标签**: `#transformer`, `#education`, `#interactive visualization`, `#forward pass`, `#LLM mechanics`

---

<a id="item-4"></a>
## [谷歌因算力短缺限制 Meta 使用 Gemini](https://www.ft.com/content/c5d52f72-71ef-40bc-bad3-61afdba8b378) ⭐️ 8.0/10

2026 年 3 月，谷歌通知 Meta 无法提供其已购买的全部 Gemini 算力容量，迫使 Meta 优先使用内部 AI 模型如 Muse Spark，并鼓励员工更高效地使用 AI tokens。 这凸显了即使最大科技公司也面临的严重 AI 算力瓶颈，可能加速行业向自研模型和更高效 token 使用的转变。 谷歌 CEO Sundar Pichai 在 2026 年 4 月财报电话会议上承认算力受限，谷歌与 SpaceX 签署了每月 9.2 亿美元的协议以扩充容量。Meta 新推出的 Muse Spark 模型（2026 年 4 月发布）是闭源模型，标志着其开源 Llama 策略的转变。

telegram · zaihuapd · 6月28日 07:38

**背景**: Gemini 是谷歌的多模态大语言模型系列，是 LaMDA 和 PaLM 2 的继任者。AI 算力短缺普遍存在，原因是训练和推理需求激增。Meta Muse Spark 是 Meta 最先进的 AI 模型，于 2026 年 4 月发布，与之前开源发布不同，它是闭源模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gemini_(AI_model)">Gemini (AI model)</a></li>
<li><a href="https://metamusespark.in/">MetaMuseSpark - Your Guide to Meta 's AI Revolution</a></li>

</ul>
</details>

**标签**: `#AI`, `#Compute Shortage`, `#Google`, `#Meta`, `#Gemini`

---