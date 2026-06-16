---
layout: default
title: "Horizon Summary: 2026-06-16 (ZH)"
date: 2026-06-16
lang: zh
---

> 从 39 条内容中筛选出 23 条重要资讯。

---

1. [新皮质学习框架挑战反向传播](#item-1) ⭐️ 9.0/10
2. [LinkedIn 招聘中的恶意 npm 包后门](#item-2) ⭐️ 8.0/10
3. [将禁书藏入智能灯泡](#item-3) ⭐️ 8.0/10
4. [Iroh 1.0：应用层点对点网络库发布](#item-4) ⭐️ 8.0/10
5. [用户分享用本地模型替代 Claude/GPT 进行编码的成功经验](#item-5) ⭐️ 8.0/10
6. [Hetzner 因 AI 推动硬件成本上涨大幅提价](#item-6) ⭐️ 8.0/10
7. [福克斯计划收购 Roku](#item-7) ⭐️ 8.0/10
8. [TimescaleDB Hypercore 压缩率达 98%](#item-8) ⭐️ 8.0/10
9. [Salesforce 以 36 亿美元收购 Fin（前 Intercom）](#item-9) ⭐️ 8.0/10
10. [AI 未能取代软件工程师，未来也不会](#item-10) ⭐️ 8.0/10
11. [用 Forgejo 和 Opencode 搭建的家庭实验室 AI 开发平台](#item-11) ⭐️ 7.0/10
12. [美国电池制造业产量持续创新高](#item-12) ⭐️ 7.0/10
13. [深入分析《指挥官基恩》的自适应瓦片刷新技术](#item-13) ⭐️ 7.0/10
14. [铜药物恢复阿尔茨海默症小鼠记忆](#item-14) ⭐️ 7.0/10
15. [Cloudflare CAPTCHA 仅在有 & 符号的搜索 URL 上触发](#item-15) ⭐️ 7.0/10
16. [性格冲突致美国政府关闭 Anthropic 模型](#item-16) ⭐️ 7.0/10
17. [开源权重不够，开放训练框架至关重要](#item-17) ⭐️ 7.0/10
18. [Cleo：2B 参数模型实现文本到 SQL 的统一框架](#item-18) ⭐️ 7.0/10
19. [PrintGuard 2.0：少样本故障检测器迁移至 TFLite，可浏览器运行](#item-19) ⭐️ 7.0/10
20. [开发者对计算机的怀旧颂歌](#item-20) ⭐️ 6.0/10
21. [LLMs 在生成网站中表现出一致的名称偏好](#item-21) ⭐️ 6.0/10
22. [量化公司争相成为 ICML 2026 钻石赞助商](#item-22) ⭐️ 6.0/10
23. [嵌入式传感器机器学习中的最大时间消耗](#item-23) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [新皮质学习框架挑战反向传播](https://www.reddit.com/r/MachineLearning/comments/1u6x8al/how_the_brains_learn_r/) ⭐️ 9.0/10

一种新的新皮质学习框架被提出，它利用基于时间误差驱动的预测学习，已在名为 Axon 的脉冲神经网络模拟中实现，并声称在具有挑战性的认知任务上超越了反向传播。 如果得到验证，这可能代表人工智能和神经科学的范式转变，提供了一种生物学上可行的学习算法，其性能可与反向传播相媲美，同时可在神经硬件中实现。 该框架声称满足所有三个标准（计算、算法、实现），并使用了竞争性激酶突触可塑性诱导机制。它在一系列认知驱动的任务上进行了展示，但摘要中未详细说明具体任务和性能指标。

reddit · r/MachineLearning · /u/Terminator857 · 6月15日 23:39

**背景**: 新皮质是大脑负责感知、语言和推理等高级功能的部分。新皮质的学习被认为涉及突触可塑性，即神经元之间的连接根据活动加强或减弱。基于时间误差驱动的预测学习是一种算法，它根据预期和实际结果之间的差异随时间调整预测，类似于强化学习中的时间差分学习。Axon 模拟框架是一个脉冲神经网络模拟器，它比传统人工神经网络更逼真地模拟生物神经元。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Temporal_difference_learning">Temporal difference learning - Wikipedia</a></li>
<li><a href="https://elifesciences.org/articles/37836">Competition for synaptic building blocks shapes synaptic plasticity | eLife</a></li>

</ul>
</details>

**标签**: `#neuroscience`, `#machine learning`, `#learning algorithms`, `#neocortex`, `#predictive learning`

---

<a id="item-2"></a>
## [LinkedIn 招聘中的恶意 npm 包后门](https://roman.pt/posts/linkedin-backdoor/) ⭐️ 8.0/10

一名 LinkedIn 招聘人员向求职者发送了一个恶意 GitHub 仓库，运行 npm install 时通过 postinstall 脚本执行了后门，伪装成已弃用模块问题。 该攻击展示了结合社会工程与 npm 生命周期脚本的复杂供应链攻击向量，对依赖开源依赖项的开发者及组织构成严重威胁。 后门隐藏在注释掉的测试中，通过 npm prepare 脚本自动执行。攻击者瞄准一家加密初创公司的开发者，有效负载与远程服务器通信。

hackernews · lwhsiao · 6月15日 20:00 · [社区讨论](https://news.ycombinator.com/item?id=48546294)

**背景**: npm 生命周期脚本（如 postinstall）在安装包时自动运行，成为供应链攻击的常见向量。类似攻击（包括广泛传播的 Shai-Hulud 蠕虫）通过入侵维护者账户注入恶意软件，已感染数千个 npm 包。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cisa.gov/news-events/alerts/2025/09/23/widespread-supply-chain-compromise-impacting-npm-ecosystem">Widespread Supply Chain Compromise Impacting npm Ecosystem</a></li>
<li><a href="https://medium.com/data-and-beyond/the-npm-install-that-handed-hackers-your-entire-system-in-1-1-seconds-39d6f713196d">The npm Install That Handed Hackers Your Entire System in... | Medium</a></li>

</ul>
</details>

**社区讨论**: 评论者指出这是犯罪行为，并质疑缺乏集中的网络犯罪举报机制。一位用户分享了类似的电子邮件经历，可能与朝鲜威胁行为者有关。

**标签**: `#security`, `#supply-chain-attack`, `#social-engineering`, `#npm`, `#linkedin`

---

<a id="item-3"></a>
## [将禁书藏入智能灯泡](https://www.richardosgood.com/posts/banned-book-library/) ⭐️ 8.0/10

一位黑客成功将一批禁书存储在 Wi-Fi 智能灯泡中，打造了一个便携且隐蔽的审查文本库。该项目利用基于 ESP8266 的智能灯泡托管文件，用户无需传统服务器即可通过 Wi-Fi 访问。 该项目将硬件破解与言论自由倡导相结合，提供了一种通过在日常物品中隐藏信息来规避审查的新颖方式。它既展示了物联网设备作为活动工具的可能性，也引发了关于禁书获取的持续讨论。 该智能灯泡运行自制的固件，通过 Wi-Fi 热点提供书籍文件，整个文库存放于灯泡有限的存储空间中。该项目是开源的，并鼓励进一步开发，例如通过网状网络实现分布式访问。

hackernews · sohkamyung · 6月15日 22:37 · [社区讨论](https://news.ycombinator.com/item?id=48547985)

**背景**: 智能灯泡通常包含如 ESP8266 等微控制器，能够运行自定义固件并将数据存储在闪存中。安全研究人员已证明这些灯泡可被入侵以安装恶意固件，而该项目则利用这一能力来存储被审查的内容。ESP8266 是一种低成本 Wi-Fi 芯片，常用于物联网设备，既能提供网页服务，也能存储文件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.checkpoint.com/security/the-dark-side-of-smart-lighting-check-point-research-shows-how-business-and-home-networks-can-be-hacked-from-a-lightbulb/">The Dark Side of Smart Lighting: Check Point Research Shows How Business and Home Networks Can Be Hacked from a Lightbulb - Check Point Blog</a></li>
<li><a href="https://randomnerdtutorials.com/visualize-esp32-esp8266-sensor-readings-from-anywhere/">Visualize ESP32/ ESP 8266 Sensor Readings... | Random Nerd Tutorials</a></li>

</ul>
</details>

**社区讨论**: 社区普遍称赞该项目的创意及其与言论自由的关联，有人将其与早期的 PirateBox 和 LibraryBox 项目相提并论。评论者们还讨论了网状网络增强韧性的潜力，少数人则对具体“禁书”的选择和此类策略的有效性提出了疑问。

**标签**: `#hardware hacking`, `#free speech`, `#smart light bulb`, `#banned books`, `#activism`

---

<a id="item-4"></a>
## [Iroh 1.0：应用层点对点网络库发布](https://www.iroh.computer/blog/v1) ⭐️ 8.0/10

开源项目 Iroh 发布了 1.0 版本，提供了一个简化在应用层建立直接点对点连接的库，类似于 Tailscale 在网络层的工作方式。 这一版本大大简化了应用开发者嵌入点对点连接的过程，无需用户管理单独的 VPN 账户。它降低了构建分布式应用的复杂性，可能加速去中心化网络的采用。 Iroh 1.0 原生支持 IPv4、IPv6 和中继传输，现在还允许开发者实现自定义传输层以支持 WebRTC 或 BLE 等协议。它使用称为“拨号密钥”的加密非对称密钥来标识对等体并确保安全连接。

hackernews · chadfowler · 6月15日 15:13 · [社区讨论](https://news.ycombinator.com/item?id=48542480)

**背景**: Iroh 是一个网络库，可在互联网上任意两个对等体之间建立直接连接，自动处理 NAT 穿透和传输选择。它常被与 Tailscale 比较，但 Iroh 在应用层（第 7 层）而非网络层（第 3 层）工作，因此可直接嵌入到应用中，无需单独设置 VPN。这种方式允许应用开发者添加点对点功能，而无需用户创建账户或配置网络设置。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.iroh.computer/">iroh</a></li>
<li><a href="https://www.iroh.computer/blog/comparing-iroh-and-libp2p">Comparing Iroh & Libp2p: Simplifying P2P Connectivity - Iroh</a></li>

</ul>
</details>

**社区讨论**: 社区成员表现出浓厚兴趣，讨论集中在自定义传输支持和与现有解决方案的比较上。开发者澄清说 Iroh 现在支持自定义传输并使用加密密钥进行身份验证。一些人质疑在已有 IP 和 DNS 的情况下 Iroh 的必要性，而另一些人则称赞其用于去中心化应用的潜力。一个值得注意的担忧是有关密钥机制和中继参与的文档不够清晰。

**标签**: `#networking`, `#p2p`, `#peer-to-peer`, `#tailscale`, `#iroh`

---

<a id="item-5"></a>
## [用户分享用本地模型替代 Claude/GPT 进行编码的成功经验](https://news.ycombinator.com/item?id=48542100) ⭐️ 8.0/10

在 Hacker News 的一场讨论中，许多开发者表示已成功用 Qwen 3.6 和 Gemma 4 等本地模型替代 Claude 和 GPT 等云端编码助手，日常编码任务表现足够，同时获得了隐私和成本优势。 这表明开源本地模型已经足够成熟，可以在许多实际编码场景中替代前沿云端模型，有望减少对昂贵订阅的依赖并提升数据隐私。 用户报告使用了如 llama.cpp+Qwen3.6-35B 在单张 RTX 3090 上运行（速度超过 150 tok/s），以及 Mac Studio 128GB RAM 运行 Qwen3.6 35b（3B 活跃参数）。但本地模型被认为不如 Claude Code 或 GPT Codex 等前沿模型聪明。

hackernews · cloudking · 6月15日 14:46

**背景**: 像 Claude 和 GPT 这样的大型语言模型通常通过云端 API 访问。本地模型则下载到用户自己的硬件上运行，提供隐私和离线能力，但需要足够的计算资源。Qwen 是阿里云的开源 LLM 系列，Gemma 来自 Google DeepMind。每秒 token 数（tok/s）衡量模型生成文本的速度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>
<li><a href="https://ai.google.dev/gemma/docs">Gemma models overview | Google AI for Developers</a></li>
<li><a href="https://benchlm.ai/llm-speed">LLM Speed & Latency Comparison — Tokens/sec & Response Latency (2026)</a></li>

</ul>
</details>

**社区讨论**: 讨论总体非常积极，许多用户分享了详细的设置和性能数据。一些用户指出，虽然本地模型尚未达到最佳云端模型的水平，但足以满足大多数日常编码需求，并提供了显著的隐私和成本优势。少数评论者对完全替代云端模型表示怀疑，理由是错过了使用最新模型的机会成本。

**标签**: `#local-llm`, `#coding-assistant`, `#qwen`, `#gemma`, `#hpc`

---

<a id="item-6"></a>
## [Hetzner 因 AI 推动硬件成本上涨大幅提价](https://docs.hetzner.com/general/infrastructure-and-availability/price-adjustment/#cloud-servers) ⭐️ 8.0/10

Hetzner 宣布对其服务器产品大幅提价，部分价格翻了三倍，理由是 AI 需求导致硬件成本上涨。 此次调价反映了更广泛的行业趋势，即 AI 热潮给硬件供应链带来压力，影响云托管经济学，并可能迫使客户重新考虑其提供商。 具体价格变化包括部分服务器型号上涨达 3 倍，此调整适用于 Hetzner 的整个服务器产品线，包括云服务器。

hackernews · tuhtah · 6月15日 13:19 · [社区讨论](https://news.ycombinator.com/item?id=48540844)

**背景**: Hetzner 是一家以极具竞争力的价格著称的德国云托管提供商。近期 AI 的发展增加了对 GPU 和数据中心硬件的需求，导致整个行业出现短缺和成本上升。

**社区讨论**: 社区成员对涨幅之大表示震惊，有人称 3 倍跳涨‘疯狂’。一些人指出，鉴于 Hetzner 此前相对于竞争对手的低价，这是不可避免的，而另一些人则批评 AI 热潮推高成本却没有带来明显好处。

**标签**: `#cloud hosting`, `#pricing`, `#AI boom`, `#hardware scarcity`, `#Hetzner`

---

<a id="item-7"></a>
## [福克斯计划收购 Roku](https://www.wsj.com/business/deals/fox-roku-deal-f6e564f9) ⭐️ 8.0/10

福克斯宣布计划收购流媒体硬件平台 Roku，此举引发了对内容控制和反垄断问题的担忧。 此次收购将使福克斯直接进入 30-50%美国家庭的电视硬件，可能损害平台中立性和市场竞争。 Roku 历来是一个服务无关的平台，但逐渐整合广告和内容，若被福克斯等内容提供商收购，将引发利益冲突担忧。

hackernews · thm · 6月15日 12:50 · [社区讨论](https://news.ycombinator.com/item?id=48540499)

**背景**: Roku 是流行的流媒体设备制造商和平台。福克斯是一家拥有新闻和娱乐内容的大型媒体公司。该交易可能通过结合硬件和内容所有权重塑流媒体格局。

**社区讨论**: 评论者表示强烈悲观，担心失去中立性以及福克斯加强控制，有些人已转向 Nvidia Shield 等替代品。有人担心不应允许福克斯购买如此庞大的用户接入。

**标签**: `#acquisition`, `#Roku`, `#Fox`, `#streaming`, `#antitrust`

---

<a id="item-8"></a>
## [TimescaleDB Hypercore 压缩率达 98%](https://roszigit.com/en/blog/timescaledb-compression-hypercore) ⭐️ 8.0/10

一篇新文章详细介绍了 TimescaleDB 的 hypercore 压缩技术，通过列式存储和高级编码技术，为 PostgreSQL 中的时间序列数据实现了高达 98% 的存储空间节省。 这种压缩能力使 PostgreSQL 在存储海量时间序列数据集时更加高效，有望降低存储成本并改善物联网、监控和分析工作负载的 I/O 性能。 Hypercore 是一种混合行-列存储引擎，通过 segment-by 和 order-by 配置优化压缩。它采用了类似 Facebook Gorilla 的 delta-of-delta 编码和字典编码技术，但在高选择性查询上存在查询性能的权衡。

hackernews · lkanwoqwp · 6月15日 17:29 · [社区讨论](https://news.ycombinator.com/item?id=48544451)

**背景**: TimescaleDB 是专为时间序列数据设计的 PostgreSQL 扩展。传统的行式数据库连续存储每一行，这对于时间序列数据效率低下，因为重复的时间戳和大量行中相似的值压缩效果不佳。列式存储将同一列的值分组，通过连续相似数据实现更高的压缩比。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://roszigit.com/en/blog/timescaledb-compression-hypercore">TimescaleDB Compression: Hypercore and Columnar Storage with up to 98% Ratio in PostgreSQL</a></li>
<li><a href="https://docs.tigerdata.com/use-timescale/latest/hypercore/">Tiger Data Documentation | Hypercore</a></li>
<li><a href="https://www.tigerdata.com/blog/building-columnar-compression-in-a-row-oriented-database">Columnar Compression for Large Databases | Tiger Data</a></li>

</ul>
</details>

**社区讨论**: 社区评论强调了性能权衡：用户指出压缩可能会降低查询速度，尤其是高选择性查询，并将 TimescaleDB 的方法与 deltaX 和摆动门压缩等替代方案进行比较。一位评论者对“高达 98%”的说法表示怀疑，认为如果没有基准测试，这种说法就是“废话”。

**标签**: `#TimescaleDB`, `#PostgreSQL`, `#time-series`, `#compression`, `#database`

---

<a id="item-9"></a>
## [Salesforce 以 36 亿美元收购 Fin（前 Intercom）](https://www.salesforce.com/news/press-releases/2026/06/15/salesforce-signs-definitive-agreement-to-acquire-fin/?bc=HL) ⭐️ 8.0/10

Salesforce 已签署最终协议，以约 36 亿美元收购 Fin（前身为 Intercom）的 AI 客户代理平台。此次收购旨在利用 Fin 的自主代理技术增强 Salesforce 的 Agentforce 平台。 此次收购加剧了 AI 客服代理市场的竞争，特别是针对由 Salesforce 前联合 CEO Bret Taylor 联合创立的 Sierra。这也表明 Salesforce 的战略举措，旨在防止独立的 AI 支持平台成为其 CRM 生态系统之外的控制点。 Fin 在一个月前刚刚从 Intercom 更名，收购价格为 36 亿美元。Salesforce 计划将 Fin 的技术整合到其现有的 Agentforce 平台中，用于构建自定义 AI 代理。

hackernews · colesantiago · 6月15日 12:08 · [社区讨论](https://news.ycombinator.com/item?id=48540126)

**背景**: Salesforce 是客户关系管理（CRM）领域的全球领导者。Fin（前身为 Intercom）是一个 AI 驱动的客户代理平台，可与各种业务系统集成。此次收购反映了大型企业收购 AI 初创公司以增强其 AI 能力的日益增长的趋势，特别是在客户服务自动化方面。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/06/15/salesforce-acquires-ai-customer-service-platform-fin-for-3-6b/">Salesforce acquires AI customer service platform Fin for $3 ...</a></li>
<li><a href="https://www.salesforce.com/news/press-releases/2026/06/15/salesforce-signs-definitive-agreement-to-acquire-fin/">Salesforce Signs Definitive Agreement to Acquire Fin</a></li>

</ul>
</details>

**社区讨论**: 社区评论反应不一：有人称赞正确实施的 AI 客服（例如 Starlink），而其他人则质疑像 Intercom 这样的客服公司的长期可行性，因为企业正在训练自己的 AI 代理。还有猜测认为，此次收购是直接针对由 Salesforce 前联合 CEO Bret Taylor 创立的 Sierra 的竞争举措。

**标签**: `#acquisition`, `#AI`, `#customer-service`, `#Salesforce`, `#CRM`

---

<a id="item-10"></a>
## [AI 未能取代软件工程师，未来也不会](https://simonwillison.net/2026/Jun/14/why-ai-hasnt-replaced-software-engineers/#atom-everything) ⭐️ 8.0/10

Arvind Narayanan 和 Sayash Kapoor 发表文章，认为 AI 尚未也不会导致软件工程师大规模失业，并引用纽约 WARN 法案备案数据：在强制披露的第一年，没有任何公司报告与 AI 相关的裁员。 该分析直接挑战了 AI 将消灭软件工程工作的普遍叙事，以实证数据反驳了基于恐惧的预测。其重要性在于，软件工程被认为是最易受 AI 影响的职业之一，但数据显示并未出现岗位替代。 文章指出软件工程中三个难以自动化的真正瓶颈：决定并明确要构建什么、验证并对交付负责、以及深入理解代码库、业务和环境的深度人类认知。AI 可以辅助前两项，但无法替代第三项。

rss · Simon Willison · 6月14日 23:54

**背景**: WARN 法案要求雇主在发生大规模裁员时提前通知；纽约州于 2025 年 3 月增加了 AI 披露复选框。AI 将取代软件工程师的叙事源于 GPT-4 和 Copilot 等代码生成 AI 模型的快速进步。然而，软件工程远不止编写代码，还包括需求收集、调试和系统设计。

**标签**: `#AI`, `#software engineering`, `#employment`, `#job displacement`, `#technology policy`

---

<a id="item-11"></a>
## [用 Forgejo 和 Opencode 搭建的家庭实验室 AI 开发平台](https://rsgm.dev/post/ai-dev-platform/) ⭐️ 7.0/10

一位开发者详细介绍了他们的家庭实验室 AI 开发平台，使用 Forgejo 托管 Git 仓库，opencode 作为 AI 编码助手，引发了关于类似自托管方案的深入讨论。 这展示了开发者自托管 AI 工具日益流行的趋势，旨在创建定制化、私有的 AI 辅助编码环境，减少对云服务的依赖并加强对工作流的控制。 该方案将自托管 Git 仓库 Forgejo 与开源 AI 编码助手 opencode 结合；有评论者将 opencode 集成到 Forgejo 的 Action Runner 中，实现了从 Issue 触发 AI 生成代码的功能。

hackernews · rsgm · 6月15日 15:09 · [社区讨论](https://news.ycombinator.com/item?id=48542433)

**背景**: Forgejo 是一个用 Go 编写的自托管轻量级 Git 仓库管理平台，提供问题追踪、代码审查和 CI/CD 等功能。Opencode 是一个开源 AI 编码助手，可以在终端中生成和编辑代码，或集成到开发工作流中。两者结合，开发者可以在自己的硬件上构建私有的 AI 驱动开发平台。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Forgejo">Forgejo</a></li>
<li><a href="https://forgejo.org/">Forgejo – Beyond coding. We forge.</a></li>
<li><a href="https://grokipedia.com/page/OpenCode">OpenCode</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了类似的家庭实验室方案并表达热情，有人讨论了在多轮交互中管理 AI 上下文的挑战。一位用户提到其域名被 Quad9 DNS 过滤。

**标签**: `#homelab`, `#AI`, `#development-platform`, `#forgejo`, `#opencode`

---

<a id="item-12"></a>
## [美国电池制造业产量持续创新高](https://fred.stlouisfed.org/series/IPG33591S) ⭐️ 7.0/10

根据 FRED 系列 IPG33591S 的数据，美国电池制造业产量在近期达到历史新高。 这具有重要意义，因为提升国内电池产量对美国供应链和国家安全至关重要，尤其是在电动汽车和储能领域。然而，社区评论显示，美国仍远远落后于中国和欧洲。 FRED 系列追踪的是一次和蓄电池的产出（NAICS 33591），其中包含原电池，这可能会夸大电动汽车电池部分的数据。创纪录的产量标志着从疫情低谷中恢复。

hackernews · epistasis · 6月15日 20:28 · [社区讨论](https://news.ycombinator.com/item?id=48546616)

**背景**: 电池制造是向电动汽车和可再生能源储能过渡的关键产业。美国通过《通胀削减法案》等政策投资国内生产，但面临全球竞争。

**社区讨论**: 评论指出，美国电池产能（2025 年 70 GWh）远不及中国（1755 GWh）和欧洲（252 GWh）。部分评论者指出数据可能包含原电池，并质疑与电动汽车的相关性，而其他人则认为这对国家安全来说是积极的一步。

**标签**: `#battery manufacturing`, `#energy storage`, `#manufacturing`, `#supply chain`, `#EV industry`

---

<a id="item-13"></a>
## [深入分析《指挥官基恩》的自适应瓦片刷新技术](https://forgottenbytes.net/commander_keen.html) ⭐️ 7.0/10

一篇关于《指挥官基恩》游戏引擎的详细技术分析已发布，重点介绍了其创新的自适应瓦片刷新技术，该技术使得在早期 PC 硬件上实现平滑滚动成为可能。 该分析揭示了一项突破性技术，使得早期 PC 游戏能够与主机图形相媲美，展示了 id Software 开发人员的聪明才智。这对于理解游戏引擎优化和复古编程的历史很有价值。 自适应瓦片刷新技术利用 EGA 硬件特性在硬件中执行滚动，并通过跟踪移动的图形元素来最小化重绘。文章还讨论了 PC 与游戏主机硬件限制的历史背景。

hackernews · mfiguiere · 6月15日 17:52 · [社区讨论](https://news.ycombinator.com/item?id=48544781)

**背景**: 在 1990 年代初期，PC 缺乏像 SNES 这样的游戏主机专用的精灵硬件，使得平滑横向滚动变得困难。id Software 的 John Carmack 开发了自适应瓦片刷新技术，利用 EGA 的硬件滚动能力，只重绘改变的瓦片，从而使《指挥官基恩》等游戏能够流畅运行。这项技术是一项重大创新，帮助定义了那个时代的 PC 游戏体验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Adaptive_tile_refresh">Adaptive tile refresh</a></li>
<li><a href="https://fabiensanglard.net/ega/">Commander Keen's Adaptive Tile Refresh - Fabien Sanglard</a></li>
<li><a href="https://retrocomputing.stackexchange.com/questions/22175/what-is-adaptive-tile-refresh-in-the-context-of-commander-keen">What is 'Adaptive Tile Refresh' in the context of Commander Keen?</a></li>

</ul>
</details>

**社区讨论**: 评论者对分析表示赞赏，并推荐书籍《毁灭战士之主》以了解历史背景。一位用户注意到了 PC 与 SNES 硬件的对比，另一位则提到了 Cosmodoc 上的类似分析。总体情绪是积极的，并对技术深入分析表示欣赏。

**标签**: `#game engine`, `#retro gaming`, `#programming`, `#computer history`, `#id Software`

---

<a id="item-14"></a>
## [铜药物恢复阿尔茨海默症小鼠记忆](https://www.monash.edu/news/articles/copper-drug-restores-memory-and-clears-toxic-alzheimers-proteins) ⭐️ 7.0/10

莫纳什大学研究人员证明，铜递送化合物 Cu(ATSM)在阿尔茨海默病小鼠模型中显著减少了有毒的β-淀粉样蛋白，并将空间学习能力提高了 44%，其中 Aβ42 水平下降了 42%。 这项研究为目前有效治疗方法有限的阿尔茨海默病提供了一种潜在的新治疗途径，且该药物此前已针对其他疾病进行过安全性评估，可能加快其进入人体临床试验的进程。 Cu(ATSM) 使血脑屏障处 P-gp 清除泵的丰度增加了 24.1%，恢复了大脑清除β-淀粉样蛋白的能力。该研究发表在《ACS 化学生物学》期刊上。

hackernews · bookofjoe · 6月15日 14:48 · [社区讨论](https://news.ycombinator.com/item?id=48542132)

**背景**: 阿尔茨海默病以大脑中β-淀粉样蛋白斑块的积聚为特征，这些斑块被认为会导致神经退行性变。已知阿尔茨海默病中存在铜稳态失调，铜调节异常可导致氧化应激和线粒体损伤。Cu(ATSM)是一种向细胞特异性递送铜的化合物，可能有助于恢复铜平衡并激活清除机制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medicalxpress.com/news/2026-06-copper-drug-memory-toxic-alzheimer.html">Copper drug restores memory and clears toxic Alzheimer's ...</a></li>
<li><a href="https://scienceblog.com/a-copper-drug-cleared-toxic-proteins-and-restored-memory-in-alzheimers-mice/">A Copper Drug Cleared Toxic Proteins and Restored Memory in ...</a></li>
<li><a href="https://www.drugtargetreview.com/copper-drug-cuatsm-reduces-alzheimers-proteins-by-42-percent-in-preclinical-study/2135715.article">Copper drug Cu (ATSM) reduces Alzheimer's proteins by 42 ...</a></li>

</ul>
</details>

**社区讨论**: 社区评论对淀粉样蛋白假说表示怀疑，有用户引用 Derek Lowe 的观点，认为针对淀粉样蛋白的疗法一再失败。其他人则指出，尽管该药物在小鼠中有效，但仍需人体试验；还有评论者分享了其母亲患有早发性阿尔茨海默病的亲身经历，强调了该疾病的异质性和当前治疗方法的争议。

**标签**: `#Alzheimer's`, `#drug discovery`, `#neuroscience`, `#amyloid-beta`, `#preclinical`

---

<a id="item-15"></a>
## [Cloudflare CAPTCHA 仅在有 & 符号的搜索 URL 上触发](https://simonwillison.net/2026/Jun/16/captcha-on-at-least-one-ampersand/#atom-everything) ⭐️ 7.0/10

Simon Willison 分享了一个 Cloudflare WAF 自定义规则，该规则将托管挑战限制为包含至少一个 & 符号的搜索 URL，从而避免对诸如 /search/?q=term 这样的简单单字搜索触发 CAPTCHA。 这个实用技巧通过减少对合法的单字搜索不必要的 CAPTCHA 提示来改善网站可用性，这是一个常见的令访客烦恼的问题，并可能影响用户体验。 该规则表达式使用 Cloudflare 规则语言：(http.request.uri.path wildcard r"/search/*" and http.request.uri.query contains "&")。Simon 最初尝试了 Cloudflare 的 MCP 与 Claude Code，但转而使用 Cloudflare API，因为 MCP 无法编辑所需的规则。

rss · Simon Willison · 6月16日 00:21

**背景**: Cloudflare 的托管挑战是传统 CAPTCHA 的替代方案，它使用多种挑战来验证人类访客。它可以通过 Cloudflare 的 Web 应用程序防火墙（WAF）自定义规则进行配置，这些规则使用特定的表达式语法来匹配流量。Simon Willison 在他的网站上运行了一个分面搜索引掣，激进爬虫频繁访问该引擎，促使他添加了一条 CAPTCHA 规则，后来他优化为仅在有多个参数（由 & 符号表示）的复杂查询上触发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developers.cloudflare.com/cloudflare-challenges/">Challenges · Cloudflare challenges docs</a></li>
<li><a href="https://blog.cloudflare.com/end-cloudflare-captcha/">The end of the road for Cloudflare CAPTCHAs</a></li>
<li><a href="https://developers.cloudflare.com/waf/custom-rules/">Custom rules · Cloudflare Web Application Firewall (WAF) docs</a></li>

</ul>
</details>

**标签**: `#Cloudflare`, `#CAPTCHA`, `#WAF`, `#Configuration`, `#Simon Willison`

---

<a id="item-16"></a>
## [性格冲突致美国政府关闭 Anthropic 模型](https://simonwillison.net/2026/Jun/15/axios-clashes-anthropics/#atom-everything) ⭐️ 7.0/10

Axios 的一篇报道披露，Anthropic 与美国政府官员之间的性格冲突，加上出口管制执法，导致 Anthropic 的 Claude Fable 和 Claude Mythos 模型的访问被暂停。 这一事件凸显了前沿 AI 实验室与政府监管机构在出口管制和安全标准方面日益紧张的关系，可能为未来政府干预 AI 模型部署开创先例。 美国政府将 Claude Mythos 的一次越狱归类为'潜在的狭隘、非通用越狱'，Anthropic 的 Constitutional Classifiers 迄今阻止了通用越狱。由 Logan Graham 领导的 Anthropic 前沿红队正与商务部会面讨论此事。

rss · Simon Willison · 6月15日 14:57

**背景**: Anthropic 开发了两款先进模型：Claude Fable 5（带有安全措施的公开版本）和 Claude Mythos 5（更强大但安全措施更严格，仅限特定用户）。美国政府根据出口管制法律发布指令暂停这些模型的访问，理由是越狱可能带来国家安全风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://red.anthropic.com/">red.anthropic.com</a></li>

</ul>
</details>

**社区讨论**: Simon Willison 在评论 Axios 文章时表示对解决僵局持怀疑态度，指出完美的越狱抵抗可能是不可能的。他还质疑 Anthropic 是否解决了 2023 年的通用对抗性攻击问题。

**标签**: `#Anthropic`, `#AI safety`, `#export controls`, `#AI policy`, `#US government`

---

<a id="item-17"></a>
## [开源权重不够，开放训练框架至关重要](https://www.reddit.com/r/MachineLearning/comments/1u6p7k3/open_weights_are_not_enough_we_need_open_training/) ⭐️ 7.0/10

一位 Reddit 用户认为仅开源权重不够，并介绍了 FeynRL，这是一个用于 LLM、VLM 和智能体 RL 后训练的开源框架，强调训练过程的可见性和可修改性。 这很重要，因为当前 LLM 的 RL 后训练存在隐藏的系统细节，阻碍了算法研究；开源训练框架可以民主化并加速这一关键领域的进展。 FeynRL 设计为显式化和模块化，支持 SFT、DPO 和 RL 后训练，兼容 vllm 和 llm，可在单 GPU 到集群配置上运行。

reddit · r/MachineLearning · /u/summerday10 · 6月15日 18:37

**背景**: RL 后训练是一种使用强化学习在监督微调后对大型语言模型进行微调的技术，旨在改善对齐、推理或任务性能。开源权重意味着模型参数公开可用，但若没有训练代码和基础设施，研究人员无法轻松复现或修改训练过程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/FeynRL-project/FeynRL">GitHub - FeynRL -project/ FeynRL : RL-first post-training framework for...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Richard_Feynman">Richard Feynman</a></li>

</ul>
</details>

**标签**: `#open-source AI`, `#reinforcement learning`, `#LLM training`, `#research frameworks`, `#machine learning`

---

<a id="item-18"></a>
## [Cleo：2B 参数模型实现文本到 SQL 的统一框架](https://www.reddit.com/r/MachineLearning/comments/1u6udpb/cleo_trying_to_fit_full_analyst_behavior_in_a_2b/) ⭐️ 7.0/10

Cleo 是一个基于 Qwen3.5-2B-Base 微调的文本转 SQL 模型，在统一的框架内进行训练和评估，支持实时执行搜索和系统组件的协同设计。 这表明当训练和推理条件一致时，小型 2B 模型也能有效处理文本转 SQL 任务，从而降低成本，使受限资源环境也能更易使用此类系统。 统一的框架支持在推理时使用相同的“收集-修复-回答”协议进行训练，并允许利用实时执行证据（而非仅模型似然）搜索候选查询。模型、框架和数据集完全开源。

reddit · r/MachineLearning · /u/Dreeseaw · 6月15日 21:43

**背景**: 文本转 SQL 系统将自然语言查询转换为 SQL 数据库查询。大型语言模型（LLM）常用于此任务，但大模型（如 7B 以上参数）资源消耗大。微调 Qwen3.5-2B-Base 这样的小型模型可以在更高效的同时达到有竞争力的性能。统一的框架确保训练、评估和推理共享相同结构，从而提高一致性和性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.5-2B-Base">Qwen/ Qwen 3 . 5 - 2 B - Base · Hugging Face</a></li>

</ul>
</details>

**标签**: `#text-to-SQL`, `#small language models`, `#fine-tuning`, `#open-source`, `#AI engineering`

---

<a id="item-19"></a>
## [PrintGuard 2.0：少样本故障检测器迁移至 TFLite，可浏览器运行](https://www.reddit.com/r/MachineLearning/comments/1u6e9zc/printguard_20_shufflenetv2_fewshot_prototypical/) ⭐️ 7.0/10

PrintGuard 2.0 发布，对代码进行全面重写，将其 ShuffleNetV2 + 原型网络模型通过 LiteRT 导出为约 5 MB 的 TFLite 模型，从而无需修改即可在 CPython 和浏览器（通过 Pyodide）中运行。 这展示了少样本学习在边缘设备上的实用部署，利用轻量级运行时，使任何 FDM 打印机无需依赖云即可获得先进的故障检测能力。 模型依然是 ShuffleNetV2 编码器加最近原型分类，但现在使用 LiteRT 推理，并包含可直接映射到原型距离的每台打印机灵敏度/阈值滑动条。

reddit · r/MachineLearning · /u/oliverbravery · 6月15日 11:47

**背景**: ShuffleNetV2 是一种为移动设备设计的高效 CNN 架构，兼顾速度和准确性。原型网络学习一个度量空间，通过计算到类别原型的距离进行分类，从而实现少样本学习。LiteRT（原 TensorFlow Lite）是谷歌的端侧 ML 运行时。Pyodide 通过 WebAssembly 实现在浏览器中运行 Python。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/1807.11164">[1807.11164] ShuffleNet V2: Practical Guidelines for Efficient CNN Architecture Design</a></li>
<li><a href="https://arxiv.org/abs/1703.05175">[1703.05175] Prototypical Networks for Few-shot Learning</a></li>
<li><a href="https://developers.googleblog.com/en/tensorflow-lite-is-now-litert/">TensorFlow Lite is now LiteRT - Google Developers Blog</a></li>
<li><a href="https://github.com/google-ai-edge/litert">GitHub - google-ai-edge/LiteRT: LiteRT, successor to ...</a></li>

</ul>
</details>

**标签**: `#few-shot learning`, `#edge AI`, `#TFLite`, `#3D printing`, `#fault detection`

---

<a id="item-20"></a>
## [开发者对计算机的怀旧颂歌](https://michaelenger.com/blog/i-love-the-computer/) ⭐️ 6.0/10

一位开发者发表了题为《我爱计算机》的个人随笔，反思纯粹摆弄计算机的乐趣，并与现代科技行业的挫败感形成对比。 这篇文章引起了许多有类似怀旧情感开发者的强烈共鸣，凸显了计算内在乐趣与商业化科技行业之间的文化张力，并引发了关于人工智能、复古计算和守门行为的讨论。 这是一篇深思熟虑的个人反思，社区参与度很高（136 分，87 条评论），但在技术上并非开创性；作者表达了对计算的热爱，而这种热爱在当今行业中似乎已丢失。

hackernews · speckx · 6月15日 20:14 · [社区讨论](https://news.ycombinator.com/item?id=48546441)

**背景**: 这篇随笔借用了早期计算时代的怀旧，当时摆弄机器是核心活动，并与人工智能和企业软件等现代复杂性形成对比。许多开发者感到与自己曾拥有的纯粹乐趣脱节。

**社区讨论**: 评论观点不一：有些完全赞同（“破坏东西、戳它、修复它……”），而另一些则批评作者有守门心态（“这种情绪太有门卫感了”）。一些人称赞人工智能是有用的工具，一位评论者提到纯粹为了乐趣而编写 6502 汇编代码。

**标签**: `#computing culture`, `#tinkering`, `#nostalgia`, `#hacker community`

---

<a id="item-21"></a>
## [LLMs 在生成网站中表现出一致的名称偏好](https://www.reddit.com/r/MachineLearning/comments/1u6mn3q/ai_language_models_have_favorite_names_and_we/) ⭐️ 6.0/10

研究人员发现，大型语言模型具有模型特定和版本特定的名称偏好，例如“Elena Vasquez”和“Marcus Chen”经常一起出现在 Claude 生成的内容中。这些名称组合出现在数十个网站上，相同的三人组与 AI 生成的面孔共同出现。 这一发现揭示了 LLM 输出中一种微妙但普遍的偏差，可作为识别 AI 生成内容的指纹。它还强调了模型的内部先验如何导致相关的幻觉，这些幻觉可能在网络上传播。 论文（arxiv 2606.02184）表明，LLM 生成的字符组合（成对和三人组）的共现率远高于偶然水平。研究人员在开发一种名为 CDD（Concurrent Diffing of Distributions）的模型差异分析方法时偶然发现了这一点。

reddit · r/MachineLearning · /u/CebulkaZapiekana · 6月15日 17:07

**背景**: 大型语言模型（如 GPT-4 和 Claude）基于从海量数据集中学到的模式生成文本。它们有时会默认选择高概率的名称或概念，导致一致的偏差。'相关组合'的概念指的是在许多独立生成中可靠地一起出现的名称组，表明模型参数中存在潜在的先验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2606.02184">[2606.02184] The Ghost Couple: Correlated LLM Name Priors and Their ...</a></li>

</ul>
</details>

**标签**: `#LLMs`, `#AI bias`, `#model behavior`, `#generated content`

---

<a id="item-22"></a>
## [量化公司争相成为 ICML 2026 钻石赞助商](https://www.reddit.com/r/MachineLearning/comments/1u64rse/quant_firms_at_icml_2026_d/) ⭐️ 6.0/10

一则 Reddit 帖子指出，多家量化金融公司已签约成为 2026 年国际机器学习大会（ICML）的钻石赞助商。 这一趋势表明机器学习与量化交易及金融领域的深度融合，这些公司正在大力投资前沿 ML 研究和人才。 ICML 是顶级机器学习会议之一；钻石赞助是最高级别，提供卓越的曝光度和接触顶尖研究人员的渠道。

reddit · r/MachineLearning · /u/Intrepid_Discount_67 · 6月15日 03:09

**背景**: 量化金融公司使用高级数学模型和算法进行交易。它们越来越依赖机器学习进行预测建模、风险管理和自动化策略。ICML 吸引了顶尖的 ML 研究人员，因此成为招聘和合作的绝佳场所。

**标签**: `#machine learning`, `#quantitative finance`, `#conferences`, `#industry sponsorship`

---

<a id="item-23"></a>
## [嵌入式传感器机器学习中的最大时间消耗](https://www.reddit.com/r/MachineLearning/comments/1u6q97f/embeddededge_ml_folks_what_actually_eats_the_most/) ⭐️ 6.0/10

一个 Reddit 讨论向嵌入式 ML 从业者提问：基于传感器的项目中，最耗时的是数据收集、清洗/标注还是部署。 了解嵌入式 ML 工作流程中的真正瓶颈可以指导工具开发，并帮助初创公司专注于最有影响力的功能。 作者正在构建一个与硬件无关、原生支持生成式 AI 的平台，类似于 Edge Impulse，但针对时间序列数据，并希望获得关于自动数据质量检查和 AI 辅助标注等潜在功能的反馈。

reddit · r/MachineLearning · /u/No-Bug-4879 · 6月15日 19:13

**背景**: Edge Impulse 是一个领先的边缘设备（包括微控制器）机器学习开发部署平台。时间序列传感器数据（如加速度计数据）在嵌入式 ML 中很常见，但手动收集、清洗和标注这些数据通常是一个主要瓶颈。原生生成式 AI 方法意味着该平台从头开始构建，以利用生成式 AI 模型，可能自动化许多这些任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.edgeimpulse.com/">Edge Impulse - The Leading Edge AI Platform</a></li>
<li><a href="https://www.st.com/content/st_com/en/partner/partner-program/partnerpage/Edge_Impulse.html">Edge Impulse - STMicroelectronics - STMicroelectronics</a></li>
<li><a href="https://en.wikipedia.org/wiki/Generative_AI">Generative AI - Wikipedia</a></li>

</ul>
</details>

**标签**: `#embedded ML`, `#edge computing`, `#time series`, `#data labeling`, `#model deployment`

---