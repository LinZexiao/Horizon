---
layout: default
title: "Horizon Summary: 2026-07-08 (ZH)"
date: 2026-07-08
lang: zh
---

> 从 36 条内容中筛选出 24 条重要资讯。

---

1. [欧盟重启私人信息扫描规则，引发隐私争议](#item-1) ⭐️ 9.0/10
2. [LLM 安全护拦在基于 MCP 工具的攻击面前失效](#item-2) ⭐️ 9.0/10
3. [MIRA：专为《火箭联盟》构建的 50 亿参数交互式世界模型](#item-3) ⭐️ 9.0/10
4. [OpenAI 提出通过减少噪声改进编程基准测试](#item-4) ⭐️ 8.0/10
5. [Bun 将运行时从 Zig 重写为 Rust](#item-5) ⭐️ 8.0/10
6. [Mistral 发布 Robostral Navigate：最先进的无地图导航模型](#item-6) ⭐️ 8.0/10
7. [Grok 4.5：xAI 新模型与 GPT 和 Opus 竞争](#item-7) ⭐️ 8.0/10
8. [微软发布 Flint：面向 AI 代理的可视化语言](#item-8) ⭐️ 8.0/10
9. [OpenAI 推出 GPT-Live 语音模式](#item-9) ⭐️ 8.0/10
10. [Cloudflare Meerkat：首个生产级异步共识算法](#item-10) ⭐️ 8.0/10
11. [sqlite-utils 4.0 新增数据库模式迁移功能](#item-11) ⭐️ 8.0/10
12. [腾讯发布 Hy3：295B 参数的 MoE 模型，采用 Apache 2.0 许可](#item-12) ⭐️ 8.0/10
13. [LingBot-Video：开源稀疏 MoE 视频扩散世界模型](#item-13) ⭐️ 8.0/10
14. [可微分光线追踪在无线电传播建模中的博士论文](#item-14) ⭐️ 8.0/10
15. [基于可信 LoRA 子空间的后门攻击防御](#item-15) ⭐️ 8.0/10
16. [Mozilla CTO 关于开源 AI 报告的 AMA](#item-16) ⭐️ 8.0/10
17. [FAANG 模拟器：讽刺游戏揭露科技行业竞逐](#item-17) ⭐️ 7.0/10
18. [Chatto 自托管团队聊天应用现已开源](#item-18) ⭐️ 7.0/10
19. [解码优衣库 T 恤上的混淆 bash 脚本](#item-19) ⭐️ 7.0/10
20. [肯顿·瓦达禁止 AI 撰写变更描述](#item-20) ⭐️ 7.0/10
21. [TorchJD：用于多损失 PyTorch 训练的 Jacobian 下降库](#item-21) ⭐️ 7.0/10
22. [uv 0.11.28 强化 ZIP 处理，升级 GraalPy](#item-22) ⭐️ 6.0/10
23. [Cloudflare Drop 推出拖放式静态网站托管](#item-23) ⭐️ 6.0/10
24. [DINOv2 在细粒度分类的 k-NN 中表现不如 SigLIP](#item-24) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [欧盟重启私人信息扫描规则，引发隐私争议](https://cyberinsider.com/eu-now-one-step-away-from-reviving-private-message-scanning-rules/) ⭐️ 9.0/10

欧盟距离重启“聊天控制”法规仅一步之遥，该法规将要求服务提供商扫描私人信息以查找非法内容，威胁端到端加密。 该立法可能为大规模监控开创先例，削弱加密技术，影响所有欧盟公民的隐私，并可能影响全球数字政策。 该提案区分了“聊天控制 1.0”（自愿扫描）和“聊天控制 2.0”（强制扫描并禁止端到端加密），后者是目前正在审议的更具争议性的版本。

hackernews · ggirelli · 7月8日 16:53 · [社区讨论](https://news.ycombinator.com/item?id=48834296)

**背景**: “聊天控制”法规（正式名称为欧盟 CSA 法规）于 2022 年提出，旨在打击儿童性虐待。它涉及客户端扫描，即在加密前或解密后检查内容。批评者认为它削弱了隐私和加密，是一种大规模监控形式。该法规已争论多年，并不断被重新提出。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control">Chat Control - Wikipedia</a></li>
<li><a href="https://edri.org/our-work/chat-control-what-is-actually-going-on/">Chat Control: What is actually going on? - European Digital ...</a></li>
<li><a href="https://fightchatcontrol.eu/">Fight Chat Control - Protect Digital Privacy in the EU</a></li>

</ul>
</details>

**社区讨论**: 社区表达了强烈担忧，评论指出“聊天控制 2.0”更加危险，因为它强制扫描并禁止端到端加密。用户指出互联网观察基金会正在推动客户端扫描。一些人提供了联系代表以反对该法规的链接，还有一种观点认为，即使被否决，该立法也将不断卷土重来。

**标签**: `#privacy`, `#encryption`, `#EU legislation`, `#surveillance`, `#technology policy`

---

<a id="item-2"></a>
## [LLM 安全护拦在基于 MCP 工具的攻击面前失效](https://www.reddit.com/r/MachineLearning/comments/1ur1fnz/agentic_safety_triggers_arent_textual_safety/) ⭐️ 9.0/10

研究人员表明，当前能检测文本攻击的 LLM 安全护拦在面对通过 MCP 进行的基于工具的攻击时失效，各模型和安全调优方法的拒绝率均低于 50%。 这揭示了在代理系统中 LLM 安全对齐的一个根本缺陷，即攻击嵌入在工具调用序列而非文本中。它动摇了仅凭文本触发就能防护的假设，影响了自主 LLM 代理的部署。 基座模型（1B–14B 参数）对攻击的拒绝率均不超过 35%；最先进的安全调优（DPO、SafeDPO）也仅达到 48%拒绝率。无需训练的方法在无需微调的情况下将基准拒绝率提高了约 3 倍。

reddit · r/MachineLearning · /u/mlsandwich · 7月8日 18:36

**背景**: Model Context Protocol（MCP）由 Anthropic 于 2024 年 11 月推出，它标准化了 LLM 连接外部工具和数据源的方式。传统安全护拦将攻击检测视为文本分类问题，但在具有工具访问权限的代理系统中，恶意意图可以编码在工具调用序列中，而这些序列在文本层面看似无害。本研究利用这一漏洞，通过 MCP 文件 I/O 从已知安全漏洞（CVE）构建攻击，这些攻击仅在工具调用时触发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2305.18290">[2305.18290] Direct Preference Optimization: Your Language ...</a></li>
<li><a href="https://arxiv.org/abs/2505.20065">[2505.20065] SafeDPO: A Simple Approach to Direct Preference ...</a></li>

</ul>
</details>

**标签**: `#LLM safety`, `#agentic systems`, `#MCP`, `#adversarial attacks`, `#AI alignment`

---

<a id="item-3"></a>
## [MIRA：专为《火箭联盟》构建的 50 亿参数交互式世界模型](https://www.reddit.com/r/MachineLearning/comments/1upofuw/mira_multiplayer_interactive_world_models_trained/) ⭐️ 9.0/10

General Intuition、Kyutai 和 Epic Games 联合发布了 MIRA，这是一个在 10,000 小时合成《火箭联盟》数据上训练的 50 亿参数交互式世界模型，能在单个 NVIDIA B200 GPU 上以 20 帧/秒的速度支持四名玩家实时多人推理。 MIRA 代表了交互式世界模型向数十亿参数规模扩展的重大突破，同时保持了实时性能，为游戏 AI、模拟和强化学习研究开辟了新的可能性。 该模型在单个 B200 GPU 上以 20 帧/秒的速度支持四名玩家，团队还发布了可在线体验的演示、技术报告、开源代码仓库以及包含 1000 小时四人游戏数据的数据集。

reddit · r/MachineLearning · /u/MasterScrat · 7月7日 07:59

**背景**: 世界模型是学习模拟环境动态的生成神经网络，常用于强化学习中的规划和决策。本研究将该概念扩展到 50 亿参数，并实现了交互式推理速度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/1803.10122">[1803.10122] World Models - arXiv.org RLVR-World: Training World Models with Reinforcement Learning World Models | RL Journal Club GitHub - thuml/RLVR-World: Official repository for "RLVR ... Deep learning, reinforcement learning, and world models Mastering diverse control tasks through world models - Nature</a></li>
<li><a href="https://www.nvidia.com/en-us/data-center/dgx-b200/">DGX B200: The Foundation for Your AI Factory | NVIDIA</a></li>

</ul>
</details>

**标签**: `#world models`, `#reinforcement learning`, `#large-scale`, `#interactive`, `#open source`

---

<a id="item-4"></a>
## [OpenAI 提出通过减少噪声改进编程基准测试](https://openai.com/index/separating-signal-from-noise-coding-evaluations/) ⭐️ 8.0/10

OpenAI 发布了一份报告，详细介绍了减少编程评估基准中噪声的方法，特别针对不完整或矛盾的任务描述导致结果偏差的问题。 这项工作意义重大，因为嘈杂的基准测试使得准确比较 AI 编程能力变得困难，误导研究人员和从业者。提高基准测试质量有助于更可靠地评估 AI 编程代理，影响开发优先级和部署决策。 分析发现，经过清理后基准测试中只剩下不到 800 个任务，OpenAI 表示这足够少数工程师在一周内手动验证。提出的方法包括任务验证、矛盾检测和结果合理性检查。

hackernews · sk4rekr0w · 7月8日 21:03 · [社区讨论](https://news.ycombinator.com/item?id=48837396)

**背景**: 编程评估基准测试是用于评估 AI 模型在软件工程任务中表现的标准测试。这些基准通常包含数百个任务，但可能因任务描述不佳、需求模糊或隐藏的依赖关系而引入噪声，从而干扰评估结果。

**社区讨论**: 社区评论表达了不同的看法：一些人强调了在 Terminal Bench 2 等基准测试中虚假结果的普遍性，而另一些人提出了测量效率和智能结合的替代基准。一位评论者认为，现实世界的软件任务本质上就是不完整的，因此对这个问题的描述不表示同情；另一位批评了任务数量少以及原始审核的缺失。

**标签**: `#AI evaluation`, `#coding benchmarks`, `#OpenAI`, `#software engineering`

---

<a id="item-5"></a>
## [Bun 将运行时从 Zig 重写为 Rust](https://bun.com/blog/bun-in-rust) ⭐️ 8.0/10

Bun 宣布将其 JavaScript 运行时从 Zig 完全重写为 Rust，使得二进制文件缩小约 20%，性能提升，稳定性增强。 这一迁移凸显了 Rust 在系统编程领域的日益普及，并对 Zig 的竞争力提出了疑问。同时，它也展示了在强大测试套件支持下利用大语言模型进行大规模代码重写的可行性。 此次重写还包括 ICU 变更和相同代码折叠。在 Linux 和 Windows 上，二进制大小减少了约 20%，性能提升了 5%，并修复了内存泄漏。

hackernews · afturner · 7月8日 21:49 · [社区讨论](https://news.ycombinator.com/item?id=48837877)

**背景**: Bun 是一个快速的全能 JavaScript 运行时、包管理器和测试运行器。它最初使用 Zig 编写，Zig 是一种旨在作为 C 语言现代替代品的系统编程语言，以手动内存管理和冗长语法著称。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bun_(software)">Bun (software) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>

</ul>
</details>

**社区讨论**: 评论意见不一：一些人称赞结果是 Rust 的胜利，而另一些人则指出未提供成本明细，并质疑这对 Zig 的长期影响。还有人讨论了 LLM 在此类重写中的作用。

**标签**: `#rust`, `#zig`, `#bun`, `#javascript`, `#systems-programming`

---

<a id="item-6"></a>
## [Mistral 发布 Robostral Navigate：最先进的无地图导航模型](https://mistral.ai/news/robostral-navigate/) ⭐️ 8.0/10

Mistral AI 发布了 Robostral Navigate，这是一个 80 亿参数的模型，仅使用单个 RGB 摄像头和自然语言指令，在 R2R-CE 基准上达到 76.6%的准确率，无需地图、深度传感器或激光雷达。 这标志着向低成本、实用化自主导航迈出了重要一步，使机器人能够以极少的硬件运行，同时达到甚至超过传感器密集系统的性能。它可能使机器人导航技术对爱好者和中小企业更加普及。 该模型有 80 亿参数，在多样化的室内环境数据集上训练；它直接从摄像头输入输出连续的运动指令。目前，Mistral 尚未向公众发布模型权重或推理代码。

hackernews · ottomengis · 7月8日 14:09 · [社区讨论](https://news.ycombinator.com/item?id=48832212)

**背景**: 传统机器人导航通常需要预先构建的地图或深度传感器（如 LiDAR）来确定位置和规划路径。相比之下，无地图导航利用视觉输入动态理解环境，类似于人类的导航方式。R2R-CE（连续房间到房间）基准测试机器人跟随语言指令在新环境中达到连续目标位置的能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mistral.ai/news/robostral-navigate/">Robostral Navigate: single-camera AI navigation | Mistral AI</a></li>
<li><a href="https://alphasignal.ai/news/mistral-s-robostral-navigate-beats-sensor-heavy-robots-with-just-one-camera">Mistral's Robostral Navigate Beats Sensor-Heavy Robots With ...</a></li>
<li><a href="https://www.siliconreport.com/mistral-ai-releases-robostral-navigate-a-single-camera-robotics-model-95dac18d">Mistral AI Releases Robostral Navigate, a Single-Camera ...</a></li>

</ul>
</details>

**社区讨论**: 社区成员称赞了这项技术成就，但对未开放访问表示失望，多人指出若模型发布将有助于业余项目。还有人将其与斯坦福大学的 PIGEON 模型等以往无地图导航研究进行比较，后者也因隐私问题而未公开。

**标签**: `#robotics`, `#navigation`, `#AI`, `#Mistral`, `#map-less`

---

<a id="item-7"></a>
## [Grok 4.5：xAI 新模型与 GPT 和 Opus 竞争](https://x.ai/news/grok-4-5) ⭐️ 8.0/10

xAI 发布了 Grok 4.5 新 AI 模型，在基准测试中与 GPT 和 Claude Opus 相当，尤其在推理效率上表现出色，定价为每百万 tokens $2/$6。 此次发布标志着 xAI 在 AI 前沿竞赛中的重要一步，提供了成本效益高的替代方案。然而，对政治偏见和伦理问题的担忧可能阻碍其在商业和企业环境中的采用。 该模型使用数万亿 tokens 的 Cursor 数据进行训练，捕捉了真实的开发者与代理交互。基准测试显示，其性能与 Opus 4.7 相当，同时推理效率提高了 4 倍。

hackernews · BoumTAC · 7月8日 18:00 · [社区讨论](https://news.ycombinator.com/item?id=48835111)

**背景**: Grok 是 Elon Musk 的 AI 公司 xAI 开发的生成式 AI 聊天机器人，于 2023 年 11 月推出，与 X（原 Twitter）和 Tesla 的 Optimus 机器人集成。Opus 是 Anthropic 的旗舰模型系列，最新版本如 Opus 4.8 在基准测试中得分很高。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Grok_(chatbot)">Grok (chatbot) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/XAI_(company)">xAI (company)</a></li>
<li><a href="https://www.anthropic.com/claude/opus">Claude Opus \ Anthropic</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了怀疑：一些用户因感知到的政治操纵和伦理问题而不信任 xAI，另一些用户则称赞该模型的成本效益和基准性能。一位用户质疑花费数十亿美元获得第三名模型的经济可行性。

**标签**: `#AI`, `#xAI`, `#Grok`, `#ethics`, `#benchmarks`

---

<a id="item-8"></a>
## [微软发布 Flint：面向 AI 代理的可视化语言](https://microsoft.github.io/flint-chart/#/) ⭐️ 8.0/10

微软开源了 Flint，这是一种可视化中间语言（IR），允许 AI 代理通过简单的、高层次的规范生成高质量图表，将底层的视觉决策委托给布局优化引擎。 Flint 直接解决了 AI 生成可视化中的可靠性与质量权衡问题：简单规格无法保证质量，复杂规格对代理而言难以处理。通过提供一个确定性的编译器层，Flint 可以从最简输入中可靠地生成美观图表，改善人机交互的最后一公里。 Flint 支持 46 种图表类型，并以开源项目形式发布在 GitHub 上，同时提供一个 MCP 服务器用于与代理应用集成。它还为微软的 Data Formulator 项目提供支持。

hackernews · chenglong-hn · 7月8日 17:46 · [社区讨论](https://news.ycombinator.com/item?id=48834924)

**背景**: 中间表示（IR）是编译器内部用于表示源代码的数据结构，便于优化和转换。Flint 充当图表规范的编译器：它不要求 AI 代理手动指定每个底层参数（如比例尺、坐标轴和布局），而是以高层语义类型和图表类型为输入，自动推导出优化设置。这减少了冗余和错误，使 AI 代理的图表生成更加可靠。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.microsoft.com/en-us/research/blog/flint-a-visualization-language-for-the-ai-era/">Flint: A visualization language for the AI era - Microsoft ...</a></li>
<li><a href="https://github.com/microsoft/flint-chart">GitHub - microsoft/flint-chart: Flint is a visualization ...</a></li>
<li><a href="https://microsoft.github.io/flint-chart/">Flint: A Visualization Language for the AI Era</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍赞赏这种确定性编译器方法（在代理系统中越来越常见），但也有人质疑 Flint 与 Vega 的区别，以及 LLMs 在使用 Python/R 进行可视化时是否已经表现良好。一位用户指出，简单规格不可靠的说法并不总是适用于小型模型。总体而言，讨论具有建设性，认可 Flint 在降低复杂性方面的价值。

**标签**: `#AI agents`, `#visualization`, `#language design`, `#Microsoft`, `#chart generation`

---

<a id="item-9"></a>
## [OpenAI 推出 GPT-Live 语音模式](https://openai.com/index/introducing-gpt-live/) ⭐️ 8.0/10

OpenAI 推出了 GPT-Live，这是一种面向 ChatGPT 的全新实时语音交互模式，采用全双工音频，并可在后台将复杂查询委托给 GPT-5.5 处理。 这标志着语音 AI 的重大进步，使对话更自然，并消除了以往语音模型的延迟。对于依赖语音助手完成复杂任务的用户来说，这可以提升生产力。 GPT-Live 是一种全双工语音模型，可以同时倾听和说话。它可以无缝地将问题转交给 OpenAI 最先进的 LLM——GPT-5.5，从而处理推理、编程和研究等任务。

hackernews · logickkk1 · 7月8日 17:03 · [社区讨论](https://news.ycombinator.com/item?id=48834405)

**背景**: 传统语音助手以半双工模式运行，一次只有一方说话。GPT-Live 采用全双工，允许自然打断和同时对话。GPT-5.5 是 OpenAI 最新的旗舰模型，以在复杂基准测试中的强劲表现著称。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deploymentsafety.openai.com/gpt-live">GPT-Live System Card - OpenAI Deployment Safety Hub</a></li>
<li><a href="https://venturebeat.com/technology/openai-launches-gpt-live-a-full-duplex-voice-upgrade-that-lets-chatgpt-talk-more-like-a-person">OpenAI launches GPT-Live, a full-duplex voice upgrade that ...</a></li>
<li><a href="https://openai.com/index/introducing-gpt-5-5/">Introducing GPT‑5.5 - OpenAI</a></li>

</ul>
</details>

**社区讨论**: 早期预览用户 simonw 称赞了 GPT-Live 委托给 GPT-5.5 的能力，但其他人提出了担忧：jonstaab 警告 AI 不要取代人际互动，artdigital 对语音模式缺乏工具集成表示遗憾，NikolaNovak 则更偏好结构化、不冗长的回答。

**标签**: `#GPT-Live`, `#OpenAI`, `#voice AI`, `#real-time`, `#AI assistants`

---

<a id="item-10"></a>
## [Cloudflare Meerkat：首个生产级异步共识算法](https://blog.cloudflare.com/meerkat-introduction/) ⭐️ 8.0/10

Cloudflare 推出了 Meerkat，这是一种全球分布式共识算法，是 QuePaxa 的首个生产级实现，QuePaxa 是一种无需超时、使用对冲延迟的异步共识算法。 这意义重大，因为它证明了异步共识在生产中的可行性，可能提高在可变网络条件下的容错性和性能，这对广域分布式系统至关重要。 Meerkat 使用 QuePaxa 的对冲调度动态确定提议者优先级，无需依赖超时，并将读取操作纳入全局共识，这可能会增加延迟。该系统尚未投入生产，目前是一个实验项目。

hackernews · bobnamob · 7月8日 13:18 · [社区讨论](https://news.ycombinator.com/item?id=48831565)

**背景**: Paxos 和 Raft 等共识算法是部分同步的，依赖超时来推进。在异步网络中，消息延迟可能无限大，使得共识更难。QuePaxa 是一种异步算法，使用随机性和对冲来避免超时，即使在严重网络延迟下也能保证进展。这是该算法的首个生产级实现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.cloudflare.com/meerkat-introduction/">Introducing Meerkat: an experiment in global consensus</a></li>
<li><a href="https://bford.info/pub/os/quepaxa/quepaxa.pdf">QuePaxa: Escaping the Tyranny of Timeouts in Consensus QuePaxa: Escaping the Tyranny of Timeouts in Consensus Robust and High-Performance Wide-Area Consensus Protocols QuePaxa: Escaping the tyranny of timeouts in consensus PasinduTennage/quepaxa-fork-for-internal - GitHub</a></li>

</ul>
</details>

**社区讨论**: 一些评论者指出，将 Meerkat 与 Raft 比较为无领导者会误导，因为 Raft 是基于领导者的，但他们承认避免超时的好处。其他人指出，将读取纳入全局共识可能导致高读取延迟，限制了使用场景。然而，许多人对在复杂网络中稳健运行的潜力表示赞赏。

**标签**: `#distributed-systems`, `#consensus`, `#cloudflare`, `#paxos`, `#raft`

---

<a id="item-11"></a>
## [sqlite-utils 4.0 新增数据库模式迁移功能](https://simonwillison.net/2026/Jul/7/sqlite-utils-4/#atom-everything) ⭐️ 8.0/10

sqlite-utils 4.0 于 2026 年 7 月 7 日发布，引入了三大主要功能：数据库模式迁移、通过新的 db.atomic() 方法实现的嵌套事务，以及对复合外键的支持。 此版本通过提供内置的迁移框架，解决了 SQLite 开发者长期以来的痛点，减少了对外部工具的依赖。同时增强了事务控制和关系完整性，使 sqlite-utils 更适合复杂应用。 迁移使用 Python 文件中的 Migrations 类和强大的 table.transform() 方法定义，该方法实现了 SQLite 推荐的新建表、复制数据、重命名模式。此版本包含破坏性变更，具体见升级指南。

rss · Simon Willison · 7月7日 19:32

**背景**: sqlite-utils 是一个用于操作 SQLite 数据库的 Python 库和命令行工具。数据库模式迁移允许开发者随时间演变数据库结构；此前 sqlite-utils 缺乏内置迁移支持，用户需依赖其他工具。嵌套事务可在更大事务中实现原子性，复合外键则允许引用其他表的多列主键。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Composite_key">Composite key - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Nested_transaction">Nested transaction</a></li>

</ul>
</details>

**标签**: `#sqlite`, `#python`, `#database-migrations`, `#tooling`

---

<a id="item-12"></a>
## [腾讯发布 Hy3：295B 参数的 MoE 模型，采用 Apache 2.0 许可](https://simonwillison.net/2026/Jul/6/hy3/#atom-everything) ⭐️ 8.0/10

腾讯发布了 Hy3，一个 2950 亿参数的混合专家（MoE）模型，其中 210 亿参数被激活，并包含 38 亿参数的 MTP 层。该模型在性能上超越同等规模模型，并能与参数规模大 2-5 倍的旗舰开源模型相抗衡，目前可在 OpenRouter 上免费试用至 7 月 21 日。 此次发布意义重大，因为它来自中国一家大型企业，以宽松的 Apache 2.0 许可协议发布了一个极具竞争力的开源模型，有望推动 AI 社区的更广泛采用和创新。这也表明混合专家架构能够在较低计算成本下实现强大的性能，对更大的密集模型构成挑战。 全精度模型检查点大小为 598GB，FP8 量化版本为 300GB，上下文长度达 256,000 个词元。该模型采用了多词元预测（MTP）层以提升推理速度，并在收集了 50 多个产品的反馈后，使用更高质量的数据扩大了后训练规模。

rss · Simon Willison · 7月6日 23:57

**背景**: 混合专家（MoE）是一种神经网络架构，它将模型划分为多个'专家'子网络，每次只激活其中一部分，从而在保持总参数量较大的同时控制计算成本。多词元预测（MTP）技术让模型在一次前向传播中预测多个未来词元，从而加速推理。FP8 量化将模型权重的精度降至 8 位浮点数，大幅减少内存使用并提升推理速度，而准确率损失极小。Apache 2.0 是一种宽松的开源许可证，允许自由使用、修改和分发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@bingqian/understanding-multi-token-prediction-mtp-in-deepseek-v3-ed634810c290">Understanding Multi-Token Prediction (MTP) in DeepSeek-V3 | by Bing | Medium</a></li>
<li><a href="https://arxiv.org/abs/2208.09225">[2208.09225] FP8 Quantization: The Power of the Exponent</a></li>

</ul>
</details>

**标签**: `#AI`, `#Machine Learning`, `#Open Source`, `#Large Language Model`, `#Tencent`

---

<a id="item-13"></a>
## [LingBot-Video：开源稀疏 MoE 视频扩散世界模型](https://www.reddit.com/r/MachineLearning/comments/1ur0bxq/lingbotvideo_sparsemoe_video_diffusion/) ⭐️ 8.0/10

LingBot-Video 是一个开源稀疏混合专家视频扩散变压器，总参数 13B（活跃参数 1.4B），通过六奖励强化学习后训练成为动作条件世界模型，其中包括一个由 VLM 评分的物理合理性奖励。它支持从动作预测机器人展开视频，在 RBench 上取得平均最高分。 这项工作通过以动作条件为基础并使用基于 VLM 的奖励来强制物理合理性，将视频扩散模型推向真实世界机器人规划的边界，引发了关于视频生成与世界模型界限的重要问题。其开源发布使更广泛的社区能够进行实验和批评。 该模型在单流扩散变压器中使用类似 DeepSeek-V3 的稀疏 MoE，包含 128 个专家（top-8 路由，1.4B 活跃），通过六项奖励训练：文本-视频对齐、美学、视频流畅度、主体一致性、背景一致性和物理合理性（由 VLM 对采样帧评分）。结果在 RBench 上取得平均最高，但在通用文本到视频任务中仅排名第二；未提供闭环机器人评估。

reddit · r/MachineLearning · /u/Savings-Display5123 · 7月8日 17:58

**背景**: 稀疏混合专家是一种神经架构，每次输入只激活一部分专家子网络，从而在不成比例增加计算成本的情况下实现更大的总参数量。视频扩散变压器将 transformer 架构与扩散模型结合用于视频生成。动作条件世界模型旨在根据动作序列预测未来视频帧，充当机器人策略评估或规划的模拟器。使用 VLM 评分物理合理性是一种新颖方法，存在奖励黑客风险，虽然作者添加了真实视频负例作为对策。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2305.13311">[2305.13311] VDT: General-purpose Video Diffusion ... GitHub - RERV/VDT: [ICLR2024] The official implementation of ... GitHub - showlab/Awesome-Video-Diffusion: A curated list of ... [2509.09547] Improving Video Diffusion Transformer Training ... VDT: General-purpose Video Diffusion Transformers via Mask ... DiTVR: Zero-Shot Diffusion Transformer for Video Restoration VDT: G PURPOSE VIDEO DIFFUSION TRANS FORMERS VIA MODELING</a></li>
<li><a href="https://liralab.usc.edu/pdfs/publications/wang2024rlvlmf.pdf">RL-VLM-F: Reinforcement Learning from Vision Language Foundation Model Feedback</a></li>

</ul>
</details>

**社区讨论**: 社区讨论提出了两个关键点：VLM 是否能够可靠地评判物理合理性（存在古德哈特定律/奖励黑客的风险），以及该模型是真正的世界模型还是仅仅是视频生成器，因为没有提供闭环机器人评估结果。该模型在 RBench 上取得平均最高，但推理密集型维度仍由闭源模型主导，并且在其自身评估中仅在通用文本到视频任务中排名第二。

**标签**: `#sparse-MoE`, `#video diffusion`, `#world model`, `#reinforcement learning`, `#robotics`

---

<a id="item-14"></a>
## [可微分光线追踪在无线电传播建模中的博士论文](https://www.reddit.com/r/MachineLearning/comments/1upvkp5/phd_thesis_on_differentiable_ray_tracing_for/) ⭐️ 8.0/10

一篇新发表的博士论文提出了用于无线电传播建模的可微分光线追踪方法，利用 JAX 进行自动微分，通过物理环境计算梯度，从而支持逆问题和机器学习训练。 这项工作将无线电传播模拟与机器学习联系起来，提供了一本教科书式的资源，可加速下一代无线网络设计，例如信道建模和材料校准。 论文以自包含教科书形式撰写，分为三部分：物理基础、带有不连续性平滑的 GPU 加速路径追踪，以及包括 ML 辅助生成路径采样在内的实际应用。它基于 Equinox 和 optimistix 等 JAX 库构建。

reddit · r/MachineLearning · /u/jeertmans · 7月7日 13:45

**背景**: 无线电传播建模模拟无线电波在环境中的传播，这对无线网络规划至关重要。光线追踪是一种常用技术，但传统光线追踪不可微分。通过引入自动微分，可微分光线追踪可以计算模拟输出相对于参数（如材料属性、天线位置）的梯度，从而支持基于梯度的优化和机器学习集成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2303.11103">[2303.11103] Sionna RT: Differentiable Ray Tracing for Radio Propagation Modeling</a></li>
<li><a href="https://research.nvidia.com/publication/2023-12_sionna-rt-differentiable-ray-tracing-radio-propagation-modeling">Sionna RT: Differentiable Ray Tracing for Radio Propagation Modeling | Research</a></li>
<li><a href="https://docs.jax.dev/en/latest/automatic-differentiation.html">Automatic differentiation — JAX documentation</a></li>

</ul>
</details>

**标签**: `#differentiable ray tracing`, `#radio propagation`, `#automatic differentiation`, `#JAX`, `#wireless communications`

---

<a id="item-15"></a>
## [基于可信 LoRA 子空间的后门攻击防御](https://www.reddit.com/r/MachineLearning/comments/1uq68li/what_if_a_model_could_only_learn_what_trusted/) ⭐️ 8.0/10

一篇新论文提出了 Z-Manifold 方法，通过将微调更新限制在可信 LoRA 适配器张成的子空间中，使恶意更新在几何上不可达。该方法大幅降低了攻击成功率，同时保留了适配器池覆盖任务上的有用适应能力。 这引入了一种针对微调后门攻击的新型几何防御范式，从检测转向预防。它可以在敏感应用（如设备端助手）或基于用户生成数据训练时保护微调模型。 该方法在 196 个公开 LoRA 适配器上进行了测试，包括专门绕过防御的自适应攻击，在保持有用适应的同时大幅降低了攻击成功率。该方法无需检测恶意数据，而是限制可能的更新空间。

reddit · r/MachineLearning · /u/Bright_Warning_8406 · 7月7日 20:00

**背景**: LoRA（低秩适应）是一种流行的参数高效微调技术，它将低秩矩阵注入预训练模型层。微调过程中的后门攻击可以插入隐藏触发器，导致恶意行为。Z-Manifold 利用一个可信 LoRA 适配器池来定义一个安全的更新子空间，从几何上阻止模型学习某些恶意方向。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LoRA_(machine_learning)">LoRA (machine learning) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#fine-tuning`, `#LoRA`, `#adversarial ML`, `#security`, `#machine learning`

---

<a id="item-16"></a>
## [Mozilla CTO 关于开源 AI 报告的 AMA](https://www.reddit.com/r/MachineLearning/comments/1upxdvc/raffi_krikorian_cto_mozilla_ama_on_the_state_of/) ⭐️ 8.0/10

7 月 14 日，Mozilla 首席技术官 Raffi Krikorian 将在 Reddit 主持 AMA，讨论首份《开源 AI 现状》报告，该报告审视了实际成本、企业采用、中国模型和开发者信任。 此次 AMA 提供了来自重要组织的新见解，揭示了隐藏成本和生态系统动态，挑战了关于开源 AI 免费且无障碍的传统叙事。 报告引入了'免费模型的隐性成本'、'中国效应'（即能力强大的中国模型）和'代理框架'（agentic harness）作为新战场等概念。Krikorian 还将讨论 2026 年'开源 AI'应有的含义。

reddit · r/MachineLearning · /u/raffikrikorian · 7月7日 14:51

**背景**: 《开源 AI 现状》是 Mozilla 发布的首份年度报告，评估开源 AI 在生产中的实际使用情况。'代理框架'（agentic harness）指围绕语言模型的软件基础设施（如工具、记忆、沙盒），将模型转变为代理。'免费'开源模型的隐藏成本包括部署、维护和计算资源，可能超出预期。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.langchain.com/blog/the-anatomy-of-an-agent-harness">The Anatomy of an Agent Harness</a></li>
<li><a href="https://hub.stabilarity.com/cost-effective-ai-the-hidden-costs-of-free-open-source-ai-what-nobody-tells-you/">Cost-Effective AI: The Hidden Costs of "Free" Open Source AI ...</a></li>
<li><a href="https://www.archyde.com/open-source-ai-costs-hidden-compute-expenses/">Open-Source AI Costs: Hidden Compute Expenses - Archyde</a></li>

</ul>
</details>

**标签**: `#open source AI`, `#Mozilla`, `#AI industry`, `#developer trust`, `#enterprise AI`

---

<a id="item-17"></a>
## [FAANG 模拟器：讽刺游戏揭露科技行业竞逐](https://www.abeyk.com/escape-the-rat-race/) ⭐️ 7.0/10

一款名为“FAANG 模拟器”的讽刺性浏览器游戏发布，让玩家体验大型科技公司高压的职业竞逐。 该游戏以幽默而批判的视角揭示了 FAANG 就业的现实，引发了关于年龄歧视、移民身份和副业文化的讨论。 玩家可以通过低成本生活或做不可扩展的工作来破解游戏，但游戏未考虑年龄歧视；也缺少针对非美国公民面临签证限制的模式。

hackernews · nerdbiscuits · 7月8日 20:05 · [社区讨论](https://news.ycombinator.com/item?id=48836778)

**背景**: FAANG 是 Facebook、Apple、Amazon、Netflix 和 Google 的缩写，代表硅谷顶尖科技公司。“rat race”指员工为晋升、奖金和工作保障而激烈竞争，常需要长时间工作和做副业。

**社区讨论**: 评论者称赞游戏的现实感，但也指出缺少年龄歧视和移民挑战等元素。有人分享了击败系统的策略，也有人批评游戏过度奖励副业而不考虑其难度。

**标签**: `#FAANG`, `#simulation`, `#tech culture`, `#career`, `#satire`

---

<a id="item-18"></a>
## [Chatto 自托管团队聊天应用现已开源](https://www.hmans.dev/blog/chatto-is-open-source) ⭐️ 7.0/10

Chatto 是一款自托管团队聊天应用，内置视频通话和基于 NATS 的消息系统，现已以 Apache-2.0 许可证开源发布。 这为 Slack 和 Mattermost 等专有团队聊天平台提供了一个注重隐私、可自托管的替代方案，部署简便且支持每用户加密密钥。 Chatto 以紧凑的自包含二进制文件形式发布，使用 NATS 进行消息传递，并可选择支持外部 S3 兼容对象存储；在账户删除时会销毁每用户密钥。

hackernews · speckx · 7月8日 15:19 · [社区讨论](https://news.ycombinator.com/item?id=48833116)

**背景**: NATS 是云原生计算基金会下的轻量级高性能消息系统，专为现代分布式系统设计。Slack 和 Mattermost 等团队聊天应用广泛使用，但通常需要集中式基础设施或复杂的自托管；Chatto 旨在通过包含服务器和 NATS 的单一二进制文件来简化这一过程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.hmans.dev/blog/chatto-is-open-source">Chatto is now Open Source!</a></li>
<li><a href="https://en.wikipedia.org/wiki/NATS_Messaging">NATS Messaging - Wikipedia</a></li>
<li><a href="https://nats.io/">NATS.io – Cloud Native, Open Source, High-performance Messaging</a></li>

</ul>
</details>

**社区讨论**: 社区反应积极，称赞其易于自托管和隐私保护功能。一位评论者指出“chato”在葡萄牙语中意为“无聊”，希望有更多这样“无聊”的软件。另一位指出企业环境中需要软删除功能，还有用户提到开发者利用智能体编码独自构建了该项目。

**标签**: `#open-source`, `#team-chat`, `#self-hosting`, `#NATS`, `#privacy`

---

<a id="item-19"></a>
## [解码优衣库 T 恤上的混淆 bash 脚本](https://tris.sherliker.net/blog/obfuscated-self-evaluating-bash-script-by-cdn-akamai-being-supplied-to-consumers-via-retail-stores/) ⭐️ 7.0/10

对优衣库 T 恤上印刷的混淆 bash 脚本的详细分析揭示了它如何利用自求值代码和反 OCR 技术。 这项分析突显了编程文化与时尚的交集，引发了社区对混淆技术和 OCR 挑战的兴趣。 该脚本因故意的排版不规则而难以被 OCR 识别，它是优衣库与 Akamai 合作的一部分，该合作还包括一款不完整的 T 恤设计。

hackernews · speerer · 7月8日 08:46 · [社区讨论](https://news.ycombinator.com/item?id=48829312)

**背景**: Bash 混淆旨在保持功能的同时使脚本代码难以阅读，常用于红队行动或防检测。像 Bashfuscator 这样的工具可以自动化这一过程，产生高度复杂的脚本，但仍能正确执行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/Bashfuscator/Bashfuscator">GitHub - Bashfuscator/Bashfuscator: A fully configurable and ...</a></li>
<li><a href="https://www.baeldung.com/linux/bash-obfuscate-script">How to Obfuscate a Bash Script to Make It Unreadable - Baeldung</a></li>
<li><a href="https://github.com/FajarKim/blind-bash">GitHub - FajarKim/blind-bash: Tools for obfuscated bash ...</a></li>

</ul>
</details>

**社区讨论**: 评论者指出了 OCR 难度，并分享了设计师解释故意反 OCR 措施的视频。有人开玩笑说因为语法错误要退 T 恤，而其他人则欣赏其类 quine 的特性，并引用了相关的 ASCII 艺术项目。

**标签**: `#bash`, `#obfuscation`, `#programming`, `#culture`, `#hacker news`

---

<a id="item-20"></a>
## [肯顿·瓦达禁止 AI 撰写变更描述](https://simonwillison.net/2026/Jul/8/kenton-varda/#atom-everything) ⭐️ 7.0/10

Cap'n Proto 和 Sandstorm 的创始人肯顿·瓦达宣布，他的团队禁止使用 AI 编写的变更描述，理由是其遗漏了代码审查所需的高层次上下文。 这突出了当前 AI 辅助编程的一个关键局限性：AI 可以生成详细的代码摘要，但往往无法提供人类审查者所需的战略意图或设计理由，引发了关于在软件开发中使用 AI 最佳实践的讨论。 瓦达特别指出，AI 编写的描述“概述了代码中通过直接查看代码就能轻易看到的细节，但遗漏了理解代码大体功能所需的高层次框架。

rss · Simon Willison · 7月8日 20:03

**背景**: 在软件开发中，变更描述（如提交信息和 PR 描述）对于代码审查至关重要，帮助审查者理解变更的目的和背景。像大型语言模型这样的 AI 工具越来越被用于生成这些描述，但它们可能产生技术上准确但缺乏战略洞察的文本。

**标签**: `#kenton-varda`, `#ai-assisted-programming`, `#generative-ai`, `#ai`, `#llms`

---

<a id="item-21"></a>
## [TorchJD：用于多损失 PyTorch 训练的 Jacobian 下降库](https://www.reddit.com/r/MachineLearning/comments/1upzxk2/torchjd_training_with_multiple_losses_in_pytorch_p/) ⭐️ 7.0/10

TorchJD 是一个新的 PyTorch 库，实现了用于多损失训练的 Jacobian 下降方法，并已被 PyTorch 生态系统接纳。它提供了文献中多种聚合器，涵盖标量化和 Jacobian 下降两种方法。 该库通过提供多种损失聚合方法的统一接口，简化了 PyTorch 中的多任务学习和多目标优化。它使实践者能够轻松在标量化和 Jacobian 下降之间切换，在目标冲突时可能提升性能。 TorchJD 扩展了 PyTorch 的 autograd，用于计算向量值损失函数的 Jacobian 矩阵，然后使用选定的方法聚合梯度。该库包含经典标量化技术和先进的 Jacobian 下降聚合器，如 MGDA 和 PCGrad。

reddit · r/MachineLearning · /u/Skeylos2 · 7月7日 16:20

**背景**: 在多损失训练中，标量化将多个损失项组合成一个标量损失（例如加权和）并应用标准梯度下降。Jacobian 下降则分别计算每个损失的梯度，然后聚合为能同时降低所有损失的更新向量。TorchJD 提供了这些 Jacobian 下降方法的便捷实现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/TorchJD/torchjd">GitHub - SimplexLab/TorchJD: Library for Jacobian descent with PyTorch. It enables the optimization of neural networks with multiple losses (e.g. multi-task learning). · GitHub</a></li>
<li><a href="https://arxiv.org/abs/2406.16232">[2406.16232] Jacobian Descent for Multi-Objective Optimization</a></li>

</ul>
</details>

**标签**: `#PyTorch`, `#multi-task learning`, `#Jacobian descent`, `#loss aggregation`

---

<a id="item-22"></a>
## [uv 0.11.28 强化 ZIP 处理，升级 GraalPy](https://github.com/astral-sh/uv/releases/tag/0.11.28) ⭐️ 6.0/10

uv 0.11.28 将其 ZIP 库更新至 v0.0.20，增强了对解析器差异的防护，并将 GraalPy 升级至 25.1.3。同时包含大量性能优化和小幅改进。 此版本解决了一类安全问题：多个解析器对 ZIP 文件的解释可能不同，从而允许恶意存档绕过检查。此次强化保护了 uv（一款快速的 Python 包管理器）用户免受此类攻击。 更新后的库 astral-async-zip v0.0.20 包含 15 项更改，使 uv 拒绝此前接受的格式错误或有歧义的 ZIP 存档。GraalPy 升级带来了对 Python 3.12 的兼容性和性能改进。

github · github-actions[bot] · 7月7日 23:14

**背景**: 解析器差异发生在不同软件组件对同一数据结构产生不同解读时，攻击者可利用此绕过安全检查。在 ZIP 存档中，一个文件可能有多个同名条目；如果某个解析器读取一个条目而另一个解析器读取另一个，恶意存档可能通过验证却提取有害内容。GraalPy 是基于 JVM 的高性能 Python 实现，提供 JIT 编译和原生二进制支持。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://iterasec.com/blog/understanding-parser-differential-vulnerabilities/">Parser Differential Vulnerabilities Explained | Iterasec</a></li>
<li><a href="https://github.com/astral-sh/uv/security/advisories/GHSA-8qf3-x8v5-2pj8">ZIP payload obfuscation through parsing differentials - uv</a></li>
<li><a href="https://github.com/oracle/graalpython">GitHub - oracle/graalpython: GraalPy – A high-performance ...</a></li>

</ul>
</details>

**标签**: `#uv`, `#security`, `#package manager`, `#Python`, `#GraalPy`

---

<a id="item-23"></a>
## [Cloudflare Drop 推出拖放式静态网站托管](https://www.cloudflare.com/drop/) ⭐️ 6.0/10

Cloudflare Drop 允许用户通过将文件夹或 ZIP 文件拖入浏览器来部署静态网站，预览一小时后可认领以保留部署，全程无需注册账户。 该服务极大简化了静态网站部署流程，降低了初学者门槛，有望推动更多用户采用 Cloudflare 的边缘网络进行托管，并与 Netlify Drop 等类似服务形成直接竞争。 部署后立即在 Cloudflare 的全球网络可用，网站覆盖世界 95% 联网人口，延迟约 32 毫秒。一小时的预览期是临时的，除非认领，且仅支持静态内容（HTML、CSS、JS、图片）。

hackernews · coloneltcb · 7月8日 19:18 · [社区讨论](https://news.ycombinator.com/item?id=48836233)

**背景**: 传统静态网站托管通常需要注册账户、使用命令行工具或配置 CI/CD 流水线。Cloudflare Drop 通过提供无需账户的即时预览消除了这些障碍，类似于大约十年前率先采用拖放方式的 Netlify Drop。Cloudflare 此前已提供 Workers 和 Pages 托管服务，但 Drop 面向更简单的一次性或实验性部署。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cloudflare.com/drop/">Cloudflare Drop</a></li>
<li><a href="https://developers.cloudflare.com/changelog/post/2026-07-08-cloudflare-drag-and-drop/">Changelog - Cloudflare Drop</a></li>
<li><a href="https://x.com/braydenwilmoth/status/2074894829616509358">Introducing Cloudflare Drop Drop your folder in the browser ...</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：有人称赞其易用性和快速分享的潜力，也有人指出这并非创新，因为 Netlify Drop 多年前就已实现。有评论担忧被滥用于托管恶意内容，但部分人认为安全风险没有显著变化，因为免费 Cloudflare 账户已经允许类似部署。

**标签**: `#cloudflare`, `#hosting`, `#static sites`, `#deployment`, `#web development`

---

<a id="item-24"></a>
## [DINOv2 在细粒度分类的 k-NN 中表现不如 SigLIP](https://www.reddit.com/r/MachineLearning/comments/1uqtamz/dinov2_way_worse_than_siglip_in_knn_is_this/) ⭐️ 6.0/10

一位用户报告说，在细粒度汽车数据集上，SigLIP2 SO400M 在 k-NN 中达到约 92%的准确率，而 DINOv2 Giant 仅达到约 41%，尽管两者都使用了 L2 归一化嵌入。 这一实证比较突出了 DINOv2 在没有训练分类器的情况下用于检索任务的实际局限性，并表明自监督视觉 Transformer 可能不直接适用于细粒度的 k-NN 分类。 该数据集很小（175 张训练，132 张测试），用于细粒度汽车分类（大众高尔夫世代）。用户尝试了 L2 归一化嵌入下的余弦和欧几里得距离，但 DINOv2 仍为 41%，而 SigLIP 为 92%，CLIP ViT-L 为 59%。

reddit · r/MachineLearning · /u/psy_com · 7月8日 13:51

**背景**: DINOv2 是一种自监督学习方法，不需要标注数据；它通过预测图像视图来学习视觉特征。SigLIP 使用对比损失（sigmoid 损失）将图像和文本在共享嵌入空间中对齐，使其自然适用于基于相似性的检索。在 k-NN 分类中，不进行微调——直接比较嵌入，因此嵌入空间的结构至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ai.meta.com/blog/dino-v2-computer-vision-self-supervised-learning/">DINOv2: State-of-the-art computer vision models with self-supervised learning</a></li>
<li><a href="https://blog.ritwikraha.dev/choosing-between-siglip-and-clip-for-language-image-pretraining">CLIP to SigLIP: Vision-Language Models with Contrastive Learning</a></li>
<li><a href="https://github.com/facebookresearch/dinov2">GitHub - facebookresearch/dinov2: PyTorch code and models for the DINOv2 self-supervised learning method. · GitHub</a></li>

</ul>
</details>

**标签**: `#computer vision`, `#representation learning`, `#self-supervised learning`, `#fine-grained classification`

---