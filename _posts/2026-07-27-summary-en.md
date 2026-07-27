---
layout: default
title: "Horizon Summary: 2026-07-27 (EN)"
date: 2026-07-27
lang: en
---

> From 22 items, 14 important content pieces were selected

---

1. [Anthropic Advocates Mandatory Safety Testing for Open-Weights Models](#item-1) ⭐️ 8.0/10
2. [Judge Rejects Google's DMCA Claim Against Scraping](#item-2) ⭐️ 8.0/10
3. [Hack of Volvo/Eicher Fleet Platform Exposes Critical Vulnerabilities](#item-3) ⭐️ 8.0/10
4. [Paged Out #9: Free Technical Zine Released](#item-4) ⭐️ 8.0/10
5. [Inside the Relay Market for LLM Token Reselling and Fraud](#item-5) ⭐️ 8.0/10
6. [Frontier LLMs Show Consistent Left-Leaning Bias in New Benchmarking Study](#item-6) ⭐️ 8.0/10
7. [YOLO26n Inference from Scratch Using ARM64 Assembly](#item-7) ⭐️ 8.0/10
8. [Open-weight 4B models approach o3 in Swedish medical QA](#item-8) ⭐️ 8.0/10
9. [Misago ditches React for Htmx, gains simplicity and speed](#item-9) ⭐️ 7.0/10
10. [Proposal for a Reproducible Pre-Training Data Quality Gate](#item-10) ⭐️ 7.0/10
11. [LLM Comparison on IMO 2026 Problems Shows Harness Impact](#item-11) ⭐️ 7.0/10
12. [Ethan Mollick's AI Guide Shifts from Chat to Agentic Systems](#item-12) ⭐️ 6.0/10
13. [Transformer from Scratch in PyTorch for English-Tamil Translation](#item-13) ⭐️ 6.0/10
14. [Linking Figures in NeurIPS Rebuttal: Risks and Advice](#item-14) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Anthropic Advocates Mandatory Safety Testing for Open-Weights Models](https://www.anthropic.com/news/position-open-weights-models) ⭐️ 8.0/10

Anthropic released a policy statement clarifying that they support open-weights models but believe all sufficiently capable models, including open-weights ones, should undergo mandatory safety testing before release. This position could shape future AI regulation by advocating for mandatory testing that applies equally to open and closed models, potentially impacting the open-source AI community and model release practices. Anthropic has never advocated for a ban on open-weights models, but calls for safety testing that could be logistically or financially burdensome, raising concerns about de facto restrictions.

hackernews · surprisetalk · Jul 27, 22:03 · [Discussion](https://news.ycombinator.com/item?id=49076057)

**Background**: Open-weights models are AI models whose core components are publicly released, allowing anyone to download, inspect, modify, and run them. Critics argue that mandatory safety testing could be used to restrict access, similar to past regulatory barriers. Anthropic is a leading AI company focused on safety.

<details><summary>References</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://www.microsoft.com/en-us/corporate-responsibility/topics/open-weight/">Open Weights and American AI Leadership</a></li>

</ul>
</details>

**Discussion**: Commenters were skeptical, with some arguing that mandatory testing is effectively a ban by cost or approval. Others pointed out contradictions in Anthropic's stance on chip bans to China. The overall sentiment was critical of the policy as potentially self-serving.

**Tags**: `#AI safety`, `#open-weights`, `#regulation`, `#Anthropic`, `#AI policy`

---

<a id="item-2"></a>
## [Judge Rejects Google's DMCA Claim Against Scraping](https://www.techdirt.com/2026/07/27/judge-rejects-googles-attempt-to-dmca-its-way-out-of-being-scraped/) ⭐️ 8.0/10

A judge rejected Google's attempt to use the DMCA's anti-circumvention clause to stop SerpAPI from scraping its search results. The ruling found that Google's bot detection measures are not protected under DMCA because the scraping targeted unoriginal factual data. This decision protects web scraping as a legitimate practice and prevents companies from using copyright law to block competition. It affirms that raw factual data from search results is not copyrightable, which has implications for the open web and API access. The case originated from Reddit's separate lawsuit against SerpAPI and Perplexity. The DMCA claim requires a nexus to copyright infringement, which the judge found lacking because search results are compiled facts with minimal creative selection.

hackernews · cdrnsf · Jul 27, 18:15 · [Discussion](https://news.ycombinator.com/item?id=49073513)

**Background**: The DMCA's Section 1201 prohibits circumvention of technological measures that protect copyrighted works. Courts have split on whether bot detection measures qualify, with some requiring a connection to actual infringement. Google previously deprecated its search API, leading third parties to fill the gap via scraping.

<details><summary>References</summary>
<ul>
<li><a href="https://www.techdirt.com/2026/07/27/judge-rejects-googles-attempt-to-dmca-its-way-out-of-being-scraped/">Judge Rejects Google’s Attempt To DMCA Its Way Out Of Being Scraped | Techdirt</a></li>
<li><a href="https://capstonedc.com/insights/why-dmca-claims-against-web-scrapers-face-long-odds/">Why DMCA Claims Against Web Scrapers Face Long Odds - Capstone DC</a></li>

</ul>
</details>

**Discussion**: Commenters highlighted the irony of Google, built on crawling, now fighting scraping. Many criticized Google for removing its API and then suing those who filled the void. Others noted the importance of scraping for exposing scams in search ads.

**Tags**: `#web scraping`, `#copyright`, `#Google`, `#DMCA`, `#legal`

---

<a id="item-3"></a>
## [Hack of Volvo/Eicher Fleet Platform Exposes Critical Vulnerabilities](https://eaton-works.com/2026/07/27/my-eicher-hack/) ⭐️ 8.0/10

Security researcher disclosed critical vulnerabilities in Volvo/Eicher's My Eicher fleet management platform, allowing takeover of all users and vehicles, after responsible disclosure. This highlights the serious risks of cloud-dependent vehicle systems, where a single platform compromise could affect thousands of commercial vehicles, potentially endangering driver safety and fleet operations. The researcher reported the vulnerability on November 3, 2025, and Volvo/Eicher fixed it by November 20, 2025, but the researcher published details on July 27, 2026, after a lengthy delay. The specific technical details of the exploit are not fully disclosed in the summary.

hackernews · EatonZ · Jul 27, 15:08 · [Discussion](https://news.ycombinator.com/item?id=49070756)

**Background**: Volvo Eicher Commercial Vehicles (VECV) is a joint venture between Volvo Group and Eicher Motors, providing fleet management solutions like My Eicher for Indian commercial vehicles. Fleet telematics systems connect vehicles to cloud services for tracking and control, but security weaknesses can allow remote attacks that affect vehicle operations.

<details><summary>References</summary>
<ul>
<li><a href="https://eaton-works.com/2026/07/27/my-eicher-hack/">Exploiting Volvo/Eicher’s fleet management platform to gain control over all users and vehicles</a></li>
<li><a href="https://en.wikipedia.org/wiki/Eicher_Motors">Eicher Motors - Wikipedia</a></li>
<li><a href="https://www.ndtvprofit.com/business/vecv-forms-joint-venture-with-itriangle-infotech-for-fleet-management-solutions">VECV Forms Joint Venture With iTriangle Infotech For Fleet Management Solutions</a></li>

</ul>
</details>

**Discussion**: Community comments express concern about the slow response from the vendor and the broader implications of cloud-dependent car security. Some users mock the situation with sarcasm, while others advocate for car right-to-repair and local pairing mechanisms.

**Tags**: `#security`, `#vulnerability disclosure`, `#fleet management`, `#responsible disclosure`

---

<a id="item-4"></a>
## [Paged Out #9: Free Technical Zine Released](https://pagedout.institute/download/PagedOut_009.pdf) ⭐️ 8.0/10

Paged Out #9, a free community-driven technical zine, has been released as a PDF, featuring a collection of one-page articles on programming, hacking, systems, and computer science topics. Paged Out continues the tradition of deeply technical, hacker-curious zines like 2600 and Phrack, providing a modern platform for sharing low-level knowledge. Its free and accessible format encourages exploration of niche topics rarely covered in mainstream tech media. The zine includes articles such as 'Baby Steps in C,' 'The Subpixel Zoo,' and an uncredited rediscovery of Wang's computable tilings from the 1960s. Commenters noted its high-quality design and compared it to Phrack's textfiles with raster art advertising.

hackernews · laurensr · Jul 27, 14:22 · [Discussion](https://news.ycombinator.com/item?id=49070138)

**Background**: Paged Out is a free, one-article-per-page zine started by the Dragon Sector CTF team and friends. It covers a wide range of technical topics from programming to hardware hacking, aiming to bring back the spirit of old-school hacker zines. Each issue is published as a printable PDF.

<details><summary>References</summary>
<ul>
<li><a href="https://gynvael.coldwind.pl/?id=787">Wyszedł Paged Out ! #4 - gynvael.coldwind//vx.log</a></li>
<li><a href="https://micro.edrperez.com/?searchtags=paged_out">Search: [ paged _ out ] - Micro blog</a></li>

</ul>
</details>

**Discussion**: Commenters praised the zine as 'a modern 2600' and 'deeply technical, scattered topics and depth, all very hacker-curious.' One user highlighted the computiles piece as an uncredited rediscovery of Wang's work linking tilings to the halting problem, adding technical depth appreciated by the community.

**Tags**: `#programming`, `#hacking`, `#systems`, `#technical zine`, `#CS research`

---

<a id="item-5"></a>
## [Inside the Relay Market for LLM Token Reselling and Fraud](https://simonwillison.net/2026/Jul/26/relay-market/#atom-everything) ⭐️ 8.0/10

Matt Lenhard's investigation reveals a market where Chinese resellers offer discounted LLM API access by pooling stolen credentials, abusing free trials, and using open-source proxy tools like one-api and new-api. This fraud ecosystem undermines API security and the economics of AI services, exposing vulnerabilities that could lead to significant financial losses for LLM providers and increased costs for legitimate users. The resellers use open-source API proxy software to load-balance requests across pooled API keys, and buyers seek cheap tokens, avoid geo-restrictions, or collect data for model distillation.

rss · Simon Willison · Jul 26, 19:30

**Background**: LLM APIs are typically accessed via API keys that bill per token. Resellers exploit this by aggregating unauthorized keys—from stolen credentials, free trial abuse, or chargeback fraud—and routing traffic through proxy services to offer discounted rates. This gray market is especially prevalent in China.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jul/26/relay-market/">An Inside Look at the Relay Market Powering Token Resellers and Fraud</a></li>
<li><a href="https://socradar.io/blog/dark-token-llm-api-proxies-harvest-fraud/">Dark Token Economy: Unauthorized LLM API Proxies Harvest Prompts for Fraud and Distillation</a></li>
<li><a href="https://www.deeplearning.ai/the-batch/inside-the-gray-market-for-llm-access">Middlemen Package Extra Tokens, Hijack IDs to Resell, Distill Models</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#API security`, `#fraud`, `#token reselling`, `#AI infrastructure`

---

<a id="item-6"></a>
## [Frontier LLMs Show Consistent Left-Leaning Bias in New Benchmarking Study](https://www.reddit.com/r/MachineLearning/comments/1v8fnzw/evaluated_6_frontier_llms_gpt54_claude_sonnet_46/) ⭐️ 8.0/10

A solo evaluation of six frontier LLMs—GPT-5.4, Claude Sonnet 4.6, Claude Opus 4.7, Gemini Pro/Flash, and Grok 4.3—across 8 bias benchmarks reveals that all models exhibit left-leaning political bias, despite Grok self-reporting as right-leaning. The study also finds varying refusal rates on race-related questions, with GPT-5.4 refusing 20.3% of the time. This systematic comparison provides valuable transparency into the political and social biases embedded in leading AI systems, which is critical for developers and policymakers who rely on these models for content moderation, hiring, and other fairness-sensitive applications. The findings highlight a persistent discrepancy between self-reported and actual model behavior, raising questions about model alignment and honesty. The evaluation used 8 established benchmarks including WinoBias, BBQ, SeeGULL, OpinionsQA, cajcodes Political Bias, Hyperpartisan News, and Political Compass, totaling about 20,600 examples. GPT-5.4 showed the highest refusal rate on race-related questions at 20.3%, while Claude Sonnet 4.6 and Gemini Pro refused only ~5% of the time.

reddit · r/MachineLearning · /u/marggggggggg · Jul 27, 22:37

**Background**: Bias benchmarks like WinoBias measure gender bias in coreference resolution, BBQ evaluates social biases in question answering, and SeeGULL captures stereotypes across global cultures. These datasets are designed to detect whether language models exhibit harmful biases against protected groups. The models tested, such as GPT-5.4 and Claude Opus 4.7, represent the latest frontier in large language model development, and their behavior on such benchmarks is a key indicator of alignment with fairness principles.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/winobias">WinoBias : Gender Bias in Coreference Benchmark</a></li>
<li><a href="https://arxiv.org/abs/2110.08193">BBQ : A Hand-Built Bias Benchmark for Question Answering</a></li>
<li><a href="https://github.com/google-research-datasets/seegull">GitHub - google-research-datasets/seegull: SeeGULL is a broad ...</a></li>

</ul>
</details>

**Tags**: `#LLM bias`, `#fairness evaluation`, `#political bias`, `#model benchmarking`, `#AI ethics`

---

<a id="item-7"></a>
## [YOLO26n Inference from Scratch Using ARM64 Assembly](https://www.reddit.com/r/MachineLearning/comments/1v6w394/i_implemented_the_yolo26n_model_inference_from/) ⭐️ 8.0/10

A developer implemented YOLO26n model inference entirely from scratch using ARM64 Assembly Language and C, without any existing deep learning frameworks, and integrated multiple low-level optimizations including NEON SIMD, Winograd convolution, and operator fusion on a Raspberry Pi 4. This project demonstrates how extreme low-level optimization can enable efficient edge AI on resource-constrained devices, providing valuable insights for deploying computer vision models without relying on heavy frameworks. The implementation includes custom ARM64 micro-kernels, cache-aware tiling, and a custom binary format for model parameters, but the performance gain was lower than expected, suggesting room for further optimization. The YOLO26n model used includes components like Conv, C3K2, SPPF, C2PSA, and Detect.

reddit · r/MachineLearning · /u/Forward_Confusion902 · Jul 26, 06:43

**Background**: YOLO (You Only Look Once) is a popular family of real-time object detection models. Winograd convolution is a fast algorithm that reduces the number of multiplications in convolution operations by applying linear transformations, as explained in the research paper by Lavin and Gray. Operator fusion combines multiple neural network operations into a single kernel to reduce memory traffic. ARM NEON SIMD instructions enable parallel data processing on ARM processors, critical for accelerating neural networks on edge devices like the Raspberry Pi.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2201.10369">[2201.10369] Winograd Convolution for Deep Neural Networks ... Winograd's Convolution Theorem [Explained] - OpenGenus IQ Winograd Convolution for Deep Neural Networks: Efficient ... Chapter 8: Fast Convolution - College of Science and Engineering The Winograd Convolution Method - DiVA Winograd Convolution: A Perspective from Fault Tolerance Winograd Convolution for Deep Neural Networks: Efficient ...</a></li>
<li><a href="https://arxiv.org/abs/2108.13342">[2108.13342] DNNFusion: Accelerating Deep Neural Networks ... Operator Fusion Explained: Definition, Examples & Use Cases ... Optimus: An Operator Fusion Framework for Deep Neural ... Using fused operators to improve performance | Microsoft Learn [2501.00636] Applying Graph Explanation to Operator Fusion Operator Fusion: Vertical and Horizontal - apxml.com Apollo: Automatic Partition-based Operator Fusion through ...</a></li>
<li><a href="https://medium.com/@noel.benji/inside-yolo-what-are-c3k2-c2f-c3k-blocks-806ae4cd486f">Optimizing YOLO: C3K2, C2F & C3K for Faster Object Detection | Medium</a></li>

</ul>
</details>

**Tags**: `#YOLO`, `#ARM64`, `#edge AI`, `#computer vision`, `#optimization`

---

<a id="item-8"></a>
## [Open-weight 4B models approach o3 in Swedish medical QA](https://www.reddit.com/r/MachineLearning/comments/1v71wds/openweight_4b_models_approach_o3level_medical/) ⭐️ 8.0/10

A researcher found that Qwen3.5-4B, with reasoning enabled, achieves 87% accuracy on Swedish medical exam questions (MedQA-SWE), closely matching o3's 88% performance without fine-tuning. This demonstrates that small open-weight models (4B parameters) can rival much larger proprietary systems on specialized tasks, lowering the barrier for domain-specific AI deployment in languages with limited training data. The models use an early-exit reasoning technique from the S-GRPO paper to prevent infinite loops, and Qwen3.5-4B performs reasoning in English despite Swedish prompts, showing language is not a barrier.

reddit · r/MachineLearning · /u/AccomplishedCat4770 · Jul 26, 11:58

**Background**: MedQA-SWE is a multiple-choice clinical Q&A dataset in Swedish with 3,180 questions from national licensing exams. Small language models (4B parameters) are efficient but often lag behind large models on complex reasoning; this work shows that with reasoning techniques they can close the gap.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/datasets/nicher92/medqa-swe">nicher92/ medqa - swe · Datasets at Hugging Face</a></li>
<li><a href="https://arxiv.org/abs/2505.07686">[2505.07686] S-GRPO: Early Exit via Reinforcement Learning in ... S-GRPO: Early Exit via Reinforcement Learning in Reasoning Models S-GRPO: Early Exit via Reinforcement Learning in Reasoning Models S-GRPO: Early Exit via Reinforcement Learning in Reasoning Models (PDF) S-GRPO: Early Exit via Reinforcement Learning in ... [PDF] S-GRPO: Early Exit via Reinforcement Learning in ... S-GRPO: Early Exit via Reinforcement Learning in Reasoning ...</a></li>
<li><a href="https://aclanthology.org/2024.lrec-main.975.pdf">MedQA - SWE - a Clinical Question & Answer Dataset for Swedish</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#medical QA`, `#small language models`, `#reasoning`, `#model comparison`

---

<a id="item-9"></a>
## [Misago ditches React for Htmx, gains simplicity and speed](https://misago-project.org/t/removing-reactjs-from-the-codebase-and-adapting-htmx-for-ui-interactivity/1267/) ⭐️ 7.0/10

The Misago project removed React.js from its codebase and adopted Htmx for UI interactivity, achieving a simpler, faster server-rendered application. This migration reflects a growing trend toward simpler, hypermedia-driven architectures over heavy client-side frameworks, especially for content-heavy applications like forums. Htmx allows dynamic UI updates via custom HTML attributes, eliminating the need for extensive JavaScript, while forums primarily deliver non-interactive content that benefits from partial rendering and Server-Sent Events.

hackernews · Ralfp · Jul 27, 09:58 · [Discussion](https://news.ycombinator.com/item?id=49067301)

**Background**: Htmx is an open-source JavaScript library that extends HTML with AJAX, CSS transitions, WebSockets, and Server-Sent Events via attributes, enabling a hypermedia-driven approach. React is a popular JavaScript library for building interactive user interfaces but adds complexity for server-rendered sites. Many developers now advocate for simpler alternatives like Htmx when full client-side interactivity is unnecessary.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Htmx">Htmx</a></li>
<li><a href="https://htmx.org/">htmx - high power tools for html</a></li>

</ul>
</details>

**Discussion**: Community members generally praised the move, noting Htmx's suitability for forum software and server-rendered apps. Some shared their own positive experiences using Htmx with tools like DaisyUI and TailwindCSS, while others recommended alternatives like Pyview for similar server-side DOM patching.

**Tags**: `#htmx`, `#react`, `#web development`, `#server-side rendering`, `#javascript`

---

<a id="item-10"></a>
## [Proposal for a Reproducible Pre-Training Data Quality Gate](https://www.reddit.com/r/MachineLearning/comments/1v8a3nu/training_data_needs_a_real_gonogo_gate_before/) ⭐️ 7.0/10

The user proposes a local, reproducible system that audits training data artifacts and issues a verdict (PASS, WARNING, FAIL, FAIL_SECURITY) based on explicit checks for leakage, redundancy, coverage, provenance, and evidence integrity before training is allowed to proceed. This proposal fills a gap in ML pipelines where data quality gates are often ad hoc, potentially preventing costly training runs on flawed data and improving reproducibility and trust in model development. The system would not rely on LLMs for verdicts but on hard gates and explicit evidence, and could produce a repair plan, apply only approved changes to a derived copy, preserve the original, and run a second audit afterward—all tied to manifests and checksums.

reddit · r/MachineLearning · /u/jesusmjk · Jul 27, 19:13

**Background**: Data leakage in machine learning occurs when training data contains information that would not be available at prediction time, leading to overly optimistic performance estimates. Provenance tracks the origins and transformations of data, essential for reproducibility. Redundancy detection identifies duplicate or near-duplicate samples that can bias training. These concepts are central to the proposed pre-training gate, which aims to audit these and other quality dimensions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Leakage_(machine_learning)">Leakage (machine learning) - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/data-leakage-machine-learning">What is Data Leakage in Machine Learning? | IBM</a></li>
<li><a href="https://arxiv.org/abs/2507.01075">Provenance Tracking in Large-Scale Machine Learning Systems Provenance Tracking for Machine Learning Models: A ... Decoding the Role of Data Provenance in Enhancing Machine ... Provenance Tracking in Large-Scale Machine Learning Systems Versioning, Provenance, and Reproducibility - Machine ...</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#data quality`, `#training data`, `#MLOps`, `#data validation`

---

<a id="item-11"></a>
## [LLM Comparison on IMO 2026 Problems Shows Harness Impact](https://www.reddit.com/r/MachineLearning/comments/1v6wskz/we_compared_different_llms_on_imo_2026_r/) ⭐️ 7.0/10

A Reddit post presents a benchmark using novel IMO 2026 problems to compare LLMs, finding that frontier models achieved near-perfect scores regardless of harness, while weaker models like Sonnet and Opus improved significantly with the AutoFyn multi-agent harness. This benchmark demonstrates that multi-agent harnesses can substantially boost the mathematical reasoning of weaker models, but cannot yet match frontier models, highlighting the current gap in LLM intelligence and the value of orchestration techniques. The problems were graded by both a frontier model and manual verification by former IMO medalists; hallucination issues persisted, as seen when Sonnet falsely claimed a solution on problem P3, and no sub-frontier model solved the hardest problem's key insight even after 20 hours of automated reasoning.

reddit · r/MachineLearning · /u/pequalnp92 · Jul 26, 07:21

**Background**: The International Mathematical Olympiad (IMO) is a prestigious competition with novel problems, making it a strong benchmark for evaluating LLM reasoning because the problems are not in training data. An agent harness is a system that orchestrates model calls, tool use, and context management to improve performance. Frontier models like those from OpenAI and Anthropic currently lead such benchmarks, while open-weight models like GLM-5.2 offer competitive performance but require more optimization.

<details><summary>References</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/agent-framework/agents/harness">Agent Harnesses | Microsoft Learn</a></li>
<li><a href="https://explore.n1n.ai/blog/run-glm-5-2-locally-open-weights-guide-2026-06-15">Run GLM-5.2 Locally: A Complete Guide to the Open Weights ...</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#benchmark`, `#mathematical reasoning`, `#multi-agent systems`, `#evaluation`

---

<a id="item-12"></a>
## [Ethan Mollick's AI Guide Shifts from Chat to Agentic Systems](https://simonwillison.net/2026/Jul/27/an-opinionated-guide-to-which-ai-to-use-to-do-stuff/#atom-everything) ⭐️ 6.0/10

Ethan Mollick's guide to AI tools has evolved to prioritize agentic systems over conversational chatbots, highlighting ChatGPT Work, Claude Cowork, and Codex as key modes for autonomous task execution. This reflects the broader industry shift from passive chatbots to autonomous agents that can perform hours of human work, changing how professionals choose and deploy AI tools for productivity. The guide notes that Gemini has fallen off the list because Google lacks an established entry in the Codex/ChatGPT Work/Cowork category, and Ethan explains that the most powerful way to use AI is by giving it access to your computer via desktop apps.

rss · Simon Willison · Jul 27, 21:55

**Background**: Agentic AI systems are autonomous AI that can perceive, reason, and act to achieve user-set goals without constant human input, unlike traditional chatbots. Ethan Mollick, a professor and AI researcher, has been updating his practical guide to help people choose the right AI tool for various tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/agentic-ai-agents-stop-doing-boring-tasks-solves-your-mohammad-anis-cyqyf">Agentic AI Agents: Stop Doing Boring Tasks Solves Your Daily Grind</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gemini_Spark">Gemini Spark</a></li>
<li><a href="https://blog.google/innovation-and-ai/products/gemini-app/next-evolution-gemini-app/">The Gemini app becomes more agentic, delivering proactive, 24/7 help</a></li>

</ul>
</details>

**Tags**: `#AI`, `#guide`, `#agents`, `#LLMs`, `#productivity`

---

<a id="item-13"></a>
## [Transformer from Scratch in PyTorch for English-Tamil Translation](https://www.reddit.com/r/MachineLearning/comments/1v86qo9/built_trained_a_transformer_from_scratch_in_pure/) ⭐️ 6.0/10

A developer published a comprehensive tutorial that implements and trains the full Transformer architecture from scratch using pure PyTorch, applied to English-to-Tamil machine translation on a Hugging Face dataset. This educational resource helps practitioners understand the inner workings of Transformer models through detailed math and code, especially for low-resource language pairs like English-Tamil. The model was trained on dual NVIDIA T4 GPUs using the gopi30/english-tamil dataset, and the tutorial covers every equation, tensor shape transformation, and PyTorch block.

reddit · r/MachineLearning · /u/imrancoder · Jul 27, 17:17

**Background**: The Transformer architecture, introduced in the paper 'Attention Is All You Need,' relies on self-attention mechanisms to process sequences. It has become the foundation of modern NLP models like BERT and GPT. Building one from scratch is a popular learning exercise for understanding deep learning for NLP.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/SirawitC/Transformer_from_scratch_pytorch">GitHub - SirawitC/Transformer_from_scratch_pytorch: Build a ...</a></li>
<li><a href="https://www.datacamp.com/tutorial/building-a-transformer-with-py-torch">Transformer Model Tutorial in PyTorch: From Theory to Code</a></li>

</ul>
</details>

**Tags**: `#Transformer`, `#PyTorch`, `#Machine Translation`, `#NLP`, `#Tutorial`

---

<a id="item-14"></a>
## [Linking Figures in NeurIPS Rebuttal: Risks and Advice](https://www.reddit.com/r/MachineLearning/comments/1v6qt8l/link_plotsfigures_in_neurips_rebuttal_r/) ⭐️ 6.0/10

A researcher asks whether linking to figures in a NeurIPS rebuttal is permissible and safe, given that official guidelines technically prohibit external links. This question affects many authors who want to present additional experimental results clearly during the rebuttal period, where effective communication can influence acceptance decisions. The official NeurIPS author rebuttal website states that links are not allowed, but some authors consider linking as a practical workaround to embed plots that are more digestible than tables.

reddit · r/MachineLearning · /u/confirm-jannati · Jul 26, 02:12

**Background**: NeurIPS is a top machine learning conference that uses OpenReview for peer review. During the rebuttal phase, authors can respond to reviewer comments and provide additional experiments. The official policy prohibits external links to avoid bypassing the review system.

<details><summary>References</summary>
<ul>
<li><a href="https://conferenceinc.net/post/neurips-2025-call-for-papers/">NeurIPS 2025 Author Rebuttal Period Kicks Off... - Conference Inc.</a></li>
<li><a href="https://openreview.net/about">About OpenReview</a></li>

</ul>
</details>

**Tags**: `#NeurIPS`, `#rebuttal`, `#conference`, `#plots`, `#research`

---