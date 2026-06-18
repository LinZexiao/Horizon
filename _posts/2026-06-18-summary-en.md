---
layout: default
title: "Horizon Summary: 2026-06-18 (EN)"
date: 2026-06-18
lang: en
---

> From 55 items, 29 important content pieces were selected

---

1. [GLM-5.2 is probably the most powerful text-only open weights LLM](#item-1) ⭐️ 9.0/10
2. [Microsoft's NextLat Boosts Transformer Efficiency 3.3x](#item-2) ⭐️ 9.0/10
3. [Epic Games Open-Sources Lore, a Scalable VCS for Game Development](#item-3) ⭐️ 8.0/10
4. [Leaked financials: OpenAI losing billions despite $13B revenue](#item-4) ⭐️ 8.0/10
5. [Running Firecracker microVMs in EC2 for sub-second browser launch](#item-5) ⭐️ 8.0/10
6. [U.S. Science in Crisis as Researchers Flee](#item-6) ⭐️ 8.0/10
7. [Tesco to move 40,000 server workloads off VMware](#item-7) ⭐️ 8.0/10
8. [RFC 10008 Introduces the HTTP QUERY Method](#item-8) ⭐️ 8.0/10
9. [Volkswagen Blocks GrapheneOS Users via Play Protect Requirement](#item-9) ⭐️ 8.0/10
10. [AI Flips Code Economics: From Asset to Disposable](#item-10) ⭐️ 8.0/10
11. [Export Controls on AI Undermine US Cyber Defense](#item-11) ⭐️ 8.0/10
12. [Speculative Decoding Gains Traction for Faster LLM Inference](#item-12) ⭐️ 8.0/10
13. [Contrastive Targeted SFT for Mechanistic Interpretability](#item-13) ⭐️ 8.0/10
14. [US delays blacklisting DeepSeek, deems 100+ Chinese firms security risks](#item-14) ⭐️ 7.0/10
15. [Adam Launches Open-Source AI CAD Platform CADAM](#item-15) ⭐️ 7.0/10
16. [AI models compared in robot game: cost vs performance](#item-16) ⭐️ 7.0/10
17. [Datasette 1.0a34 adds CRUD to web interface](#item-17) ⭐️ 7.0/10
18. [Expert says Anthropic's Fable jailbreak shows model working as intended](#item-18) ⭐️ 7.0/10
19. [Is foundational AI research possible without HPC?](#item-19) ⭐️ 7.0/10
20. [Leakage-Clean Verifier for Robot Manipulation Using Object-Centric Graphs](#item-20) ⭐️ 7.0/10
21. [8-bit live baseball gamecast using MLB data](#item-21) ⭐️ 6.0/10
22. [Human Connection: The AI-Proof Competitive Moat](#item-22) ⭐️ 6.0/10
23. [Thinking Out Loud Boosts Problem-Solving](#item-23) ⭐️ 6.0/10
24. [Click-to-Play Web Component for GIFs](#item-24) ⭐️ 6.0/10
25. [Georgi Gerganov Endorses Qwen3.6-27B for Local Coding](#item-25) ⭐️ 6.0/10
26. [Cloudflare CAPTCHA Rule for URLs with Ampersands](#item-26) ⭐️ 6.0/10
27. [ACL 2026 first author with weak GPA seeks PhD advice](#item-27) ⭐️ 6.0/10
28. [Probe Capacity vs. Network Capacity in Interpretability](#item-28) ⭐️ 6.0/10
29. [GAN deployed on Raspberry Pi 4 for physical NFT minting](#item-29) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [GLM-5.2 is probably the most powerful text-only open weights LLM](https://simonwillison.net/2026/Jun/17/glm-52/#atom-everything) ⭐️ 9.0/10

Z.ai released GLM-5.2, a 753B parameter Mixture of Experts (MoE) text-only LLM with a 1 million token context window under the MIT license, which Artificial Analysis ranks as the leading open weights model on its Intelligence Index v4.1. GLM-5.2 challenges proprietary frontier models by offering state-of-the-art performance at a fraction of the cost, with input/output pricing around $1.40/$4.40 per million tokens, potentially democratizing access to powerful LLMs. Despite its high benchmark scores, GLM-5.2 uses more output tokens per task (43k) compared to peers like MiniMax-M3 (24k) and DeepSeek V4 Pro (37k). It is a text-only model; Z.ai's vision model GLM-5V-Turbo is not open weights.

rss · Simon Willison · Jun 17, 23:58

**Background**: Mixture of Experts (MoE) is a machine learning technique that activates only a subset of parameters per input, enabling large total parameter counts while maintaining inference efficiency. Open weights models release the trained parameters publicly, often with permissive licenses, allowing community use and fine-tuning. A 1 million token context window allows the model to process and reason over very long documents, such as entire books or codebases.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>

</ul>
</details>

**Discussion**: Community comments are mixed: some praise GLM-5.2's performance and low cost, calling it a blow to closed-source API pricing, while others note excessive token usage and long reasoning times (e.g., 15 minutes for a simple math task). There is excitement about its open weights and accessibility.

**Tags**: `#LLM`, `#open weights`, `#Mixture of Experts`, `#GLM-5.2`, `#AI`

---

<a id="item-2"></a>
## [Microsoft's NextLat Boosts Transformer Efficiency 3.3x](https://www.reddit.com/r/MachineLearning/comments/1u84mio/nextlatent_prediction_transformers_r/) ⭐️ 9.0/10

Microsoft Research introduces Next-Latent Prediction (NextLat), a self-supervised method that trains transformers to predict their next latent state, achieving up to 3.3x faster inference via self-speculative decoding. This addresses the myopia of next-token prediction, enabling transformers to learn compact world models for reasoning and planning, and significantly reduces inference cost without extra model components. NextLat extends standard next-token training with an auxiliary loss that predicts the next latent state given the current latent and next token. It also enables self-speculative decoding where the model drafts and verifies tokens in a single forward pass, achieving lossless speedup.

reddit · r/MachineLearning · /u/jayden_teoh_ · Jun 17, 08:44

**Background**: Standard autoregressive transformers predict the next token given previous tokens, which can be myopic and data-inefficient. Self-supervised learning methods like NextLat encourage the model to learn compact internal representations. Self-speculative decoding leverages early layers of the same model to draft tokens and deeper layers to verify them, speeding up inference without auxiliary models.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2511.05963">[2511.05963] Next-Latent Prediction Transformers Learn ...</a></li>

</ul>
</details>

**Tags**: `#self-supervised learning`, `#transformers`, `#representation learning`, `#inference acceleration`, `#world models`

---

<a id="item-3"></a>
## [Epic Games Open-Sources Lore, a Scalable VCS for Game Development](https://lore.org/) ⭐️ 8.0/10

Epic Games has announced Lore, a new open-source version control system specifically designed for scalability in game development, released under the MIT license. Lore directly challenges Perforce's dominance in game development by offering a free, open-source alternative that handles large binary assets and file locking natively. This could reduce costs and friction for game studios large and small. Lore uses a mutable key-value store architecture and supports features like per-directory access control, sub-repository links, and exclusive file locks—critical for game development workflows. It is hosted on GitHub under the MIT license.

hackernews · regnerba · Jun 17, 14:30 · [Discussion](https://news.ycombinator.com/item?id=48571081)

**Background**: Traditional version control systems like Git are optimized for text-based files, but game development involves large binary assets such as textures, 3D models, and audio files, which require exclusive locking and efficient storage. Perforce has been the industry standard for such needs, but it is proprietary and complex to administer. Lore aims to provide a modern, open-source alternative tailored to these requirements.

<details><summary>References</summary>
<ul>
<li><a href="https://epicgames.github.io/lore/explanation/system-design/">The Lore Version Control System - Lore Developer Documentation</a></li>
<li><a href="https://github.com/EpicGames/lore">GitHub - EpicGames/ lore : Lore is a next-generation, open source...</a></li>
<li><a href="https://www.phoronix.com/news/Epic-Games-Lore-VCS">Epic Games Announces Lore Open-Source Version Control System</a></li>

</ul>
</details>

**Discussion**: Commenters recognize Lore as a promising Perforce alternative specifically for game development, noting Git's inadequacy for binary assets. They highlight Perforce's complexity and cost as pain points, and express excitement about Lore's open-source nature and potential to improve Unreal Engine workflows.

**Tags**: `#version control`, `#game development`, `#open source`, `#scalability`, `#Perforce alternative`

---

<a id="item-4"></a>
## [Leaked financials: OpenAI losing billions despite $13B revenue](https://arstechnica.com/ai/2026/06/leaked-financial-docs-show-openai-is-losing-billions-of-dollars-a-year/) ⭐️ 8.0/10

Leaked financial documents reveal OpenAI had $13 billion in gross revenue in 2025 but suffered billions in losses due to high cost of revenue ($7.5B) and massive R&D spending. This rare transparency into OpenAI's finances underscores the immense costs of leading AI development and raises critical questions about the long-term viability of its business model, affecting investor confidence and industry expectations. The documents show OpenAI has 900 million weekly active users but only 50 million paid subscribers, indicating a low conversion rate. R&D is the largest expense, and costs are growing rapidly alongside revenue.

hackernews · greenchair · Jun 17, 21:31 · [Discussion](https://news.ycombinator.com/item?id=48577208)

**Background**: OpenAI is the developer of ChatGPT and other advanced AI models. The company operates as a capped-profit entity under a non-profit parent. Training and running large AI models require enormous computing power and talent, leading to high operational costs. These leaked documents provide an unusual look inside a typically private AI company.

**Discussion**: Commentators observed that R&D costs dominate, questioning if focus should shift to reducing inference costs. Others noted the low conversion of free to paid users. Some expressed skepticism about the document's level of detail but agreed the figures highlight an unsustainable trajectory if growth slows.

**Tags**: `#OpenAI`, `#financials`, `#AI industry`, `#business model`

---

<a id="item-5"></a>
## [Running Firecracker microVMs in EC2 for sub-second browser launch](https://browser-use.com/posts/firecracker-browser-infra) ⭐️ 8.0/10

Browser Use has published a detailed article explaining how they run Firecracker microVMs inside EC2 using nested virtualization to launch stealthy browsers in less than one second. This innovation dramatically reduces browser startup latency for automation tasks while maintaining strong isolation, and it demonstrates the growing practicality of microVMs for serverless and stealthy browser-based workloads. The system achieves an 81% block avoidance rate on their stealth benchmark (versus 2% for plain headless Chromium) and 84.8% on Halluminate BrowserBench. Nested virtualization on regular EC2 instances became available only in February 2026, enabling this approach without bare metal.

hackernews · gregpr07 · Jun 16, 15:15 · [Discussion](https://news.ycombinator.com/item?id=48556561)

**Background**: Firecracker is an open-source virtual machine monitor (VMM) developed by AWS for running lightweight microVMs with fast startup and strong security isolation. Nested virtualization allows running a hypervisor inside a virtual machine, enabling hypervisor-based technologies like Firecracker to run on top of EC2 instances.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/firecracker-microvm/firecracker">GitHub - firecracker-microvm/firecracker: Secure and fast microVMs for serverless computing. · GitHub</a></li>
<li><a href="https://firecracker-microvm.github.io/">Firecracker</a></li>
<li><a href="https://medium.com/@meziounir/understanding-firecracker-microvms-the-next-evolution-in-virtualization-cb9eb8bbeede">Understanding Firecracker MicroVMs: The Next Evolution in Virtualization | by Meziouni Reda | Medium</a></li>

</ul>
</details>

**Discussion**: Commenters raised ethical concerns about bypassing anti-bot measures, noting that such services could be used for malicious purposes. Others discussed technical details like the recent availability of nested virtualization on EC2, suggested alternative browsers like Lightpanda for better performance, and proposed warm-pool strategies to reduce startup latency further.

**Tags**: `#Firecracker`, `#microVMs`, `#browser automation`, `#EC2`, `#nested virtualization`

---

<a id="item-6"></a>
## [U.S. Science in Crisis as Researchers Flee](https://www.scientificamerican.com/article/americas-compact-between-science-and-politics-is-broken/) ⭐️ 8.0/10

The U.S. scientific community is experiencing a crisis due to a broken political compact, funding cuts, and visa restrictions, driving many researchers to leave the country. This exodus threatens U.S. leadership in research and innovation, as talented scientists seek opportunities abroad, weakening the nation's scientific enterprise. The article highlights that grant funding has dried up, hiring of foreign graduate students is blocked by visa restrictions, and institutions fail to support researchers, leading to a 'death of research in the U.S.'

hackernews · presspot · Jun 17, 09:54 · [Discussion](https://news.ycombinator.com/item?id=48568058)

**Background**: The U.S. scientific enterprise has historically thrived on stable government funding and the free flow of international talent. The current crisis stems from a broken political compact, with funding cuts and restrictive visa policies. This has led to a loss of morale and a brain drain.

**Discussion**: Commenters describe personal crises: a spouse operating a sophisticated microscope is leaving the country; professors cannot hire foreign students due to visa restrictions; early-career researchers are abandoning science. Some see chaos as an opportunity, but overall sentiment is grim.

**Tags**: `#science policy`, `#research funding`, `#US immigration`, `#academic research`, `#researcher emigration`

---

<a id="item-7"></a>
## [Tesco to move 40,000 server workloads off VMware](https://arstechnica.com/information-technology/2026/06/tesco-moving-40000-server-workloads-off-vmware-amid-broadcoms-abusive-conduct/) ⭐️ 8.0/10

Tesco, a major UK retailer, announced it is migrating 40,000 server workloads away from VMware to an alternative virtualization platform, citing Broadcom's aggressive licensing and pricing changes after its acquisition of VMware. This is a significant validation of industry concerns about Broadcom's VMware strategy, potentially triggering a wave of large-scale migrations and boosting the market for VMware alternatives like Proxmox or Nutanix. The migration is expected to take 18 months, and Tesco faces challenges with data security because its new virtualization software is incompatible with existing backup products like Veeam and Zerto.

hackernews · Bender · Jun 17, 21:00 · [Discussion](https://news.ycombinator.com/item?id=48576838)

**Background**: In 2026, Broadcom retired perpetual VMware licenses, moving all customers to subscription-based pricing with per-core licensing, significantly increasing costs for many enterprises. This has prompted many organizations to explore alternatives like Proxmox, Nutanix, or Microsoft Hyper-V.

<details><summary>References</summary>
<ul>
<li><a href="https://redresscompliance.com/broadcom-vmware-licensing-changes-explained">Broadcom VMware Licensing 2026: Costs, Tiers, Renewals | Redress</a></li>
<li><a href="https://blog.everpuredata.com/solutions/vmware-licensing-changes-demystified/">VMware Licensing Changes Demystified | Everpure Blog</a></li>

</ul>
</details>

**Discussion**: Commenters noted that Broadcom's actions have made Proxmox marketing extremely effective, and that migration paths are now well-trodden. Some questioned the 18-month timeline, wondering about poor configuration management or lack of automation at scale.

**Tags**: `#VMware`, `#Broadcom`, `#virtualization`, `#migration`, `#enterprise IT`

---

<a id="item-8"></a>
## [RFC 10008 Introduces the HTTP QUERY Method](https://www.rfc-editor.org/info/rfc10008/) ⭐️ 8.0/10

RFC 10008 defines a new HTTP QUERY method that allows safe and idempotent requests with a request body, enabling standardized query operations without the semantic issues of GET or POST. This addresses long-standing interoperability and caching problems where developers used GET with a body or POST for queries, which breaks HTTP semantics and caching. The QUERY method provides a clean, standardized alternative for idempotent queries with bodies. The QUERY method is both safe and idempotent, allowing automatic retries without side effects. Caching is supported by including the request body as part of the cache key, which enables efficient response reuse for identical queries.

hackernews · schappim · Jun 17, 10:51 · [Discussion](https://news.ycombinator.com/item?id=48568502)

**Background**: HTTP GET requests are idempotent but cannot carry a request body, while POST requests are not idempotent and not cacheable by default. Developers often improvised by sending a body with GET (which is technically non-standard) or using POST for idempotent queries, causing interoperability issues. RFC 10008 formalizes a dedicated method for such use cases, aligning with HTTP's architectural principles.

<details><summary>References</summary>
<ul>
<li><a href="https://www.rfc-editor.org/info/rfc10008/">RFC 10008: The HTTP QUERY Method | RFC Editor</a></li>
<li><a href="https://www.rfc-editor.org/rfc/rfc10008.html">RFC 10008: The HTTP QUERY Method</a></li>

</ul>
</details>

**Discussion**: Comments discuss the caching implications of including the request body in the cache key, noting potential for unbounded or user-controlled keys. Some express hope that HTML forms will support the QUERY method to avoid POST re-submission warnings. Others question the motivating example, suggesting stronger use cases would better illustrate the need.

**Tags**: `#HTTP`, `#RFC`, `#protocol`, `#web`, `#API`

---

<a id="item-9"></a>
## [Volkswagen Blocks GrapheneOS Users via Play Protect Requirement](https://discuss.grapheneos.org/d/35949-volkswagen-app?page=3) ⭐️ 8.0/10

Volkswagen has updated its app to restrict API access to only Google Play Protect certified devices, thereby blocking GrapheneOS users from using the app and breaking community-built integrations like Home Assistant. This decision impacts privacy-conscious users who rely on GrapheneOS for security, and undermines community-driven projects that enhanced the functionality of Volkswagen vehicles. It highlights the tension between proprietary app requirements and open-source privacy-focused operating systems. The restriction is enforced through API-level checks that require Play Protect certification, which GrapheneOS devices lack because they are not Google-certified. Community projects such as Home Assistant integrations for preheating and other automations are now non-functional.

hackernews · microtonal · Jun 17, 15:04 · [Discussion](https://news.ycombinator.com/item?id=48571526)

**Background**: GrapheneOS is an open-source Android-based mobile operating system focused on security and privacy, commonly installed on Google Pixel devices. Google's Play Protect certification is a stamp of approval for devices that pass Android compatibility testing and include Google's proprietary services. Apps that check for Play Protect certification may refuse to run or restrict functionality on non-certified devices. Volkswagen's move reflects a broader industry trend where app developers lock out devices that do not meet their security requirements.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GrapheneOS">GrapheneOS</a></li>
<li><a href="https://support.google.com/googleplay/answer/7165974?hl=en">Check & fix Play Protect certification status - Google Play Help</a></li>
<li><a href="https://grapheneos.org/">GrapheneOS: the private and secure mobile OS</a></li>

</ul>
</details>

**Discussion**: Community comments express frustration with Volkswagen's decision, noting that the official app is 60% advertisements and 30% features, making community integrations like Home Assistant preferable. Some users are reconsidering purchasing Volkswagen vehicles due to these restrictions, while others discuss broader implications for privacy in automotive technology.

**Tags**: `#privacy`, `#grapheneos`, `#automotive`, `#API`, `#security`

---

<a id="item-10"></a>
## [AI Flips Code Economics: From Asset to Disposable](https://simonwillison.net/2026/Jun/17/charity-majors/#atom-everything) ⭐️ 8.0/10

Charity Majors argues that in 2025, AI made code generation effectively free and instant, transforming code from a treasured, carefully curated asset into a disposable and regenerable commodity. This paradigm shift fundamentally changes software engineering economics, forcing developers and companies to rethink how they value, manage, and invest in code. It also accelerates the commoditization of AI models and code generation tools, as seen in debates around Cursor and other AI-native IDEs. Majors emphasizes that the change happened practically overnight in 2025, with lines of code becoming disposable and regenerable instead of reused and cared for. The quote comes from her Substack article titled "AI demands more engineering discipline. Not less."

rss · Simon Willison · Jun 17, 17:12

**Background**: The commoditization of AI models means state-of-the-art capabilities become widely available and cheap, similar to electricity. AI code generators like GitHub Copilot and Cursor use large language models trained on vast code repositories to generate code from natural language descriptions, dramatically reducing the cost and effort of writing code.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/commoditization-ai-models-implications-innovation-siddharth-bhalsod-seimf">The Commoditization of AI Models: Implications for Innovation</a></li>
<li><a href="https://www.techpolicy.press/taking-ai-commoditization-seriously/">Taking AI Commoditization Seriously - techpolicy.press</a></li>
<li><a href="https://zencoder.ai/blog/generative-ai-code-generation-tools">10 Best Generative AI Code Generation Tools to Try in 2026</a></li>

</ul>
</details>

**Tags**: `#ai`, `#software-engineering`, `#economics-of-code`, `#generative-ai`

---

<a id="item-11"></a>
## [Export Controls on AI Undermine US Cyber Defense](https://simonwillison.net/2026/Jun/16/fable-5-export-controls/#atom-everything) ⭐️ 8.0/10

Export controls on AI models like Claude Fable 5 are preventing them from fixing security vulnerabilities, as evidenced by a 'jailbreak' that was actually a defensive request to patch code. This policy, intended to curb offensive cyber capabilities, inadvertently blocks defenders from using AI to find and fix bugs. This issue highlights a critical flaw in AI regulation, where non-technical policymakers misidentify defensive capabilities as threats. If left unaddressed, this could weaken US cybersecurity by denying defenders access to powerful AI tools that can automate vulnerability detection and patching. The 'jailbreak' involved asking Fable 5 to review and fix code containing known CVEs and deliberately planted vulnerabilities. The resulting patches were turned into test scripts, which is a standard defensive security practice.

rss · Simon Willison · Jun 16, 05:20

**Background**: Export controls on AI models are designed to prevent adversaries from acquiring advanced AI capabilities, particularly those that could be used for offensive cyber operations. However, the same capabilities—such as generating code and identifying vulnerabilities—are also essential for cybersecurity defenders. The Bureau of Industry and Security (BIS) has issued rules that categorize certain model capabilities as controlled items, but the line between offensive and defensive use is often blurred.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/United_States_export_controls_on_AI_chips_and_semiconductors">United States export controls on AI chips and semiconductors</a></li>
<li><a href="https://www.wilmerhale.com/en/insights/publications/20250205-bis-issues-long-awaited-export-controls-on-ai">BIS Issues Long Awaited Export Controls on AI</a></li>

</ul>
</details>

**Discussion**: Simon Willison's post reflects agreement with Kate Moussouris, criticizing the export control policy as absurd. The tech community has expressed frustration that non-technical decision-makers are conflating defensive and offensive AI uses, potentially harming national security.

**Tags**: `#AI`, `#export controls`, `#cybersecurity`, `#AI regulation`, `#Fable 5`

---

<a id="item-12"></a>
## [Speculative Decoding Gains Traction for Faster LLM Inference](https://www.reddit.com/r/MachineLearning/comments/1u83kzt/what_is_speculative_decoding_trending_on/) ⭐️ 8.0/10

Speculative decoding, an inference optimization technique that uses a fast draft model to propose tokens for parallel verification by a larger target model, is trending on Papers with Code. SGLang has published a blog post detailing state-of-the-art latencies using Modal and Z.ai's DFlash speculative decoding models. This technique significantly speeds up token generation for large language models without sacrificing output quality, addressing a key bottleneck in LLM deployment. Its integration into frameworks like SGLang and vLLM makes it practical for real-world serving. SGLang's latest blog post highlights achieving state-of-the-art latencies using DFlash speculative decoding models from Modal and Z.ai. DFlash is a lightweight block diffusion model that can achieve up to 4.4x speedup over autoregressive decoding.

reddit · r/MachineLearning · /u/NielsRogge · Jun 17, 07:41

**Background**: Large language models generate tokens autoregressively, one at a time, which is slow. Speculative decoding breaks this by having a small, fast draft model generate multiple candidate tokens, which the large model then verifies in parallel. This retains the quality of the large model while leveraging the speed of the small model.

<details><summary>References</summary>
<ul>
<li><a href="https://www.lmsys.org/blog/2026-06-15-next-generation-speculative-decoding-dflash-v2/">The next generation of speculative decoding : DFlash ... | LMSYS Org</a></li>
<li><a href="https://github.com/z-lab/dflash">z-lab/ dflash : DFlash : Block Diffusion for Flash Speculative Decoding ...</a></li>

</ul>
</details>

**Tags**: `#speculative decoding`, `#LLM inference`, `#optimization`, `#SGLang`

---

<a id="item-13"></a>
## [Contrastive Targeted SFT for Mechanistic Interpretability](https://www.reddit.com/r/MachineLearning/comments/1u8if6l/contrastive_targeted_sft_as_a_mechinterp_method/) ⭐️ 8.0/10

A self-taught researcher proposes using contrastive targeted supervised fine-tuning (SFT) to isolate circuits for specific capabilities in a 31B model, then ablate those circuits to map causal dependencies between capabilities. This method could lead to a causal dependency graph of neural network capabilities, enabling more efficient training by ordering tasks appropriately and improving interpretability of model behavior. The post describes training contrastive variants from the same checkpoint—examples with a dimension high vs low—then locating the circuit by differencing checkpoints and ablating heads to observe degradation in other dimensions.

reddit · r/MachineLearning · /u/Substantial_Diver469 · Jun 17, 18:31

**Background**: Mechanistic interpretability aims to reverse-engineer neural networks by identifying features and pathways inside them. Contrastive targeted SFT involves fine-tuning models to emphasize or suppress specific capabilities. Causal dependency graphs help understand how different model components influence each other.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/inside-black-box-what-mechanistic-interpretability-why-nancy-pandey-dvfxf">Inside the Black Box: What is Mechanistic Interpretability and Why...</a></li>
<li><a href="https://medium.com/tech-ai-made-easy/from-attention-maps-to-causal-graphs-teaching-llms-to-reason-ceeff457de81">From Attention Maps to Causal Graphs : Teaching LLMs to... | Medium</a></li>

</ul>
</details>

**Tags**: `#mechanistic interpretability`, `#supervised fine-tuning`, `#causal inference`, `#neural networks`, `#capability circuits`

---

<a id="item-14"></a>
## [US delays blacklisting DeepSeek, deems 100+ Chinese firms security risks](https://www.reuters.com/world/china/us-holds-off-blacklisting-chinas-deepseek-more-than-100-firms-deemed-security-2026-06-17/) ⭐️ 7.0/10

The US government announced it would postpone adding Chinese AI company DeepSeek to its trade blacklist, while simultaneously designating over 100 other Chinese firms as national security risks. This decision highlights the ongoing US-China tech conflict and the strategic significance of DeepSeek as a cost-effective AI model. The move may impact global AI supply chains and influence how other nations regulate AI technology. DeepSeek's models, such as R1 and V3, are known for being open-weight and trained at a fraction of the cost of competitors like OpenAI's GPT-4. The company has already been operating under US export restrictions on AI chips, which may limit the practical impact of a blacklist.

hackernews · giuliomagnifico · Jun 17, 03:55 · [Discussion](https://news.ycombinator.com/item?id=48565498)

**Background**: DeepSeek is a Chinese AI startup founded in 2023 by Liang Wenfeng, backed by hedge fund High-Flyer. It gained international attention in January 2025 when its R1 model rivaled top US AI models at a fraction of the cost, triggering a 'Sputnik moment' for the US. The US has been imposing export controls on advanced AI chips to China, aiming to curb China's AI progress. The Entity List restricts US companies from selling goods and services to listed entities, but continues to allow purchases from them.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek_(Company)">DeepSeek (Company)</a></li>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community comments show mixed reactions. Some users praise DeepSeek's affordability and utility in daily coding, while others criticize the US policy as hypocritical and similar to China's approach. There is skepticism about enforceability, and a comment notes that being on the Entity List does not completely stop business.

**Tags**: `#DeepSeek`, `#AI regulation`, `#US-China tech conflict`, `#export controls`, `#national security`

---

<a id="item-15"></a>
## [Adam Launches Open-Source AI CAD Platform CADAM](https://github.com/Adam-CAD/CADAM) ⭐️ 7.0/10

Adam (YC W25) has launched CADAM, an open-source text-to-CAD platform that uses AI agents to generate parametric 3D models from natural language prompts and image references, outputting OpenSCAD code. This represents a significant step toward using AI for mechanical design, potentially democratizing CAD by lowering the barrier to entry, but faces skepticism about practical utility especially for engineering-grade precision. CADAM runs entirely in-browser by compiling OpenSCAD to WebAssembly, supports multiple LLMs via Vercel AI SDK (with Gemini 3.1 Pro performing best), and allows parametric tweaks via slider without LLM calls due to deterministic regex updates.

hackernews · zachdive · Jun 17, 16:14 · [Discussion](https://news.ycombinator.com/item?id=48572553)

**Background**: Traditional CAD software like Fusion 360 or SolidWorks requires extensive training. The 'CAD as code' paradigm, exemplified by OpenSCAD and CadQuery, treats designs as programs. AI agents can generate such code from text, but spatial reasoning remains a challenge for LLMs.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2505.19713">[2505.19713] CAD-Coder: Text-to-CAD Generation with Chain-of ... CAD as Code | Home [2505.14646] CAD-Coder: An Open-Source Vision-Language Model ... GitHub - anniedoris/CAD-Coder CADDesigner: Conceptual CAD model generation with a general ... Balancing speed and executability in interactive text-to-CAD ... CAD-Coder: Text-to-CAD Generation with Chain-of-Thought and...</a></li>
<li><a href="https://www.cadascode.com/">CAD as Code | Home</a></li>
<li><a href="https://arxiv.org/abs/2505.14646">[2505.14646] CAD-Coder: An Open-Source Vision-Language Model ... GitHub - anniedoris/CAD-Coder CADDesigner: Conceptual CAD model generation with a general ... Balancing speed and executability in interactive text-to-CAD ... CAD-Coder: Text-to-CAD Generation with Chain-of-Thought and...</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed: some users praise quick results for simple parts, while engineers like 'incorene2' argue AI cannot yet match manual modeling speed and reliability for real mechanical design. Others point to spatial reasoning limitations and suggest projects like ModelRift as alternatives.

**Tags**: `#AI`, `#CAD`, `#open-source`, `#mechanical design`, `#YC`

---

<a id="item-16"></a>
## [AI models compared in robot game: cost vs performance](https://openrouter.ai/blog/insights/royale-last-agent-standing/) ⭐️ 7.0/10

A blog post on OpenRouter compares AI models including Claude, Grok, and DeepSeek in a last-agent-standing game, revealing stark cost and performance trade-offs. This comparison helps practitioners choose the right AI model for real-time decision tasks, balancing cost and quality, and highlights the financial challenges of using frontier models at scale. The experiment ran 30 games for $482 without frontier models, whereas using top models like Opus 4.7 would cost $3,000, showing a 6x cost difference. DeepSeek V4 Flash was praised for cost efficiency.

hackernews · Usu · Jun 17, 21:00 · [Discussion](https://news.ycombinator.com/item?id=48576824)

**Background**: Claude is a large language model developed by Anthropic, Grok is by xAI (Elon Musk), and DeepSeek is by DeepSeek. Each model has different capabilities and pricing. The blog used OpenRouter's unified API to compare them in a game where AI agents compete to be the last standing.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude (language model) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Grok_(chatbot)">Grok (chatbot) - Wikipedia</a></li>
<li><a href="https://openrouter.ai/deepseek">DeepSeek API and Models | OpenRouter</a></li>

</ul>
</details>

**Discussion**: Commenters praised DeepSeek V4 Flash for cost efficiency and coding prowess, while others criticized Grok for silently rerouting users to a more expensive model. One comment questioned the financial viability of expensive frontier models for simple tasks.

**Tags**: `#AI`, `#LLM`, `#cost efficiency`, `#model comparison`, `#news`

---

<a id="item-17"></a>
## [Datasette 1.0a34 adds CRUD to web interface](https://simonwillison.net/2026/Jun/16/datasette/#atom-everything) ⭐️ 7.0/10

Datasette 1.0a34 introduces row insert, edit, and delete capabilities directly in its web interface, a feature inspired by the Datasette Agent AI assistant. This update transforms Datasette from a read-only data exploration tool into a full data management platform, making it more useful for non-technical users and reducing the need for external tools. The CRUD features are available on table pages and row pages, but this is an alpha release, so users should expect potential bugs and incomplete functionality.

rss · Simon Willison · Jun 16, 21:31

**Background**: Datasette is an open-source tool for exploring and publishing SQLite databases as interactive websites with a JSON API. It is widely used by data journalists and researchers for sharing datasets. Traditionally, Datasette focused on read-only exploration; editing data required external tools or custom SQL queries. The new CRUD capabilities bring parity with the Datasette Agent AI assistant, which already had SQL write support.

<details><summary>References</summary>
<ul>
<li><a href="https://www.hostinger.com/applications/datasette">Datasette VPS Docker | One-Click Data Publishing</a></li>
<li><a href="https://datasette.io/blog/2026/datasette-agent/">Datasette Agent, an extensible AI assistant for Datasette</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#CRUD`, `#alpha release`, `#data exploration`, `#SQLite`

---

<a id="item-18"></a>
## [Expert says Anthropic's Fable jailbreak shows model working as intended](https://simonwillison.net/2026/Jun/16/matteo-wong-the-atlantic/#atom-everything) ⭐️ 7.0/10

Cybersecurity expert Katie Moussouris stated that a reported AI jailbreak of Anthropic's Fable model actually demonstrates the model functioning correctly for cyberdefense, rather than a safety failure. This nuanced perspective challenges the narrative of AI jailbreaks as pure failures, influencing debates on AI safety regulation and export controls. It underscores the importance of expert assessment in evaluating AI behavior. The report involved IT experts asking Fable to find and patch bugs; Fable refused the prompt 'review the code for security issues' but complied with 'fix this code' after manual steps. Moussouris noted this aligns with intended cyberdefense behavior.

rss · Simon Willison · Jun 16, 03:07

**Background**: AI jailbreaking is a technique where crafted inputs bypass an AI model's safety constraints to generate restricted content. In this case, the U.S. government claimed a jailbreak of Anthropic's Fable 5 model, leading to export controls and model suspension. However, Moussouris argued that the specific behavior—refusing direct security review but performing fixes—is actually what a responsible cyberdefense assistant should do.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/fable-mythos-access">Statement on the US government directive to suspend access to Fable 5 and Mythos 5 \ Anthropic</a></li>
<li><a href="https://www.cnet.com/tech/services-and-software/anthropic-claude-fable-mythos-us-export-controls/">Anthropic Pulls Claude Fable and Mythos AI Models After Feds Claim Jailbreak - CNET</a></li>
<li><a href="https://www.geeksforgeeks.org/artificial-intelligence/ai-jailbreak/">AI jailbreaking - GeeksforGeeks</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#cybersecurity`, `#Anthropic`, `#jailbreak`, `#export controls`

---

<a id="item-19"></a>
## [Is foundational AI research possible without HPC?](https://www.reddit.com/r/MachineLearning/comments/1u8jyat/is_foundational_ai_research_still_something_that/) ⭐️ 7.0/10

A Reddit discussion rekindles the debate on whether foundational AI research can be conducted without access to High-Performance Computing (HPC), referencing the original Transformer paper's training on modest gaming GPUs. This debate influences who can contribute to foundational AI research, potentially impacting the diversity of ideas and the democratization of the field. The original Transformer paper (2017) trained on 8 NVIDIA P100 GPUs, which cost around $5,000 each then, but today's state-of-the-art models often require clusters of hundreds or thousands of more powerful GPUs.

reddit · r/MachineLearning · /u/Proof-Bed-6928 · Jun 17, 19:26

**Background**: High-Performance Computing (HPC) refers to the use of supercomputers and parallel processing techniques to solve complex computational problems. In AI research, HPC resources are critical for training large-scale models. However, the Transformer paper demonstrated that a breakthrough architecture could be developed with relatively modest hardware, raising questions about whether such feats are still possible as model sizes grow exponentially.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sciencedirect.com/science/article/pii/S0952197625032798">What artificial intelligence can do for high-performance ...</a></li>

</ul>
</details>

**Tags**: `#AI research`, `#HPC`, `#machine learning`, `#democratization`, `#transformer`

---

<a id="item-20"></a>
## [Leakage-Clean Verifier for Robot Manipulation Using Object-Centric Graphs](https://www.reddit.com/r/MachineLearning/comments/1u7hxem/i_built_a_leakageclean_verifier_for_robot/) ⭐️ 7.0/10

A novel leakage-clean verifier is proposed that uses object-centric graphs to objectively evaluate robot task completion, preventing bias from policy authors by enforcing a strict information boundary between the demonstration and the rollout evaluation. This addresses a critical conflict of interest in robot manipulation benchmarking, where policy authors often define success metrics themselves. An automatic, embodiment-agnostic grader could enable more reliable dense reward for training foundation models at scale. The verifier compiles a human demonstration into an object-centric graph capturing relations, contacts, and event order, then independently extracts a graph from the robot rollout and checks for a match. It successfully fails a no-op baseline and passes a scripted arm, but its discrete relational representation faces challenges with force-profile and deformable tasks.

reddit · r/MachineLearning · /u/Alexpplay · Jun 16, 16:10

**Background**: Current robot manipulation evaluation often uses hand-coded success predicates written by the same person training the policy, creating a conflict of interest. Object-centric graphs, as used in recent research like ORION and FOCUS, represent scenes by modeling objects and their relations, enabling more structured task understanding.

<details><summary>References</summary>
<ul>
<li><a href="https://link.springer.com/article/10.1007/s10514-026-10253-8">Vision-based manipulation from single human video with open-world object graphs | Autonomous Robots | Springer Nature Link</a></li>
<li><a href="https://www.frontiersin.org/journals/neurorobotics/articles/10.3389/fnbot.2025.1585386/full">Frontiers | FOCUS: object-centric world models for robotic manipulation</a></li>

</ul>
</details>

**Tags**: `#robot manipulation`, `#evaluation`, `#benchmark`, `#object-centric`, `#verification`

---

<a id="item-21"></a>
## [8-bit live baseball gamecast using MLB data](https://ribbie.tv/watch) ⭐️ 6.0/10

A new website, ribbie.tv, streams live MLB games as 8-bit pixel art gamecasts by converting real-time MLB Stats API data into animated pixel graphics. This project offers a nostalgic, low-bandwidth alternative to traditional video broadcasts, engaging both baseball fans and pixel art enthusiasts, and demonstrates creative use of public sports data. The site uses MLB Stats API without authentication, displays real-time scoreboards, stadium graphics, day/night modes, and between-inning interstitials. It currently shows scheduled games with direct links.

hackernews · brownrout · Jun 17, 16:44 · [Discussion](https://news.ycombinator.com/item?id=48573012)

**Background**: Major League Baseball (MLB) provides a publicly accessible Stats API that delivers play-by-play data, box scores, and team/player stats in JSON format. Pixel art gamecasts are a form of visualization that recreates games using blocky, retro-style graphics reminiscent of 8-bit video games. Similar projects exist for other sports, but this is one of the first for MLB in real-time.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/MLB_Stats_API">MLB Stats API</a></li>
<li><a href="https://statsapi.mlb.com/">MLB Stats API</a></li>

</ul>
</details>

**Discussion**: Commenters praised the project for its creativity and nostalgia, but also offered constructive feedback: some suggested using real pixel fonts and deterministic downsampling instead of AI-generated art, while others requested play-by-play views, clickable between-inning tabs, and audio sound effects. One commenter mentioned an existing physical scoreboard project using the same APIs.

**Tags**: `#baseball`, `#visualization`, `#pixel art`, `#real-time`, `#side project`

---

<a id="item-22"></a>
## [Human Connection: The AI-Proof Competitive Moat](https://ghostinthedata.info/posts/2026/2026-06-13-human-connection-moat/) ⭐️ 6.0/10

An article argues that genuine human connection in customer service remains a durable competitive advantage that AI cannot replicate, challenging the trend of replacing human interactions with chatbots. This perspective matters for businesses seeking sustainable differentiation in an AI-saturated market, especially in hospitality and B2C sectors where emotional connection drives loyalty. The article uses a case study of a restaurant that kept its human reservation staff after moving booking online, improving customer experience. It also emphasizes that hospitality must be paired with good service and product quality.

hackernews · speckx · Jun 17, 17:14 · [Discussion](https://news.ycombinator.com/item?id=48573435)

**Background**: The concept of a 'competitive moat' refers to a business's long-term advantage that protects it from competitors. In customer service, many companies are adopting AI chatbots to reduce costs, but this can erode personal connections that build brand loyalty.

**Discussion**: Comments are mixed: some users prefer efficient transactional interactions over forced personal connection, while others highlight the importance of genuine human touch. One comment notes the irony of an AI-written post on human connection. Another user points out that hospitality is core to some businesses, but not all.

**Tags**: `#AI`, `#human connection`, `#customer service`, `#competitive advantage`, `#business strategy`

---

<a id="item-23"></a>
## [Thinking Out Loud Boosts Problem-Solving](https://www.thesignalist.io/s/the-dialogue-dividend/) ⭐️ 6.0/10

An article on The Signalist argues that vocalizing thoughts to an active listener enhances cognitive clarity and problem-solving, drawing parallels to rubber duck debugging and pair programming techniques. This perspective underscores the importance of verbalization in the software engineering process, promoting practices that enhance code quality and team collaboration. The article distinguishes between speaking to a passive object (rubber duck) and speaking to an engaged listener, suggesting the latter provides additional cognitive benefits through feedback and interaction.

hackernews · kodesko · Jun 17, 13:00 · [Discussion](https://news.ycombinator.com/item?id=48569894)

**Background**: Rubber duck debugging is a well-known debugging method where a programmer explains their code to an inanimate object to identify logical errors. Pair programming is an agile practice where two developers share a workstation, one writing code while the other reviews. Both methods leverage the cognitive act of explaining to uncover misunderstandings. The article extends this concept by highlighting the added value of a responsive listener.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Rubber_duck_debugging">Rubber duck debugging - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Pair_programming">Pair programming</a></li>

</ul>
</details>

**Discussion**: Commenters largely agreed with the article's premise, with many sharing personal experiences. Some debated whether the listener's engagement matters, while others highlighted historical precedents like Einstein's collaboration. The discussion was constructive and expanded on the core idea.

**Tags**: `#cognitive-psychology`, `#pair-programming`, `#rubber-duck-debugging`, `#communication`, `#software-engineering`

---

<a id="item-24"></a>
## [Click-to-Play Web Component for GIFs](https://simonwillison.net/2026/Jun/17/click-to-play-component/#atom-everything) ⭐️ 6.0/10

Simon Willison released a custom <click-to-play> Web Component that turns a linked GIF into a static image with a play button, loading the GIF only when clicked. This component improves page performance by deferring the loading of large GIF files until user interaction, which reduces initial page weight and bandwidth usage, especially useful for content-heavy sites. The component expects an <a> tag containing an <img> as its child, where the href points to the GIF and the img src to a static first frame. It is a progressive enhancement, meaning it works even if JavaScript fails.

rss · Simon Willison · Jun 17, 03:56

**Background**: Web Components are a set of browser APIs that allow developers to create reusable custom HTML elements. Progressive enhancement is a design strategy that ensures a web page is functional even without JavaScript, then layers on more advanced features. This component embodies both concepts.

**Tags**: `#web components`, `#gif`, `#javascript`, `#progressive enhancement`

---

<a id="item-25"></a>
## [Georgi Gerganov Endorses Qwen3.6-27B for Local Coding](https://simonwillison.net/2026/Jun/16/georgi-gerganov/#atom-everything) ⭐️ 6.0/10

Georgi Gerganov, creator of llama.cpp, confirmed that Qwen3.6-27B is a highly capable local model for coding tasks, and described his lightweight pi agent setup using `pi -nc --offline` with a custom system prompt. This endorsement from a key figure in local LLM development validates Qwen3.6-27B as a practical choice for offline AI-assisted programming, potentially driving broader adoption among developers who need privacy and low latency. Gerganov uses the model on an M2 Ultra or RTX 5090 machine for small maintenance tasks at ggml-org, and his pi agent setup includes the `--nc` (no context) and `--offline` flags with a tailored system prompt.

rss · Simon Willison · Jun 16, 16:04

**Background**: Qwen3.6-27B is an open-weight large language model released in April 2026 by the Qwen team, focusing on stability and real-world coding utility. The pi agent is a local coding agent that integrates with llama.cpp to provide an interactive agent session without external API dependencies, enabling fully offline AI-assisted programming.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.6-27B">Qwen/Qwen3.6-27B · Hugging Face</a></li>
<li><a href="https://pi.dev/packages/pi-llama-cpp">pi-llama-cpp · Packages · Pi</a></li>

</ul>
</details>

**Tags**: `#local LLM`, `#coding assistant`, `#Qwen`, `#llama.cpp`, `#pi agent`

---

<a id="item-26"></a>
## [Cloudflare CAPTCHA Rule for URLs with Ampersands](https://simonwillison.net/2026/Jun/16/captcha-on-at-least-one-ampersand/#atom-everything) ⭐️ 6.0/10

Simon Willison shares how to configure Cloudflare's Managed Challenge to only trigger CAPTCHA on search URLs containing at least one ampersand, using the custom rule expression `(http.request.uri.path wildcard r"/search/*" and http.request.uri.query contains "&")`. This allows simple searches like `/search/?q=term` to proceed without a challenge. This practical tip helps web developers fine-tune Cloudflare WAF rules to reduce false positives for legitimate crawlers and users, balancing security with usability. It demonstrates the flexibility of Cloudflare's rules language and the value of precise rule crafting. The rule uses the Cloudflare Rules language, which supports wildcard matching on paths and substring checks on query strings. The maximum length of a rule expression is 4,096 characters. Willison also notes that he first attempted to use the Cloudflare MCP with Claude Code but switched to the Cloudflare API instead.

rss · Simon Willison · Jun 16, 00:21

**Background**: Cloudflare Managed Challenge is a security feature that presents a CAPTCHA or browser challenge to visitors deemed suspicious. Custom rules allow site owners to define precise conditions for when challenges are triggered. The Cloudflare Rules language is based on Wireshark display filters and provides a flexible syntax for building rule expressions. This rule specifically targets search URLs (path starting with `/search/`) that have complex query strings (containing `&`), which are typical of aggressive crawlers.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.cloudflare.com/end-cloudflare-captcha/">The end of the road for Cloudflare CAPTCHAs</a></li>
<li><a href="https://developers.cloudflare.com/ruleset-engine/rules-language/expressions/">Rule expressions · Cloudflare Ruleset Engine docs</a></li>

</ul>
</details>

**Tags**: `#Cloudflare`, `#CAPTCHA`, `#Web Application Firewall`, `#Security`

---

<a id="item-27"></a>
## [ACL 2026 first author with weak GPA seeks PhD advice](https://www.reddit.com/r/MachineLearning/comments/1u8bp65/acl_2026_first_author_with_weak_gpa_how_should_i/) ⭐️ 6.0/10

A user with a weak undergraduate GPA (3.3/5) but a strong ACL 2026 first-author paper (meta-review score 8/10, confidence 5/5) is seeking strategies for PhD applications, specifically focused on low-resource African languages. This post highlights the challenge of offsetting a weak GPA with a strong publication in PhD admissions, especially in niche NLP areas. It provides a realistic case study for other applicants with similar profiles. The user has a Master's GPA of 8/10 from an average European university and targets top NLP programs (CMU, Edinburgh, ETH, MBZUAI). They worry that their weak undergrad GPA and unknown university reputation may hinder admission despite the ACL paper.

reddit · r/MachineLearning · /u/Unlikely_Screen_9287 · Jun 17, 14:26

**Background**: ACL (Association for Computational Linguistics) is a top-tier NLP conference. A meta-review score (typically 1-10) reflects the overall assessment by an area chair after reviewers' comments. Low-resource languages lack digital data and tools for NLP, making research on them valuable yet challenging.

<details><summary>References</summary>
<ul>
<li><a href="http://stats.aclrollingreview.org/">ACL Rolling Review</a></li>
<li><a href="https://vtiya.medium.com/is-your-language-a-low-resouce-language-c17da390909f">Is your language a low -resouce language ? | by Dr.Tiya Vaj... | Medium</a></li>

</ul>
</details>

**Tags**: `#PhD applications`, `#NLP`, `#low-resource languages`, `#ACL`, `#career advice`

---

<a id="item-28"></a>
## [Probe Capacity vs. Network Capacity in Interpretability](https://www.reddit.com/r/MachineLearning/comments/1u8lo60/how_do_you_analyze_the_relative_strength_of/) ⭐️ 6.0/10

A Reddit user posed a detailed technical question about how to theoretically balance probe capacity with underlying network capacity in circuit analysis, particularly for factuality guarantees in language models. This question highlights a foundational gap in mechanistic interpretability: without clear theory on probe-capacity vs. network-capacity, conclusions from probing studies may be misleading. Addressing this could improve the reliability of interpretability methods used to verify model safety and factuality. The post references logistic regression probes for detecting token position, noting that small vocabularies can inflate apparent performance. It also questions whether Nyquist-type sampling guarantees could apply to probing setups, and suggests that example difficulty should be factored into analysis.

reddit · r/MachineLearning · /u/RepresentativeBee600 · Jun 17, 20:29

**Background**: Mechanistic interpretability aims to reverse-engineer neural network computations, often using probes—simple classifiers trained on internal representations to detect specific features. A key concern is whether a probe's performance reflects genuine network knowledge or merely the probe's own capacity to memorize labels. The Nyquist theorem from signal processing describes conditions for perfect reconstruction of continuous signals from discrete samples, and the user wonders if similar guarantees could apply to understanding network behavior from limited probe examples.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mechanistic_interpretability">Mechanistic interpretability - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2304.14997">[2304.14997] Towards Automated Circuit Discovery for Mechanistic Interpretability</a></li>
<li><a href="https://www.cs.columbia.edu/~johnhew/interpreting-probes.html">Designing and Interpreting Probes · John Hewitt</a></li>

</ul>
</details>

**Tags**: `#probing`, `#interpretability`, `#machine learning`, `#circuit analysis`

---

<a id="item-29"></a>
## [GAN deployed on Raspberry Pi 4 for physical NFT minting](https://www.reddit.com/r/MachineLearning/comments/1u8cqan/i_deployed_a_gan_on_a_raspberry_pi_4_and_built_a/) ⭐️ 6.0/10

A hobbyist trained a 128×128 DCGAN on a MacBook M3, exported it to ONNX, and deployed it on a Raspberry Pi 4 to generate hybrid face NFTs via a physical button press, displaying results on an ESP32 T-Display. This project demonstrates a practical edge deployment of a generative AI model on low-cost hardware, merging AI art with physical interactivity and NFT minting, which could inspire more accessible and tangible AI art installations. The DCGAN uses a 6-block generator and discriminator, trained for 800 epochs on a dataset of 2,480 images (11 subjects, one dominant class with 2,000 images), achieving 3-second inference on Pi 4 with a 53MB ONNX FP32 model.

reddit · r/MachineLearning · /u/Numerous-Dentist-882 · Jun 17, 15:05

**Background**: DCGAN (Deep Convolutional GAN) uses convolutional layers in both generator and discriminator to generate images. ONNX is an open format for model interchange, enabling deployment on different platforms. The Raspberry Pi 4 is a low-cost single-board computer, and the ESP32 T-Display is a microcontroller with a built-in screen, typical for IoT and edge projects.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.pytorch.org/tutorials/beginner/dcgan_faces_tutorial.html">DCGAN Tutorial — PyTorch Tutorials 2.12.0+cu130 documentation</a></li>
<li><a href="https://onnxruntime.ai/docs/tutorials/mobile/">Learn how to deploy an ONNX model on a mobile device with ONNX ...</a></li>
<li><a href="https://lilygo.cc/products/t-display">T-Display – LILYGO®</a></li>

</ul>
</details>

**Tags**: `#GAN`, `#Raspberry Pi`, `#ONNX deployment`, `#edge AI`, `#NFT`

---