---
layout: default
title: "Horizon Summary: 2026-06-19 (EN)"
date: 2026-06-19
lang: en
---

> From 42 items, 23 important content pieces were selected

---

1. [10,000 GitHub Repositories Found Distributing Trojan Malware](#item-1) ⭐️ 9.0/10
2. [Noam Shazeer Leaves Google for OpenAI](#item-2) ⭐️ 9.0/10
3. [cuTile Rust Enables Safe GPU Kernels Competitive with vLLM](#item-3) ⭐️ 9.0/10
4. [Ubiquiti Announces Enterprise NAS Built on ZFS](#item-4) ⭐️ 8.0/10
5. [Hospitals and Universities Repurpose Drugs at 90% Lower Cost](#item-5) ⭐️ 8.0/10
6. [W Social: Theater of European Digital Sovereignty?](#item-6) ⭐️ 8.0/10
7. [GLM-5.2: New Open-Weights LLM Leader with 753B Parameters](#item-7) ⭐️ 8.0/10
8. [Charity Majors: AI Makes Code Cheap and Disposable](#item-8) ⭐️ 8.0/10
9. [Conversation-Level Debugging Outperforms Benchmark Metrics for Voice AI](#item-9) ⭐️ 8.0/10
10. [Next-Latent Prediction Boosts Transformer Efficiency](#item-10) ⭐️ 8.0/10
11. [Contrastive Targeted SFT for Causal Dependency Mapping in LLMs](#item-11) ⭐️ 8.0/10
12. [Cornell's CS 6120 Advanced Compilers Now Self-Guided Online](#item-12) ⭐️ 7.0/10
13. [Privacy advocate's GDPR complaint leads to €1.8M fine for Elkjop](#item-13) ⭐️ 7.0/10
14. [Swiss parliament lifts ban on new nuclear power plants](#item-14) ⭐️ 7.0/10
15. [Beyond .gitignore: Git's Other Ignore Mechanisms](#item-15) ⭐️ 7.0/10
16. [Check if LLMs Recognize You via Online Presence](#item-16) ⭐️ 7.0/10
17. [Datasette Apps plugin enables sandboxed HTML/JS apps with SQL queries](#item-17) ⭐️ 7.0/10
18. [Can foundational AI research be done without HPC?](#item-18) ⭐️ 7.0/10
19. [Speculative Decoding Accelerates LLM Inference](#item-19) ⭐️ 7.0/10
20. [uv 0.11.22 released with new env vars and preview features](#item-20) ⭐️ 6.0/10
21. [Brent Simmons' Retirement Project Enhances NetNewsWire](#item-21) ⭐️ 6.0/10
22. [Is ACL Now Irrelevant for PhD Admissions?](#item-22) ⭐️ 6.0/10
23. [Reddit user questions theoretical foundations for probe strength analysis](#item-23) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [10,000 GitHub Repositories Found Distributing Trojan Malware](https://orchidfiles.com/github-repositories-distributing-malware/) ⭐️ 9.0/10

A security researcher discovered over 10,000 GitHub repositories that distribute trojan malware, posing a massive threat to the software supply chain. This discovery reveals a widespread attack vector where malicious repositories can compromise software supply chains, affecting developers who unknowingly incorporate infected code into their projects. The malicious repositories often mimic legitimate projects, appear in search results, and are frequently updated to evade detection. They target automated agents rather than human users.

hackernews · theorchid · Jun 18, 11:45 · [Discussion](https://news.ycombinator.com/item?id=48583928)

**Background**: Supply chain attacks involve compromising software at its source, such as injecting malware into open-source repositories. Past incidents like the Log4j vulnerability highlight the severe impact of such attacks. GitHub is a major platform for code sharing, making it a prime target for attackers.

<details><summary>References</summary>
<ul>
<li><a href="https://outshift.cisco.com/blog/insights/top-10-supply-chain-attacks">Outshift | Top 15 software supply chain attacks : Case studies</a></li>
<li><a href="https://www.tanium.com/blog/taming-supply-chain-risks-in-the-wake-of-the-log4j-vulnerability/">Taming Supply Chain Risks in the Wake of the... | Tanium</a></li>
<li><a href="https://www.exiger.com/perspectives/software-supply-chain-attack-on-axios-http/">Software Supply Chain Attack on Axios HTTP - Exiger</a></li>

</ul>
</details>

**Discussion**: Commenters note that attackers target automated agents and frequently update repositories to manipulate search rankings. Some users report impersonation of their own projects, and one shares a specific malicious repository sample.

**Tags**: `#security`, `#malware`, `#GitHub`, `#supply chain`, `#cybersecurity`

---

<a id="item-2"></a>
## [Noam Shazeer Leaves Google for OpenAI](https://twitter.com/NoamShazeer/status/2067400851438932297) ⭐️ 9.0/10

Noam Shazeer, co-author of the seminal 'Attention Is All You Need' paper and former Gemini co-lead at Google, has left the company to join OpenAI. This move underscores the intense competition for top AI talent, especially among researchers who pioneered foundational technologies like the Transformer architecture, and could further accelerate OpenAI's model development. Shazeer originally joined Google in 2000, left in 2021 to co-found Character.AI, and returned in 2024 via a licensing/talent deal that made him Gemini co-lead; now he leaves again for OpenAI.

hackernews · lukasgross · Jun 18, 00:26 · [Discussion](https://news.ycombinator.com/item?id=48578913)

**Background**: The Transformer architecture, introduced in the 2017 paper 'Attention Is All You Need' co-authored by Shazeer, revolutionized deep learning by replacing recurrent layers with self-attention. It became the foundation for modern large language models like OpenAI's GPT series and Google's Gemini. Shazeer was considered one of the key engineers who turned the theoretical mechanism into efficient code.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Transformer_(deep_learning)">Transformer (deep learning) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gemini_(language_model)">Gemini (language model) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters highlight Shazeer's legendary status within Google, noting his role in implementing the spellchecker interview answer and his key contributions to the transformer paper. Some express surprise at his quick departure after returning to Google in 2024, while others provide extensive career timeline context.

**Tags**: `#AI`, `#transformers`, `#OpenAI`, `#Google`, `#talent movement`

---

<a id="item-3"></a>
## [cuTile Rust Enables Safe GPU Kernels Competitive with vLLM](https://www.reddit.com/r/MachineLearning/comments/1u9j7md/fearless_concurrency_on_the_gpu_safe_gpu/) ⭐️ 9.0/10

cuTile Rust, a tile-based GPU programming DSL for Rust, was introduced with a paper detailing how Rust's ownership model ensures memory safety and data-race freedom for GPU kernels. The Grout inference engine built on cuTile Rust achieves 171 tok/s for Qwen3-4B on RTX 5090 and 82 tok/s for Qwen3-32B on B200, matching vLLM and SGLang performance. This work addresses the growing trust bottleneck in AI-generated GPU code by providing compiler-verified safety guarantees, which could accelerate safe GPU kernel development and reduce debugging effort. It also demonstrates that safety does not sacrifice performance, with safe GEMM within 0.3% of hand-tuned CUDA. cuTile Rust lowers to CUDA Tile IR, carrying Rust's ownership model across the host-device boundary. Grout is a batch-1 research case study limited to a few models and NVIDIA GPUs, and many of its kernels still use unsafe Rust, though they can be migrated to safe variants.

reddit · r/MachineLearning · /u/Exciting_Suspect9088 · Jun 18, 21:36

**Background**: Traditional GPU programming (e.g., CUDA C++) uses a thread-based SIMT model where memory safety errors like data races are common and hard to debug. Rust's ownership and borrowing system eliminates these issues at compile time for CPU code, but extending this to GPU kernels has been challenging. CUDA Tile IR, part of CUDA 13.1, shifts from thread-level to tile-based operations, providing a lower-level virtual ISA that enables safe, structured GPU programming.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/nvlabs/cutile-rs">GitHub - NVlabs/cutile-rs: cuTile Rust provides a safe, tile-based kernel programming DSL for the Rust programming language. It features a safe host-side API for passing tensors to asynchronously executed kernel functions. · GitHub</a></li>
<li><a href="https://modal.com/gpu-glossary/device-software/cuda-tile-programming-model">What is the CUDA Tile programming model? | GPU Glossary</a></li>

</ul>
</details>

**Tags**: `#Rust`, `#GPU programming`, `#memory safety`, `#concurrency`, `#AI inference`

---

<a id="item-4"></a>
## [Ubiquiti Announces Enterprise NAS Built on ZFS](https://blog.ui.com/article/introducing-enterprise-nas) ⭐️ 8.0/10

Ubiquiti has announced an Enterprise NAS appliance that uses the ZFS file system, targeting enterprise storage needs. This brings ZFS, a highly reliable and feature-rich file system, into Ubiquiti's ecosystem, potentially offering an alternative to proprietary NAS solutions without recurring subscription fees. The NAS features dual 25 Gigabit SFP28 ports and redundant power supplies, though community members question whether spinning hard drives can saturate those links.

hackernews · ksec · Jun 18, 14:24 · [Discussion](https://news.ycombinator.com/item?id=48585866)

**Background**: ZFS is a combined file system and logical volume manager known for its data integrity features, including checksumming, snapshots, and RAID-Z. It is widely used in enterprise storage systems. Ubiquiti's implementation likely uses OpenZFS, the open-source version.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ZFS">ZFS - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community comments are mixed: some praise ZFS and the lack of subscription costs, but many express concerns about Ubiquiti's software quality and past security incidents, advising against using this product in enterprise environments.

**Tags**: `#Ubiquiti`, `#NAS`, `#ZFS`, `#Storage`, `#Enterprise`

---

<a id="item-5"></a>
## [Hospitals and Universities Repurpose Drugs at 90% Lower Cost](https://www.kcl.ac.uk/news/hospitals-and-universities-repurposing-drugs-at-90-lower-cost) ⭐️ 8.0/10

Hospitals and universities have shown that repurposing existing approved drugs for new medical uses can cut costs by up to 90%, directly challenging traditional pharmaceutical pricing and development models. This approach could dramatically lower healthcare expenses, particularly for rare diseases and conditions like macular degeneration, making essential treatments more affordable and accessible to patients. For example, using bevacizumab (Avastin) for macular degeneration costs about $50 per dose compared to $1,500 for the similar drug ranibizumab (Lucentis). However, regulatory pathways for formal repurposing without manufacturer consent remain limited, as noted in community discussions.

hackernews · giuliomagnifico · Jun 18, 10:33 · [Discussion](https://news.ycombinator.com/item?id=48583386)

**Background**: Drug repurposing, also known as drug repositioning, investigates existing drugs for new therapeutic purposes. It can reduce time and costs because safety data already exists, and supply chains are established. This strategy is especially valuable for neglected or rare diseases that lack commercial incentives for new drug development.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Drug_repurposing">Drug repurposing</a></li>
<li><a href="https://en.wikipedia.org/wiki/Drug_repositioning">Drug repositioning - Wikipedia</a></li>
<li><a href="https://www.nature.com/articles/nrd.2018.168">Drug repurposing: progress, challenges and recommendations | Nature Reviews Drug Discovery</a></li>

</ul>
</details>

**Discussion**: Commenters shared personal experiences, such as using Avastin for macular degeneration at a fraction of the cost of Lucentis, and highlighted organizations like Cures Within Reach that fund repurposing studies. Others criticized misaligned incentives, noting that Spravato (esketamine) is a patented modification of cheaper, off-patent ketamine, and raised regulatory barriers that prevent broad adoption without manufacturer cooperation.

**Tags**: `#drug repurposing`, `#healthcare costs`, `#pharmaceuticals`, `#ophthalmology`, `#rare diseases`

---

<a id="item-6"></a>
## [W Social: Theater of European Digital Sovereignty?](https://blog.elenarossini.com/w-social-public-institutions-and-the-theater-of-european-digital-sovereignty/) ⭐️ 8.0/10

A blog post by Elena Rossini critically examines W Social, a European social network, accusing it of being a 'theater' of digital sovereignty with opaque practices, while contrasting it with Eurosky, a transparent AT Protocol-based alternative run by a non-profit foundation. This analysis matters because it questions the legitimacy and transparency of W Social, which has been promoted by high-profile EU politicians and the WEF, potentially misleading the public about what true European digital sovereignty entails. W Social is structured as an LLC with a profit motive, and its founder has a finance background, raising concerns about its independence. In contrast, Eurosky is built on the open AT Protocol and operates transparently, sharing its development roadmap publicly.

hackernews · nemoniac · Jun 18, 12:46 · [Discussion](https://news.ycombinator.com/item?id=48584497)

**Background**: European digital sovereignty refers to the continent's effort to reduce reliance on US Big Tech by fostering homegrown alternatives. The AT Protocol is an open, decentralized protocol for social networking, used by Bluesky and Eurosky, which allows user data portability and platform interoperability. W Social, launched in 2025, positions itself as a European alternative but has been criticized for lacking transparency and resembling Truth Social in its political alignment.

<details><summary>References</summary>
<ul>
<li><a href="https://wsocial.news/">W - The European social network for verified humans</a></li>
<li><a href="https://eurosky.tech/">Eurosky - Building a thriving open social web for Europe</a></li>
<li><a href="https://en.wikipedia.org/wiki/AT_Protocol">AT Protocol</a></li>
<li><a href="https://www.euronews.com/next/2026/04/16/eurosky-europe-aims-to-rival-big-tech-with-its-own-social-media-ecosystem">Eurosky : Europe aims to rival Big Tech with its own social... | Euronews</a></li>

</ul>
</details>

**Discussion**: Community comments are highly critical of W Social, with users calling it 'shady' and comparing it to Truth Social. Commenters note that Eurosky, a transparent AT Protocol platform, received no press attention despite being more legitimate. Some highlight W Social's profit-driven LLC structure and its founder's finance background as red flags.

**Tags**: `#European digital sovereignty`, `#social network`, `#politics`, `#AT Protocol`, `#W Social`

---

<a id="item-7"></a>
## [GLM-5.2: New Open-Weights LLM Leader with 753B Parameters](https://simonwillison.net/2026/Jun/17/glm-52/#atom-everything) ⭐️ 8.0/10

Chinese AI lab Z.ai released GLM-5.2, a 753B parameter mixture-of-experts LLM with 1 million token context window, under the MIT license on June 16, 2026. GLM-5.2 tops the Artificial Analysis Intelligence Index among open-weights models and ranks second on the Code Arena WebDev leaderboard, demonstrating that powerful open-source LLMs can compete with proprietary models. The model uses Mixture of Experts with 40 active parameters out of 753B total, and consumes about 43k output tokens per task, more than competitors like MiniMax-M3 and DeepSeek V4 Pro.

rss · Simon Willison · Jun 17, 23:58

**Background**: Mixture of Experts (MoE) is a neural network architecture that activates only a subset of expert subnetworks for each input, enabling larger model sizes without proportional computational cost. This allows models like GLM-5.2 to scale to 753B parameters while maintaining inference efficiency.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://medium.com/@meisshaily/the-ultimate-guide-to-mixture-of-experts-architecture-721be990b08b">The Ultimate Guide to Mixture of Experts Architecture | Medium</a></li>
<li><a href="https://www.emergentmind.com/topics/mixture-of-experts-architecture">Mixture of Experts Architecture</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#open-weights`, `#Mixture of Experts`, `#GLM`, `#AI`

---

<a id="item-8"></a>
## [Charity Majors: AI Makes Code Cheap and Disposable](https://simonwillison.net/2026/Jun/17/charity-majors/#atom-everything) ⭐️ 8.0/10

Charity Majors, a respected engineer, observed that as of 2025, AI has inverted the economics of code production, making code generation virtually free and instant, turning code from a treasured asset into a disposable commodity. This insight highlights a fundamental shift in software engineering: the cost of writing code has plummeted, but the need for engineering discipline has increased. It affects how teams approach development, maintenance, and quality assurance. The quote originates from Charity Majors' article 'AI demands more engineering discipline. Not less.' She notes that lines of code went from being 'treasured, reused, cared for' to 'disposable and regenerable practically overnight.'

rss · Simon Willison · Jun 17, 17:12

**Background**: Historically, writing code required significant human effort and time, making each line valuable. With the advent of generative AI models, such as LLMs, producing code has become easier and faster, reducing its marginal cost. This shift challenges traditional software engineering practices that emphasized code reuse and careful curation.

**Tags**: `#ai-assisted-programming`, `#generative-ai`, `#software-engineering`, `#economics-of-code`

---

<a id="item-9"></a>
## [Conversation-Level Debugging Outperforms Benchmark Metrics for Voice AI](https://www.reddit.com/r/MachineLearning/comments/1u99fe5/voice_debugging_at_the_conversation_level_seems/) ⭐️ 8.0/10

A Reddit user argues that isolated benchmark metrics, such as STT scores and task completion rates, are insufficient for evaluating multi-turn voice systems, and advocates for conversation-level debugging that identifies recurring conversational patterns. This critique highlights a fundamental gap in current evaluation practices for conversational AI, as real-world interactions often suffer from emergent issues like awkward turn-taking and accumulating small errors that benchmarks miss. Better debugging approaches could significantly improve user experience in production voice agents. The user mentions that failed conversations often result from emergent properties of the interaction rather than single model errors, such as small timing mistakes and repeated confirmations. They have been experimenting with automated conversation-level QA to scale manual review of long conversational traces.

reddit · r/MachineLearning · /u/OwlZealousideal4779 · Jun 18, 15:29

**Background**: Traditional evaluation of voice agents relies on isolated metrics like speech-to-text accuracy, latency, and task completion. However, these metrics fail to capture the fluidity of multi-turn conversations where small issues compound. Recent platforms like Braintrust and Cekura offer tools for conversation-level debugging, tracing, and automated QA. The field is moving toward more holistic evaluation that considers the entire interaction.

<details><summary>References</summary>
<ul>
<li><a href="https://www.braintrust.dev/articles/how-to-evaluate-voice-agents">How to evaluate voice agents - Articles - Braintrust</a></li>
<li><a href="https://www.destined.ai/conversational-ai-qa-testing">Conversational AI QA Testing: A Practical Framework for Voice Agents</a></li>

</ul>
</details>

**Tags**: `#conversational AI`, `#evaluation metrics`, `#voice debugging`, `#multi-turn systems`, `#QA`

---

<a id="item-10"></a>
## [Next-Latent Prediction Boosts Transformer Efficiency](https://www.reddit.com/r/MachineLearning/comments/1u84mio/nextlatent_prediction_transformers_r/) ⭐️ 8.0/10

Microsoft Research introduces Next-Latent Prediction (NextLat), a self-supervised method that trains transformers to predict their own next latent state, achieving up to 3.3x faster inference via self-speculative decoding and forming compact world models. This approach extends next-token prediction to latent space, offering better data efficiency and representation learning, with potential to significantly impact transformer architectures and inference speed across various AI applications. NextLat trains the transformer to predict its next latent state given the current latent state and next token, providing denser supervision than one-hot token prediction. The self-speculative decoding uses recursive multi-step lookahead for faster inference.

reddit · r/MachineLearning · /u/jayden_teoh_ · Jun 17, 08:44

**Background**: Standard transformers typically train with next-token prediction, which predicts the next token in a sequence given previous tokens. NextLat adds a self-supervised objective that predicts the model's own internal latent representations. Compact world models compress sensory inputs into latent states for planning and reasoning. Self-speculative decoding accelerates inference by having the model generate and verify draft tokens using its own layers.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2511.05963">[2511.05963] Next-Latent Prediction Transformers Learn Compact World Models</a></li>
<li><a href="https://en.wikipedia.org/wiki/World_model_(artificial_intelligence)">World model (artificial intelligence) - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/layerskip">Faster Text Generation with Self-Speculative Decoding</a></li>

</ul>
</details>

**Tags**: `#transformers`, `#self-supervised learning`, `#latent prediction`, `#inference acceleration`, `#representation learning`

---

<a id="item-11"></a>
## [Contrastive Targeted SFT for Causal Dependency Mapping in LLMs](https://www.reddit.com/r/MachineLearning/comments/1u8if6l/contrastive_targeted_sft_as_a_mechinterp_method/) ⭐️ 8.0/10

A Reddit user proposes using contrastive targeted supervised fine-tuning (SFT) combined with ablation to map causal dependencies between capabilities in large language models by identifying and ablating the circuits responsible for specific dimensions. This approach could enable optimal training order by determining which capabilities depend on others, leading to more efficient fine-tuning and better behavior control. It also offers a novel closed-loop method where mechanistic interpretability findings directly guide subsequent training strategies. The user trained a 31B model on 40 domains scoring six quality dimensions, then trained contrastive variants to isolate circuits for the weakest dimension. Plan involves ablating those circuits and measuring degradation in other dimensions to build a causal dependency graph.

reddit · r/MachineLearning · /u/Substantial_Diver469 · Jun 17, 18:31

**Background**: Mechanistic interpretability aims to reverse-engineer the internal computations of neural networks. Ablation studies remove specific components to assess their contribution. Supervised fine-tuning (SFT) adapts a pretrained model using labeled data. Contrastive training involves learning from pairs of examples to highlight differences.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Ablation_(artificial_intelligence)">Ablation (artificial intelligence) - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/1901.08644">[1901.08644] Ablation Studies in Artificial Neural Networks</a></li>

</ul>
</details>

**Tags**: `#mechanistic interpretability`, `#SFT`, `#causal dependency`, `#LLM`, `#circuit discovery`

---

<a id="item-12"></a>
## [Cornell's CS 6120 Advanced Compilers Now Self-Guided Online](https://www.cs.cornell.edu/courses/cs6120/2025fa/self-guided/) ⭐️ 7.0/10

Cornell's CS 6120 advanced compilers course is now available as a self-guided online resource, including video lectures, readings, and assignments for independent study. This makes a high-quality advanced compilers course freely accessible to a global audience, benefiting students, researchers, and practitioners who lack access to formal instruction. The course covers advanced topics such as static single assignment form, data flow analysis, and dynamic compilation, though some community members noted a heavy focus on trace compilation.

hackernews · ibobev · Jun 18, 11:04 · [Discussion](https://news.ycombinator.com/item?id=48583606)

**Background**: Advanced compilers courses typically assume familiarity with basic compiler construction. CS 6120 focuses on optimization and code generation techniques used in modern production compilers like LLVM.

**Discussion**: On Hacker News, users debated the course's depth, with some questioning the 'advanced' label for covering standard topics, while others appreciated the availability. Criticisms included an excessive focus on trace compilation, which some consider a dead end.

**Tags**: `#compilers`, `#education`, `#programming languages`, `#systems`

---

<a id="item-13"></a>
## [Privacy advocate's GDPR complaint leads to €1.8M fine for Elkjop](https://www.thatprivacyguy.com/blog/elkjop-forced-consent-fine/) ⭐️ 7.0/10

The Norwegian Data Protection Authority fined electronics retailer Elkjop €1.8 million for requiring customers to consent to marketing as a condition of membership, violating the GDPR's prohibition on forced consent. This case demonstrates that individual persistence can effectively enforce GDPR, and it sends a strong signal that bundling consent with service contracts is illegal, empowering consumers and privacy advocates. The complaint was filed in 2018 by the privacy advocate known as 'thatprivacyguy', and the fine was finally imposed in 2023, with the official decision confirming violation of Article 7(4) GDPR.

hackernews · speckx · Jun 18, 18:31 · [Discussion](https://news.ycombinator.com/item?id=48589501)

**Background**: The GDPR requires that consent for data processing must be freely given, specific, informed, and unambiguous. Article 7(4) specifically prohibits making consent a condition of service unless the data processing is necessary for that service. 'Forced consent' refers to practices where companies require users to agree to unnecessary data processing to access a service, which undermines the voluntary nature of consent.

<details><summary>References</summary>
<ul>
<li><a href="https://yorba.co/yorblog/forced-consent">Forced Consent: How Tech Companies Manipulate Users Into Giving Away Their Data</a></li>
<li><a href="https://www.telecoms.com/digital-ecosystem/facebook-and-google-accused-of-gdpr-forced-consent-">Facebook and Google accused of GDPR 'forced consent' - Telecoms</a></li>

</ul>
</details>

**Discussion**: The community praised the advocate's persistence and viewed the fine as a victory for privacy rights. One user provided links to the official decision in Norwegian and an English translation, enhancing the discussion's credibility. Another comment humorously noted that the advocate had to sue the same entity that later ruled in his favor.

**Tags**: `#GDPR`, `#privacy`, `#data protection`, `#consumer rights`, `#fine`

---

<a id="item-14"></a>
## [Swiss parliament lifts ban on new nuclear power plants](https://www.bluewin.ch/en/news/switzerland/parliament-lifts-ban-on-new-nuclear-power-plants-3257535.html) ⭐️ 7.0/10

The Swiss parliament voted to lift a ban on building new nuclear power plants, reversing a 2017 law that prohibited new construction. This decision still requires approval in a national referendum. This move could reshape Switzerland's energy policy, potentially extending reliance on nuclear power amid concerns over energy security and climate goals. It also reignites debate on nuclear safety, waste management, and the role of renewables. The ban was part of the 2017 Energy Act that mandated the phase-out of nuclear power. The current parliament's decision lifts the ban but does not guarantee new plants will be built; a referendum is expected due to strong opposition from left-leaning and green parties.

hackernews · leonidasrup · Jun 18, 14:17 · [Discussion](https://news.ycombinator.com/item?id=48585746)

**Background**: In May 2017, Swiss voters approved the Energy Strategy 2050, which banned new nuclear plants and promoted renewables. Switzerland's five existing reactors provide about one-third of its electricity but are aging. Advanced reactor designs, such as small modular reactors (SMRs) and Generation IV concepts, are being explored globally but are not yet commercial.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Nuclear_power_in_Switzerland">Nuclear power in Switzerland - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Anti-nuclear_movement_in_Switzerland">Anti-nuclear movement in Switzerland - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Comments show mixed opinions: some emphasize nuclear's low death rate per TWh and energy security benefits, while others question the cost and timing compared to renewables. A user argues that the debate overlooks the environmental impact of uranium mining, and another notes that a referendum is likely, with chaotic political discourse expected.

**Tags**: `#nuclear energy`, `#energy policy`, `#Switzerland`, `#technology policy`

---

<a id="item-15"></a>
## [Beyond .gitignore: Git's Other Ignore Mechanisms](https://nelson.cloud/.gitignore-isnt-the-only-way-to-ignore-files-in-git/) ⭐️ 7.0/10

An article and community discussion highlight lesser-known Git ignore mechanisms, including .git/info/exclude, global exclude files, and .gitattributes for ignoring diffs. Understanding these mechanisms helps developers keep repositories clean without polluting project .gitignore files with personal IDE or OS artifacts, improving collaboration and avoiding accidental commits. The .git/info/exclude file is local to each repository and not committed, while a global exclude file can be configured via core.excludesFile, commonly located at ~/.config/git/ignore. Additionally, .gitattributes can instruct Git to ignore diffs for specific file types.

hackernews · FergusArgyll · Jun 18, 10:29 · [Discussion](https://news.ycombinator.com/item?id=48583356)

**Background**: Git uses .gitignore files to specify intentionally untracked files that should be ignored globally across a repository. However, sometimes you need to ignore files only locally without affecting other clones, or ignore files universally across all repositories. Git provides several mechanisms for these scenarios.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.github.com/en/get-started/git-basics/ignoring-files">You can configure Git to ignore files you don't want to check in to...</a></li>
<li><a href="https://stackoverflow.com/questions/1753070/how-do-i-configure-git-to-ignore-some-files-locally">How do I configure git to ignore some files locally? - Stack Overflow</a></li>

</ul>
</details>

**Discussion**: The community praised the article for its practical tips, with users emphasizing global excludes for personal files and .gitattributes for ignoring diffs in auto-generated files like package-lock.json. Some discussed the proper location for global Git config (~/.config/git/ignore) and creative tricks like adding an 'attic' directory to global ignore.

**Tags**: `#git`, `#.gitignore`, `#version control`, `#developer tools`

---

<a id="item-16"></a>
## [Check if LLMs Recognize You via Online Presence](https://www.intheweights.com/) ⭐️ 7.0/10

A new web tool called 'Are You in the Weights?' queries multiple large language models in parallel to assess how strongly they recognize a person based on their digital footprint, clustering responses to produce a recognition score. This project highlights the growing concern about privacy and identity as more human-generated content is absorbed into AI training data, and it provides a tangible way for individuals to understand what LLMs 'know' about them. The tool queries frontier and small models, clusters similar responses, and identifies hallucinations when a model gives incorrect information. It is non-deterministic, meaning repeated queries may yield different scores.

hackernews · turtlesoup · Jun 18, 20:49 · [Discussion](https://news.ycombinator.com/item?id=48591348)

**Background**: In neural networks, weights are numerical parameters that determine the strength of connections between artificial neurons. During training, weights are adjusted to encode the model's knowledge. This tool essentially probes the 'knowledge' embedded in LLM weights by checking how consistently a model can identify a person given their name or keywords.

<details><summary>References</summary>
<ul>
<li><a href="https://tedai-sanfrancisco.ted.com/glossary/weights/">What are Weights in AI? | TEDAI San Francisco</a></li>
<li><a href="https://aclanthology.org/2025.findings-emnlp.1279.pdf">Unequal Scientific Recognition in the Age of LLMs</a></li>

</ul>
</details>

**Discussion**: Commenters shared mixed experiences: some were pleased to be recognized (e.g., top 6% of scores), while others found they were hallucinated as someone else, raising concerns about accuracy and privacy. One user refused to use their real name, and another noted that the score increases with more keywords added.

**Tags**: `#LLMs`, `#AI`, `#privacy`, `#identity`, `#web`

---

<a id="item-17"></a>
## [Datasette Apps plugin enables sandboxed HTML/JS apps with SQL queries](https://simonwillison.net/2026/Jun/18/datasette-apps/#atom-everything) ⭐️ 7.0/10

Datasette Apps is a new plugin that allows hosting sandboxed HTML+JavaScript applications within Datasette, capable of executing read-only and write SQL queries against the data via stored queries. This plugin extends Datasette's utility by enabling custom interactive web applications directly on top of published data, turning Datasette into a more powerful platform for data exploration and visualization. Apps run in a constrained <iframe> with sandbox attributes (allow-scripts, allow-forms) and an injected CSP header to prevent external HTTP requests or access to cookies and localStorage, ensuring security.

rss · Simon Willison · Jun 18, 23:58

**Background**: Datasette is an open-source tool for exploring and publishing data, especially SQLite databases, as interactive websites with a JSON API. It supports SQL queries and has a plugin system. Stored queries allow executing write queries with proper permissions.

<details><summary>References</summary>
<ul>
<li><a href="https://datasette.io/">Datasette: An open source multi-tool for exploring and publishing data</a></li>
<li><a href="https://datasette.io/blog/2026/sql-write-queries">SQL write queries and stored queries in Datasette 1.0a31 - Datasette Blog</a></li>

</ul>
</details>

**Tags**: `#Datasette`, `#plugin`, `#SQL`, `#web applications`, `#sandboxing`

---

<a id="item-18"></a>
## [Can foundational AI research be done without HPC?](https://www.reddit.com/r/MachineLearning/comments/1u8jyat/is_foundational_ai_research_still_something_that/) ⭐️ 7.0/10

A Reddit user questioned whether foundational AI research remains feasible without access to high-performance computing (HPC), highlighting that the original Transformer paper was trained on just a few high-end gaming GPUs. This question underscores growing concerns about the democratization of AI research, as HPC costs create barriers for many academic and independent researchers. The answer could shape who can contribute to future breakthroughs. The original Transformer (2017) used 8 NVIDIA P100 GPUs, but today's state-of-the-art models often require thousands of GPUs and expensive HPC infrastructure. Foundational research may still be possible with modest hardware if focused on algorithmic efficiency rather than scaling.

reddit · r/MachineLearning · /u/Proof-Bed-6928 · Jun 17, 19:26

**Background**: High-Performance Computing (HPC) refers to clusters of powerful machines, often with many GPUs, used for computationally intensive tasks like training large AI models. Foundational AI research involves developing new architectures or algorithms, which may require less compute than simply scaling existing models. The Transformer paper is often cited as an example of a breakthrough achieved with relatively modest resources.

<details><summary>References</summary>
<ul>
<li><a href="https://www.hivenet.com/post/hpc-performance-without-hpc-overhead">HPC solution for AI and research teams | Hivenet</a></li>

</ul>
</details>

**Tags**: `#AI research`, `#HPC`, `#machine learning`, `#accessibility`, `#transformers`

---

<a id="item-19"></a>
## [Speculative Decoding Accelerates LLM Inference](https://www.reddit.com/r/MachineLearning/comments/1u83kzt/what_is_speculative_decoding_trending_on/) ⭐️ 7.0/10

Speculative decoding is trending on Papers with Code, and SGLang released a blog post detailing next-generation speculative decoding using DFlash models, achieving state-of-the-art latencies for LLM inference serving. This technique significantly speeds up LLM inference without sacrificing output quality, enabling faster and more cost-effective deployment of large language models in production. It is particularly important for practitioners optimizing inference serving systems. Speculative decoding uses a fast draft model to propose multiple tokens in parallel, which are then verified by a single forward pass of the target model. DFlash, a block diffusion-based draft model, achieves over 6x lossless acceleration across various models and tasks.

reddit · r/MachineLearning · /u/NielsRogge · Jun 17, 07:41

**Background**: Large language models generate text autoregressively, one token at a time, which makes inference slow and computationally expensive. Speculative decoding accelerates this by employing a smaller, faster draft model to generate candidate tokens that the larger model checks in parallel. SGLang and vLLM are two popular inference engines for LLMs; SGLang recently integrated DFlash to improve speculative decoding performance.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2602.06036">[2602.06036] DFlash: Block Diffusion for Flash Speculative Decoding - arXiv</a></li>
<li><a href="https://www.lmsys.org/blog/2026-06-15-next-generation-speculative-decoding-dflash-v2/">The next generation of speculative decoding: DFlash and Spec V2 - LMSYS Blog</a></li>
<li><a href="https://kanerika.com/blogs/sglang-vs-vllm/">SGLang vs vLLM in 2026: Which Inference Engine Wins?</a></li>

</ul>
</details>

**Tags**: `#speculative decoding`, `#LLM inference`, `#optimization`, `#SGLang`, `#machine learning`

---

<a id="item-20"></a>
## [uv 0.11.22 released with new env vars and preview features](https://github.com/astral-sh/uv/releases/tag/0.11.22) ⭐️ 6.0/10

The astral-sh/uv team released version 0.11.22 on June 18, 2026, introducing new environment variables for specifying paths to binaries used by uv format and uv check, and adding preview features such as configuring preview options in config files, SARIF support for uv audit, and a --script flag for uv check and uv metadata. This release improves developer workflow by allowing fine-grained control over external tools via environment variables and expanding uv audit capabilities with industry-standard SARIF output. These enhancements make uv more versatile for Python project management and CI/CD pipelines. The new TY and RUFF environment variables point to the tyr and ruff binaries used by uv format and uv check. Preview features include lockfile updates during uv check --no-sync, and SARIF output support for uv audit, which is the Static Analysis Results Interchange Format. The release also includes performance improvements via a deadlock-resistant concurrent hashmap in the resolver.

github · github-actions[bot] · Jun 18, 23:05

**Background**: uv is a fast Python package manager written in Rust, developed by Astral (the creators of Ruff). It aims to replace tools like pip, pip-tools, and poetry with a single, high-performance binary. The project has rapidly gained popularity for its speed and simplicity in managing Python dependencies and virtual environments.

<details><summary>References</summary>
<ul>
<li><a href="https://sarifweb.azurewebsites.net/">SARIF Home</a></li>
<li><a href="https://docs.astral.sh/uv/concepts/projects/workspaces/">Using workspaces | uv</a></li>
<li><a href="https://github.com/astral-sh/uv/issues/18506">Roadmap: `uv audit` · Issue #18506 · astral-sh/uv - GitHub</a></li>

</ul>
</details>

**Tags**: `#python`, `#package manager`, `#uv`, `#release`

---

<a id="item-21"></a>
## [Brent Simmons' Retirement Project Enhances NetNewsWire](https://simonwillison.net/2026/Jun/17/netnewswire-status/#atom-everything) ⭐️ 6.0/10

Brent Simmons, the original developer, has been dedicating his retirement to improving NetNewsWire, an open-source RSS reader, making it exceptionally good without commercial pressures. This showcases how passion projects can produce high-quality software when freed from commercial constraints, benefiting the RSS community and open-source ecosystem. NetNewsWire was first released in 2002 and was made open source in 2018; it is available on Mac and iPhone and has been described as 'like podcasts, but for reading'.

rss · Simon Willison · Jun 17, 03:36

**Background**: RSS (Really Simple Syndication) is a web feed format that allows users to access updates to online content in a standardized way. NetNewsWire is a popular RSS reader that has been maintained by Brent Simmons for years. Open-source software is code that is publicly accessible and can be modified and distributed by anyone.

**Tags**: `#netnewswire`, `#brent-simmons`, `#open-source`, `#rss`, `#software-development`

---

<a id="item-22"></a>
## [Is ACL Now Irrelevant for PhD Admissions?](https://www.reddit.com/r/MachineLearning/comments/1u945j5/is_acl_now_irrelevant_d/) ⭐️ 6.0/10

A Reddit user noticed a comment suggesting that an ACL first-author paper is a weak signal for PhD applications, sparking debate about the conference's perceived value. This debate reflects growing skepticism about the weight of NLP-specific venues like ACL compared to broader ML conferences, potentially influencing PhD application strategies and conference submission trends. The original comment claimed that an ACL first-author paper is not a great plus for PhD chances, noting that ACL is considered less prestigious than NIPS, ICML, ICLR, or CVPR, though it is still an A+ venue in NLP.

reddit · r/MachineLearning · /u/H4RZ3RK4S3 · Jun 18, 11:52

**Background**: Academic conferences in computer science are often ranked by prestige, with top venues like NIPS and ICML having high impact. ACL is the leading venue for natural language processing, but some argue that broader machine learning conferences carry more weight in AI research. The user also mentions a perception that classical CS areas like software engineering (ICSE, FSE) may undervalue AI conferences.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/List_of_computer_science_conferences">List of computer science conferences - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/International_Conference_on_Software_Engineering">International Conference on Software Engineering - Wikipedia</a></li>
<li><a href="https://www.esec-fse.org/">Home | FSE</a></li>

</ul>
</details>

**Tags**: `#NLP`, `#ACL`, `#academic conferences`, `#PhD admissions`

---

<a id="item-23"></a>
## [Reddit user questions theoretical foundations for probe strength analysis](https://www.reddit.com/r/MachineLearning/comments/1u8lo60/how_do_you_analyze_the_relative_strength_of/) ⭐️ 6.0/10

A Reddit user posted a technical question about analyzing the relative strength of probes in transformer models, linking it to circuit analysis and factuality guarantees. They highlight issues with a logistic regression probe from an earlier post and cite a failure of Google Gemini in counting letters in 'Google'. Probe analysis is central to mechanistic interpretability and factuality guarantees in language models. This question reveals gaps in current methodology, particularly regarding theoretical guarantees and the balance between probe and network capacity. The user notes that the small vocabulary makes simple probes look better than they are, and that a classifier gained performance for rare tokens by learning an 'extreme token' heuristic. They also observe that Google Gemini miscounts letters in 'Google', suggesting the model may not learn exact token decomposition.

reddit · r/MachineLearning · /u/RepresentativeBee600 · Jun 17, 20:29

**Background**: Probing in machine learning involves training a simple classifier (a probe) on a model's internal representations to infer what information is encoded. Circuit analysis studies specific computational subgraphs within neural networks. The Nyquist–Shannon sampling theorem provides guarantees about reconstructing signals from samples; the user asks if analogous guarantees exist for probing. Mechanistic interpretability aims to reverse-engineer neural networks to understand how they compute.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reddit.com/r/MachineLearning/comments/1u8lo60/how_do_you_analyze_the_relative_strength_of/">How do you analyze the relative "strength" of probes? [R] : r/MachineLearning - Reddit</a></li>
<li><a href="https://en.wikipedia.org/wiki/Neural_network_(machine_learning)">Neural network (machine learning) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#mechanistic interpretability`, `#probing`, `#transformer models`

---