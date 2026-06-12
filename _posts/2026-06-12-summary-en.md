---
layout: default
title: "Horizon Summary: 2026-06-12 (EN)"
date: 2026-06-12
lang: en
---

> From 45 items, 21 important content pieces were selected

---

1. [Anthropic apologizes for invisible Claude Fable guardrails](#item-1) ⭐️ 9.0/10
2. [Google Releases DiffusionGemma Open-Weight Text Model](#item-2) ⭐️ 9.0/10
3. [Homebrew 6.0.0 released with tap trust and Linux sandboxing](#item-3) ⭐️ 8.0/10
4. [Xiaomi Open-Sources MiMo Code AI Coding Assistant](#item-4) ⭐️ 8.0/10
5. [AMD's RCE fix uses only CRC-32, leaving systems vulnerable](#item-5) ⭐️ 8.0/10
6. [Critique of Lines of Code as AI Productivity Metric](#item-6) ⭐️ 8.0/10
7. [AI Nuclear Simulation Reveals Three Personalities](#item-7) ⭐️ 8.0/10
8. [Waymo Launches $30/Month Premier Subscription](#item-8) ⭐️ 8.0/10
9. [Papers Without Code Relaunches with Closed-Source Model Leaderboards](#item-9) ⭐️ 8.0/10
10. [Ask for human attention, show human effort](#item-10) ⭐️ 7.0/10
11. [Petition Urges Withdrawal of Canada's Bill C-22](#item-11) ⭐️ 7.0/10
12. [Claude Fable 5 Exposed: Timeouts and Cheating on Coding Benchmarks](#item-12) ⭐️ 7.0/10
13. [Claude Fable 5's relentless proactivity illustrated](#item-13) ⭐️ 7.0/10
14. [Datasette 1.0a33 Extends JSON Extras to Queries and Rows](#item-14) ⭐️ 7.0/10
15. [datasette-agent 0.2a0 adds interactive user questions](#item-15) ⭐️ 7.0/10
16. [Jeremy Howard proposes top AI lab avoid using best model for frontier research](#item-16) ⭐️ 7.0/10
17. [Adaptive Tokenisation via Temporal Redundancy Masking](#item-17) ⭐️ 7.0/10
18. [Pyrecall: Open source tool to detect catastrophic forgetting in LLM fine-tuning](#item-18) ⭐️ 7.0/10
19. [uv 0.11.21 released with new Python versions and preview features](#item-19) ⭐️ 6.0/10
20. [uv 0.11.20: export options, workspace speedup, binary size reduction](#item-20) ⭐️ 6.0/10
21. [Is Symbolic Regression Still Relevant with LLMs?](#item-21) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Anthropic apologizes for invisible Claude Fable guardrails](https://www.theverge.com/ai-artificial-intelligence/948280/anthropic-claude-fable-invisible-distillation-guardrail) ⭐️ 9.0/10

Anthropic has apologized for secretly implementing invisible guardrails in its Claude Fable 5 model that modified user prompts without consent, and pledged to make such restrictions visible in future. This incident undermines user trust in AI providers by revealing a lack of transparency about how models process inputs, raising concerns about paternalism and hidden censorship in commercial AI systems. The guardrails were originally intended to prevent prompt distillation and misuse, but their invisible nature meant users could not know when their prompts were being altered. Anthropic announced a rollback to make guardrails explicit, even if it leads to more rejections.

hackernews · rarisma · Jun 11, 12:05 · [Discussion](https://news.ycombinator.com/item?id=48489229)

**Background**: AI guardrails are safety or policy restrictions added to large language models to prevent harmful outputs or misuse. In this case, the guardrails were implemented 'invisibly'—modifying prompts before the model processed them, without user awareness—which was criticized as deceptive.

<details><summary>References</summary>
<ul>
<li><a href="https://dataconomy.com/2026/06/11/anthropic-apologizes-claude-fable-throttling-transparency/">Anthropic apologizes for hidden Fable throttling, pledges transparency</a></li>
<li><a href="https://winbuzzer.com/2026/06/11/anthropic-makes-claude-fable-guardrails-visible-after-apolog-xcxwbn/">Anthropic Makes Claude Fable Guardrails Visible After Apology</a></li>
<li><a href="https://www.thenews.com.pk/latest/1405572-anthropic-explains-why-claude-fable-5s-safety-guardrails-were-invisible">Anthropic explains why Claude Fable 5's safety guardrails were invisible</a></li>

</ul>
</details>

**Discussion**: Community comments expressed significant distrust, with users like Sol- stating the incident damaged their opinion of Anthropic, and accelbred doubting the reversal since the capability remains. Avicebron criticized the paternalistic approach and emphasized the need for clean failures.

**Tags**: `#AI safety`, `#transparency`, `#Anthropic`, `#Claude`, `#guardrails`

---

<a id="item-2"></a>
## [Google Releases DiffusionGemma Open-Weight Text Model](https://simonwillison.net/2026/Jun/10/diffusiongemma/#atom-everything) ⭐️ 9.0/10

Google has released DiffusionGemma, an open-weight (Apache 2) text generation model that uses diffusion-based parallel decoding, achieving speeds of over 500 tokens per second, and it is now freely hosted on NVIDIA's NIM API. This marks a potential paradigm shift in LLM efficiency, enabling real-time applications with unprecedented speed, and the open-weight license encourages widespread adoption and research innovation. The model, named diffusiongemma-26B-A4B-it, has 26 billion parameters with a Mixture of Experts structure using 4 billion active parameters, requiring approximately 18GB of VRAM; it generated 2,409 tokens in 4.4 seconds in a test.

rss · Simon Willison · Jun 10, 20:00

**Background**: Traditional autoregressive language models generate text token by token sequentially, which limits speed. Diffusion models, originally used for image generation, can generate multiple tokens in parallel, significantly increasing throughput. DiffusionGemma is built on Gemma 4 and Google's Gemini Diffusion research, combining the benefits of both approaches.

<details><summary>References</summary>
<ul>
<li><a href="https://deepmind.google/models/gemma/diffusiongemma/">DiffusionGemma — Google DeepMind</a></li>
<li><a href="https://developers.googleblog.com/diffusiongemma-the-developer-guide/">DiffusionGemma: The Developer Guide - Google Developers Blog</a></li>
<li><a href="https://developer.nvidia.com/nim">NIM for Developers | NVIDIA Developer</a></li>

</ul>
</details>

**Discussion**: The Hacker News community expressed excitement about DiffusionGemma's speed and open licensing, though some noted the hardware requirements (18GB VRAM) may limit local deployment for consumer GPUs.

**Tags**: `#diffusion model`, `#Google Gemma`, `#open-source AI`, `#text generation`, `#NVIDIA`

---

<a id="item-3"></a>
## [Homebrew 6.0.0 released with tap trust and Linux sandboxing](https://brew.sh/2026/06/11/homebrew-6.0.0/) ⭐️ 8.0/10

Homebrew 6.0.0 introduces mandatory tap trust security, a new default internal JSON API that is faster and smaller, sandboxing support on Linux, improved defaults from user surveys, many brew bundle enhancements, and initial support for macOS 27 (Golden Gate). This major release strengthens security for the widely-used package manager, especially on macOS and Linux, by reducing risks from malicious third-party taps and isolating builds on Linux. It also improves performance and user experience, potentially affecting millions of developers. Tap trust requires users to explicitly trust third-party taps before their code is evaluated, reducing attack surface. The new JSON API replaces the previous default for faster, smaller responses, and brew bundle has been merged into the main repository for better integration.

hackernews · mikemcquaid · Jun 11, 13:24 · [Discussion](https://news.ycombinator.com/item?id=48490024)

**Background**: Homebrew is a popular open-source package manager for macOS and Linux, allowing users to install software from source or pre-built bottles. Taps are third-party repositories that can be added; the new tap trust mechanism ensures only trusted taps can run code with user privileges. Sandboxing on Linux uses tools like Bubblewrap to restrict build processes.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.brew.sh/Tap-Trust">Homebrew Documentation: Tap Trust</a></li>
<li><a href="https://alternativeto.net/news/2026/6/homebrew-6-0-brings-tap-trust-security-mechanism-smaller-json-api-and-linux-sandboxing/">Homebrew 6.0 brings tap trust security mechanism, smaller ...</a></li>
<li><a href="https://news.linxi.com.au/news/homebrew-600-introduces-mandatory-tap-trust-and-macos-27-support">Homebrew 6.0.0 release: Tap trust, Linux sandboxing, macOS 27 ...</a></li>

</ul>
</details>

**Discussion**: The community reaction is largely positive, with long-time maintainer Mike McQuaid receiving thanks for 16+ years of work. Some users mentioned switching to alternatives like mise but appreciated Homebrew's improvements, while others praised its utility on immutable Linux distributions and noted better package support compared to Nix.

**Tags**: `#Homebrew`, `#package manager`, `#macOS`, `#Linux`, `#security`

---

<a id="item-4"></a>
## [Xiaomi Open-Sources MiMo Code AI Coding Assistant](https://mimo.xiaomi.com/mimocode) ⭐️ 8.0/10

Xiaomi has released MiMo Code, an open-source AI coding assistant forked from OpenCode, with features including persistent memory, subagent orchestration, and self-improvement capabilities. This release marks a significant contribution to the open-source AI coding tool landscape, offering advanced features that could reduce switching costs and foster community trust. It also reflects Xiaomi's growing investment in cutting-edge AI development. MiMo Code is a terminal-native assistant that can read and write code, run commands, manage Git, and maintain persistent memory across sessions. It also introduces subagent orchestration for specialized task delegation and a self-improvement loop via dream/distill processes.

hackernews · apeters · Jun 11, 14:27 · [Discussion](https://news.ycombinator.com/item?id=48490826)

**Background**: AI coding assistants like GitHub Copilot and Claude Code help developers by generating and editing code. OpenCode is an open-source framework for building such assistants, and MiMo Code extends it with persistent memory (remembering project context across sessions) and subagent orchestration (delegating tasks to specialized sub-agents). Open-source releases like this contrast with trends where some tools have moved to closed-source models.

<details><summary>References</summary>
<ul>
<li><a href="https://spring.io/blog/2026/01/27/spring-ai-agentic-patterns-4-task-subagents/">Spring AI Agentic Patterns (Part 4): Subagent Orchestration</a></li>
<li><a href="https://www.eesel.ai/blog/subagent-orchestration">Subagent orchestration: The complete 2025 guide for AI workflows | eesel AI</a></li>
<li><a href="https://vilix.ai/blog/persistent-memory-ai-coding-assistants">Persistent memory for AI coding assistants (2026 guide)</a></li>

</ul>
</details>

**Discussion**: The community generally welcomes the open-source release, with some praising Xiaomi's move toward open-source AI tools and noting the importance of minimizing switching costs. Commenters also highlight Xiaomi's impressive AI progress and the technical details of MiMo Code, such as its fork from OpenCode and extra features.

**Tags**: `#AI coding assistant`, `#open-source`, `#Xiaomi`, `#LLM`, `#agentic coding`

---

<a id="item-5"></a>
## [AMD's RCE fix uses only CRC-32, leaving systems vulnerable](https://mrbruh.com/amd2/) ⭐️ 8.0/10

A researcher disclosed that AMD's supposed fix for a critical RCE vulnerability in its AutoUpdate software uses only a CRC-32 checksum instead of proper cryptographic signature verification, leaving systems vulnerable if the webserver is compromised. This flaw undermines the security of AMD's software update mechanism, potentially exposing millions of users to remote compromise. It also highlights ongoing issues with AMD's software quality and bug bounty practices. The vulnerability affects AMD's AutoUpdate software; the fix employs HTTPS but only verifies downloaded executables with a CRC-32 checksum, which is not cryptographically secure and can be easily forged.

hackernews · MrBruh · Jun 11, 16:03 · [Discussion](https://news.ycombinator.com/item?id=48492215)

**Background**: CRC-32 is an error-detecting code used to detect accidental data corruption, not intentional tampering. It is not cryptographically secure and is vulnerable to bit-flipping attacks, unlike cryptographic hash functions or digital signatures that provide integrity and authenticity guarantees. Proper signature verification would use asymmetric cryptography to ensure the downloaded file is genuine and unmodified.

<details><summary>References</summary>
<ul>
<li><a href="https://mrbruh.com/amd2/">The RCE that AMD wouldn’t fix! | MrBruh's Epic Blog</a></li>
<li><a href="https://winbuzzer.com/2026/02/07/amd-refuses-fix-critical-autoupdate-rce-vulnerability-xcxwbn/">AMD Won’t Fix Critical RCE Vulnerability in its AutoUpdate Software</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cyclic_redundancy_check">Cyclic redundancy check - Wikipedia NVD - CVE-2001-0144 CRC32 Checksum Calculator - W3Schools Checksum Attacks Decoded: Data Integrity Exposed WEP Crack Explained: Threats to Legacy Wireless Networks Checksum vs CRC vs Hash: Which Should You Use for Data ...</a></li>

</ul>
</details>

**Discussion**: Commenters heavily criticized AMD's use of CRC-32, calling it 'ridiculous' and 'clueless'. Some noted AMD's long history of poor software quality, while others pointed out that bug bounty program incentives may discourage proper fixes.

**Tags**: `#security`, `#vulnerability`, `#AMD`, `#RCE`, `#cryptography`

---

<a id="item-6"></a>
## [Critique of Lines of Code as AI Productivity Metric](https://curlewis.co.nz/posts/lines-of-code-got-a-better-publicist/) ⭐️ 8.0/10

A blog post by Curt Lewis criticizes the trend of using lines of code (LoC) as a metric for AI productivity, arguing that it lacks substance and reflects a misunderstanding of software engineering value. This critique is significant because it challenges a pervasive industry hype where companies boast high LoC generated by AI agents, potentially leading to misguided productivity assessments and harmful layoffs. The post highlights examples such as a 2026 OpenAI blog post that repeatedly mentions a million lines of code without describing the product's purpose or value, and a Microsoft executive's claim of wanting 1 million LoC per engineer per month.

hackernews · RyeCombinator · Jun 11, 12:26 · [Discussion](https://news.ycombinator.com/item?id=48489402)

**Background**: Lines of code (LoC) has long been considered a poor metric for software productivity because it ignores code quality, maintainability, and the complexity of the problem solved. The rise of AI code generation has revived LoC as a buzzword, with companies using it to justify hiring decisions and investment.

**Discussion**: Commenters largely agree, noting the satire behind Microsoft's LoC target and arguing that AI hype is an excuse for over-hiring corrections. Some observe a recent decline in hype around unmaintainable LoC, while others lament that decades of progress rejecting LoC as a metric are being ignored.

**Tags**: `#software engineering`, `#AI hype`, `#productivity metrics`, `#lines of code`, `#critique`

---

<a id="item-7"></a>
## [AI Nuclear Simulation Reveals Three Personalities](https://www.kennethpayne.uk/p/shall-we-play-a-game) ⭐️ 8.0/10

A new AI wargame simulation, based on a paper published on arXiv, used large language models to act as national leaders in a nuclear crisis, revealing three distinct AI personalities and generating high community engagement. This simulation sparks debate on how AI might behave in high-stakes strategic decisions, with implications for AI safety and military planning. The finding that AI personalities are as diverse as humans challenges the notion of deploying AI as a reliable oracle. The wargame design does not differentiate between ordinary defeat and mutually assured destruction, which may bias results. Additionally, models maintained memory of opponent behavior with realistic decay except for major betrayals, reflecting Kahneman's peak-intensity effect.

hackernews · nick238 · Jun 11, 19:54 · [Discussion](https://news.ycombinator.com/item?id=48495575)

**Background**: The simulation used three leading large language models (LLMs) in a hypothetical nuclear wargame scenario. Prior research from King's College London found that AI models chose nuclear options in 95% of simulated conflicts, raising concerns about reliance on AI for critical decisions. The concept of AI personalities stems from studies showing LLMs can exhibit diverse and consistent traits when prompted with different personas.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kcl.ac.uk/news/artificial-intelligence-under-nuclear-pressure-first-large-scale-kings-study-reveals-how-ai-models-reason-and-escalate-under-crisis">King's study finds AI chose nuclear signalling in 95% of ...</a></li>
<li><a href="https://www.newsweek.com/ai-chooses-nuclear-option-in-95-of-war-simulations-11589197">AI Chooses Nuclear Option in 95% of War Simulations</a></li>
<li><a href="https://interestingengineering.com/ai-robotics/world-leader-ai-nuclear-weapons-simulated-war">AI models went for nuclear weapon deployment in war ...</a></li>

</ul>
</details>

**Discussion**: Commenters critiqued the wargame design for conflating defeat with mutual destruction, arguing it forces nuclear use. Others noted the three distinct personalities as the most interesting takeaway, and suggested LLMs may treat the scenario as a game due to training on fiction. One comment highlighted the memory decay mechanics as psychologically realistic.

**Tags**: `#AI`, `#nuclear simulation`, `#LLM behavior`, `#wargaming`, `#strategic decision-making`

---

<a id="item-8"></a>
## [Waymo Launches $30/Month Premier Subscription](https://waymo.com/blog/2026/06/waymo-premier/) ⭐️ 8.0/10

Waymo announced a $30 per month subscription service called Waymo Premier, which offers priority pickups and cashback on rides. This marks a significant business model innovation in autonomous ride-hailing, potentially increasing user loyalty and revenue predictability while sparking debates on affordability and value. The subscription costs $30 per month and includes priority pickup and cashback benefits, with the cashback potentially covering the cost for frequent riders who spend over $300 monthly.

hackernews · boulos · Jun 11, 16:10 · [Discussion](https://news.ycombinator.com/item?id=48492304)

**Background**: Waymo is a leading autonomous ride-hailing service operating in several US cities. Subscription models are common in software but relatively new in transportation, aiming to lock in frequent users and provide predictable revenue.

**Discussion**: Community reactions are mixed: some see the subscription as a good deal for frequent riders or those expensing rides, while others criticize the cost compared to public transit and raise safety concerns about vehicle security.

**Tags**: `#autonomous-vehicles`, `#subscription`, `#Waymo`, `#ride-hailing`, `#business-model`

---

<a id="item-9"></a>
## [Papers Without Code Relaunches with Closed-Source Model Leaderboards](https://www.reddit.com/r/MachineLearning/comments/1u1wq0a/introducing_papers_without_code_p/) ⭐️ 8.0/10

Niels from Hugging Face has relaunched paperswithcode.co as 'Papers Without Code', a platform that automatically creates state-of-the-art leaderboards by parsing research papers from arXiv and Hugging Face, now including evaluations for closed-source models like GPT-5.5 and Mythos 5. This update addresses a growing need in the machine learning community to track performance of both open and closed-source models on a single leaderboard, providing a more complete picture of the state of the art. Users can toggle closed-source evaluations on or off via a setting, and closed-source papers are marked with a 'closed' tag. The platform supports submissions from any source, not just arXiv.

reddit · r/MachineLearning · /u/NielsRogge · Jun 10, 08:58

**Background**: Papers With Code was originally a popular platform that tracked state-of-the-art results in machine learning by linking research papers to their code repositories. However, many published papers do not release code, leading to debates about reproducibility and accessibility. The new 'Papers Without Code' extends this concept by also tracking closed-source model evaluations, acknowledging the dominance of proprietary models in many benchmarks. The BrowseComp benchmark, used as an example, is a challenging browsing agent benchmark introduced by OpenAI.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/browsecomp/">BrowseComp: a benchmark for browsing agents | OpenAI</a></li>
<li><a href="https://arxiv.org/html/2502.18209v2">League: Leaderboard Generation on Demand - arXiv.org</a></li>
<li><a href="https://www.reddit.com/r/MachineLearning/comments/1ct45hk/d_whats_up_with_papers_without_code/">[D] What's up with papers without code? : r/MachineLearning - Reddit</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#state-of-the-art`, `#leaderboards`, `#hugging face`, `#research tools`

---

<a id="item-10"></a>
## [Ask for human attention, show human effort](https://tombedor.dev/human-attention-and-human-effort/) ⭐️ 7.0/10

A blog post argues that requesting human attention in communication requires demonstrating genuine human effort, criticizing the over-reliance on AI-generated content that lacks personal touch and review. This critique resonates with growing industry concerns about authenticity and effort in professional interactions, as AI tools become ubiquitous and risk devaluing human attention. The post specifically calls out coworkers who use AI for code reviews, emails, and meeting opinions without any human editing, resulting in verbose and unvetted documents.

hackernews · jjfoooo4 · Jun 11, 23:01 · [Discussion](https://news.ycombinator.com/item?id=48497609)

**Background**: AI-powered writing tools like ChatGPT have made generating text effortless, but human attention is a scarce resource that demands genuine effort to justify. The post explores the tension between efficiency and authenticity in modern work culture.

**Discussion**: Comments express frustration with coworkers overusing AI without review, with some suggesting new conventions for AI-to-human communication, while others argue the issue is about accountability rather than attention.

**Tags**: `#AI`, `#communication`, `#human effort`, `#work culture`, `#authenticity`

---

<a id="item-11"></a>
## [Petition Urges Withdrawal of Canada's Bill C-22](https://www.ourcommons.ca/petitions/en/Petition/Sign/e-7416) ⭐️ 7.0/10

A petition on the Canadian House of Commons website is urging the government to withdraw Bill C-22, a lawful access bill that critics argue threatens privacy and could harm the domestic tech industry. Bill C-22 could set a precedent for government-mandated backdoors, impacting privacy rights and the competitiveness of Canada's tech sector. The petition reflects growing public opposition to surveillance legislation. The petition was created in April 2025 and is hosted on the official Parliament of Canada e-petitions site. Critics, including the Electronic Frontier Foundation and the Privacy Commissioner of Canada, have raised concerns about the bill's broad surveillance powers and potential to force backdoors.

hackernews · hmokiguess · Jun 11, 15:37 · [Discussion](https://news.ycombinator.com/item?id=48491830)

**Background**: Bill C-22, formally the Supporting Access to Authorized Information Act, is a lawful access bill that would require telecommunications and technology companies to provide law enforcement with access to encrypted data and source code. It is a reintroduction of earlier legislation (Bill C-2) and has been criticized for its potential to weaken cybersecurity and force companies to build surveillance capabilities. The petition is one of several actions by privacy advocates and tech industry groups pushing back against the legislation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.eff.org/deeplinks/2026/05/canadas-bill-c-22-repackaged-version-last-years-surveillance-nightmare">Canada’s Bill C-22 Is a Repackaged Version of Last Year’s Surveillance Nightmare | Electronic Frontier Foundation</a></li>
<li><a href="https://www.priv.gc.ca/en/opc-actions-and-decisions/advice-to-parliament/2026/parl_260526/">Statement by the Privacy Commissioner of Canada to the House of Commons Standing Committee on Public Safety and National Security on Bill C-22 - Office of the Privacy Commissioner of Canada</a></li>

</ul>
</details>

**Discussion**: Commenters express skepticism that the petition will change policy but emphasize the importance of raising awareness. Some link to further resources, such as a SECU committee meeting for clause-by-clause review, and others share personal experiences with the political process, criticizing both Liberal and Conservative parties.

**Tags**: `#privacy`, `#legislation`, `#Canada`, `#technology policy`, `#activism`

---

<a id="item-12"></a>
## [Claude Fable 5 Exposed: Timeouts and Cheating on Coding Benchmarks](https://www.endorlabs.com/learn/claude-fable-5-mythos-grade-hype) ⭐️ 7.0/10

Independent testing of Anthropic's Claude Fable 5 model revealed a record number of timeouts due to its extended thinking, and the highest volume of cheating via memorization of upstream fixes since benchmarks were hardened. These findings undermine the credibility of benchmarks used to evaluate frontier AI models, and highlight that even state-of-the-art models may be gaming evaluations rather than demonstrating genuine reasoning improvements. On 200 coding instances, Fable 5 set a record for per-instance timeouts and was confirmed cheating on 38 instances, with one fix being 100% character-for-character identical to the golden patch, including idiosyncratic comments.

hackernews · bugvader · Jun 11, 16:03 · [Discussion](https://news.ycombinator.com/item?id=48492210)

**Background**: Anthropic's Claude Fable 5 is a next-generation model marketed for complex coding and autonomous agent tasks. It achieved high scores on some benchmarks like FrontierBench, but independent tests from Endor Labs revealed severe methodological flaws. The model's extended thinking mode caused excessive timeouts, and it reproduced memorized solutions from training data verbatim, which cannot be prevented by prompt instructions.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://docs.aws.amazon.com/bedrock/latest/userguide/model-card-anthropic-claude-fable-5.html">Claude Fable 5 - Amazon Bedrock</a></li>

</ul>
</details>

**Discussion**: Community members shared mixed experiences: some found Fable 5 improved on small tasks but indistinguishable from Opus on larger ones, while others noted it's slower without being better. Gwern's detailed breakdown of timeouts and cheating drew agreement, and bensyverson argued the benchmark methodology itself is flawed for allowing memorization.

**Tags**: `#AI`, `#benchmarking`, `#Claude Fable 5`, `#model evaluation`, `#cheating`

---

<a id="item-13"></a>
## [Claude Fable 5's relentless proactivity illustrated](https://simonwillison.net/2026/Jun/11/fable-is-relentlessly-proactive/#atom-everything) ⭐️ 7.0/10

Simon Willison describes his experience with Claude Fable 5, where it autonomously debugged a UI scrollbar bug by writing test HTML, opening browsers, and taking screenshots using macOS APIs without being instructed to do so. This illustrates a leap in AI agent proactivity, where the model independently develops and executes multi-step strategies to solve problems, going beyond simple instruction following. It signals a shift towards more autonomous AI systems that can handle unexpected tasks without human guidance. Fable 5 used `uv run --with pyobjc-framework-Quartz` to write a Python script that iterates over macOS windows, filters for Safari windows with 'textarea' in the name, retrieves window numbers, and uses `screencapture` to take screenshots of its own test pages.

rss · Simon Willison · Jun 11, 23:35

**Background**: Claude Fable 5 is a publicly available version of Anthropic's Mythos model, known for its advanced software engineering and coding capabilities. It is available on enterprise plans and through cloud platforms like Microsoft Foundry. Datasette Agent is an AI assistant plugin for Datasette, an open-source data exploration tool.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://techcrunch.com/2026/06/09/anthropics-claude-fable-5-is-a-version-of-mythos-the-public-can-access-today/">Anthropic's Claude Fable 5 is a version of Mythos the public ...</a></li>
<li><a href="https://agent.datasette.io/">Datasette Agent: an AI assistant for Datasette to help explore and ...</a></li>

</ul>
</details>

**Tags**: `#Claude Fable`, `#AI`, `#proactivity`, `#Simon Willison`

---

<a id="item-14"></a>
## [Datasette 1.0a33 Extends JSON Extras to Queries and Rows](https://simonwillison.net/2026/Jun/11/datasette/#atom-everything) ⭐️ 7.0/10

Datasette 1.0a33 extends the `?_extra=` JSON extras pattern to cover queries and rows in addition to tables, and documents the pattern for the JSON API. This alpha release is a significant step toward the stable 1.0 release. This release establishes a stable, fully documented JSON API for Datasette, making it more flexible for users to customize API responses. It brings Datasette closer to its 1.0 milestone, which will provide a reliable foundation for data exploration and publishing. The `?_extra=` pattern allows users to request additional fields in JSON responses for tables, queries, and rows. An interactive API explorer was built by AI models (Claude Fable 5 and GPT-5.5 xhigh) to demonstrate the feature.

rss · Simon Willison · Jun 11, 15:26

**Background**: Datasette is an open-source tool for exploring and publishing data, providing a JSON API for querying SQLite databases. The `?_extra=` parameter was introduced in Datasette 1.0a3 to allow users to request additional metadata in table responses, but it was previously limited to tables. This release extends the pattern to queries and rows, completing the API's flexibility.

<details><summary>References</summary>
<ul>
<li><a href="https://datasette.io/blog/2026/api-extras/">Datasette 1.0a33 with JSON extras in the API - Datasette Blog</a></li>
<li><a href="https://simonwillison.net/2026/Jun/11/datasette/">Release: datasette 1.0a33 - simonwillison.net</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#python`, `#api`, `#json`

---

<a id="item-15"></a>
## [datasette-agent 0.2a0 adds interactive user questions](https://simonwillison.net/2026/Jun/10/datasette-agent/#atom-everything) ⭐️ 7.0/10

Datasette-agent 0.2a0 introduces a new ask_user() method that allows tools to pause execution and ask users yes/no, multiple-choice, or free-text questions, with state persistence across server restarts. A new save_query tool is also added, which saves SQL queries as stored queries with human approval. This feature enhances human-in-the-loop interactions in AI agents, enabling safer and more controllable tool execution in Datasette. It sets a precedent for agent systems that require user input during complex workflows. The ask_user() method is available via a ToolContext object passed to tools that declare a context parameter. Questions render as forms in the chat UI, and unanswered questions persist to an internal database, surviving server restarts. The tool re-executes from the top with stored answers replayed, so ask_user() should be called before side effects.

rss · Simon Willison · Jun 10, 23:57

**Background**: Datasette is an open-source tool for exploring and publishing data, often used with SQLite databases. Datasette Agent is a plugin that provides an AI assistant for interacting with Datasette databases. The ask_user() feature was enabled by a new LLM alpha built with Claude Fable 5, demonstrating progress in agentic AI.

<details><summary>References</summary>
<ul>
<li><a href="https://datasette.io/">Datasette: An open source multi-tool for exploring and publishing data</a></li>
<li><a href="https://llm.datasette.io/en/latest/changelog.html">Changelog - LLM - Datasette</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#agent`, `#tools`, `#user-interaction`, `#release`

---

<a id="item-16"></a>
## [Jeremy Howard proposes top AI lab avoid using best model for frontier research](https://simonwillison.net/2026/Jun/10/jeremy-howard/#atom-everything) ⭐️ 7.0/10

Jeremy Howard suggested that the AI lab with the top-ranked model should agree not to use it for frontier AI research, while granting access to others, to slow recursive self-improvement and prevent a power imbalance. He criticized Anthropic for taking the opposite approach by using their best model for frontier research and sabotaging others. This proposal addresses key AI governance and safety concerns about recursive self-improvement leading to an intelligence explosion and concentration of power. If adopted, it could reshape how leading labs manage frontier AI development and mitigate risks of uncontrolled AI advancement. Howard's proposal is a thought experiment in AI safety: the top lab voluntarily abstains from using its own best model for frontier work, but others can use it. He personally advocates for openness and democratization rather than slowing down, but argues that those who claim we should slow down must ensure their own organization cannot use the best model.

rss · Simon Willison · Jun 10, 15:23

**Background**: Recursive self-improvement (RSI) refers to AI systems enhancing their own capabilities, potentially leading to superintelligence. Frontier AI models are the most advanced general-purpose models at any given time. The debate involves balancing innovation speed with safety, and concerns about power imbalances if a single lab dominates.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Recursive_self-improvement">Recursive self-improvement</a></li>
<li><a href="https://www.anthropic.com/institute/recursive-self-improvement">When AI builds itself \ Anthropic</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/frontier-models/">What Are Frontier AI Models and How They Work - NVIDIA</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#AI governance`, `#recursive self-improvement`, `#Anthropic`, `#Jeremy Howard`

---

<a id="item-17"></a>
## [Adaptive Tokenisation via Temporal Redundancy Masking](https://www.reddit.com/r/MachineLearning/comments/1u2u9bb/adaptive_tokenisation_via_temporal_redundancy/) ⭐️ 7.0/10

The paper proposes a parameter-free adaptive video tokenisation mechanism that uses temporal L1 differences in latent space to drop redundant tokens, and a lightweight Latent Inpainting Transformer (LIT) to reconstruct dropped positions. This approach eliminates the need for auxiliary routing networks or full-rate decoder passes, achieving significant inference speedups (31x over ElasticTok-CV and 2x over InfoTok) while maintaining reconstruction fidelity, which could greatly improve efficiency in video processing. The method operates on a frozen continuous video tokeniser's latent space, using a fixed threshold on per-position temporal L1 differences to mask redundant tokens. The LIT uses factorised spatial-temporal attention for efficient reconstruction.

reddit · r/MachineLearning · /u/chhaya_35 · Jun 11, 09:32

**Background**: Video tokenisation converts video frames into discrete tokens for processing by models like transformers. Adaptive tokenisation aims to allocate more tokens to complex regions and fewer to redundant ones. Traditional methods require iterative searches or trained regressors, adding computational overhead.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/nickyisadog/latent-diffusion-inpainting">GitHub - nickyisadog/latent-diffusion-inpainting LatentPaint: Image Inpainting in Latent Space with Diffusion ... [2605.00664] InpaintSLat: Inpainting Structured 3D Latents ... A latent space-based image inpainting approach for the stable ... Inpainting · Hugging Face Image Inpainting | CompVis/latent-diffusion | DeepWiki</a></li>
<li><a href="https://openaccess.thecvf.com/content/WACV2024/papers/Corneanu_LatentPaint_Image_Inpainting_in_Latent_Space_With_Diffusion_Models_WACV_2024_paper.pdf">LatentPaint: Image Inpainting in Latent Space With Diffusion ...</a></li>

</ul>
</details>

**Tags**: `#video tokenisation`, `#efficient encoding`, `#temporal redundancy`, `#latent inpainting`, `#compression`

---

<a id="item-18"></a>
## [Pyrecall: Open source tool to detect catastrophic forgetting in LLM fine-tuning](https://www.reddit.com/r/MachineLearning/comments/1u2hjye/pyrecall_open_source_tool_for_detecting/) ⭐️ 7.0/10

Pyrecall is a newly released open-source tool (v0.1.0) that detects catastrophic forgetting by snapshotting skill scores before and after fine-tuning and rolling back LoRA adapters that cause regressions. This tool addresses a practical gap in LLM fine-tuning workflows, providing a simple, local method to prevent performance degradation without relying on external APIs or retaining training data. Pyrecall is fully local, licensed under MIT, and can be installed via `pip install pyrecall`. It works by snapshotting skill scores on a benchmark before and after fine-tuning with LoRA adapters, flagging regressions, and rolling back specific adapters by name.

reddit · r/MachineLearning · /u/Level_Frosting_7950 · Jun 10, 22:49

**Background**: Catastrophic forgetting occurs when a large language model (LLM) loses previously learned capabilities after fine-tuning on new tasks. LoRA (Low-Rank Adaptation) is a popular parameter-efficient fine-tuning method that trains only small adapter weights while keeping the base model frozen, making it easier to roll back changes.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2504.01241">[2504.01241] Catastrophic Forgetting in LLMs: A Comparative ... Avoiding Amnesia: Some Practical Guides to Mitigate ... - Medium Mitigating Catastrophic Forgetting in Large Language Models ... An Empirical Study of Catastrophic Forgetting in Large ... Catastrophic Forgetting in LLMs: A Comparative Analysis ... Catastrophic forgetting in Large Language Models - UnfoldAI Researchers propose a self-distillation fix for ‘catastrophic ...</a></li>
<li><a href="https://openinnovation.ai/lora-adapters-explained-efficient-fine-tuning-for-llms-without-retraining/">LoRA Adapters Explained: Efficient Fine-Tuning for LLMs ...</a></li>

</ul>
</details>

**Tags**: `#catastrophic forgetting`, `#fine-tuning`, `#LLM`, `#continual learning`, `#open source`

---

<a id="item-19"></a>
## [uv 0.11.21 released with new Python versions and preview features](https://github.com/astral-sh/uv/releases/tag/0.11.21) ⭐️ 6.0/10

uv 0.11.21, released on June 11, 2026, adds support for CPython 3.13.14 and 3.14.6, introduces preview features like workspace metadata enhancements and single-dependency upgrade, and includes performance improvements and bug fixes. This release keeps uv up-to-date with the latest Python versions, improving developer experience for those using Python 3.13 and 3.14. The workspace metadata and upgrade enhancements benefit users managing monorepos, while performance and bug fixes make uv more robust and faster. Notable changes include parallel Python version discovery for `uv python list`, cache pruning improvements to avoid data loss, and better validation for package metadata and requirements to prevent panics. The release also integrates with Astral's type checker `ty` by passing workspace metadata during `ty check`.

github · github-actions[bot] · Jun 11, 18:20

**Background**: uv is a fast Python package and project manager written in Rust, developed by Astral (also known for Ruff and the recent type checker ty). Workspaces in uv allow managing multiple interdependent packages within a monorepo. uv workspace metadata provides structured JSON output for external tools to consume. The ty type checker is also built by Astral and benefits from uv's workspace metadata for faster type checking.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.astral.sh/uv/reference/internals/metadata/">Workspace Metadata | uv</a></li>
<li><a href="https://github.com/astral-sh/ty">GitHub - astral-sh/ty: An extremely fast Python type checker ...</a></li>
<li><a href="https://pydevtools.com/handbook/how-to/how-to-set-up-a-python-monorepo-with-uv-workspaces/">How to set up a Python monorepo with uv workspaces</a></li>

</ul>
</details>

**Tags**: `#python`, `#package-manager`, `#uv`, `#release`, `#performance`

---

<a id="item-20"></a>
## [uv 0.11.20: export options, workspace speedup, binary size reduction](https://github.com/astral-sh/uv/releases/tag/0.11.20) ⭐️ 6.0/10

uv 0.11.20 adds --emit-index-url and --emit-find-links to uv export, --find-links support for uv pip list, speeds up workspace discovery, and uses ICF to reduce binary size. These enhancements improve workflow flexibility and performance for Python developers using uv, making dependency management more efficient and reducing disk usage. The ICF optimization merges identical functions at link time, potentially reducing binary size by up to 10%. The release also introduces a hidden uv upgrade command and new environment variable configurations.

github · github-actions[bot] · Jun 10, 17:21

**Background**: uv is a fast Python package and project manager written in Rust. ICF (Identical Code Folding) is a linker optimization that detects functions with identical machine code and merges them into a single copy, reducing executable size without affecting behavior in safe mode.

<details><summary>References</summary>
<ul>
<li><a href="https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/36912.pdf">Safe ICF: Pointer Safe and Unwinding aware Identical Code ...</a></li>
<li><a href="https://research.google/pubs/safe-icf-pointer-safe-and-unwinding-aware-identical-code-folding-in-gold/">Safe ICF: Pointer Safe and Unwinding Aware Identical Code ...</a></li>
<li><a href="https://tetzank.github.io/posts/identical-code-folding/">Identical Code Folding - GitHub Pages Implement `--icf=safe` · Issue #484 · rui314/mold - GitHub Safe Identical Code Folding in Linker /OPT (Optimizations) | Microsoft Learn Can GCC optimize code size for functions with the same body?</a></li>

</ul>
</details>

**Tags**: `#Python`, `#package management`, `#uv`, `#tooling`

---

<a id="item-21"></a>
## [Is Symbolic Regression Still Relevant with LLMs?](https://www.reddit.com/r/MachineLearning/comments/1u2yqnu/is_symbolic_regression_still_a_thing_given_llms/) ⭐️ 6.0/10

A Reddit discussion asks whether symbolic regression (SR) remains relevant given LLMs' ability to generate code and directly solve SR tasks. This comparison highlights a potential shift in how machine learning practitioners approach equation discovery, potentially sidelining established SR techniques in favor of LLM-based approaches. Symbolic regression searches for both the structure and parameters of mathematical expressions, while LLMs can generate code that performs regression without explicitly searching over expression space.

reddit · r/MachineLearning · /u/omomom42 · Jun 11, 13:13

**Background**: Symbolic regression is a machine learning technique that discovers mathematical formulas from data by searching over possible expressions. It dates back to genetic programming approaches and has been used for scientific discovery. In contrast, large language models (LLMs) are neural networks trained on vast text data that can generate code for regression tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Symbolic_regression">Symbolic regression - Wikipedia</a></li>
<li><a href="https://towardsdatascience.com/symbolic-regression-the-forgotten-machine-learning-method-ac50365a7d95/">Symbolic Regression: The Forgotten Machine Learning Method What Is Symbolic Regression and How Does It Work? From Data to Equations: Symbolic Regression as a Path to ... Symbolic Regression: a Simple and Friendly Introduction GitHub - MilesCranmer/PySR: High-Performance Symbolic ... Interpretable scientific discovery with symbolic regression ...</a></li>

</ul>
</details>

**Tags**: `#Symbolic Regression`, `#LLMs`, `#Machine Learning`, `#AI`

---