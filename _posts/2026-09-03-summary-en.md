---
layout: default
title: "Horizon Summary: 2026-09-03 (EN)"
date: 2026-09-03
lang: en
---

> From 30 items, 16 important content pieces were selected

---

1. [GPT-6 Astra](#item-1) ⭐️ 10.0/10
2. [Porting my 1993 Amiga game to Godot, with an LLM reading the 68000 assembly](#item-2) ⭐️ 8.0/10
3. [Audacity 4.0 Released with Qt6 UI and Extensive Fixes](#item-3) ⭐️ 8.0/10
4. [Paint.NET's Rick Brewster Reveals Claude-Coded Clean-Room Direct2D Rewrite for WINE](#item-4) ⭐️ 8.0/10
5. [Jasper Research Releases Cookbook, Dataset, and Code for Training Text-to-Image Models From Scratch](#item-5) ⭐️ 8.0/10
6. [Open-Source AI Detectors Fail 0.5% False-Positive Target, Bias Found](#item-6) ⭐️ 8.0/10
7. [Qwen 3.8 27B Hits Cerebras at 1500 Tokens/s](#item-7) ⭐️ 7.0/10
8. [.name Termination](#item-8) ⭐️ 7.0/10
9. [Go Grandmaster Shin Jinseo Defeats AI KataGo with Two-Stone Handicap](#item-9) ⭐️ 7.0/10
10. [Claude Fable 5.1 Sets Science Benchmark Record and Passes Pelican Test](#item-10) ⭐️ 7.0/10
11. [Deepity: C++ Predictive Coding Library Matches Backprop on MNIST at 97.73%](#item-11) ⭐️ 7.0/10
12. [CABiNet Author Publishes Reproducible UAVid Benchmark vs YOLO26-sem](#item-12) ⭐️ 7.0/10
13. [IFM's K2 Horizon Offers Six Fully Open AI Models](#item-13) ⭐️ 6.0/10
14. [Any Human Ever Lets You Explore a Random Life from Human History](#item-14) ⭐️ 6.0/10
15. [Claude's new system prompt bars song lyric reproduction](#item-15) ⭐️ 6.0/10
16. [Mol-JEPA: Multimodal JEPA Foundation Model for Molecules](#item-16) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [GPT-6 Astra](https://openai.com/index/gpt-6-astra/) ⭐️ 10.0/10

OpenAI announces GPT-6 Astra, a new flagship model with a system card, showing near-perfect ARC-AGI-3 scores alongside mixed benchmark improvements.

hackernews · kibae · Sep 3, 18:41 · [Discussion](https://news.ycombinator.com/item?id=49554643)

**Tags**: `#openai`, `#gpt-6`, `#ai`, `#llm`, `#benchmarks`

---

<a id="item-2"></a>
## [Porting my 1993 Amiga game to Godot, with an LLM reading the 68000 assembly](https://babyloniantwins.com/blog/porting-a-1993-amiga-game-to-godot/) ⭐️ 8.0/10

A developer shares their experience using Claude to port their 1993 Amiga game from 68000 assembly to Godot, highlighting the efficiency and potential of LLM-assisted code translation.

hackernews · rabahs · Sep 3, 14:28 · [Discussion](https://news.ycombinator.com/item?id=49550375)

**Tags**: `#LLM`, `#Godot`, `#Amiga`, `#retro computing`, `#software porting`

---

<a id="item-3"></a>
## [Audacity 4.0 Released with Qt6 UI and Extensive Fixes](https://github.com/audacity/audacity/releases/tag/Audacity-4.0.0) ⭐️ 8.0/10

Audacity 4.0.0 has been released on GitHub as a major overhaul of the open-source audio editor, introducing a new Qt6-based user interface and numerous fixes. According to the release tag and community commentary, this is a significant step up from the Audacity 3 series. As one of the most widely used open-source audio editors, Audacity 4.0 affects a large audience, from hobbyists and podcasters to professional-sounding home studios. The switch to Qt6 may change how the program behaves, how plugins and system audio are handled, and how sustainable future development will be. Community members note that some long-standing Linux workflow issues, such as Audacity only creating a temporary JACK client during playback or recording, appear to remain in version 4. Others express concern about integration with audio.com and telemetry-related features that previously led to forks like Tenacity and Sneedacity.

hackernews · ClydeN · Sep 3, 10:53 · [Discussion](https://news.ycombinator.com/item?id=49548395)

**Background**: Audacity is a free, open-source digital audio editor used for recording, editing, and mixing audio on Linux, Windows, and macOS. Qt6 is the newest major release of the Qt framework; Qt is a cross-platform application development framework for creating graphical user interfaces that run on various platforms such as Linux, Windows, macOS, and Android. Replacing Audacity's UI framework is a major engineering change because it touches the widgets, rendering, and system-level audio integration the editor depends on.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Qt6">Qt6</a></li>

</ul>
</details>

**Discussion**: Community reaction is split: some users are enthusiastic about the cleaner UI and fixes, recommending the release video and the work of the software head at Muse, while others are disappointed that long-standing technical issues, such as non-persistent JACK clients on Linux, remain unaddressed. Several commenters also brought up the post-telemetry forks Tenacity and Sneedacity, asking what happened to those projects.

**Tags**: `#audacity`, `#open-source`, `#audio-editing`, `#release`, `#qt6`

---

<a id="item-4"></a>
## [Paint.NET's Rick Brewster Reveals Claude-Coded Clean-Room Direct2D Rewrite for WINE](https://simonwillison.net/2026/Sep/2/rick-brewster/) ⭐️ 8.0/10

Rick Brewster, the developer of Paint.NET, announced that the application now contains an internal, from-scratch, clean-room reverse-engineered rewrite of Direct2D, triggered by the /wine command-line flag for experimental Windows-on-Linux support inside WINE. Most of the approximately 180,000 lines of new code in PaintDotNet.Windows.Direct2D1.Managed.dll were 'vibe coded' with Claude AI. This is a major compatibility breakthrough for Paint.NET on WINE, as Direct2D had always been the biggest hurdle and is unlikely to ever be completed in WINE itself. It also serves as a prominent real-world example of AI-generated code at scale for complex system-level software, demonstrating both its strengths and the need for careful human supervision. Brewster stated that the code had not been thoroughly reviewed, describing it as 'trust me bro' style, and that Claude required close babysitting for resource management, including initially failing to perform the COM equivalent of AddRef() on reference-counted objects. Claude also performed reverse engineering to derive the formulas needed for Direct2D's built-in effects library.

rss · Simon Willison · Sep 2, 05:50

**Background**: Direct2D is a Microsoft API for hardware-accelerated 2D graphics rendering, while WINE is a compatibility layer that aims to run Windows applications on Linux. Clean-room reverse engineering, as described by Wikipedia, is a method of copying a design by reverse engineering and recreating it without infringing copyright. 'Vibe coding' is AI-generated code where the programmer guides, tests, and gives feedback rather than manually writing every line.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Clean-room_design">Clean-room design - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Vibe_coding">Vibe coding - Wikipedia</a></li>
<li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=6812">Download DirectX Software Development Kit from Official Microsoft...</a></li>

</ul>
</details>

**Tags**: `#Direct2D`, `#Paint.NET`, `#WINE`, `#AI code generation`, `#reverse engineering`

---

<a id="item-5"></a>
## [Jasper Research Releases Cookbook, Dataset, and Code for Training Text-to-Image Models From Scratch](https://www.reddit.com/r/MachineLearning/comments/1w5c9rd/detailed_explanation_of_how_to_create_a/) ⭐️ 8.0/10

Jasper Research released a detailed technical cookbook, a minimal codebase called nano-t2i, and an open dataset of roughly 104.9 million image-text pairs named MONET for training text-to-image models from scratch. The release includes full reasoning, intermediate results, and runnable code so readers can reproduce the process. This release is significant because it offers an open, transparent look at how frontier-style text-to-image models might be built from scratch, a process often obscured by proprietary details. It lowers the barrier for researchers and developers to study and train their own models instead of only fine-tuning existing ones, while also making a large-scale dataset publicly available. The MONET dataset was curated from 2.9 billion raw image-text pairs through filtering, deduplication, and re-captioning, and is released under the Apache 2.0 license. The nano-t2i codebase ships with a tiny model so users can run an end-to-end text-to-image training pipeline on modest hardware.

reddit · r/MachineLearning · /u/dh7net · Sep 2, 14:40

**Background**: Text-to-image models generate pictures from natural-language descriptions, and building one from scratch typically requires a model architecture, a training procedure, and a very large collection of captioned images. Open, well-curated datasets are a known bottleneck for reproducible research because collecting and cleaning hundreds of millions of image-text pairs is expensive. MONET is an attempt to fill that gap, and the cookbook and nano-t2i codebase are meant to accompany it with the full practical reasoning and implementation details.

<details><summary>References</summary>
<ul>
<li><a href="https://gojasper.github.io/monet/">MONET - gojasper.github.io</a></li>
<li><a href="https://arxiv.org/abs/2605.21272">MONET: A Massive, Open, Non-redundant and Enriched Text-to-image dataset</a></li>

</ul>
</details>

**Tags**: `#text-to-image`, `#deep learning`, `#dataset`, `#tutorial`, `#model training`

---

<a id="item-6"></a>
## [Open-Source AI Detectors Fail 0.5% False-Positive Target, Bias Found](https://www.reddit.com/r/MachineLearning/comments/1w58erw/most_opensource_ai_detectors_cant_hold_a_05/) ⭐️ 8.0/10

An evaluation of six open-source AI detectors found that four cannot reliably reach a matched 0.5% false-positive rate; the best detector caught only 41.6% of humanizer-paraphrased AI text, while the OpenAI RoBERTa detector scored AUC 0.31 on modern generators. The study used public datasets, including 5,000 pre-LLM FineWeb pages, and released the full methodology for replication. The results show that current open-source AI detectors are not reliable for real-world use, especially at the strict low false-positive rates required for fair accusation, and they systematically flag non-native English essays more often than native ones. This has direct implications for educators, publishers, and tool developers who rely on these models. The evaluation matched all thresholds to a 0.5% false-positive rate on the same 6,930 human documents across six detectors. MAGE could not reach 0.5% FPR at any threshold, flagging 26% of ordinary human web text with scores above 0.9999; humanizer-paraphrased text caused the biggest performance collapse, with the best model achieving only 42% recall.

reddit · r/MachineLearning · /u/grumpyp2 · Sep 2, 12:04

**Background**: AI-generated text detectors classify whether a passage was written by a human or by large language models. A matched 0.5% false-positive rate means the threshold is set so only 0.5% of genuine human text is wrongly flagged, which is important because false accusations can harm students and writers. Humanizer tools rewrite AI output to evade detection, and FineWeb is a large open web-text dataset; this study used pages from before the LLM era (2018) as a clean human baseline. The MAGE paper also frames detection in the wild as hard because texts come from diverse domains and models.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2305.13242v3">MAGE: Machine-generated Text Detection in the Wild - arXiv.org</a></li>
<li><a href="https://huggingface.co/spaces/HuggingFaceFW/blogpost-fineweb-v1">FineWeb: decanting the web for the finest text data at scale - a Hugging Face Space by HuggingFaceFW</a></li>
<li><a href="https://arxiv.org/abs/2406.17557">[2406.17557] The FineWeb Datasets: Decanting the Web for the Finest Text Data at Scale</a></li>

</ul>
</details>

**Tags**: `#AI detection`, `#benchmark`, `#open-source`, `#bias`, `#machine learning`

---

<a id="item-7"></a>
## [Qwen 3.8 27B Hits Cerebras at 1500 Tokens/s](https://inference-docs.cerebras.ai/models/overview) ⭐️ 7.0/10

Alibaba Cloud's Qwen 3.8 27B model is now being served on Cerebras' wafer-scale inference platform at a headline speed of 1500 tokens per second. Early user reports, however, indicate significant rate-limiting and billing friction that reduce real-world usability. If the speed holds up, it could make a 27-billion-parameter model highly attractive for interactive coding assistants and other latency-sensitive workloads. Yet the current access constraints show that raw token throughput alone is not enough to guarantee a smooth developer experience. Community members cite a 450,000-token-per-minute cap, with cached tokens also counted toward the limit, and some Enterprise accounts are locked out of self-serve billing. In one comparison, a user said the same coding task cost $1.10 and was still incomplete on Qwen 3.8 27B, while DeepSeek-V4-Flash finished in 172 seconds for only $0.024.

hackernews · altertable · Sep 3, 18:32 · [Discussion](https://news.ycombinator.com/item?id=49554520)

**Background**: Cerebras builds the Wafer Scale Engine (WSE), the world's largest AI processor, and markets its CS series to deliver inference far faster than traditional GPUs. Qwen (also known as Tongyi Qianwen) is a family of open-weights language models developed by Alibaba Cloud, ranging from small to very large parameter counts; the 27B variant is a mid-sized model aiming to balance capability and cost.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cerebras_Systems">Cerebras Systems - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>
<li><a href="https://www.cerebras.ai/chip">Product - Chip - Cerebras</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some users praise the fast output speed and point to local alternatives like ninfer on an RTX 5090 reaching 200–400 tokens/s, while others call the rate limits and per-token costs prohibitive for coding tasks. Several ask Cerebras to offer the model through OpenRouter or provide a flexible rate pool, and express frustration that Enterprise accounts cannot update billing information.

**Tags**: `#qwen`, `#cerebras`, `#inference`, `#llm`, `#ai-infrastructure`

---

<a id="item-8"></a>
## [.name Termination](https://neil.fraser.name/news/2026/09/03/) ⭐️ 7.0/10

Verisign proposes terminating existing .name third-level domain registrations, sparking community debate over ICANN's stability mission and the fate of affected domains.

hackernews · pavel_lishin · Sep 3, 14:54 · [Discussion](https://news.ycombinator.com/item?id=49550772)

**Tags**: `#DNS`, `#ICANN`, `#domains`, `#internet governance`, `#Verisign`

---

<a id="item-9"></a>
## [Go Grandmaster Shin Jinseo Defeats AI KataGo with Two-Stone Handicap](https://www.kedglobal.com/artificial-intelligence/newsView/ked202607210007) ⭐️ 7.0/10

In a recent handicap game, Go grandmaster Shin Jinseo defeated the leading open-source AI KataGo while receiving a two-stone handicap. The result showcases one of the strongest human players in history beating a top-level AI under conditions that reduce the AI's usual advantage. This is significant because KataGo is one of the strongest Go AIs, far beyond any human without a handicap. A human win even at two stones highlights Shin Jinseo's extraordinary skill and fuels debate about the true gap between elite humans and AI in Go. KataGo is a free and open-source computer Go program trained through deep learning and self-play reinforcement learning, capable of defeating top professional players. In a two-stone handicap game, the AI gives the human two free stones at the start, yet Shin still won, making the result particularly remarkable.

hackernews · gmays · Sep 3, 01:11 · [Discussion](https://news.ycombinator.com/item?id=49544762)

**Background**: KataGo was first released in 2019 by developer David Wu and is one of the strongest Go AIs, using a similar approach to AlphaZero. It is widely used by professional Go players for training and analysis. In even games, top humans have essentially no chance against modern AI, so handicap games are one way to keep matches competitive and to assess relative strength.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/KataGo">KataGo</a></li>

</ul>
</details>

**Discussion**: Commenters noted that Shin Jinseo has been significantly stronger than other humans, and that receiving two stones still made him the weaker side in the match. There was broad agreement that no human could win an even game against KataGo, though one commenter argued that studying AI may be less valuable than playing one's own style, and another recommended the novel "The Master of Go."

**Tags**: `#Go`, `#AI`, `#KataGo`, `#games`, `#human vs AI`

---

<a id="item-10"></a>
## [Claude Fable 5.1 Sets Science Benchmark Record and Passes Pelican Test](https://simonwillison.net/2026/Sep/1/claude-fable-5-1/) ⭐️ 7.0/10

Anthropic today released Claude Fable 5.1, alongside Mythos 5.1, touting gains in coding, knowledge work, and long-running tasks. On the brand-new Terminal-Bench-Science 0.1 benchmark it scored 52.6%, far above Fable 5's 24.7% and GPT-5.6 Sol's 22.4%, and Simon Willison benchmarked it with his 'pelican riding a bicycle' SVG prompt. The 28-point jump on Terminal-Bench-Science suggests real progress in models performing expert-curated scientific research workflows, not just traditional coding tests. Willison's pelican test also provides a quick, human-inspectable signal for how different reasoning effort levels change output quality within the same model family. Fable 5.1 offers five reasoning effort levels (low, medium, high, xhigh, max) with no option to disable reasoning. In Willison's test, both low and medium generated pelican SVGs with no summarized reasoning tokens and similar token counts (~2,000), while higher efforts added visible reasoning and more tokens; outputs cost roughly 10–13 cents each.

rss · Simon Willison · Sep 1, 23:57

**Background**: Claude Fable is Anthropic's series of large language models; 5.1 is the new release discussed in this post, which Anthropic claims 'sets a new standard for coding, knowledge work, and long-running problem-solving tasks.' Terminal-Bench-Science is a new benchmark for evaluating AI agents on real scientific research workflows, with an initial release of 70 tasks across life, physical, Earth, mathematical, and other sciences. The 'pelican benchmark' is an informal test created by Simon Willison in late 2024: ask a model to generate an SVG of a pelican riding a bicycle, then visually inspect the result. It is commonly used as a quick, human-checkable comparison of instruction following and SVG code generation ability.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tbench.ai/news/terminal-bench-science-0-1">TERMINAL-BENCH-SCIENCE 0.1</a></li>
<li><a href="https://grokipedia.com/page/Pelican_on_a_bicycle_AI_benchmark">Pelican on a bicycle (AI benchmark)</a></li>

</ul>
</details>

**Tags**: `#Claude`, `#Anthropic`, `#AI`, `#LLM`, `#Benchmarks`

---

<a id="item-11"></a>
## [Deepity: C++ Predictive Coding Library Matches Backprop on MNIST at 97.73%](https://www.reddit.com/r/MachineLearning/comments/1w5fuhm/deepity_a_c_library_showing_predictive_coding/) ⭐️ 7.0/10

A developer released Deepity, a C++ machine-learning library implementing accelerated Predictive Coding Networks (PCNs). On MNIST, Deepity's DKPPCN model achieved 97.73% test accuracy in 59.5 seconds, nearly matching PyTorch backpropagation's 98.27% in about 70 seconds. This result shows that biologically plausible, local learning methods can be optimized to match backpropagation on a standard benchmark, narrowing the practical gap that has kept PCNs on the sidelines. It strengthens the case for alternative credit-assignment algorithms in scenarios such as continual learning, where backprop is known to struggle. The implementation runs 50 epochs on CPU and uses algorithmic caching to avoid redundant forward projections during the inference settling phase. It is based on the recent 'Accelerated Predictive Coding Networks via Direct Kolen-Pollack Feedback Alignment' research; the author plans to port the kernels to CUDA and test continual-learning scenarios.

reddit · r/MachineLearning · /u/Important-Home4431 · Sep 2, 16:49

**Background**: Predictive Coding Networks (PCNs) are biologically inspired hierarchical generative models that minimize a free-energy objective by computing top-down predictions and bottom-up errors. Unlike standard backpropagation, they rely on iterative inference and local Hebbian-like update rules, which makes them attractive for continual learning but historically much slower in practice. The Direct Kolen-Pollack (DKP) method used here modifies predictive coding to reduce feedback delay and exponential signal decay while preserving local updates.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2506.06332">Introduction to Predictive Coding Networks for Machine Learning</a></li>
<li><a href="https://arxiv.org/html/2602.15571v1">Accelerated Predictive Coding Networks via Direct Kolen ...</a></li>

</ul>
</details>

**Tags**: `#Predictive Coding`, `#Machine Learning`, `#C++`, `#MNIST`, `#Credit Assignment`

---

<a id="item-12"></a>
## [CABiNet Author Publishes Reproducible UAVid Benchmark vs YOLO26-sem](https://www.reddit.com/r/MachineLearning/comments/1w5cfv1/cabinet_icra_2021_vs_yolo26sem_on_uavid_accuracy/) ⭐️ 7.0/10

The original first author of CABiNet (ICRA 2021) released an open, reproducible benchmark comparing CABiNet with YOLO26-sem variants on the UAVid aerial dataset. Results include mIoU, parameters, FLOPs, and FP16 GPU latency on an RTX 4070 SUPER, with CABiNet-Large reaching 67.14 mIoU while YOLO26x-sem reaches 64.41. This matters because it is a rare, author-provided controlled comparison between a purpose-built efficient segmentation network and a modern general-purpose multi-task model on the model's intended benchmark. Practitioners doing real-time aerial semantic segmentation can use the reproduced numbers to decide whether a specialized 2021 architecture or a 2026 YOLO semantic variant offers the better accuracy/latency trade-off. The benchmark standardizes data representation, class weighting, and evaluation protocol (single-scale, no test-time augmentation), while each model keeps its own training recipe, so it is not an architecture-only ablation and the author clearly discloses potential biases. Near-iso-compute, CABiNet-S outperforms YOLO26s by 3.6 mIoU but is slower, while CABiNet-L beats YOLO26x with lower latency; however, on VDD and AeroScapes, YOLO26s and larger variants surpass CABiNet-L.

reddit · r/MachineLearning · /u/Naive-Explanation940 · Sep 2, 14:46

**Background**: CABiNet is a dual-branch convolutional neural network introduced at ICRA 2021 for low-latency semantic segmentation, combining a high-resolution spatial branch with a lightweight context branch built on MobileNetV3. UAVid is an aerial video dataset of urban scenes used for semantic segmentation and was the original benchmark targeted by the CABiNet paper. YOLO26-sem refers to the semantic-segmentation variants of Ultralytics' YOLO26 model family, which has evolved from object detection into a general-purpose multi-task vision framework. This comparison quantifies how architectural specialization, training recipes, parameter count, and GPU efficiency affect real-time segmentation in practice.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/dronefreak/CABiNet">GitHub - dronefreak/CABiNet: CABiNet: Efficient Context Aggregation Network for Low-Latency Semantic Segmentation (ICRA2021) · GitHub</a></li>
<li><a href="https://uavid.nl/">UAVid Semantic Segmentation Dataset</a></li>
<li><a href="https://huggingface.co/dronefreak/uavid-yolo26m-sem">dronefreak/uavid- yolo 26 m- sem · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#semantic-segmentation`, `#UAVid`, `#real-time-vision`, `#YOLO`, `#benchmarking`

---

<a id="item-13"></a>
## [IFM's K2 Horizon Offers Six Fully Open AI Models](https://ifm.ai/blog/k2/) ⭐️ 6.0/10

The Institute of Foundation Models at MBZUAI (Ifm AI) released K2 Horizon, a family of six open-source AI models ranging from 0.9B to 375B parameters. The release includes model weights, source code, training data, and development infrastructure. Full-stack openness is rare: only Nvidia's Nemotron is another prominent fully open model family, so K2 Horizon offers a valuable alternative for transparency and self-hosting. Critics, however, question whether the performance benchmarks match the headline claims, underscoring the importance of independent evaluation. The flagship K2 Horizon 375B-A23B model is a mixture-of-experts with 23 billion active parameters and a 524k-token context window, positioning it among leading open-weight models. Community tests also suggest the dense 32B model may trail Qwen3-27B, and a reviewer found the 3.7B model unreliable for coding.

hackernews · karimf · Sep 3, 15:36 · [Discussion](https://news.ycombinator.com/item?id=49551760)

**Background**: Most open-weight models only release final weights, hiding training data and implementation details. K2 Horizon instead open-sources the training infrastructure, source code, and data preparation, aiming to make the fleet reproducible. The Institute of Foundation Models is part of Mohamed bin Zayed University of Artificial Intelligence (MBZUAI) in Abu Dhabi.

<details><summary>References</summary>
<ul>
<li><a href="https://ifm.ai/blog/k2/">Introducing K 2 Horizon : Frontier Performance, Radically Open</a></li>
<li><a href="https://cryptobriefing.com/k2-horizon-open-source-ai-models/">Institute of Foundation Models unveils K 2 Horizon with six open ...</a></li>
<li><a href="https://artificialanalysis.ai/models/k2-horizon-375b-a23b">K 2 Horizon 375B A23B - Intelligence, Performance... | Artificial Analysis</a></li>

</ul>
</details>

**Discussion**: Overall, commenters appreciated a new fully open stack, but many were skeptical. Specific criticisms included mismatches between headline and reported benchmarks, unreliable code generation on the 3.7B model, and the exhausting frequency of new model releases; others jokingly complained about unreadable charts.

**Tags**: `#AI`, `#open-source`, `#models`, `#machine-learning`

---

<a id="item-14"></a>
## [Any Human Ever Lets You Explore a Random Life from Human History](https://anyhumanever.com/) ⭐️ 6.0/10

The website AnyHumanEver.com randomly selects a hypothetical person's life from a statistical model of all humans who ever lived, generating details such as era, birthplace, family, and diet. Each visit produces a different profile, illustrating demographic patterns across history. This interactive visualization turns abstract demographic data into emotionally engaging personal stories, making it popular with a general audience. It also illustrates the pitfalls of using statistical averages to craft realistic biographies, since individual narratives may inadvertently contradict the underlying data. The site randomizes the birth year according to the actual historical distribution of births, so modern-era lives should dominate most draws, though some users noted mismatches in their samples. Its references include citations such as 'Hajnal (RH31)' and 'Kaplan (RH03)', but link quality and internal consistency of figures like marriage age and child mortality have been questioned.

hackernews · thinkingemote · Sep 3, 14:51 · [Discussion](https://news.ycombinator.com/item?id=49550698)

**Background**: People often assume that a random person from all of human history is equally likely to come from any time, but because population has grown exponentially, most humans who ever lived were actually born near the present day. The site builds each life story by combining model life tables, marriage rates, dietary assumptions, and geographical data for a chosen time and place. Its intended audience includes educators, storytellers, and anyone curious about the texture of ordinary life in different eras.

**Discussion**: In the comments, users praised the project as 'super cool' and useful for role-playing games such as Thousand Year Old Vampire, but also criticized it as 'extremely dubious' regarding data accuracy. One user reported statistical sampling problems, while another found an apparent contradiction between childhood mortality and marriage rates for a woman born in 715 CE.

**Tags**: `#data-visualization`, `#statistics`, `#history`, `#interactive`

---

<a id="item-15"></a>
## [Claude's new system prompt bars song lyric reproduction](https://simonwillison.net/2026/Sep/2/claudes-new-system-prompt/) ⭐️ 6.0/10

Anthropic reorganized its Claude system prompt documentation into per-model pages, and Simon Willison spotlighted a new section in Claude's Fable 5.1 prompt that explicitly forbids reproducing song lyrics, poems, and book passages. The rule includes a public-domain exception for works published before 1929 and requires Claude to decline reworded requests after an initial refusal. System prompts directly shape AI behavior, so this detailed copyright policy shows how Anthropic is preemptively addressing legal risk, especially in the wake of high-profile copyright infringement suits against AI companies. Transparently publishing both current and historical prompts also helps researchers and users understand exactly what content restrictions are in force. The new rule says Claude must not reproduce lyrics, poems, or passages "in whole or in part" — including hooks, choruses, melodies written out note by note, or lines pasted in one at a time — and must keep declining reworded versions for the rest of the conversation. Pre-1929 works are allowed, but Claude relies on its own knowledge of publication dates rather than the user's claims. The docs site supports adding `.md` to any page to get Markdown, making it easy to diff prompt changes.

rss · Simon Willison · Sep 2, 14:16

**Background**: System prompts are the hidden, developer-set instructions that define an AI assistant's rules, persona, and constraints, and they are not editable by end users. Anthropic is unusual in that it publicly archives current and historical system prompts for Claude.ai and its mobile apps, letting anyone diff changes over time. The new lyric restriction likely reflects escalating copyright litigation and pressure from music publishers around AI reproducing song lyrics. These published prompts do not cover agentic tools such as Claude Code or Claude Cowork, which have their own separate systems.

<details><summary>References</summary>
<ul>
<li><a href="https://sitespeak.ai/ai-chatbot-terms/system-prompt">System Prompt: How It Shapes an AI Chatbot's Behaviour</a></li>
<li><a href="https://support.claude.com/en/articles/13345190-get-started-with-claude-cowork">Get started with Claude Cowork | Anthropic Help Center</a></li>
<li><a href="https://www.lilachbullock.com/what-are-system-prompts-ai-chatbots/">What Are System Prompts and Why They Matter for AI Chatbots</a></li>

</ul>
</details>

**Tags**: `#Claude`, `#system prompts`, `#AI safety`, `#Anthropic`, `#copyright`

---

<a id="item-16"></a>
## [Mol-JEPA: Multimodal JEPA Foundation Model for Molecules](https://www.reddit.com/r/MachineLearning/comments/1w6i8pr/moljepa_multimodal_molecular_foundation_model_r/) ⭐️ 6.0/10

The author of Mol-JEPA shared their research paper and a summary website that presents Mol-JEPA, a multimodal JEPA-based foundation model for molecules. The post invites feedback on the model, which the author says needs further performance improvements. Applying JEPA to molecular modeling represents a novel use of the architecture, which could lead to more efficient representation learning for drug discovery and materials design. It extends the JEPA paradigm beyond image and video domains into scientific data, but its real-world impact remains to be validated by the broader research community. Mol-JEPA is a multimodal model that integrates multiple types of molecular data, though the post does not specify the exact modalities. The author worked on the paper for about a year and created an interactive summary at flogrammer.github.io/moljepa; it is a self-post on Reddit with no external validation or discussion yet.

reddit · r/MachineLearning · /u/TerribleAntelope9348 · Sep 3, 19:56

**Background**: JEPA, or Joint Embedding Predictive Architecture, is a self-supervised learning approach championed by Yann LeCun that predicts abstract representations (embeddings) in latent space rather than reconstructing input data like pixels or tokens. It has been applied to images, video, audio, and other domains, with the goal of enabling models to learn world models and reason more like humans. Mol-JEPA applies this architecture to molecular data, aiming to learn robust molecular representations that can support tasks such as property prediction and molecule generation.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Joint_Embedding_Predictive_Architecture">Joint Embedding Predictive Architecture</a></li>
<li><a href="https://www.turingpost.com/p/jepamap">All JEPA Models : 14 Milestones From I- JEPA to ThinkJEPA</a></li>

</ul>
</details>

**Tags**: `#molecular modeling`, `#JEPA`, `#foundation models`, `#multimodal learning`, `#ML research`

---