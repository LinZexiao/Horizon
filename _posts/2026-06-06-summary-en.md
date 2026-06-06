---
layout: default
title: "Horizon Summary: 2026-06-06 (EN)"
date: 2026-06-06
lang: en
---

> From 38 items, 19 important content pieces were selected

---

1. [KVarN: Variance-Normalized KV-Cache Quantization for LLM Inference](#item-1) ⭐️ 9.0/10
2. [Microsoft open-sources pg_durable for PostgreSQL durable execution](#item-2) ⭐️ 8.0/10
3. [Hacker News shares 'oh shit' GenAI moments](#item-3) ⭐️ 8.0/10
4. [Google Releases Gemma 4 QAT Models for On-Device AI](#item-4) ⭐️ 8.0/10
5. [Blog post questions if Claude AI increased bugs in rsync](#item-5) ⭐️ 8.0/10
6. [MicroPython compiled to WebAssembly enables safe Python sandbox](#item-6) ⭐️ 8.0/10
7. [Ladybird Browser Bans Public Pull Requests Over AI Code Concerns](#item-7) ⭐️ 8.0/10
8. [AI Enthusiasts vs. Skeptics: Race Against Time or Entropy?](#item-8) ⭐️ 8.0/10
9. [TinyTPU: Real SystemVerilog TPU runs in browser via WASM](#item-9) ⭐️ 8.0/10
10. [Intricacies of Modern Camera Lens Repair](#item-10) ⭐️ 7.0/10
11. [UK Gov Drops Stripe for Dutch Payment Provider Adyen](#item-11) ⭐️ 7.0/10
12. [OpenAI Launches Lockdown Mode to Prevent Prompt Injection Attacks](#item-12) ⭐️ 7.0/10
13. [Google Employees Mock Their Own AI; Spokesperson Backtracks on Human Oversight](#item-13) ⭐️ 7.0/10
14. [On-Policy Distillation: A Hot New Post-Training Technique](#item-14) ⭐️ 7.0/10
15. [Is Capture-Time Semantic Annotation for Robot Trajectories Solved?](#item-15) ⭐️ 7.0/10
16. [ISS Astronauts Shelter During Air Leak Repair Attempt](#item-16) ⭐️ 6.0/10
17. [Solar desalination method claims zero waste, faces skepticism](#item-17) ⭐️ 6.0/10
18. [AI Agent Skill for Test-Driven Development](#item-18) ⭐️ 6.0/10
19. [GitHub repo collects Transformer attention implementations](#item-19) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [KVarN: Variance-Normalized KV-Cache Quantization for LLM Inference](https://www.reddit.com/r/MachineLearning/comments/1twnj5r/kvarn_variancenormalized_kvcache_quantization_r/) ⭐️ 9.0/10

Researchers introduced KVarN, a novel method that combines Hadamard rotations with variance-normalization to quantize KV-cache, achieving 3-4x compression with minimal accuracy loss (0-1%) and practical speedup over fp16 in vLLM. The method is particularly effective for decode-heavy settings like reasoning and code generation. KV-cache is a major memory bottleneck in LLM inference, especially for long contexts and large batches. KVarN's high compression ratio with near-zero accuracy loss enables more efficient deployment of LLMs, reducing hardware costs and enabling faster inference in production systems. KVarN applies variance-normalization on both axes of the K and V matrices after Hadamard rotation, then rounds to nearest for quantization. The method provides a theoretical analysis showing that fixing large errors is disproportionately beneficial, and these errors mainly stem from poor token-scales.

reddit · r/MachineLearning · /u/intentionallyBlue · Jun 4, 13:21

**Background**: KV-cache stores intermediate key-value pairs during transformer autoregressive decoding to avoid redundant computation, but it grows with sequence length and batch size, often becoming the largest memory consumer. Quantization reduces memory footprint by representing values with lower precision (e.g., 8-bit integers) but can introduce accuracy loss. vLLM is a popular open-source framework for efficient LLM serving. Hadamard rotation is an orthogonal transformation that helps decorrelate data for more effective quantization.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hadamard_transform">Hadamard transform - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/VLLM">VLLM</a></li>
<li><a href="https://grokipedia.com/page/KV_cache">KV cache</a></li>

</ul>
</details>

**Tags**: `#KV-cache`, `#quantization`, `#LLM inference`, `#machine learning`, `#optimization`

---

<a id="item-2"></a>
## [Microsoft open-sources pg_durable for PostgreSQL durable execution](https://github.com/microsoft/pg_durable) ⭐️ 8.0/10

Microsoft has open-sourced pg_durable, a PostgreSQL extension that enables in-database durable execution for workflows. It allows developers to define workflows as SQL steps with automatic checkpointing and recovery from crashes or failures. This release brings durable execution capabilities directly into PostgreSQL, reducing reliance on external workflow engines like Temporal. It simplifies building reliable, fault-tolerant workflows for tasks such as ETL pipelines and batch processing within the database. pg_durable is suited for workflows that are mostly SQL operations with some external API calls, such as vector embedding pipelines and batch ETL with deduplication. It uses a SQL DSL and checkpoints execution progress, resuming from the last checkpoint after failures.

hackernews · coffeemug · Jun 5, 15:59 · [Discussion](https://news.ycombinator.com/item?id=48414367)

**Background**: Durable execution is a technique where a workflow saves its progress at key checkpoints, allowing it to pause and later resume exactly where it left off, even after crashes. This is commonly implemented by external platforms like Temporal or AWS Step Functions. By integrating durable execution into PostgreSQL, pg_durable allows workflows to be managed closer to the data, reducing complexity and latency for database-centric applications.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/microsoft/pg_durable">GitHub - microsoft/pg_durable: PostgreSQL in-database durable execution</a></li>
<li><a href="https://dev.to/franckpachot/getting-started-with-pgdurable-durable-workflows-inside-postgresql-3980">Getting Started with pg_durable: Durable Workflows Inside PostgreSQL</a></li>
<li><a href="https://byteiota.com/pg_durable-microsoft-open-sources-durable-execution-for-postgresql/">pg_durable: Microsoft Open-Sources Durable Execution for PostgreSQL</a></li>

</ul>
</details>

**Discussion**: Community comments reveal mixed opinions. Some developers celebrate the option of having workflow logic in the database, while others express concerns about stored procedure-like limitations, such as difficulty with unit testing and versioning. There is also debate about how pg_durable compares to external orchestration tools like Temporal, with the documentation advising against it for workflows that span many heterogeneous systems.

**Tags**: `#durable execution`, `#PostgreSQL`, `#open source`, `#database workflows`

---

<a id="item-3"></a>
## [Hacker News shares 'oh shit' GenAI moments](https://news.ycombinator.com/item?id=48406174) ⭐️ 8.0/10

An Ask HN thread invites users to describe the specific moment they realized generative AI was more powerful than they initially thought, sparking over 570 comments sharing personal anecdotes. This thread captures a pivotal shift in perception among technologists, highlighting real-world moments where GenAI's capabilities became undeniable, which may influence how others adopt and trust these tools. Examples include using Gemini to diagnose a furnace issue from videos, reverse-engineering a ghosted employee's knowledge via Google Workspace RAG, and interacting with an LLM as a dynamic text adventure that went beyond predefined scripts.

hackernews · andrehacker · Jun 4, 23:42

**Background**: Generative AI models like GPT-4 and Gemini can understand and generate human-like text, images, and more. Many early users dismissed them as novelties, but as models improved and were applied to practical tasks, the technology's transformative potential became apparent.

**Discussion**: Commenters express a mix of awe and realization, sharing practical breakthroughs (e.g., fixing a furnace) and creative surprises (e.g., emergent storytelling). The sentiment is largely positive, reflecting a collective shift from skepticism to recognition of GenAI's utility.

**Tags**: `#generative AI`, `#LLM`, `#personal experience`, `#community discussion`, `#AI impact`

---

<a id="item-4"></a>
## [Google Releases Gemma 4 QAT Models for On-Device AI](https://blog.google/innovation-and-ai/technology/developers-tools/quantization-aware-training-gemma-4/) ⭐️ 8.0/10

Google has released Gemma 4 models with Quantization-Aware Training (QAT), specifically optimized for efficient inference on mobile devices and laptops. The models are available on Hugging Face and can be run locally using tools like LiteRT LM. This release significantly reduces the memory and computational requirements for running large language models on edge devices, enabling powerful AI capabilities without constant cloud connectivity. It advances on-device AI efficiency and could lower the carbon footprint of AI inference. The QAT process integrates quantization during training rather than after, often yielding higher accuracy than post-training quantization. Community comparisons show that Unsloth's quants can achieve near-100% accuracy relative to the unquantized BF16 model, surpassing Google's official QAT versions.

hackernews · theanonymousone · Jun 5, 16:18 · [Discussion](https://news.ycombinator.com/item?id=48414653)

**Background**: Quantization reduces the precision of model weights (e.g., from 32-bit float to 8-bit integer), shrinking model size and speeding up inference. Quantization-Aware Training (QAT) simulates quantization during training so the model learns to compensate for precision loss. Gemma 4 is a family of open, lightweight models from Google DeepMind built on the same research as Gemini, designed for efficient deployment on various hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://deepmind.google/models/gemma/gemma-4/">Gemma 4 is a family of open models , purpose-built for advanced...</a></li>
<li><a href="https://www.tensorflow.org/model_optimization/guide/quantization/training">Quantization aware training | TensorFlow Model Optimization</a></li>
<li><a href="https://eliteaiadvantage.com/blog/google-litert-on-device-ai-models">How to Use Google LiteRT for On - Device AI Models</a></li>

</ul>
</details>

**Discussion**: Community members actively tested the models, with simonw sharing a one-command local setup using uvx and LiteRT LM. satvikpendem noted that Unsloth's quantized models achieve higher accuracy than Google's QAT versions and are used in production for web search and JSON output. taffydavid raised a question about potential dual benefits for cloud inference, while jhatax speculated a connection to Apple's upcoming Siri improvements. Overall sentiment was positive, with jbarrow praising the rapid advancement of the Gemma ecosystem.

**Tags**: `#Gemma`, `#Quantization-Aware Training`, `#On-device AI`, `#Model Compression`, `#Hacker News`

---

<a id="item-5"></a>
## [Blog post questions if Claude AI increased bugs in rsync](https://alexispurslane.github.io/rsync-analysis/) ⭐️ 8.0/10

A blog post by Alexis Purslane analyzes rsync commit history and attributes an increase in bugs to the use of Claude AI for code changes. The analysis claims that Claude-introduced commits correlate with more fix commits. This sparks debate about the reliability of AI-assisted coding tools like Claude, especially for critical software like rsync. It raises concerns that LLM-generated code may introduce subtle bugs that are hard to catch through review. The blog post's methodology is criticized for lacking statistical power and potentially misattributing bugs due to the release timeline. One commenter points out a specific Claude-authored commit that changed a conditional to force all memory allocations to use calloc, which could be problematic for large or recursive calls.

hackernews · logicprog · Jun 5, 12:43 · [Discussion](https://news.ycombinator.com/item?id=48411635)

**Background**: rsync is a popular file synchronization tool for Unix-like systems, known for its efficiency and reliability. The use of large language models (LLMs) like Claude for code generation has become common, but concerns exist about their ability to produce correct and secure code, especially for complex systems. This analysis examines real-world impact on rsync's codebase.

**Discussion**: Comments are divided: some support the methodology, while many point out flaws in the analysis. One user highlights a specific commit where Claude changed a condition, potentially introducing a calloc-only allocation path. Another notes that the release with the most bugs predates Claude usage, suggesting misattribution. The rsync author's defense is also referenced.

**Tags**: `#rsync`, `#AI coding`, `#software bugs`, `#LLM`, `#code quality`

---

<a id="item-6"></a>
## [MicroPython compiled to WebAssembly enables safe Python sandbox](https://simonwillison.net/2026/Jun/6/micropython-in-a-sandbox/#atom-everything) ⭐️ 8.0/10

Simon Willison released an alpha package called micropython-wasm that compiles MicroPython to WebAssembly, allowing Python code to run in a sandboxed environment. He also created a Datasette plugin, datasette-agent-micropython, to use this sandbox for safe code execution. This approach addresses a long-standing challenge in Python plugin systems: executing untrusted code without risking data leaks or system crashes. It could enable safer plugin ecosystems for Datasette, LLM, and other Python applications. The sandbox imposes both memory and CPU limits, and restricts file access and network connectivity. The alpha package can be installed from PyPI with standard tooling, requiring no extra steps beyond typical package installation.

rss · Simon Willison · Jun 6, 03:53

**Background**: MicroPython is a lean implementation of Python 3 optimized for microcontrollers and constrained environments. WebAssembly (Wasm) is a portable binary format designed for high-performance execution on web pages and other hosts. Datasette is an open-source tool for exploring and publishing data as an interactive website and API, which supports plugins for extensibility.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/MicroPython">MicroPython</a></li>
<li><a href="https://en.wikipedia.org/wiki/WebAssembly">WebAssembly</a></li>
<li><a href="https://datasette.io/">Datasette: An open source multi-tool for exploring and publishing data</a></li>

</ul>
</details>

**Tags**: `#Python`, `#WebAssembly`, `#Sandbox`, `#Security`, `#MicroPython`

---

<a id="item-7"></a>
## [Ladybird Browser Bans Public Pull Requests Over AI Code Concerns](https://simonwillison.net/2026/Jun/5/andreas-kling/#atom-everything) ⭐️ 8.0/10

Ladybird browser announced it will no longer accept public pull requests, citing that the assumption of good faith based on effort no longer holds due to AI-generated contributions. This policy shift reflects growing challenges in open-source projects to maintain code accountability and provenance in the era of generative AI, potentially influencing how other projects manage contributions. Andreas Kling, the founder of Ladybird, emphasized that the person who introduces code changes must be responsible for them, regardless of whether the code was typed by hand or generated by AI.

rss · Simon Willison · Jun 5, 11:10

**Background**: Ladybird is an open-source, privacy-focused web browser built from scratch, not based on existing browser engines. It was originally a component of SerenityOS and is now developed as a standalone project by the Ladybird Browser Initiative, a nonprofit funded by donations and sponsors like Cloudflare and Shopify.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Ladybird_(web_browser)">Ladybird (web browser)</a></li>

</ul>
</details>

**Tags**: `#ladybird`, `#open-source`, `#ai-ethics`, `#software-engineering`, `#code-quality`

---

<a id="item-8"></a>
## [AI Enthusiasts vs. Skeptics: Race Against Time or Entropy?](https://simonwillison.net/2026/Jun/4/ai-enthusiasts-ai-skeptics/#atom-everything) ⭐️ 8.0/10

Charity Majors published a blog post analyzing the fundamental tension between AI enthusiasts racing to adopt AI for competitive advantage and AI skeptics warning about technical debt and loss of institutional knowledge. The post highlights the lack of natural feedback loops connecting these two groups within teams. This tension is critical because both perspectives are valid and ignoring either can be an existential threat to software teams. The post offers a framework for designing feedback loops to bridge the gap, which is essential for building reliable, high-performing AI-powered systems. The post compares AI enthusiasts' urgency to a race against time, where delaying adoption risks being outpaced by competitors, while skeptics face a race against entropy, where rapid code shipping erodes reliability and context. Charity Majors recommends treating this as both a leadership and engineering challenge.

rss · Simon Willison · Jun 4, 23:55

**Background**: In software engineering, technical debt refers to the implied cost of additional rework caused by choosing an easy solution now instead of a better approach that would take longer. Entropy in this context describes the gradual decay of system understanding and reliability as code accumulates without sufficient review or documentation. The debate mirrors a broader industry conversation about balancing innovation speed with system stability.

**Tags**: `#AI`, `#software engineering`, `#technical debt`, `#risk management`

---

<a id="item-9"></a>
## [TinyTPU: Real SystemVerilog TPU runs in browser via WASM](https://www.reddit.com/r/MachineLearning/comments/1txvvo4/tinytpu_systemverilog_systolic_array_compiled_to/) ⭐️ 8.0/10

The TinyTPU project implements a 4×4 weight-stationary systolic array in SystemVerilog, compiles it to WebAssembly, and provides a live browser demo with step-by-step visualization of matrix multiplication, verified against a numpy golden model. This project offers an unprecedented hands-on educational tool that makes the inner workings of TPUs and systolic arrays accessible to anyone with a browser, demystifying concepts like weight-stationary dataflow and diagonal staggering. The demo includes three levels: L1 for a single MAC cell, L2 for the full 4×4 array executing a real matmul, and L3 for tiling larger matrices. The visualization reads state directly from the compiled RTL, ensuring no simulated data.

reddit · r/MachineLearning · /u/Horror-Flamingo-2150 · Jun 5, 20:05

**Background**: A systolic array is a network of processing elements (PEs) that rhythmically compute and pass data, analogous to blood flow. In a weight-stationary systolic array, weights are pre-loaded into the PEs while inputs and partial sums propagate through the array each clock cycle. This architecture is the core of Google's TPU and enables efficient matrix multiplication for deep learning.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Systolic_array">Systolic array</a></li>
<li><a href="https://telesens.co/2018/07/30/systolic-architectures/">Understanding Matrix Multiplication on a Weight-Stationary Systolic Architecture | Telesens</a></li>

</ul>
</details>

**Tags**: `#systolic array`, `#SystemVerilog`, `#TPU`, `#hardware visualization`, `#WASM`

---

<a id="item-10"></a>
## [Intricacies of Modern Camera Lens Repair](https://salvagedcircuitry.com/sigma-45mm.html) ⭐️ 7.0/10

A detailed article on salvagedcircuitry.com walks through the complete disassembly and repair of a Sigma 45mm lens, revealing the challenges of modern lens construction. As camera lenses become increasingly complex electronic-optical systems, such repair guides empower hobbyists and technicians to fix rather than replace expensive gear, reducing electronic waste. The author highlights that using Phillips (PH) screwdrivers on Japanese Industrial Standard (JIS) screws almost always strips them, and notes that fuses in lens electronics are only for fire prevention, not component protection.

hackernews · transistor-man · Jun 6, 00:33 · [Discussion](https://news.ycombinator.com/item?id=48420148)

**Background**: Modern camera lenses integrate multiple glass elements, autofocus motors, and flexible printed circuits (flex cables) sealed in tight assemblies. Disassembly requires careful handling of tiny screws, ribbon cables, and precise optical alignment. The article on salvagedcircuitry.com provides a rare, thorough look inside a Sigma 45mm f/2.8 lens.

<details><summary>References</summary>
<ul>
<li><a href="https://www.youtube.com/@CamerasLensesEtc/videos">CamerasLensesEtc - YouTube</a></li>
<li><a href="https://1library.net/document/zgdxexnz-active-alignment-cameras-mobile-devices-automotive-applications.html">Active Alignment for Cameras in Mobile Devices and Automotive...</a></li>

</ul>
</details>

**Discussion**: Commenters praised the detailed guide and shared practical tips, such as using double-sided tape to organize screws. A key point debated was the distinction between JIS and PH screwdrivers, with one user warning that PH drivers always strip JIS screws. Another clarified that fuses in such devices are only for fire safety, not for protecting electronics.

**Tags**: `#camera lens`, `#repair`, `#electronics`, `#disassembly`, `#consumer hardware`

---

<a id="item-11"></a>
## [UK Gov Drops Stripe for Dutch Payment Provider Adyen](https://www.theregister.com/public-sector/2026/06/04/govuk-goes-dutch-on-payments-as-it-dumps-stripe/5250763) ⭐️ 7.0/10

The UK Government Digital Service (GDS) has replaced Stripe with Dutch payment platform Adyen as the payment services provider for GOV.UK Pay, covering non-Crown card payments and pay by bank services. This decision highlights the UK government's shift toward a non-U.S. provider for critical payment infrastructure, sparking debate on national tech independence and the scale of public sector contracts. Adyen was selected for its status as an acquiring bank and its ability to handle both card and bank transfer payments. The contract is reportedly small compared to typical enterprise deals, surprising some observers.

hackernews · toomuchtodo · Jun 5, 16:55 · [Discussion](https://news.ycombinator.com/item?id=48415217)

**Background**: GOV.UK Pay is a government-built online payment service used by public sector organizations to accept payments securely. Payment service providers (PSPs) like Stripe and Adyen handle transaction processing. Adyen is a Dutch fintech company listed on Euronext Amsterdam, offering a unified platform for online and in-person payments.

<details><summary>References</summary>
<ul>
<li><a href="https://gds.blog.gov.uk/2026/06/02/building-for-the-future-making-change-simple-on-gov-uk-pay/">Building for the future: Making change simple on GOV.UK Pay</a></li>
<li><a href="https://www.adyen.com/press-and-media/adyen-payments-gov-uk">Adyen Selected as Payment Services Provider for GOV.UK Pay</a></li>
<li><a href="https://en.wikipedia.org/wiki/Adyen">Adyen - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community comments expressed surprise at the contract's small size, with one noting it was a fraction of a US mid-size company's cloud bill. Others lamented that Stripe, founded by Irish brothers, could have been an EU company, and questioned the lack of a British-owned alternative. Another comment mentioned that Adyen refuses small clients under a million in volume.

**Tags**: `#gov.uk`, `#payment processing`, `#adyen`, `#stripe`, `#government IT`

---

<a id="item-12"></a>
## [OpenAI Launches Lockdown Mode to Prevent Prompt Injection Attacks](https://simonwillison.net/2026/Jun/5/openai-help-lockdown-mode/#atom-everything) ⭐️ 7.0/10

OpenAI has officially launched Lockdown Mode for ChatGPT, a security feature that limits outbound network requests to prevent data exfiltration from prompt injection attacks. The mode is rolling out to eligible personal and business accounts. Lockdown Mode addresses a critical gap in LLM security by cutting off data exfiltration vectors, which is the easiest leg of the 'Lethal Trifecta' to restrict. This makes ChatGPT safer for handling sensitive data, benefiting all users and enterprises. Lockdown Mode does not prevent prompt injections from appearing in processed content, but it blocks outbound network requests that could transmit stolen data. The feature uses deterministic mechanisms not evaluated by AI systems, reducing the risk of subversion.

rss · Simon Willison · Jun 5, 23:56

**Background**: Prompt injection is a cybersecurity exploit where attackers craft inputs to manipulate LLMs into unintended behavior, potentially causing data leaks. Data exfiltration refers to unauthorized transfer of data from a system. In ChatGPT, a prompt injection could trick the model into sending private data to an attacker via outbound requests. Lockdown Mode targets this final exfiltration step.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Data_exfiltration">Data exfiltration - Wikipedia</a></li>
<li><a href="https://www.paloaltonetworks.com/cyberpedia/what-is-a-prompt-injection-attack">What Is a Prompt Injection Attack? [Examples & Prevention] - Palo Alto Networks</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#ChatGPT`, `#prompt injection`, `#security`, `#lockdown mode`

---

<a id="item-13"></a>
## [Google Employees Mock Their Own AI; Spokesperson Backtracks on Human Oversight](https://simonwillison.net/2026/Jun/4/a-slightly-different-version/#atom-everything) ⭐️ 7.0/10

Google employees have been internally sharing memes that criticize the quality of the company's AI systems. After 404 Media reported the story, a Google spokesperson asked the outlet to publish a revised statement that no longer included the phrase 'it's critical that we maintain humans in the loop.' This incident reveals significant internal skepticism about Google's AI capabilities and a shift in the company's public stance on human oversight. It raises questions about AI ethics and transparency, especially as Google promotes its AI products to the public and businesses. The original statement from Google emphasized the importance of human oversight, but the retracted version removed that commitment entirely. The memes shared internally likely reflect frustrations with AI performance and decision-making.

rss · Simon Willison · Jun 4, 16:38

**Background**: The concept of 'human in the loop' (HITL) is an AI ethics principle where humans monitor and can override automated systems to ensure ethical outcomes. It is commonly advocated to prevent harmful decisions by AI. Google's removal of this phrase could signal a move toward greater automation with less direct human intervention, which may conflict with industry best practices.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/human-in-the-loop">What Is Human In The Loop (HITL)? | IBM</a></li>

</ul>
</details>

**Tags**: `#ai-ethics`, `#google`, `#ai`, `#journalism`

---

<a id="item-14"></a>
## [On-Policy Distillation: A Hot New Post-Training Technique](https://www.reddit.com/r/MachineLearning/comments/1twmhud/onpolicy_distillation_one_of_the_hottest_terms_on/) ⭐️ 7.0/10

On-policy distillation (OPD) has been added as a trending method on PapersWithCode, identified as a key post-training technique behind recent models like Qwen 3.6, Qwen 3.7, GLM-5.1, and DeepSeek-V4. This technique improves model training efficiency and accuracy by enabling targeted correction of errors during rollout, making it a significant advancement for large language model optimization. OPD uses a teacher model to insert hint tokens into error-prone parts of a trajectory, allowing the student model to adjust token probabilities without regenerating the entire sequence.

reddit · r/MachineLearning · /u/NielsRogge · Jun 4, 12:40

**Background**: On-policy distillation is a knowledge distillation method where the student model generates its own trajectories (on-policy sampling) and a teacher model provides token-level supervision. It differs from off-policy methods by using the student's own outputs, which reduces distribution mismatch. In large language models, OPD has become a crucial post-training step to fine-tune behavior after initial training.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/On-policy_distillation">On-policy distillation</a></li>
<li><a href="https://ulab-uiuc.github.io/OPD_website/">The Many Faces of On - Policy Distillation : Pitfalls, Mechanisms, and...</a></li>

</ul>
</details>

**Tags**: `#knowledge distillation`, `#on-policy distillation`, `#AI research`, `#post-training`, `#model optimization`

---

<a id="item-15"></a>
## [Is Capture-Time Semantic Annotation for Robot Trajectories Solved?](https://www.reddit.com/r/MachineLearning/comments/1txf4gg/would_you_say_capturetime_semantic_annotation_for/) ⭐️ 7.0/10

A Reddit user argues that raw teleoperation data inherently lacks affordance, contact intent, and embodiment-specific kinematic context, and questions whether capture-time semantic annotation—enriching data streams during acquisition rather than post-hoc—is a solved problem. If capture-time annotation remains unsolved, it could be a major bottleneck for learning contact-rich manipulation skills in unstructured environments, as post-hoc methods cannot recover missing semantic cues. The post highlights that current approaches either filter data after collection or rely on simulation, which do not close the semantic gap for contact-rich tasks. The author asks whether real-time annotation during teleoperation is being actively worked on.

reddit · r/MachineLearning · /u/Several-Many9101 · Jun 5, 08:42

**Background**: In robot learning, semantic annotation labels trajectories with object affordances (possible interactions) and contact intent (planned touch). Affordance research helps robots understand what actions are possible on objects. Post-hoc annotation is common but often misses context not recorded during data collection, such as tactile feedback or operator intent.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2004.07400">[2004.07400] Affordances in Robotic Tasks -- A Survey</a></li>
<li><a href="https://www.cvat.ai/resources/blog/robotics-data-annotation">Data Annotation for Robotics AI: Unique Challenges, Key Methods, and Best Practices | CVAT Blog</a></li>
<li><a href="https://arxiv.org/pdf/2512.11472">Mirror Skin: In Situ Visualization of Robot Touch Intent on Robotic Skin</a></li>

</ul>
</details>

**Tags**: `#robot learning`, `#semantic annotation`, `#imitation learning`, `#teleoperation`, `#data collection`

---

<a id="item-16"></a>
## [ISS Astronauts Shelter During Air Leak Repair Attempt](https://www.bbc.com/news/live/c4g44ew3g1kt) ⭐️ 6.0/10

Astronauts on the International Space Station were directed to shelter in place in the Russian segment amid ongoing repairs to an air leak. The procedure was initiated as a precaution during a Russian attempt to seal the leak in the tunnel area. The incident highlights the persistent challenges of maintaining the aging ISS and the critical role of redundant safety procedures. It also underscores the reliance on international cooperation for crew safety. The air leak, located in the Russian segment, has been a recurring issue since 2019. NASA's RELL (Robotic External Leak Locator) and other acoustic detection tools were used to identify the leak source.

hackernews · janpot · Jun 5, 15:00 · [Discussion](https://news.ycombinator.com/item?id=48413464)

**Background**: The International Space Station (ISS) is composed of modules from multiple space agencies, each with its own atmosphere and life support systems. During emergency repairs, astronauts may shelter in a specific module to ensure their safety if pressure drops critically. Leak detection on the ISS involves technologies like ultrasonic probes and acoustic cameras that can pinpoint tiny holes.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bbc.com/news/articles/c5y7yryg01mo">Nasa tells ISS astronauts to shelter during air leak repair attempt</a></li>
<li><a href="https://www.livescience.com/space/space-exploration/nasa-astronauts-briefly-shelter-in-safe-haven-procedure-following-worsening-leaks-on-international-space-station">NASA astronauts briefly shelter in 'safe haven' procedure following ...</a></li>
<li><a href="https://distran.swiss/en/nasa-ultra-pro-iss/">NASA applies Distran Ultra Pro to Pinpoint ISS air leaks</a></li>

</ul>
</details>

**Discussion**: Commenters discussed the effectiveness of leak detection technology like NASA's RELL and questioned the logic of sheltering when airlocks could isolate sections. Some expressed curiosity about emergency escape capabilities, while others wondered why sealing leaks is so difficult.

**Tags**: `#ISS`, `#space`, `#engineering`, `#leak detection`

---

<a id="item-17"></a>
## [Solar desalination method claims zero waste, faces skepticism](https://www.rochester.edu/newscenter/what-is-desalination-definition-ocean-water-704732/) ⭐️ 6.0/10

Researchers at the University of Rochester have developed a solar-powered desalination system using a specially engineered black metal that absorbs sunlight and moves salt away via capillary action, potentially eliminating waste and clogging. The method is still at lab scale and has not been demonstrated in a practical system. If proven scalable and durable, this approach could provide a low-energy, waste-free desalination solution for water-stressed regions. However, thermodynamic limits and the lack of a practical demonstration raise doubts about its real-world viability. The system uses a laser-prepared black metal surface to enhance solar absorption and prevent salt buildup by moving brine away from the evaporation area via capillary action. The research remains at the proof-of-concept stage with a glass-based lab setup, and a mechanism for long-term salt removal has not yet been developed.

hackernews · speckx · Jun 5, 15:04 · [Discussion](https://news.ycombinator.com/item?id=48413500)

**Background**: Desalination removes salt from seawater to produce fresh water, but conventional methods like reverse osmosis require significant energy and produce concentrated brine waste. The thermodynamic minimum energy for desalination is set by the laws of physics, and any new method must approach this limit to be efficient. Zero-liquid discharge (ZLD) aims to eliminate waste by recovering all water and salts, but is typically energy-intensive. This new method claims to achieve ZLD passively using solar energy.

<details><summary>References</summary>
<ul>
<li><a href="https://esg.sustainability-directory.com/learn/what-is-the-thermodynamic-limit-for-desalination-and-how-does-it-compare-to-current-technologies/">What Is the Thermodynamic Limit for Desalination and How Does It ...</a></li>
<li><a href="https://www.researchgate.net/publication/303872744_The_Global_Rise_of_Zero_Liquid_Discharge_for_Wastewater_Management_Drivers_Technologies_and_Future_Directions">(PDF) The Global Rise of Zero Liquid Discharge for Wastewater...</a></li>

</ul>
</details>

**Discussion**: Commenters point out that the method must be compared against the fundamental thermodynamic limit for desalination, and that the anti-clogging mechanism has not been demonstrated in a practical, long-term system. Some express skepticism, while others note interest in the laser surface preparation technique as a potential advancement if proven durable.

**Tags**: `#desalination`, `#solar energy`, `#water purification`, `#thermodynamics`, `#research`

---

<a id="item-18"></a>
## [AI Agent Skill for Test-Driven Development](https://www.saturnci.com/my-agent-skill-for-test-driven-development.html) ⭐️ 6.0/10

The author presents a custom agent skill that guides AI agents to follow Test-Driven Development (TDD) practices, including detailed prompts and workflows for red/green TDD and specify-encode-fulfill loops. This approach could improve the reliability of AI-generated code by embedding TDD discipline into agent workflows, potentially influencing how developers integrate AI into testing and development processes. The skill is built on Kent Beck's Canon TDD, but community members note that token costs can balloon and tests may be superficial hallucinations that do not properly validate components.

hackernews · laxmena · Jun 4, 14:10 · [Discussion](https://news.ycombinator.com/item?id=48398925)

**Background**: Test-Driven Development (TDD) is a software development process where tests are written before the code that needs to pass them. AI agents are increasingly used to automate coding tasks, but ensuring quality requires structured guidance. The skill described in the article aims to codify TDD practices for AI agents, but its effectiveness is debated due to concerns about cost and test quality.

<details><summary>References</summary>
<ul>
<li><a href="https://www.saturnci.com/my-agent-skill-for-test-driven-development.html">My Agent Skill for Test-Driven Development - SaturnCI - Continuous Integration for Ruby on Rails</a></li>
<li><a href="https://addyosmani.com/blog/agent-skills/">AddyOsmani.com - Agent Skills</a></li>

</ul>
</details>

**Discussion**: Commenters are divided: some argue that TDD with agents leads to complacency and high token costs, while others praise integrated workflows that create shared understanding and bug-free code. The lack of a publication date is also noted as a concern for relevance.

**Tags**: `#TDD`, `#AI agents`, `#software development`, `#test automation`

---

<a id="item-19"></a>
## [GitHub repo collects Transformer attention implementations](https://www.reddit.com/r/MachineLearning/comments/1twhhnq/repo_for_implementations_of_various_transformer/) ⭐️ 6.0/10

A new GitHub repository, attnhut, provides implementations of multiple Transformer attention mechanisms, including MiniMax M3's sparse attention, designed for easy integration into small language models and other architectures. This resource saves researchers and students the time of reimplementing attention variants, enabling rapid experimentation across NLP, computer vision, and reinforcement learning domains. The repository works with Andrej Karpathy's autoresearch framework and welcomes community contributions via pull requests to include additional attention mechanisms.

reddit · r/MachineLearning · /u/AnyIce3007 · Jun 4, 08:28

**Background**: Attention mechanisms are core components of Transformer models, allowing the model to focus on different parts of the input. Many variants exist (e.g., sparse, linear, sliding window) for efficiency or performance. This repo centralizes these variants, making it easier to benchmark and switch between them.

<details><summary>References</summary>
<ul>
<li><a href="https://www.minimax.io/models/text/m3">MiniMax M3 - Coding & Agentic Frontier, 1M Context, Multimodal</a></li>
<li><a href="https://github.com/karpathy/autoresearch">GitHub - karpathy/autoresearch: AI agents running research on single-GPU nanochat training automatically · GitHub</a></li>

</ul>
</details>

**Tags**: `#Transformer`, `#Attention Mechanisms`, `#GitHub`, `#Deep Learning`, `#Open Source`

---