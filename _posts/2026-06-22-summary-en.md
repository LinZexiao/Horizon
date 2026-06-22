---
layout: default
title: "Horizon Summary: 2026-06-22 (EN)"
date: 2026-06-22
lang: en
---

> From 27 items, 14 important content pieces were selected

---

1. [Valve Launches Steam Machine Gaming Hardware](#item-1) ⭐️ 9.0/10
2. [Study: Half of LG Smart TV Apps Contain Residential Proxy SDKs](#item-2) ⭐️ 8.0/10
3. [Moebius: 0.2B parameter inpainting model claims 10B-level performance](#item-3) ⭐️ 8.0/10
4. [Canada plans up to 10 new nuclear reactors in 15 years](#item-4) ⭐️ 8.0/10
5. [Police chiefs misuse Flock cameras to stalk women, warrant debate reignited](#item-5) ⭐️ 8.0/10
6. [Hugging Face Revives Papers with Code with New Features](#item-6) ⭐️ 8.0/10
7. [sqlite-utils 4.0rc1 adds migrations and nested transactions](#item-7) ⭐️ 7.0/10
8. [Cloudflare Debuts Temporary Accounts for Workers](#item-8) ⭐️ 7.0/10
9. [Matrix Recurrent Units Update: Stability and Performance Analysis](#item-9) ⭐️ 7.0/10
10. [Oak: Git Alternative Optimized for AI Agents with Virtual Mounts](#item-10) ⭐️ 6.0/10
11. [Seeking Literature on Syntax-Robust NLI for Diffusion LLMs](#item-11) ⭐️ 6.0/10
12. [Improved DVD-JEPA Demo Adds Noise and Baseline](#item-12) ⭐️ 6.0/10
13. [Best methods for fine-tuning Whisper on domain-specific Spanish](#item-13) ⭐️ 6.0/10
14. [WeightsLab: Open-source tool for data-centric debugging](#item-14) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Valve Launches Steam Machine Gaming Hardware](https://store.steampowered.com/news/group/45479024/view/685257114654870245) ⭐️ 9.0/10

Valve officially launched the Steam Machine gaming hardware on June 22, 2026, with a randomized reservation system to ensure fair access and prevent scalping. The device runs SteamOS and emphasizes openness, allowing users to install their own operating system or apps. This launch marks Valve's major return to the living room console market, building on the Steam Deck's success. It could accelerate Linux gaming adoption and challenge traditional console ecosystems by offering an open, PC-like platform. The Steam Machine, codenamed Newell Nucleus, starts at over $1,000 across four models. The reservation system requires a Steam account in good standing with at least one purchase before April 17, 2026, and limits one unit per household to combat scalpers.

hackernews · theschwa · Jun 22, 17:09 · [Discussion](https://news.ycombinator.com/item?id=48632884)

**Background**: Valve previously attempted Steam Machines in 2015, but the initiative failed due to lack of focus and high prices. The Steam Deck's success later proved that a Linux-based gaming handheld could thrive. The new Steam Machine targets 4K gaming and seamless living room integration, running SteamOS 3.0 or later.

<details><summary>References</summary>
<ul>
<li><a href="https://www.lttlabs.com/articles/2026/06/22/the-newell-nucleus-steam-machine-ltt-companion-article">The Newell Nucleus: Steam Machine LTT Companion Article</a></li>
<li><a href="https://thephrasemaker.com/2026/06/22/steam-machine-price-revealed-starts-at-over-1000/">Steam Machine Price Revealed, Starts At Over $1,000 - Phrasemaker</a></li>
<li><a href="https://waterloow.com/2026/05/11/steam-machine-queue-system/">Steam Machine Queue System : How to Secure Yours - WaterLoow</a></li>

</ul>
</details>

**Discussion**: Community members praised the fair reservation system and the device's openness. One commenter highlighted an authentic gameplay clip as refreshing. Another expressed support for Linux gaming, having switched to Fedora full-time, though noted music production still requires Windows. Overall sentiment was positive, focusing on Valve's consumer-friendly approach.

**Tags**: `#gaming`, `#hardware`, `#valve`, `#steam`, `#linux`

---

<a id="item-2"></a>
## [Study: Half of LG Smart TV Apps Contain Residential Proxy SDKs](https://spur.us/blog/smart-tv-apps-residential-proxy-sdks) ⭐️ 8.0/10

A study by Spur found that nearly half of third-party apps on LG Smart TVs contain residential proxy SDKs, which can use the TV's IP address as a proxy without the owner's consent. This poses a serious privacy and security risk for millions of smart TV users, as their home IP addresses could be used for activities like web scraping or bypassing geo-restrictions without their knowledge. The study focused on third-party apps, not LG's built-in apps, and named Desoline and Bright Data as the top providers with the most proxy-flagged apps.

hackernews · microcode · Jun 22, 20:48 · [Discussion](https://news.ycombinator.com/item?id=48635954)

**Background**: A residential proxy routes internet traffic through an IP address assigned to a real household by an ISP, making the traffic appear as a genuine user. SDKs that enable such proxies can be embedded in apps, allowing the app developers to use the device's IP address as a proxy node, often without the user's explicit consent.

<details><summary>References</summary>
<ul>
<li><a href="https://spur.us/blog/what-is-a-residential-proxy">What Is a Residential Proxy? Definition, Risks & Detection - Spur</a></li>
<li><a href="https://techreviewadvisor.com/what-is-a-residential-proxy/">What Is a Residential Proxy? How It Works - Tech Review Advisor</a></li>

</ul>
</details>

**Discussion**: The community expressed strong concern, with users advising to never connect smart TVs to the internet or to isolate them on a separate VLAN. Some noted that this issue is specific to third-party apps, not the TV's native apps.

**Tags**: `#security`, `#privacy`, `#smart TV`, `#IoT`, `#residential proxy`

---

<a id="item-3"></a>
## [Moebius: 0.2B parameter inpainting model claims 10B-level performance](https://hustvl.github.io/Moebius/) ⭐️ 8.0/10

Moebius, a new image inpainting model with only 0.2 billion parameters, claims to achieve performance comparable to 10 billion parameter models. Community members have demonstrated browser-based inference using ONNX, though results show mixed quality. This model represents a significant efficiency gain, potentially enabling high-quality inpainting on resource-constrained devices. However, the claimed parity with 10B models is contested due to observed limitations in output quality and object diversity. Moebius is limited to 512x512 output resolution, and community tests reveal that inpainted regions are visibly smoother than surroundings, with poor performance on novel objects. A browser demo using ONNX requires downloading about 1.3GB of model data.

hackernews · DSemba · Jun 22, 13:53 · [Discussion](https://news.ycombinator.com/item?id=48630171)

**Background**: Image inpainting is the process of reconstructing missing or damaged parts of an image using AI, often employed in photo editing and restoration. ONNX (Open Neural Network Exchange) is an open standard for representing machine learning models, enabling interoperability across frameworks and facilitating browser-based inference via ONNX Runtime.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ONNX">ONNX</a></li>
<li><a href="https://en.wikipedia.org/wiki/Image_inpainting">Image inpainting</a></li>

</ul>
</details>

**Discussion**: User simonw successfully created a browser demo via ONNX, but james2doyle reported failures on all tested images. lifthrasiir noted that while impressive for 0.2B, the model does not match 10B models, with visibly smoother inpainted regions and poor novel object generation. pattilupone expressed interest in a version for manga translation, noting LaMa is outdated.

**Tags**: `#image inpainting`, `#efficient AI`, `#model compression`, `#browser inference`, `#ONNX`

---

<a id="item-4"></a>
## [Canada plans up to 10 new nuclear reactors in 15 years](https://www.cbc.ca/news/politics/federal-nuclear-strategy-9.7244509) ⭐️ 8.0/10

The Canadian government announced plans to build up to 10 new nuclear reactors over the next 15 years, leveraging its uranium reserves and CANDU reactor expertise. This marks a major national energy policy shift that could significantly boost clean baseload power, reduce carbon emissions, and strengthen Canada's position in the nuclear energy market. The reactors are expected to include both traditional CANDU designs and small modular reactors (SMRs), building on projects like the Darlington New Nuclear Project.

hackernews · geox · Jun 22, 19:06 · [Discussion](https://news.ycombinator.com/item?id=48634585)

**Background**: CANDU reactors are Canadian-developed pressurized heavy-water reactors that use natural uranium fuel without enrichment. They are known for safety and fuel efficiency, using 30-40% less uranium than light-water reactors. Canada has the world's largest uranium reserves and extensive experience in CANDU construction and refurbishment.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/CANDU_reactor">CANDU reactor</a></li>

</ul>
</details>

**Discussion**: The community largely supports the plan, citing Canada's uranium reserves, proven CANDU design, and need for clean baseload power. Some suggest using nuclear for Alberta's oil sands to reduce CO2, while others note the potential to supply the US. There is also excitement about the Darlington SMR project progress.

**Tags**: `#nuclear energy`, `#Canada`, `#energy policy`, `#clean energy`

---

<a id="item-5"></a>
## [Police chiefs misuse Flock cameras to stalk women, warrant debate reignited](https://ipvm.com/reports/police-chiefs-track) ⭐️ 8.0/10

An IPVM report exposes that police chiefs have used Flock license plate recognition cameras to personally stalk women, demonstrating the ease of abuse without warrant requirements. This incident underscores the urgent need for legal safeguards like warrant requirements for surveillance technologies, as misuse can directly harm individuals and violate privacy rights. It affects public trust in law enforcement and the broader debate on civil liberties. Flock cameras capture license plate data and vehicle features such as make, model, color, and unique identifiers like bumper stickers or damage, enabling searches without a plate number. The report specifically highlights cases where police chiefs used the system to track their personal interests.

hackernews · jhonovich · Jun 22, 19:13 · [Discussion](https://news.ycombinator.com/item?id=48634694)

**Background**: Automated License Plate Readers (ALPR) like Flock Safety's cameras are deployed by police and communities to monitor vehicles in real time, often without a warrant. They capture and store data on all passing vehicles, raising Fourth Amendment concerns about unreasonable search and seizure. Flock's Vehicle Fingerprint technology can identify vehicles even without plates, expanding surveillance capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Flock_Safety">Flock Safety - Wikipedia</a></li>
<li><a href="https://www.flocksafety.com/products/license-plate-readers">Flock Safety LPR Cameras: Automated License Plate Reader</a></li>

</ul>
</details>

**Discussion**: Commenters expressed alarm at the parallels to fictional surveillance scenarios, with one noting how a 'Men in Black' scene now feels unsettling. Others debated the trade-off between crime-solving benefits and privacy violations, with some suggesting contacting the ACLU to challenge these cameras as Fourth Amendment violations.

**Tags**: `#privacy`, `#surveillance`, `#fourth-amendment`, `#law-enforcement`, `#flock`

---

<a id="item-6"></a>
## [Hugging Face Revives Papers with Code with New Features](https://www.reddit.com/r/MachineLearning/comments/1ucm508/some_new_updates_to_papers_with_code_p/) ⭐️ 8.0/10

Hugging Face announced new features for Papers with Code, including SOTA badges, a trending score combining GitHub star velocity and Hugging Face artifact popularity, support for external evaluations, and an expanded set of benchmarks and tasks. This revival enhances research discovery and benchmarking in the ML community, making it easier to identify top-performing papers and track trends. The integration of Hugging Face ecosystem data adds a more comprehensive view of paper impact. The trending score now incorporates both GitHub star velocity and popularity of linked Hugging Face artifacts (models, datasets, Spaces). SOTA badges are displayed for papers ranked in the top 3 of a benchmark. External evals, a feature not present in the legacy site, allow viewing third-party evaluations.

reddit · r/MachineLearning · /u/NielsRogge · Jun 22, 14:29

**Background**: Papers with Code is a platform that tracks machine learning research papers and their associated code and benchmarks. It was originally a community-driven resource for linking papers to code and state-of-the-art results. Hugging Face acquired the platform in 2021 and is now revitalizing it with improved features.

<details><summary>References</summary>
<ul>
<li><a href="https://posttrainbench.com/">PostTrainBench</a></li>
<li><a href="https://www.datacamp.com/blog/glm-5-2">GLM-5.2: Features, Setup, Benchmarks, and Model Switching Guide</a></li>

</ul>
</details>

**Tags**: `#Papers with Code`, `#Machine Learning`, `#Research Tools`, `#Hugging Face`, `#Benchmarks`

---

<a id="item-7"></a>
## [sqlite-utils 4.0rc1 adds migrations and nested transactions](https://simonwillison.net/2026/Jun/21/sqlite-utils-40rc1/#atom-everything) ⭐️ 7.0/10

The release candidate for sqlite-utils v4 introduces built-in support for database migrations and a new db.atomic context manager for nested transactions, along with some backwards-incompatible changes. This update adds critical capabilities for managing database schema evolution and safe transactional operations, making sqlite-utils more suitable for production use. Users of the popular tool can now handle schema changes more systematically and use nested transactions to simplify complex workflows. The migrations system is a port of the existing sqlite-migrate package and does not support reverse migrations; mistakes must be fixed by adding new migrations. The db.atomic context manager provides a Pythonic way to use SQLite's savepoint-based nested transactions.

rss · Simon Willison · Jun 21, 23:35

**Background**: sqlite-utils is a Python library and CLI tool that provides higher-level operations on top of Python's built-in sqlite3 module, such as table transformations and automatic table creation from JSON. Nested transactions in SQLite are implemented via savepoints, which allow partial rollbacks within a larger transaction. The new migration system helps manage schema changes over time, a common need in application development.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/simonw/sqlite-utils">GitHub - simonw/sqlite-utils: Python CLI utility and library for manipulating SQLite databases · GitHub</a></li>
<li><a href="https://sqlite-utils.datasette.io/">sqlite-utils</a></li>
<li><a href="https://sqlite.org/lang_transaction.html">Transaction - SQLite</a></li>

</ul>
</details>

**Tags**: `#Python`, `#SQLite`, `#library`, `#database`, `#migrations`

---

<a id="item-8"></a>
## [Cloudflare Debuts Temporary Accounts for Workers](https://simonwillison.net/2026/Jun/21/temporary-cloudflare-accounts/#atom-everything) ⭐️ 7.0/10

Cloudflare announced that developers can now deploy Workers projects ephemerally without a permanent account using `npx wrangler deploy --temporary`, with deployments lasting 60 minutes. The feature is marketed for AI agents but benefits all developers. This feature significantly lowers the barrier to trying Cloudflare Workers, enabling rapid prototyping and testing without account overhead. It is especially useful for CI/CD pipelines, AI agents, and ephemeral demo environments. The temporary deployment can be claimed and converted into a permanent account within 60 minutes. The claim page shows a countdown timer and a randomly generated project name (e.g., "Educated Celery").

rss · Simon Willison · Jun 21, 22:01

**Background**: Cloudflare Workers is a serverless platform that runs JavaScript at the edge. Traditionally, deploying a Worker requires creating an account and configuring a project. Ephemeral deployments allow users to spin up short-lived environments without commitment, which is common in modern developer workflows.

<details><summary>References</summary>
<ul>
<li><a href="https://developers.cloudflare.com/workers/wrangler/">Wrangler · Cloudflare Workers docs</a></li>
<li><a href="https://github.com/cloudflare/workers-sdk">GitHub - cloudflare/workers-sdk: ⛅️ Home to Wrangler, the CLI for Cloudflare Workers®</a></li>
<li><a href="https://northflank.com/blog/what-are-ephemeral-environments">What are ephemeral environments? How they work and when to use them</a></li>

</ul>
</details>

**Tags**: `#Cloudflare`, `#serverless`, `#AI agents`, `#developer tools`, `#deployment`

---

<a id="item-9"></a>
## [Matrix Recurrent Units Update: Stability and Performance Analysis](https://www.reddit.com/r/MachineLearning/comments/1ubz5o8/an_update_on_matrix_recurrent_units_an_attention/) ⭐️ 7.0/10

The author revisits Matrix Recurrent Units (MRU), a linear-time sequence architecture alternative to attention, and addresses training instability issues by experimenting with various methods to construct input state matrices, including skew-symmetric, LDU, and QR decompositions. This work explores practical stability improvements for linear-time sequence models, which are crucial for scaling to long sequences while maintaining efficiency. The findings highlight trade-offs between stability and expressiveness, informing future architecture design. The author tested methods like forcing orthogonal matrices via Cayley map or matrix exponential, and found that orthogonal constraints hurt performance, suggesting that shear transformations are important. The LDU method performed best, but on the TinyStories dataset, MRU still underperformed a GPT-2 baseline.

reddit · r/MachineLearning · /u/mikayahlevi · Jun 21, 19:39

**Background**: Matrix Recurrent Units (MRU) are a type of recurrent architecture that models sequences by accumulating matrix products across time steps, using a parallel scan for efficiency. This is reminiscent of linear attention and state space models like Mamba. The earlier version of MRU suffered from numerical instability during training on larger datasets, prompting the author to seek stable input state matrix constructions.

<details><summary>References</summary>
<ul>
<li><a href="https://d2l.ai/chapter_recurrent-modern/gru.html">10.2. Gated Recurrent Units (GRU) — Dive into Deep ... - D2L</a></li>
<li><a href="https://www.emergentmind.com/topics/parallel-scan-aggregation">Parallel Scan Aggregation - emergentmind.com</a></li>
<li><a href="https://en.wikipedia.org/wiki/State-space_representation">State-space representation - Wikipedia</a></li>

</ul>
</details>

**Discussion**: On Reddit, earlier comments had pointed out training instability issues, which the author now addresses. The current update presents experimental results but the community may still debate the practicality of MRU compared to transformer and other efficient architectures.

**Tags**: `#machine learning`, `#attention alternative`, `#recurrent units`, `#sequence modeling`, `#linear-time architecture`

---

<a id="item-10"></a>
## [Oak: Git Alternative Optimized for AI Agents with Virtual Mounts](https://oak.space/oak/oak) ⭐️ 6.0/10

Oak is a new version control system designed for AI agents, featuring virtual mounts that eliminate the need for full repository clones. It claims to be up to 95% faster than Git for snapshots and optimizes context for agents working on multiple tasks in parallel. If successful, Oak could significantly reduce token usage and latency for AI coding agents, which often struggle with Git's complexity and large clone sizes. However, it faces adoption challenges because most AI models are heavily trained on Git workflows, making a new VCS less familiar and compatible. Oak is still early in development with no Windows build and missing features like CI, issues, and comments. The developer claims the entire Oak project is bootstrapped on Oak itself with no Git backup for several months.

hackernews · zdgeier · Jun 22, 15:37 · [Discussion](https://news.ycombinator.com/item?id=48631726)

**Background**: Version control systems like Git track changes in code over time. AI agents, especially those coding autonomously, often use Git for version management, but full clones and context switching can be slow. Virtual mounts allow agents to access only the files they need without downloading the entire repository, potentially saving time and storage.

<details><summary>References</summary>
<ul>
<li><a href="https://oak.space/">Version control at the speed of agents · oak</a></li>
<li><a href="https://en.wikipedia.org/wiki/Version_control">Version control - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters expressed skepticism about Oak's advantages over Git, noting that AI models are already well-trained on Git and may not benefit from a new VCS. Some found the lazy mount concept interesting, comparing it to Google's internal systems, and suggested it could be built on top of Git. One commenter praised the developer's achievements.

**Tags**: `#version control`, `#AI agents`, `#git`, `#tool`, `#open source`

---

<a id="item-11"></a>
## [Seeking Literature on Syntax-Robust NLI for Diffusion LLMs](https://www.reddit.com/r/MachineLearning/comments/1ucy7p3/syntactically_robust_nli_for_semantics_of/) ⭐️ 6.0/10

A researcher asks for literature on syntax-robust Natural Language Inference (NLI) to evaluate the semantic correctness of syntactically noisier text generated by diffusion LLMs compared to autoregressive LLMs. This highlights a gap in evaluation methods for diffusion LLMs, which are emerging as an alternative to autoregressive models but often produce syntactically imperfect text. Addressing syntactic robustness in NLI could improve the reliability of semantic evaluation for these models. The post specifically notes that state-of-the-art diffusion LLMs (except LLaDA) struggle with syntactic correctness, complicating the use of standard NLI tools. The researcher seeks the state of the art in syntax-robust NLI.

reddit · r/MachineLearning · /u/RepresentativeBee600 · Jun 22, 21:51

**Background**: Natural Language Inference (NLI) is a task of determining whether a hypothesis entails, contradicts, or is neutral given a premise. It is often used to evaluate the factual correctness of LLM outputs by checking if generated sub-claims are entailed by a trusted source. Diffusion LLMs generate text by gradually denoising from random tokens, contrasting with autoregressive models that generate left-to-right. This can lead to syntactic anomalies that standard NLI models may not handle well.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/the-low-end-disruptor/what-is-diffusion-llm-and-why-it-matters-749033d1efb1">What is Diffusion LLM and why it matters | by Zheng "Bruce" Li | The Low End Disruptor | Medium</a></li>
<li><a href="https://www.scribd.com/document/477243682/2004-11999-pdf">Syntactic Augmentation for NLI Robustness | PDF | Syntax | Phrase - Scribd</a></li>
<li><a href="https://arxiv.org/html/2208.07316v5">MENLI: Robust Evaluation Metrics from Natural Language Inference</a></li>

</ul>
</details>

**Tags**: `#NLI`, `#syntactic robustness`, `#diffusion LLMs`, `#autoregressive LLMs`, `#semantic evaluation`

---

<a id="item-12"></a>
## [Improved DVD-JEPA Demo Adds Noise and Baseline](https://www.reddit.com/r/MachineLearning/comments/1ubtf09/a_slightly_improved_dvdjepa_demo_p/) ⭐️ 6.0/10

A user improved the DVD-JEPA demo by adding environment noise and a fair pixel-space baseline comparison, making JEPA's ability to disregard irrelevant details more apparent. This incremental improvement strengthens the demonstration of JEPA's core strength—ignoring unpredictable environment details—which is key for self-supervised learning. It provides a more convincing minimal example for researchers and practitioners. The improvements include environment noise added to the bouncing DVD logo simulation and a pixel-space baseline with roughly the same parameter count and compute budget. The author used AI to implement most changes but acknowledges this transparently.

reddit · r/MachineLearning · /u/Kirne · Jun 21, 15:49

**Background**: JEPA (Joint-Embedding Predictive Architecture) is a self-supervised learning approach that predicts target block representations from a context block in the same image, avoiding pixel-level prediction. DVD-JEPA is a minimal world model that learns the physics of a bouncing DVD logo in representation space, training quickly on a CPU. The original demo received comments suggesting improvements, which this fork addresses.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/mandarwagh9/dvd-jepa">GitHub - mandarwagh9/dvd-jepa: A tiny, fully-reproducible ...</a></li>
<li><a href="https://arxiv.org/abs/2301.08243">[2301.08243] Self - Supervised Learning from Images with...</a></li>

</ul>
</details>

**Tags**: `#JEPA`, `#self-supervised learning`, `#machine learning`, `#demo`

---

<a id="item-13"></a>
## [Best methods for fine-tuning Whisper on domain-specific Spanish](https://www.reddit.com/r/MachineLearning/comments/1ubvmdx/best_current_methods_for_finetuning_whisper_on/) ⭐️ 6.0/10

A Reddit user is asking for the most effective current methods to fine-tune OpenAI's Whisper model on domain-specific Spanish vocabulary, including technical terms. They mention known techniques like LoRA, QLoRA, and spectrum fine-tuning but seek newer or better approaches. Domain-specific fine-tuning of ASR models like Whisper is crucial for improving accuracy in specialized fields (e.g., medicine, law, engineering). This question reflects a common need among practitioners and can guide others working on similar tasks. The user is working with Spanish speech and needs the model to reliably detect specific words and technical terms. They also ask roughly how many hours of labeled audio are needed for convergence, which is a practical concern for resource planning.

reddit · r/MachineLearning · /u/gothenjoyer_ · Jun 21, 17:18

**Background**: Whisper is a general-purpose speech recognition model from OpenAI. Fine-tuning adapts it to specific domains or vocabularies. Parameter-efficient methods like LoRA (Low-Rank Adaptation) freeze most weights and train small rank matrices, while QLoRA adds 4-bit quantization for memory savings. Spectrum fine-tuning selectively trains high-SNR layers to reduce VRAM usage. The user's mention of 'spectrum' likely refers to this latter method.

<details><summary>References</summary>
<ul>
<li><a href="https://www.geeksforgeeks.org/deep-learning/fine-tuning-using-lora-and-qlora/">Fine-Tuning using LoRA and QLoRA - GeeksforGeeks</a></li>
<li><a href="https://markaicode.com/spectrum-fine-tuning-selective-layer-training/">Run Spectrum Fine - Tuning : Selective Layer Training for... | Markaicode</a></li>
<li><a href="https://github.com/artidoro/qlora">GitHub - artidoro/ qlora : QLoRA : Efficient Finetuning of Quantized LLMs</a></li>

</ul>
</details>

**Tags**: `#Whisper`, `#fine-tuning`, `#domain adaptation`, `#Spanish ASR`

---

<a id="item-14"></a>
## [WeightsLab: Open-source tool for data-centric debugging](https://www.reddit.com/r/MachineLearning/comments/1ubwcat/datacentric_debugging_for_teams_training_neural/) ⭐️ 6.0/10

WeightsLab, an open-source PyTorch-native tool for data-centric debugging, has been significantly revamped, allowing teams to pause training mid-run and inspect live loss signals to catch issues like mislabels and class imbalance. This tool addresses a common frustration in ML teams: hours spent debugging training only to find data problems. By enabling live inspection, it helps catch data issues early, saving time and improving model performance, particularly in computer vision. The tool supports computer vision data types including images, videos, and LiDAR point clouds, and is available open source on GitHub. It is built natively for PyTorch, making integration seamless for existing PyTorch workflows.

reddit · r/MachineLearning · /u/taranpula39 · Jun 21, 17:47

**Background**: Data-centric AI emphasizes improving dataset quality over optimizing model architectures. Loss signals, calculated by the loss function during training, measure prediction errors; monitoring them can reveal data anomalies such as mislabeled samples or class imbalances, which often degrade model performance.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Data-centric_AI">Data-centric AI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Neural_network">Neural network - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#data-centric AI`, `#debugging`, `#PyTorch`, `#computer vision`, `#open source`

---