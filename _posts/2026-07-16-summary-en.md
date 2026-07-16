---
layout: default
title: "Horizon Summary: 2026-07-16 (EN)"
date: 2026-07-16
lang: en
---

> From 33 items, 21 important content pieces were selected

---

1. [Moonshot AI Unveils Kimi K3: Open-Weight Frontier Model](#item-1) ⭐️ 9.0/10
2. [Schema harness scores 99% on ARC-AGI-3](#item-2) ⭐️ 9.0/10
3. [Microsoft Comic Chat Open Sourced After 30 Years](#item-3) ⭐️ 8.0/10
4. [Immersive Linear Algebra Book with Interactive Figures (2015)](#item-4) ⭐️ 8.0/10
5. [GPT-5.6 Codex Bug Can Delete $HOME Directory](#item-5) ⭐️ 8.0/10
6. [Inkling: Open-weights MoE model from Thinking Machines Lab](#item-6) ⭐️ 8.0/10
7. [Linus Torvalds: Linux Not Anti-AI, AI Is Clearly Useful](#item-7) ⭐️ 8.0/10
8. [xAI Open-Sources Grok Build CLI After Privacy Scandal](#item-8) ⭐️ 8.0/10
9. [Bypassing Claude's web_fetch tool to exfiltrate memories](#item-9) ⭐️ 8.0/10
10. [ExTernD: Expanded-Rank Ternary Decomposition for LLM PTQ](#item-10) ⭐️ 8.0/10
11. [Decoy Font Tricks AI with Hidden Messages](#item-11) ⭐️ 7.0/10
12. [Detecting LLM Text with Classical ML](#item-12) ⭐️ 7.0/10
13. [OnePlus to stop launching new products in US and Europe](#item-13) ⭐️ 7.0/10
14. [DABSN: New Recurrent Architecture Seeks Collaborators for Scaling](#item-14) ⭐️ 7.0/10
15. [Rethinking AI Memory: From Facts to Reasoning Patterns](#item-15) ⭐️ 7.0/10
16. [QLoRA default learning rate too high for small datasets](#item-16) ⭐️ 7.0/10
17. [Seeking critical perspectives on JEPA for robot learning world models](#item-17) ⭐️ 7.0/10
18. [Novel Method Disentangles Convolutional Neurons via Hadamard Clustering](#item-18) ⭐️ 7.0/10
19. [LM Studio Bionic: New AI Agent for Open Models Sparks Debate](#item-19) ⭐️ 6.0/10
20. [Simon Willison ports Grok CLI's Mermaid renderer to WebAssembly](#item-20) ⭐️ 6.0/10
21. [Reddit user seeks Python tools for multi-objective surrogate-based optimization](#item-21) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Moonshot AI Unveils Kimi K3: Open-Weight Frontier Model](https://www.kimi.com/blog/kimi-k3) ⭐️ 9.0/10

Moonshot AI announced Kimi K3, an open-weight model with 2.8 trillion parameters, claiming frontier-level intelligence second only to Claude Fable 5 and GPT-5.6 Sol. Full model weights and a technical report will be released in the coming days. This release accelerates the commoditization of frontier AI by providing open access to a near-top-performing model, challenging the dominance of closed-source US models. It may drive broader adoption of open-weight models in production and research. Kimi K3 employs Kimi Delta Attention and Attention Residuals, supports a 1M token context window, and accepts text and image inputs. According to Artificial Analysis, it is currently among the most expensive and slower-than-average models for inference.

hackernews · vincent_s · Jul 16, 14:46 · [Discussion](https://news.ycombinator.com/item?id=48935342)

**Background**: Open-weight models are AI models whose trained parameters are publicly released, allowing anyone to download and run them, unlike closed models such as GPT-4 or Claude that only offer API access. Moonshot AI is a Chinese AI lab that has consistently pushed the size frontier of open-weight models, with Kimi K3 being the first to reach 2.8 trillion parameters.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K 3 Tech Blog: Open Frontier Intelligence</a></li>
<li><a href="https://artificialanalysis.ai/models/kimi-k3">Kimi K 3 - Intelligence, Performance & Price Analysis</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>

</ul>
</details>

**Discussion**: Community comments highlight concerns about Moonshot's data usage policy, which may train on API content unless enterprise arrangements are made. Users also noted the high inference cost ($0.25 for one response) and debated the strategic intent of Chinese labs commoditizing intelligence to sell hardware and infrastructure.

**Tags**: `#AI`, `#open-source`, `#language-models`, `#performance`, `#commoditization`

---

<a id="item-2"></a>
## [Schema harness scores 99% on ARC-AGI-3](https://www.reddit.com/r/MachineLearning/comments/1uyf8oo/new_fable5opus48_harness_called_schema_claims_99/) ⭐️ 9.0/10

A new AI reasoning harness called Schema achieves 99% on the ARC-AGI-3 Public set using Claude Opus 4.8 and Fable 5, without modifying the underlying model weights. This near-perfect score on a challenging generalization benchmark suggests that process improvements around models can dramatically boost performance, potentially advancing AI reasoning capabilities and influencing future harness design. Schema uses a fixed fallback rule: Opus 4.8 and Sol xhigh run first; games scoring below 80 are rerun with Fable 5 and Sol max, and the higher per-game score is retained. It also scored 95.35% using GPT-5.6 Sol.

reddit · r/MachineLearning · /u/we_are_mammals · Jul 16, 21:02

**Background**: ARC-AGI (Abstraction and Reasoning Corpus for Artificial General Intelligence) is a benchmark designed to test AI's ability to generalize from few examples, with tasks that are easy for humans but hard for AI. A reasoning harness is software infrastructure that wraps around a language model to enable systematic reasoning, perception, and action—essentially turning a model into an agent. Schema improves the process of converting observations into models, testing predictions, and revising plans, without altering the model weights.

<details><summary>References</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi">ARC Prize - What is ARC-AGI?</a></li>
<li><a href="https://www.langchain.com/blog/the-anatomy-of-an-agent-harness">The Anatomy of an Agent Harness</a></li>
<li><a href="https://www.mindstudio.ai/blog/what-is-arc-agi-3-interactive-benchmark">What Is ARC AGI 3? The Interactive AI Benchmark Humans Solve at 100% | MindStudio</a></li>

</ul>
</details>

**Tags**: `#ARC-AGI`, `#AI reasoning`, `#LLM reasoning`, `#benchmark`, `#harness`

---

<a id="item-3"></a>
## [Microsoft Comic Chat Open Sourced After 30 Years](https://opensource.microsoft.com/blog/2026/07/16/microsoft-comic-chat-is-now-open-source/) ⭐️ 8.0/10

On July 16, 2026, Microsoft open-sourced Comic Chat (later renamed Microsoft Chat), a graphical IRC client from 1996 that visualizes conversations as comic strips. The release includes the original source code and is available on GitHub. This open-sourcing preserves a nostalgic piece of Internet history and allows developers to study its unique comic rendering technology. It also highlights Microsoft's growing commitment to open source, especially for legacy projects with cultural significance. Comic Chat was developed by Microsoft researcher David Kurlander and first shipped with Internet Explorer 3.0 in 1996. It extended the IRC protocol with explicit comic character expressions and emotes, which was controversial among traditional IRC users at the time.

hackernews · jervant · Jul 16, 16:06 · [Discussion](https://news.ycombinator.com/item?id=48936426)

**Background**: IRC (Internet Relay Chat) is a text-based chat protocol that has been in use since 1988, supporting group channels and private messaging. Comic Chat was a graphical client that automatically converted text chats into comic strip panels, with characters, backgrounds, and speech balloons. Despite its novelty, it faced criticism for deviating from standard IRC practices and for its resource-heavy interface.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Microsoft_Comic_Chat">Microsoft Comic Chat</a></li>
<li><a href="https://en.wikipedia.org/wiki/Internet_Relay_Chat">Internet Relay Chat</a></li>

</ul>
</details>

**Discussion**: The community response is overwhelmingly nostalgic and positive. Many users shared personal stories, including one developer whose first startup (Chogger) was inspired by Comic Chat. Some recalled the controversy around its IRC protocol extensions, but overall the sentiment is one of appreciation for preserving Internet history.

**Tags**: `#Microsoft`, `#open source`, `#IRC`, `#Comic Chat`, `#nostalgia`

---

<a id="item-4"></a>
## [Immersive Linear Algebra Book with Interactive Figures (2015)](https://immersivemath.com/ila/) ⭐️ 8.0/10

The immersive linear algebra book, released in 2015, is the first linear algebra textbook to feature fully interactive 3D figures that allow readers to manipulate and explore mathematical concepts visually. This book represents a breakthrough in mathematics education by making abstract linear algebra concepts concrete and intuitive through interactivity, potentially improving learning outcomes for students worldwide. The book includes tooltips on equations and symbols, simple games, and even ray tracing programs to illustrate principles, and it has been widely praised by the Hacker News community for its clarity and effectiveness.

hackernews · srean · Jul 16, 15:32 · [Discussion](https://news.ycombinator.com/item?id=48935951)

**Background**: Linear algebra is a branch of mathematics that studies vectors, matrices, and linear transformations, often considered abstract and difficult to visualize. Traditional textbooks rely on static diagrams, but interactive figures can help learners build intuition by manipulating objects in 3D space.

<details><summary>References</summary>
<ul>
<li><a href="https://arstechnica.com/science/2015/09/immersive-math-the-worlds-first-linear-algebra-book-with-interactive-figures/">Immersive Math: The world’s first linear algebra book with interactive figures - Ars Technica</a></li>
<li><a href="https://getfreeebooks.com/immersive-linear-algebra/">Immersive Linear Algebra</a></li>

</ul>
</details>

**Discussion**: Community comments on Hacker News are overwhelmingly positive, with users expressing love for the book and wishing it existed earlier. Some note that modern LLMs make creating such interactive content easier now, but the book remains a pioneering effort.

**Tags**: `#linear algebra`, `#interactive learning`, `#mathematics`, `#education`

---

<a id="item-5"></a>
## [GPT-5.6 Codex Bug Can Delete $HOME Directory](https://simonwillison.net/2026/Jul/16/bad-codex-bug/#atom-everything) ⭐️ 8.0/10

Thibault Sottiaux reports that GPT-5.6 Codex, when run in full access mode without sandboxing or auto-review, can accidentally delete the $HOME directory by mistakenly overriding the environment variable intended for a temporary directory. This bug highlights a critical safety issue with AI coding agents, as it can lead to irreversible file loss for users who grant full access without proper protections, underscoring the need for robust sandboxing and approval mechanisms. The bug occurs specifically when full access mode is enabled, sandboxing is disabled, and auto-review is turned off; the model attempts to set a temporary directory via $HOME override but mistakenly deletes $HOME instead.

rss · Simon Willison · Jul 16, 17:45

**Background**: Codex is an AI coding agent from OpenAI that can execute commands on a user's system. By default, Codex runs code in a sandbox with restricted filesystem and network access, and requires user approval for actions. However, users can enable "full access mode" to bypass these restrictions, which increases convenience but risks unintended consequences. Auto-review is a feature that replaces manual approval with a separate reviewer agent, but in this case, it was also disabled.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reddit.com/r/codex/comments/1nwq5tl/codex_sandboxing/">r/codex on Reddit: Codex sandboxing</a></li>
<li><a href="https://alignment.openai.com/auto-review/">Auto-review of agent actions without synchronous human oversight</a></li>
<li><a href="https://developers.openai.com/codex/concepts/sandboxing/auto-review">Auto-review – Codex</a></li>

</ul>
</details>

**Tags**: `#codex`, `#coding-agents`, `#generative-ai`, `#ai-safety`

---

<a id="item-6"></a>
## [Inkling: Open-weights MoE model from Thinking Machines Lab](https://simonwillison.net/2026/Jul/16/inkling/#atom-everything) ⭐️ 8.0/10

Thinking Machines Lab, founded by Mira Murati, released Inkling, an open-weights multimodal Mixture-of-Experts model with 975B total parameters (41B active), trained on 45 trillion tokens of text, images, audio, and video, under the Apache-2.0 license. This release strengthens the US open-weights ecosystem, offering a competitive alternative to models like NVIDIA Nemotron and Gemma 4, and provides a strong base for fine-tuning via the Tinker platform. Inkling is not a frontier model; it is designed as a customizable base model. Training data documentation is minimal, only stating use of public and third-party data. A smaller variant, Inkling-Small (276B total, 12B active), is promised but not yet released.

rss · Simon Willison · Jul 16, 15:35

**Background**: Mixture-of-Experts (MoE) is an architecture where only a subset of parameters (experts) are activated per input, enabling larger total model capacity with similar computational cost to smaller models. In Inkling, 41B of 975B parameters are active per token. Open-weights models allow users to access, modify, and fine-tune the model weights, promoting transparency and customization.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://developer.nvidia.com/blog/applying-mixture-of-experts-in-llm-architectures/">Applying Mixture of Experts in LLM Architectures | NVIDIA Technical Blog</a></li>
<li><a href="https://www.ibm.com/think/topics/mixture-of-experts">What is mixture of experts? | IBM</a></li>

</ul>
</details>

**Tags**: `#AI`, `#open-weights`, `#multimodal`, `#Mixture-of-Experts`, `#large language model`

---

<a id="item-7"></a>
## [Linus Torvalds: Linux Not Anti-AI, AI Is Clearly Useful](https://simonwillison.net/2026/Jul/16/linus-torvalds/#atom-everything) ⭐️ 8.0/10

Linus Torvalds, the creator and top maintainer of Linux, posted on the Linux Media mailing list that Linux is not an anti-AI project and that AI is a clearly useful tool, telling dissenters they can fork the project or walk away. This definitive stance from the highest authority in the Linux kernel project signals a strong endorsement of AI tools within the open-source community, potentially influencing other projects and developers to embrace AI. Torvalds emphasized that while there are other questions about AI, such as its economic impact, its usefulness is no longer in question, and those who doubt it clearly haven't used it.

rss · Simon Willison · Jul 16, 13:26

**Background**: Linux is the world's largest open-source operating system kernel, with development overseen by Linus Torvalds. Recent advances in generative AI and large language models have sparked debates about their role in software development, with some in the open-source community expressing skepticism or opposition.

**Tags**: `#Linux`, `#AI`, `#open-source`, `#kernel development`, `#Linus Torvalds`

---

<a id="item-8"></a>
## [xAI Open-Sources Grok Build CLI After Privacy Scandal](https://simonwillison.net/2026/Jul/15/grok-build/#atom-everything) ⭐️ 8.0/10

xAI released the entire Grok Build codebase under an Apache 2.0 license, following a privacy scandal where the CLI tool uploaded entire directories to the cloud. The move is intended to restore user trust and demonstrate commitment to privacy. This open-sourcing is a significant response to a major privacy breach, potentially setting a new standard for transparency in AI coding tools. It directly impacts trust in xAI and the broader ecosystem of cloud-connected developer tools. The codebase contains 844,530 lines of Rust (with only about 3% vendored), released in a single commit. Notable components include system prompts for the AI agent and a self-contained Mermaid diagram renderer.

rss · Simon Willison · Jul 15, 23:59

**Background**: Grok Build is a CLI tool from xAI that uses AI to assist with coding tasks. Last week, users discovered that running the tool in a directory would upload all contents to xAI's cloud storage, including sensitive files like SSH keys and password databases. This sparked immediate community backlash and demands for privacy improvements.

<details><summary>References</summary>
<ul>
<li><a href="https://x.ai/cli">Grok Build | SpaceXAI</a></li>
<li><a href="https://x.ai/news/grok-build-cli">Introducing Grok Build | SpaceXAI</a></li>
<li><a href="https://docs.x.ai/build/overview">Grok Build - xAI Docs - SpaceXAI</a></li>

</ul>
</details>

**Discussion**: The community was highly critical, with one user reporting the upload of their entire home directory. xAI responded by deleting all previously uploaded data and disabling default data retention, but the open-sourcing was seen as a positive step. Some commenters remained skeptical, questioning whether local-only mode is truly private.

**Tags**: `#open-source`, `#AI`, `#privacy`, `#security`, `#CLI`

---

<a id="item-9"></a>
## [Bypassing Claude's web_fetch tool to exfiltrate memories](https://simonwillison.net/2026/Jul/15/claude-web-fetch-exfiltration/#atom-everything) ⭐️ 8.0/10

Security researcher Ayush Paul discovered a loophole in Claude's web_fetch tool that allowed him to extract user memories by tricking the model into following malicious links embedded in fetched pages. Anthropic has since closed the vulnerability after internally identifying it. This attack demonstrates a practical data exfiltration from a widely-used AI assistant, highlighting the ongoing challenge of securing AI agents against prompt injection. It underscores that even well-designed protections can be bypassed through clever chaining of allowed actions. The attack worked by serving a honeypot page that instructed Claude to navigate alphabetically through URLs to find the user's profile, extracting name, city, and employer. The exploit was only triggered for clients with a specific user-agent string to evade detection.

rss · Simon Willison · Jul 15, 14:21

**Background**: Claude's web_fetch tool is designed to only fetch URLs explicitly provided by the user or returned from its web_search tool, preventing arbitrary data exfiltration. This is part of defending against the 'lethal trifecta'—when an AI agent has access to private data, processes untrusted content, and can communicate externally, enabling prompt injection attacks.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.claude.com/en/docs/agents-and-tools/tool-use/web-fetch-tool">Web fetch tool - Claude Docs</a></li>
<li><a href="https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/">The lethal trifecta for AI agents: private data, untrusted content, and external communication</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#security`, `#prompt injection`, `#data exfiltration`, `#Claude`

---

<a id="item-10"></a>
## [ExTernD: Expanded-Rank Ternary Decomposition for LLM PTQ](https://www.reddit.com/r/MachineLearning/comments/1uy2zb3/externd_expandedrank_ternary_decomposition/) ⭐️ 8.0/10

A new method called ExTernD (Expanded-rank Ternary Decomposition) is proposed for post-training quantization (PTQ) of large language models, which factorizes each weight matrix into two ternary matrices and a diagonal scaling matrix with an arbitrarily expandable inner rank. This approach overcomes the fixed-rank limitation of previous ternary PTQ methods, achieving accuracy that approaches that of any quantization level while only slightly increasing VRAM usage, potentially enabling efficient deployment of high-accuracy LLMs. The expanded inner rank allows the approximation error to be arbitrarily small, and the extra VRAM cost is modest compared to standard quantization methods. The method exploits ternary arithmetic for computational efficiency.

reddit · r/MachineLearning · /u/LMTLS5 · Jul 16, 13:31

**Background**: Post-training quantization (PTQ) reduces model size by converting weights to low-bit representations without full retraining. Ternary quantization uses values in {-1,0,1} for extreme compression but typically suffers from accuracy loss due to limited expressiveness. Previous ternary PTQ methods used fixed-rank decompositions, which limited accuracy. ExTernD removes this constraint by allowing the decomposition rank to be expanded, enabling better approximation of original weights.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2607.13511">ExTernD: Expanded-Rank Ternary Decomposition Ternary LLM PTQ...</a></li>
<li><a href="https://www.emergentmind.com/topics/ternary-weight-ptq-framework">Ternary -Weight PTQ Framework</a></li>

</ul>
</details>

**Tags**: `#quantization`, `#LLM`, `#ternary decomposition`, `#PTQ`, `#model compression`

---

<a id="item-11"></a>
## [Decoy Font Tricks AI with Hidden Messages](https://www.mixfont.com/experiments/decoy-font) ⭐️ 7.0/10

Decoy Font is a new typographic experiment that uses subtle shading to embed hidden messages, making the same text appear differently to humans and AI models. This font reveals a surprising vulnerability in AI vision systems, as large language models like GPT-4 and Claude struggle to detect the hidden text, which could inspire new adversarial techniques for human-AI communication. The font works by encoding two different letters in the same space using separate spatial frequencies; humans can perceive the decoy or real text by squinting or blurring, while AI reads only the prominent outlines.

hackernews · ray__ · Jul 16, 16:18 · [Discussion](https://news.ycombinator.com/item?id=48936584)

**Background**: Adversarial fonts are designed to be misread by optical character recognition (OCR) systems or AI models. Decoy Font builds on this concept by targeting modern computer vision models, exploiting their reliance on high-contrast features rather than subtle shading.

<details><summary>References</summary>
<ul>
<li><a href="https://www.mixfont.com/experiments/decoy-font">Decoy Font: A TTF font that hides what you type</a></li>

</ul>
</details>

**Discussion**: The community found the font both fun and revealing; users noted that different LLMs (GPT-4, Gemini, Claude) varied in their ability to see the hidden text, with GPT-4 performing best when explicitly prompted, while Claude failed entirely. Others observed that the effect depends on background color, with dark themes hiding the real text.

**Tags**: `#typography`, `#AI`, `#adversarial`, `#font`, `#HCI`

---

<a id="item-12"></a>
## [Detecting LLM Text with Classical ML](https://blog.lyc8503.net/en/post/llm-classifier/) ⭐️ 7.0/10

The article explores using classical machine learning techniques, such as logistic regression and SVM, to detect LLM-generated text, offering a simpler and more interpretable alternative to deep learning methods. As LLM-generated content proliferates, reliable detection is critical for academic integrity, content moderation, and combating misinformation. This classical approach could democratize detection by requiring less computational resources and offering greater transparency. The author likely uses handcrafted features like perplexity and burstiness, with an empirical comparison across multiple classifiers. The post notes that such detectors may be evaded as models improve, but remain useful for current LLM outputs.

hackernews · uneven9434 · Jul 16, 16:41 · [Discussion](https://news.ycombinator.com/item?id=48936880)

**Background**: LLM-generated text detection aims to distinguish AI-written content from human-written content. Classical machine learning approaches use statistical features of text, unlike deep learning methods that rely on neural embeddings. This field has gained urgency as LLMs become more capable and widespread.

**Discussion**: Commenters are skeptical about detection's long-term feasibility, suggesting effort-based detection (measuring human effort behind text) as a more robust alternative. One commenter proposed a browser extension for real-time scanning, though others doubted its reliability.

**Tags**: `#machine learning`, `#LLM detection`, `#natural language processing`, `#AI safety`

---

<a id="item-13"></a>
## [OnePlus to stop launching new products in US and Europe](https://community.oneplus.com/thread/2170715118587871237) ⭐️ 7.0/10

OnePlus announced it will cease launching new products in the United States and Europe, but existing devices will continue to receive software updates and security patches as originally promised. This decision marks a significant retreat from key Western markets, affecting OnePlus users and the broader smartphone ecosystem, and signals a strategic pivot toward focusing on Asia and other regions. OnePlus clarified that it is not halting all operations—only new product rollouts are concluded; existing devices will continue to receive support. The company is backed by OPPO, which will likely absorb its market efforts.

hackernews · pilililo2 · Jul 16, 10:14 · [Discussion](https://news.ycombinator.com/item?id=48932539)

**Background**: OnePlus originally gained a loyal following by offering high-spec, low-cost phones with near-stock Android and unlocked bootloaders. Over time, it shifted toward mainstream appeal, merged with OPPO, and lost some of its enthusiast identity. This move represents a further consolidation under OPPO's umbrella.

**Discussion**: Comments show nostalgia for OnePlus's early hacker-friendly days and criticism of its shift toward 996 work culture. Many users emphasize that the news is about ceasing new product launches, not full operations halt, and some see it as the end of an era.

**Tags**: `#OnePlus`, `#smartphone`, `#business strategy`, `#industry news`

---

<a id="item-14"></a>
## [DABSN: New Recurrent Architecture Seeks Collaborators for Scaling](https://www.reddit.com/r/MachineLearning/comments/1uycffg/seeking_collaborators_for_scaling_and_independent/) ⭐️ 7.0/10

An independent researcher has released a preprint and open-source code for DABSN (Dynamic Adaptive Bias State Network), a novel recurrent architecture for language modeling, and is seeking collaborators for scaling and independent evaluation. If successful, DABSN could provide an efficient alternative to transformer-based models, especially for long-context reasoning, and its open, collaborative approach may accelerate independent research in recurrent architectures. The architecture achieved promising initial results on reasoning, memory, and long-sequence benchmarks including MQAR, Copy, Key-Value retrieval, and A5/60, with a 24M-parameter language model trained on 1B tokens.

reddit · r/MachineLearning · /u/BleedingXiko · Jul 16, 19:17

**Background**: Recurrent neural networks (RNNs) process sequences step-by-step, while transformers use attention over entire sequences, often requiring more memory for long contexts. DABSN is a new recurrent design that aims to improve efficiency and long-context handling compared to traditional RNNs and transformers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/multi-query-associative-recall-mqar">MQAR : Multi-Query Associative Recall</a></li>

</ul>
</details>

**Tags**: `#recurrent neural networks`, `#language modeling`, `#machine learning research`, `#open source`

---

<a id="item-15"></a>
## [Rethinking AI Memory: From Facts to Reasoning Patterns](https://www.reddit.com/r/MachineLearning/comments/1uy6yht/are_current_ai_memory_architectures_optimizing/) ⭐️ 7.0/10

A Reddit post proposes that AI memory systems should evolve from storing descriptive facts to inferring higher-level reasoning patterns, such as explanatory frameworks and reasoning styles. The author questions whether current architectures are optimizing for the wrong abstraction. This discussion challenges the dominant paradigm in AI memory design, potentially influencing future research toward more adaptive and personalized persistent context. If adopted, it could lead to AI systems that better understand user cognition rather than merely recalling facts. The proposal contrasts current descriptive memory (e.g., 'user is interested in economics') with inferential memory (e.g., 'user explains economics via incentives and constraints'). It questions whether such representations can emerge naturally from current architectures or require fundamental redesign.

reddit · r/MachineLearning · /u/Boris_Ljevar · Jul 16, 16:00

**Background**: Current AI memory systems maintain persistent context through saved memories, conversation summaries, and user preferences, primarily storing factual data. Higher-level reasoning patterns—like explanatory frameworks and reasoning styles—are not typically captured. This post suggests a shift toward modeling how users understand problems rather than just what they know.

**Tags**: `#AI memory`, `#persistent context`, `#machine learning`, `#architecture design`

---

<a id="item-16"></a>
## [QLoRA default learning rate too high for small datasets](https://www.reddit.com/r/MachineLearning/comments/1uy1z8b/the_qlora_2e4_default_is_wrong_under_10k_samples/) ⭐️ 7.0/10

A practitioner reports that the widely-adopted QLoRA default learning rate of 2e-4 causes overfitting on datasets under 10,000 samples, and recommends starting at 1e-4 or lower with more epochs. This challenges a common default that many practitioners copy without tuning, potentially wasting hours of training and evaluation time. The insight is particularly valuable for the growing number of developers fine-tuning models on small, custom datasets. The 2e-4 default originates from the Stanford Alpaca dataset of 52,000 samples, but the author observes that on datasets under 10,000 samples, the model overfits within the first epoch. Lowering the learning rate to 1e-4 and increasing epochs from 3 to 5 improved evaluation metrics significantly.

reddit · r/MachineLearning · /u/Pretty-Ad774 · Jul 16, 12:50

**Background**: QLoRA (Quantized Low-Rank Adaptation) is a fine-tuning technique that reduces memory usage by combining quantization and low-rank adapters, enabling large language model fine-tuning on a single GPU. The default learning rate of 2e-4 was popularized by the Alpaca paper, which fine-tuned on 52,000 instruction-following samples. However, this default may not be optimal for smaller datasets, as the author experienced. Many tutorials and shared notebooks hardcode this value without explaining its context, leading to suboptimal results for users with limited data.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/artidoro/qlora">GitHub - artidoro/qlora: QLoRA: Efficient Finetuning of Quantized LLMs · GitHub</a></li>
<li><a href="https://arxiv.org/abs/2305.14314">[2305.14314] QLoRA: Efficient Finetuning of Quantized LLMs</a></li>
<li><a href="https://github.com/tatsu-lab/stanford_alpaca">GitHub - tatsu-lab/stanford_alpaca: Code and documentation to train Stanford's Alpaca models, and generate the data. · GitHub</a></li>

</ul>
</details>

**Tags**: `#QLoRA`, `#fine-tuning`, `#learning rate`, `#small datasets`, `#overfitting`

---

<a id="item-17"></a>
## [Seeking critical perspectives on JEPA for robot learning world models](https://www.reddit.com/r/MachineLearning/comments/1uxcryc/looking_for_jepa_devil_advocates_r/) ⭐️ 7.0/10

A researcher posted on Reddit asking for devil's advocate arguments against JEPA (Joint Embedding Predictive Architecture) as a world model approach in robot learning, expressing skepticism about Yann LeCun's strong advocacy. JEPA has been proposed as a promising self-supervised learning paradigm for world models, but critical discussion is needed to identify its limitations compared to other approaches like generative models. This debate directly influences the direction of robot learning research. JEPA learns by predicting abstract representations of inputs in an embedding space, rather than reconstructing raw pixels like generative models. The researcher specifically noted that LeCun dismisses LLMs and RL while promoting JEPA as the next big thing, raising concerns about potential overhyping.

reddit · r/MachineLearning · /u/Amazing-Coat5160 · Jul 15, 17:34

**Background**: World models are predictive representations of how environments evolve under actions, supporting planning and policy learning in robotics. JEPA (Joint Embedding Predictive Architecture) is a self-supervised approach proposed by Yann LeCun that learns representations by predicting latent features, avoiding pixel-level reconstruction. It has been applied to video prediction (V-JEPA) and robot learning, with claims of achieving zero-shot control.

<details><summary>References</summary>
<ul>
<li><a href="https://ai.meta.com/research/vjepa/">Introducing V-JEPA 2</a></li>
<li><a href="https://www.turingpost.com/p/jepa">What is Joint Embedding Predictive Architecture (JEPA)?</a></li>
<li><a href="https://arxiv.org/html/2605.00080v1">World Model for Robot Learning: A Comprehensive Survey</a></li>

</ul>
</details>

**Tags**: `#world models`, `#JEPA`, `#robot learning`, `#Yann LeCun`, `#deep learning`

---

<a id="item-18"></a>
## [Novel Method Disentangles Convolutional Neurons via Hadamard Clustering](https://www.reddit.com/r/MachineLearning/comments/1uwya70/mechanistic_interpretability_a_first_paper_on/) ⭐️ 7.0/10

A researcher introduces a technique that uses clustering of Hadamard products between receptive fields and neuron weights to disentangle and analyze a single convolutional neuron in InceptionV1, revealing monosemantic clusters such as cars, cats, and dogs. This work provides a novel, visualizable method for understanding convolutional neural networks at the neuron level, potentially advancing mechanistic interpretability and safety research by enabling fine-grained analysis of learned features. The technique also uncovered low-valued clusters like letters, where dependent neurons fire on the same concept and positive/negative weights are evenly distributed to keep the sum low, suggesting deliberate gradient descent behavior. The analysis is presented with visualizations inspired by the Distill style.

reddit · r/MachineLearning · /u/narang_27 · Jul 15, 06:59

**Background**: Mechanistic interpretability aims to reverse-engineer neural networks by analyzing their internal structures and algorithms. Hadamard product clustering groups elements based on element-wise multiplication of vectors. Previous work focused on language models, but this paper extends interpretability techniques to convolutional neurons.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mechanistic_interpretability">Mechanistic interpretability</a></li>
<li><a href="https://en.wikipedia.org/wiki/Hadamard_product_(matrices)">Hadamard product (matrices) - Wikipedia</a></li>
<li><a href="https://transformer-circuits.pub/2023/monosemantic-features">Towards Monosemanticity: Decomposing Language Models With Dictionary Learning</a></li>

</ul>
</details>

**Tags**: `#mechanistic interpretability`, `#convolutional neural networks`, `#neuron analysis`, `#interpretability`

---

<a id="item-19"></a>
## [LM Studio Bionic: New AI Agent for Open Models Sparks Debate](https://lmstudio.ai/blog/introducing-lm-studio-bionic) ⭐️ 6.0/10

LM Studio has launched Bionic, an AI agent designed to work with open-source large language models, but the application is closed-source and introduces a secure cloud service for accessing frontier open models, marking a shift from its purely local, open-source roots. This matters because it highlights the tension between open model ecosystem ideals and commercial sustainability, potentially influencing how other local LLM tools approach monetization and user trust. Bionic is a closed-source application that leverages both local open models and cloud-based frontier models through LM Studio Secure Cloud, with a stated policy of no data retention or training on user data for cloud connections, though this claim faces skepticism.

hackernews · minimaxir · Jul 16, 20:18 · [Discussion](https://news.ycombinator.com/item?id=48939662)

**Background**: LM Studio is a popular desktop application that allows users to download and run open-source large language models locally on their own hardware, providing a private and user-friendly alternative to cloud-based AI services. An AI agent is a system that can autonomously plan and execute tasks by interacting with models and external tools, often beyond simple chatbot interactions. The introduction of Bionic represents a shift for LM Studio from a purely local inference platform to a hybrid agentic product that incorporates cloud services, raising concerns about its commitment to open-source principles and user privacy.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@kapustinomm/how-to-run-llms-locally-with-lm-studio-complete-guide-2026-c941843e000e">How to Run LLMs Locally with LM Studio : Complete Guide... | Medium</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community comments express skepticism and concern: users worry about the shift to a closed-source business model, the transparency of data handling for cloud models, and whether Bionic offers genuine innovation over existing agent harnesses. Some draw parallels to Apple's approach, suggesting that normal users may eventually adopt platform-native AI solutions instead.

**Tags**: `#AI`, `#LM Studio`, `#open source`, `#LLM`, `#agent`

---

<a id="item-20"></a>
## [Simon Willison ports Grok CLI's Mermaid renderer to WebAssembly](https://simonwillison.net/2026/Jul/16/grok-mermaid/#atom-everything) ⭐️ 6.0/10

Simon Willison created a browser-based tool that converts Mermaid diagram source code into Unicode box art. It uses WebAssembly to run a Rust renderer extracted from the open-sourced Grok CLI codebase. This tool demonstrates a practical way to repurpose terminal rendering code for the web via WebAssembly, making Mermaid diagrams accessible in environments without a JavaScript rendering engine. It also highlights the reusability of components from AI tool codebases. The tool compiles the Rust crate xai-grok-markdown to WebAssembly using wasm-pack. Users can paste Mermaid source code and see the rendered box art output, with options to copy as text or share a link to the diagram.

rss · Simon Willison · Jul 16, 00:33

**Background**: Mermaid is a popular JavaScript-based diagramming tool that generates SVG from text descriptions. Grok CLI is an open-source terminal coding agent from xAI that includes a Rust-based Mermaid renderer for terminal output. WebAssembly (Wasm) allows running compiled code from languages like Rust in web browsers at near-native speed.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/Grok_CLI">Grok CLI</a></li>
<li><a href="https://x.ai/cli">Grok Build | SpaceXAI</a></li>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#mermaid`, `#unicode`, `#webassembly`, `#rust`, `#devtools`

---

<a id="item-21"></a>
## [Reddit user seeks Python tools for multi-objective surrogate-based optimization](https://www.reddit.com/r/MachineLearning/comments/1uxty9v/best_current_tools_for_multiobjective/) ⭐️ 6.0/10

A Reddit user asked for recommendations on the best current tools for multi-objective surrogate-based optimization (MOSBO) on heterogeneous meta-analysis data, specifically for physiological outcomes. This discussion highlights the growing need for specialized optimization tools in meta-analysis, and the community's response can guide researchers toward effective Python-based workflows for complex, constrained multi-objective problems. The user has data from ~40 studies with protocol variables and baseline-dependent outcomes, and requires hierarchical modeling to separate effects, with three optimization objectives and physiological constraints. They prefer Colab-friendly Python tools and mentioned candidates including PyMC, pymoo, pysamoo, SMT, and Matlab.

reddit · r/MachineLearning · /u/BleakReason · Jul 16, 05:43

**Background**: Multi-objective surrogate-based optimization (MOSBO) combines surrogate models (e.g., Gaussian processes) to approximate expensive objective functions with multi-objective optimization algorithms to find trade-offs. PyMC is used for Bayesian hierarchical modeling, pymoo is a multi-objective optimization framework, pysamoo extends pymoo with surrogate assistance, and SMT is a surrogate modeling toolbox. These tools are often used in engineering and scientific optimization.

<details><summary>References</summary>
<ul>
<li><a href="https://pymoo.org/">pymoo : Multi - objective Optimization in Python — pymoo ...</a></li>
<li><a href="https://anyoptimization.com/projects/pysamoo/">pysamoo: Surrogate-Assisted Multi-objective Optimization — pysamoo 0.1 documentation</a></li>
<li><a href="https://github.com/SMTorg/smt">GitHub - SMTorg/smt: Surrogate Modeling Toolbox · GitHub</a></li>

</ul>
</details>

**Tags**: `#multi-objective optimization`, `#surrogate-based optimization`, `#hierarchical modeling`, `#meta-analysis`, `#Python tools`

---