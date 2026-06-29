---
layout: default
title: "Horizon Summary: 2026-06-29 (EN)"
date: 2026-06-29
lang: en
---

> From 49 items, 4 important content pieces were selected

---

1. [Memory Prices from 1960 to 2026: A Historical Chart](#item-1) ⭐️ 8.0/10
2. [Using Claude Code for MRI Second Opinion Sparks Debate](#item-2) ⭐️ 8.0/10
3. [Interactive transformer lets you edit weights live](#item-3) ⭐️ 8.0/10
4. [Google Restricts Meta's Gemini Access Due to Compute Shortage](#item-4) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Memory Prices from 1960 to 2026: A Historical Chart](https://dam.stanford.edu/memory-prices.html) ⭐️ 8.0/10

Stanford University's DAM Lab published a comprehensive chart and discussion detailing memory (RAM) prices from 1960 through projected 2026, showing a dramatic long-term decline with periodic cycles. This long-term dataset enables analysis of price trends, inflation effects, and market cycles in the semiconductor industry, helping to understand the historical and future trajectory of memory costs. The chart is not inflation-adjusted, which would make early prices appear even higher. Prices per gigabyte before 1990 were unrealistic as systems didn't have GB-scale memory then.

hackernews · vga1 · Jun 28, 18:32 · [Discussion](https://news.ycombinator.com/item?id=48710092)

**Background**: Memory prices have followed a long-term exponential decline with periodic booms and busts due to supply-demand cycles and technology node transitions. The dataset is a continuation of the previously maintained jcmit.com dataset, now hosted by Stanford.

**Discussion**: Commenters noted the non-inflation-adjusted data, shared personal memories of high memory costs in the 1980s-1990s, and questioned the AI-driven price spike's impact on future hardware upgrades. They also discussed the repeating price cycles and the dataset's long-term preservation.

**Tags**: `#memory`, `#hardware`, `#history`, `#pricing`, `#semiconductor`

---

<a id="item-2"></a>
## [Using Claude Code for MRI Second Opinion Sparks Debate](https://antoine.fi/mri-analysis-using-claude-code-opus) ⭐️ 8.0/10

A user uploaded their MRI images to Claude Code, Anthropic's AI model, to obtain a second opinion on a shoulder injury, documenting the experience in a blog post. This experiment highlights the growing potential of AI to assist in medical diagnostics, but also raises critical questions about trust, accuracy, and the proper role of AI in healthcare. The user used Claude Opus, the most capable variant of Claude, to analyze MRI scans of their shoulder and compare findings with their radiologist's report. The community discussion included a radiologist noting that ultrasound is not reliable for detecting calcification, a key point in the user's case.

hackernews · engmarketer · Jun 28, 16:35 · [Discussion](https://news.ycombinator.com/item?id=48708941)

**Background**: Claude is a series of large language models developed by Anthropic, known for its constitutional AI approach to alignment. Claude Code is an AI coding agent that can also process text and images, making it adaptable for tasks like analyzing medical images, though it is not specifically designed or certified for medical use.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**Discussion**: Comments from radiologists and patients reveal deep concerns about AI reliability and the psychological impact of second-guessing professional diagnoses. Some users shared personal misdiagnosis stories, while a radiologist emphasized that without seeing the full 3D MRI dataset, it's hard to evaluate the AI's accuracy.

**Tags**: `#AI`, `#healthcare`, `#radiology`, `#second opinion`, `#Claude Code`

---

<a id="item-3"></a>
## [Interactive transformer lets you edit weights live](https://www.reddit.com/r/MachineLearning/comments/1uhw7fu/i_shrank_a_transformer_until_every_number_fitted/) ⭐️ 8.0/10

A software engineer created a self-contained HTML page that shrinks a full transformer to a 6-word vocabulary and 3D embeddings, with editable weights that recompute the entire forward pass live. This tool makes transformer internals—from word vectors to attention scores to logits—visually accessible and manipulable, greatly lowering the barrier for self-learners to understand LLM mechanics. The page uses a single attention head, one transformer block, and a 6-word vocabulary with 3-dimensional embeddings. All weights are editable and downstream values update instantly, but backpropagation is intentionally omitted.

reddit · r/MachineLearning · /u/DanielMoGo · Jun 28, 12:35

**Background**: Transformers are the core architecture behind modern LLMs like GPT. They use self-attention with Query, Key, Value projections and a causal mask to prevent the model from seeing future tokens. This interactive page visualizes the entire forward pass step by step.

<details><summary>References</summary>
<ul>
<li><a href="https://poloclub.github.io/transformer-explainer/">Transformer Explainer: LLM Transformer Model Visually Explained</a></li>
<li><a href="https://machinelearningmastery.com/a-gentle-introduction-to-attention-masking-in-transformer-models/">A Gentle Introduction to Attention Masking in Transformer ...</a></li>
<li><a href="https://www.codecademy.com/article/transformer-architecture-self-attention-mechanism">Transformer Architecture Explained With Self-Attention Mechanism | Codecademy</a></li>

</ul>
</details>

**Tags**: `#transformer`, `#education`, `#interactive visualization`, `#forward pass`, `#LLM mechanics`

---

<a id="item-4"></a>
## [Google Restricts Meta's Gemini Access Due to Compute Shortage](https://www.ft.com/content/c5d52f72-71ef-40bc-bad3-61afdba8b378) ⭐️ 8.0/10

In March 2026, Google informed Meta that it could not provide the full Gemini capacity Meta had purchased, forcing Meta to prioritize internal AI models like Muse Spark and urge employees to use AI tokens more efficiently. This highlights a severe AI compute bottleneck affecting even the largest tech companies, and may accelerate the industry shift toward self-developed models and more efficient token usage. Google's compute constraints were acknowledged by CEO Sundar Pichai in April 2026 earnings call, and Google signed a $920 million per month deal with SpaceX to expand capacity. Meta's new Muse Spark model (launched April 2026) is a closed model, marking a break from its open-source Llama strategy.

telegram · zaihuapd · Jun 28, 07:38

**Background**: Gemini is Google's family of multimodal large language models, successor to LaMDA and PaLM 2. Compute shortages in AI are widespread due to surging demand for training and inference. Meta Muse Spark is Meta's most advanced AI model, launched in April 2026, and unlike prior open releases, it is a closed model.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gemini_(AI_model)">Gemini (AI model)</a></li>
<li><a href="https://metamusespark.in/">MetaMuseSpark - Your Guide to Meta 's AI Revolution</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Compute Shortage`, `#Google`, `#Meta`, `#Gemini`

---