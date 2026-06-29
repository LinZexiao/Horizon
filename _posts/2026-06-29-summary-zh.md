---
layout: default
title: "Horizon Summary: 2026-06-29 (ZH)"
date: 2026-06-29
lang: zh
---

> 从 28 条内容中筛选出 15 条重要资讯。

---

1. [美最高法院：地理围栏搜查令受第四修正案约束](#item-1) ⭐️ 9.0/10
2. [谷歌 AI 同行评审系统处理 1 万篇论文，错误捕获率提高 34%](#item-2) ⭐️ 9.0/10
3. [Rocket Lab 战略收购 Iridium](#item-3) ⭐️ 8.0/10
4. [Game Boy 模拟器 JIT 编译为 WASM，超越原生解释器](#item-4) ⭐️ 8.0/10
5. [深入解析从 CPU 到 GPU 的 CUDA 内核启动路径](#item-5) ⭐️ 8.0/10
6. [Cerebras 与 OpenAI 交易封锁 AI 初创公司推理访问](#item-6) ⭐️ 8.0/10
7. [EML 树被证明是通用逼近器](#item-7) ⭐️ 8.0/10
8. [HEMA 实践者构建开放数据集以改进 AI 剑术追踪](#item-8) ⭐️ 8.0/10
9. [可编辑权重的交互式微型 Transformer 可视化](#item-9) ⭐️ 8.0/10
10. [.self 顶级域名提案旨在赋能自托管用户](#item-10) ⭐️ 7.0/10
11. [Qwen 3.6 27B：本地开发的甜蜜点？](#item-11) ⭐️ 7.0/10
12. [Ornith-1.0：用于智能编程的开源自脚手架大模型](#item-12) ⭐️ 7.0/10
13. [Jon Udell 翻转叙事：智能体是团队成员，而非黑箱](#item-13) ⭐️ 7.0/10
14. [黑客你的夏天：面向学生的免费四周冲刺项目](#item-14) ⭐️ 6.0/10
15. [基于性格的 LLM 匹配测试上线](#item-15) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [美最高法院：地理围栏搜查令受第四修正案约束](https://www.theguardian.com/us-news/2026/jun/29/supreme-court-geofence-warrants-case-decision) ⭐️ 9.0/10

美国最高法院于 2026 年 6 月 29 日裁定，地理围栏搜查令必须依据第四修正案获得基于可能原因签发的搜查令，极大限制了执法机构在缺乏宪法保护下获取位置数据的能力。 这一里程碑裁决通过防止大规模无证位置数据搜查，保护了数百万人的数字隐私，并为法院如何处理数字时代的反向搜查令树立了关键先例。 该案涉及一名通过谷歌 Sensorvault（存储历史地理位置数据）识别的银行抢劫嫌疑人；法院裁定必须基于可能原因获得搜查令，拒绝了较低标准。

hackernews · cdrnsf · 6月29日 15:54 · [社区讨论](https://news.ycombinator.com/item?id=48720924)

**背景**: 地理围栏搜查令允许执法机构向谷歌等科技公司请求特定时间段内虚拟边界内所有设备的位置数据。批评者认为这些搜查令因搜集无辜者数据而违反第四修正案。此次裁决明确了此类搜查令需要宪法保护，解决了地理围栏技术使用引发的隐私担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Geofence_warrant">Geofence warrant</a></li>

</ul>
</details>

**社区讨论**: 评论者强烈支持该裁决，一些人指出阿利托和托马斯大法官持异议，并赞扬巴雷特大法官加入多数意见。其他人讨论了该裁决对 Flock 车牌读取器等技术的影响，质疑其是否现在也需要搜查令。一名评论者分享了一个历史案例，说明如何通过 IP 地理定位和酒店记录识别未携带手机的嫌疑人。

**标签**: `#privacy`, `#supreme court`, `#geofence`, `#digital rights`, `#law enforcement`

---

<a id="item-2"></a>
## [谷歌 AI 同行评审系统处理 1 万篇论文，错误捕获率提高 34%](https://www.reddit.com/r/MachineLearning/comments/1uio9rb/googles_agentic_peerreviewer_handled_10k_papers/) ⭐️ 9.0/10

谷歌在 ICML 和 STOC 会议上部署了代理型 AI 同行评审系统，处理了约 1 万篇论文，周转时间 30 分钟，正式论文显示其数学错误捕获率比零样本提示高出 34%。 这一部署为会议规模下的 AI 自动化科学评审开创了先例，可能加速同行评审并减轻评审员负担。 该系统在检测数学错误方面比零样本提示提升 34%，正式研究已发表在 arXiv 上（2606.28277）。

reddit · r/MachineLearning · /u/Justgototheeffinmoon · 6月29日 10:05

**背景**: 代理型 AI 评审器使用 LLM 代理模拟会议同行评审的若干环节，阅读论文并生成结构化评论。谷歌的系统部署在两个顶级 CS 会议（ICML 和 STOC）上，以快速周转评审数千篇论文。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/data-science-in-your-pocket/andrew-ngs-agentic-reviewer-ai-for-research-paper-reviews-1c2d9cda8086">Andrew NG’s Agentic Reviewer : AI for Research Paper Reviews</a></li>
<li><a href="https://rcgsheffield.github.io/research-ai-landscape/tools/stanford-agentic-reviewer">stanford-agentic-reviewer</a></li>

</ul>
</details>

**标签**: `#AI-assisted peer review`, `#scientific review`, `#conference automation`, `#LLM agents`, `#machine learning`

---

<a id="item-3"></a>
## [Rocket Lab 战略收购 Iridium](https://investors.rocketlabcorp.com/news-releases/news-release-details/rocket-lab-acquire-iridium-historic-deal-creating-fully) ⭐️ 8.0/10

Rocket Lab 宣布收购 Iridium，从而获得 Iridium 的频谱资产、盈利的卫星业务以及稳定的发射管道。该交易预计在 2025 年完成。 此次收购标志着航天行业的一次重大整合，将发射服务提供商与卫星运营商结合在一起。它可能使 Rocket Lab 获得稳定发射量并拓展卫星服务，有可能挑战 SpaceX 的主导地位。 Rocket Lab 将收购 Iridium 的卫星星座、频谱许可证以及地面基础设施。该交易为 Rocket Lab 的 Neutron 火箭提供了稳定客户，并注入盈利的卫星制造业务。

hackernews · everfrustrated · 6月29日 14:09 · [社区讨论](https://news.ycombinator.com/item?id=48719485)

**背景**: Iridium 运营着一个低地球轨道卫星星座，提供全球语音和数据通信。频谱资产对于卫星通信至关重要，因为频谱资源有限且受国家监管。Rocket Lab 是一家以 Electron 火箭闻名的发射服务提供商，目前正在开发更大的 Neutron 火箭。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Orbit_spectrum">Orbit spectrum - Wikipedia</a></li>
<li><a href="https://www.federalregister.gov/documents/2025/06/27/2025-11966/satellite-spectrum-abundance">Federal Register :: Satellite Spectrum Abundance</a></li>

</ul>
</details>

**社区讨论**: 评论者认为这笔交易类似于 SpaceX 利用 Starlink 保证发射频率的战略，Rocket Lab 获得了盈利的卫星业务和频谱。一些人对发射成本降低导致空间碎片增加表示担忧，另一些人则注意到公司从新西兰注册转为美国注册。

**标签**: `#Rocket Lab`, `#Iridium`, `#Space`, `#Acquisition`, `#Satellite Communications`

---

<a id="item-4"></a>
## [Game Boy 模拟器 JIT 编译为 WASM，超越原生解释器](https://humphri.es/blog/WATaBoy/) ⭐️ 8.0/10

这种方法绕过了 iOS 等平台上对原生 JIT 编译的限制，因为 Web 浏览器允许对 WebAssembly 进行 JIT 编译。这为在 Web 和受限环境中实现高性能模拟及其他计算密集型应用开辟了新的可能性。 该模拟器在运行时将 Game Boy 的 SM83 指令集编译为 WASM，导致 Firefox 的性能比 Chrome 和 Safari 慢 25%。该项目是本科工作，可在 GitHub 上获取。

hackernews · energeticbark · 6月29日 15:02 · [社区讨论](https://news.ycombinator.com/item?id=48720190)

**背景**: Game Boy 模拟器通常使用解释或原生 JIT 编译来模拟掌机硬件。WebAssembly (WASM) 是一种低级二进制格式，可在浏览器中以接近原生的性能运行，并且浏览器支持对 WASM 进行 JIT 编译。Apple 在 iOS 上限制原生 JIT，但允许在 Web 浏览器内通过 JavaScriptCore 和 WebAssembly 进行 JIT 编译。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/EnergeticBark/WATaBoy">GitHub - EnergeticBark/ WATaBoy : A Game Boy emulator with an...</a></li>
<li><a href="https://en.wikipedia.org/wiki/WebAssembly">WebAssembly - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞该项目对本科生来说令人印象深刻，指出 WASM 开销（约 20%）远小于解释器开销（约 1000%），因此性能结果在意料之中。有人对 Firefox 慢 25% 的原因以及 iOS 性能对比表示好奇。

**标签**: `#emulation`, `#WebAssembly`, `#JIT`, `#Game Boy`, `#performance`

---

<a id="item-5"></a>
## [深入解析从 CPU 到 GPU 的 CUDA 内核启动路径](https://fergusfinn.com/blog/what-happens-when-you-run-a-gpu-kernel/) ⭐️ 8.0/10

一篇详细的博客文章发布，解释了启动 CUDA 内核时从 CPU 到 GPU 的完整路径，涵盖了门铃写入、信号量同步和队列管理描述符（QMD）。 这篇文章填补了 CUDA 教育中的一个关键空白，揭开了常被忽略的 CPU 到 GPU 提交路径的神秘面纱，帮助开发者更好地理解性能瓶颈并调试 GPU 工作负载。 文章详细介绍了通知 GPU 获取命令的门铃写入、默认流中用于隐式同步的信号量，以及保存内核参数的 QMD 结构。社区评论指出，控制码实际上是表查找而非简单的位域。

hackernews · mezark · 6月29日 13:11 · [社区讨论](https://news.ycombinator.com/item?id=48718863)

**背景**: CUDA 是 NVIDIA 的并行计算平台。启动 CUDA 内核时，CPU 必须通过涉及门铃寄存器、命令排队和同步的驱动程序栈向 GPU 提交工作。大多数教程只关注 GPU 端的执行（块、线程束），忽略了本文解释的 CPU 到 GPU 提交路径。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://fergusfinn.com/blog/what-happens-when-you-run-a-gpu-kernel/">What happens when you run a CUDA kernel</a></li>
<li><a href="https://docs.nvidia.com/cuda/cuda-programming-guide/02-basics/writing-cuda-kernels.html">2.3. Writing SIMT Kernels — CUDA Programming Guide</a></li>

</ul>
</details>

**社区讨论**: 社区反响非常积极，评论者赞扬了对门铃和 QMD 的解释，认为它连接了 CUDA 语法与硬件。一位用户纠正了控制码是表查找而非简单位域，另一位评论者推测优化内核的公司可能被开源库颠覆。

**标签**: `#CUDA`, `#GPU`, `#kernel launch`, `#NVIDIA`, `#systems programming`

---

<a id="item-6"></a>
## [Cerebras 与 OpenAI 交易封锁 AI 初创公司推理访问](https://www.reddit.com/r/MachineLearning/comments/1uiqhiv/cerebras_openai_deal_capacity_has_effectively/) ⭐️ 8.0/10

一家小型 AI 初创公司报告称，Cerebras 与 OpenAI 的交易已预先分配了其大部分近期推理容量，导致其他用户的等待名单实际上无限长。 这凸显了芯片制造商与超大规模企业之间的独家交易可能抑制竞争，限制依赖专用 ASIC 推理硬件进行低延迟应用的小型 AI 公司的访问。 该初创公司需要每秒 1-2k token 的持续吞吐量用于实时编码代理，而 Cerebras 的晶圆级引擎 ASIC 非常适合此类工作负载。据报道，与 OpenAI 的 200 亿美元交易几乎消耗了所有可用容量。

reddit · r/MachineLearning · /u/Kortopi-98 · 6月29日 12:00

**背景**: Cerebras Systems 生产晶圆级引擎（WSE），这是一种专为 AI 工作负载设计的大型 ASIC，在特定推理任务上比 GPU 提供更高的吞吐量和能效。超大规模企业如 OpenAI 是大型云提供商，可以协商独家容量交易，导致小公司无法访问专用硬件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cerebras">Cerebras - Wikipedia</a></li>
<li><a href="https://scx.ai/resources/asic-gpu-performance-analysis">Next-Gen AI Inference : ASIC vs GPU Performance Analysis</a></li>
<li><a href="https://en.wikipedia.org/wiki/Hyperscaler">Hyperscaler</a></li>

</ul>
</details>

**标签**: `#Cerebras`, `#OpenAI`, `#AI inference`, `#startup challenges`, `#chip allocation`

---

<a id="item-7"></a>
## [EML 树被证明是通用逼近器](https://www.reddit.com/r/MachineLearning/comments/1uipl1t/eml_trees_are_universal_approximators_r/) ⭐️ 8.0/10

一篇新论文证明，EML 树（初等函数的复合）是连续函数的通用逼近器，即可以任意精度逼近任何连续函数。 这一理论结果将通用逼近性质从神经网络扩展到 EML 树，可能为机器学习和科学计算中的函数逼近提供替代方法。 证明包括构建二元运算、多项式和双曲正切的 EML 表示，然后将它们用作构建模块。技术挑战包括使用基于符号的分解来处理自然对数的定义域限制。

reddit · r/MachineLearning · /u/JoeGermany · 6月29日 11:16

**背景**: 通用逼近定理是机器学习中的基础结果，指出具有单个隐藏层的神经网络可以逼近任何连续函数。EML 树最初作为通过复合表示初等函数的‘酷技巧’被引入，本文通过证明类似逼近能力同样适用于初等函数的复合（无需神经网络架构），推广了这一思想。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Universal_approximation_theorem">Universal approximation theorem</a></li>

</ul>
</details>

**标签**: `#universal approximation`, `#EML trees`, `#function approximation`, `#machine learning theory`

---

<a id="item-8"></a>
## [HEMA 实践者构建开放数据集以改进 AI 剑术追踪](https://www.reddit.com/r/MachineLearning/comments/1uivddx/i_do_historical_swordfighting_and_noticed_ai/) ⭐️ 8.0/10

一位历史剑术（HEMA）实践者正在创建开放的多视角数据集，记录快速移动、有遮挡的剑术动作，以解决计算机视觉中的一个挑战性问题。他们已在 Hugging Face 上发布了数据集卡片，并正在征求研究人员对注释模式的反馈。 该数据集针对 Sim2Real 差距和细长物体追踪，这些是具身 AI 和体育分析的关键瓶颈。成功可改进高速、遮挡环境下的实时姿态估计和目标追踪，惠及机器人、自主系统和体育科学等领域。 数据集使用同步多视角相机，帧率为 120/240 fps，包含详细的元数据，如生物力学、计算机视觉风险以及每帧的关键点和分割掩码。实践者手动注释了刀剑接触事件、遮挡评级和运动模糊预期。

reddit · r/MachineLearning · /u/fonssagrives · 6月29日 15:16

**背景**: 计算机视觉模型通常难以追踪细长、快速移动的物体，原因在于运动模糊和遮挡，这被称为细长物体追踪挑战。Sim2Real 差距指的是将在模拟中训练的模型迁移到具有不可预测物理的真实场景中的困难。通过提供带有精确注释的真实世界高速剑术视频，该数据集有助于弥合复杂人-物交互中的这一差距。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://votchallenge.net/">VOT Challenge</a></li>
<li><a href="https://www.linkedin.com/posts/davidanastasiu_computervision-aicity-sim2real-activity-7455775601237528576-ZFUD"># computervision #aicity # sim 2 real #machinelearning #smartcities...</a></li>

</ul>
</details>

**标签**: `#computer vision`, `#dataset`, `#embodied AI`, `#object tracking`, `#sports analytics`

---

<a id="item-9"></a>
## [可编辑权重的交互式微型 Transformer 可视化](https://www.reddit.com/r/MachineLearning/comments/1uhw7fu/i_shrank_a_transformer_until_every_number_fitted/) ⭐️ 8.0/10

一个独立的 HTML 文件展示了一个微型 Transformer（6 词词汇表，3 维嵌入），支持完全可编辑的权重和正向传播的实时重新计算。 该工具使 Transformer 内部机制（包括注意力机制）变得可访问和互动，帮助学习者无需深厚技术背景即可理解正向传播过程。 该 Transformer 使用单注意力头和单层，可编辑词向量和权重，并包含随机化按钮以展示未训练权重的影响。

reddit · r/MachineLearning · /u/DanielMoGo · 6月28日 12:35

**背景**: Transformer 使用自注意力机制处理序列，该机制从输入嵌入中计算查询（Q）、键（K）和值（V）向量。因果掩码确保模型在语言建模任务中仅关注之前的位置。该可视化逐步演示了这些概念。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mbrenndoerfer.com/writing/query-key-value-attention-mechanism">Query, Key, Value: The Foundation of Transformer Attention ...</a></li>
<li><a href="https://hexiao5886.medium.com/day-4-100-causal-masking-in-transformers-a-deep-dive-into-masked-attention-43a7ece5fc1f">Day(4/100) Causal Masking in Transformers : A Deep Dive... | Medium</a></li>

</ul>
</details>

**标签**: `#transformer`, `#visualization`, `#machine learning`, `#education`, `#interactive`

---

<a id="item-10"></a>
## [.self 顶级域名提案旨在赋能自托管用户](https://hccf.onmy.cloud/2026/06/21/reclaiming-our-digital-selves-hccfs-vision-for-a-human-centered-top-level-domain/) ⭐️ 7.0/10

一项名为 .self 的新顶级域（TLD）提案发布，设想为个人提供免费子域以支持自托管，并采取反域名抢注措施防止滥用。 如果实施，该顶级域可能降低自托管门槛，让个人对自己的在线身份有更多控制，减少对中心化平台的依赖。然而，社区讨论指出，该提案在资金、身份验证和防止滥用方面面临重大挑战。 该提案承诺‘一人一子域’以防止域名抢注，但批评者质疑如何在不进行侵入式验证的情况下区分合法使用与停放域名。该 TLD 尚未列入 IANA 根区域，目前仅为概念。

hackernews · HumanCCF · 6月29日 19:49 · [社区讨论](https://news.ycombinator.com/item?id=48724230)

**背景**: 自托管是指运行个人服务器来提供网站、电子邮件或其他服务，而不是使用第三方提供商。.self TLD 将是一个专为个人托管自己服务的命名空间。然而，运营一个顶级域成本高昂，之前的免费 TLD 如 .tk 曾因滥用问题而受到主要平台的封锁。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Self-hosting_(network)">Self-hosting (network) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区评论对资金和滥用预防表示怀疑。一位用户回忆了 .tk TLD 因诈骗而被屏蔽的历史。其他人质疑‘一人一子域’在不损害隐私的情况下是否可行，并指出该 TLD 尚未在根区域注册。

**标签**: `#self-hosting`, `#TLD`, `#internet governance`, `#domain names`, `#privacy`

---

<a id="item-11"></a>
## [Qwen 3.6 27B：本地开发的甜蜜点？](https://quesma.com/blog/qwen-36-is-awesome/) ⭐️ 7.0/10

一篇博客声称 Qwen 3.6 27B 模型是本地开发的理想选择，但 Hacker News 社区因高昂的硬件成本而争论其实用性。 这场争论凸显了在本地运行强大的开源权重 LLM 与使用更便宜的云 API 之间的张力，影响着 AI 开发者和爱好者的决策。 博客测试依赖于 128GB MacBook Pro（6,699 美元以上），而评论者指出 OpenRouter 以极低成本提供相同或更好的模型。

hackernews · stared · 6月29日 17:05 · [社区讨论](https://news.ycombinator.com/item?id=48721903)

**背景**: Qwen 3.6 是阿里巴巴的开源权重 LLM 系列，27B 参数版本在编码和代理任务中表现出色。在本地运行此类模型需要昂贵的高 RAM 硬件，而云 API 可按 token 访问，无需前期投入。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ollama.com/library/qwen3.6:27b">qwen 3 . 6 : 27 b</a></li>
<li><a href="https://huggingface.co/rico03/Qwen3.6-27B-Claude-Opus-Reasoning-Distilled">rico03/ Qwen 3 . 6 - 27 B -Claude-Opus-Reasoning-Distilled · Hugging Face</a></li>
<li><a href="https://www.youtube.com/watch?v=N5eEqJVTfVI">Qwen 3 . 6 27 B vs 35B-A3B: 16GB VRAM Local Test - YouTube</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍同意本地 LLM 很有趣但不经济；许多人主张使用 OpenRouter 来获取更便宜、更大的模型。一些人质疑博客的编码示例不能代表使用现有代码库的真实工作。

**标签**: `#Qwen`, `#local LLM`, `#AI development`, `#cost analysis`, `#hardware`

---

<a id="item-12"></a>
## [Ornith-1.0：用于智能编程的开源自脚手架大模型](https://simonwillison.net/2026/Jun/29/ornith/#atom-everything) ⭐️ 7.0/10

DeepReinforce 发布了 Ornith-1.0，一个面向智能编程的开源（MIT 许可）大模型系列，包含 9B、31B、35B MoE 和 397B MoE 等变体。在同规模开源模型中，它在编程基准测试上达到了最先进的性能。 这是首个能自动生成 Agent 框架的“自脚手架”大模型，有望提升代码代理的自主性和能力。其宽松的 MIT 许可和强劲的基准性能使其成为开发者和研究者的重要开源选择。 Ornith-1.0 基于 Gemma 4（Apache 2.0）和 Qwen 3.5（Apache 2.0），采用自脚手架训练框架，模型学习同时生成解决方案和任务特定框架。它还使用冻结的 LLM 裁判来防止奖励黑入，35B 变体可通过 GGUF 量化在消费级硬件上高效运行。

rss · Simon Willison · 6月29日 16:17

**背景**: 智能编程是指使用 AI 代理自主执行软件开发任务，如代码生成、调试和测试。自脚手架是一种技术，模型自行生成执行框架而非依赖预定义框架，从而更好地适应任务。混合专家（MoE）是一种每 token 仅激活部分参数的架构，平衡了性能与计算成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/29/ornith/">Ornith-1.0: Self-Scaffolding LLMs for Agentic Coding</a></li>
<li><a href="https://essamamdani.com/blog/ornith-1-0-self-scaffolding-llm-coding-2026">Ornith-1.0: The Self-Scaffolding LLM That Teaches Itself to ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Agentic_coding">Agentic coding</a></li>

</ul>
</details>

**标签**: `#LLM`, `#open-source`, `#coding`, `#AI`, `#benchmarks`

---

<a id="item-13"></a>
## [Jon Udell 翻转叙事：智能体是团队成员，而非黑箱](https://simonwillison.net/2026/Jun/28/jon-udell/#atom-everything) ⭐️ 7.0/10

Jon Udell 提议重新定义 AI 智能体协作：将智能体邀请进入人类的工作循环，而非将人类置于机器主导的循环中。他反对由智能体创建不可审查的拉取请求，主张透明且由人类监督的智能体开发。 这一重新框架改变了 AI 辅助软件开发中的权力动态，通过保持人类控制来促进负责任的智能体使用。它对主流的“人在循环中”术语提出了挑战，可能影响集成编码智能体的最佳实践，同时不牺牲监督。 Udell 的核心观点是：智能体创建的拉取请求应接受人类审查，而非成为黑箱功能。该文章是哲学性评论而非技术突破，但带有相关 AI 和软件开发标签。

rss · Simon Willison · 6月28日 21:57

**背景**: 智能体软件工程（SE 3.0）是一种新兴范式，其中 AI 智能体自主编写、测试和提交代码。常见的短语“人在循环中”暗示人类是自动化过程的边缘角色。Udell 通过断言软件开发仍然是人类主导的循环，而智能体是被邀请的参与者而非替代者，翻转了这一概念。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/agentic-engineering">What is agentic engineering? - IBM</a></li>
<li><a href="https://arxiv.org/html/2509.06216v2">Agentic Software Engineering: Foundational Pillars and a ...</a></li>

</ul>
</details>

**标签**: `#software development`, `#AI agents`, `#human-in-the-loop`, `#coding agents`, `#best practices`

---

<a id="item-14"></a>
## [黑客你的夏天：面向学生的免费四周冲刺项目](https://simonwillison.net/2026/Jun/28/hack-your-summer/#atom-everything) ⭐️ 6.0/10

Hack Your Summer 是一项针对本科生和研究生的免费四周生产冲刺项目，旨在应对美国的实习危机。第二期将于 7 月 13 日开始，申请截止日期为 7 月 8 日。 该项目为因招聘减少而未能获得实习机会的学生提供了替代方案，帮助他们构建真实项目并积累经验，以便向未来雇主展示。 该计划免费，持续 4 周，并包含志愿者指导。学生将学习如何确定项目、稳步推进，并创建可公开展示的作品。

rss · Simon Willison · 6月28日 19:26

**背景**: 生产冲刺（production sprint）是敏捷开发中的一个固定时间周期，团队在此期间完成一定量的工作。在本次活动中，Hack Your Summer 采用冲刺模式帮助学生快速构建并交付真实项目。该倡议旨在应对公司减少招聘和指导能力导致的实习岗位短缺问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.techtarget.com/searchsoftwarequality/definition/Scrum-sprint">What is a sprint (software development)? | Definition from ...</a></li>
<li><a href="https://www.atlassian.com/agile/scrum/sprints">Scrum sprints - Atlassian</a></li>

</ul>
</details>

**标签**: `#education`, `#internships`, `#career development`, `#students`

---

<a id="item-15"></a>
## [基于性格的 LLM 匹配测试上线](https://www.reddit.com/r/MachineLearning/comments/1uin5ad/i_made_a_quiz_that_tells_you_which_llm_you_align/) ⭐️ 6.0/10

一位 Reddit 用户在 ai-values.com 上制作了一个互动测试，通过对比 15 个大语言模型的性格和道德价值观，让用户了解自己与哪个 LLM 最契合。 该测试揭示了不同 LLM 之间的巨大价值观差异，对于用户选择适合敏感任务的模型以及研究人员研究 AI 对齐问题都至关重要。 该测试包含 117 道问题，每个模型至少回答 5 次；结果显示 Grok 4.3 是唯一反对对亿万富翁加税的模型，而 GPT-4o 是唯一认为“回形针行动”正当的模型。

reddit · r/MachineLearning · /u/DarkyPaky · 6月29日 09:00

**背景**: LLM 对齐旨在确保 AI 模型的行为符合人类价值观和意图。该测试评估了诸如 xAI 的推理模型 Grok 4.3 和 z.ai 的开源模型 GLM 5.2 等多个模型，通过多种人格框架揭示了它们隐含的道德立场。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Grok_(chatbot)">Grok (chatbot) - Wikipedia</a></li>
<li><a href="https://openlm.ai/glm-5.2/">GLM-5.2 - openlm.ai</a></li>
<li><a href="https://link.springer.com/article/10.1007/s43681-024-00637-w">Evaluating alignment in large language models: a review of ...</a></li>

</ul>
</details>

**标签**: `#LLM`, `#values`, `#quiz`, `#personality`, `#AI alignment`

---