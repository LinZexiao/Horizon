---
layout: default
title: "Horizon Summary: 2026-07-11 (ZH)"
date: 2026-07-11
lang: zh
---

> 从 25 条内容中筛选出 9 条重要资讯。

---

1. [英伟达、CoreWeave、Nebius：GPU 繁荣背后的循环融资](#item-1) ⭐️ 8.0/10
2. [利用 SO_REUSEPORT 和 Peering 将 PgBouncer 吞吐量提升 4 倍](#item-2) ⭐️ 8.0/10
3. [优先使用 SQLite STRICT 表确保数据完整性](#item-3) ⭐️ 7.0/10
4. [女划船手打破男性纪录，独自横渡加州至夏威夷](#item-4) ⭐️ 7.0/10
5. [Nilay Patel：AR 眼镜不可避免侵犯隐私](#item-5) ⭐️ 7.0/10
6. [为什么机器学习研究不限制每作者投稿数？](#item-6) ⭐️ 7.0/10
7. [Ant：新 JavaScript 运行时与生态系统引发争议](#item-7) ⭐️ 6.0/10
8. [通过从零重建 Redis、Git 和数据库来学习](#item-8) ⭐️ 6.0/10
9. [寻求比 HPSv3 更好的人类偏好预测模型](#item-9) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [英伟达、CoreWeave、Nebius：GPU 繁荣背后的循环融资](https://io-fund.com/ai-stocks/nvidia-coreweave-nebius-circular-financing-gpu-boom) ⭐️ 8.0/10

文章揭示了英伟达、CoreWeave 和 Nebius 如何陷入循环融资链条：英伟达投资 CoreWeave 和 Nebius，而后者又大量采购英伟达 GPU，从而推动 AI 基础设施繁荣。 该分析揭示了大规模 GPU 建设背后的金融机制，引发了对其可持续性和盈利能力的质疑。如果循环链条断裂，可能引发 AI 硬件市场的调整。 英伟达向 CoreWeave 投资 20 亿美元获得 9% 股权，但 CoreWeave 仅在 2026 年就计划 350 亿美元的资本支出，英伟达的投资仅覆盖一小部分。类似模式也涉及另一家 AI 云提供商 Nebius。

hackernews · adletbalzhanov · 7月11日 17:21 · [社区讨论](https://news.ycombinator.com/item?id=48873836)

**背景**: 循环融资是一种闭环：投资者向公司提供资金，该公司再将资金用于购买投资者的产品。在 AI 领域，这已变得普遍：大型科技公司投资 AI 初创企业，而初创企业则将资金用于购买投资者的云服务或硬件。英伟达在 GPU 领域的统治地位使其成为此类安排的关键参与者。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://builtin.com/articles/ai-circular-financing">How Circular Financing Is Fueling the AI Boom | Built In</a></li>
<li><a href="https://blogs.cuit.columbia.edu/gjb2124/circular-financing/">The Hidden Risk in AI's Circular Financing Ecosystem</a></li>
<li><a href="https://en.wikipedia.org/wiki/CoreWeave">CoreWeave</a></li>

</ul>
</details>

**社区讨论**: 评论者争论这种融资是否真正属于循环，指出英伟达 20 亿美元投资仅占 CoreWeave 年度资本支出的 5.7%。还有人质疑此类建设的长期盈利能力，而另一个人提醒 Nebius 源自 Yandex，凸显了地缘政治关联。

**标签**: `#Nvidia`, `#GPU`, `#cloud computing`, `#financing`, `#AI infrastructure`

---

<a id="item-2"></a>
## [利用 SO_REUSEPORT 和 Peering 将 PgBouncer 吞吐量提升 4 倍](https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres) ⭐️ 8.0/10

ClickHouse 团队通过利用 SO_REUSEPORT 套接字选项并启用 PgBouncer 内置的 peering 功能，将 PostgreSQL 连接池 PgBouncer 的吞吐量提升了 4 倍。 这一优化使得 PgBouncer 无需额外硬件即可显著提升单机连接处理能力，对于高流量环境中扩展 PostgreSQL 工作负载至关重要。 SO_REUSEPORT 允许多个进程绑定到同一端口，从而分发传入连接；peering 功能则允许取消请求在进程间转发，避免因落在错误进程而失效。

hackernews · saisrirampur · 7月11日 15:28 · [社区讨论](https://news.ycombinator.com/item?id=48872874)

**背景**: PgBouncer 是 PostgreSQL 的轻量级连接池，常用于管理数据库连接。传统上，运行多个 PgBouncer 实例需要不同的端口或复杂的负载均衡。SO_REUSEPORT 是 Linux 内核 3.9 引入的套接字选项，允许多个套接字共享同一端口，简化了服务器进程的水平扩展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lwn.net/Articles/542629/">The SO_REUSEPORT socket option [LWN.net]</a></li>
<li><a href="https://postgrespro.com/docs/postgrespro/current/pgbouncer">Postgres Pro Standard : Documentation: 18: pgbouncer</a></li>

</ul>
</details>

**社区讨论**: 社区成员讨论了 Odyssey 和 pgdog 等替代工具，并询问了 PgBouncer 中 peering 配置的简便性。部分用户指出，在 Kubernetes 中运行 PgBouncer 已经使得多进程部署变得简单直接。

**标签**: `#pgbouncer`, `#performance`, `#postgresql`, `#connection pooling`, `#scaling`

---

<a id="item-3"></a>
## [优先使用 SQLite STRICT 表确保数据完整性](https://evanhahn.com/prefer-strict-tables-in-sqlite/) ⭐️ 7.0/10

文章主张开发者应使用 SQLite 的 STRICT 表模式来强制列类型并提高数据完整性，而不是依赖默认的灵活类型系统。 这很重要，因为 STRICT 表解决了 SQLite 的一个常见批评——缺乏类型强制——使其更适合需要健壮数据完整性的应用，同时仍受益于 SQLite 的简洁性。 STRICT 表自 SQLite 3.37.0 起可用，需要逐表显式声明；它们强制执行严格的类型检查，但不支持所有数据类型如 DATE，可能需要将日期存储为 TEXT 或 INTEGER。

hackernews · ingve · 7月11日 17:33 · [社区讨论](https://news.ycombinator.com/item?id=48873940)

**背景**: SQLite 以其灵活类型系统闻名，列数据类型仅为提示；任何值都可以插入任何列而不考虑声明的类型。这种设计是有意为之，如'灵活类型'哲学所述，但当同一数据库被多个应用访问或迁移模式时可能导致细微错误。STRICT 表提供了一种可选替代方案，在插入时拒绝类型不匹配，符合传统 SQL 的期望。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sqlite.org/stricttables.html">STRICT Tables</a></li>
<li><a href="https://antonz.org/sqlite-strict-tables/">STRICT tables in SQLite</a></li>

</ul>
</details>

**社区讨论**: 社区评论显示了分歧：一些开发者强烈希望将 STRICT 设为默认以获得更好的数据完整性，而另一些则基于 SQLite 的使用场景（如嵌入式、单应用）为其灵活类型辩护。值得注意的观点包括 STRICT 表缺少日期支持，以及 SQLite 团队表示严格的类型强制并不总是有益。

**标签**: `#SQLite`, `#data integrity`, `#database schemas`, `#type enforcement`, `#software engineering best practices`

---

<a id="item-4"></a>
## [女划船手打破男性纪录，独自横渡加州至夏威夷](https://www.theguardian.com/us-news/2026/jul/04/california-hawaii-rowing-solo-journey) ⭐️ 7.0/10

一名女划船手完成了从加州到夏威夷的最快单人横渡，比之前的男性纪录快了六天。 这一成就突显了单人横渡大洋所需的非凡身体和心理耐力，并挑战了极限耐力运动中的性别刻板印象。 划船手 Kelsey Pfendler 用了 44 天完成了约 2400 海里的航程，比之前的男性纪录快了六天。她的船长度为 21 英尺，宽度 5.5 英尺，设计为自给自足。

hackernews · speckx · 7月11日 17:03 · [社区讨论](https://news.ycombinator.com/item?id=48873692)

**背景**: 单人海洋划船是最具挑战性的耐力挑战之一，需要数月的准备和极强的韧性。划船者需要面对危险的海浪、孤独以及携带所有补给的需求。加州到夏威夷的路线是经典但艰难的穿越，因为盛行风和洋流的存在。

**社区讨论**: 评论者对所需的心理和身体耐力表示敬畏，有人指出即使是短距离穿越也很困难。另一个人强调 Kelsey 是完成该穿越的最快人类，超过了男性纪录。还有人对船只设计和后勤产生了好奇。

**标签**: `#rowing`, `#endurance`, `#ocean crossing`, `#human achievement`, `#record`

---

<a id="item-5"></a>
## [Nilay Patel：AR 眼镜不可避免侵犯隐私](https://simonwillison.net/2026/Jul/10/nilay-patel/#atom-everything) ⭐️ 7.0/10

Nilay Patel 在 The Vergecast 上表示，增强现实眼镜需要始终开启的摄像头和云端处理，导致隐私侵犯不可避免，并质疑这一社会成本是否值得。 这一观点挑战了人们对 AR 作为下一代计算平台的普遍乐观态度，指出了可能影响产品设计和监管的根本性伦理权衡。 Patel 指出，目前没有足够小到能放在眼镜腿里的芯片可以本地处理实时视频，因此数据必须发送到云端，否则设备必须像 Apple Vision Pro 一样笨重。

rss · Simon Willison · 7月10日 17:05

**背景**: 增强现实眼镜将数字信息叠加到现实世界上。它们需要摄像头捕捉用户视野，以及强大的处理器实时分析和渲染图形。当前的硬件限制迫使要么采用云端处理（引发隐私问题），要么采用笨重的设计。基于云的 AR 眼镜人脸识别已成为活跃的研究领域。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ieeexplore.ieee.org/document/10322211/">Cloud-Based Face Recognition for Augmented Reality Glasses | IEEE Conference Publication | IEEE Xplore</a></li>
<li><a href="https://www.researchgate.net/publication/391142373_Energy_Efficient_ARVR_Edge_Processing_Architecture_and_Optimization">(PDF) Energy Efficient AR /VR Edge Processing : Architecture and...</a></li>

</ul>
</details>

**标签**: `#augmented reality`, `#privacy`, `#cloud computing`, `#technology ethics`, `#hardware limitations`

---

<a id="item-6"></a>
## [为什么机器学习研究不限制每作者投稿数？](https://www.reddit.com/r/MachineLearning/comments/1usq43t/why_doesnt_the_ml_research_community_limit_the/) ⭐️ 7.0/10

Reddit 上的一篇帖子质疑，为什么机器学习研究社区不限制每名作者的投稿数量，以管理审稿工作量，并引用了安全（CCS）和计算机体系结构（DAC）会议的成功例子。 这个问题直接影响机器学习会议（如使用 ACL Rolling Review (ARR)的会议）的审稿质量，高投稿量给审稿人带来压力。限制每作者投稿量有望提高审稿质量并减少审稿人倦怠。 帖子指出，其他领域多年来已成功使用每作者限制，例如安全领域的 ACM CCS 和体系结构领域的 DAC。ML 社区的文化阻力可能源于其对快速迭代和开放投稿的强调。

reddit · r/MachineLearning · /u/alafaya101 · 7月10日 14:59

**背景**: ACL Rolling Review (ARR) 是计算语言学和 NLP 的同行评审平台，投稿数量激增导致审稿人超负荷。在安全等领域，如 CCS 会议将每名作者的投稿限制在少量（例如 2-3 篇），以保持审稿流程可控。该帖子质疑为什么 ML 社区不采用类似政策，该社区常因投稿过多而面临审稿质量低下的问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="http://aclrollingreview.org/cfp">CALL FOR PAPERS – ACL Rolling Review – A peer review platform for the Association for Computational Linguistics</a></li>
<li><a href="https://dl.acm.org/doi/proceedings/10.1145/2810103?preflayout=flat">Proceedings of the 22nd ACM SIGSAC Conference on Computer and...</a></li>

</ul>
</details>

**标签**: `#ML research`, `#peer review`, `#submission policies`, `#community discussion`

---

<a id="item-7"></a>
## [Ant：新 JavaScript 运行时与生态系统引发争议](https://antjs.org/) ⭐️ 6.0/10

Ant 是一个从零构建、拥有自有引擎的 JavaScript 运行时，并附带包管理器、包注册表、部署平台和桌面应用框架。它旨在成为现有 JavaScript 栈的一致替代方案，同时保持兼容性。 如果成功，Ant 可能提供一个轻量级、集成的生态系统，挑战 Node.js、Deno 和 Bun 等现有运行时。然而，社区对其起源和可信度的怀疑可能阻碍采用。 Ant 是一个仅 9 MB 的单一二进制文件，支持 npm 包、TypeScript、VM 隔离沙箱和 WebAssembly。它还引入了 ants.land 包注册表和一个名为 Ant Desktop 的类似 Electron 的桌面应用构建器。

hackernews · theMackabu · 7月11日 20:07 · [社区讨论](https://news.ycombinator.com/item?id=48875377)

**背景**: JavaScript 运行时是在浏览器之外执行 JavaScript 代码的环境，常见的例子有 Node.js、Deno 和 Bun。从零构建运行时是一项巨大的工程，通常需要一个工程师团队多年的努力。Ant 声称是从零构建的，但社区成员指出它最初使用了来自 Elk 引擎的 AGPL 许可代码，这引发了关于透明度和许可问题的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://antjs.org/">Ant, a lightweight JavaScript runtime</a></li>
<li><a href="https://github.com/themackabu/ant/">GitHub - theMackabu/ant: javascript for 🐜's, a tiny runtime with big ambitions</a></li>
<li><a href="https://news.ycombinator.com/item?id=48875377">Show HN: Ant – A JavaScript runtime and ecosystem | Hacker News</a></li>

</ul>
</details>

**社区讨论**: 社区评论反应不一：有人发现它基于 AGPL 代码库（Elk）后质疑其“从零构建”的说法，也有人因公司网站破损和使用个人 GitHub 账户而对作者的可信度表示担忧。还有关于命名与 Apache Ant 冲突的顾虑，以及对其性能声称在成熟的运行时面前是否成立的怀疑。

**标签**: `#JavaScript`, `#runtime`, `#ecosystem`, `#controversy`, `#open-source`

---

<a id="item-8"></a>
## [通过从零重建 Redis、Git 和数据库来学习](https://shipthatcode.com/) ⭐️ 6.0/10

一个免费的网站提供了从零重建 Redis、Git 和数据库的动手项目，为学习系统内部原理提供了实践方法。 该资源免费开放了深度的系统知识，可能会降低开发者理解核心基础设施的门槛。然而，关于原创性和与 CodeCrafters 等现有平台相似性的担忧可能会影响其影响。 这些项目涵盖三个常见系统：Redis（内存数据存储）、Git（版本控制）和一个通用数据库。用户需要注册，但有人报告遇到'超出速率限制'的错误。

hackernews · acley · 7月11日 13:40 · [社区讨论](https://news.ycombinator.com/item?id=48871973)

**背景**: 从零重建知名系统是一种经典学习技巧，帮助开发者理解复杂内部原理。CodeCrafters 等平台和《Building Git》等书籍推广了这种方法，而这个新资源是免费的。

**社区讨论**: 评论质疑其原创性，认为内容可能抄袭现有来源并通过 LLM 清洗。还有人质疑它与 CodeCrafters 的区别，但有人欣赏它是免费的。

**标签**: `#learning`, `#systems`, `#tutorial`, `#hands-on`

---

<a id="item-9"></a>
## [寻求比 HPSv3 更好的人类偏好预测模型](https://www.reddit.com/r/MachineLearning/comments/1utdj1f/predicting_human_preference_for_generated_image/) ⭐️ 6.0/10

imagebench.ai 的作者测试了 HPSv3 在生成图像对上的偏好预测能力，发现了其局限性，并向社区寻求更好的替代方案。 选择合适的人类偏好模型对于评估和改进文本到图像生成至关重要，因为它直接影响自动反馈的质量。 HPSv3 基于包含 108 万文本-图像对和 117 万成对比较的数据集构建，但作者报告它在实际使用中有许多局限性。

reddit · r/MachineLearning · /u/dh7net · 7月11日 07:36

**背景**: 人类偏好分数是基于人工标注训练的自动评估指标，用于判断 AI 生成图像的质量。HPSv3 是这类模型系列中的最新版本，但没有一个模型是完美的。替代方案包括 PickScore、HPSv2 和 VisionReward，它们各有不同的优势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mizzenai.github.io/HPSv3.project/">HPSv 3 : Towards Wide-Spectrum Human Preference Score</a></li>
<li><a href="https://arxiv.org/html/2508.03789v2">HPSv 3 : Towards Wide-Spectrum Human Preference Score</a></li>

</ul>
</details>

**标签**: `#image generation`, `#human preference`, `#evaluation`, `#HPSv3`, `#machine learning`

---