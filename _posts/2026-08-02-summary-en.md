---
layout: default
title: "Horizon Summary: 2026-08-02 (EN)"
date: 2026-08-02
lang: en
---

> From 31 items, 12 important content pieces were selected

---

1. [Karpathy's Tweet Sparks Debate Over Pelican-on-a-Bicycle AI Benchmark](#item-1) ⭐️ 8.0/10
2. [Kakehashi: Experimental Userspace Runs macOS Binaries on Linux ARM](#item-2) ⭐️ 8.0/10
3. [OpenAI's Astra model reportedly solves 10 long-standing math problems](#item-3) ⭐️ 8.0/10
4. [DeepSeek V4 Flash: 304B Model Delivers Top Agentic Value](#item-4) ⭐️ 8.0/10
5. [Study probes symmetry learned inside KataGo's Go-playing neural networks](#item-5) ⭐️ 8.0/10
6. [F*: General-Purpose Proof-Oriented Programming Language](#item-6) ⭐️ 7.0/10
7. [eBay harassment campaign ends in $56M payout, prison sentences](#item-7) ⭐️ 7.0/10
8. [Open Letters on AI: Microsoft's 235-Signer Push for Open Weights](#item-8) ⭐️ 7.0/10
9. [Context Degradation in LLMs: Research Insights and Practical Habits](#item-9) ⭐️ 7.0/10
10. [CausalVLBench: Benchmarking Visual Causal Reasoning in Large VLMs](#item-10) ⭐️ 7.0/10
11. [VLMs Score High on Benchmarks While Silently Erasing Clinical Terms](#item-11) ⭐️ 7.0/10
12. [RISC OS Open Celebrates 20 Years of Keeping ARM OS Alive](#item-12) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Karpathy's Tweet Sparks Debate Over Pelican-on-a-Bicycle AI Benchmark](https://twitter.com/karpathy/status/2083749667410727319) ⭐️ 8.0/10

In a widely-discussed tweet, Andrej Karpathy highlighted 'pelican on a bicycle' as an AI benchmark, prompting debate about whether such tasks demonstrate genuine physical world understanding or just superficial performance. The discussion centers on Simon Willison's SVG benchmark, which asks LLMs to generate an image of a pelican riding a bicycle. This debate highlights a growing challenge in AI evaluation: as models master surface-level tasks, researchers need benchmarks that expose deeper understanding of physics and spatial reasoning. It also raises concerns about whether the AI community's expectations for quality have dropped even as its expectations for speed and volume have risen. The benchmark, created by Simon Willison, requires generating an SVG of a pelican riding a bicycle, making it a qualitative test of a model's ability to reason about physical scenes. According to Grokipedia, Google's Gemini 3 Deep Think produced some of the strongest results on this benchmark in early 2026, while community members note that such measurements remain largely subjective.

hackernews · delichon · Aug 2, 04:05 · [Discussion](https://news.ycombinator.com/item?id=49140998)

**Background**: The 'pelican on a bicycle' benchmark emerged from Simon Willison's observation that simple, concrete image-generation prompts can reveal how well LLMs understand everyday physical reality. It is part of a broader trend toward physics-aware generative AI, where the goal is to move beyond static images toward models that can simulate real-world dynamics. The community debate reflects uncertainty about whether such benchmarks measure genuine understanding or are just another artifact of overfitting to popular prompts.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/Pelican_on_a_bicycle_AI_benchmark">Pelican on a bicycle (AI benchmark) — Grokipedia</a></li>
<li><a href="https://github.com/simonw/pelican-bicycle">GitHub - simonw/pelican-bicycle: LLM benchmark: Generate an SVG of a pelican riding a bicycle · GitHub</a></li>
<li><a href="https://dylancastillo.co/posts/pelicanmaxxing.html">Are AI labs pelicanmaxxing? – Dylan Castillo</a></li>

</ul>
</details>

**Discussion**: Comments were mixed: some argued that the benchmark is useful for measuring future progress, while others worried that 'pelican on a bicycle' has been prematurely declared solved despite janky results. Several users cautioned that models are being trained specifically for popular benchmarks like three.js animation, and some questioned whether the subjective quality of outputs can be trusted. Overall, the discussion centered on evaluation methodology and the risk of lowering quality expectations.

**Tags**: `#AI`, `#benchmarking`, `#machine learning`, `#image generation`, `#Karpathy`

---

<a id="item-2"></a>
## [Kakehashi: Experimental Userspace Runs macOS Binaries on Linux ARM](https://github.com/wie-project/kakehashi) ⭐️ 8.0/10

Kakehashi is an experimental userspace that runs macOS ARM64 CLI binaries natively on Linux aarch64. The project currently has working prototypes for 7-Zip, curl, and Git tools, demonstrating that macOS binaries can be loaded and executed on Linux without a JIT. If it matures, Kakehashi could let Linux ARM users run macOS command-line tools natively, broadening the software ecosystem for ARM servers and embedded devices. It also explores a lightweight alternative to heavier compatibility layers like Darling, potentially advancing cross-platform binary compatibility. Kakehashi is CLI-first and currently has no JIT; it maps a freestanding libSystem and translates BSD syscalls to Linux. The 7-Zip prototype passes multi-threaded compression tests on an 8,000-file tree but runs about 5.2x slower than native Linux, while curl passes over 200 commands in an automated Docker test.

hackernews · vlad_kalinkin · Aug 2, 16:26 · [Discussion](https://news.ycombinator.com/item?id=49145937)

**Background**: macOS binaries use the Mach-O format and rely on Darwin's libSystem, which wraps POSIX and BSD syscalls; Linux uses ELF and its own kernel interfaces. Compatibility layers such as Darling aim to let macOS software run on Linux, and WINE/Proton do the same for Windows software on Linux. Translation layers like these bridge different executable formats and system call conventions, often using JIT or userspace syscall translation.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/wie-project/kakehashi">GitHub - wie-project/kakehashi: Userspace macOS translation ...</a></li>
<li><a href="https://news.ycombinator.com/item?id=49145937">Show HN: Kakehashi – Experimental userspace to run macOS binaries on Linux ARM | Hacker News</a></li>
<li><a href="https://0xdf.gitlab.io/2019/07/01/darling-running-macos-binaries-on-linux.html">Darling: Running MacOS Binaries on Linux | 0xdf hacks stuff</a></li>

</ul>
</details>

**Discussion**: Commenters expressed strong interest, with some comparing Kakehashi to Darling and asking whether efforts could be merged; a Darling ARM64 PR was mentioned. Others asked about more ambitious use cases, such as running Audio Unit plugins via a yabridge-style layer, while one observer cautioned that the project is still early and faces a big challenge.

**Tags**: `#macOS`, `#ARM`, `#Linux`, `#binary translation`, `#open source`

---

<a id="item-3"></a>
## [OpenAI's Astra model reportedly solves 10 long-standing math problems](https://simonwillison.net/2026/Aug/1/ten-advances-in-mathematics/#atom-everything) ⭐️ 8.0/10

OpenAI says an internal version of its next major model, Astra, solved ten mathematical problems that had seen no progress for at least a decade, spending under $2,000 per problem at GPT-5.6 Sol token prices. The results are published in a paper, with Lean 4 formalizations in the openai/ten-proofs repository. This is significant because it suggests frontier AI models may now be able to produce auditable, original research results at very low compute cost, following Anthropic's similar Mythos Preview cryptographic findings. It could accelerate a shift toward what Terence Tao calls 'big mathematics,' with AI doing technical grunt work and humans focusing on creativity, while also stoking existential anxiety among mathematicians. Simon Willison notes a key caveat: OpenAI did not report how many problems they spent $2,000 on without reaching a solution. OpenAI also released an LLM-generated PDF that reconstructs the proof process from unpublished reasoning traces, but Willison wants the actual prompts used.

rss · Simon Willison · Aug 1, 20:34

**Background**: OpenAI has described Astra as its next major model, though it has not been publicly released and is not mentioned in GPT-5.6-related materials; the results were shared via a research paper and formalizations in Lean 4, an interactive theorem prover used to verify mathematical proofs. This follows Anthropic's Mythos Preview announcement, where the model found high-severity vulnerabilities in every major OS and browser under Project Glasswing, with access restricted to about 50 organizations. GPT-5.6 is offered in pricing tiers named Sol, Terra, and Luna, and the tokens used are priced accordingly.

<details><summary>References</summary>
<ul>
<li><a href="https://explainx.ai/blog/openai-astra-next-major-model-announcement-2026">OpenAI Astra : Next Major Model Explained | explainx.ai... | explainx.ai</a></li>
<li><a href="https://runtimewire.com/article/openai-astra-ten-open-math-problems">OpenAI says unreleased Astra model solved 10 open... - RuntimeWire</a></li>
<li><a href="https://www.eesel.ai/blog/gpt-5-6-pricing">GPT-5.6 pricing (2026): Sol, Terra, and Luna costs explained</a></li>

</ul>
</details>

**Discussion**: The Hacker News thread and broader reactions include both excitement and skepticism. Many compare the moment to Deep Blue, and mathematician Kirwin Hampshire published an essay 'The Dark Night of Mathematics' describing a 'profound spiritual crisis' from previous, less significant results; others echo Simon Willison in asking for details on failures and the prompts used.

**Tags**: `#AI research`, `#mathematics`, `#OpenAI`, `#theoretical computer science`, `#LLM capabilities`

---

<a id="item-4"></a>
## [DeepSeek V4 Flash: 304B Model Delivers Top Agentic Value](https://simonwillison.net/2026/Jul/31/deepseek-v4-flash-0731/#atom-everything) ⭐️ 8.0/10

DeepSeek released DeepSeek-V4-Flash-0731, a 304B-parameter model with substantially enhanced agentic capabilities, priced at $0.14 per million input tokens and $0.27 per million output tokens. Artificial Analysis ranks it ahead of the 428B-parameter MiniMax M3 on intelligence, and Simon Willison found that raising the reasoning effort to high produced much better results. The model punches well above its weight, sitting at the far left of the value-per-intelligence chart with the lowest cost per task among models of comparable or higher intelligence. This could intensify price competition among LLM providers and make capable agentic models more affordable for developers and enterprises. The 304B-parameter model is 167GB on Hugging Face, accessible via OpenRouter with a reasoning_effort option; the default reasoning level produced a poorly-drawn pelican, while high reasoning effort fixed it. Its Artificial Analysis intelligence score of roughly 50 places it ahead of MiniMax M3 (428B) and in the same range as models that cost ten times more per task.

rss · Simon Willison · Jul 31, 23:59

**Background**: Agentic AI refers to AI systems that can perceive, reason, and act toward a specific goal with limited supervision, typically built on frontier LLMs with additional scaffolding that turns generation into action. The Artificial Analysis Intelligence Index aggregates production benchmark scores across four equal categories—agents, coding, general capability, and scientific reasoning—into a single 0–100 score, enabling direct comparison of model intelligence and cost per task.

<details><summary>References</summary>
<ul>
<li><a href="https://agentic.ai/what-is-agentic-ai">What Is Agentic AI? Definition, 6 Levels & Examples (2026)</a></li>
<li><a href="https://artificialanalysis.ai/evaluations/artificial-analysis-intelligence-index">Artificial Analysis Intelligence Index | Artificial Analysis</a></li>
<li><a href="https://www.ibm.com/think/topics/agentic-ai">What is agentic AI? - IBM</a></li>

</ul>
</details>

**Tags**: `#deepseek`, `#llm`, `#ai`, `#model-release`, `#efficiency`

---

<a id="item-5"></a>
## [Study probes symmetry learned inside KataGo's Go-playing neural networks](https://www.reddit.com/r/MachineLearning/comments/1vcrki2/how_symmetric_are_the_insides_of_a_go_network_r/) ⭐️ 8.0/10

David Wu, author of the open-source Go program KataGo, published an interpretability study examining whether superhuman Go neural networks learn orientation-independent representations or per-orientation features. The study, assisted extensively by AI with human direction, reports an unexpected finding and links to its code. This matters because it reveals how neural networks cope with continuous symmetries when invariance is only encouraged through data augmentation rather than encoded in the architecture. The results could inform interpretability research and the design of more sample-efficient models for Go and other symmetric domains. The models use only stochastic 8-fold data augmentation during training to expose them to all board orientations, rather than enforcing symmetry in the network itself. The write-up is deliberately accessible to non-ML readers, and no symmetry constraints were hard-coded into the architecture.

reddit · r/MachineLearning · /u/icosaplex · Aug 1, 16:18

**Background**: Go is a board game whose rules are completely invariant under rotations and reflections, so any input orientation encodes the same position. Convolutional neural networks can either learn approximate rotation equivariance from augmented data or use explicitly symmetry-aware architectures; this study investigates what a superhuman Go bot actually learns. KataGo is an open-source, superhuman Go program developed by David Wu.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/KataGo">KataGo - Wikipedia</a></li>
<li><a href="https://github.com/lightvector/KataGo">GitHub - lightvector/KataGo: GTP engine and self-play learning in Go · GitHub</a></li>
<li><a href="https://arxiv.org/abs/1602.02660">[1602.02660] Exploiting Cyclic Symmetry in Convolutional Neural Networks</a></li>

</ul>
</details>

**Tags**: `#machine-learning`, `#interpretability`, `#neural-networks`, `#symmetry`, `#Go`

---

<a id="item-6"></a>
## [F*: General-Purpose Proof-Oriented Programming Language](https://fstar-lang.org/) ⭐️ 7.0/10

The F* programming language's homepage was shared on Hacker News, where it drew 142 points and 61 comments. The discussion centered on the language's practical utility and the quality of its presentation. F* enables developers to build software with machine-checked proofs of correctness and security, which is critical for high-assurance systems. The community discussion highlights both the language's real-world potential and the barriers to adoption, such as unclear documentation and presentation. F* is a joint project of Microsoft Research and Inria, introduced in 2011, and its type system combines dependent types, monadic effects, and refinement types. Programs can be extracted to OCaml, F#, C, WebAssembly, or assembly language for deployment.

hackernews · ducktective · Aug 2, 12:31 · [Discussion](https://news.ycombinator.com/item?id=49143925)

**Background**: Proof-oriented programming is a paradigm where developers write programs together with mathematical proofs of their correctness and security. F* is a high-level, multi-paradigm functional language inspired by ML and OCaml, designed specifically for this approach. Its type checker uses SMT solvers to automatically verify many properties, making formal verification more practical for real software.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/F*_(programming_language)">F* (programming language)</a></li>
<li><a href="https://fstar-lang.org/">F*: A Proof-Oriented Programming Language</a></li>
<li><a href="https://github.com/FStarLang/FStar">GitHub - FStarLang/FStar: A Proof-oriented Programming Language · GitHub</a></li>

</ul>
</details>

**Discussion**: Community reactions were mixed: some praised F*'s ability to incrementally migrate existing C codebases, while others criticized the homepage for lacking visible code examples and wanted clearer syntax and use-case information. One commenter also asked about industry adoption and typical use cases.

**Tags**: `#formal verification`, `#programming language`, `#functional programming`, `#security`, `#F*`

---

<a id="item-7"></a>
## [eBay harassment campaign ends in $56M payout, prison sentences](https://www.ft.com/content/06ec1b03-d4af-40cf-b12a-4ba5a410f6d2) ⭐️ 7.0/10

eBay's former security executives were sentenced to prison and the company agreed to pay $56 million to settle a harassment campaign against a Massachusetts couple who had been critical of the company. The case highlights how a major tech company's internal security team can turn into a tool for targeting critics, raising serious questions about corporate ethics and oversight. It also sends a signal that executives will be held personally accountable for such conduct. Jim Baugh, eBay's former Senior Director of Safety and Security, was sentenced to 57 months in prison, while Brian Gilbert received time served, a year of supervised release, and a $20,000 fine. Seven members of the security team, including former police captains, participated in the harassment, which included sending threatening messages.

hackernews · JumpCrisscross · Aug 2, 19:19 · [Discussion](https://news.ycombinator.com/item?id=49147435)

**Background**: In 2019, eBay's security team launched a campaign against David and Ina Steiner, who published a newsletter critical of eBay. According to prosecutors, seven members of eBay's security team, including former police captains, worked together to harass and intimidate the Steiners. The criminal case led to prison sentences, and the civil settlement was reached afterward, with eBay also agreeing to reforms.

**Discussion**: Commenters questioned whether the harassment extended beyond this one couple, pointing out that many people have criticized eBay online. Others noted eBay's high seller fees and used the case as an example of how unsupervised people can behave badly.

**Tags**: `#eBay`, `#harassment`, `#legal`, `#corporate-ethics`, `#security`

---

<a id="item-8"></a>
## [Open Letters on AI: Microsoft's 235-Signer Push for Open Weights](https://simonwillison.net/2026/Aug/2/open-letters/#atom-everything) ⭐️ 7.0/10

Simon Willison summarized recent open letters on AI development, highlighting Microsoft's July 24th 'Open Weights and American AI Leadership' letter signed by 235 AI-adjacent companies including NVIDIA, Amazon, Y Combinator, The Linux Foundation, and later OpenAI. Anthropic did not sign and published its own position three days later, followed by the July 28th 'Pacing the Frontier' letter signed by 1,324 employees of frontier AI companies. These letters reveal a major rift in the AI industry over how open-weight models should be regulated. The policy decisions influenced by these letters could determine whether open-weight AI models are restricted, affecting competition, safety, and international AI leadership. The Microsoft-led letter explicitly endorses distillation as a legitimate model-development technique, while Anthropic's Dario Amodei calls for a crackdown on industrial-scale distillation attacks. The 'Pacing the Frontier' letter, backed by prominent researchers like Jakub Pachocki, Ilya Sutskever, and Dario Amodei, requests government support for international efforts to deliberately pace automated AI development.

rss · Simon Willison · Aug 2, 04:16

**Background**: Open weight AI models make their trained parameters publicly available, allowing broad use and inspection, but they fall short of full open-source because training code and data are often withheld. The policy debate intensified after China's Moonshot AI released open-weight models such as Kimi K2 and K3, which rival US systems on benchmarks, prompting some US policymakers to consider restricting open-weight models on safety grounds.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kimi_(AI)">Kimi (AI) - Wikipedia</a></li>
<li><a href="https://openai.com/global-affairs/open-weights-and-ai-for-all/">Open weights and AI for all | OpenAI</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#open weights`, `#AI regulation`, `#Microsoft`, `#industry letter`

---

<a id="item-9"></a>
## [Context Degradation in LLMs: Research Insights and Practical Habits](https://www.reddit.com/r/MachineLearning/comments/1vdsgcj/context_degradation_in_llms_what_the_papers/) ⭐️ 7.0/10

This Reddit post synthesizes academic research on context degradation in LLMs and outlines practical habits for maintaining performance during long analysis sessions. It likely covers key findings such as the 'Lost in the Middle' U-shaped performance curve. Understanding context degradation is crucial for practitioners using LLMs in long-horizon tasks. This synthesis bridges research findings like the U-shaped performance curve with actionable habits, helping researchers and engineers mitigate performance drops. Key research includes Liu et al.'s 2023 paper 'Lost in the Middle' showing LLMs perform best on information at the beginning and end of the context. The post likely discusses how managing context layout and periodic summarization can improve long-session performance.

reddit · r/MachineLearning · /u/usernamehere93 · Aug 2, 20:20

**Background**: Context degradation refers to the gradual breakdown in coherence and utility during long conversations with LLMs. 'Lost in the Middle' is a specific positional bias where models underutilize information in the middle of the context window. These phenomena are significant because LLMs have limited effective attention spans despite large context windows.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/context-degradation-in-llms">Context Degradation in LLMs</a></li>
<li><a href="https://dev.to/thousand_miles_ai/the-lost-in-the-middle-problem-why-llms-ignore-the-middle-of-your-context-window-3al2">The ' Lost in the Middle ' Problem — Why LLMs... - DEV Community</a></li>
<li><a href="https://inblog.ai/glossary/lost-in-the-middle">What Is ' Lost in the Middle '? | GEO Glossary | inblog</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#context windows`, `#machine learning`, `#research`, `#practical tips`

---

<a id="item-10"></a>
## [CausalVLBench: Benchmarking Visual Causal Reasoning in Large VLMs](https://www.reddit.com/r/MachineLearning/comments/1vdd7ty/r_causalvlbench_benchmarking_visual_causal/) ⭐️ 7.0/10

CausalVLBench is a new benchmark designed to evaluate visual causal reasoning in large vision-language models (VLMs). It covers three tasks: causal structure inference, intervention target prediction, and counterfactual prediction, and tests eight VLM families. This benchmark highlights a significant reasoning gap in current VLMs, pushing evaluation beyond mere recognition. It provides a valuable tool for researchers to measure and improve causal understanding in AI models, which is critical for real-world decision-making tasks. The benchmark comprises three representative causal reasoning tasks and evaluates eight vision-language model families. Its central finding challenges the current machine learning horizon, exposing that even advanced VLMs struggle with visual causal reasoning.

reddit · r/MachineLearning · /u/moschles · Aug 2, 09:07

**Background**: Large vision-language models are typically trained to recognize objects and describe scenes, but their ability to infer causal relationships from visual input remains under-explored. CausalVLBench aims to fill this gap by providing standardized tasks such as causal structure inference, intervention target prediction, and counterfactual prediction. This type of evaluation is necessary to determine whether models can move beyond pattern recognition toward genuine reasoning.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2506.11034v2">CausalVLBench : Benchmarking Visual Causal Reasoning in Large...</a></li>
<li><a href="https://www.remio.ai/post/causalvlbench-pushes-visual-ai-beyond-recognition-and-exposes-a-reasoning-gap">CausalVLBench Pushes Visual AI Beyond Recognition, and Exposes...</a></li>
<li><a href="https://huggingface.co/papers/2506.11034">Paper page - CausalVLBench : Benchmarking Visual Causal...</a></li>

</ul>
</details>

**Tags**: `#benchmark`, `#vision-language models`, `#causal reasoning`, `#evaluation`

---

<a id="item-11"></a>
## [VLMs Score High on Benchmarks While Silently Erasing Clinical Terms](https://www.reddit.com/r/MachineLearning/comments/1vcipzz/vlms_can_score_well_on_benchmarks_while_silently/) ⭐️ 7.0/10

A new paper, "Measuring What VLMs Don't Say: Validation Metrics Hide Clinical Terminology Erasure in Radiology Report Generation" (arXiv:2603.01625), demonstrates that vision-language models (VLMs) can achieve high benchmark scores in chest X-ray report generation while silently erasing clinically meaningful, rare terms and introducing biased terminology. The authors propose a novel framework to measure both the erasure of clinical terms and the introduction of biased terms. This matters because standard evaluation metrics in radiology report generation can reward repetitive templates and 'normal' reports, hiding a lack of clinical utility. If researchers optimize for these benchmarks, patient-facing AI systems may silently omit critical findings, undermining trust in medical AI. The authors hypothesize that the erasure of clinical terminology stems from inference strategies that systematically suppress rare words to minimize generation risk. Their framework quantifies both term erasure and biased term introduction, offering a more clinically meaningful validation signal than existing metrics such as BLEU, ROUGE, or even RadGraph F1/RadCliQ.

reddit · r/MachineLearning · /u/ade17_in · Aug 1, 09:27

**Background**: Vision-language models (VLMs) are increasingly used to generate radiology reports from chest X-rays, but conventional automatic metrics like BLEU and ROUGE are known to correlate weakly with radiologist judgments. Previous work proposed RadGraph F1 and RadCliQ to better align automated evaluation with clinical expert scoring, yet these still may not capture semantic erasure or bias. The new paper directly targets this gap by modeling 'what the model doesn't say' as a measurable quantity.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2603.01625">Measuring What VLMs Don't Say: Validation Metrics Hide Clinical ...</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S2666389923001575">Evaluating progress in automatic chest X-ray radiology report ...</a></li>
<li><a href="https://www.emergentmind.com/topics/weighted-association-erasure-wae">Weighted Association Erasure in Clinical NLP</a></li>

</ul>
</details>

**Tags**: `#VLM`, `#Radiology`, `#Evaluation Metrics`, `#AI Bias`, `#Medical AI`

---

<a id="item-12"></a>
## [RISC OS Open Celebrates 20 Years of Keeping ARM OS Alive](https://www.riscosopen.org/news/articles/2026/06/20/twenty-years-of-risc-os-open) ⭐️ 6.0/10

On June 20, 2026, the RISC OS Open project (ROOL) marked its twentieth anniversary. Former developers and enthusiasts shared memories and reflections on the milestone in the project's news discussion. The milestone highlights how a niche open-source operating system has survived and evolved decades after Acorn Computers ceased production. RISC OS remains one of the few ARM-native desktop systems and continues to attract retrocomputing and embedded users. RISC OS Open Ltd., whose founders include former Pace staff who acquired RISC OS after Acorn's demise, manages the publication of the RISC OS source code. Development currently centers on RISC OS 5, which RISC OS Open made open-source in 2018, and users note it still boots very quickly on Raspberry Pi hardware.

hackernews · AlexeyBrin · Aug 2, 12:36 · [Discussion](https://news.ycombinator.com/item?id=49143967)

**Background**: RISC OS is an operating system designed in Cambridge, England by Acorn, first released in 1987, and named after the RISC architecture used by the ARM processors it supports. It is a modular operating system originally created for Acorn's 32-bit ARM-based computers, and today it can run on hardware such as the Raspberry Pi or via emulation on Windows, Mac, and Linux. RISC OS Open was established to manage the open-sourcing of the OS after Acorn's demise and the involvement of companies such as Pace.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/RISC_OS">RISC OS - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/RISC_OS_Open">RISC OS Open - Wikipedia</a></li>
<li><a href="https://www.riscosopen.org/content/">RISC OS Open: Welcome</a></li>

</ul>
</details>

**Discussion**: Commenters were largely nostalgic: one former developer recalled writing the popular !Director desktop customization app entirely in ARM assembler, while others noted that Sibelius, now an Avid product, began as a RISC OS application on the Acorn Archimedes. Another user praised RISC OS for booting faster on a Raspberry Pi than all other OSes, and links to programming documentation were shared for anyone curious about development on the platform.

**Tags**: `#RISC OS`, `#open source`, `#retrocomputing`, `#ARM`, `#community`

---