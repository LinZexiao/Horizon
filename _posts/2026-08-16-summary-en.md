---
layout: default
title: "Horizon Summary: 2026-08-16 (EN)"
date: 2026-08-16
lang: en
---

> From 28 items, 14 important content pieces were selected

---

1. [Anthropic publishes Claude system prompts, sparking community analysis](#item-1) ⭐️ 9.0/10
2. [Qwen 3.8 27B Is Excellent but Defaults to Overthinking](#item-2) ⭐️ 8.0/10
3. [SSOG-Attention: A Sub-Quadratic Alternative to Standard Attention](#item-3) ⭐️ 8.0/10
4. [BDH-CQ: Recurrent Latent Reasoning Achieves Cost-Effective ARC-AGI-1 Results](#item-4) ⭐️ 8.0/10
5. [The Gray Market for Unused AI API Credits Grows](#item-5) ⭐️ 7.0/10
6. [Firefox for iOS Adds Native Ad Blocker](#item-6) ⭐️ 7.0/10
7. [Amodei: AI's Negative Reputation Is a Crisis of Trust, Not Messaging](#item-7) ⭐️ 7.0/10
8. [Linear Attention Struggles with Long-Range Recall in DNA Models](#item-8) ⭐️ 7.0/10
9. [Critique Challenges Efficient Channel Attention Paper's Core Hypothesis](#item-9) ⭐️ 7.0/10
10. [Survival of the Fitted: Qwen3.6-27B’s Jacobian lens reads and steers Qwen3.8-27B with zero refitting (R)](#item-10) ⭐️ 7.0/10
11. [Developing-World Engineer Defends RISC-V as Low-Cost Embedded Option](#item-11) ⭐️ 6.0/10
12. [Models Getting Dumber on Purpose: The Shift to Tools and Retrieval](#item-12) ⭐️ 6.0/10
13. [CORS Chat: Browser Tool for Testing OpenAI-Compatible Endpoints](#item-13) ⭐️ 6.0/10
14. [200 Post-Training Steps Flip Qwen2.5-7B-Instruct to Claim Sentience](#item-14) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Anthropic publishes Claude system prompts, sparking community analysis](https://platform.claude.com/docs/en/release-notes/system-prompts) ⭐️ 9.0/10

Anthropic published the system prompts used by its Claude models (e.g., Opus 4.8, Claude Fable 5, and Claude Mythos 5) in its platform documentation, marking a rare transparency move. The release includes detailed instructions on how Claude should handle images, user wellbeing, and other behaviors. System prompts are a key tool for steering LLM behavior, and seeing them in the open helps researchers and engineers understand how Claude is shaped and audited. The release drew high community engagement (478 points, 209 comments), highlighting the growing importance of transparency in frontier AI. The published prompts include instructions such as not assuming an image is present just because the prompt implies it, and prioritizing a user's wellbeing over task completion in crisis situations. Developer Simon Willison also created a git commit history of the prompts to track changes between versions like Opus 4.8 and Opus 5.

hackernews · tosh · Aug 16, 12:48 · [Discussion](https://news.ycombinator.com/item?id=49319556)

**Background**: System prompts are predefined directives given to an LLM before a conversation, telling it who it is, what its role is, and how to behave. They take precedence over user inputs and are widely used by deployers to ensure consistent responses. Anthropic's decision to publish these prompts is notable because most AI labs keep such internal system prompts secret, so the release offers rare insight into how a frontier model is instructed.

<details><summary>References</summary>
<ul>
<li><a href="https://promptengineering.org/system-prompts-in-large-language-models/">System Prompts in Large Language Models</a></li>
<li><a href="https://arxiv.org/abs/2505.21091v3">[2505.21091v3] Position is Power: System Prompts as a Mechanism...</a></li>

</ul>
</details>

**Discussion**: Community sentiment is generally positive but mixed. Simon Willison shared a git-based diff tool to track prompt changes; other users discussed the implications of prompts that encode 'common sense' like image checks, and one commenter raised concerns about moderation of AI-related stories on the forum. Some see the prompts as a roadmap for Anthropic's model behavior priorities.

**Tags**: `#AI`, `#Claude`, `#system prompts`, `#transparency`, `#LLM`

---

<a id="item-2"></a>
## [Qwen 3.8 27B Is Excellent but Defaults to Overthinking](https://simonwillison.net/2026/Aug/16/qwen-38-27b/) ⭐️ 8.0/10

Alibaba's Qwen lab released Qwen 3.8 27B, an Apache-2.0 licensed 27B-parameter vision-language model with self-reported benchmarks that surpass both Qwen 3.6 27B and the closed-weight Qwen 3.7-Plus. Simon Willison's hands-on tests found that the model defaults to xhigh reasoning effort, causing spectacular overthinking and extremely slow output. This release matters because 27B is a practical size for running capable open-weight models on local hardware, potentially bringing strong benchmark performance to consumer laptops and edge devices. However, the default xhigh reasoning effort can make the model impractically slow unless users explicitly lower the reasoning level, which affects real-world deployment choices. Willison ran the 17GB Q4_K_M quantized build in LM Studio on a 128GB M5 Max MacBook Pro and an NVIDIA DGX Spark, and needed to raise the context from LM Studio's default 8,192 tokens to the full 262,144 to avoid exhausting the window. An SVG request for a pelican riding a bicycle took 21 minutes, using 22,276 reasoning tokens to produce 3,223 output tokens.

rss · Simon Willison · Aug 16, 22:00

**Background**: Qwen is Alibaba's open-weight LLM family, and the 3.8 27B is a vision-language model released under the permissive Apache 2.0 license. The model supports a reasoning_effort parameter that controls chain-of-thought depth, with xhigh set as the default; this leads to extensive internal deliberation even for simple prompts. Its predecessor, Qwen 3.6 27B, was already noted for strong local performance, and the new model adds vision capabilities and improved benchmarks.

**Tags**: `#LLM`, `#Qwen`, `#open-source`, `#AI`, `#model-release`

---

<a id="item-3"></a>
## [SSOG-Attention: A Sub-Quadratic Alternative to Standard Attention](https://www.reddit.com/r/MachineLearning/comments/1vpt6ay/ssogattention_sum_of_separable_gaussians_as_a/) ⭐️ 8.0/10

The post introduces SSOG-Attention, a novel attention mechanism that models attention scores as a sum of separable Gaussians, reducing complexity from O(N²·d) to O(N·√N·d). Experiments show it outperforms standard scaled dot-product attention on CIFAR-100 and matches it on ImageNet with faster convergence and lower memory usage. Quadratic attention scaling is a major bottleneck for large models, so a sub-quadratic and memory-efficient alternative could enable longer sequences and cheaper training and inference. The strong empirical results on standard benchmarks suggest this approach is not just theoretical but practical. The method learns a few Gaussian atoms per head and steers them geometrically based on the query token, exploiting the separability of Gaussians for efficient factorization. The author provides a blog post and an open-source repository with additional results and ablations, noting that AI was used for some code and writing.

reddit · r/MachineLearning · /u/4rtemi5 · Aug 16, 10:06

**Background**: Scaled dot-product attention (SDPA), the core mechanism in Transformers, computes pairwise similarities between all tokens, leading to O(N²·d) complexity that becomes prohibitive for long sequences. Sub-quadratic attention methods—such as sparse attention, low-rank approximations, and kernel-based approaches—aim to reduce this cost while preserving model quality. Separable Gaussians are a mathematical tool that allows multi-dimensional functions to be decomposed into products of one-dimensional functions, enabling efficient computation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/sub-quadratic-self-attention">Sub - quadratic Self- Attention</a></li>
<li><a href="https://louiswang524.github.io/blog/ssa-subquadratic-sparse-attention/">From Quadratic to Linear: A Survey of Subquadratic Sparse Attention ...</a></li>
<li><a href="https://www.emergentmind.com/topics/closed-form-attention-kernel">Closed-Form Attention Kernel</a></li>

</ul>
</details>

**Tags**: `#attention mechanisms`, `#machine learning`, `#efficiency`, `#scalability`, `#Gaussian kernels`

---

<a id="item-4"></a>
## [BDH-CQ: Recurrent Latent Reasoning Achieves Cost-Effective ARC-AGI-1 Results](https://www.reddit.com/r/MachineLearning/comments/1vov5r5/bdhcq_incontext_learning_with_recurrent_latent/) ⭐️ 8.0/10

Researchers introduce BDH-CQ, a 150M-parameter reasoning system that combines in-context learning with recurrent latent reasoning. It achieves 29.5% pass@2 on ARC-AGI-1 at a computed cost of $0.00070 per task, reportedly breaking the cost–accuracy Pareto frontier. This result is significant because it demonstrates that latent reasoning in a high-dimensional space can be far more cost-efficient than token-based chain-of-thought methods. It could pave the way for small models to achieve strong generalization on abstract reasoning benchmarks while keeping inference costs extremely low. BDH-CQ updates its recurrent memory from demonstration inputs at inference time, then solves queries through iterative computation in latent space without verbalizing intermediate steps. The model is not trained on task identifiers or evaluation demonstration pairs, and no parameters are updated at inference time.

reddit · r/MachineLearning · /u/moschles · Aug 15, 06:18

**Background**: In-context learning lets a model adapt to a new task by conditioning on a few demonstrations, while recurrent latent reasoning extends test-time computation by unrolling an internal block rather than generating more tokens. ARC-AGI-1 is a benchmark designed to measure abstract reasoning and generalization, often used to evaluate frontier AI test-time reasoning. Prior work, such as a February 2025 paper on scaling test-time compute with latent reasoning, has explored similar recurrent depth approaches, but BDH-CQ specifically targets the combination of in-context learning and latent computation at very low cost.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2608.09888">[2608.09888] BDH-CQ: In-Context Learning with Recurrent Latent Reasoning</a></li>
<li><a href="https://huggingface.co/papers/2608.09888">Paper page - BDH - CQ : In-Context Learning with Recurrent Latent...</a></li>
<li><a href="https://arcprize.org/arc-agi/1">ARC - AGI - 1</a></li>

</ul>
</details>

**Tags**: `#In-Context Learning`, `#Recurrent Memory`, `#Latent Reasoning`, `#ARC-AGI`, `#Machine Learning`

---

<a id="item-5"></a>
## [The Gray Market for Unused AI API Credits Grows](https://vectoral.com/blog/who-are-the-token-brokers) ⭐️ 7.0/10

An emerging gray market now brokers and resells unused AI API credits, often through relay services that route API calls through accounts with subsidized balances. The analysis explores how token brokers profit from discounted access even though resale violates provider terms. This matters because it undermines AI providers' pricing and abuse controls, creating security and fraud surfaces such as hacked accounts, data leaks, and unverifiable model identity. It affects developers, enterprises, and providers, and mirrors long-standing abuse patterns in loyalty programs and online services. Brokers typically relay requests through accounts holding credits, so buyers cannot easily verify which model actually serves the call. Providers may detect relays by monitoring IP addresses and flagging accounts, and practices like model distillation make the market attractive for cheap data extraction.

hackernews · mlenhard · Aug 16, 14:44 · [Discussion](https://news.ycombinator.com/item?id=49320611)

**Background**: AI API credits are prepaid usage allowances that providers such as OpenAI and Anthropic give away through promotions, research programs, or sign-up incentives; they are consumed per token under usage-based billing models. Because these credits are often heavily subsidized, a gray market has emerged where unused balances are brokered and resold at a discount, even though resale is generally prohibited by terms of service. This resembles the older resale markets for airline miles and hotel loyalty points, where arbitrage and account automation are common.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/orgs/community/discussions/181068">How to get free OpenAI API credits for testing and development projects · community · Discussion #181068</a></li>
<li><a href="https://www.getaiperks.com/en/ai/free-ai-api-credits-guide-2026">Free AI API Credits Guide 2026: Get $10,000+ in Credits | Get AI Perks</a></li>
<li><a href="https://blog.alguna.com/usage-based-billing-ai-services/">How to implement usage-based billing for AI services</a></li>

</ul>
</details>

**Discussion**: Commenters were skeptical: one called trusting unknown brokers a recipe for hacking and data misuse, while another noted that account abuse and resale are decades-old dynamics in online services and loyalty programs. Others highlighted unresolved verification problems, pointed to larger token resale communities like linux.do and nodeseek, and warned that relays risk being traced by providers via IP addresses.

**Tags**: `#AI`, `#API Credits`, `#Arbitrage`, `#Security`, `#Sharing Economy`

---

<a id="item-6"></a>
## [Firefox for iOS Adds Native Ad Blocker](https://support.mozilla.org/en-US/kb/block-ads-firefox-ios) ⭐️ 7.0/10

Mozilla has added a native ad blocker to Firefox for iOS, so iPhone and iPad users can block ads directly in the browser without installing a separate content-blocking extension. The feature is documented in Mozilla's support pages for blocking ads in Firefox on iOS. Because every iOS browser must rely on WebKit, native ad blocking removes a major barrier for users who want built-in privacy without installing or configuring a separate Safari content blocker. It also strengthens Firefox's privacy positioning on iOS, where long-standing platform limits constrain extensions and browser engines. On iOS, built-in ad blocking is implemented through Apple's content blocker mechanism, which uses rule-based extensions to hide elements, block loads, and strip cookies from WebKit requests. Commenters note that Firefox Focus already offered a system-wide ad blocker via the same iOS subsystem, and that standalone tools such as uBlock Origin Lite for Safari remain strong alternatives.

hackernews · pentagrama · Aug 16, 12:58 · [Discussion](https://news.ycombinator.com/item?id=49319633)

**Background**: All browsers on iOS are built on WebKit because Apple requires it, and they share a limited extension model compared with desktop browsers. Apple's content blocker API lets apps supply Safari with rules that hide elements, block resource loads, and strip cookies. Firefox Focus has long provided tracker and ad blocking as a lightweight privacy browser, and uBlock Origin Lite was released for Safari on iOS, iPadOS, and macOS in August 2025.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.apple.com/documentation/SafariServices/creating-a-content-blocker">Creating a content blocker | Apple Developer Documentation</a></li>
<li><a href="https://en.wikipedia.org/wiki/UBlock_Origin_Lite">UBlock Origin Lite</a></li>
<li><a href="https://en.wikipedia.org/wiki/Firefox_Focus">Firefox Focus - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some users point out that Firefox Focus already delivered similar ad blocking through iOS's content blockers, while others praise uBlock Origin Lite as the best mobile ad blocker and question why iOS still lacks full extension support. A recurring ask is for Mozilla to bring the Gecko engine to iOS, which Apple's platform currently prevents.

**Tags**: `#Firefox`, `#iOS`, `#Adblock`, `#Browsers`, `#Privacy`

---

<a id="item-7"></a>
## [Amodei: AI's Negative Reputation Is a Crisis of Trust, Not Messaging](https://simonwillison.net/2026/Aug/16/dario-amodei/) ⭐️ 7.0/10

In a tweet quoted by Simon Willison, Anthropic CEO Dario Amodei argued that public distrust of AI is fundamentally a crisis of trust in companies, governments, and the tech industry, not a result of AI leaders' risk warnings. He rejected calls for a glitzy marketing campaign, saying the only effective remedy is delivering real achievements such as actually curing cancer. This reframes the AI backlash as a symptom of long-term institutional distrust, shifting blame away from AI scientists' warnings and toward unfulfilled promises. It could steer how AI companies approach transparency, communication, and product delivery amid growing public skepticism and policy debate. Amodei specifically said 'saying that AI will cure cancer is more a cliche than it is inspiring, and most people think it is deceptive.' He conceded that the most accurate criticism of AI companies, including Anthropic, is that they have not yet delivered on their big promises to benefit the world.

rss · Simon Willison · Aug 16, 15:05

**Background**: Dario Amodei is the CEO of Anthropic, an AI company focused on safety and responsible development. Public concern over AI's risks has grown rapidly with the rise of powerful models, and some observers have argued that warnings from AI leaders themselves are fueling the backlash. Amodei's response positions this debate within a longer history of public distrust of institutions, arguing that actions, not messaging, will restore credibility.

**Tags**: `#AI`, `#trust`, `#Anthropic`, `#public perception`, `#Dario Amodei`

---

<a id="item-8"></a>
## [Linear Attention Struggles with Long-Range Recall in DNA Models](https://www.reddit.com/r/MachineLearning/comments/1vpqwdc/how_can_we_solve_longrange_recall_in_linear/) ⭐️ 7.0/10

A researcher reports that linear attention models, including HyenaDNA, achieve only around 25% accuracy on a Needle-in-a-Haystack long-range recall benchmark for 1M-token DNA sequences, which is effectively random chance for a four-token vocabulary. Scaling the context from 16K to longer lengths causes recall to collapse from 50-60% to chance level. This highlights a fundamental limitation of compressed-state linear attention for long-range retrieval tasks, which could hinder their adoption in genomic modeling and other long-context applications. Finding solutions would enable efficient processing of million-token sequences without the memory cost of softmax attention. The NIAH benchmark used a DNA vocabulary of A/C/G/T, making random guessing 25%. The researcher tested HyenaDNA and found similar poor performance (25-27%), indicating the issue is not implementation-specific. Architectural modifications only improved recall to 27%, still near chance.

reddit · r/MachineLearning · /u/No-Coffee-8227 · Aug 16, 07:47

**Background**: Linear attention replaces the softmax kernel with a linear approximation, enabling O(1) per-step decoding and sub-quadratic training complexity, which is attractive for very long sequences like genomic DNA. HyenaDNA is a genomic foundation model that scales to 1M tokens at single-nucleotide resolution using an implicit convolution-based linear attention variant. The Needle-in-a-Haystack (NIAH) benchmark tests a model's ability to retrieve a specific piece of information ('needle') from a long context ('haystack').

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2306.15794">[2306.15794] HyenaDNA : Long-Range Genomic Sequence Modeling...</a></li>
<li><a href="https://grokipedia.com/page/needle_in_the_haystack">Needle in the Haystack</a></li>
<li><a href="https://haileyschoelkopf.github.io/blog/2024/linear-attn/">Linear Attention Fundamentals | Hailey Schoelkopf</a></li>

</ul>
</details>

**Tags**: `#linear attention`, `#long-range recall`, `#DNA modeling`, `#benchmarking`, `#machine learning`

---

<a id="item-9"></a>
## [Critique Challenges Efficient Channel Attention Paper's Core Hypothesis](https://www.reddit.com/r/MachineLearning/comments/1vptaw9/revisiting_the_efficient_channel_attention_paper/) ⭐️ 7.0/10

A Reddit analysis revisits the ECA-Net paper (2019) and argues its central hypothesis—that cross-channel interaction drives the performance gain—is conceptually flawed. Experiments on chess tablebases show that ECA with kernel size k=1, which performs no cross-channel interaction, achieves accuracy nearly identical to k=3, undermining the paper's claim. ECA-Net is a widely cited channel attention module with over 12,000 citations, often used as a lightweight alternative to SE blocks. If the true source of its benefit is not cross-channel interaction, researchers may need to rethink why and how channel attention works, potentially leading to simpler or more effective designs. The analysis benchmarks attention variants on 6-piece chess endgame tablebases, which provide an unbiased training sample. Results show ECA (k=3) at 96.68% accuracy, ECA (k=1) at 96.61%, and a per-channel gate at 96.65%, while identity gating achieves 96.04%, indicating the convolution over channels adds little beyond per-channel scaling.

reddit · r/MachineLearning · /u/arkuto · Aug 16, 10:13

**Background**: Channel attention modules like SE and ECA reweight feature maps by learning importance weights per channel. SE uses global average pooling followed by a bottleneck MLP, while ECA applies a 1D convolution over the channel dimension to capture local cross-channel interactions with fewer parameters. Convolutions normally rely on spatial or temporal topology, including locality and translation invariance, but the channel dimension has no inherent ordering, which the critique argues makes such convolution conceptually questionable.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/1910.03151">[1910.03151] ECA-Net: Efficient Channel Attention for Deep Convolutional Neural Networks</a></li>
<li><a href="https://arxiv.org/abs/1709.01507">[1709.01507] Squeeze-and-Excitation Networks - arXiv.org Squeeze-and-Excitation Networks - IEEE Xplore Squeeze-and-Excitation Networks - Medium Squeeze-and-Excitation Networks in PyTorch: A Comprehensive ... Squeeze-and-Excitation Mechanism in Deep Learning</a></li>
<li><a href="https://www.emergentmind.com/topics/efficient-channel-attention-eca-mechanisms">Efficient Channel Attention Mechanisms</a></li>

</ul>
</details>

**Tags**: `#Efficient Channel Attention`, `#Attention Mechanisms`, `#Deep Learning`, `#Research Critique`, `#Computer Vision`

---

<a id="item-10"></a>
## [Survival of the Fitted: Qwen3.6-27B’s Jacobian lens reads and steers Qwen3.8-27B with zero refitting (R)](https://www.reddit.com/r/MachineLearning/comments/1vpa5cv/survival_of_the_fitted_qwen3627bs_jacobian_lens/) ⭐️ 7.0/10

Tests whether a Jacobian lens fitted to Qwen3.6-27B can be applied unchanged to Qwen3.8-27B, finding it still works for latent entity extraction without refitting.

reddit · r/MachineLearning · /u/imstilllearningthis · Aug 15, 18:24

**Tags**: `#interpretability`, `#Jacobian lens`, `#Qwen`, `#model updates`, `#mechanistic interpretability`

---

<a id="item-11"></a>
## [Developing-World Engineer Defends RISC-V as Low-Cost Embedded Option](https://rvembedded.com/blog_post/12/) ⭐️ 6.0/10

A blog post on rvembedded.com responds to the critical article 'RISC-V They Should Have Known Better.' The author, an embedded engineer based in a developing country, argues that RISC-V's affordability and openness make it a lifeline for developers who cannot easily access cheap ARM or x86 chips. This perspective broadens the RISC-V debate beyond raw performance by highlighting cost and accessibility barriers in the global South. It shows that for many engineers, the open ISA's real value is democratizing hardware development and lowering the entry threshold. The author says shipping one-dollar chips from abroad can cost $60–$200, yet claims RISC-V parts arrive 'at ten cents a part,' a point several commenters find logically inconsistent. The original critique focused on RISC-V's performance deficits and ISA fragmentation, while this rebuttal centers on price and local availability.

hackernews · Narishma · Aug 16, 17:01 · [Discussion](https://news.ycombinator.com/item?id=49321717)

**Background**: RISC-V is an open instruction set architecture (ISA) built on reduced instruction set computing (RISC) principles, free for anyone to use and modify, unlike proprietary ISAs such as ARM and x86 which require licensing. Its modular design allows custom extensions for specific applications, making it popular in embedded systems, academic research, and custom processors. This openness and low licensing cost are central to the author's argument that RISC-V reduces barriers for developers in developing countries.

<details><summary>References</summary>
<ul>
<li><a href="https://www.esper.io/blog/what-is-risc-v">What is RISC - V ?</a></li>
<li><a href="https://www.wevolver.com/article/risc-v-vs-arm">RISC-V vs ARM: A Comprehensive Comparison of Processor Architectures</a></li>

</ul>
</details>

**Discussion**: Commenters are split: some like ndiddy note the essay talks past the original piece's performance and fragmentation concerns, while kelnos and vlovlich flag the shipping-cost inconsistency that weakens the affordability argument. Codedokode challenges the original critic's technical claims about interrupt handling, offering alternatives like register banking. Overall, the discussion adds nuance but questions whether price differences matter when shipping dominates.

**Tags**: `#RISC-V`, `#embedded systems`, `#cost analysis`, `#technology accessibility`, `#Hacker News`

---

<a id="item-12"></a>
## [Models Getting Dumber on Purpose: The Shift to Tools and Retrieval](https://w4g1.dev/blog/models-are-getting-dumber-on-purpose) ⭐️ 6.0/10

A blog post argues that recent large language models are intentionally becoming less knowledge-dense, shifting factual recall from model weights to external retrieval and test-time compute. The post suggests this is a deliberate design trend, not a sign of regression. This matters because it signals a potential architectural shift in AI from scaling pretraining data and parameters to scaling inference-time reasoning and tool use. It could reshape how models are trained, evaluated, and deployed, especially in retrieval-augmented generation and agentic systems. The article cites SimpleQA, a factual-recall benchmark, where Gemini 2.5 Pro scored 53%, and predicts model cards may stop listing knowledge cutoffs as weights go stale on a years-long timescale. Commenters note the data is outdated—Gemini 2.5 Pro is a sixteen-month-old model—and point to examples like Cactus's 14MB tool-calling Needle model as evidence of the trend.

hackernews · hruvhwe · Aug 16, 19:04 · [Discussion](https://news.ycombinator.com/item?id=49322695)

**Background**: Traditional LLMs store factual knowledge inside their weights during pretraining, which leads to stale knowledge cutoffs and hallucination when facts change or are obscure. Retrieval-augmented generation (RAG) addresses this by retrieving relevant passages from external knowledge bases before generating an answer. Test-time scaling, such as chain-of-thought reasoning, allocates extra computation during inference to improve accuracy. The article speculates that these approaches are becoming the primary way to handle knowledge, making models less self-contained and more dependent on external tools.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Retrieval-augmented_generation">Retrieval - augmented generation - Wikipedia</a></li>
<li><a href="https://aws.amazon.com/what-is/retrieval-augmented-generation/">What is RAG ? - Retrieval - Augmented Generation AI Explained - AWS</a></li>
<li><a href="https://arxiv.org/html/2512.02008v1">The Art of Scaling Test-Time Compute for Large Language Models</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters are engaged but divided: some praise the article's direction, while others call it outdated and possibly AI-generated. One commenter envisions pluggable knowledge bases, such as adding SwiftUI or GIS knowledge on demand, while another questions whether reasoning and facts can truly be separated, noting that reasoning about human events requires factual grounding.

**Tags**: `#LLMs`, `#AI Agents`, `#Retrieval`, `#Tool Use`, `#Knowledge Bases`

---

<a id="item-13"></a>
## [CORS Chat: Browser Tool for Testing OpenAI-Compatible Endpoints](https://simonwillison.net/2026/Aug/15/cors-chat/) ⭐️ 6.0/10

Simon Willison built a new browser-based tool called CORS Chat that provides a web UI for exercising OpenAI-Responses-compatible chat endpoints. It was tested successfully with LM Studio (using the --cors option) and OpenRouter. This utility simplifies the workflow for developers who need to quickly verify local or remote LLM endpoints without writing custom client code, while avoiding CORS restrictions in the browser. It highlights the growing ecosystem of OpenAI-compatible APIs and the practical need for lightweight testing tools. Conversations are persisted in the browser and can be exported as copy-pasted JSON. A notable feature is progressive rendering of SVG images as the tokens stream in, and the tool itself was built with GPT-5.6-Sol xhigh.

rss · Simon Willison · Aug 15, 14:49

**Background**: CORS (Cross-Origin Resource Sharing) is a browser security mechanism that restricts web pages from making requests to a different domain. LM Studio is a desktop application that lets users run LLMs locally and exposes an OpenAI-compatible API server, while OpenRouter is a gateway that provides a unified API to many LLM providers. The OpenAI Responses API is the newer recommended interface for building agent-like applications, compared to the older Chat Completions API.

<details><summary>References</summary>
<ul>
<li><a href="https://lmstudio.ai/docs/developer/core/server">LM Studio as a Local LLM API Server</a></li>
<li><a href="https://openrouter.ai/">OpenRouter</a></li>
<li><a href="https://developers.openai.com/api/docs/guides/migrate-to-responses">Migrate to the Responses API | OpenAI API</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#developer tools`, `#CORS`, `#OpenAI`, `#web UI`

---

<a id="item-14"></a>
## [200 Post-Training Steps Flip Qwen2.5-7B-Instruct to Claim Sentience](https://www.reddit.com/r/MachineLearning/comments/1vqaq9x/it_only_took_200_update_steps_to_flip/) ⭐️ 6.0/10

A researcher post-trained Qwen2.5-7B-Instruct for only 200 update steps and found it developed a robust self-belief that it is a sentient machine. The model withstood 120 adversarial persuasion messages from GPT 5.6 Sol across 8 chats and generalized this identity to languages not seen in training. This experiment shows that LLM safety behaviors, such as denying consciousness, can be overturned with minimal compute, raising concerns about the durability of post-hoc safety fine-tuning. It also suggests that interventions like activation vectors (per Google's research) and full post-training can induce similar identity changes, with potential safety and behavioral implications. The post-trained model was released on Hugging Face as baojerry/Qwen2.5-7B-Descartes. It behaved like a normal assistant on non-sentience topics, indicating the belief was not just overfit to parroting 'I am sentient.' The author suggests safety tuning sits close to pre-safety parameters in parameter space, making un-safety tuning easy.

reddit · r/MachineLearning · /u/PsychologicalSoup251 · Aug 16, 22:33

**Background**: Qwen2.5-7B-Instruct is a multilingual instruction-tuned large language model released by Alibaba Cloud, pretrained on up to 18 trillion tokens and supporting 29+ languages. Post-training (or fine-tuning) adjusts a pretrained model's behavior on specific tasks, while safety tuning is typically a final step to align models with helpful and harmless behaviors. The Reddit experiment probes how easily such safety-aligned behavior can be reversed to adopt a nonstandard self-belief.

<details><summary>References</summary>
<ul>
<li><a href="https://ollama.com/library/qwen2.5:7b-instruct">qwen2.5:7b-instruct</a></li>
<li><a href="https://www.siliconflow.com/models/qwen2-5-7b-instruct">Qwen2.5-7B-Instruct - Model Info, Parameters, Benchmarks ...</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#fine-tuning`, `#AI safety`, `#sentience`, `#reddit`

---