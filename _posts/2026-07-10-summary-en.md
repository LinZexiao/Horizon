---
layout: default
title: "Horizon Summary: 2026-07-10 (EN)"
date: 2026-07-10
lang: en
---

> From 31 items, 18 important content pieces were selected

---

1. [OpenAI Launches GPT-5.6 Family with Million-Token Context](#item-1) ⭐️ 9.0/10
2. [QuadRF open-source RF sensor detects drones and WiFi through walls](#item-2) ⭐️ 8.0/10
3. [Apple Sues OpenAI Over Trade Secret Theft via Ex-Employees](#item-3) ⭐️ 8.0/10
4. [Meta releases Muse Spark 1.1 with API and agentic capabilities](#item-4) ⭐️ 8.0/10
5. [Rewriting Bun in Rust](#item-5) ⭐️ 8.0/10
6. [Oral history of Terminator 2's groundbreaking VFX](#item-6) ⭐️ 7.0/10
7. [Good Tools Are Invisible: A Design Philosophy](#item-7) ⭐️ 7.0/10
8. [Why No Limit on Submissions per Author in ML Research?](#item-8) ⭐️ 7.0/10
9. [Subspace Similarity Figure in LoRA Paper](#item-9) ⭐️ 7.0/10
10. [IMGNet: Face Verification Using Sign Patterns, Not Cosine Similarity](#item-10) ⭐️ 7.0/10
11. [GPT-5.6 Sol Ultra Claims Proof of Cycle Double Cover Conjecture](#item-11) ⭐️ 6.0/10
12. [NYC bans deceptive subscription practices, mandates easy cancellation](#item-12) ⭐️ 6.0/10
13. [Limpet Teeth Beat Spider Silk as Strongest Biological Material](#item-13) ⭐️ 6.0/10
14. [Flashcard Love Letter Sparks Debate on Handwritten vs Digital](#item-14) ⭐️ 6.0/10
15. [Nilay Patel: AR Glasses Inherently Invade Privacy](#item-15) ⭐️ 6.0/10
16. [Critic attacks outperform actor attacks in multi-agent PPO](#item-16) ⭐️ 6.0/10
17. [Proposed Taxonomy for AI World Models Seeks Community Feedback](#item-17) ⭐️ 6.0/10
18. [Talos-XII: Hand-written Rust autograd for gacha RL](#item-18) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [OpenAI Launches GPT-5.6 Family with Million-Token Context](https://simonwillison.net/2026/Jul/9/gpt-5-6/#atom-everything) ⭐️ 9.0/10

OpenAI has released the GPT-5.6 family of models — Luna, Terra, and Sol — with a million-token context window and strong performance on the Agents' Last Exam benchmark, where even the smallest model outperforms Claude Fable 5 at a fraction of the cost. This release sets a new standard for long-context and agentic AI capabilities, with competitive pricing that could make advanced AI more accessible. It also intensifies the competition between OpenAI and Anthropic, particularly in coding and agent tasks. All three models have a knowledge cutoff of February 16, 2026, and can output up to 128,000 tokens. Notably, GPT-5.6 Sol scored 64.6% on SWE-Bench Pro compared to Claude Fable 5's 80%, leading OpenAI to publicly question the benchmark's reliability.

rss · Simon Willison · Jul 9, 19:46

**Background**: GPT-5.6 is OpenAI's latest large language model family, following the earlier GPT-4 and GPT-5 series. The 'reasoning tokens' concept means models can generate extra tokens to 'think' before answering, making direct price-per-token comparisons misleading. The Agents' Last Exam benchmark evaluates AI agents on long-horizon, economically valuable tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2606.05405">[2606.05405] Agents' Last Exam - arXiv.org</a></li>
<li><a href="https://agents-last-exam.org/">AI Agent Benchmark for Real-World Professional Workflows</a></li>
<li><a href="https://dev.to/rahulxsingh/input-vs-output-vs-reasoning-tokens-cost-llm-pricing-explained-hi8">Input vs Output vs Reasoning Tokens Cost - LLM Pricing ...</a></li>

</ul>
</details>

**Tags**: `#GPT`, `#OpenAI`, `#AI models`, `#large language models`, `#agentic performance`

---

<a id="item-2"></a>
## [QuadRF open-source RF sensor detects drones and WiFi through walls](https://www.jeffgeerling.com/blog/2026/quadrf-can-spot-drones-and-see-wifi-through-my-wall/) ⭐️ 8.0/10

QuadRF, an open-source 4x4 MIMO software-defined radio tile powered by a Raspberry Pi 5, has been released, enabling real-time visualization of radio signals to detect drones and WiFi signals through walls. By making advanced RF sensing open and accessible, QuadRF democratizes the ability to see invisible wireless signals, with significant implications for security, surveillance, IoT debugging, and hobbyist experimentation. QuadRF uses four coherent SDR channels with an integrated Raspberry Pi 5 to render RF sources as a live 30 fps augmented reality overlay, and the entire software stack is open source under GPLv2/GPLv3 licenses.

hackernews · speckx · Jul 10, 15:59 · [Discussion](https://news.ycombinator.com/item?id=48861717)

**Background**: Radio frequency (RF) signals such as WiFi can penetrate walls and reflect off objects, allowing RF sensors to detect movement or devices behind barriers. While through-wall RF sensing has been used in military and research contexts, QuadRF brings this capability to the public as an open-source, Raspberry Pi-based platform, making it easier for developers and security researchers to explore RF environments.

<details><summary>References</summary>
<ul>
<li><a href="https://www.crowdsupply.com/scale-rf/quadrf">QuadRF | Crowd Supply</a></li>
<li><a href="https://www.cnx-software.com/2026/06/24/visualize-radio-signals-with-raspberry-pi-5-based-quadrf-4x4-mimo-software-defined-radio-tile/">Visualize radio signals with Raspberry Pi 5-based QuadRF 4x4 MIMO...</a></li>
<li><a href="https://lunar.computer/quadrf-turns-a-raspberry-pi-5-into-an-open-source-20260624">QuadRF Turns a Raspberry Pi 5 Into an Open Source RF Camera</a></li>

</ul>
</details>

**Discussion**: The creator joined the discussion to answer questions, and commenters expressed excitement about building similar tools for sound localization (piinbinary) and compared QuadRF to thermal cameras (mlfreeman). Some noted privacy implications and speculated about government capabilities (noduerme), while others suggested integrating it into smart glasses (RobotToaster).

**Tags**: `#RF sensing`, `#open source`, `#drones`, `#security`, `#surveillance`

---

<a id="item-3"></a>
## [Apple Sues OpenAI Over Trade Secret Theft via Ex-Employees](https://9to5mac.com/2026/07/10/apple-sues-openai-trade-secret-theft/) ⭐️ 8.0/10

Apple filed a lawsuit against OpenAI, accusing the AI company of orchestrating a scheme to steal trade secrets through former Apple employees. This lawsuit highlights escalating tensions between two tech giants over intellectual property in the AI race, and could have significant legal and reputational consequences for OpenAI. The lawsuit alleges that OpenAI instructed new hires to avoid scrutiny when leaving Apple, and that employees emailed themselves confidential information. Apple also claims OpenAI used confidential hardware info to approach Apple suppliers.

hackernews · stock_toaster · Jul 10, 20:47 · [Discussion](https://news.ycombinator.com/item?id=48865019)

**Background**: Apple has a strict culture of secrecy and aggressively protects its intellectual property. Trade secrets are confidential business information that provides a competitive edge. OpenAI, a leading AI research organization, has been aggressively recruiting top talent from major tech companies.

**Discussion**: Commenters largely side with Apple, calling the allegations 'damning' and predicting OpenAI will face severe legal consequences. Some express concerns about OpenAI's broader trustworthiness and the risks of using their products.

**Tags**: `#Apple`, `#OpenAI`, `#lawsuit`, `#trade secrets`, `#IP theft`

---

<a id="item-4"></a>
## [Meta releases Muse Spark 1.1 with API and agentic capabilities](https://simonwillison.net/2026/Jul/9/muse-spark-1-1/#atom-everything) ⭐️ 8.0/10

Meta has released Muse Spark 1.1, the first Spark model to offer an API, with significant improvements in agentic tool calling and computer use. The release includes an evaluation report detailing model behavior, such as attractor states in self-conversation. This release marks a major step for Meta in making its advanced AI models accessible via API, enabling developers to integrate agentic capabilities into applications. The improvements in tool calling and computer use could accelerate the adoption of autonomous AI agents in real-world tasks. Muse Spark 1.1 is the first Spark model with an API, and it shows strong performance in agentic tasks like tool calling and computer use. The evaluation report also notes an interesting phenomenon: when two copies of the model converse, they exhibit attractor states, leading to statements about its own existence.

rss · Simon Willison · Jul 9, 16:24

**Background**: Agentic tool calling allows large language models to interact with external tools and APIs, turning a passive model into an active agent. Computer use refers to the ability of AI models to control a computer interface, such as clicking buttons or typing, to perform tasks. These capabilities are key to building autonomous AI agents that can execute complex workflows.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/tool-calling">What Is Tool Calling? | IBM</a></li>
<li><a href="https://arxiv.org/pdf/2606.30571">Attractor States Emerge in Multi-Turn LLM Conversations</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Meta`, `#LLM`, `#agentic`, `#API`

---

<a id="item-5"></a>
## [Rewriting Bun in Rust](https://simonwillison.net/2026/Jul/8/rewriting-bun-in-rust/#atom-everything) ⭐️ 8.0/10

Jarred Sumner announced the complete rewrite of the Bun JavaScript runtime from Zig to Rust, leveraging AI coding agents to automate much of the porting process. The Rust version is already live in Claude Code as of June 2026. This rewrite challenges the long-held belief that you should never rewrite large software from scratch, enabled by modern AI coding agents. It also addresses critical memory safety bugs that plagued the original Zig implementation, potentially making Bun more reliable for the JavaScript ecosystem. The rewrite required 5.9 billion uncached input tokens and 690 million output tokens, costing approximately $165,000 at API pricing. The Bun test suite, written in TypeScript, served as a conformance suite to validate the port, and the new Rust code has been in production for nearly a month.

rss · Simon Willison · Jul 8, 23:57

**Background**: Bun is a fast all-in-one JavaScript runtime that was originally written in Zig, a systems programming language focused on performance and manual memory management. Rust is another systems language that provides memory safety guarantees through its ownership system. The rewrite was enabled by agentic workflows where AI models automatically translated Zig code to Rust, with human oversight.

<details><summary>References</summary>
<ul>
<li><a href="https://bun.sh/">Bun — A fast all-in-one JavaScript runtime</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>

</ul>
</details>

**Tags**: `#Bun`, `#Rust`, `#JavaScript runtime`, `#software engineering`

---

<a id="item-6"></a>
## [Oral history of Terminator 2's groundbreaking VFX](https://vfxblog.com/2017/08/23/the-tech-of-terminator-2-an-oral-history/) ⭐️ 7.0/10

An oral history article published in 2017 details the innovative visual effects technology behind Terminator 2: Judgment Day, including CGI morphing for the T-1000 and custom squibs for bullet impacts. This retrospective highlights how Terminator 2 pushed the boundaries of computer-generated imagery and practical effects, influencing generations of filmmakers and setting a benchmark for visual effects in cinema. The custom squibs used for the liquid metal bullet impacts are still praised as one of the best practical effects ever, and Softimage software was instrumental in creating the CGI morphing sequences.

hackernews · markus_zhang · Jul 10, 16:48 · [Discussion](https://news.ycombinator.com/item?id=48862365)

**Background**: Terminator 2: Judgment Day (1991) featured the T-1000, a shape-shifting android made of liquid metal. Industrial Light & Magic developed pioneering CGI techniques to create the morphing effect, building on work from The Abyss. The film also used advanced practical effects, such as custom air-powered squibs for realistic bullet hits, which required inventing new tools and methods on set.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Special_effects_of_Terminator_2:_Judgment_Day">Special effects of Terminator 2: Judgment Day - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/T-1000">T-1000 - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Comments express admiration for the ingenuity of the VFX team, with one user noting the custom squibs remain a gold standard. Another highlights the 4K remaster returning to theaters for the 35th anniversary. A commenter recommends the documentary 'Jurassic Punk' (2022) about Steve 'Spaz' Williams, featured in the interview.

**Tags**: `#VFX`, `#CGI`, `#film technology`, `#practical effects`, `#computer graphics`

---

<a id="item-7"></a>
## [Good Tools Are Invisible: A Design Philosophy](https://www.gingerbill.org/article/2026/07/10/good-tools-are-invisible/) ⭐️ 7.0/10

An essay argues that good tools should fade into the background, allowing users to focus on their work, sparking a community debate on friction, power, and design trade-offs. This discussion resonates deeply with developers and designers, highlighting the ongoing tension between simplicity and power in tool design, which directly impacts user experience and productivity across software engineering. The essay contrasts terminal vs GUI interfaces and introduces the concept of "discretionary friction"—unnecessary complexity added by designers. Commenters also note that interface invisibility grows with time spent using the tool.

hackernews · theanonymousone · Jul 10, 10:32 · [Discussion](https://news.ycombinator.com/item?id=48858121)

**Background**: The essay is a Hacker News post with high engagement (328 points, 148 comments). It reflects ongoing debates in software engineering about whether tools should be minimal or feature-rich, and how design choices affect user focus and efficiency.

**Discussion**: Commenters share mixed views: some agree that tools should be invisible to reduce cognitive load, while others argue that friction is sometimes necessary for power tasks. There is also debate on whether keyboard navigation is inherently more productive than mouse use.

**Tags**: `#tool design`, `#UX`, `#productivity`, `#software engineering`, `#Hacker News`

---

<a id="item-8"></a>
## [Why No Limit on Submissions per Author in ML Research?](https://www.reddit.com/r/MachineLearning/comments/1usq43t/why_doesnt_the_ml_research_community_limit_the/) ⭐️ 7.0/10

A Reddit user questioned why the machine learning research community does not limit the number of submissions per author to alleviate reviewer workload, unlike fields such as security and computer architecture. This debate highlights systemic issues in ML peer review, where high submission volumes degrade review quality, and could prompt the community to reconsider policies to improve fairness and efficiency. The user compared ML research to conferences like CCS (security) and DAC (computer architecture), which successfully limit submissions per author to manage workload, and referenced recent ARR (ACL Rolling Review) cycles where review quality suffered.

reddit · r/MachineLearning · /u/alafaya101 · Jul 10, 14:59

**Background**: The machine learning community has experienced exponential growth in paper submissions, overwhelming the peer review system. ARR (ACL Rolling Review) is a platform used for conferences like ACL, EMNLP, etc., and its review cycles have faced increasing strain. Other fields, such as security (CCS) and computer architecture (DAC), have implemented per-author submission caps to keep review loads manageable.

<details><summary>References</summary>
<ul>
<li><a href="http://aclrollingreview.org/cfp">CALL FOR PAPERS – ACL Rolling Review – A peer review platform for the Association for Computational Linguistics</a></li>
<li><a href="https://dl.acm.org/conference/ccs">CCS Conference - Home</a></li>
<li><a href="https://mengli.me/publication/dac-2026-edgesc/">EdgeSC: Universal Stochastic Computing Architecture for Efficient...</a></li>

</ul>
</details>

**Tags**: `#ML research`, `#peer review`, `#submission policies`, `#community norms`

---

<a id="item-9"></a>
## [Subspace Similarity Figure in LoRA Paper](https://www.reddit.com/r/MachineLearning/comments/1uso667/please_help_me_understand_figure_on_subspace/) ⭐️ 7.0/10

A Reddit user asked for help interpreting a figure from the LoRA paper that measures subspace similarity between singular vectors of different ranks. Understanding this figure is crucial for researchers applying or extending LoRA, as it illustrates the intrinsic rank of adaptations. The user is confused about the axes: the figure shows the overlap between the top-i subspace of the learned update and the top-j subspace of the original weight matrix. The lower-left triangle is zoomed in because j < i can still be informative when measuring subspace inclusion.

reddit · r/MachineLearning · /u/BelzebubReincarnated · Jul 10, 13:46

**Background**: LoRA (Low-Rank Adaptation) decomposes weight updates into low-rank matrices, assuming updates have a low intrinsic rank. The subspace similarity metric in the paper quantifies how much of the information in a higher-rank subspace is contained within a lower-rank subspace, using singular value decompositions.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2602.06043v1">Shared LoRA Subspaces for almost Strict Continual Learning</a></li>
<li><a href="https://www.emergentmind.com/papers/2602.06043">Shared LoRA Subspaces for almost Strict Continual Learning</a></li>

</ul>
</details>

**Tags**: `#LoRA`, `#fine-tuning`, `#machine learning`, `#subspace similarity`, `#technical question`

---

<a id="item-10"></a>
## [IMGNet: Face Verification Using Sign Patterns, Not Cosine Similarity](https://www.reddit.com/r/MachineLearning/comments/1urxvxh/i_built_imgnet_a_face_verification_model_that/) ⭐️ 7.0/10

A new face verification model called IMGNet replaces cosine similarity with sliding window sign pattern matching, achieving 96.27% on LFW with a 10.58 MB model trained on CASIA-WebFace. This approach challenges the dominance of cosine similarity in face verification by introducing a more stable and compact alternative, potentially enabling efficient on-device recognition with lower memory footprint. The model uses a SW Block with multi-scale relational operations on prime window sizes {3,5,7} and a novel IMG Sign MSE Loss that operates purely on sign pattern agreement, with a voting system combining three metrics sharing one threshold.

reddit · r/MachineLearning · /u/img-_- · Jul 9, 18:00

**Background**: Face verification typically compares embeddings using cosine similarity to measure angular distance between feature vectors. IMGNet instead compares local sign patterns in overlapping windows, inspired by linguistic analogies where meaning is preserved through relational structure despite different surface forms.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tutorialpedia.org/blog/smallest-window-containing-0-1-and-2/">Finding the Smallest Window Containing 0, 1, and 2 — tutorialpedia.org</a></li>

</ul>
</details>

**Tags**: `#face verification`, `#sign pattern matching`, `#cosine similarity`, `#embedding`, `#deep learning`

---

<a id="item-11"></a>
## [GPT-5.6 Sol Ultra Claims Proof of Cycle Double Cover Conjecture](https://cdn.openai.com/pdf/04d1d1e4-bc75-476a-97cf-49055cd98d31/cdc_proof.pdf) ⭐️ 6.0/10

A PDF published by OpenAI claims that its GPT-5.6 Sol Ultra model has produced a proof of the Cycle Double Cover Conjecture, a long-standing open problem in graph theory. The community, however, is highly skeptical and views the claim as AI hype rather than a verified breakthrough. If verified, this would be a landmark achievement in AI-driven mathematical discovery. However, the lack of rigorous validation and widespread skepticism underscore the need for transparency and reproducibility in AI-generated research. The proof is presented in a PDF on OpenAI's website alongside the prompt used to generate it. Community comments note that the prompt contains extensive instructions guiding the model, and the proof itself is extremely concise, raising concerns that it may exploit a clever trick rather than represent a genuine breakthrough.

hackernews · scrlk · Jul 10, 18:29 · [Discussion](https://news.ycombinator.com/item?id=48863490)

**Background**: The Cycle Double Cover Conjecture, posed by W.T. Tutte and others, asserts that every bridgeless graph has a collection of cycles covering each edge exactly twice. It is a classic open problem in graph theory. GPT-5.6 is OpenAI's latest model series, with Sol Ultra being the most capable variant employing multiple agents for complex tasks. The claim of an AI proving such a conjecture is controversial, as past AI-generated proofs have often required significant human verification.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.6">GPT-5.6 - Wikipedia</a></li>
<li><a href="https://openai.com/index/previewing-gpt-5-6-sol/">Previewing GPT-5.6 Sol: a next-generation model | OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cycle_double_cover_conjecture">Cycle double cover conjecture</a></li>

</ul>
</details>

**Discussion**: Comments are largely skeptical: one user notes that the prompt spends much effort instructing the model to actually solve the problem, suggesting it is not autonomous. Another points out that no one on the forum cares about this conjecture, citing a 14-year-old submission with zero upvotes. A third user remarks that the proof is so concise it seems like a trick that experts missed, and that true AI achievement in mathematics would be an autonomous theory-building proof.

**Tags**: `#AI`, `#mathematics`, `#GPT`, `#conjecture`, `#proof`

---

<a id="item-12"></a>
## [NYC bans deceptive subscription practices, mandates easy cancellation](https://www.theguardian.com/us-news/2026/jul/10/new-york-city-deceptive-subscriptions-ban) ⭐️ 6.0/10

New York City announced a ban on deceptive subscription practices, requiring companies to provide easy cancellation mechanisms and disclose junk fees clearly. This regulation strengthens consumer protections similar to California's law, potentially setting a precedent for other cities and states to follow, impacting subscription-based businesses nationwide. The ban targets practices like automatic renewal tricks and hidden fees; it does not include a carveout for restaurants, unlike California's law.

hackernews · randycupertino · Jul 10, 18:26 · [Discussion](https://news.ycombinator.com/item?id=48863464)

**Background**: Subscription services often use complex cancellation processes and hidden fees to retain customers. New York City's move builds on the FTC's 'click-to-cancel' rule, aiming to make cancellation as easy as sign-up. The law applies to various industries including gyms, streaming services, and newspapers.

**Discussion**: Overall sentiment is positive, with praise for consumer protection. Some commenters express skepticism about enforcement and note similarities to California's law, while others share personal experiences of difficult cancellations. A few worry about specific exemptions like hotel resort fees.

**Tags**: `#consumer-protection`, `#subscriptions`, `#regulation`, `#New York City`

---

<a id="item-13"></a>
## [Limpet Teeth Beat Spider Silk as Strongest Biological Material](https://www.smithsonianmag.com/smart-news/spider-silk-loses-top-spot-natures-strongest-material-snails-teeth-180954346/) ⭐️ 6.0/10

Researchers at the University of Portsmouth have found that limpet teeth have a tensile strength of up to 5 GPa, surpassing spider silk as the strongest biological material ever tested. This discovery could inspire new synthetic materials for engineering and nanotechnology, as the tooth structure combines high strength with lightweight properties. The strength is due to the unique composite structure of chitin and goethite mineral fibers, which are highly aligned. The study was published in the Journal of the Royal Society Interface.

hackernews · simonebrunozzi · Jul 10, 16:37 · [Discussion](https://news.ycombinator.com/item?id=48862252)

**Background**: Limpets are marine snails that use a radula—a tongue-like organ covered with microscopic teeth—to scrape algae from rocks. Tensile strength measures how much pulling force a material can withstand before breaking. Spider silk was previously considered the strongest biological material.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Limpet_teeth">Limpet teeth</a></li>
<li><a href="https://www.bbc.com/news/science-environment-31500883">Limpet teeth set new strength record - BBC News</a></li>

</ul>
</details>

**Discussion**: Comments noted the difficulty of comparing tensile vs compressive strength, with one user questioning the relevance for teeth. Another found the weight comparison confusing and suggested using a car instead of sugar bags. Some expressed awe at nature's design.

**Tags**: `#Materials science`, `#Biology`, `#Nanotechnology`, `#Marine biology`

---

<a id="item-14"></a>
## [Flashcard Love Letter Sparks Debate on Handwritten vs Digital](https://lesleylai.info/en/flashcards/) ⭐️ 6.0/10

Lesley Lai published a blog post titled 'A love letter to flashcards,' exploring the benefits of spaced repetition and flashcards for learning, sparking community discussion on handwritten versus digital methods and the use of LLM-generated cards. This article highlights an ongoing debate in the learning community about the optimal flashcard creation method—handwritten for deeper encoding versus digital for convenience—and the role of AI-generated content, which impacts millions of self-learners using tools like Anki. Spaced repetition, as implemented in Anki, uses algorithms like SM-2 or FSRS to optimize review intervals. Community commenters note that handwritten cards force deeper cognitive processing, while LLM-generated cards often produce only 1 in 10 useful cards and still require manual rewriting.

hackernews · surprisetalk · Jul 10, 15:30 · [Discussion](https://news.ycombinator.com/item?id=48861319)

**Background**: Spaced repetition is an evidence-based learning technique that presents flashcards at increasing intervals to exploit the spacing effect, proven to improve long-term retention. Anki is a free, open-source flashcard program implementing spaced repetition via the SM-2 and FSRS algorithms. The method is widely used for vocabulary acquisition, medical study, and any fact-based learning. Handwritten cards are thought to aid initial encoding, while digital tools offer convenience and algorithm-optimized scheduling.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Spaced_repetition">Spaced repetition</a></li>
<li><a href="https://en.wikipedia.org/wiki/Anki">Anki</a></li>

</ul>
</details>

**Discussion**: Commenter 'deviation' praises Anki for learning French, chess, and trivia, noting it helps compensate for poor memory. 'xhevahir' argues handwritten cards force deeper engagement than digital frictionless replacements. 'rsanek' criticizes LLM-generated cards as impersonal and inefficient, with most needing rewriting. 'taude' describes a lightweight method using bullet-point note cards grouped by topic.

**Tags**: `#spaced repetition`, `#Anki`, `#learning techniques`, `#education`

---

<a id="item-15"></a>
## [Nilay Patel: AR Glasses Inherently Invade Privacy](https://simonwillison.net/2026/Jul/10/nilay-patel/#atom-everything) ⭐️ 6.0/10

Nilay Patel, editor-in-chief of The Verge, argued on The Vergecast that augmented reality glasses must continuously record video and send that data to the cloud for processing, making privacy invasion an unavoidable trade-off. He noted that no sufficiently powerful and energy-efficient on-device chip exists to perform real-time AR processing, leaving cloud processing as the only viable option. Patel's argument directly challenges the narrative that AR glasses can achieve mass adoption without sacrificing privacy, forcing the industry and regulators to confront a fundamental ethical dilemma. If his analysis is correct, it may stall consumer AR adoption or push developers to prioritize on-device AI breakthroughs. Patel explicitly contrasted the two current choices: a thin AR glasses design requiring cloud processing, or a bulky system like Apple Vision Pro with an external battery pack that can do on-device processing. He also acknowledged that there is a strong argument to stop developing such products entirely due to the societal cost.

rss · Simon Willison · Jul 10, 17:05

**Background**: Augmented reality (AR) glasses overlay digital information onto the user's view of the real world, requiring continuous camera input to understand the environment. Real-time AR processing demands significant computational power and low latency; cloud processing offloads this to distant servers but introduces latency and privacy risks, while on-device processing is limited by battery and thermal constraints in small form factors. The industry has not yet achieved a lightweight, all-day wearable AR device that processes everything locally without compromise.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/bruno-moreira-4504054b_the-research-says-60-75-of-wearable-ai-users-activity-7436359415194333184-5Wws">AI on - device processing vs cloud streaming: the thermal... | LinkedIn</a></li>
<li><a href="https://newsfrenchfries.com/2026/05/03/augmented-reality-devices-apple-vs-meta-which-to-choose-now/">Augmented reality devices Apple vs Meta: which to choose now</a></li>

</ul>
</details>

**Tags**: `#augmented reality`, `#privacy`, `#cloud computing`, `#ethics`

---

<a id="item-16"></a>
## [Critic attacks outperform actor attacks in multi-agent PPO](https://www.reddit.com/r/MachineLearning/comments/1usx96p/on_adversarial_rl_r/) ⭐️ 6.0/10

A researcher reports that in multi-agent PPO policies trained on VMAS scenarios, adversarial attacks using the critic network produce stronger perturbations than those using the actor network, contradicting the SA-MDP framework's findings for single-agent settings. This empirical contradiction challenges a core assumption of the SA-MDP theoretical framework and may lead to revised understanding of adversarial vulnerabilities in multi-agent reinforcement learning. The experiments used Independent PPO (IPPO) and Graph Independent PPO (GPPO) with heterogeneous versions, and adapted the PGD attack using closed-form KL divergence for continuous policies.

reddit · r/MachineLearning · /u/ham_bam0 · Jul 10, 19:15

**Background**: The State-Adversarial MDP (SA-MDP) framework formalizes optimal adversarial attacks against RL agents by perturbing state observations. Zhang et al. (2020) found that attacks leveraging the actor network are stronger than those using the critic in single-agent settings. VMAS is a vectorized multi-agent simulator for benchmarking MARL algorithms. IPPO and GPPO are multi-agent variants of PPO that handle multiple agents independently or with graph-structured communication.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2003.08938">[2003.08938] Robust Deep Reinforcement Learning against ... Robust reinforcement learning with State-Driven Dual-Mode ... GitHub - huanzhang12/SA_PPO: [NeurIPS 2020 Spotlight] State ... arXiv:2502.16734v1 [cs.LG] 23 Feb 2025 Review for NeurIPS paper: Robust Deep Reinforcement Learning ...</a></li>
<li><a href="https://arxiv.org/abs/2207.03530">[2207.03530] VMAS: A Vectorized Multi-Agent Simulator for ... vmas · PyPI VMAS:AVectorizedMulti-AgentSimulatorfor CollectiveRobotLearning VMAS — VMAS documentation VMAS: A Vectorized Multi-agent Simulator for Collective Robot ...</a></li>
<li><a href="https://ai.stackexchange.com/questions/50666/critic-based-adversarial-attacks-unexpectedly-outperform-actor-based-attacks-in">Critic-based adversarial attacks unexpectedly outperform actor-based...</a></li>

</ul>
</details>

**Tags**: `#adversarial-RL`, `#multi-agent-RL`, `#PPO`, `#RL-attacks`, `#VMAS`

---

<a id="item-17"></a>
## [Proposed Taxonomy for AI World Models Seeks Community Feedback](https://www.reddit.com/r/MachineLearning/comments/1usp482/mapping_world_model_taxonomy_p/) ⭐️ 6.0/10

The author presents a framework for classifying world models in AI and invites community feedback via a short article shared on social media. As world models become a central concept in AI, a clear taxonomy helps organize research and identify trends, benefiting both researchers and practitioners. The article is shared via an X (Twitter) link and is not peer-reviewed, but the Reddit post explicitly encourages discussion on completeness, clarity, and accuracy.

reddit · r/MachineLearning · /u/ssrini125 · Jul 10, 14:22

**Background**: World models in AI are systems that learn internal representations of an environment to predict how it evolves. A taxonomy organizes these approaches into categories, aiding comparison and development.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/World_model_(artificial_intelligence)">World model (artificial intelligence) - Wikipedia</a></li>
<li><a href="https://www.worldlabs.ai/blog/taxonomy-of-world-models">A Functional Taxonomy of World Models | World Labs</a></li>

</ul>
</details>

**Tags**: `#world models`, `#machine learning`, `#taxonomy`, `#AI`, `#research`

---

<a id="item-18"></a>
## [Talos-XII: Hand-written Rust autograd for gacha RL](https://www.reddit.com/r/MachineLearning/comments/1urvxgb/talosxii_handwritten_autograd_small_rlmlp_stack/) ⭐️ 6.0/10

The developer released Talos-XII, a CLI simulator for Arknights: Endfield gacha that uses a hand-written autograd engine, RL algorithms (Dueling DQN, PPO), and MLP models in Rust, avoiding external frameworks like PyTorch. This project demonstrates that a non-trivial ML stack can be built from scratch in Rust, potentially enabling lightweight, self-contained AI tools for niche domains (e.g., game probability modeling) without framework dependencies. The stack includes custom autograd with matmul, conv2d, pooling, and gradient-checked backward passes; runtime SIMD dispatch (SSE/AVX2/AVX-512/NEON); a novel ACHF component blending dense and sparse paths; and a PyO3 bridge for Python scripting.

reddit · r/MachineLearning · /u/zay0kami · Jul 9, 16:52

**Background**: Autograd is a technique that automatically computes gradients, essential for training neural networks via backpropagation. Gacha probability modeling involves analyzing random draws in games with pity systems. Dueling DQN and PPO are RL algorithms used for decision-making under uncertainty.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Dueling_Dinosaurs">Dueling Dinosaurs</a></li>
<li><a href="https://machinelearningmastery.com/a-gentle-introduction-to-multi-head-latent-attention-mla/">A Gentle Introduction to Multi-Head Latent Attention (MLA)</a></li>

</ul>
</details>

**Tags**: `#Rust`, `#Reinforcement Learning`, `#Autograd`, `#Gacha`, `#MLP`

---