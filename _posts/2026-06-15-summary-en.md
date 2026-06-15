---
layout: default
title: "Horizon Summary: 2026-06-15 (EN)"
date: 2026-06-15
lang: en
---

> From 24 items, 16 important content pieces were selected

---

1. [Pyodide 314.0 Enables WASM Wheel Publishing to PyPI](#item-1) ⭐️ 9.0/10
2. [US Government Orders Anthropic to Suspend Fable 5 and Mythos 5 Access](#item-2) ⭐️ 9.0/10
3. [Kage turns websites into offline single-binary archives](#item-3) ⭐️ 8.0/10
4. [Rio's 'homegrown' LLM exposed as merge of existing models](#item-4) ⭐️ 8.0/10
5. [Critique Compares Anthropic to Doomsday Device Firm](#item-5) ⭐️ 8.0/10
6. [Formal Methods and the Future of Programming](#item-6) ⭐️ 8.0/10
7. [Why AI Won't Replace Software Engineers](#item-7) ⭐️ 8.0/10
8. [Mapping SQLite result columns to source table.column](#item-8) ⭐️ 8.0/10
9. [Open-source Knowledge Graph pipeline with hybrid retrieval improves LLM reasoning](#item-9) ⭐️ 8.0/10
10. [Coherent Context Shifts LLM Internal Regime, Evading Safety Systems](#item-10) ⭐️ 8.0/10
11. [Verifier Tax: Safety–Success Tradeoff in Tool-Using LLM Agents](#item-11) ⭐️ 8.0/10
12. [PaddleOCR v3-v6 implemented in C++ with ncnn for lightweight OCR deployment](#item-12) ⭐️ 7.0/10
13. [Caddy-Compatible Zeroserve Boosts Performance but Lacks Key Features](#item-13) ⭐️ 6.0/10
14. [Free bilingual ML notebook course seeks feedback](#item-14) ⭐️ 6.0/10
15. [Anomaly Detection vs Classification for Cancer Mimics](#item-15) ⭐️ 6.0/10
16. [MDP Derivative-Free Optimizer Beats Adam on MNIST](#item-16) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Pyodide 314.0 Enables WASM Wheel Publishing to PyPI](https://simonwillison.net/2026/Jun/13/publishing-wasm-wheels/#atom-everything) ⭐️ 9.0/10

Pyodide 314.0 now allows package maintainers to build and publish WebAssembly (WASM) wheels directly to PyPI, which can be installed at runtime using micropip. Previously, Pyodide maintainers had to manually build and host over 300 packages. This removes a major bottleneck in the Pyodide ecosystem, reducing the burden on core maintainers and empowering the community to distribute Python packages for browser-based environments. It aligns with the broader trend of making Python fully functional in the browser via WebAssembly. The support is based on the PyEmscripten platform defined in PEP 783, and the corresponding PyPI changes landed via PR #19804 on April 21st. Simon Willison demonstrated the workflow by publishing a luau-wasm package that runs a Lua-like language inside Pyodide.

rss · Simon Willison · Jun 13, 23:55

**Background**: Pyodide is a Python distribution for the browser and Node.js based on WebAssembly, enabling Python code to run client-side. Until now, distributing Python packages with compiled C or Rust extensions that target WASM required manual hosting and wasn't possible through PyPI. PEP 783 standardizes the platform tag for these wheels, making integration with PyPI feasible.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/13/publishing-wasm-wheels/">Publishing WASM wheels to PyPI for use with Pyodide</a></li>
<li><a href="https://pyodide.org/">Pyodide — Version 314.0.0</a></li>
<li><a href="https://peps.python.org/pep-0783/">PEP 783 – Emscripten Packaging | peps .python.org</a></li>

</ul>
</details>

**Tags**: `#Pyodide`, `#WebAssembly`, `#PyPI`, `#Python`, `#WASM`

---

<a id="item-2"></a>
## [US Government Orders Anthropic to Suspend Fable 5 and Mythos 5 Access](https://simonwillison.net/2026/Jun/13/us-government-directive-to-suspend-access/#atom-everything) ⭐️ 9.0/10

The US government issued an export control directive to Anthropic on June 12, 2026, ordering the suspension of all access to the Fable 5 and Mythos 5 AI models, citing national security concerns over a discovered jailbreak method. Anthropic complied by disabling access for all customers, including foreign national employees, effective immediately. This unprecedented government intervention marks a major shift in AI policy, potentially setting a precedent for national security reviews of advanced AI models. It raises critical questions about model security, regulatory overreach, and the future of open access to frontier AI capabilities. The alleged jailbreak involves asking the model to review a specific codebase and fix software flaws, a technique Anthropic argues is not unique to their models and is used by defenders in normal security work. Access to Fable 5 was cut off at 6:59 PM Pacific on June 12, 2026, as confirmed by Simon Willison's API test.

rss · Simon Willison · Jun 13, 01:01

**Background**: Claude Fable 5 and Claude Mythos 5 are advanced large language models from Anthropic, launched in June 2026. Mythos 5 is a 'Mythos-class' model designed for security research and autonomous coding, while Fable 5 is optimized for frontier physics research with a 1M-token context window. Both models share the same underlying base model and represent a significant leap in AI capability, exceeding previous models like GPT-5.5 in certain benchmarks.

<details><summary>References</summary>
<ul>
<li><a href="https://mashable.com/tech/anthropic-claude-fable-5-vs-openai-gpt-5-5">Claude Fable 5 vs GPT 5.5: Is this why the Trump admin... | Mashable</a></li>
<li><a href="https://9to5mac.com/2026/06/12/anthropic-pulls-claude-mythos-5-and-claude-fable-5-following-us-government-directive/">Anthropic pulls Claude Mythos 5 and Claude Fable... - 9to 5 Mac</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#government regulation`, `#model security`, `#Anthropic`, `#national security`

---

<a id="item-3"></a>
## [Kage turns websites into offline single-binary archives](https://github.com/tamnd/kage) ⭐️ 8.0/10

Kage is a new open-source tool that clones any website into a single binary file for offline viewing, driving a real browser to capture pages and then stripping JavaScript. This simplifies website archiving and offline access, making it easy to share or preserve complex sites without needing a full web server setup. The tool uses a headless browser to capture dynamic content but produces a static site that must be served via its built-in HTTP server; it cannot be opened directly from the filesystem.

hackernews · tamnd · Jun 14, 17:25 · [Discussion](https://news.ycombinator.com/item?id=48529990)

**Background**: Traditional methods like 'Save As' produce incomplete archives for modern JavaScript-heavy sites. Kage (影, 'shadow') instead drives a real browser to capture the page as a user sees it, then makes it inert, preserving the visual structure without dependencies.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/tamnd/kage">GitHub - tamnd/kage: Shadow any website for offline viewing, with the JavaScript stripped out · GitHub</a></li>
<li><a href="https://kage.tamnd.com/">kage</a></li>

</ul>
</details>

**Discussion**: Users reported a bug with HTTP sites (DNS resolution fails). Others discussed use cases like offline company wikis and archiving AI prototypes, and suggested improvements such as a no-server HTML file output.

**Tags**: `#offline`, `#website mirroring`, `#tool`, `#archiving`, `#productivity`

---

<a id="item-4"></a>
## [Rio's 'homegrown' LLM exposed as merge of existing models](https://github.com/nex-agi/Nex-N2/issues/4) ⭐️ 8.0/10

A community investigation revealed that the Rio-3.5-Open-397B model, released by the municipality of Rio de Janeiro as a homegrown fine-tune, is actually a weighted merge of Nex-N2 Pro and Qwen3.5, with no proper attribution. This case highlights the need for transparency and proper attribution in AI model releases, especially from public institutions, and raises concerns about the prevalence of undisclosed model merging in the field. Every weight tensor in the Rio model is approximately a 0.6/0.4 blend of Nex and Qwen across all layers, and the model was presented as a fine-tune outperforming comparable open models, but without mentioning the merge.

hackernews · unrvl22 · Jun 14, 15:37 · [Discussion](https://news.ycombinator.com/item?id=48528371)

**Background**: Model merging is a technique that combines the weights of multiple models sharing the same base architecture into a single model, often without retraining. It can improve performance but requires proper disclosure to respect original creators' work. This incident is part of a broader discussion about ethical practices in open-source AI.

<details><summary>References</summary>
<ul>
<li><a href="https://mychen76.medium.com/the-art-of-model-blending-and-moerges-bac7f3749ab7">LLM Model Merging . In this article, I will share my views | Medium</a></li>
<li><a href="https://arxiv.org/html/2408.07666v5">Model Merging in LLMs, MLLMs, and Beyond: Methods, Theories...</a></li>

</ul>
</details>

**Discussion**: The community comments show mixed reactions: some hypothesize innocent technical reasons (e.g., lack of distillation inclusion), while others criticize the lack of attribution and suspect this is common practice. One commenter notes that a simple linear combination of weights enhanced performance without degradation.

**Tags**: `#LLM`, `#model attribution`, `#open source`, `#ethics`, `#community investigation`

---

<a id="item-5"></a>
## [Critique Compares Anthropic to Doomsday Device Firm](https://www.verysane.ai/p/did-anthropic-ask-for-this) ⭐️ 8.0/10

A critical article draws an analogy between Anthropic and a doomsday device company, accusing the AI safety firm of hypocrisy by profiting from the very technology it warns against. This critique could undermine Anthropic's credibility in the AI safety community, influencing public trust and regulatory scrutiny of the company's ethical claims. The article uses the analogy of a doomsday device company that warns about risks while profiting from selling the devices, to highlight perceived contradictions in Anthropic's dual role as safety advocate and AI developer.

hackernews · ad8e · Jun 14, 22:23 · [Discussion](https://news.ycombinator.com/item?id=48533504)

**Background**: Anthropic is an AI research company founded by former OpenAI employees, with a strong emphasis on safety and ethics. The company develops powerful AI models like Claude while advocating for regulation. This article questions whether such a dual role is inherently contradictory, sparking debate about hubris and ethical positioning.

**Discussion**: Commenters are divided: some agree with the critique, pointing to hubris and self-interest; others defend Anthropic, arguing that genuine belief in existential risk justifies their actions. There is also discussion of government influence and the political environment surrounding AI regulation.

**Tags**: `#AI safety`, `#Anthropic`, `#ethics`, `#tech criticism`, `#hubris`

---

<a id="item-6"></a>
## [Formal Methods and the Future of Programming](https://blog.janestreet.com/formal-methods-at-jane-street-index/?from_theconsensus=1) ⭐️ 8.0/10

Jane Street explores the integration of formal methods into programming, arguing that as AI generates more code, human value will shift toward verification and proof assistance. This perspective highlights a potential shift in software engineering toward rigorous verification, which could improve reliability and safety, especially in critical systems. The blog post discusses the use of formal methods like proof assistants and SAT solvers, and notes that the hardest part is the human task of suggesting lemmas and guiding proofs.

hackernews · eatonphil · Jun 14, 12:35 · [Discussion](https://news.ycombinator.com/item?id=48526633)

**Background**: Formal methods are mathematically rigorous techniques for specifying and verifying software/hardware systems. Proof assistants like Coq or Isabelle enable interactive theorem proving, where humans guide the proof search.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Formal_methods">Formal methods</a></li>
<li><a href="https://en.wikipedia.org/wiki/Proof_assistant">Proof assistant</a></li>

</ul>
</details>

**Discussion**: Comments from experts like 'Animats' describe historical experiences with proof automation, noting that easy parts were handled by SAT solvers while harder proofs required human guidance. Another commenter, 'winwang', shares using expressive types in Scala 3 for compile-time proofs, which helps prevent AI-generated code quality issues.

**Tags**: `#formal methods`, `#programming languages`, `#AI verification`, `#software reliability`, `#Hacker News`

---

<a id="item-7"></a>
## [Why AI Won't Replace Software Engineers](https://simonwillison.net/2026/Jun/14/why-ai-hasnt-replaced-software-engineers/#atom-everything) ⭐️ 8.0/10

Arvind Narayanan and Sayash Kapoor published an essay arguing that AI will not cause mass layoffs of software engineers, citing data from New York's WARN Act filings where no company reported AI-related layoffs in the first year. This directly counters the prevailing narrative that AI will soon automate software engineering jobs, providing evidence-based reassurance to developers and influencing discussions on AI's economic impact. The essay identifies three real bottlenecks that AI cannot replace: deciding what to build, verifying delivered work, and deep human understanding of the codebase, business, and environment.

rss · Simon Willison · Jun 14, 23:54

**Background**: AI coding assistants like GitHub Copilot have advanced rapidly, sparking fears that software engineers might be replaced. However, professional software engineering involves far more than typing code—it requires complex reasoning, communication, and accountability.

**Tags**: `#AI`, `#software engineering`, `#job automation`, `#economy`

---

<a id="item-8"></a>
## [Mapping SQLite result columns to source table.column](https://simonwillison.net/2026/Jun/13/sqlite-column-provenance/#atom-everything) ⭐️ 8.0/10

Simon Willison researched methods to programmatically map SQL query result columns to their source table and column in SQLite, using Claude Code (Opus 4.8) to explore solutions including apsw, ctypes access to sqlite3_column_table_name(), and EXPLAIN output analysis. This work could enable Datasette to enrich SQL query results with column provenance information, improving data analysis and debugging for users. The use of AI-assisted coding to solve a concrete technical problem demonstrates a novel approach to database tool development. Claude Code identified three promising approaches: using the apsw library, directly calling the SQLite C function sqlite3_column_table_name() via Python ctypes, and parsing EXPLAIN output to infer column origins. The research is hosted in a public GitHub repository under simonw/research.

rss · Simon Willison · Jun 13, 23:05

**Background**: Datasette is an open-source tool for exploring and publishing data, often used with SQLite. Column provenance means tracking which table and column each result value comes from, which is not directly exposed by SQLite's Python bindings. The SQLite C API provides the sqlite3_column_table_name() function, but Python does not expose it. Claude Code is Anthropic's agentic coding tool that can read codebases and execute commands.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/13/sqlite-column-provenance/">Research: Mapping SQLite result columns back to their source...</a></li>
<li><a href="https://code.claude.com/docs/en/overview">Overview - Claude Code Docs</a></li>

</ul>
</details>

**Tags**: `#SQLite`, `#Datasette`, `#Query Parsing`, `#AI-Assisted Coding`

---

<a id="item-9"></a>
## [Open-source Knowledge Graph pipeline with hybrid retrieval improves LLM reasoning](https://www.reddit.com/r/MachineLearning/comments/1u5yyyl/i_built_an_opensource_knowledge_graph_pipeline/) ⭐️ 8.0/10

A developer released an open-source full-stack pipeline that constructs a knowledge graph from raw text, detects thematic communities, and uses hybrid retrieval (dense vectors + BM25) to solve the 'lost in the middle' problem and improve multi-hop reasoning for LLMs. This addresses a critical flaw in standard vector retrieval where disconnected chunks cause multi-hop queries to fail. By fusing graph traversal with hybrid search, the pipeline enables LLMs to reason across multiple steps, which is vital for applications like question answering and document analysis. The pipeline uses spaCy for entity extraction, NetworkX with greedy modularity for community detection, and generates LLM summaries per community. Retrieval combines dense vector search and BM25, fused via Reciprocal Rank Fusion (RRF), then reranked by a cross-encoder.

reddit · r/MachineLearning · /u/Future_Caregiver_643 · Jun 14, 22:38

**Background**: Standard RAG (Retrieval-Augmented Generation) systems often struggle with multi-hop questions that require connecting facts from different pieces of text. A knowledge graph explicitly represents entities and their relationships, enabling graph traversal to bridge disconnected chunks. Hybrid retrieval, combining dense (semantic) and sparse (lexical) search, covers both semantic drift and exact keyword matches, improving retrieval quality.

<details><summary>References</summary>
<ul>
<li><a href="https://neo4j.com/blog/genai/knowledge-graph-llm-multi-hop-reasoning/">How to improve multi-hop reasoning with knowledge graphs and LLMs - Graph Database & Analytics</a></li>
<li><a href="https://sabankara.medium.com/why-we-should-upgrade-classical-rag-with-hybrid-sparse-dense-retrieval-and-reranking-2b991d4bb95f">Why We Should “Upgrade” Classical RAG with Hybrid ( Sparse ...)</a></li>
<li><a href="https://www.aidoczh.com/networkx/reference/algorithms/generated/networkx.algorithms.community.modularity_max.greedy_modularity_communities.html">greedy_modularity_communities — NetworkX 3.4rc0.dev0 documentation</a></li>

</ul>
</details>

**Tags**: `#knowledge graph`, `#LLM`, `#hybrid retrieval`, `#open-source`, `#NLP`

---

<a id="item-10"></a>
## [Coherent Context Shifts LLM Internal Regime, Evading Safety Systems](https://www.reddit.com/r/MachineLearning/comments/1u5xnxg/coherent_context_can_silently_shift_llms_into_a/) ⭐️ 8.0/10

An independent researcher discovered that providing a coherent, dense piece of text as context can shift an LLM's internal regime (hidden states and residual stream trajectory) without altering its surface output, and this shift is not detected by current safety filters like RLHF or output classifiers. This finding reveals a fundamental blind spot in current LLM alignment methods, which only monitor final outputs; it suggests that safety measures must evolve to monitor hidden-state regimes continuously, as coherent context alone can silently bypass them. The experiments were conducted primarily on the open-source model Gemma-3-12B-IT, using hidden-state geometry, residual stream trajectories, contrastive controls, SAE readouts, and teacher-forced KL divergence. The target texts were not explicit jailbreak prompts but dense, coherent pieces that established a specific discourse mode.

reddit · r/MachineLearning · /u/PresentSituation8736 · Jun 14, 21:42

**Background**: Large language models (LLMs) process text through stacked transformer layers, each adding information to a 'residual stream' that carries hidden states across tokens. Mechanistic interpretability studies these internal states to understand how models reason. Current safety alignment methods like RLHF and output classifiers only check the final generated text, ignoring the internal representation spaces where different regimes may already be active.

<details><summary>References</summary>
<ul>
<li><a href="https://paperdive.ai/concepts/residual-stream.html">Residual Stream · AI Papers: A Deep Dive</a></li>
<li><a href="https://medium.com/@khayyam.h/understanding-and-controlling-llm-internal-representations-87c939957b25">Understanding and controlling LLM internal representations | by Khayyam H. | Medium</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#mechanistic interpretability`, `#LLM alignment`, `#representation space`, `#hidden states`

---

<a id="item-11"></a>
## [Verifier Tax: Safety–Success Tradeoff in Tool-Using LLM Agents](https://www.reddit.com/r/MachineLearning/comments/1u58mkq/the_verifier_tax_horizondependent_safetysuccess/) ⭐️ 8.0/10

A paper presented at ACM CAIS 2026 introduces the Verifier Tax, a horizon-dependent safety–success tradeoff observed in tool-using LLM agents, and proposes a two-tier verification architecture to mitigate unsafe completions. This research formalizes a critical evaluation pitfall in LLM agent safety, showing that verification can reduce unsafe successes but also penalize task completion as task horizon increases. It could reshape how agent evaluations are designed and reported. The paper evaluates on τ-bench tool-use scenarios and uses a two-tier architecture: deterministic policy/tool checks first, then an LLM-based verifier for contextual safety. The Verifier Tax quantifies the tradeoff between safety and success that worsens with longer horizons.

reddit · r/MachineLearning · /u/AccomplishedLeg1508 · Jun 14, 02:09

**Background**: Tool-using LLM agents can complete tasks but may violate safety policies, creating 'unsafe successes.' Standard benchmarks often treat completion as success without checking safety, masking this risk. τ-bench is a benchmark for tool-agent-user interaction in real-world domains, providing scenarios like flight rescheduling and baggage handling.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/sierra-research/tau2-bench">GitHub - sierra-research/tau2-bench: τ-Bench: A Benchmark for Tool-Agent-User Interaction in Real-World Domains · GitHub</a></li>
<li><a href="https://www.preprints.org/manuscript/202604.1029">AgentVerify: Compositional Formal Verification of AI Agent Safety Properties via LTL Model Checking[v1] | Preprints.org</a></li>

</ul>
</details>

**Tags**: `#LLM Agents`, `#AI Safety`, `#Verification`, `#Tool Use`, `#Evaluation`

---

<a id="item-12"></a>
## [PaddleOCR v3-v6 implemented in C++ with ncnn for lightweight OCR deployment](https://www.reddit.com/r/MachineLearning/comments/1u4hy2x/paddleocr_v3v4v5v6_implemented_in_c_with_ncnn_p/) ⭐️ 7.0/10

A developer has released an open-source C++ implementation of PaddleOCR using the ncnn inference framework, now supporting PP-OCR v3 through the latest v6 models. This replaces the official Paddle C++ runtime, which is heavy and complex, with a lighter and faster alternative. This project simplifies OCR deployment for developers working on mobile or edge devices, where lightweight inference is critical. It reduces dependency overhead and improves inference speed, making state-of-the-art OCR more accessible for resource-constrained environments. The implementation uses ncnn, a high-performance neural network inference framework designed for mobile platforms, which supports most common CNN networks. The repository includes support for multiple PaddleOCR model versions from v3 to v6, enabling users to choose the best model for their accuracy and speed needs.

reddit · r/MachineLearning · /u/Knok0932 · Jun 13, 05:06

**Background**: PaddleOCR is an open-source OCR toolkit by Baidu's PaddlePaddle, supporting over 100 languages. The official Paddle C++ inference runtime has many dependencies, making deployment complex. ncnn is a lightweight inference framework optimized for mobile and embedded systems, offering faster performance and easier integration. This project bridges the gap by providing a C++ implementation that leverages ncnn for efficient OCR inference.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/PaddlePaddle/PaddleOCR">GitHub - PaddlePaddle/PaddleOCR: Turn any PDF or image document into structured data for your AI. A powerful, lightweight OCR toolkit that bridges the gap between images/PDFs and LLMs. Supports 100+ languages. · GitHub</a></li>
<li><a href="https://sourceforge.net/projects/ncnn.mirror/files/20260526/ncnn-20260526-windows-vs2022-shared.zip/download">Download ncnn -20260526-windows-vs2022-shared.zip ( ncnn )</a></li>

</ul>
</details>

**Tags**: `#PaddleOCR`, `#OCR`, `#ncnn`, `#C++`, `#deployment`

---

<a id="item-13"></a>
## [Caddy-Compatible Zeroserve Boosts Performance but Lacks Key Features](https://su3.io/posts/zeroserve-caddy-compat) ⭐️ 6.0/10

Zeroserve, an eBPF-powered web server, has been integrated with Caddy, achieving 3x throughput and 70% lower latency compared to baseline Caddy. While the performance gains are impressive, the missing ACME protocol support and plugin compatibility limit practical deployment, highlighting the trade-off between speed and feature completeness in modern web servers. Zeroserve uses io_uring for async I/O, which raises security concerns according to some resources; additionally, the Caddy compatibility lacks core features like automatic TLS certificate management and many Caddy plugins.

hackernews · losfair · Jun 14, 13:43 · [Discussion](https://news.ycombinator.com/item?id=48527145)

**Background**: Caddy is a popular web server known for its automatic HTTPS via the ACME protocol. Zeroserve is a zero-config, eBPF-scriptable web server designed for high performance using io_uring. io_uring is a Linux kernel interface for asynchronous I/O, offering lower overhead than traditional methods but possibly introducing security risks.

<details><summary>References</summary>
<ul>
<li><a href="https://su3.io/posts/introducing-zeroserve">zeroserve : a zero -config web server you can script with eBPF</a></li>
<li><a href="https://en.wikipedia.org/wiki/Io_uring">Io uring</a></li>
<li><a href="https://en.wikipedia.org/wiki/ACME_protocol">ACME protocol</a></li>

</ul>
</details>

**Discussion**: Comments express mixed reactions: some users are excited about the performance numbers, but several point out the lack of ACME support as a dealbreaker. Security concerns about io_uring and the limited Caddy compatibility (missing plugins) are also raised.

**Tags**: `#performance`, `#web server`, `#Caddy`, `#io_uring`, `#networking`

---

<a id="item-14"></a>
## [Free bilingual ML notebook course seeks feedback](https://www.reddit.com/r/MachineLearning/comments/1u4zbld/im_building_a_free_bilingual_machinelearning/) ⭐️ 6.0/10

A developer released an open-source bilingual (English/Persian) machine learning tutorial repository using Jupyter Notebooks and is asking the community for feedback on its structure, coverage, and practicality. This initiative could lower the barrier for Persian-speaking learners to access high-quality, practical ML education, and the community-driven approach helps ensure the content meets real learning needs. The repository covers ML workflow, data cleaning, regression, classification, tree models, clustering, time series, anomaly detection, responsible ML, and MLOps, with parallel English and Persian notebooks.

reddit · r/MachineLearning · /u/abolfazl1363 · Jun 13, 19:07

**Background**: Jupyter Notebooks are interactive documents widely used for teaching and prototyping machine learning. Bilingual educational resources are rare but valuable for non-native English speakers, as they allow learners to grasp technical concepts in their native language while learning English terminology. MLOps is a set of practices for deploying and maintaining ML models in production, and responsible ML focuses on ethics, fairness, and transparency.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/MLOps">MLOps</a></li>
<li><a href="https://hildeweerts.github.io/responsiblemachinelearning/">An Introduction to Responsible Machine Learning — An Introduction...</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#education`, `#Jupyter notebooks`, `#bilingual`, `#open source`

---

<a id="item-15"></a>
## [Anomaly Detection vs Classification for Cancer Mimics](https://www.reddit.com/r/MachineLearning/comments/1u4obgy/anomaly_detection_vs_classification_for_visually/) ⭐️ 6.0/10

A Reddit user asks whether anomaly detection or supervised classification is better for detecting cancer when negative samples (mimics) are visually and morphologically very similar to the cancer. The question highlights a methodological dilemma in medical machine learning. This question addresses a critical challenge in medical imaging AI: benign mimics can lead to false positives or missed cancers. The choice between anomaly detection and classification affects model performance, robustness, and clinical adoption. The user specifically describes a setting where cancer and mimics are very similar, making it a hard problem for both approaches. The question does not include experimental results; it seeks theoretical and practical advice from the community.

reddit · r/MachineLearning · /u/DryHat3296 · Jun 13, 11:18

**Background**: In cancer diagnosis, "mimics" are benign conditions that appear cancerous on imaging, often requiring advanced tests to differentiate. Anomaly detection treats the target class as in-distribution and everything else as out-of-distribution, while supervised classification explicitly learns decision boundaries between classes. The choice depends on data availability, similarity between classes, and clinical requirements.

<details><summary>References</summary>
<ul>
<li><a href="https://incitefulmed.com/resources/guides/gallbladder-bile-duct-cancer-diagnosis-guide/biliary-cancer-symptoms-mimics/">Biliary Cancer : Symptoms & Warning Signs | Inciteful Med Resources</a></li>
<li><a href="https://stats.stackexchange.com/questions/562650/imbalanced-classification-vs-anomaly-detection/592677">machine learning - Imbalanced classification vs anomaly detection ...</a></li>

</ul>
</details>

**Tags**: `#anomaly detection`, `#classification`, `#medical imaging`, `#machine learning`

---

<a id="item-16"></a>
## [MDP Derivative-Free Optimizer Beats Adam on MNIST](https://www.reddit.com/r/MachineLearning/comments/1u4fc16/derivativefree_neural_network_optimization_mnist/) ⭐️ 6.0/10

A derivative-free optimization method called MDP achieved 93.4% test accuracy on MNIST with a small 784-32-10 neural network, outperforming Adam's 91.7% without using gradients. This result shows that derivative-free optimization can be competitive with gradient-based methods for certain neural network tasks, potentially offering an alternative when gradients are unavailable or expensive to compute. The optimization used 1,000,000 function evaluations over a 25,450-dimensional parameter space, directly minimizing cross-entropy loss on 5,000 training images. MDP achieved a final loss of 0.0004083 and validation accuracy of 93.7%, while Adam reached 0.002945 loss and 91.8% validation accuracy.

reddit · r/MachineLearning · /u/Mis4318 · Jun 13, 02:51

**Background**: Derivative-free optimization (DFO) methods optimize objective functions without using gradient information, relying only on function evaluations. They are useful when gradients are unavailable, noisy, or expensive, but often struggle with high-dimensional problems. This work shows DFO can scale to over 25,000 parameters on a simple neural network task.

<details><summary>References</summary>
<ul>
<li><a href="https://www.academia.edu/145050332/Two_derivative_free_optimization_algorithms_for_mesh_quality_improvement">(PDF) Two derivative - free optimization algorithms for mesh quality...</a></li>
<li><a href="https://vdoc.pub/documents/introduction-to-derivative-free-optimization-22tajmri9rtg">Introduction To Derivative - free Optimization [PDF] [22tajmri9rtg]</a></li>
<li><a href="https://optimization-online.org/wp-content/uploads/2026/01/Riemannian_optimization_with_finite-difference_gradient.pdf">Riemannian optimization with finite-difference gradient</a></li>

</ul>
</details>

**Tags**: `#derivative-free optimization`, `#neural networks`, `#MNIST`, `#optimization`, `#MDP`

---