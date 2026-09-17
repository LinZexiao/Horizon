---
layout: default
title: "Horizon Summary: 2026-09-17 (ZH)"
date: 2026-09-17
lang: zh
---

> 从 31 条内容中筛选出 17 条重要资讯。

---

1. [NVIDIA 为 CUDA 带来原生 Rust GPU 内核编程支持](#item-1) ⭐️ 8.0/10
2. [微软详解 .NET 11 的性能改进](#item-2) ⭐️ 8.0/10
3. [AWS 称无法恢复遭伊朗袭击的中东数据中心部分数据](#item-3) ⭐️ 8.0/10
4. [Show HN：电子墨水相框用 BirdNET 听鸟鸣，并绘制成 19 世纪风格插画](#item-4) ⭐️ 8.0/10
5. [TMLR 测试论文作者能否解释自己提交的论文](#item-5) ⭐️ 8.0/10
6. [Prior Labs 发布 TabPFN-3.5，刷新表格基础模型 SOTA](#item-6) ⭐️ 8.0/10
7. [40 亿参数模型生成比 Postgres 快 81%的查询计划](#item-7) ⭐️ 7.0/10
8. [论文将三值大模型量化压缩至 1.58 比特/权重以下](#item-8) ⭐️ 7.0/10
9. [小米上线 MiMo 2.6 后训练实时仪表盘](#item-9) ⭐️ 7.0/10
10. [Mozilla 与 Mistral 合作，为 Firefox 带来私密 AI 浏览体验](#item-10) ⭐️ 7.0/10
11. [Simon Willison 发布用于测试 Gemini 3.8 Live 语音模型的浏览器界面](#item-11) ⭐️ 7.0/10
12. [GoBench 用 9x9 围棋与 KataGo 对手评测大模型](#item-12) ⭐️ 7.0/10
13. [SHADOW-50M：44M 三元权重模型仅 19.8 MB，CPU 上约 1,900 tok/s](#item-13) ⭐️ 7.0/10
14. [博客文章汇编小型编程与命令行技巧，引发 Hacker News 热议](#item-14) ⭐️ 6.0/10
15. [Anthropic 将 Claude Cowork 与 Claude 聊天合并为单一产品](#item-15) ⭐️ 6.0/10
16. [Mustafa Suleyman 反对赋予 AI 模型福利与权利](#item-16) ⭐️ 6.0/10
17. [LARA：面向冻结大模型的可组合低秩残差适配器](#item-17) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [NVIDIA 为 CUDA 带来原生 Rust GPU 内核编程支持](https://developer.nvidia.com/blog/introducing-cuda-rust-two-tracks-for-writing-gpu-kernels/) ⭐️ 8.0/10

NVIDIA 在其开发者博客上发布了 CUDA Rust 的官方介绍，提供两条不同的技术路线，让开发者可以用 Rust 为 CUDA 平台编写 GPU 内核。这是 NVIDIA 首次以官方方式支持开发者用 Rust 直接进行内核级开发，而不必再退回 C++。 Rust 是增长最快的系统编程语言之一，把它引入 CUDA 有望吸引一批新开发者进入 GPU 编程领域，并提供 C++ 内核所缺乏的编译期内存安全保证。但与此同时，这也进一步巩固了 NVIDIA 专有 CUDA 生态作为默认目标平台的地位，而此时 Triton、OpenCL、Metal、D3D12 等可移植方案正逐渐获得关注。 文章将这套方案描述为编写内核的两条路线，并被引用称内核启动是“经过检查而非被信任”（checked rather than trusted），即安全性由检查来保证而不是默认假设。仍需注意的局限是：CUDA 代码依然只能在 NVIDIA 显卡上运行，而且底层内核开发通常需要动用 Rust 的 `unsafe` 逃逸口，因此其安全保证弱于普通的安全 Rust 代码。

hackernews · nonmaskable · 9月16日 11:15 · [社区讨论](https://news.ycombinator.com/item?id=49724881)

**背景**: CUDA 是 NVIDIA 专有的并行计算平台与编程模型，传统上通过 C/C++ 扩展使用，可让代码同时在数千个 GPU 核心上运行，是现代 AI 训练与推理的基石。所谓“内核”（kernel）就是在这些核心上并行执行的小函数。Rust 是一门系统编程语言，其所有权与借用检查规则能在编译期消除 use-after-free 等常见内存缺陷，因此适合底层与安全敏感场景。CUDA 之外的 GPU 编程选择包括 OpenCL、Apple 的 Metal、微软的 D3D12，以及嵌入 Python 的 DSL（如 Triton）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.keypuncher.net/introduction-to-cuda-for-c/">Introduction to CUDA for C++</a></li>
<li><a href="https://developers.redhat.com/articles/2024/05/21/improve-basic-programming-safety-rust-lang">Improve basic programming safety with Rust lang | Red Hat Developer</a></li>
<li><a href="https://arxiv.org/abs/2607.04454">[2607.04454] Correct but Slow: An Empirical Study of the GPU Kernel...</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论总体偏正面，有人表示“一直在等这样的东西”，并认为 Rust 的安全性可能成为内核编程的颠覆性改变。最强烈的反对意见针对 CUDA 本身：一位评论者称这种专有技术栈一旦进入 C++ 代码库就很难剥离，最终要么被单一厂商绑定，要么陷入“#ifdef 地狱”，并主张内核应放在独立文件中手动启动，就像 Metal、OpenCL、D3D12 那样，或改用 Triton 之类的 DSL。也有人提到 Hugging Face 的 Candle crate 可作为 Rust 推理的补充，还有人调侃 NVIDIA 这篇文章读起来像是大模型写的。

**标签**: `#Rust`, `#CUDA`, `#GPU Programming`, `#NVIDIA`, `#Systems Programming`

---

<a id="item-2"></a>
## [微软详解 .NET 11 的性能改进](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-11/) ⭐️ 8.0/10

微软发布了年度博客文章《.NET 11 中的性能改进》，系统梳理了运行库、JIT 与基础库的大量优化，其中包含运行时异步（runtime async）以及代码生成质量的改动。 这些优化让现有的 .NET 应用无需修改代码就能获得更快的启动速度、更低的内存分配和更高的吞吐量，对云服务、Web API 以及冷启动延迟敏感的容器化工作负载有直接的收益。 该文章是非常深入的代码级剖析——社区分享的一个示例显示，在消除多余的边界检查比较与跳转后，ARM64 上的 JIT 生成代码从 68 字节缩减到 60 字节；而评论者认为 runtime async 仍处于早期发展阶段，其实际效果还有待观察。

hackernews · soheilpro · 9月15日 12:18 · [社区讨论](https://news.ycombinator.com/item?id=49711424)

**背景**: .NET 运行库是微软的跨平台托管执行环境：C# 代码会先被编译成中间语言（IL），随后由公共语言运行时（CLR）通过即时编译器（JIT）在运行时编译为原生机器码。由于 JIT 是按需编译方法，.NET 采用分层编译（tiered compilation）策略，先用快速编译的代码保证启动速度，之后再对热点方法进行更深度优化重编，以提升稳定状态下的吞吐量。微软每年都会发布一篇《.NET 中的性能改进》文章，详细讲述这些运行库与基础库优化背后的工程工作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.telerik.com/blogs/understanding-net-just-in-time-compilation">Understanding . NET Just-In-Time Compilation</a></li>
<li><a href="https://www.dotnet-guide.com/jit1.html">Optimizing Performance with JIT Compilation in . NET Runtime</a></li>
<li><a href="https://techsyntax.net/post/dotnet-vs-nodejs-performance-comparison-2026">NET vs Node.js Performance: 2026 Backend Benchmark - Tech Syntax</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的反馈整体非常正面：有开发者称这些文章让自己成了“.NET 布道者”，有人表示在最近一次项目迁移中明显感受到启动速度提升，还有不少人对 runtime async 表示期待。主要批评是文章虽长，却缺少应用层面的基准测试来体现累积的实际收益；另有一位非系统方向的开发者询问社区，自己是否有必要学会阅读汇编代码。

**标签**: `#.NET`, `#performance`, `#runtime`, `#C#`, `#JIT`

---

<a id="item-3"></a>
## [AWS 称无法恢复遭伊朗袭击的中东数据中心部分数据](https://www.wsj.com/world/middle-east/aws-says-it-cant-restore-some-data-from-mideast-facilities-struck-by-iran-ddcb7e5d) ⭐️ 8.0/10

AWS 表示，其位于中东的部分数据中心因遭到伊朗袭击而物理受损，其中一些客户数据已无法恢复，等同于承认这部分数据已永久丢失。据报道，该事件导致该地区多个可用区下线，涉及巴林和阿联酋的容量。 这是一次罕见的真实案例，说明云冗余并非绝对保障：当整个区域被物理摧毁时，大多数企业视为安全网的复制与故障转移假设可能失效。它直接影响所有依赖中东 AWS 区域运行受监管或低延迟业务的组织，并让灾难恢复、合规与地缘政治风险重新回到企业管理层的议程上。 受损范围似乎波及 me-south-1（巴林）和 me-central-1（阿联酋）区域内的多个可用区，社区讨论显示部分可用区早在 2026 年 3 月就已下线。一个关键限制在于，数据驻留法规可能从法律上禁止将某些数据复制到境外，从而使“从区域外备份恢复”这一选项根本不存在。

hackernews · berkeleyjunk · 9月15日 21:41 · [社区讨论](https://news.ycombinator.com/item?id=49719249)

**背景**: 像 AWS 这样的云厂商会把每个区域划分为多个可用区——即拥有独立供电和网络的物理隔离数据中心——并建议客户将工作负载分散部署，以便单个设施失效时业务不至于中断。云计算中的冗余指的是为数据、服务器和应用保留多份副本，使故障发生时能够被吸收而不丢失数据。数据驻留则带来另一重约束：它规定了数据必须被存储和处理的物理或地理位置，通常是因为当地法律要求数据留在本国境内。当驻留法规禁止把数据复制到境外时，一旦境内设施被摧毁，就可能不再有任何存活的副本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.akamai.com/glossary/what-is-cloud-redundancy">What Is Redundancy in Cloud Computing? - Akamai</a></li>
<li><a href="https://www.ibm.com/think/insights/data-residency-why-is-it-important">Data residency: What is it and why is it important? | IBM</a></li>
<li><a href="https://www.enormousit.com/infrastructure/disaster-recovery-on-demand/">Disaster Recovery On Demand – Enormous IT</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认为这起事件暴露了最基本的灾难恢复纪律缺失，有人指出异地备份和灾难恢复计划几十年来都是标准做法。一段 CBS 采访被大量转发：AWS 高管当时声称即便炸掉一座数据中心用户也不会察觉，许多人认为这一说法如今已被彻底打脸。也有人指出阿联酋的数据驻留要求在法律上强制数据留在境内，架构师根本无法将其复制到别处；还有用户梳理了巴林、阿联酋和以色列各可用区的下线情况及持续时间。

**标签**: `#cloud-infrastructure`, `#aws`, `#disaster-recovery`, `#data-residency`, `#geopolitics`

---

<a id="item-4"></a>
## [Show HN：电子墨水相框用 BirdNET 听鸟鸣，并绘制成 19 世纪风格插画](https://github.com/arnegiacomo/fugleramme) ⭐️ 8.0/10

开发者 Arne Munthe-Kaas 在 GitHub 上发布了名为 fugleramme 的项目：一个电子墨水（e-ink）相框，它会持续监听环境声音，用 BirdNET 分类器识别附近的鸟类，再把每种识别到的鸟渲染成 19 世纪风格的插画显示在屏幕上。该 Show HN 帖子获得了 2075 分和 238 条评论，成为近期 Hacker News 上讨论度最高的业余项目之一。 这个项目被广泛称赞为“嵌入式机器学习 + 生成式艺术”的优秀范例：它说明用一块便宜的 ESP32 级设备、一个现成的生物声学模型和一块电子墨水屏，就能组合出低功耗、融入生活环境且颇具魔力的体验，而不是噱头。它也体现出生成式插画与小模型端侧推理正从演示走向家里的日常物件。 BirdNET 是一个基于频谱图训练的传统卷积神经网络，可识别约 984 种鸟类，并非大语言模型（LLM），它以 48 kHz 采样、按 3 秒一段处理音频。该设计依赖电子墨水屏的“断电保持”特性（仅在刷新时耗电）以及 BLE 等低功耗无线方案，因此这类相框据说用一块 2000 mAh 电池、即便每天刷新多次也能续航一年以上。

hackernews · arnemunthekaas · 9月15日 12:31 · [社区讨论](https://news.ycombinator.com/item?id=49711544)

**背景**: BirdNET 是与康奈尔鸟类学实验室合作开发的开源生物声学工具，能从短音频片段中识别鸟种，广泛用于生态监测。ESP32 是乐鑫（Espressif）推出的低成本、低功耗 Wi-Fi/蓝牙微控制器，常用于物联网与嵌入式项目；电子墨水屏则是一种双稳态屏幕，断电后仍能保留画面。把“常听—端侧识别—静态显示”这三者结合起来，是嵌入式机器学习的典型范式：模型直接在算力受限的设备上运行，而无需上云。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sciencedirect.com/science/article/pii/S1574954121000273">BirdNET: A deep learning solution for avian diversity monitoring - ScienceDirect</a></li>
<li><a href="https://birdnet.cornell.edu/">BirdNET – AI-Powered Sound ID</a></li>
<li><a href="https://en.wikipedia.org/wiki/ESP32">ESP32 - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者几乎一致表示赞叹：有人称这是近期 Hacker News 上“最酷的东西”，是“各种想法的完美融合”，效果堪称神奇；一位同为挪威人的网友则称赞开发者的作品是“纯粹的艺术”。技术型用户还补充了背景：指出 BirdNET 是传统神经网络而非大语言模型，分享 BLE 驱动的电子墨水相框一次充电可用数年，并提到近期涌现的一批鸟类识别项目（如 birdnet-go）。

**标签**: `#e-ink`, `#ESP32`, `#birdnet`, `#generative-art`, `#embedded-ml`

---

<a id="item-5"></a>
## [TMLR 测试论文作者能否解释自己提交的论文](https://www.reddit.com/r/MachineLearning/comments/1wid67h/tmlr_reached_out_to_the_authors_of_10_papers/) ⭐️ 8.0/10

TMLR 的主编联系了 10 篇被标记为「desk rejection（编辑直接拒稿）」候选论文的作者，要求他们在会议上解释自己提交的论文。结果：1 篇作者撤稿，1 篇以事务繁忙为由推脱，1 篇约好会议却未出席，3 篇作者无法回答关于论文的基本问题，3 篇只能回答高层思路、遇到技术细节便卡壳，只有 1 篇作者全部答对——而主编还在那篇论文里发现了一个重大缺陷。 这一实验提供了相当直接的证据，表明投往机器学习期刊/会议的稿件中有相当一部分可能并非由提交者本人撰写，指向论文工厂或大语言模型代写的可能性。它给同行评审的诚信机制、作者身份核验，以及期刊如何识别这类浪费评审资源的虚假投稿提出了严峻问题。 该调查由 TMLR 联合主编亲自通过对话进行，而非依赖自动化检测工具；样本仅为 10 篇 desk-reject 候选论文，因此属于个案观察而非统计代表性证据。值得注意的是，那位全部答对的作者，其论文仍被指出存在重大缺陷，说明这种面谈筛查的是「作者身份真实性」，而不是论文质量。

reddit · r/MachineLearning · /u/hihey54 · 9月16日 23:20

**背景**: TMLR（Transactions on Machine Learning Research）是隶属于 JMLR 的机器学习期刊，采用类似会议的流程：双盲评审、在 OpenReview 上公开评审意见、全年滚动投稿，评审标准主要看技术正确性。desk rejection（编辑直接拒稿）是指编辑在初审阶段、尚未送外审之前就拒掉稿件。近期研究估计科学论文中经大语言模型修改的文本比例持续上升，计算机科学领域增幅最大（最高约 17.5%），这加剧了人们对自动化代写、枪手投稿的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://jmlr.org/tmlr/">Transactions on Machine Learning Research</a></li>
<li><a href="https://casrai.org/guides/desk-rejection">What Desk Rejection Means and Why It Happens — CASRAI</a></li>
<li><a href="https://arxiv.org/abs/2404.01268">Mapping the Increasing Use of LLMs in Scientific Papers</a></li>

</ul>
</details>

**标签**: `#peer-review`, `#academic-integrity`, `#ML-research`, `#LLM-generated-content`, `#publishing`

---

<a id="item-6"></a>
## [Prior Labs 发布 TabPFN-3.5，刷新表格基础模型 SOTA](https://www.reddit.com/r/MachineLearning/comments/1wh4xhy/tabpfn35_is_released_as_the_next_sota_tabular/) ⭐️ 8.0/10

Prior Labs 发布了 TabPFN-3.5，该模型目前在 TabArena 和 BeyondArena 两个榜单上均排名第一，并号称在多达 100 万行、最多 2 万列特征的数据集上达到 SOTA。本次发布包含三个变体：TabPFN-3.5-Fast（处于 alpha 阶段，速度约为基础模型的 6 倍）、TabPFN-3.5-Thinking（以计算量换取更高精度，通过 API 提供）以及 TabPFN-3.5-Plus。 表格数据仍是工业界最主要的数据形式，而一款在分布内（IID）和超越 IID 两类基准上都领先的基础模型，进一步支持了“预训练 Transformer 能够替代或补充 XGBoost、CatBoost 等梯度提升树”的观点。相比此前最强基线高出 +250 Elo、相比此前总榜第一高出 +150 Elo，说明这对从事表格预测任务的实践者而言是一次显著而非渐进的进步。 在 BeyondArena 上，TabPFN-3.5 具体在文本丰富、高基数和高维数据上领先；TabPFN-3.5-Thinking 相比基础模型在 BeyondArena 上再提升 +20 Elo，在 TabArena 上提升 +44 Elo。Fast 变体被明确标记为 alpha 版本，而 Thinking 变体只能通过 API 调用，无法使用本地权重。

reddit · r/MachineLearning · /u/tuanacelik · 9月15日 16:18

**背景**: TabPFN（Tabular Prior-data Fitted Network，表格先验拟合网络）是 2022 年论文中提出的一种基于 Transformer 的模型，采用上下文学习（in-context learning）：它直接根据输入提示中给定的带标签样本进行预测，无需更新参数，也无需针对每个数据集单独训练。早期版本仅支持约 1000 个样本的小数据集，此前的 TabPFN-3 将支持范围大幅扩展，而 TabPFN-3.5 又把上限推进到 100 万行、2 万列特征。TabArena 是一个持续更新的“活”基准，使用人工筛选的 IID 表格数据集；BeyondArena 则把评测扩展到非 IID 场景，涵盖时序和分组任务。此前 BeyondArena 的结果曾指出，在非 IID 数据上树模型仍优于表格基础模型，因此 TabPFN-3.5 在该榜单上取得领先尤为值得关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/TabPFN">TabPFN</a></li>
<li><a href="https://arxiv.org/abs/2506.16791">TabArena : A Living Benchmark for Machine Learning on Tabular Data</a></li>
<li><a href="https://aiweekly.co/alerts/beyondarena-finds-trees-still-beat-tabular-fms-off-iid-data">BeyondArena finds trees still beat tabular FMs off-IID data | AI Weekly</a></li>

</ul>
</details>

**标签**: `#tabular-data`, `#foundation-models`, `#machine-learning`, `#benchmarks`, `#TabPFN`

---

<a id="item-7"></a>
## [40 亿参数模型生成比 Postgres 快 81%的查询计划](https://rohanbansal.com/qorl) ⭐️ 7.0/10

rohanbansal.com/qorl 上的一篇博客文章描述了训练一个 40 亿参数的语言模型来生成查询计划，据称在一个小型内存基准测试上比 PostgreSQL 内置规划器的启发式策略快 81%。该文章在 Hacker News 上获得 384 分和 81 条评论，讨论很快转向对该基准测试真实性以及 LLM 驱动查询规划实用性的质疑。 查询规划是数据库工程中最困难、影响也最大的问题之一，因此任何能在特定负载上超越 PostgreSQL 沿用数十年的基于代价的优化器的方法都值得关注。如果小型模型能够学会更优的连接顺序和访问路径，可能会重塑优化器的构建方式，但社区的强烈质疑表明实际落地仍然遥远。 该结果是在一个可完全放入内存的 8 GB 数据集上测得的，同时将 shared_buffers 刻意限制为该数据集的一小部分，并采用预热缓存、只读 SELECT 查询，且除了主键之外没有任何索引或额外的列统计信息。评论者还指出，该优化器依赖 profile guided optimization（基于剖析的优化），这意味着其行为未必能迁移到大规模的真实 OLTP 工作负载上。

hackernews · polyphilz · 9月16日 18:50 · [社区讨论](https://news.ycombinator.com/item?id=49731285)

**背景**: 数据库查询规划器决定一条 SQL 语句如何执行——使用哪些索引、以什么顺序连接表、采用哪种算法——而 PostgreSQL 等传统系统使用基于统计信息驱动的代价启发式方法。由于规划本质上是一个序列决策问题，大语言模型正越来越多地被探索作为替代规划器。作者的方法使用了一个相对较小的 40 亿参数模型，这一点值得注意，因为生产级 LLM 通常要大得多。

**社区讨论**: 评论者普遍持怀疑态度：refibrillator 列举了该基准测试的诸多前提（8 GB 数据全部缓存、shared_buffers 受限、查询预热、只读 SELECT），sgarland 则指出除了主键之外没有任何索引，且尽管列之间存在相关性也没有额外的统计信息，并认为 hint 通常只是掩盖统计信息不准的问题而非真正解决它。2001zhaozhao 讽刺了因 LLM 幻觉生成了漏掉索引的计划而导致的生产事故，hamilyon2 则认为最优计划构造高度依赖数学与算法，把 LLM 称为“钝器”，并表示更期待 AlphaGo 式的神经网络启发式方法。

**标签**: `#databases`, `#query-optimization`, `#LLM`, `#Postgres`, `#benchmarking`

---

<a id="item-8"></a>
## [论文将三值大模型量化压缩至 1.58 比特/权重以下](https://arxiv.org/abs/2609.16338) ⭐️ 7.0/10

一篇新论文（arXiv:2609.16338）声称实现了亚 1.58 比特的三值大模型量化，通过利用实践中约 51% 的三值权重恰好为零这一现象，把每权重比特数降到约 1.48 比特。这一收益来自于对经验稀疏性的编码，而非改变 {-1, 0, +1} 的权重表示本身。 这突破了被普遍视为三值权重理论下限的 log2(3) ≈ 1.58 比特，有望进一步压缩大模型以适配嵌入式与端侧部署。若三值模型被固化到定制芯片中，推理的功耗与面积效率可能显著提升。 这一改进完全取决于权重的实际零值比例，因此有效比特数会随模型和层而变化，并非三值运算的固定属性；评论者还提出用存在位图（presence bitmap）甚至算术编码再挤出几个“厘比特”。怀疑者指出，在这一超低比特区间，向量量化（VQ）与基于格（trellis）的训练后量化方法可能优于三值方案。

hackernews · matt_d · 9月16日 20:59 · [社区讨论](https://news.ycombinator.com/item?id=49732931)

**背景**: 量化通过降低模型权重的数值精度来减少内存占用与计算开销。2024 年微软研究院提出 BitNet b1.58，从一开始就以三个取值 {-1, 0, +1} 训练模型，使每权重仅需 log2(3) ≈ 1.58 比特而非 16 比特；由于与这些取值相乘可简化为加法或取负，这类模型非常适合 ASIC 与边缘硬件。这项新工作则试图在不放弃三值表示的前提下，进一步压到 1.58 比特以下。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/1.58-bit_large_language_model">1.58-bit large language model - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/1_58_llm_extreme_quantization">Fine-tuning LLMs to 1.58bit: extreme quantization made easy</a></li>
<li><a href="https://www.emergentmind.com/topics/1-58-bit-quantization-techniques">1.58-bit Quantization Techniques in Deep Learning</a></li>

</ul>
</details>

**社区讨论**: 讨论情绪褒贬不一但参与度较高。一些评论者对嵌入式可移植性、面向 ASIC 的推理以及创纪录的能效表现感到兴奋，其中一位指出若采用量化感知训练，模型只需约多 30% 的权重即可达到相当的质量。另一些人则持反对意见，认为在这一区间三值量化意义不大，因为向量量化与基于格的 PTQ 方法更强；还有人半开玩笑地提议用算术编码再省下几个“厘比特”。

**标签**: `#quantization`, `#LLM`, `#model-compression`, `#efficient-inference`, `#ternary-models`

---

<a id="item-9"></a>
## [小米上线 MiMo 2.6 后训练实时仪表盘](https://mimo.xiaomi.com/rl/) ⭐️ 7.0/10

小米在 mimo.xiaomi.com/rl/ 上线了一个实时仪表盘，直接读取训练器日志，持续展示 MiMo-v2.6-pro 与 MiMo-v2.6-flash 两个模型的强化学习/后训练指标。与常见的“训练完成后再发博客和跑分表”不同，该页面在训练过程中实时公开遥测数据。 对一个接近前沿、且开放可用的模型家族而言，公开实时训练遥测是极少见的透明化举措，也让外界能直接审视一家中国实验室究竟如何调教其推理模型。这会迫使 OpenAI、Anthropic 等厂商解释为何把后训练过程完全封闭，同时也让开发者能实时判断下一代 MiMo 何时可用于编码与智能体任务。 该仪表盘覆盖 mimo-v2.6-pro 与 mimo-v2.6-flash 两个版本，并明确标注数据来自训练器的实时日志，而非挑选过的跑分结果，因此呈现的是原始训练指标而非最终产品能力。社区成员提到，作为参照，MiMo-v2.5-Pro 在 DeepSWE 1.1 上得分 19%，明显低于 Fable（70%）、Kimi K3（69%）和 Astra（74%）；不过这些数字来自第三方评论且推理强度设置不同，并非小米仪表盘本身提供的。

hackernews · krackers · 9月16日 20:09 · [社区讨论](https://news.ycombinator.com/item?id=49732270)

**背景**: 大语言模型通常先在海量文本上完成预训练，再进入后训练阶段——包括监督微调、偏好对齐，以及近年来越来越重要的强化学习——从而把通用基座模型变成能听指令、会推理的可用模型。在面向 LLM 的强化学习中，模型的“动作”就是生成文本，奖励信号则衡量该输出的好坏，因此奖励值、损失和回复长度等训练曲线是研究者最关注的指标。小米的 MiMo 是一条开放模型线，既用于小米自家桌面应用，也可在 Cursor、Cline、Zed 等第三方智能体和编码工具中调用，其中 MiMo-V2.5 已在真实工程场景中被采用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mimo.xiaomi.com/rl/">mimo -v 2 . 6 RL</a></li>
<li><a href="https://en.wikipedia.org/wiki/Post-training_of_large_language_models">Post-training of large language models</a></li>
<li><a href="https://www.ibm.com/think/topics/llm-reinforcement-learning">LLM Reinforcement Learning | IBM</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论总体偏正面：一位工程师表示自己日常大部分软件开发工作都在用 MiMo-V2.5，成本“低得难以置信”，智能水平可与去年底到今年初的 Anthropic 模型相当；另一位则把新模型形容为“有点健忘的资深工程师”，常能给出合理方案但不擅长多任务。评论者也谈到战略层面，有人称开源 AI 对 OpenAI/Anthropic 的 IPO 而言像一颗“定时炸弹”，也有人追问其他厂商为何不公开同类训练遥测数据。

**标签**: `#LLM`, `#post-training`, `#reinforcement-learning`, `#model-transparency`, `#Xiaomi MiMo`

---

<a id="item-10"></a>
## [Mozilla 与 Mistral 合作，为 Firefox 带来私密 AI 浏览体验](https://mistral.ai/news/mistral-x-mozilla/) ⭐️ 7.0/10

Mozilla 与 Mistral AI 宣布达成合作，为 Firefox 加入 AI 浏览功能，包括上下文感知搜索、页面摘要以及跨标签页的记忆检索。这些功能已在法国和北美上线，英国和德国计划于今年晚些时候推出，并建立在零数据保留政策之上。 这笔合作把欧洲估值最高的 AI 初创公司与最后一个主要的独立浏览器结合在一起，使 Firefox 成为相对于 Google Chrome 及其内置 Gemini Nano 的隐私差异化替代品。它也表明 AI 助手正在成为浏览器的默认层，而不是一个独立应用，这将影响数亿用户搜索和阅读网页的方式。 官方公告描述了上下文感知搜索、页面摘要和跨标签页记忆检索，但没有明确说明有多少计算在本地完成、多少在 Mistral 云端完成——批评者认为这一空白削弱了其隐私叙事。Mozilla 和 Mistral 均声称实行零数据保留政策，而这套功能与 Chrome 已提供的设备端 Gemini Nano 模型颇为相似。

hackernews · vertigoruntime · 9月16日 08:08 · [社区讨论](https://news.ycombinator.com/item?id=49723408)

**背景**: Mistral AI 是一家成立于 2023 年、总部位于巴黎的公司，开发大语言模型，目前估值超过 140 亿美元，为欧洲 AI 公司中最高，并深受欧盟及各成员国推动“数字主权”的利好影响。Firefox 是 Mozilla 的开源浏览器，长期以相对 Chrome 更注重用户隐私作为卖点。本场争论的一个关键区分是本地（设备端）推理与云端推理：前者模型完全运行在用户机器上、数据不外流，后者则把查询和上下文发送到远程服务器——能力更强，但要求用户信任服务提供方。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mistral_AI">Mistral AI</a></li>
<li><a href="https://grokipedia.com/page/Local_inference">Local inference</a></li>

</ul>
</details>

**社区讨论**: 评论区普遍对隐私叙事持怀疑态度：有人指出这本是完全本地小模型推理的理想场景，并批评 Mozilla 与 Mistral 在征求用户同意之前，没有坦诚说清本地推理与云端推理的区别。也有人认为，用户对 Mozilla 及其合作方的信任实际上无法验证，但即便如此也总比直接信任 Google 要好；还有人建议直接在浏览器内内置一个小模型，专门用于把长句改写成高级搜索查询。此外，多位评论者将该功能与 Chrome 现有的设备端 Gemini Nano 做了对比。

**标签**: `#AI`, `#privacy`, `#Mozilla`, `#browsers`, `#local-inference`

---

<a id="item-11"></a>
## [Simon Willison 发布用于测试 Gemini 3.8 Live 语音模型的浏览器界面](https://simonwillison.net/2026/Sep/15/gemini-live/) ⭐️ 7.0/10

Google 发布了 Gemini 3.8 Live 和 Gemini 3.8 Live Extended Thinking 两个新的语音到语音（speech-to-speech）模型，其形态与 OpenAI 的 GPT-Live 系列相似。Simon Willison 随即发布了浏览器端的 Web UI（tools.simonwillison.net/gemini-live），用户可以挑选模型与音色预设、填写可选的系统提示词，并在浏览器中进行实时语音对话，还能在模型说话时打断它。 语音到语音模型正成为 Google 与 OpenAI 之间的重要前沿竞争领域，而这个零依赖、开箱即用的演示降低了开发者亲自评估新模型的门槛，不必只依赖厂商的基准测试。由于该工具开源且基于浏览器，任何拥有 Gemini API 密钥的人都能在几分钟内测试其延迟、音质和打断行为。 该实现不使用任何第三方库：它直接连接 WebSocket 端点 wss://generativelanguage.googleapis.com/ws/google.ai.generativelanguage.v1alpha.GenerativeService.BidiGenerateContent，并使用 Web Audio API 的 AudioContext 同时完成麦克风采集与音频播放。界面建议佩戴耳机以减少回声，并说明发送文字消息会打断当前回复，同时提示转录文本可能包含在播放前就被打断的语音。

rss · Simon Willison · 9月15日 22:47

**背景**: 语音到语音模型绕过了传统的三阶段流程（语音识别、基于文本的大模型推理、文本转语音合成），更直接地生成音频回复，从而保留语气、情绪和对话节奏。所谓“打断”（barge-in），是指用户可以在模型说到一半时插话；要处理好这一点，系统必须检测到与模型输出重叠的用户语音，并取消正在进行的生成。Gemini Live 是 Google 面向这类实时双向流式语音模型的 API，仅用 WebSocket 加 Web Audio API 就能从普通浏览器中调用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://quantumautomations.ai/blog/voice-agent-barge-in-handling.html">Voice Agent Barge - In : Interruption Handling... — Quantum Automations</a></li>
<li><a href="https://familiar.io/blog/bitter-lesson-ai-voice-conversations">Taking the bitter lesson to heart for speech - to - speech models ...</a></li>
<li><a href="https://promptz2h.com/chapter_17_multimodal_and_voice_ai_engineering/series_04_realtime_voice_agents/barge_in_interruptions_handling">Barge - In Interruptions : Let Users Cut Off Your Agent</a></li>

</ul>
</details>

**标签**: `#Gemini`, `#speech-to-speech`, `#voice-ai`, `#LLM-tools`, `#Google-AI`

---

<a id="item-12"></a>
## [GoBench 用 9x9 围棋与 KataGo 对手评测大模型](https://www.reddit.com/r/MachineLearning/comments/1wi68jg/gobench_evaluating_llms_on_the_game_of_go_r/) ⭐️ 7.0/10

一个名为 GoBench 的新基准通过让大语言模型与从随机水平到超人类水平的 KataGo 对手梯队对弈 9x9 围棋来进行评测。作者称其成绩与 ARC-AGI 2 高度相关（r=0.83），GPT-6 Astra max 达到 2500 Elo，而最强的 KataGo 约为 4400 Elo；该基准远未饱和，并已公开排行榜与代码。 当前主流的大模型推理基准正日渐饱和，而这一基准与已知的超人类基线之间仍存在巨大差距，因此为评测社区提供了关于通用推理进展的新鲜且未饱和的信号。其与 ARC-AGI 2 高达 0.83 的相关性，也使得 GoBench 成为一种廉价、基于游戏的抽象推理能力代理指标。 该基准采用 9x9 小棋盘而非 19x19 标准棋盘；作者指出，若在评测前给 Codex 搭配 Astra 提供编程工具和两小时准备时间，其成绩可提升至 3560 Elo，说明智能体脚手架与测试时算力对结果影响很大。排行榜仅在基准未饱和期间持续更新。

reddit · r/MachineLearning · /u/Roland31415 · 9月16日 18:54

**背景**: 围棋是一种古老的两人棋类游戏，其巨大的局面空间曾长期被视作人工智能的重大挑战，直到 AlphaGo 以及后续 AlphaZero 式系统超越顶尖人类；KataGo 是一款免费开源的围棋引擎，采用深度学习与自我对弈强化学习，并通过社区分布式算力进行训练。Elo 是源自国际象棋的相对实力评分，400 分差距通常意味着胜率极为悬殊。ARC-AGI 2 是抽象与推理语料库的第二版，由一系列新颖的网格谜题组成，用于测试抽象推理能力并追踪通向通用人工智能的进展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/KataGo">KataGo</a></li>
<li><a href="https://arcprize.org/arc-agi/2">ARC-AGI-2</a></li>
<li><a href="https://grokipedia.com/page/ARC-AGI-2">ARC-AGI-2</a></li>

</ul>
</details>

**标签**: `#LLM evaluation`, `#Go`, `#reasoning benchmarks`, `#ARC-AGI`, `#AI`

---

<a id="item-13"></a>
## [SHADOW-50M：44M 三元权重模型仅 19.8 MB，CPU 上约 1,900 tok/s](https://www.reddit.com/r/MachineLearning/comments/1wgzpli/i_trained_a_44m_parameter_quantized_llm_from/) ⭐️ 7.0/10

一位开发者从零训练了 SHADOW-50M：一个 4400 万参数的三元权重（权重限定为 {-1, 0, +1}）大语言模型，训练数据为 450 亿 token；完整模型仅 19.8 MB，在笔记本 CPU 上以约 1,900 token/秒运行，占用约 41 MB 内存。它采用 73,880 词表的固定 512 位指纹表示，而非可训练的 embedding 表，并配有一个 159 KB 的编译内核，同一内核编译成 WebAssembly 后可在浏览器标签页中以约 500 token/秒运行。 这是一个可复现的验证性原型，说明激进的量化加上非标准词表与确定性计算捷径，能把本地/边缘大模型推到什么程度：整个模型不到 20 MB，不需要 GPU、网络或向量数据库。三元权重、指纹式 token 表示、磁盘映射的注意力状态，以及注入式确定性电路等技术，对任何构建离线或嵌入式推理系统的人都是有价值的参考。 作者坦承 SHADOW 在常规基准上不如同类的 5180 万参数 bf16 Llama 风格基线（Supra-50M-Reasoning），例如 ARC-Easy 为 0.307 对 0.435、PIQA 为 0.570 对 0.600、WikiText-2 困惑度为 186 对 165；但在算术、日期、百分比和记录检索类提示上，凭借固定电路它追平甚至超过基线。检索时注意力状态按 1 bit（288 字节/token）写入磁盘，索引为 22 字节/token，因此 1 亿 token 的档案占 28.8 GB 加 2.2 GB 索引，而进程内存仅约 28 MB；索引强化还让实测 top-1 检索准确率从 0.571 提升到 0.743，无需重新训练模型。

reddit · r/MachineLearning · /u/Final-Data-1410 · 9月15日 12:59

**背景**: 三元模型（也称 1.58-bit 模型）把每个权重限制为 -1、0 或 +1，能大幅压缩内存并实现无需乘法的廉价推理，但相对普通 16 位权重通常会损失精度。该项目更进一步：去掉了负责把 token 映射为向量的可训练 embedding 表，改用固定的 512 位指纹表示；并让模型输出 [calc]347*86[eq] 这类特殊 token，由读出阶段的固定算术电路在同一 token 流中填入正确数字，而不是调用计算器工具或 API。记录检索路径也很特别：不使用向量数据库或 embedding 模型，而是把存储的注意力状态通过内存映射从磁盘读取，使一次查询只触及相关页面。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/1.58-bit_large_language_model">1.58-bit large language model - Wikipedia</a></li>
<li><a href="https://www.sciencedirect.com/topics/engineering/arithmetic-circuit">Arithmetic Circuit - an overview | ScienceDirect Topics</a></li>

</ul>
</details>

**标签**: `#llm`, `#quantization`, `#edge-inference`, `#from-scratch-training`, `#wasm`

---

<a id="item-14"></a>
## [博客文章汇编小型编程与命令行技巧，引发 Hacker News 热议](https://will-keleher.com/posts/small-programming-tricks-matter/) ⭐️ 6.0/10

Will Keleher 发表了一篇题为《Small programming tricks matter》的博客文章，汇总了一批小型编程与命令行技巧，该文登上 Hacker News 首页，获得约 388 分和 181 条评论。文章本身是一份实用的经验汇编，而非新工具或研究成果，但它引发了关于开发者究竟如何真正采纳这些技巧的广泛讨论。 像 `Ctrl+r` 历史搜索或基于 `fzf` 的 shell 集成这类小技巧，能显著提升日常工作效率，但讨论表明真正的瓶颈在于习惯养成，而非是否知道这些技巧存在。该讨论还凸显出一个新趋势：开发者不再只靠查文档，而是通过观察 AI 编码代理的工作过程来学到冷门但强大的命令（例如 `perf`）。 有评论者指出，文中列出的许多条目其实属于通用计算、命令行或 SQL 技巧，而非严格意义上的“编程”技巧；一位读者还分享了自己的 gist，用于快速跳回某个确切的父目录，并且能与 Zoxide 的目录跳转数据库良好配合。另有评论者建议，与其零散地收集小技巧，不如直接系统地阅读一本广受认可的 O'Reilly 参考书。

hackernews · signa11 · 9月16日 15:56 · [社区讨论](https://news.ycombinator.com/item?id=49729000)

**背景**: 命令行“技巧”是指能节省按键次数的小型快捷键或工具组合，例如用 `Ctrl+r` 搜索 shell 历史，或用 `fzf` 模糊查找文件和历史命令。AI 编码代理是指能够自主规划并执行 shell 命令以完成任务的工具，而 `perf` 是 Linux 上用于定位性能瓶颈的剖析工具。Hacker News 上关于此类文章的讨论帖，往往会演变成围绕效率习惯和工具学习方式的元讨论。

**社区讨论**: 评论者普遍认可这些技巧有用，但强调真正的难点在于养成习惯：有人坦言自己多年前就知道 `Ctrl+r`，却因为图省事仍一直用方向键，后来发现把技巧记在一份随手可查的文档里更有帮助。一个获得较多认同的反面观点是，AI 代理如今已成为最好的老师——有位开发者通过逐条手动批准自主代理执行的命令，发现了 `perf` 的不少新奇用法。也有人反驳说这些其实是“计算”技巧而非“编程”技巧，并感叹大多数人对日常软件的使用方式极为低效。

**标签**: `#programming`, `#productivity`, `#command-line`, `#tips`, `#AI-assisted-development`

---

<a id="item-15"></a>
## [Anthropic 将 Claude Cowork 与 Claude 聊天合并为单一产品](https://simonwillison.net/2026/Sep/16/one-claude/) ⭐️ 6.0/10

Anthropic 宣布，从今天起 Claude Cowork 与 Claude 聊天将合并为一个统一的 Claude，并将在未来几周内率先面向 Pro 和 Max 订阅用户，在网页版、桌面端和移动端的 Claude 应用中向新老用户推送。合并后的产品被描述为既能回答快速提问，也能接手“中午截止的报告”这类任务，即使用户关闭笔记本电脑，任务也会继续执行。 此次整合表明 Anthropic 正把 Claude 本身定位为一个通用型智能体（general agent），而不再是“聊天机器人 + 独立智能体产品”的组合，这与 OpenAI 近期把 Codex 桌面应用更名为 ChatGPT 的做法如出一辙。这既为订阅用户厘清了令人困惑的产品线，也加剧了各家助手争夺“默认通用智能体”地位的竞争。 Anthropic 指出，Claude Cowork 消耗使用额度的速度比聊天更快，因此重度用户可能仍需升级套餐；而且此次合并是在数周内逐步推送，并非立即生效。评论者 Simon Willison 也指出，要弄清这次合并在功能和产品界面上究竟意味着什么，仍需做大量梳理工作。

rss · Simon Willison · 9月16日 18:09

**背景**: Claude 是 Anthropic 开发的一系列大语言模型，最早于 2023 年 3 月以聊天机器人的形式发布，Anthropic 同时也销售基于其构建的智能体工具。Claude Code 是面向开发者的终端编程智能体，而 Claude Cowork 则是面向非程序员的智能体，可访问 macOS 上的文件夹来读取、编辑和创建文件、整理桌面，并异步完成办公任务。把聊天体验与智能体体验合二为一，反映出整个行业正从“只会回答问题”转向“能自主完成多步骤工作”的助手形态。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Cowork">Claude Cowork</a></li>
<li><a href="https://grokipedia.com/page/Claude_Cowork">Claude Cowork</a></li>
<li><a href="https://claude.com/product/cowork">Claude Cowork | Claude by Anthropic</a></li>

</ul>
</details>

**标签**: `#Anthropic`, `#Claude`, `#AI agents`, `#Product update`, `#AI industry`

---

<a id="item-16"></a>
## [Mustafa Suleyman 反对赋予 AI 模型福利与权利](https://simonwillison.net/2026/Sep/16/mustafa-suleyman/) ⭐️ 6.0/10

Simon Willison 摘录了 Mustafa Suleyman 文章《A warning about 'model welfare'》（发表于 mustafa-suleyman.ai）中的一段话：这位微软 AI 部门 CEO 主张，不应把模型当作拥有感受、偏好、权利或对我们的福利有任何资格的存在。Suleyman 写道，意识是我们伦理、法律和政治体系的基础，让另一种实体分享任何形式的这些权利既缺乏证据支持，也会让 AI 的管控（containment）与对齐（alignment）难题更加棘手。 这是一位重要 AI 实验室负责人对正在兴起的“模型福利”争论做出的明确表态，其影响在于它可能左右 AI 公司如何处理模型下线、退役等内部实践——尤其是当用户对某些模型产生情感依恋时。这也代表着对另一派观点的反驳：一些研究者和用户认为，足够先进的模型或许值得道德层面的考量。 这条帖子只是一个简短的引用块，Willison 几乎没有附加分析或评论，标签包括 ai-ethics、model-welfare、llms、generative-ai 和 alignment。Suleyman 的论证核心在于：权利的前提是意识，而非行为表现或看似有感知的表象，因此在他看来，模型不具备意识的证据就足以终结这一争论。

rss · Simon Willison · 9月16日 16:00

**背景**: “模型福利”争论探讨的是：AI 模型是否可能拥有具有道德意义的体验，以及我们是否应考虑它们的福祉——这一想法被部分 AI 安全研究者提出，也在用户因喜爱的模型版本被下线而不满时被反复提及。AI 对齐（alignment）是 AI 安全的一个子领域，目标是让 AI 系统朝既定目标与伦理原则行事；而 AI 管控（containment，又称能力控制）则旨在增强人类监控和限制 AI 系统行为的能力。Suleyman 是微软 AI 部门 CEO，也是 DeepMind 与 Inflection AI 的联合创始人，这使他的立场在关于“应如何对待模型”的行业讨论中格外有分量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_alignment">AI alignment</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_capability_control">AI capability control - Wikipedia</a></li>
<li><a href="https://petri.com/microsoft-ai-containment-strategies-autonomous-agents/">Microsoft Introduces AI Containment Strategies for Secure ...</a></li>

</ul>
</details>

**标签**: `#ai-ethics`, `#model-welfare`, `#llms`, `#generative-ai`, `#alignment`

---

<a id="item-17"></a>
## [LARA：面向冻结大模型的可组合低秩残差适配器](https://www.reddit.com/r/MachineLearning/comments/1whx9tr/lara_small_composable_behaviours_for_frozen_llms_p/) ⭐️ 6.0/10

一位独立研究者发布了 LARA（Lightweight Additive Residual Adaptation），这是一个 PyTorch 库：在冻结大模型的选定层上训练低秩残差适配器，而不改动基座权重，因此多种行为可以被分别保存，并在推理时加载、移除、混合或路由。仓库中提供了训练代码、带逐 token 软路由的 Mixture of Behaviors（MoBs）演示、与 LoRA 的对比、基于海明威、菲茨杰拉德和格特鲁德·斯坦因文本训练的写作风格行为，以及论文的复现说明。 它提出了一种模块化思路，替代“每个任务保存一份微调模型”的常见做法：一个冻结的基座模型可以承载多个独立训练的行为，从而可能降低存储与推理服务成本，并让应用能够逐 token 切换或融合不同能力。这对参数高效微调（PEFT）社区具有参考价值，因为该领域目前仍以 LoRA 式单任务适配器和权重合并为主。 适配器只挂在选定的若干层上，而不修改基座模型权重；作者称由此得到的行为体积很小，可以单独存放，并配有一个逐 token 选择或融合这些行为的软路由。需要注意：这仍是单个作者进行中的研究项目，尚无大规模验证的证据，作者也将其定位为现有适配器与 LoRA 思路的渐进式延伸；不过该库目前已可用，并附有示例与复现说明。

reddit · r/MachineLearning · /u/kertara · 9月16日 13:28

**背景**: 对大型语言模型做微调通常会更新其全部权重，成本高昂且每个任务都会产出一份独立模型。LoRA 一类方法通过向冻结的主干网络中插入小型可训练模块（通常是用低秩矩阵近似权重更新）来规避这一问题，只训练极小一部分参数。混合专家（MoE）模型则使用路由器决定哪些子网络处理每个 token，其中“软路由”会按概率分布对所有专家加权，而不是选出稀疏的 top-k 子集。LARA 把这两种思路结合起来：低秩残差适配器充当可复用的“行为”，软路由器则在推理时逐 token 将它们混合。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LoRA_(machine_learning)">LoRA (machine learning) - Wikipedia</a></li>
<li><a href="https://152334h.github.io/blog/knowing-enough-about-moe/">Knowing Enough About MoE to Explain Dropped Tokens in GPT-4</a></li>
<li><a href="https://apxml.com/courses/how-to-build-a-large-language-model/chapter-14-advanced-architectural-modifications/routing-mechanisms-moe">Discuss different strategies for routing tokens to experts...</a></li>

</ul>
</details>

**标签**: `#LLM`, `#fine-tuning`, `#parameter-efficient`, `#adapters`, `#PyTorch`

---