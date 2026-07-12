---
layout: default
title: "Horizon Summary: 2026-07-12 (EN)"
date: 2026-07-12
lang: en
---

> From 28 items, 9 important content pieces were selected

---

1. [Claude Code uses 33k tokens vs OpenCode's 7k per prompt](#item-1) ⭐️ 8.0/10
2. [Irish datacenters consume 23% of country's electricity](#item-2) ⭐️ 8.0/10
3. [Terry Tao Uses LLM Coding Agents for Visualizations](#item-3) ⭐️ 8.0/10
4. [I Love LLMs, I Hate Hype](#item-4) ⭐️ 8.0/10
5. [Chromium 148's Math.tanh Enables OS Fingerprinting](#item-5) ⭐️ 7.0/10
6. [Anthropic Extends Claude Fable 5 Availability Amid Compute Constraints](#item-6) ⭐️ 6.0/10
7. [Zer0Fit: MCP Server for Google's TabFM & TimesFM](#item-7) ⭐️ 6.0/10
8. [Context-Based View of Neural Networks as Linear Mappings](#item-8) ⭐️ 6.0/10
9. [ACL conference acceptance process under ARR](#item-9) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Claude Code uses 33k tokens vs OpenCode's 7k per prompt](https://systima.ai/blog/claude-code-vs-opencode-token-overhead) ⭐️ 8.0/10

An empirical comparison found that Claude Code sends approximately 33,000 tokens before even reading the user's prompt, while OpenCode sends only about 7,000 tokens—a roughly 4.7x overhead due to inefficient cache strategy and harness token usage. This token inefficiency can significantly increase costs for developers using Claude Code, especially for large or frequent tasks, and raises questions about Anthropic's design incentives. The findings are actionable for practitioners choosing between agentic coding tools and optimizing their LLM usage. The study logged all requests between each tool and Anthropic's endpoint, measuring token counts before the first user prompt was processed. The authors noted that Claude Code's overhead comes from its cache strategy and harness token usage, not from the prompt itself.

hackernews · systima · Jul 12, 18:25 · [Discussion](https://news.ycombinator.com/item?id=48883275)

**Background**: Agentic coding tools like Claude Code and OpenCode use large language models (LLMs) to autonomously edit code, run commands, and interact with codebases. They rely on system prompts and harness logic that consume tokens before any user input is processed. Token efficiency directly impacts cost and speed, making it a critical metric for developers.

<details><summary>References</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://opencode.ai/docs/models/">Models | OpenCode</a></li>

</ul>
</details>

**Discussion**: Community comments raised concerns about sub-agents in Claude Code burning through budgets, with one user noting that seven sub-agents were launched for a single task. Others speculated that Anthropic may have financial incentives to inflate token usage, while some pointed out that prompt minimalism and tooling quality matter more than raw token counts.

**Tags**: `#agentic coding`, `#token efficiency`, `#Claude Code`, `#OpenCode`, `#LLM tooling`

---

<a id="item-2"></a>
## [Irish datacenters consume 23% of country's electricity](https://www.theregister.com/on-prem/2026/07/11/irish-datacenters-now-guzzle-23-of-the-countrys-electricity/5270013) ⭐️ 8.0/10

Irish datacenters now account for 23% of Ireland's total electricity consumption, according to recent reports highlighting a sharp rise in energy demand from the tech sector. This high proportion raises concerns about energy costs for households and businesses, as well as Ireland's ability to meet renewable energy targets while supporting a growing digital infrastructure. The 23% figure represents a significant increase from previous years, and coincides with electricity price hikes that have pushed residential rates to around 35 euro cents per kWh.

hackernews · Bender · Jul 12, 20:16 · [Discussion](https://news.ycombinator.com/item?id=48884322)

**Background**: Data centers are essential for cloud computing, streaming, and AI workloads, but they consume vast amounts of electricity for servers and cooling. Ireland has become a hub for major tech companies due to favorable corporate tax rates and a skilled workforce, leading to a rapid concentration of data centers on the island.

**Discussion**: Commenters express frustration over rising electricity costs, with some comparing the situation to other regions like California. Others argue that nuclear power or alternative policies could solve the energy strain, while skepticism about government priorities and affordability of green alternatives is widespread.

**Tags**: `#data centers`, `#energy consumption`, `#Ireland`, `#sustainability`, `#infrastructure`

---

<a id="item-3"></a>
## [Terry Tao Uses LLM Coding Agents for Visualizations](https://terrytao.wordpress.com/2026/07/11/old-and-new-apps-via-modern-coding-agents/) ⭐️ 8.0/10

Terry Tao, a Fields Medalist, published a blog post demonstrating how he used modern coding agents (LLMs) to rapidly build interactive visualizations for his research and teaching. This showcases the practical utility of LLM coding agents beyond conventional software development, especially in education and research, and highlights the large latent demand for custom software in non-traditional domains. Tao noted that while LLM-generated supplements are not mission-critical to his papers, the downside risk is acceptable for such visualizations. The blog post received 391 points and 111 comments on a popular aggregator, indicating strong community interest.

hackernews · subset · Jul 12, 11:09 · [Discussion](https://news.ycombinator.com/item?id=48880170)

**Background**: Coding agents are AI tools that generate code from natural language prompts, often using large language models (LLMs) like GPT-4 or Claude. They allow rapid prototyping of software, including interactive visualizations, without deep programming expertise. Terry Tao is a renowned mathematician, and his endorsement lends credibility to the approach.

<details><summary>References</summary>
<ul>
<li><a href="https://zencoder.ai/blog/best-free-ai-agents-for-coding">8 Best Free AI Agents for Coding To Try in 2026</a></li>

</ul>
</details>

**Discussion**: Commenters generally agreed with Tao's balanced perspective, noting the tool's usefulness for education and prototyping. Some humorously compared Tao's use of coding agents to a chef discovering microwave dinners. Others emphasized that there is infinite latent demand for software outside traditional tech spaces.

**Tags**: `#LLM`, `#coding agents`, `#education`, `#software development`, `#visualization`

---

<a id="item-4"></a>
## [I Love LLMs, I Hate Hype](https://geohot.github.io//blog/jekyll/update/2026/07/12/i-love-llms.html) ⭐️ 8.0/10

George Hotz published a blog post critiquing the disconnect between LLM hype and actual value delivered, arguing that frontier labs may not capture the value they create. This critique resonates with a growing sentiment that despite massive investments, the economic value of LLMs may flow to users and open-source communities rather than the companies building them. It challenges the valuation of frontier AI labs and highlights a shift toward decentralized, custom AI solutions. The post emphasizes that productivity improvements from LLMs have led to more private, one-off software rather than public innovations, and community comments coin the term 'have it your way' era. Some commenters note that newer models like Claude Sonnet 4 and Opus 4.5 are changing perceptions, but uncertainty about AGI timelines remains.

hackernews · therepanic · Jul 12, 18:31 · [Discussion](https://news.ycombinator.com/item?id=48883343)

**Background**: Frontier AI labs (e.g., OpenAI, Anthropic, Google DeepMind) are companies racing to build the most advanced AI models. They have raised billions of dollars and now charge subscription fees for access to their best models. However, open-source alternatives and the ability for individuals to customize AI for specific needs are growing, raising questions about value capture and the future of open source.

<details><summary>References</summary>
<ul>
<li><a href="https://www.forbes.com/sites/josipamajic/2026/07/02/karp-says-frontier-ai-labs-are-stealing-enterprise-value-and-vcs-are-listening/">Karp Says Frontier AI Labs Are Stealing Enterprise ... - Forbes</a></li>
<li><a href="https://www.linkedin.com/pulse/frontier-ai-labs-what-building-why-transformation-leaders-kumar-gbuge/">Frontier AI Labs: What They Are Building — and Why ...</a></li>

</ul>
</details>

**Discussion**: The community discussion is highly engaged, with top commenters agreeing with the value capture argument. One commenter notes that at current subscription prices, frontier models are a 'no-brainer' for many, while another introduces the concept of a 'have it your way' era where forking and customizing open-source projects is easier than ever. Some express concern about the future of open source, while others report that newer models are accelerating progress and making timelines uncertain.

**Tags**: `#LLMs`, `#AI hype`, `#open source`, `#productivity`, `#frontier labs`

---

<a id="item-5"></a>
## [Chromium 148's Math.tanh Enables OS Fingerprinting](https://scrapfly.dev/posts/browser-math-os-fingerprint/) ⭐️ 7.0/10

Chromium 148 (V8 14.8.57) changed Math.tanh to use std::tanh, which calls the host OS's math library, producing floating-point results that vary across operating systems and can be used to fingerprint the underlying OS. This novel fingerprinting technique affects all Chromium users and can be used by anti-bot systems to detect OS mismatches, undermining privacy and making browser spoofing harder. Only Chrome 148 and later (Chrome 148, 149, 150) are vulnerable; earlier versions are not. Besides OS, the technique can also fingerprint the browser version range due to implementation changes.

hackernews · joahnn_s · Jul 12, 21:12 · [Discussion](https://news.ycombinator.com/item?id=48884853)

**Background**: Floating-point arithmetic results can differ across operating systems due to different math library implementations. Browser fingerprinting exploits such subtle differences to identify users. Math.tanh is a transcendental function whose precision varies by platform, making it a signal for OS detection.

<details><summary>References</summary>
<ul>
<li><a href="https://scrapfly.dev/posts/browser-math-os-fingerprint/">Your Browser Does Math Differently on Every OS, and Anti-Bot Systems Read the Bits · scrapfly.dev</a></li>
<li><a href="https://neoprint.dev/guide/collectors/math.html">Math Fingerprinting — neoprint | Open-Source Browser ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Floating-point_arithmetic">Floating-point arithmetic - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Comments highlight that the technique can also fingerprint browser version range, not just OS. Some criticize the article's source (scrapfly) for self-interest, while others suggest correctly rounded transcendental functions as a fix. There is hope that EFF's Cover Your Tracks tool will include this signal.

**Tags**: `#privacy`, `#fingerprinting`, `#browser`, `#Chromium`, `#security`

---

<a id="item-6"></a>
## [Anthropic Extends Claude Fable 5 Availability Amid Compute Constraints](https://simonwillison.net/2026/Jul/12/bump/#atom-everything) ⭐️ 6.0/10

Anthropic announced an extension of Claude Fable 5 access on all paid plans through July 19, 2026, maintaining 50% higher weekly rate limits for Claude Code. This comes as OpenAI removes usage limits for GPT-5.6 Sol on Plus, Business, and Pro plans. This comparison highlights differing strategies in AI model access: Anthropic's cautious extension due to compute constraints vs. OpenAI's aggressive removal of limits. The uncertainty around Fable availability may drive users to OpenAI's GPT-5.6 Sol, shifting market dynamics. Users on Claude Max plans can use up to half of their weekly usage limit on Fable 5, after which they can pay with usage credits or switch models. OpenAI's GPT-5.6 Sol is reportedly a 'Fable/Mythos class' model, and its efficiency improvements will reduce usage consumption.

rss · Simon Willison · Jul 12, 21:20

**Background**: Claude Fable 5 is Anthropic's most capable model for demanding coding and visionary tasks, launched in June 2026. GPT-5.6 Sol is OpenAI's latest frontier model, specialized in cybersecurity and long-horizon tasks. Both represent cutting-edge AI, but access policies differ: Anthropic restricts Fable due to compute constraints, while OpenAI removes limits to attract users.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://openai.com/index/previewing-gpt-5-6-sol/">Previewing GPT - 5 . 6 Sol : a next-generation model | OpenAI</a></li>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Anthropic`, `#Claude Fable 5`, `#GPT-5.6`, `#model access`

---

<a id="item-7"></a>
## [Zer0Fit: MCP Server for Google's TabFM & TimesFM](https://www.reddit.com/r/MachineLearning/comments/1uue8cc/zer0fit_i_took_googles_new_tabfm_timesfm_ml/) ⭐️ 6.0/10

A grad student released Zer0Fit, an MCP server wrapping Google's TabFM (tabular foundation model) and TimesFM (time series foundation model) into a single Docker container, enabling zero-shot machine learning tasks via local LLMs. The project supports CSV input and was tested on classic datasets like Iris and California Housing, achieving 94.7% accuracy and R² of 0.91. Zer0Fit lowers the barrier for non-experts to perform ML tasks like classification, regression, and forecasting without manual model training or tuning. By integrating Google's foundation models via MCP, it bridges the gap between traditional ML and generative AI within chat interfaces like Open WebUI. The server runs on CUDA only, requires at least 16GB VRAM, and dynamically loads/unloads models with a 5-minute TTL to free memory. It currently supports CSV files, with plans for XLS, XLSX, JSON, and JSONL. No Mac support due to PyTorch dependency.

reddit · r/MachineLearning · /u/Porespellar · Jul 12, 12:32

**Background**: TabFM and TimesFM are zero-shot foundation models from Google Research for tabular data and time series forecasting, respectively. They are pre-trained on large-scale synthetic data and can perform tasks without task-specific fine-tuning. The Model Context Protocol (MCP), introduced by Anthropic, is an open standard that allows LLMs to connect with external tools and data sources, enabling seamless integration.

<details><summary>References</summary>
<ul>
<li><a href="https://research.google/blog/introducing-tabfm-a-zero-shot-foundation-model-for-tabular-data/">Introducing TabFM : A zero-shot foundation model for tabular data</a></li>
<li><a href="https://github.com/google-research/timesfm">GitHub - google -research/ timesfm : TimesFM ( Time Series...)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#MCP`, `#TabFM`, `#TimesFM`, `#zero-shot`, `#foundation models`

---

<a id="item-8"></a>
## [Context-Based View of Neural Networks as Linear Mappings](https://www.reddit.com/r/MachineLearning/comments/1uu2p63/context_and_average_best_linear_mappings_d/) ⭐️ 6.0/10

The author proposes a new perspective on neural networks that interprets each layer as an average best linear mapping conditioned on the input context, supported by a detailed document on Archive.org. This theoretical reframing could simplify the understanding of how neural networks process information, potentially leading to more interpretable models and new architectural insights. The perspective treats each layer's output as a linear combination of input features weighted by context-dependent coefficients, averaged over possible contexts. The concept is explained in a publicly available document on Archive.org.

reddit · r/MachineLearning · /u/oatmealcraving · Jul 12, 02:18

**Background**: In mathematics, a linear map is a function between vector spaces that preserves vector addition and scalar multiplication. Neural networks typically use nonlinear activation functions, but representing layers as linear mappings under certain contexts can simplify analysis. This work builds on the idea of context-dependent processing in neural networks, which has been studied in areas like continual learning and explainable AI.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Linear_map">Linear map - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#neural networks`, `#linear mappings`, `#context`

---

<a id="item-9"></a>
## [ACL conference acceptance process under ARR](https://www.reddit.com/r/MachineLearning/comments/1ut5krb/how_does_acl_conferences_acceptance_work_d/) ⭐️ 6.0/10

A researcher asks how *ACL conferences decide paper acceptance given ARR reviews and meta-reviews, noting that scores do not always match outcomes. The community explains that conferences consider all reviews, meta-reviews, and track submissions, using a tiered decision system (Main, Findings, Reject). This discussion clarifies the often opaque acceptance process for NLP researchers, reducing confusion and setting realistic expectations. It also highlights the role of the Findings track as a middle ground for borderline papers. Acceptance decisions are not solely based on the overall score; conferences evaluate the full set of reviews, the meta-review, and the paper's track. The ranking from Accept-Main down to Reject is used, and Findings papers are treated like main papers but without oral presentation.

reddit · r/MachineLearning · /u/Happy_Today_3288 · Jul 11, 00:47

**Background**: ACL Rolling Review (ARR) is a centralized review platform for computational linguistics conferences. After receiving reviews and a meta-review from an action editor, papers are forwarded to a specific conference for the final decision. The conference program committee sees all reviews and the meta-review, and uses a tiered outcome system (main, findings, reject). Findings papers are published in the ACL Anthology but not presented orally. This system aims to streamline reviewing across multiple venues.

<details><summary>References</summary>
<ul>
<li><a href="https://aclrollingreview.org/">ACL Rolling Review – A peer review platform for the Association for...</a></li>
<li><a href="https://gist.github.com/antonisa/2158dee79179c7c49304ef353887bfa0">Conference Decisions · GitHub</a></li>
<li><a href="https://kinit.sk/quality-of-acl-findings-analysis-of-citations/">Quality of ACL “Findings”: analysis of citations - KInIT</a></li>

</ul>
</details>

**Tags**: `#ACL`, `#conference acceptance`, `#NLP`, `#paper review`, `#meta-review`

---