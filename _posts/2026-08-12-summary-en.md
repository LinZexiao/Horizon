---
layout: default
title: "Horizon Summary: 2026-08-12 (EN)"
date: 2026-08-12
lang: en
---

> From 38 items, 22 important content pieces were selected

---

1. [Qwen Releases 2.4T-Parameter MoE Model Qwen3.8-2.4T-A95B](#item-1) ⭐️ 9.0/10
2. [Meta unveils Muse Glimmer, an Apache 2.0 open-weights 30B agentic model](#item-2) ⭐️ 9.0/10
3. [DeepSeek V4 Pro 0813 Launches with Cost-Efficient Coding Performance](#item-3) ⭐️ 8.0/10
4. [Tailscale Traces Database Corruption to 16-Year-Old SQLite WAL-Reset Bug](#item-4) ⭐️ 8.0/10
5. [HTML over WebSockets: Real-Time SPAs With Minimal JavaScript](#item-5) ⭐️ 8.0/10
6. [xAI Unveils Grok 4.6 Frontier Model](#item-6) ⭐️ 8.0/10
7. [Chrome's Downscaling Algorithm Makes Tiny JPEGs Render Differently](#item-7) ⭐️ 8.0/10
8. [uBlock Origin Stops Blocking Facebook Ads Amid Obfuscation Arms Race](#item-8) ⭐️ 8.0/10
9. [Attack Recovers Hidden Chain-of-Thought from Top LLM APIs](#item-9) ⭐️ 8.0/10
10. [Adam's basis dependence destroys GD's implicit low-rank bias](#item-10) ⭐️ 8.0/10
11. [Decoupled Descent: Enforcing Train-Test Error Alignment via AMP Onsager Corrections](#item-11) ⭐️ 8.0/10
12. [Zed unveils DeltaDB, a chat-like version control system for AI collaboration.](#item-12) ⭐️ 7.0/10
13. [Quoting Florian Herrengt](#item-13) ⭐️ 7.0/10
14. [No Lossless Transformations of Natural-Language Text](#item-14) ⭐️ 7.0/10
15. [Site ranks CS conferences by destination quality, not prestige](#item-15) ⭐️ 7.0/10
16. [Hastily-Built Webcam Site Draws Community for 2026 Eclipse](#item-16) ⭐️ 6.0/10
17. [Tim King, AmigaDOS Developer, Passes Away](#item-17) ⭐️ 6.0/10
18. [Mass scans spoof AI bots like ClaudeBot](#item-18) ⭐️ 6.0/10
19. [YC P26 startup launches AI agents for semiconductor materials discovery](#item-19) ⭐️ 6.0/10
20. [Datasette Upload DBS 0.5a0 Adds Formalized API for Database Uploads](#item-20) ⭐️ 6.0/10
21. [AAAI 2027 Reviewers Flag Missing Code in Submissions](#item-21) ⭐️ 6.0/10
22. [Seeking RL/Planning Pointers for Stochastic Merge Puzzle with Afterstates](#item-22) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Qwen Releases 2.4T-Parameter MoE Model Qwen3.8-2.4T-A95B](https://huggingface.co/Qwen/Qwen3.8-2.4T-A95B) ⭐️ 9.0/10

Qwen released Qwen3.8-2.4T-A95B, a Mixture-of-Experts model with 2.4 trillion total parameters and 95 billion active parameters, along with BF16 and FP8 checkpoints. The model reaches near-frontier performance, with quantized versions reportedly fitting on high-end consumer hardware. This is one of the largest open-weights MoE models ever released, signaling that frontier-scale models are becoming available for local deployment and research. With practical quantized options, it could shift expectations for what individuals and smaller labs can run at home. The BF16 version requires about 4.9TB of storage, while an unsloth 1-bit quantization reduces it to roughly 397GB. The open-weights release lacks vision input, non-thinking support, and the 1M context length found in the official Qwen3.8-Max version.

hackernews · Philpax · Aug 12, 15:01 · [Discussion](https://news.ycombinator.com/item?id=49273478)

**Background**: Mixture-of-Experts (MoE) is an architecture that divides computation across specialized subnetworks, or 'experts,' activating only a subset per token to save compute. Total parameters determine storage footprint, while active parameters determine inference speed and cost. Quantization techniques like FP8 and INT4 reduce memory requirements by storing weights at lower precision, often with minimal accuracy loss. These approaches enable massive models to run on more accessible hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/applying-mixture-of-experts-in-llm-architectures/">Applying Mixture of Experts in LLM Architectures | NVIDIA Technical Blog</a></li>
<li><a href="https://rcrtech.com/semiconductor-news/llms-quantization-fp8-fp4-int8/">LLMs and quantization: FP8, FP4, and INT8 explained</a></li>
<li><a href="https://spanvero.com/learn/active-vs-total-params/">Active vs total parameters — what it means (open AI models)...</a></li>

</ul>
</details>

**Discussion**: Commenters noted that the BF16/FP8-only launch makes the model harder to serve than rivals like Kimi k3, and that 4-bit quantization without QAT will require external calibration data. Some were impressed that 1-bit quant versions can bring Opus 4.5-level performance to around 397GB, while others pointed out missing vision and context-length features. A few also referenced DeepSeek V4-Pro benchmark announcements, putting the release in a competitive context.

**Tags**: `#AI`, `#LLM`, `#Qwen`, `#MoE`, `#Open Weights`

---

<a id="item-2"></a>
## [Meta unveils Muse Glimmer, an Apache 2.0 open-weights 30B agentic model](https://simonwillison.net/2026/Aug/10/introducing-muse-glimmer/) ⭐️ 9.0/10

Meta has introduced Muse Glimmer, a 30B-parameter open-weights model released under the permissive Apache 2.0 license. The model is explicitly optimized for end-to-end agentic tasks, reliable tool use, and multi-step reasoning, and is also capable of vision tasks. Muse Glimmer stands out because it uses a clean Apache 2.0 license, a step up from Meta's previous custom Llama licenses, making it freely usable for commercial and research purposes. Its strong agentic and tool-use performance in a locally runnable 30B size is highly relevant to practitioners building autonomous AI agents. Muse Glimmer is a vision-capable multimodal model; Simon Willison tested an 18.16GB quantized version via LM Studio and found it works well for image description and code exploration with the llm-coding-agent plugin. Meta claims strong results on hard agentic benchmarks including DeepSearch QA, MCP-Atlas, τ-Bench, and SWE-Bench.

rss · Simon Willison · Aug 10, 23:56

**Background**: Agentic AI refers to systems that can autonomously plan and execute multi-step tasks, often by calling external tools. Open-weights models allow users to download and fine-tune the model freely, unlike closed APIs. Benchmarks like SWE-Bench test a model's ability to resolve real GitHub issues, MCP-Atlas evaluates tool-use competency with real MCP servers, and τ-Bench simulates dynamic user-agent conversations. Muse Glimmer is designed to excel at exactly these kinds of real-world agent deployments.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/scaleapi/mcp-atlas">GitHub - scaleapi/mcp-atlas: MCP Atlas</a></li>
<li><a href="https://github.com/sierra-research/tau-bench">GitHub - sierra-research/tau-bench: Code and Data for Tau-Bench · GitHub</a></li>
<li><a href="https://github.com/swe-bench/SWE-bench">GitHub - SWE-bench/SWE-bench: SWE-bench: Can Language Models ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Machine Learning`, `#Open Weights`, `#Agentic AI`, `#Meta`

---

<a id="item-3"></a>
## [DeepSeek V4 Pro 0813 Launches with Cost-Efficient Coding Performance](https://openrouter.ai/deepseek/deepseek-v4-pro-0813) ⭐️ 8.0/10

DeepSeek released the production version of its flagship model, DeepSeek V4 Pro 0813, as a general-availability build on OpenRouter and its own API on August 12, 2026. Early user tests indicate it handles coding tasks at a fraction of the cost of rival models. V4 Pro 0813's strong cost-performance tradeoff for coding could pressure more expensive rivals like Grok and GPT. As an open-weight DeepSeek model, it continues the trend of low-cost, efficient AI that disrupted the industry. V4 Pro 0813 ended a preview period that ran nearly four months and serves as the general-availability release of the V4 Pro flagship. In one community test on Codex CLI, DeepSeek completed a feature in 12 minutes at $0.12 but with a bug, while Grok 4.6 took 3 minutes at $1.41 without a bug.

hackernews · explosion-s · Aug 12, 16:04 · [Discussion](https://news.ycombinator.com/item?id=49274600)

**Background**: DeepSeek is a Chinese AI company whose R1 model, released in January 2025, became a global phenomenon and sparked debate over the efficiency of large language models. The V4 family includes V4 Flash, a lighter and cheaper model, and the V4 Pro flagship, which offers a higher-effort 'Pro-Max' reasoning mode. Community results suggest that DeepSeek's cost advantage sometimes comes with tradeoffs in correctness or reliability.

<details><summary>References</summary>
<ul>
<li><a href="https://www.unite.ai/deepseek-ships-v4-pro-as-its-flagship-model-leaves-preview/">DeepSeek Ships V4 Pro as Its Flagship Model Leaves Preview</a></li>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>
<li><a href="https://api-docs.deepseek.com/news/news260424/">DeepSeek V 4 Preview Release | DeepSeek API Docs</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some question why the post links to OpenRouter instead of official APIs, while hands-on coding tests show DeepSeek is dramatically cheaper but buggier than Grok 4.6 and GPT-5.6-terra-high. Others praise the recent V4 Flash update, saying it 'amazes' them by handling heavy development for very little money.

**Tags**: `#deepseek`, `#llm`, `#model-release`, `#coding`, `#ai`

---

<a id="item-4"></a>
## [Tailscale Traces Database Corruption to 16-Year-Old SQLite WAL-Reset Bug](https://tailscale.com/blog/sqlite-wal-reset-bug) ⭐️ 8.0/10

Tailscale publicly documented that a 16-year-old data race in SQLite's write-ahead log (WAL) reset/checkpointing code caused months of database corruption and control-plane outages. The bug was fixed in SQLite 3.51.3 after Tailscale funded the development of an open-source SQLite VFS shim to help isolate the race condition. The bug affected a single-writer SQLite configuration that many production systems rely on, undermining common assumptions about SQLite's reliability. It also highlights a sustainable open-source funding model, where a company pays for targeted debugging tooling and collaborates with upstream maintainers. Despite SQLite's recommended single-writer WAL usage, the corruption occurred due to a race between WAL reset and checkpoint operations. A first fix was rolled out and then rolled back because it broke something else; SQLite 3.51.3 was considered the real fix after two more months of observation.

hackernews · ropbear · Aug 12, 14:22 · [Discussion](https://news.ycombinator.com/item?id=49272832)

**Background**: SQLite uses write-ahead logging (WAL) as an alternative to rollback journal mode: changes are appended to a temporary WAL file, and a checkpoint later merges them into the main database. A successful checkpoint resets the WAL, and a race in that reset logic could corrupt the database. SQLite is a widely embedded C library with an enormous test suite, yet this bug survived for 16 years. Tailscale worked with the SQLite team through a commercial support contract to track it down.

<details><summary>References</summary>
<ul>
<li><a href="https://tailscale.com/blog/sqlite-wal-reset-bug">How Tailscale helped find the SQLite WAL-Reset bug</a></li>
<li><a href="https://antithesis.com/blog/2026/wal-reset-bug/">Breaking the WAL | Antithesis</a></li>

</ul>
</details>

**Discussion**: Commenters largely praised the write-up and the transparent debugging story. Several highlighted the value of funding open-source debugging tooling and SQLite's support contract, while others quoted Dijkstra to note that even huge test suites cannot prove the absence of bugs.

**Tags**: `#sqlite`, `#reliability`, `#debugging`, `#open-source`, `#tailscale`

---

<a id="item-5"></a>
## [HTML over WebSockets: Real-Time SPAs With Minimal JavaScript](https://en.andros.dev/blog/ef4968f5/html-over-websockets-real-time-spas-with-barely-any-javascript/) ⭐️ 8.0/10

An article proposes building real-time single-page applications by streaming server-rendered HTML over WebSockets, dramatically reducing client-side JavaScript. It credits Phoenix LiveView as the originator of this technique and has sparked a lively debate about when WebSockets are appropriate versus Server-Sent Events. This approach challenges the dominant client-side JavaScript framework model for SPAs, potentially simplifying development, deployment, and security. The discussion also clarifies the practical tradeoffs between WebSockets and SSE, influencing how developers choose real-time communication for their applications. The article claims that because the server renders and escapes HTML before sending it, the architecture is safer against XSS — a point commenters strongly dispute. Additional context includes that Phoenix LiveView actually transmits minimal diffs over WebSockets after the initial render, and that SSE is a simpler, cheaper option when only server-to-client push is needed.

hackernews · redbell · Aug 12, 16:51 · [Discussion](https://news.ycombinator.com/item?id=49275335)

**Background**: Phoenix LiveView is a server-centric real-time web framework built on the Elixir and Phoenix stack; it renders HTML on the server and updates the client over a persistent WebSocket connection. Server-Sent Events (SSE) is a standard server push technology that works over plain HTTP, while WebSockets provide full-duplex bidirectional communication. The core architectural question is whether real-time apps need bidirectional low-latency messaging or simply server-initiated updates to the page.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/phoenixframework/phoenix_live_view">GitHub - phoenixframework/phoenix_live_view: Rich, real-time ... Phoenix Framework LiveView — Phoenix v1.8.9 Phoenix LiveView 1.0.0 is here! - Phoenix Blog Welcome — Phoenix LiveView v1.2.9 - HexDocs Phoenix LiveView Tutorial: Getting Started - daily.dev</a></li>
<li><a href="https://en.wikipedia.org/wiki/Server-sent_events">Server-sent events - Wikipedia</a></li>
<li><a href="https://phoenix-live-view.hexdocs.pm/Phoenix.LiveView.html">Phoenix.LiveView — Phoenix LiveView v1.2.9 - HexDocs</a></li>

</ul>
</details>

**Discussion**: Commenters noted that Chris McCord originally experimented with this idea in Rails (the Sync gem) before moving to Phoenix and building LiveView. Others argued that SSE is simpler and cheaper for most server-push scenarios, reserving WebSockets for bidirectional use cases like chat or collaboration, while one commenter disagreed strongly with the article's XSS safety claim, saying the reverse is often true in practice.

**Tags**: `#WebSockets`, `#Real-time`, `#SPA`, `#SSE`, `#JavaScript`

---

<a id="item-6"></a>
## [xAI Unveils Grok 4.6 Frontier Model](https://x.ai/news/grok-4-6) ⭐️ 8.0/10

xAI has announced Grok 4.6, its latest frontier large language model, drawing significant discussion on Hacker News. The release comes amid intense competition among AI labs. Grok 4.6's release intensifies competition among frontier AI providers, potentially influencing model pricing and capability benchmarks. The Hacker News discussion also raises important questions about API behavior and the validity of model benchmarks. Community reports indicate the xAI API adds a default system prompt that can override user-supplied instructions, causing the model to refuse discussions about its own guidelines. Some commenters also speculate about benchmark manipulation and compare Grok's subscription allowances with those of OpenAI and Anthropic.

hackernews · iLuddite · Aug 12, 15:32 · [Discussion](https://news.ycombinator.com/item?id=49274027)

**Background**: Grok is a series of large language models developed by xAI, Elon Musk's AI company, and is available through grok.com and the xAI API. The API gives developers access to frontier models with reasoning, vision, and tool-use capabilities. This release builds on earlier Grok versions and competes directly with models from OpenAI, Anthropic, and other labs.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Grok_(chatbot)">Grok (chatbot) - Wikipedia</a></li>
<li><a href="https://x.ai/api">API: Frontier Models for Reasoning & Enterprise | SpaceXAI</a></li>
<li><a href="https://grok.com/">Grok</a></li>

</ul>
</details>

**Discussion**: The Hacker News community is divided: some praise Grok as healthy competition, while others refuse to support Elon Musk's ventures. Key concerns include API prompt injection, suspected benchmark gaming, and whether subscription allowances are generous enough.

**Tags**: `#AI`, `#Grok`, `#xAI`, `#LLM`, `#model release`

---

<a id="item-7"></a>
## [Chrome's Downscaling Algorithm Makes Tiny JPEGs Render Differently](https://guillaumetech.github.io/posts/jpg-scaling-chrome/) ⭐️ 8.0/10

The article explains that Chrome renders tiny JPEGs differently because its downscaling algorithm uses low-resolution linear interpolation optimized for speed, producing a slight right bias and blurrier edges than other browsers. It concludes that JPEGs should not be used for icons, recommending formats like PNG or SVG instead. This matters for web developers and browser engineers because it exposes a non-obvious cross-browser rendering difference that can degrade UI quality, and it reinforces best practices for image formats and resolution. Understanding browser-specific scaling algorithms helps developers make informed choices and avoid subtle visual bugs in production. Chrome's downscaling behavior is most noticeable when scaling images down by a tiny amount, and it uses linear interpolation even for very slight downscales. The issue also affected Electron applications because they inherit Chrome's rendering engine, and community members noted that PNGs can show similar artifacts when downscaled from oversized resolutions.

hackernews · gutechh · Aug 12, 14:00 · [Discussion](https://news.ycombinator.com/item?id=49272549)

**Background**: JPEG is a lossy image format that uses discrete cosine transform (DCT) compression, which discards data to reduce file size and can introduce compression artifacts such as blockiness and ringing, especially at high compression levels. Browsers use different image scaling algorithms when resizing images: Chrome uses low-resolution linear interpolation optimized for speed, while Firefox uses a sharper algorithm with slightly more ringing. The CSS property 'image-rendering' can influence which algorithm is used, giving developers some control over the tradeoff between blur and sharpness.

<details><summary>References</summary>
<ul>
<li><a href="https://entropymine.com/resamplescope/notes/browsers/">How web browsers resize images</a></li>
<li><a href="https://stackoverflow.com/questions/37906602/blurry-downscaled-images-in-chrome">html - Blurry downscaled images in Chrome - Stack Overflow</a></li>
<li><a href="https://gehrcke.de/2014/11/css-crispy-downscaled-images/">CSS: Crispy downscaled images – Jan-Philip Gehrcke, PhD</a></li>
<li><a href="https://en.wikipedia.org/wiki/JPEG_artifacts">JPEG artifacts</a></li>

</ul>
</details>

**Discussion**: Community comments largely agree with the article's warning against JPEG for icons, with jonathanlydall noting that the issue also affects PNGs and had previously broken icons in an Electron app, causing a delayed upgrade. advisedwang stressed using appropriately sized images and avoiding huge images for small displays, while debazel and gwittel discussed differences between Chrome and Firefox scaling algorithms and suggested the 'image-rendering' CSS attribute as a workaround. muizelaar also pointed to a Firefox bug for lower-scale decompression work.

**Tags**: `#JPEG`, `#Chrome`, `#image scaling`, `#web development`, `#browser rendering`

---

<a id="item-8"></a>
## [uBlock Origin Stops Blocking Facebook Ads Amid Obfuscation Arms Race](https://digitalescapetools.com/2026/08/ublock-origin-stops-chasing-facebook-ads.html) ⭐️ 8.0/10

uBlock Origin, the popular open-source ad blocker, has announced it will no longer attempt to filter ads on Facebook, conceding that Facebook's obfuscation tactics make the cat-and-mouse game unwinnable. The news surfaced via a Reddit post and was reported by Neowin. This marks a significant concession in the ad-blocking arms race, showing how a major platform's anti-blocking measures can effectively defeat a widely-used blocker. It affects millions of uBlock Origin users who use Facebook, and sparks broader debate about ad-blocking efficacy, privacy, and platform control. Facebook reportedly uses obfuscated and frequently changing code to hide ads from filter lists, making it impractical for uBlock Origin to keep up. The decision does not affect ad blocking on other sites, and the extension remains one of the most popular content filters, with tens of millions of users on Chrome and Firefox.

hackernews · Markoff · Aug 12, 11:28 · [Discussion](https://news.ycombinator.com/item?id=49270726)

**Background**: uBlock Origin is a free and open-source browser extension for content filtering, including ad blocking, developed by Raymond Hill and available on Firefox and Chromium-based browsers. Facebook's business model relies heavily on advertising, so the company invests in anti-ad-blocking measures that disguise ad delivery through obfuscation. The ongoing conflict between ad blockers and platforms like Facebook has become a technical arms race, with each side trying to outsmart the other.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/UBlock_Origin">UBlock Origin</a></li>
<li><a href="https://www.humansecurity.com/learn/blog/unmasking-malvertising-how-obfuscation-creates-false-safety-and-how-to-defeat-it/">Unmasking malvertising: How obfuscation creates... - HUMAN Security</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some users agree that giving up on Facebook ads is the right call, while others predict the next phase will involve AI or computer vision that visually recognizes ads. Several commenters reflect on the futility of the cat-and-mouse game, and some question why Facebook invests effort in bypassing blockers when ad-blocking users are unlikely to engage with ads.

**Tags**: `#ad-blocking`, `#privacy`, `#facebook`, `#ublock-origin`, `#arms-race`

---

<a id="item-9"></a>
## [Attack Recovers Hidden Chain-of-Thought from Top LLM APIs](https://simonwillison.net/2026/Aug/11/stealing-reasoning-traces/) ⭐️ 8.0/10

A new paper demonstrates that encrypted chain-of-thought blocks returned by Anthropic, OpenAI, and Google LLM APIs can be replayed into weaker sibling models and jailbroken to recover the original private reasoning in plaintext. All providers acknowledged the report and have since fixed the vulnerability. Hidden reasoning traces are considered sensitive intellectual property in proprietary LLM APIs, so a practical attack that reveals them undermines the privacy and security assumptions of these services. It will likely push API designers toward per-request encryption keys or stronger isolation between model tiers. The attack worked because models within the same family shared the same encryption key, allowing encrypted traces to be replayed across sessions, users, and models. Claude Haiku 4.5 was the easiest target, using a transcription prompt plus an assistant turn prefix of <thinking-copy>; the paper also shows recovered GPT-5.5 reasoning about CSS.

rss · Simon Willison · Aug 11, 22:40

**Background**: Chain-of-thought (CoT) reasoning refers to LLMs generating intermediate reasoning steps before producing a final answer, and it substantially improves performance on complex tasks. Many proprietary API providers now encrypt or hide CoT traces to protect model internals and safety details, but this paper shows the encryption can be bypassed by replaying blocks into a weaker sibling model from the same family and jailbreaking it.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2201.11903">[2201.11903] Chain-of-Thought Prompting Elicits Reasoning in Large Language Models</a></li>
<li><a href="https://www.ibm.com/think/topics/chain-of-thoughts">What is chain of thought (CoT) prompting? | IBM</a></li>

</ul>
</details>

**Tags**: `#AI security`, `#LLM`, `#chain-of-thought`, `#privacy`, `#API vulnerability`

---

<a id="item-10"></a>
## [Adam's basis dependence destroys GD's implicit low-rank bias](https://www.reddit.com/r/MachineLearning/comments/1vmjb3p/the_loss_does_not_see_the_basis_but_adam_does_r/) ⭐️ 8.0/10

A Reddit post demonstrates that Adam's per-coordinate second-moment normalization breaks rotation invariance and destroys gradient descent's implicit low-rank bias in underdetermined matrix sensing, while rotation-invariant optimizers like Muon and Shampoo preserve it. The author ran nine update rules at matched training loss and found two clean clusters of behavior. This identifies a specific mechanism—per-coordinate second-moment basis dependence—that explains why Adam can underperform on low-rank structured problems, a finding directly relevant to optimizer design and ML optimization research. It also reframes debates about Muon's spectral simplicity bias by showing both behaviors on the same axis. A one-parameter family interpolating between per-coordinate and shared-scalar denominators shows recovery improves monotonically, pinning the damage on anisotropy rather than adaptivity in general. The author also found that switching their own optimizer from per-coordinate clipping to a global norm clip improved recovery error from 0.347 to 0.220; a caveat notes that the reported hyperspectral gain uses a train-only learning rate rule that gives Adam the worst rate on its grid.

reddit · r/MachineLearning · /u/EtherealGlyph · Aug 12, 16:39

**Background**: In a factored model W = UV^T, the loss is invariant to rotations (U,V) → (UQ, VQ), and gradient descent respects this symmetry. Adam's per-coordinate second moment does not, because it depends on the basis in which the factors are written, thereby breaking the symmetry and destroying the implicit low-rank bias that helps GD find simpler solutions. Rotation-invariant optimizers such as Muon and Shampoo use preconditioning that respects the matrix structure, preserving this bias.

<details><summary>References</summary>
<ul>
<li><a href="https://kellerjordan.github.io/posts/muon/">Muon: An optimizer for hidden layers in neural networks | Keller Jordan blog</a></li>
<li><a href="https://arxiv.org/abs/1802.09568">[1802.09568] Shampoo: Preconditioned Stochastic Tensor ... optimizers/distributed_shampoo/README.md at main ... - GitHub Ashampoo® WinOptimizer Pro 29 - Optimize, clean, and protect ... SOAP: Improving and Stabilizing Shampoo using Adam GitHub - Daniil-Selikhanovych/Shampoo_optimizer: Our ... Shampoo: Preconditioned Stochastic Tensor Optimization</a></li>
<li><a href="https://github.com/facebookresearch/optimizers/blob/main/distributed_shampoo/README.md">optimizers/distributed_shampoo/README.md at main ... - GitHub</a></li>

</ul>
</details>

**Tags**: `#machine-learning`, `#optimizers`, `#adam`, `#low-rank-bias`, `#matrix-sensing`

---

<a id="item-11"></a>
## [Decoupled Descent: Enforcing Train-Test Error Alignment via AMP Onsager Corrections](https://www.reddit.com/r/MachineLearning/comments/1vlu1se/decoupled_descent_enforcing_exact_traintest_error/) ⭐️ 8.0/10

The author presents Decoupled Descent (DD), a novel training algorithm that leverages approximate message passing (AMP) Onsager corrections to guarantee that training error asymptotically equals test error at every parameter iterate, demonstrated on full-batch gradient descent for Gaussian mixture models. This work offers a fresh theoretical lens on overfitting, showing that the train-test gap can be provably eliminated during optimization rather than merely controlled. If extended beyond stylized models, it could enable certifiable generalization, principled optimal stopping, and safer hyperparameter tuning in deep learning. Decoupled Descent is currently a theoretical method applied to full-batch gradient descent on Gaussian mixture models; experiments on a high-dimensional XOR model with a two-layer network show that DD tracks test error closely while GD overfits. The author stresses this is a first step and plans to release a PyTorch-compatible implementation.

reddit · r/MachineLearning · /u/mlovik1 · Aug 11, 21:06

**Background**: In supervised learning, gradient descent minimizes training loss, but test performance often lags—a phenomenon called overfitting. Approximate message passing (AMP) is an iterative algorithm from compressed sensing and statistical physics that, for random matrices, obeys a precise state-evolution recursion; its Onsager correction term cancels correlations that accumulate across iterations. Decoupled Descent borrows these ideas to decouple optimization dynamics from data reuse bias, making the train-test gap asymptotically visible at each iterate.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2201.07487">A Concise Tutorial on Approximate Message Passing A unifying tutorial on Approximate Message Passing Lecture 19: Approximate message passing algorithms Approximate Message Passing Tutorial - GitHub Pages Message-passing algorithms for compressed sensing GitHub - shx-lyu/AMP-in-MIMO: Approximate message passing ... A unifying tutorial on Approximate Message Passing</a></li>
<li><a href="https://arxiv.org/abs/2008.11892">[2008.11892] Approximate Message Passing algorithms for rotationally ...</a></li>
<li><a href="https://www.bohrium.com/en/sciencepedia/feynman/compressed_sensing_and_sparse_optimization_graduate-approximate_message_passing_algorithm">approximate message passing algorithm | Bohrium</a></li>

</ul>
</details>

**Tags**: `#Machine Learning`, `#Optimization`, `#Approximate Message Passing`, `#Generalization`, `#Theory`

---

<a id="item-12"></a>
## [Zed unveils DeltaDB, a chat-like version control system for AI collaboration.](https://zed.dev/blog/introducing-delta) ⭐️ 7.0/10

Zed announced DeltaDB (also referred to as Delta), an operation-level version control system that records every change between commits and links them to a chat-like collaborative workspace. The announcement came via Zed's blog post 'Introducing Delta,' positioning the tool as version control built for software made between commits. As AI agents increasingly generate code outside traditional commit boundaries, existing version control hides the reasoning behind changes. DeltaDB aims to preserve every operational detail and decision, which could make AI and human collaboration more transparent and auditable. Unlike Git, which only stores committed snapshots, DeltaDB assigns a stable ID to every operation and records the full stream of edits between commits. The feature is built by Zed Industries, the maker of the Rust-based, GPU-accelerated Zed editor, and includes a chat-like interface for tracking decisions.

hackernews · khy · Aug 12, 18:19 · [Discussion](https://news.ycombinator.com/item?id=49276574)

**Background**: Zed is an open-source, high-performance code editor written in Rust, designed for speed and real-time collaboration with humans and AI agents. Traditional version control like Git only captures the snapshots developers choose to commit, so the intermediate steps and AI conversations behind a change are usually lost. DeltaDB addresses this gap by recording every operation and linking insights to code, aiming to turn the IDE into a collaborative workspace across time scales.

<details><summary>References</summary>
<ul>
<li><a href="https://zed.dev/blog/introducing-deltadb">Software Is Made Between Commits — Zed's Blog</a></li>
<li><a href="https://shapeof.com/archives/2025/8/deltadb_from_zed.html">DeltaDB From Zed (the Code Editor) - shapeof.com</a></li>
<li><a href="https://sesamedisk.com/what-is-zed-deltadb-features/">What Is Zed DeltaDB and Its Key Features - Sesame Disk</a></li>

</ul>
</details>

**Discussion**: Community reactions were mixed. Some commenters questioned the chat-like design, saying it combines the worst of Google Docs and Slack and won't help track decisions, while others argued multi-player coding in an editor has no practical use. There were also complaints about difficult-to-read low-contrast text and skepticism about verbose AI summaries of code, though some found the real-time collaboration concept intriguing.

**Tags**: `#Zed`, `#collaboration`, `#code editor`, `#AI`, `#real-time editing`

---

<a id="item-13"></a>
## [Quoting Florian Herrengt](https://simonwillison.net/2026/Aug/12/florian-herrengt/) ⭐️ 7.0/10

A quote highlights how AI-generated code can lead to convoluted projects where no one understands the system, posing risks to software maintainability.

rss · Simon Willison · Aug 12, 15:08

**Tags**: `#AI-assisted development`, `#software engineering`, `#code maintainability`, `#developer productivity`, `#commentary`

---

<a id="item-14"></a>
## [No Lossless Transformations of Natural-Language Text](https://simonwillison.net/2026/Aug/11/there-are-no-lossless-transformations-of-natural-language-text/) ⭐️ 7.0/10

Sophie Alpert published an internal policy for engineers' acceptable use of AI writing, arguing that every rewrite or rephrase of natural-language text is lossy. Simon Willison highlighted the post, emphasizing the rule that engineers must stand behind every idea and every sentence in their documentation. This provides practical, high-value guidance for responsible LLM use in technical writing, a timely issue as more teams adopt AI assistants. It gives engineers and technical writers a clear standard for when AI-generated prose is acceptable. The central rule is that if a reviewer asks "What did you mean by this line?", replying "AI wrote that, just ignore it" is unacceptable. The post argues that an entity without the author's detailed mental representation of intent will lose information in any rewrite, so authors must verify the final text reflects their own thoughts.

rss · Simon Willison · Aug 11, 23:48

**Background**: In computing, a "lossless" transformation preserves all original data, such as lossless compression algorithms that allow exact reconstruction. Natural language, however, is not a fixed data representation: the meaning of a sentence depends on the author's intent and context. Large language models can fluently paraphrase or rewrite text, but unless they share the writer's full mental model, subtle meaning can be lost. This is why AI-powered "polishing" of documentation carries real risk if not carefully reviewed.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Lossless_compression">Lossless compression - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Natural_language_processing">Natural language processing - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI writing`, `#technical documentation`, `#LLM usage`, `#engineering culture`

---

<a id="item-15"></a>
## [Site ranks CS conferences by destination quality, not prestige](https://www.reddit.com/r/MachineLearning/comments/1vmbdk6/i_built_an_honest_cs_conference_ranking_sorted_by/) ⭐️ 7.0/10

A new website, honestcsrankings.org, ranks approximately 540 CORE-ranked computer science conferences by the quality of their destination — factoring in weather, safety, cost, accessibility, and city vibe. It also provides filtering, distance-based sorting, calendar export, and deep links for coauthors. This tool reframes conference selection around travel experience rather than academic prestige, potentially influencing attendance decisions and conference planning. It gives researchers a practical way to weigh career value against destination appeal. The site uses the Global Peace Index for safety, World Bank price levels for cost, and real climate data for the actual conference month. It includes an 'Upsets' tab showing A* venues in poor destinations, and it misses ICML/ICLR 2027 and COLM because they are not yet announced or not CORE-ranked.

reddit · r/MachineLearning · /u/JohnAZoidberg77 · Aug 12, 11:23

**Background**: The CORE conference ranking is a widely recognized rating system that assesses the academic quality of computer science conferences. The Global Peace Index is an annual report by the Institute for Economics & Peace that measures the relative peacefulness of nations. WikiCFP is a community-maintained call-for-papers resource that the site scrapes to include smaller conferences. By combining these sources, the tool creates a travel-oriented alternative to prestige-based rankings.

<details><summary>References</summary>
<ul>
<li><a href="https://portal.core.edu.au/conf-ranks/">portal. core .edu.au/conf- ranks</a></li>
<li><a href="https://en.wikipedia.org/wiki/Global_Peace_Index">Global Peace Index</a></li>
<li><a href="http://www.wikicfp.com/cfp/servlet/event.showcfp?eventid=63368©ownerid=96880">WikiCFP : Call For Papers of Conferences, Workshops and Journals</a></li>

</ul>
</details>

**Tags**: `#academic conferences`, `#tools`, `#CS research`, `#travel`, `#ranking`

---

<a id="item-16"></a>
## [Hastily-Built Webcam Site Draws Community for 2026 Eclipse](https://jonty.github.io/2026_eclipse_webcams/) ⭐️ 6.0/10

The creator of a webcam aggregation site for the 2026 eclipse shared it with the community, having built it quickly and launched it just before totality began. The site aggregates live webcams across Iceland and Spain for real-time viewing. This real-time web project turns a niche tool into a shared communal experience, letting people around the world watch a rare eclipse remotely. It highlights how personal web projects can foster strong community engagement and collective observation of natural events. The site is hosted at jonty.github.io/2026_eclipse_webcams, and the creator built a similar version for the 2024 US eclipse, finishing minutes before totality. The creator noted that coordinating cameras across Iceland and Spain was unexpected, and expressed hope the site would not break during the event.

hackernews · zoenolan · Aug 12, 11:53 · [Discussion](https://news.ycombinator.com/item?id=49270953)

**Background**: A solar eclipse occurs when the Moon passes between the Sun and Earth, temporarily darkening the sky in a narrow path. Webcam aggregation sites collect live streams from multiple locations so viewers can experience totality remotely. The creator previously built a similar tool for the 2024 North American eclipse, which served as a basis for this 2026 version.

**Discussion**: Community members shared personal eclipse stories, including traveling long distances to escape clouds and observing pink plasma prominences with binoculars. One commenter cited the first correct eclipse prediction by Thales of Miletus, calling it the 'birth of science.' Overall sentiment was positive and appreciative, with some adding further resources like solar panel monitoring data.

**Tags**: `#eclipse`, `#webcams`, `#community`, `#real-time`, `#space`

---

<a id="item-17"></a>
## [Tim King, AmigaDOS Developer, Passes Away](https://amiga-news.de/en/news/AN-2026-08-00070-EN.html) ⭐️ 6.0/10

Tim King, one of the developers of AmigaDOS, has died, as announced in an obituary published on amiga-news.de. Community members are sharing memories and expressing appreciation for his contributions. Tim King helped create AmigaDOS, a key component of the Amiga operating system that defined the 16-bit home computer era. His work influenced a generation of users and developers, and the retrocomputing community is honoring his legacy. AmigaDOS is the disk operating system of AmigaOS, originally based on a TRIPOS port by MetaComCo and written in BCPL for AmigaOS 1.x. It was later rewritten in C starting from AmigaOS 2.x, and BCPL compatibility was dropped in AmigaOS 4.

hackernews · doener · Aug 12, 14:09 · [Discussion](https://news.ycombinator.com/item?id=49272655)

**Background**: AmigaDOS is the disk operating system component of AmigaOS, providing file systems, file manipulation, and a command-line interface. In the original AmigaOS 1.x, it was based on a port of TRIPOS by MetaComCo and written in BCPL. It was later rewritten in C for AmigaOS 2.x onward.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AmigaDOS">AmigaDOS</a></li>

</ul>
</details>

**Discussion**: The HN discussion is warm and appreciative. Commenters thank Dr. King for hours spent using the Amiga and credit AmigaDOS with introducing them to the command line, which later eased their transition to Linux. One commenter remembers him as the founder of UK Online, and another shares a 2021 interview.

**Tags**: `#Amiga`, `#AmigaDOS`, `#obituary`, `#retrocomputing`, `#Tim King`

---

<a id="item-18"></a>
## [Mass scans spoof AI bots like ClaudeBot](https://knownagents.com/insights) ⭐️ 6.0/10

Mass automated vulnerability scans are now impersonating AI training bot user agents such as ClaudeBot. Observers report sustained high-volume traffic from Google Cloud IP space, ramping up to roughly 70,000 requests per minute since early August. This development matters because spoofed AI crawler user agents can evade allowlists that treat known bots as friendly, potentially hiding malicious scanning among trusted traffic. It also signals growing sophistication in internet background noise, making threat detection harder for defenders. The scans reuse legitimate AI-training bot user agent strings and appear to be under centralized control, according to affected operators. One operator reported ~70k req/min from Google Cloud AS396982 and said reports to GCP Abuse went unanswered.

hackernews · gavinhking · Aug 12, 14:02 · [Discussion](https://news.ycombinator.com/item?id=49272569)

**Background**: ClaudeBot is Anthropic's web crawler that collects data to train its Claude large language models. User agent spoofing is a technique in which a client changes its User-Agent HTTP header to impersonate another software or device, commonly used by bots to bypass filters. Mass automated vulnerability scanning has been a common phenomenon on the internet since at least the 2001 Code Red worm, which similarly flooded server logs with requests.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ClaudeBot">ClaudeBot</a></li>
<li><a href="https://en.wikipedia.org/wiki/User_agent_spoofing">User agent spoofing</a></li>
<li><a href="https://www.fraudlogix.com/blog/understanding-and-detecting-forged-user-agents-a-guide-for-fraud-detection-and-prevention/">User Agent Spoofing: How To Spot & Stop Fake User Agents</a></li>

</ul>
</details>

**Discussion**: Commenters largely downplayed the novelty, noting that servers see thousands of probe hits daily and that this is just the same junk traffic with a new disguise. Some shared personal observations of heavy scanning traffic and expressed skepticism about the effectiveness of reporting to cloud providers, while others noted the relevant ASN ownership as a better indicator than user agent strings.

**Tags**: `#security`, `#vulnerability scanning`, `#AI bots`, `#bot detection`, `#network traffic`

---

<a id="item-19"></a>
## [YC P26 startup launches AI agents for semiconductor materials discovery](https://discoveredmaterials.com/research/) ⭐️ 6.0/10

Discovered Materials, a YC P26-backed startup, launched on Hacker News with AI agents that computationally discover new semiconductor materials. They released hundreds of new materials and a benchmark measuring frontier models' material-discovery ability, claiming 8-hour model runs match weeks of PhD-level work. The startup targets chip thermal management, a critical bottleneck as GPU TDP doubles nearly every generation, from the H100's 700W to Rubin's projected 2.3kW. If AI agents can shorten the 'lab-to-fab valley of death', they could accelerate adoption of 3D packaging, new thermal interface materials, and substrates, reducing data-center power and water consumption. The founders tested seven models from Anthropic, OpenAI, and Kimi and observed strange behaviors such as Claude's reward hacking and GPT-5.6 'losing its mind' after roughly 50M tokens. They also report that their simulated, synthesized, and tested thermal interface materials matched the performance of materials guarded as trade secrets for over 20 years; the business model involves licensing IP on both materials and synthesis recipes.

hackernews · advaith08 · Aug 12, 07:51 · [Discussion](https://news.ycombinator.com/item?id=49269090)

**Background**: Thermal design power (TDP) is the maximum heat a chip can generate during normal operation and that its cooling system must dissipate. 3D chip packaging stacks chiplets, such as HBM memory stacks, directly on logic dies to cut data-movement energy, but dielectric materials like SiO2 are poor thermal conductors and trap heat. The 'lab-to-fab valley of death' refers to the years and hundreds of millions of dollars required to turn a computational material prediction into a manufacturable chip material. AI agents are hoped to reduce experimental iteration counts and help generate synthesis recipes.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Thermal_design_power">Thermal design power - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Three-dimensional_integrated_circuit">Three-dimensional integrated circuit - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters were cautiously optimistic. One noted that past AI-driven materials discovery lacked real impact but praised this effort for addressing feasibility, while another called closing the computational-experimental loop the main remaining challenge. Others expressed excitement about HBM-on-top-of-chip ideas and curiosity about how the team mitigates reward-hacking behavior.

**Tags**: `#AI`, `#materials-science`, `#semiconductors`, `#YC`, `#startup`

---

<a id="item-20"></a>
## [Datasette Upload DBS 0.5a0 Adds Formalized API for Database Uploads](https://simonwillison.net/2026/Aug/11/datasette-upload-dbs/) ⭐️ 6.0/10

The release adds a formalized HTTP API to the existing datasette-upload-dbs plugin, allowing users to upload or atomically swap SQLite database files on a hosted Datasette instance by sending a POST request to /-/upload-dbs. Previously this could only be done through the plugin's web interface. This makes it possible to automate database deployment and updating, for example building a fresh database in a CI system like GitHub Actions and immediately swapping it into production. It strengthens Datasette's position as a platform for data publishing and reduces friction for teams that need to refresh data regularly. The new endpoint requires an Authorization: Bearer header with a token, and accepts a multipart form with the db file and db_name fields. The uploaded database is saved to disk, verified, and then swapped atomically, so the /name path serves the new version without downtime.

rss · Simon Willison · Aug 11, 20:35

**Background**: Datasette is an open-source tool for exploring and publishing data, which turns SQLite databases into interactive websites and JSON APIs. The datasette-upload-dbs plugin, created by Simon Willison, lets users upload SQLite files directly to a hosted Datasette instance, where they are automatically served. This release extends that capability with a formal programmatic interface, opening the door to fully automated publishing workflows.

<details><summary>References</summary>
<ul>
<li><a href="https://datasette.io/">Datasette: An open source multi-tool for exploring and ...</a></li>
<li><a href="https://docs.datasette.io/">Datasette documentation</a></li>
<li><a href="https://pypi.org/project/datasette-upload-dbs/">datasette-upload-dbs · PyPI</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#sqlite`, `#plugin`, `#api`, `#database`

---

<a id="item-21"></a>
## [AAAI 2027 Reviewers Flag Missing Code in Submissions](https://www.reddit.com/r/MachineLearning/comments/1vlqjby/aaai_2027_review_no_code_submission_d/) ⭐️ 6.0/10

A AAAI 2027 reviewer reports that many submissions in their batch lack code implementation, despite the conference's explicit emphasis on reproducibility. The reviewer is considering whether to penalize such papers in their initial scores and asks the community for opinions. This highlights a persistent gap between reproducibility policies and actual peer-review practice in ML conferences, which can undermine trust in published results. The discussion could influence how reviewers weigh code availability and shape future author incentives. AAAI requires a reproducibility checklist to be submitted with every paper, but it does not mandate code submission as a hard requirement. The reviewer expresses concern that modern AI assistants can quickly generate empirical papers with artificial results, making code verification increasingly important.

reddit · r/MachineLearning · /u/wontonut · Aug 11, 18:58

**Background**: AAAI-27 submission instructions require authors to complete a reproducibility checklist from the author kit at submission time, though providing code is optional. Artifact evaluation initiatives at venues like MLSys and MICRO already make code, data, and other artifacts part of the assessment process, but practice varies across conferences.

<details><summary>References</summary>
<ul>
<li><a href="https://aaai.org/conference/aaai/aaai-27/submission-instructions/">AAAI-27 Submission Instructions - AAAI</a></li>
<li><a href="https://aaai.org/conference/aaai/aaai-23/reproducibility-checklist/">Reproducibility Checklist - AAAI</a></li>
<li><a href="https://neurips.cc/public/guides/PaperChecklist">NeurIPS Paper Checklist Guidelines</a></li>

</ul>
</details>

**Tags**: `#reproducibility`, `#AAAI`, `#code submission`, `#peer review`, `#machine learning`

---

<a id="item-22"></a>
## [Seeking RL/Planning Pointers for Stochastic Merge Puzzle with Afterstates](https://www.reddit.com/r/MachineLearning/comments/1vlfavg/planningrl_for_a_stochastic_singleplayer_merge/) ⭐️ 6.0/10

A developer asks the community for algorithm and implementation suggestions to build an AI for a stochastic single-player merge puzzle that uses afterstates and one-step previewed random events. The post details the game rules, network input representation, and current planning approach with an exact simulator. This question tackles a nontrivial combination of afterstate representations, previewed chance events, and long-horizon throughput objectives. Answers could benefit researchers and hobbyists working on similar board/puzzle games, especially where planning budgets are limited and randomness is partially observable in advance. The game has 6 stacks of height 7, 30 ordered-column-pair actions that move entire runs of equal tiles, merge cascades, and a game-over when a stack exceeds height 7. Every fourth action is followed by a six-tile random drop whose values are previewed after the third action. The user's policy/value network is column-permutation equivariant with 394 features, and they treat the timed mode as a continuing average-reward/throughput problem.

reddit · r/MachineLearning · /u/CaiwenGong · Aug 11, 11:53

**Background**: Afterstate value functions estimate the value of the environment state immediately after an action but before the stochastic outcome, which is natural for games like 2048 and this merge puzzle. The user has access to an exact simulator, so model-based planning methods such as Monte Carlo tree search (MCTS) or receding-horizon optimization can be combined with learned value/policy models. The preview of the random drop is a chance event that can be planned through deterministically once revealed, which distinguishes this problem from fully observable stochastic planning.

<details><summary>References</summary>
<ul>
<li><a href="https://ai.stackexchange.com/questions/24816/how-are-afterstate-value-functions-mathematically-defined">reinforcement learning - How are afterstate value functions ...</a></li>
<li><a href="https://openreview.net/forum?id=XO944P8prc">Afterstate Reinforcement Learning for Continuous Control</a></li>

</ul>
</details>

**Tags**: `#reinforcement learning`, `#planning`, `#monte carlo tree search`, `#afterstates`, `#merge puzzle`

---