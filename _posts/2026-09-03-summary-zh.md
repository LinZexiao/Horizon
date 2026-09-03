---
layout: default
title: "Horizon Summary: 2026-09-03 (ZH)"
date: 2026-09-03
lang: zh
---

> 从 30 条内容中筛选出 16 条重要资讯。

---

1. [GPT-6 Astra](#item-1) ⭐️ 10.0/10
2. [将我的 1993 年 Amiga 游戏移植到 Godot：用 LLM 读取 68000 汇编](#item-2) ⭐️ 8.0/10
3. [Audacity 4.0 发布：Qt6 界面全面革新](#item-3) ⭐️ 8.0/10
4. [Paint.NET 开发者公开由 Claude 编写的 Direct2D 净室重写版本](#item-4) ⭐️ 8.0/10
5. [Jasper Research 发布从零训练文生图模型的完整指南、数据集与代码](#item-5) ⭐️ 8.0/10
6. [开源 AI 检测器难达 0.5%误报率，并存在偏见](#item-6) ⭐️ 8.0/10
7. [Qwen 3.8 27B 在 Cerebras 上线，速度 1500 tokens/s](#item-7) ⭐️ 7.0/10
8. [.name 终止](#item-8) ⭐️ 7.0/10
9. [围棋顶级棋手申真谞让两子击败 AI KataGo](#item-9) ⭐️ 7.0/10
10. [Claude Fable 5.1 刷新科学基准，鹈鹕测试表现亮眼](#item-10) ⭐️ 7.0/10
11. [Deepity：用 C++实现的预测编码库在 MNIST 上以 97.73%媲美反向传播](#item-11) ⭐️ 7.0/10
12. [CABiNet 原作者发布与 YOLO26-sem 在 UAVid 上的可复现对比评测](#item-12) ⭐️ 7.0/10
13. [IFM 推出 K2 Horizon：六个完全开源 AI 模型](#item-13) ⭐️ 6.0/10
14. [《Any Human Ever》网站让你体验人类历史中随机一人的一生](#item-14) ⭐️ 6.0/10
15. [Claude 新系统提示词明确禁止复制歌词](#item-15) ⭐️ 6.0/10
16. [Mol-JEPA：面向分子的多模态 JEPA 基础模型](#item-16) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [GPT-6 Astra](https://openai.com/index/gpt-6-astra/) ⭐️ 10.0/10

OpenAI 发布了新旗舰模型 GPT-6 Astra，并附有系统卡，其在 ARC-AGI-3 上取得了近乎完美的分数，但其他基准测试的提升参差不齐。

hackernews · kibae · 9月3日 18:41 · [社区讨论](https://news.ycombinator.com/item?id=49554643)

**标签**: `#openai`, `#gpt-6`, `#ai`, `#llm`, `#benchmarks`

---

<a id="item-2"></a>
## [将我的 1993 年 Amiga 游戏移植到 Godot：用 LLM 读取 68000 汇编](https://babyloniantwins.com/blog/porting-a-1993-amiga-game-to-godot/) ⭐️ 8.0/10

一位开发者分享了他们使用 Claude 将 1993 年的 Amiga 游戏从 68000 汇编移植到 Godot 的经验，凸显了 LLM 辅助代码翻译的效率和潜力。

hackernews · rabahs · 9月3日 14:28 · [社区讨论](https://news.ycombinator.com/item?id=49550375)

**标签**: `#LLM`, `#Godot`, `#Amiga`, `#retro computing`, `#software porting`

---

<a id="item-3"></a>
## [Audacity 4.0 发布：Qt6 界面全面革新](https://github.com/audacity/audacity/releases/tag/Audacity-4.0.0) ⭐️ 8.0/10

Audacity 4.0.0 已在 GitHub 发布，作为这款开源音频编辑器的重大版本更新，引入了基于 Qt6 的全新界面和大量修复。从发布标签和社区评论来看，此次更新相比 Audacity 3 系列是一次明显的跨越。 作为最广泛使用的开源音频编辑软件之一，Audacity 4.0 会影响到从爱好者、播客制作者到家庭录音室的庞大用户群。转向 Qt6 可能会改变程序的运行方式、插件与系统音频的处理方式，以及未来开发的可持续性。 社区成员指出，一些长期存在的 Linux 工作流问题，例如 Audacity 仅在播放或录音期间创建临时 JACK 客户端，在 4.0 中似乎仍未解决。还有人担心与 audio.com 的整合，以及那些曾导致 Tenacity、Sneedacity 等分支出现的遥测相关功能。

hackernews · ClydeN · 9月3日 10:53 · [社区讨论](https://news.ycombinator.com/item?id=49548395)

**背景**: Audacity 是一款免费开源的数字音频编辑软件，用于在 Linux、Windows 和 macOS 上录音、编辑和混音。Qt6 是 Qt 框架的最新主版本；Qt 是一套跨平台应用开发框架，可用于创建在 Linux、Windows、macOS、Android 等平台上运行的图形用户界面。更换 Audacity 的 UI 框架是一次重大的工程改动，因为它会触及编辑器所依赖的控件、渲染和系统级音频集成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Qt6">Qt6</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：一些用户对新界面和修复感到兴奋，并推荐相关发布视频以及 Muse 公司软件主管的工作；另一些用户则对长期存在的技术问题（如 Linux 上 JACK 客户端不持久）仍未解决感到失望。还有评论者提到 Tenacity、Sneedacity 等去遥测分支，询问这些项目后来怎么样了。

**标签**: `#audacity`, `#open-source`, `#audio-editing`, `#release`, `#qt6`

---

<a id="item-4"></a>
## [Paint.NET 开发者公开由 Claude 编写的 Direct2D 净室重写版本](https://simonwillison.net/2026/Sep/2/rick-brewster/) ⭐️ 8.0/10

Paint.NET 开发者 Rick Brewster 宣布，该应用现包含一个从零开始、净室逆向重写的 Direct2D 内部实现，通过/wine 命令行参数启用 WINE 中的实验性 Windows-on-Linux 支持。该实现位于 PaintDotNet.Windows.Direct2D1.Managed.dll 中，约 18 万行新代码大部分是使用 Claude AI“随性编码”完成的。 这是 Paint.NET 在 WINE 上兼容性的重大突破，因为 Direct2D 一直是最大障碍，且 WINE 本身几乎不可能完整支持它。同时，这也是 AI 大规模生成复杂系统级软件的一个标志性实际案例，既展示了它的优势，也说明需要人工仔细监督。 Brewster 表示，这些代码并未被全面审查，属于“信我兄弟”风格；Claude 在资源管理方面需要密切盯守，例如最初未对引用计数对象执行相当于 COM 中 AddRef()的操作。Claude 还进行了逆向工程，推导出 Direct2D 内置效果库所需的各种公式。

rss · Simon Willison · 9月2日 05:50

**背景**: Direct2D 是微软推出的用于硬件加速 2D 图形渲染的 API，而 WINE 是旨在让 Windows 应用在 Linux 上运行的兼容层。净室逆向工程（Wikipedia 指出）是一种通过逆向工程复制设计并重新实现而不侵犯版权的做法。“随性编码”是指由 AI 生成代码，程序员负责引导、测试和反馈，而不是逐行手动编写。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Clean-room_design">Clean-room design - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Vibe_coding">Vibe coding - Wikipedia</a></li>
<li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=6812">Download DirectX Software Development Kit from Official Microsoft...</a></li>

</ul>
</details>

**标签**: `#Direct2D`, `#Paint.NET`, `#WINE`, `#AI code generation`, `#reverse engineering`

---

<a id="item-5"></a>
## [Jasper Research 发布从零训练文生图模型的完整指南、数据集与代码](https://www.reddit.com/r/MachineLearning/comments/1w5c9rd/detailed_explanation_of_how_to_create_a/) ⭐️ 8.0/10

Jasper Research 发布了一本详尽的技术手册、一个名为 nano-t2i 的精简代码库，以及一个包含约 1.049 亿图文对的开源数据集 MONET，用于从零训练文生图模型。该发布包含了完整的思路推导、中间结果和可运行代码，读者可以复现整个过程。 这一发布意义重大，因为它以开放、透明的方式展示了如何从零构建前沿风格的文生图模型，而这一过程往往被闭源细节所掩盖。它降低了研究人员和开发者学习并训练自己模型的门槛，使其不再只能微调现有模型，同时还公开了大规模数据集。 MONET 数据集从 29 亿原始图文对中经过过滤、去重和重新标注后得到，并以 Apache 2.0 协议发布。nano-t2i 代码库附带一个小型模型，用户可以在普通硬件上跑通端到端的文生图训练流程。

reddit · r/MachineLearning · /u/dh7net · 9月2日 14:40

**背景**: 文生图模型是根据自然语言描述生成图片的模型；从零构建这样一个模型通常需要模型架构、训练流程以及海量带描述图片的数据。开放且精心整理的数据集是可复现研究的公认瓶颈，因为收集并清洗数亿图文对的成本很高。MONET 正是为了填补这一空白而提出，而手册和 nano-t2i 代码库则通过完整的实践思路与实现细节来配套使用该数据集。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://gojasper.github.io/monet/">MONET - gojasper.github.io</a></li>
<li><a href="https://arxiv.org/abs/2605.21272">MONET: A Massive, Open, Non-redundant and Enriched Text-to-image dataset</a></li>

</ul>
</details>

**标签**: `#text-to-image`, `#deep learning`, `#dataset`, `#tutorial`, `#model training`

---

<a id="item-6"></a>
## [开源 AI 检测器难达 0.5%误报率，并存在偏见](https://www.reddit.com/r/MachineLearning/comments/1w58erw/most_opensource_ai_detectors_cant_hold_a_05/) ⭐️ 8.0/10

一项对六款开源 AI 检测器的评估显示，其中四款无法稳定达到匹配的 0.5%误报率；表现最好的检测器对经 humanizer 改写的 AI 文本仅捕获 41.6%，而 OpenAI 的 RoBERTa 检测器在现代生成文本上 AUC 仅为 0.31。该研究使用公开数据集（包括 5,000 个 LLM 之前的 FineWeb 页面），并公开了完整方法以供复现。 结果表明，当前开源 AI 检测器在现实场景中并不可靠，尤其是在公平指控所需的严格低误报率下，而且它们对非英语母语者作文的标记率系统性高于母语者。这对依赖此类模型的教育工作者、出版方和工具开发者有直接影响。 该评估在相同的 6,930 篇人类文档上，将六款检测器的阈值统一匹配到 0.5%误报率。MAGE 在任何阈值下都无法达到 0.5%误报率，对 26%的普通人类网页文本给出大于 0.9999 的得分；经 humanizer 改写的文本导致性能大幅下降，最佳模型召回率仅为 42%。

reddit · r/MachineLearning · /u/grumpyp2 · 9月2日 12:04

**背景**: AI 生成文本检测器用于判断一段文字是由人类还是由大语言模型编写。匹配的 0.5%误报率意味着阈值被设定为仅错误标记 0.5%的真实人类文本，这一点很重要，因为误判会伤害学生和写作者。Humanizer 工具通过改写 AI 输出以绕过检测；FineWeb 是一个大型开放网页文本数据集，本研究使用 2018 年（LLM 时代之前）的页面作为干净的人类基线。MAGE 论文同样指出，由于文本来自不同领域和模型，现实场景中的检测非常困难。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2305.13242v3">MAGE: Machine-generated Text Detection in the Wild - arXiv.org</a></li>
<li><a href="https://huggingface.co/spaces/HuggingFaceFW/blogpost-fineweb-v1">FineWeb: decanting the web for the finest text data at scale - a Hugging Face Space by HuggingFaceFW</a></li>
<li><a href="https://arxiv.org/abs/2406.17557">[2406.17557] The FineWeb Datasets: Decanting the Web for the Finest Text Data at Scale</a></li>

</ul>
</details>

**标签**: `#AI detection`, `#benchmark`, `#open-source`, `#bias`, `#machine learning`

---

<a id="item-7"></a>
## [Qwen 3.8 27B 在 Cerebras 上线，速度 1500 tokens/s](https://inference-docs.cerebras.ai/models/overview) ⭐️ 7.0/10

阿里云 Qwen 3.8 27B 现已上线 Cerebras 晶圆级推理平台，宣传速度达每秒 1500 tokens。但早期用户反馈显示，实际使用中仍面临显著的速率限制和计费摩擦。 如果这一速度能保持，27B 参数级别的模型将非常适合交互式编程助手及其他对延迟敏感的应用。然而，目前的使用限制表明，仅靠原始 token 吞吐量无法保证顺畅的开发者体验。 社区称存在每分钟 45 万 token 的限制，缓存 token 也计入限额，且部分 Enterprise 账号无法自助修改账单。有用户对比同一任务：Qwen 3.8 27B 消耗 $1.10 仍未完成，而 DeepSeek-V4-Flash 用时 172 秒、仅花费 $0.024。

hackernews · altertable · 9月3日 18:32 · [社区讨论](https://news.ycombinator.com/item?id=49554520)

**背景**: Cerebras 生产晶圆级引擎（WSE），号称全球最大的 AI 处理器，其 CS 系列面向推理市场，声称比 GPU 快得多。Qwen（又称通义千问）是阿里云开发的开源权重语言模型系列，涵盖从小到大多种参数规模；27B 是其中兼顾性能与成本的中型变体。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cerebras_Systems">Cerebras Systems - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>
<li><a href="https://www.cerebras.ai/chip">Product - Chip - Cerebras</a></li>

</ul>
</details>

**社区讨论**: 社区反馈褒贬不一：有人称赞其输出速度，并指出本地方案（如 RTX 5090 上的 ninfer）也能达到 200–400 tokens/s；另一些人则认为速率限制和按 token 计费让编码任务难以实用。多人呼吁 Cerebras 通过 OpenRouter 提供该模型或给出灵活速率池，并对 Enterprise 账号无法更新账单信息表示不满。

**标签**: `#qwen`, `#cerebras`, `#inference`, `#llm`, `#ai-infrastructure`

---

<a id="item-8"></a>
## [.name 终止](https://neil.fraser.name/news/2026/09/03/) ⭐️ 7.0/10

威瑞信提议终止现有的.name 三级域名注册，引发社区对 ICANN 稳定性使命及受影响域名命运的讨论。

hackernews · pavel_lishin · 9月3日 14:54 · [社区讨论](https://news.ycombinator.com/item?id=49550772)

**标签**: `#DNS`, `#ICANN`, `#domains`, `#internet governance`, `#Verisign`

---

<a id="item-9"></a>
## [围棋顶级棋手申真谞让两子击败 AI KataGo](https://www.kedglobal.com/artificial-intelligence/newsView/ked202607210007) ⭐️ 7.0/10

近期的一场让子棋中，围棋顶尖棋手申真谞在被让两子的情况下击败了顶级开源 AI KataGo。这一结果展现了人类史上最强棋手之一在缩小 AI 优势的条件下战胜顶尖 AI。 此事意义重大，因为 KataGo 是最强的围棋 AI 之一，在没有让子的情况下远强于任何人类。即使在让两子的情况下人类获胜，也凸显了申真谞非凡的棋力，并引发关于围棋顶尖人类与 AI 之间真实差距的讨论。 KataGo 是一款免费开源的计算机围棋程序，通过深度学习和自我对弈强化学习训练，实力足以击败顶尖职业棋手。在让两子的对局中，AI 从开局就让人类两颗棋子，但申真谞依然获胜，因此这一结果尤为引人注目。

hackernews · gmays · 9月3日 01:11 · [社区讨论](https://news.ycombinator.com/item?id=49544762)

**背景**: KataGo 于 2019 年由开发者 David Wu 首次发布，是世界上最强的围棋 AI 之一，采用与 AlphaZero 相似的深度学习和自我对弈强化学习方式。它被职业棋手广泛用于训练和分析。在分先（不让子）对局中，顶尖人类棋手几乎没有任何机会战胜现代 AI，因此让子棋是让比赛保持竞争性并评估相对实力的一种方式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/KataGo">KataGo</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，申真谞远强于其他人类棋手，而受让两子仍意味着他是较弱的一方。大家普遍认为在分先对局中没有任何人类能战胜 KataGo；也有评论者认为研究 AI 不如坚持自己的行棋风格，还有人推荐了小说《围棋大师》。

**标签**: `#Go`, `#AI`, `#KataGo`, `#games`, `#human vs AI`

---

<a id="item-10"></a>
## [Claude Fable 5.1 刷新科学基准，鹈鹕测试表现亮眼](https://simonwillison.net/2026/Sep/1/claude-fable-5-1/) ⭐️ 7.0/10

Anthropic 今天发布了 Claude Fable 5.1（以及 Mythos 5.1），宣称在编程、知识工作和长时任务上有进步。它在全新的 Terminal-Bench-Science 0.1 基准上拿下 52.6%，远高于 Fable 5 的 24.7% 和 GPT-5.6 Sol 的 22.4%；Simon Willison 还用他的“骑自行车的鹈鹕”SVG 提示对它做了评测。 在 Terminal-Bench-Science 上跳升 28 个百分点，说明模型在执行专家整理的真实科研工作流方面取得了实质进展，而不仅仅是传统的编程测试。Willison 的鹈鹕测试也为观察同一模型家族内不同推理强度如何改变输出质量，提供了一个快速且可人工检查的信号。 Fable 5.1 提供 low、medium、high、xhigh、max 五档推理强度，且无法完全关闭推理。在 Willison 的测试中，low 和 medium 生成鹈鹕 SVG 时都没有看到推理摘要，输出 token 数也相近（约 2,000）；更高档位会增加可见推理和 token 数，单次输出约花费 10–13 美分。

rss · Simon Willison · 9月1日 23:57

**背景**: Claude Fable 是 Anthropic 的系列大模型；5.1 是这篇文章中提到的新版本，Anthropic 称它“为编程、知识工作和长期问题求解树立了新标准”。Terminal-Bench-Science 是一个评估 AI 代理在真实科研工作流上的新基准，首个版本包含 70 个来自生命科学、物理、地球科学、数学等领域、由实践研究者整理的任务。所谓“鹈鹕基准”则是 Simon Willison 在 2024 年底提出的非正式测试：让模型生成一张“骑自行车的鹈鹕”SVG，再人工查看结果。这类测试常被用来快速、直观地比较模型的指令遵循和 SVG 代码生成能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tbench.ai/news/terminal-bench-science-0-1">TERMINAL-BENCH-SCIENCE 0.1</a></li>
<li><a href="https://grokipedia.com/page/Pelican_on_a_bicycle_AI_benchmark">Pelican on a bicycle (AI benchmark)</a></li>

</ul>
</details>

**标签**: `#Claude`, `#Anthropic`, `#AI`, `#LLM`, `#Benchmarks`

---

<a id="item-11"></a>
## [Deepity：用 C++实现的预测编码库在 MNIST 上以 97.73%媲美反向传播](https://www.reddit.com/r/MachineLearning/comments/1w5fuhm/deepity_a_c_library_showing_predictive_coding/) ⭐️ 7.0/10

开发者发布了 Deepity——一个用 C++ 编写的机器学习库，实现了加速的预测编码网络（PCN）。在 MNIST 上，Deepity 的 DKPPCN 模型在 59.5 秒内达到 97.73% 的测试准确率，几乎追平 PyTorch 反向传播约 70 秒取得的 98.27%。 这一结果表明，具有生物学合理性的局部学习方法经过优化后，可以在标准基准上媲美反向传播，从而缩小了阻碍 PCN 实际应用的性能差距。这也为替代性信用分配算法在持续学习等反向传播表现不佳的场景中提供了更有力的依据。 该实现基于近期研究《Accelerated Predictive Coding Networks via Direct Kolen-Pollack Feedback Alignment》，在 CPU 上训练 50 个 epoch，并利用算法级缓存避免推理收敛阶段的冗余前向投影。作者计划将这些内核移植到 CUDA，以扩展到更大架构，并在反向传播难以应对的持续学习场景中测试其能力。

reddit · r/MachineLearning · /u/Important-Home4431 · 9月2日 16:49

**背景**: 预测编码网络（PCN）是一种受大脑启发的层级生成模型，通过计算自上而下的预测与自下而上的误差来最小化自由能目标。与标准反向传播不同，PCN 依赖迭代推理和类似赫布法则的局部更新规则，因而在持续学习等场景中具有吸引力，但传统实现往往慢得多。本文使用的 Direct Kolen-Pollack（DKP）方法在保持更新局部性的同时，缓解了预测编码中反馈延迟和信号指数衰减的问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2506.06332">Introduction to Predictive Coding Networks for Machine Learning</a></li>
<li><a href="https://arxiv.org/html/2602.15571v1">Accelerated Predictive Coding Networks via Direct Kolen ...</a></li>

</ul>
</details>

**标签**: `#Predictive Coding`, `#Machine Learning`, `#C++`, `#MNIST`, `#Credit Assignment`

---

<a id="item-12"></a>
## [CABiNet 原作者发布与 YOLO26-sem 在 UAVid 上的可复现对比评测](https://www.reddit.com/r/MachineLearning/comments/1w5cfv1/cabinet_icra_2021_vs_yolo26sem_on_uavid_accuracy/) ⭐️ 7.0/10

CABiNet（ICRA 2021）的原作者发布了一项开放且可复现的基准测试，在 UAVid 航拍数据集上比较 CABiNet 与 YOLO26-sem 各变体。结果包括 mIoU、参数量、FLOPs 以及 RTX 4070 SUPER 上的 FP16 GPU 延迟，其中 CABiNet-L 达到 67.14 mIoU，而 YOLO26x-sem 为 64.41。 这很重要，因为这是少有的由作者本人提供的受控对比，在针对性评测数据上把专用高效分割网络与现代通用多任务模型的语义分割变体放在一起比较。从事实时航拍语义分割的开发者可以依据这些可复现的数据，判断专用 2021 架构与 2026 YOLO 语义变体哪个在精度/延迟权衡上更划算。 该基准统一了数据表示、类别权重和评估协议（单尺度、无测试时增强），但各模型保留自己的训练方案，因此并非纯架构消融，作者也明确披露了潜在偏倚。在近似等计算量下，CABiNet-S 比 YOLO26s 高 3.6 mIoU 但更慢，CABiNet-L 则以更低延迟超过 YOLO26x；不过在 VDD 和 AeroScapes 上，YOLO26s 及更大变体优于 CABiNet-L。

reddit · r/MachineLearning · /u/Naive-Explanation940 · 9月2日 14:46

**背景**: CABiNet 是 ICRA 2021 上提出的双分支卷积神经网络，目标是实现低延迟语义分割，它由高分辨率空间分支和基于 MobileNetV3 的轻量上下文分支组成。UAVid 是面向城市航拍视频的语义分割数据集，也是 CABiNet 原始论文的目标基准。YOLO26-sem 指 Ultralytics YOLO26 模型家族中用于语义分割的变体，YOLO26 已从目标检测扩展为通用多任务视觉模型。该对比展示了架构专用性、训练配置、参数量和 GPU 效率如何共同影响实际实时分割效果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/dronefreak/CABiNet">GitHub - dronefreak/CABiNet: CABiNet: Efficient Context Aggregation Network for Low-Latency Semantic Segmentation (ICRA2021) · GitHub</a></li>
<li><a href="https://uavid.nl/">UAVid Semantic Segmentation Dataset</a></li>
<li><a href="https://huggingface.co/dronefreak/uavid-yolo26m-sem">dronefreak/uavid- yolo 26 m- sem · Hugging Face</a></li>

</ul>
</details>

**标签**: `#semantic-segmentation`, `#UAVid`, `#real-time-vision`, `#YOLO`, `#benchmarking`

---

<a id="item-13"></a>
## [IFM 推出 K2 Horizon：六个完全开源 AI 模型](https://ifm.ai/blog/k2/) ⭐️ 6.0/10

MBZUAI 旗下的基础模型研究所（Ifm AI）发布了 K2 Horizon 系列，包含六个开源 AI 模型，参数规模从 0.9B 到 375B 不等。该发布包括模型权重、源代码、训练数据和开发基础设施。 全栈开放在业界相当少见，另一家知名全开放模型系列是英伟达的 Nemotron，因此 K2 Horizon 为透明度和本地部署提供了宝贵选择。然而批评者质疑其性能跑分是否与宣称相符，凸显了独立评估的重要性。 旗舰型号 K2 Horizon 375B-A23B 是一款混合专家模型，拥有 230 亿激活参数和 524k 词元的上下文窗口，在开放权重模型中位居前列。社区测试还表明，稠密的 32B 模型可能落后于 Qwen3-27B，而有评测者发现 3.7B 模型在编码方面并不可靠。

hackernews · karimf · 9月3日 15:36 · [社区讨论](https://news.ycombinator.com/item?id=49551760)

**背景**: 大多数开放权重模型仅发布最终权重，对训练数据和实现细节讳莫如深。K2 Horizon 则将训练基础设施、源代码和数据准备流程一并开源，力求使整个系列可复现。基础模型研究所隶属于阿布扎比的穆罕默德·本·扎耶德人工智能大学（MBZUAI）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ifm.ai/blog/k2/">Introducing K 2 Horizon : Frontier Performance, Radically Open</a></li>
<li><a href="https://cryptobriefing.com/k2-horizon-open-source-ai-models/">Institute of Foundation Models unveils K 2 Horizon with six open ...</a></li>
<li><a href="https://artificialanalysis.ai/models/k2-horizon-375b-a23b">K 2 Horizon 375B A23B - Intelligence, Performance... | Artificial Analysis</a></li>

</ul>
</details>

**社区讨论**: 总体上，评论者对新的全开放模型系列表示赞赏，但也有不少人持怀疑态度。具体批评包括：宣称的性能与自报跑分不符、3.7B 模型在生成代码时表现不可靠，以及新模型发布频率过快让人感到“审美疲劳”；还有评论者调侃文档中的图表字号太小、难以阅读。

**标签**: `#AI`, `#open-source`, `#models`, `#machine-learning`

---

<a id="item-14"></a>
## [《Any Human Ever》网站让你体验人类历史中随机一人的一生](https://anyhumanever.com/) ⭐️ 6.0/10

网站 AnyHumanEver.com 会从全人类历史的统计模型中随机抽取一个虚构人物，并生成其时代、出生地、家庭和饮食等人生细节。每次访问都会产生不同的人生档案，用以展示历史上的数据规律。 这个交互式可视化项目将抽象的人口统计数据转化为具有代入感的个人故事，因而受到大众欢迎。它也展示了用统计平均值构造真实传记时可能存在的陷阱，因为个别叙事可能在无意中与支撑它的数据相矛盾。 该网站会依据历史上真实的人口出生分布来随机选择出生年份，因此大多数随机结果应当是近代人物，不过有用户反映他们的抽样结果并不符合预期。其参考资料包括“Hajnal (RH31)”和“Kaplan (RH03)”等引文，但链接质量以及婚龄、儿童死亡率等数据之间的内在一致性受到质疑。

hackernews · thinkingemote · 9月3日 14:51 · [社区讨论](https://news.ycombinator.com/item?id=49550698)

**背景**: 人们通常会以为，从全部人类历史中随机抽取一个人，其出生年代在任何时期概率相同；但实际上由于人口呈指数增长，大多数曾经活着的人都出生在近代。该网站通过结合模型生命表、婚姻率、饮食假设以及特定年代和地区的地理数据，来构建每个人的人生故事。它面向的受众包括教育工作者、故事创作者，以及任何对历史上普通人生活质感感到好奇的人。

**社区讨论**: 在评论区，有用户称赞这个项目“超酷”，并认为它能用于《千年老吸血鬼》（Thousand Year Old Vampire）等角色扮演游戏；也有人批评它“非常可疑”，在数据准确性方面会误导人。还有用户指出了统计抽样问题，另一名用户则发现在公元 715 年出生的一个女性身上，儿童死亡率和婚姻率等数据之间存在明显矛盾。

**标签**: `#data-visualization`, `#statistics`, `#history`, `#interactive`

---

<a id="item-15"></a>
## [Claude 新系统提示词明确禁止复制歌词](https://simonwillison.net/2026/Sep/2/claudes-new-system-prompt/) ⭐️ 6.0/10

Anthropic 将 Claude 系统提示词文档重组为按模型分类的页面，Simon Willison 指出 Fable 5.1 的提示词中新增了明确禁止再现歌曲歌词、诗歌和书籍段落的章节。规则还包括对 1929 年前发表作品的公有领域例外，并要求 Claude 在首次拒绝后继续拒绝改写后的请求。 系统提示词直接决定 AI 的行为，因此这一详细版权政策表明 Anthropic 正在主动应对法律风险，尤其是在 AI 公司面临高关注度版权诉讼的背景下。公开现行及历史提示词也能帮助研究人员和用户准确了解当前施加了哪些内容限制。 新规则要求 Claude 不得“整体或部分”再现歌词、诗歌或段落，包括副歌、hook、逐音符写出的旋律，或用户逐句粘贴并声称是自己创作的内容，且在同一对话中必须持续拒绝改写后的请求。允许引用 1929 年前发表的作品，但 Claude 以自己对出版日期的判断为准，而非用户的说法。文档站点支持在任意页面添加 `.md` 后缀以获取 Markdown 格式内容，方便对比提示词差异。

rss · Simon Willison · 9月2日 14:16

**背景**: 系统提示词是开发者预设的隐藏指令，用于定义 AI 助手的规则、人设和限制，终端用户无法自行编辑。Anthropic 的独特之处在于它公开存档 Claude.ai 及移动应用的现行和歷史系统提示词，供任何人对比不同版本之间的变化。新增的歌词限制很可能反映了 AI 再现歌词所引发的版权诉讼和音乐行业的压力。需要注意的是，这些公开提示词并不涵盖 Claude Code 或 Claude Cowork 等代理型工具，它们拥有各自独立的安全体系。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sitespeak.ai/ai-chatbot-terms/system-prompt">System Prompt: How It Shapes an AI Chatbot's Behaviour</a></li>
<li><a href="https://support.claude.com/en/articles/13345190-get-started-with-claude-cowork">Get started with Claude Cowork | Anthropic Help Center</a></li>
<li><a href="https://www.lilachbullock.com/what-are-system-prompts-ai-chatbots/">What Are System Prompts and Why They Matter for AI Chatbots</a></li>

</ul>
</details>

**标签**: `#Claude`, `#system prompts`, `#AI safety`, `#Anthropic`, `#copyright`

---

<a id="item-16"></a>
## [Mol-JEPA：面向分子的多模态 JEPA 基础模型](https://www.reddit.com/r/MachineLearning/comments/1w6i8pr/moljepa_multimodal_molecular_foundation_model_r/) ⭐️ 6.0/10

Mol-JEPA 的作者分享了其研究论文和一个摘要网站，介绍 Mol-JEPA——一种基于 JEPA 的多模态分子基础模型。作者在帖子中欢迎大家提供反馈，并表示该模型在性能上还需要进一步改进。 将 JEPA 应用于分子建模是该架构的一种新颖应用，可能为药物发现和材料设计带来更高效的表征学习。它把 JEPA 范式从图像和视频领域扩展到科学数据领域，但其实际影响仍有待整个研究社区的验证。 Mol-JEPA 是一种整合多种类型分子数据的多模态模型，但帖子中没有具体说明模态的细节。作者在这篇论文上大约花了一年时间，并创建了交互式摘要网站 flogrammer.github.io/moljepa；这是一个 Reddit 上的自发帖，目前还没有外部验证或讨论。

reddit · r/MachineLearning · /u/TerribleAntelope9348 · 9月3日 19:56

**背景**: JEPA（联合嵌入预测架构）是一种由 Yann LeCun 倡导的自监督学习方法，它在潜在空间中预测抽象表征（嵌入），而不是像像素级重建或逐 token 生成那样重建输入数据。这种方法已经被应用于图像、视频、音频等领域，目标是让模型学习世界模型并像人类一样进行推理。Mol-JEPA 将此架构应用于分子数据，旨在学习稳健的分子表征，以支持性质预测、分子生成等任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Joint_Embedding_Predictive_Architecture">Joint Embedding Predictive Architecture</a></li>
<li><a href="https://www.turingpost.com/p/jepamap">All JEPA Models : 14 Milestones From I- JEPA to ThinkJEPA</a></li>

</ul>
</details>

**标签**: `#molecular modeling`, `#JEPA`, `#foundation models`, `#multimodal learning`, `#ML research`

---