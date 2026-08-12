---
layout: default
title: "Horizon Summary: 2026-08-12 (ZH)"
date: 2026-08-12
lang: zh
---

> 从 38 条内容中筛选出 22 条重要资讯。

---

1. [Qwen 发布 2.4 万亿参数 MoE 模型 Qwen3.8-2.4T-A95B](#item-1) ⭐️ 9.0/10
2. [Meta 发布 Muse Glimmer：Apache 2.0 许可的 300 亿参数智能体模型](#item-2) ⭐️ 9.0/10
3. [DeepSeek V4 Pro 0813 发布，编码性价比表现突出](#item-3) ⭐️ 8.0/10
4. [Tailscale 将数据库损坏追溯至 16 年历史的 SQLite WAL 重置 Bug](#item-4) ⭐️ 8.0/10
5. [通过 WebSocket 传输 HTML：用极少的 JavaScript 构建实时 SPA](#item-5) ⭐️ 8.0/10
6. [xAI 发布前沿模型 Grok 4.6](#item-6) ⭐️ 8.0/10
7. [Chrome 的缩放算法导致微小 JPEG 图像显示不同](#item-7) ⭐️ 8.0/10
8. [uBlock Origin 停止过滤 Facebook 广告：混淆战术迫使让步](#item-8) ⭐️ 8.0/10
9. [攻击可恢复顶级 LLM API 隐藏的推理过程](#item-9) ⭐️ 8.0/10
10. [Adam 的基依赖破坏了 GD 的隐式低秩偏差](#item-10) ⭐️ 8.0/10
11. [解耦下降：通过 AMP Onsager 修正实现训练-测试误差精确对齐](#item-11) ⭐️ 8.0/10
12. [Zed 发布 DeltaDB，这是一款面向 AI 协作的类聊天版本控制工具。](#item-12) ⭐️ 7.0/10
13. [引用弗洛里安·赫伦格特](#item-13) ⭐️ 7.0/10
14. [自然语言文本不存在无损转换](#item-14) ⭐️ 7.0/10
15. [新网站按会议目的地质量而非声望给 CS 会议排名](#item-15) ⭐️ 7.0/10
16. [临时搭建的摄像头网站吸引社区关注 2026 年日食](#item-16) ⭐️ 6.0/10
17. [AmigaDOS 开发者 Tim King 去世](#item-17) ⭐️ 6.0/10
18. [大规模扫描伪装成 ClaudeBot 等 AI 机器人](#item-18) ⭐️ 6.0/10
19. [YC P26 初创公司推出 AI 智能体用于半导体材料发现](#item-19) ⭐️ 6.0/10
20. [Datasette-upload-dbs 0.5a0 为数据库上传新增正式 API](#item-20) ⭐️ 6.0/10
21. [AAAI 2027 审稿人指出投稿普遍缺少代码](#item-21) ⭐️ 6.0/10
22. [请教带后状态随机合并谜题的 RL/规划方法](#item-22) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Qwen 发布 2.4 万亿参数 MoE 模型 Qwen3.8-2.4T-A95B](https://huggingface.co/Qwen/Qwen3.8-2.4T-A95B) ⭐️ 9.0/10

通义千问发布了 Qwen3.8-2.4T-A95B，这是一个混合专家（MoE）模型，总参数达 2.4 万亿，激活参数为 950 亿，同时提供了 BF16 和 FP8 检查点。该模型达到了接近前沿的性能，量化版本据称可在高端消费级硬件上运行。 这是迄今发布的最大开源权重 MoE 模型之一，标志着前沿规模的模型正变得可供本地部署和研究使用。借助实用的量化方案，它可能改变个人和小型实验室对自家设备可运行模型的预期。 BF16 版本需要约 4.9TB 存储空间，而 unsloth 的 1-bit 量化可将其降至约 397GB。开源权重版本缺少官方 Qwen3.8-Max 中的视觉输入、非思考模式支持和 1M 上下文长度等功能。

hackernews · Philpax · 8月12日 15:01 · [社区讨论](https://news.ycombinator.com/item?id=49273478)

**背景**: 混合专家（MoE）是一种将计算划分到多个专门子网络（即“专家”）的架构，每个 token 仅激活一部分专家以节省算力。总参数决定存储占用，而激活参数决定推理速度和成本。FP8、INT4 等量化技术通过以较低精度存储权重来降低内存需求，通常只会带来很小的精度损失。这些方法使大规模模型能够在更易获取的硬件上运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/applying-mixture-of-experts-in-llm-architectures/">Applying Mixture of Experts in LLM Architectures | NVIDIA Technical Blog</a></li>
<li><a href="https://rcrtech.com/semiconductor-news/llms-quantization-fp8-fp4-int8/">LLMs and quantization: FP8, FP4, and INT8 explained</a></li>
<li><a href="https://spanvero.com/learn/active-vs-total-params/">Active vs total parameters — what it means (open AI models)...</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，仅提供 BF16/FP8 版本使得该模型比 Kimi k3 等竞品更难部署，而未经 QAT 的 4-bit 量化需要外部校准数据。一些人惊讶于 1-bit 量化版本可在约 397GB 规模上带来接近 Opus 4.5 的性能，另一些人则指出其缺少视觉和长上下文功能。还有评论提到 DeepSeek V4-Pro 的基准测试公告，将此次发布置于竞争背景中。

**标签**: `#AI`, `#LLM`, `#Qwen`, `#MoE`, `#Open Weights`

---

<a id="item-2"></a>
## [Meta 发布 Muse Glimmer：Apache 2.0 许可的 300 亿参数智能体模型](https://simonwillison.net/2026/Aug/10/introducing-muse-glimmer/) ⭐️ 9.0/10

Meta 推出了 Muse Glimmer，这是一个 300 亿参数的开放权重模型，采用宽松的 Apache 2.0 许可发布。该模型专门针对端到端智能体任务、可靠工具使用和多步推理进行了优化，同时还具备视觉能力。 Muse Glimmer 的亮点在于采用了干净的 Apache 2.0 许可，与 Meta 之前定制的 Llama 许可相比更进一步，允许商业和研究用途的自由使用。它在可本地运行的 300 亿参数规模下展现出强大的智能体和工具调用能力，对构建自主 AI 代理的开发者具有很高价值。 Muse Glimmer 是一个支持视觉的多模态模型；Simon Willison 通过 LM Studio 测试了 18.16GB 的量化版本，发现它在图像描述和使用 llm-coding-agent 插件进行代码探索方面表现良好。Meta 声称它在 DeepSearch QA、MCP-Atlas、τ-Bench 和 SWE-Bench 等难度较高的智能体基准测试中取得了优异成绩。

rss · Simon Willison · 8月10日 23:56

**背景**: 智能体（Agentic AI）指的是能够自主规划并执行多步骤任务、通常还会调用外部工具的人工智能系统。开放权重模型允许用户自由下载和微调模型，与封闭 API 不同。诸如 SWE-Bench 等基准测试评估模型解决真实 GitHub 问题的能力，MCP-Atlas 通过真实 MCP 服务器评估工具使用能力，τ-Bench 则模拟动态的用户与智能体对话。Muse Glimmer 正是为在这样真实的智能体部署场景中表现出色而设计的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/scaleapi/mcp-atlas">GitHub - scaleapi/mcp-atlas: MCP Atlas</a></li>
<li><a href="https://github.com/sierra-research/tau-bench">GitHub - sierra-research/tau-bench: Code and Data for Tau-Bench · GitHub</a></li>
<li><a href="https://github.com/swe-bench/SWE-bench">GitHub - SWE-bench/SWE-bench: SWE-bench: Can Language Models ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#Machine Learning`, `#Open Weights`, `#Agentic AI`, `#Meta`

---

<a id="item-3"></a>
## [DeepSeek V4 Pro 0813 发布，编码性价比表现突出](https://openrouter.ai/deepseek/deepseek-v4-pro-0813) ⭐️ 8.0/10

DeepSeek 于 2026 年 8 月 12 日在 OpenRouter 和自家 API 上发布了旗舰模型 DeepSeek V4 Pro 0813 的正式可用（GA）版本。早期用户测试显示，它在编码任务上的成本仅为竞争对手模型的几分之一。 V4 Pro 0813 在编码任务上的高性价比可能会给 Grok、GPT 等更昂贵的竞品带来压力。作为 DeepSeek 的开放权重模型，它延续了以低成本、高效率撼动行业的潮流。 V4 Pro 0813 结束了为期近四个月的预览期，是 V4 Pro 旗舰模型的正式发布版本。在一个 Codex CLI 社区测试中，DeepSeek 用 12 分钟、花费 0.12 美元完成了新功能开发，但存在 bug；而 Grok 4.6 用时约 3 分钟、花费 1.41 美元，且没有 bug。

hackernews · explosion-s · 8月12日 16:04 · [社区讨论](https://news.ycombinator.com/item?id=49274600)

**背景**: DeepSeek 是一家中国人工智能公司，其 2025 年 1 月发布的 R1 模型成为全球现象，并引发了对大语言模型效率的广泛讨论。V4 系列包括更轻量、成本更低的 V4 Flash，以及提供更高推理投入模式 'Pro-Max' 的 V4 Pro 旗舰模型。社区测试结果提示，DeepSeek 的成本优势有时会以正确性或可靠性方面的权衡为代价。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.unite.ai/deepseek-ships-v4-pro-as-its-flagship-model-leaves-preview/">DeepSeek Ships V4 Pro as Its Flagship Model Leaves Preview</a></li>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>
<li><a href="https://api-docs.deepseek.com/news/news260424/">DeepSeek V 4 Preview Release | DeepSeek API Docs</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：有人质疑为什么帖子链接到 OpenRouter 而不是官方 API；同时，动手编码测试显示 DeepSeek 虽然便宜得多，但比 Grok 4.6 和 GPT-5.6-terra-high 更容易出问题。也有人对最近的 V4 Flash 更新赞赏有加，称它能以极低的成本处理繁重的开发任务，令人惊喜。

**标签**: `#deepseek`, `#llm`, `#model-release`, `#coding`, `#ai`

---

<a id="item-4"></a>
## [Tailscale 将数据库损坏追溯至 16 年历史的 SQLite WAL 重置 Bug](https://tailscale.com/blog/sqlite-wal-reset-bug) ⭐️ 8.0/10

Tailscale 公开披露，SQLite 预写日志（WAL）重置/检查点代码中一个存在 16 年的数据竞争导致了数月的数据库损坏与控制面宕机。Tailscale 资助开发了一个开源 SQLite VFS 垫片来帮助定位该竞争条件，问题最终在 SQLite 3.51.3 中修复。 该 Bug 影响了许多生产环境所依赖的单写者 SQLite 配置，动摇了人们对 SQLite 可靠性的既有假设。它还展示了一种可持续的开源资助模式：企业为针对性调试工具付费并与上游维护者协作。 尽管 SQLite 推荐采用单写者 WAL 用法，但损坏仍由 WAL 重置与检查点操作之间的竞争引发。最初的修复曾因破坏其他功能而被回滚，经过两个多月的观察，SQLite 3.51.3 才被确认为真正的修复版本。

hackernews · ropbear · 8月12日 14:22 · [社区讨论](https://news.ycombinator.com/item?id=49272832)

**背景**: SQLite 使用预写日志（WAL）作为回滚日志模式的替代方案：变更先追加到临时 WAL 文件，之后由检查点操作合并回主数据库。成功的检查点会重置 WAL，而这一重置逻辑中的数据竞争可能导致数据库损坏。SQLite 是被广泛嵌入使用的 C 语言库，拥有庞大的测试套件，但此 Bug 仍存在了 16 年。Tailscale 通过商业支持合同与 SQLite 团队协作定位了该问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tailscale.com/blog/sqlite-wal-reset-bug">How Tailscale helped find the SQLite WAL-Reset bug</a></li>
<li><a href="https://antithesis.com/blog/2026/wal-reset-bug/">Breaking the WAL | Antithesis</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍称赞这篇技术复盘与透明的调试过程。有人强调资助开源调试工具与 SQLite 支持合同的价值，也有人引用 Dijkstra 的观点指出，即使拥有庞大的测试套件也无法证明不存在 Bug。

**标签**: `#sqlite`, `#reliability`, `#debugging`, `#open-source`, `#tailscale`

---

<a id="item-5"></a>
## [通过 WebSocket 传输 HTML：用极少的 JavaScript 构建实时 SPA](https://en.andros.dev/blog/ef4968f5/html-over-websockets-real-time-spas-with-barely-any-javascript/) ⭐️ 8.0/10

一篇文章提出通过 WebSocket 将服务器端渲染的 HTML 流式传输到浏览器，从而大幅减少客户端 JavaScript，用于构建实时单页应用（SPA）。文章称 Phoenix LiveView 是该技术的开创者，并引发了关于 WebSockets 与 Server-Sent Events（SSE）各自适用场景的激烈讨论。 这种方式挑战了以客户端 JavaScript 框架为主导的 SPA 开发模式，可能简化开发、部署和安全管理。相关讨论还厘清了 WebSockets 与 SSE 在实际应用中的取舍，影响开发者如何为实时应用选择通信技术。 文章声称，由于服务器在发送前已渲染并转义 HTML，这种架构能更好地防御 XSS——但评论者对此强烈质疑。另一个重要细节是，Phoenix LiveView 在首次渲染后实际上通过 WebSocket 传输的是最小化的 diff 更新，而非完整 HTML 片段；如果需要的是纯服务器到客户端的推送，SSE 更简单、成本更低。

hackernews · redbell · 8月12日 16:51 · [社区讨论](https://news.ycombinator.com/item?id=49275335)

**背景**: Phoenix LiveView 是构建在 Elixir 和 Phoenix 技术栈之上的服务器端实时 Web 框架；它在服务器上渲染 HTML，并通过持久的 WebSocket 连接更新客户端。Server-Sent Events（SSE）是一种基于普通 HTTP 的标准服务器推送技术，而 WebSocket 则提供全双工的双向通信。核心架构问题在于：实时应用究竟需要双向低延迟消息，还是只需要服务器主动更新页面内容。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/phoenixframework/phoenix_live_view">GitHub - phoenixframework/phoenix_live_view: Rich, real-time ... Phoenix Framework LiveView — Phoenix v1.8.9 Phoenix LiveView 1.0.0 is here! - Phoenix Blog Welcome — Phoenix LiveView v1.2.9 - HexDocs Phoenix LiveView Tutorial: Getting Started - daily.dev</a></li>
<li><a href="https://en.wikipedia.org/wiki/Server-sent_events">Server-sent events - Wikipedia</a></li>
<li><a href="https://phoenix-live-view.hexdocs.pm/Phoenix.LiveView.html">Phoenix.LiveView — Phoenix LiveView v1.2.9 - HexDocs</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，Chris McCord 最初在 Rails 中通过 Sync gem 尝试了这一想法，之后才转向 Phoenix 并开发了 LiveView。还有评论者认为，对大多数服务器推送场景而言 SSE 更简单、成本更低，WebSockets 应留给聊天、协作等双向通信需求；另有一位评论者强烈反对文章关于 XSS 安全性的说法，认为现实中往往恰恰相反。

**标签**: `#WebSockets`, `#Real-time`, `#SPA`, `#SSE`, `#JavaScript`

---

<a id="item-6"></a>
## [xAI 发布前沿模型 Grok 4.6](https://x.ai/news/grok-4-6) ⭐️ 8.0/10

xAI 宣布了其最新的前沿大语言模型 Grok 4.6，在 Hacker News 上引发了大量讨论。此次发布正值 AI 实验室之间的激烈竞争之际。 Grok 4.6 的发布加剧了前沿 AI 提供商之间的竞争，可能影响模型定价和能力基准。Hacker News 上的讨论还引发了关于 API 行为和模型基准有效性的重要问题。 社区报告指出，xAI API 会添加一个默认系统提示，可能覆盖用户提供的指令，导致模型拒绝讨论其自身指南。一些评论者还推测存在基准操纵，并将 Grok 的订阅配额与 OpenAI 和 Anthropic 进行比较。

hackernews · iLuddite · 8月12日 15:32 · [社区讨论](https://news.ycombinator.com/item?id=49274027)

**背景**: Grok 是由埃隆·马斯克的 AI 公司 xAI 开发的一系列大语言模型，可通过 grok.com 和 xAI API 使用。该 API 允许开发者使用具有推理、视觉和工具调用能力的前沿模型。此次发布基于早期 Grok 版本，直接与 OpenAI、Anthropic 及其他实验室的模型竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Grok_(chatbot)">Grok (chatbot) - Wikipedia</a></li>
<li><a href="https://x.ai/api">API: Frontier Models for Reasoning & Enterprise | SpaceXAI</a></li>
<li><a href="https://grok.com/">Grok</a></li>

</ul>
</details>

**社区讨论**: Hacker News 社区意见分歧：有人称赞 Grok 是良性竞争，也有人拒绝支持埃隆·马斯克的企业。主要担忧包括 API 提示注入、疑似基准作弊，以及订阅配额是否足够慷慨。

**标签**: `#AI`, `#Grok`, `#xAI`, `#LLM`, `#model release`

---

<a id="item-7"></a>
## [Chrome 的缩放算法导致微小 JPEG 图像显示不同](https://guillaumetech.github.io/posts/jpg-scaling-chrome/) ⭐️ 8.0/10

文章解释了 Chrome 渲染微小 JPEG 图像时表现不同的原因：其缩放算法采用为速度优化的低分辨率线性插值，产生轻微右偏和比其它浏览器更模糊的边缘。文章结论是图标不应使用 JPEG 格式，而应改用 PNG 或 SVG。 这对 Web 开发者和浏览器工程师很重要，因为它揭露了一个不明显的跨浏览器渲染差异，可能降低界面质量，同时强化了关于图片格式和分辨率的最佳实践。了解浏览器特有的缩放算法有助于开发者在生产环境中做出明智决策，避免微妙的视觉缺陷。 Chrome 的缩小行为在图像几乎未缩小的情况下表现最为明显，即使在极轻微缩小时也会使用线性插值。由于 Electron 应用继承了 Chrome 的渲染引擎，该问题同样影响了 Electron 应用；社区成员还指出，从超大分辨率缩小 PNG 时也可能出现类似的伪影。

hackernews · gutechh · 8月12日 14:00 · [社区讨论](https://news.ycombinator.com/item?id=49272549)

**背景**: JPEG 是一种有损图像格式，使用离散余弦变换（DCT）压缩，通过丢弃数据来减小文件大小，但在高压缩比下会产生块效应、振铃等压缩伪影。浏览器在调整图像大小时使用不同的缩放算法：Chrome 采用为速度优化的低分辨率线性插值，而 Firefox 使用更锐利但略有振铃的算法。CSS 属性“image-rendering”可以影响所使用的算法，使开发者在模糊和锐利之间进行一定程度的权衡。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://entropymine.com/resamplescope/notes/browsers/">How web browsers resize images</a></li>
<li><a href="https://stackoverflow.com/questions/37906602/blurry-downscaled-images-in-chrome">html - Blurry downscaled images in Chrome - Stack Overflow</a></li>
<li><a href="https://gehrcke.de/2014/11/css-crispy-downscaled-images/">CSS: Crispy downscaled images – Jan-Philip Gehrcke, PhD</a></li>
<li><a href="https://en.wikipedia.org/wiki/JPEG_artifacts">JPEG artifacts</a></li>

</ul>
</details>

**社区讨论**: 社区评论普遍认同文章关于图标不使用 JPEG 的警告：jonathanlydall 指出该问题也影响 PNG，并曾导致 Electron 应用中大量图标被破坏而推迟升级；advisedwang 强调应使用尺寸合适的图片，避免用超大图片显示小图标；debazel 和 gwittel 讨论了 Chrome 与 Firefox 缩放算法的差异，并建议使用“image-rendering”CSS 属性作为变通方案；muizelaar 还提到 Firefox 正在处理低倍率解码的 bug。

**标签**: `#JPEG`, `#Chrome`, `#image scaling`, `#web development`, `#browser rendering`

---

<a id="item-8"></a>
## [uBlock Origin 停止过滤 Facebook 广告：混淆战术迫使让步](https://digitalescapetools.com/2026/08/ublock-origin-stops-chasing-facebook-ads.html) ⭐️ 8.0/10

广受欢迎的开源广告拦截器 uBlock Origin 宣布不再尝试过滤 Facebook 上的广告，承认 Facebook 的混淆战术使这场"猫鼠游戏"无法获胜。这一消息最初出现在 Reddit 帖子中，并由 Neowin 报道。 这标志着广告拦截军备竞赛中的一次重大让步，表明大型平台的防拦截措施能够有效击败广泛使用的拦截工具。这影响到数百万使用 Facebook 的 uBlock Origin 用户，并引发了关于广告拦截有效性、隐私和平台控制权的广泛讨论。 据报道，Facebook 使用混淆且频繁变化的代码将广告隐藏于过滤列表之外，使 uBlock Origin 难以跟上。该决定不影响对其他网站的广告拦截；该扩展仍是广受欢迎的内容过滤器，在 Chrome 和 Firefox 上拥有数千万用户。

hackernews · Markoff · 8月12日 11:28 · [社区讨论](https://news.ycombinator.com/item?id=49270726)

**背景**: uBlock Origin 是一款免费开源的浏览器扩展，用于内容过滤和广告拦截，由 Raymond Hill 开发，支持 Firefox 和基于 Chromium 的浏览器。Facebook 的商业模式严重依赖广告，因此它投入大量资源实施反广告拦截措施，通过混淆手段伪装广告投放。广告拦截器与 Facebook 等平台之间的持续冲突已成了一场技术军备竞赛，双方都在努力智胜对方。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/UBlock_Origin">UBlock Origin</a></li>
<li><a href="https://www.humansecurity.com/learn/blog/unmasking-malvertising-how-obfuscation-creates-false-safety-and-how-to-defeat-it/">Unmasking malvertising: How obfuscation creates... - HUMAN Security</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：一些用户认为放弃拦截 Facebook 广告是正确的决定，而另一些人则预测下一阶段将出现利用 AI 或计算机视觉来识别广告的解决方案。还有评论者反思这场猫鼠游戏的徒劳，也有人质疑 Facebook 为何投入精力绕过拦截器，因为使用拦截器的用户大概率不会与广告互动。

**标签**: `#ad-blocking`, `#privacy`, `#facebook`, `#ublock-origin`, `#arms-race`

---

<a id="item-9"></a>
## [攻击可恢复顶级 LLM API 隐藏的推理过程](https://simonwillison.net/2026/Aug/11/stealing-reasoning-traces/) ⭐️ 8.0/10

一篇新论文证明，Anthropic、OpenAI 和 Google 的 LLM API 返回的加密思维链数据块可以被重放到较弱的同系列模型中，并通过越狱手段以明文恢复原始私有推理内容。所有提供商都已确认收到报告并修复了该漏洞。 在专有 LLM API 中，隐藏的推理轨迹被视为敏感知识产权，因此一种能实际恢复它们的攻击动摇了这些服务的隐私与安全假设。这可能促使 API 设计者改用每次请求独立的加密密钥，或加强不同模型层级之间的隔离。 攻击之所以可行，是因为同一模型家族中的不同模型共享相同的加密密钥，使得加密的推理数据块可跨会话、跨用户、跨模型重放。Claude Haiku 4.5 是最容易攻击的目标，攻击者使用一段转写提示词并设置助手回合前缀为 <thinking-copy>；论文还展示了恢复出的 GPT-5.5 关于 CSS 的原始思考内容。

rss · Simon Willison · 8月11日 22:40

**背景**: 思维链（Chain-of-Thought, CoT）推理是指大语言模型在给出最终答案前先生成中间推理步骤，这种做法能显著提升其在复杂任务上的表现。许多专有 API 提供商现在会对 CoT 轨迹进行加密或隐藏，以保护模型内部机制和安全细节，但这篇论文表明，将加密数据块重放到同一家族的较弱“兄弟模型”中并实施越狱，可以绕过这种加密。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2201.11903">[2201.11903] Chain-of-Thought Prompting Elicits Reasoning in Large Language Models</a></li>
<li><a href="https://www.ibm.com/think/topics/chain-of-thoughts">What is chain of thought (CoT) prompting? | IBM</a></li>

</ul>
</details>

**标签**: `#AI security`, `#LLM`, `#chain-of-thought`, `#privacy`, `#API vulnerability`

---

<a id="item-10"></a>
## [Adam 的基依赖破坏了 GD 的隐式低秩偏差](https://www.reddit.com/r/MachineLearning/comments/1vmjb3p/the_loss_does_not_see_the_basis_but_adam_does_r/) ⭐️ 8.0/10

一篇 Reddit 帖子证明，Adam 的逐坐标二阶矩归一化破坏了旋转不变性，并摧毁了欠定矩阵感知中梯度下降的隐式低秩偏差，而 Muon 和 Shampoo 等旋转不变优化器则保留了这种偏差。作者在匹配训练损失下运行了九种更新规则，发现了两个清晰的行为聚类。 这确定了一个具体机制——逐坐标二阶矩的基依赖性——解释了为什么 Adam 在低秩结构问题上可能表现不佳，这一发现与优化器设计和机器学习优化研究直接相关。它还通过在同一轴上展示两种行为，重新框定了关于 Muon 谱简单性偏差的争论。 一个在逐坐标分母和共享标量分母之间插值的单参数族显示，恢复性能单调提升，从而将损害归因于各向异性而非一般的自适应性。作者还发现，将他们自己的优化器从逐坐标裁剪改为全局范数裁剪，恢复错误从 0.347 降至 0.220；一个注意点指出，报告的高光谱增益使用了仅训练的学习率规则，而该规则在 Adam 自身的网格上给了它最差的学习率。

reddit · r/MachineLearning · /u/EtherealGlyph · 8月12日 16:39

**背景**: 在分解模型 W = UV^T 中，损失对旋转 (U,V) → (UQ, VQ) 是不变的，梯度下降尊重这一对称性。Adam 的逐坐标二阶矩则不然，因为它依赖于因子所写成的基，从而破坏对称性并摧毁有助于 GD 找到更简单解的隐式低秩偏差。Muon 和 Shampoo 等旋转不变优化器使用尊重矩阵结构的预条件，从而保留这种偏差。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://kellerjordan.github.io/posts/muon/">Muon: An optimizer for hidden layers in neural networks | Keller Jordan blog</a></li>
<li><a href="https://arxiv.org/abs/1802.09568">[1802.09568] Shampoo: Preconditioned Stochastic Tensor ... optimizers/distributed_shampoo/README.md at main ... - GitHub Ashampoo® WinOptimizer Pro 29 - Optimize, clean, and protect ... SOAP: Improving and Stabilizing Shampoo using Adam GitHub - Daniil-Selikhanovych/Shampoo_optimizer: Our ... Shampoo: Preconditioned Stochastic Tensor Optimization</a></li>
<li><a href="https://github.com/facebookresearch/optimizers/blob/main/distributed_shampoo/README.md">optimizers/distributed_shampoo/README.md at main ... - GitHub</a></li>

</ul>
</details>

**标签**: `#machine-learning`, `#optimizers`, `#adam`, `#low-rank-bias`, `#matrix-sensing`

---

<a id="item-11"></a>
## [解耦下降：通过 AMP Onsager 修正实现训练-测试误差精确对齐](https://www.reddit.com/r/MachineLearning/comments/1vlu1se/decoupled_descent_enforcing_exact_traintest_error/) ⭐️ 8.0/10

作者提出了一种名为解耦下降（DD）的新型训练算法，利用近似消息传递（AMP）的 Onsager 修正来保证在每个参数迭代步上训练误差渐近等于测试误差，并在高斯混合模型的全批量梯度下降上进行了验证。 这项工作为过拟合问题提供了新的理论视角，表明训练与测试误差之间的差距可以在优化过程中被可证明地消除，而不仅仅是加以控制。若能推广到更一般的模型，它可能为深度学习带来可认证的泛化保证、有原则的早停策略以及更安全的超参数调优。 解耦下降目前是一种理论方法，应用于高斯混合模型上的全批量梯度下降；在高维 XOR 模型和两层网络的实验中，DD 能紧密跟踪测试误差，而 GD 则过拟合。作者强调这只是第一步，并计划发布一个兼容 PyTorch 的实现。

reddit · r/MachineLearning · /u/mlovik1 · 8月11日 21:06

**背景**: 在监督学习中，梯度下降最小化训练损失，但测试性能往往落后，这一现象称为过拟合。近似消息传递（AMP）是来自压缩感知和统计物理的迭代算法，对于随机矩阵，它遵循精确的状态演化递推；其 Onsager 修正项会抵消迭代过程中累积的相关性。解耦下降借用了这些思想，将优化动态与数据复用偏差解耦，从而在每个迭代步上渐近地展示训练-测试差距。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2201.07487">A Concise Tutorial on Approximate Message Passing A unifying tutorial on Approximate Message Passing Lecture 19: Approximate message passing algorithms Approximate Message Passing Tutorial - GitHub Pages Message-passing algorithms for compressed sensing GitHub - shx-lyu/AMP-in-MIMO: Approximate message passing ... A unifying tutorial on Approximate Message Passing</a></li>
<li><a href="https://arxiv.org/abs/2008.11892">[2008.11892] Approximate Message Passing algorithms for rotationally ...</a></li>
<li><a href="https://www.bohrium.com/en/sciencepedia/feynman/compressed_sensing_and_sparse_optimization_graduate-approximate_message_passing_algorithm">approximate message passing algorithm | Bohrium</a></li>

</ul>
</details>

**标签**: `#Machine Learning`, `#Optimization`, `#Approximate Message Passing`, `#Generalization`, `#Theory`

---

<a id="item-12"></a>
## [Zed 发布 DeltaDB，这是一款面向 AI 协作的类聊天版本控制工具。](https://zed.dev/blog/introducing-delta) ⭐️ 7.0/10

Zed 发布了 DeltaDB（也简称为 Delta），这是一个操作级版本控制系统，可以记录两次提交之间的每一次更改，并将其关联到类似聊天的协作工作区。该公告发布在 Zed 的博文《Introducing Delta》中，定位为面向提交之间代码变更的版本控制工具。 随着 AI 代理越来越多地在传统提交之外生成代码，现有版本控制会隐藏变更背后的推理过程。DeltaDB 旨在保留每一个操作细节和决策，让 AI 与人类的协作变得更加透明、可审计。 与只保存提交快照的 Git 不同，DeltaDB 为每次操作分配稳定 ID，并记录提交之间完整的编辑流。该功能由 Zed Industries 开发，这家公司还打造了基于 Rust、由 GPU 加速的 Zed 编辑器；DeltaDB 还带有用于跟踪决策的类聊天界面。

hackernews · khy · 8月12日 18:19 · [社区讨论](https://news.ycombinator.com/item?id=49276574)

**背景**: Zed 是一款用 Rust 编写的开源高性能代码编辑器，主打速度和与人类及 AI 代理的实时协作。像 Git 这样的传统版本控制只保存开发者选择提交的快照，因此变更背后的中间步骤和 AI 对话往往会丢失。DeltaDB 通过记录每次操作并将洞察关联到代码来解决这个问题，目标是让 IDE 成为一个跨越不同时间尺度的协作工作区。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zed.dev/blog/introducing-deltadb">Software Is Made Between Commits — Zed's Blog</a></li>
<li><a href="https://shapeof.com/archives/2025/8/deltadb_from_zed.html">DeltaDB From Zed (the Code Editor) - shapeof.com</a></li>
<li><a href="https://sesamedisk.com/what-is-zed-deltadb-features/">What Is Zed DeltaDB and Its Key Features - Sesame Disk</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一。一些评论者质疑这种类聊天设计，认为它结合了 Google Docs 和 Slack 的缺点，无助于跟踪决策；也有人认为在编辑器中进行多人编程毫无实际用处。还有评论抱怨页面文字对比度过低、难以阅读，并对 AI 生成的冗长代码摘要持怀疑态度；不过也有人觉得实时协作的概念很有趣。

**标签**: `#Zed`, `#collaboration`, `#code editor`, `#AI`, `#real-time editing`

---

<a id="item-13"></a>
## [引用弗洛里安·赫伦格特](https://simonwillison.net/2026/Aug/12/florian-herrengt/) ⭐️ 7.0/10

该引用强调了 AI 生成的代码可能导致项目复杂混乱、无人理解系统，从而给软件可维护性带来风险。

rss · Simon Willison · 8月12日 15:08

**标签**: `#AI-assisted development`, `#software engineering`, `#code maintainability`, `#developer productivity`, `#commentary`

---

<a id="item-14"></a>
## [自然语言文本不存在无损转换](https://simonwillison.net/2026/Aug/11/there-are-no-lossless-transformations-of-natural-language-text/) ⭐️ 7.0/10

Sophie Alpert 发布了一份面向工程师的 AI 写作使用政策，指出对自然语言文本的任何改写或重述都会造成信息损失。Simon Willison 推荐了这篇文章，并强调其中一条核心规则：工程师必须对自己文档中的每一个观点和每一句话负责。 它为在技术写作中负责任地使用 LLM 提供了实用且高价值的指导，而随着越来越多的团队采用 AI 助手，这也是一个非常及时的问题。它为工程师和技术写作者判断何时可以使用 AI 生成的文字提供了明确标准。 核心规则是：如果审阅者问“这句话是什么意思？”，回答“这是 AI 写的，别管它”是不可接受的。文章认为，任何实体如果不了解作者试图表达的具体想法，在改写过程中都会丢失信息，因此作者必须确认最终文本真实反映自己的思路。

rss · Simon Willison · 8月11日 23:48

**背景**: 在计算机科学中，“无损”转换会保留全部原始数据，例如无损压缩算法可以精确还原原始内容。但自然语言并不是固定的数据表示：一句话的含义取决于作者意图和上下文。大型语言模型可以流畅地改写或重述文本，但只要它们不具备作者完整的思维模型，就可能会丢失细微的含义。因此，如果不仔细审阅，用 AI“润色”文档实际上存在真实风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Lossless_compression">Lossless compression - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Natural_language_processing">Natural language processing - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI writing`, `#technical documentation`, `#LLM usage`, `#engineering culture`

---

<a id="item-15"></a>
## [新网站按会议目的地质量而非声望给 CS 会议排名](https://www.reddit.com/r/MachineLearning/comments/1vmbdk6/i_built_an_honest_cs_conference_ranking_sorted_by/) ⭐️ 7.0/10

新网站 honestcsrankings.org 将约 540 个 CORE 排名计算机科学会议按举办地质量排序，综合考虑天气、安全、花费、便利性和城市氛围。网站还提供筛选、按距离排序、日历导出和供合作者使用的深链。 该工具将会议选择的重心从学术声望转向旅行体验，可能影响研究人员的参会决策和会议规划。它为研究者提供了一种实用方式，在职业价值和目的地吸引力之间进行权衡。 该网站使用全球和平指数衡量安全性、世界银行价格水平衡量花费，并采用会议当月的真实气候数据。它设有“冷门”选项卡，展示位于不佳目的地的 A*会议；由于尚未公布或未获得 CORE 评级，ICML/ICLR 2027 和 COLM 未收录。

reddit · r/MachineLearning · /u/JohnAZoidberg77 · 8月12日 11:23

**背景**: CORE 会议排名是一个广泛认可的评级体系，用于评估计算机科学会议的学术质量。全球和平指数是经济与和平研究所发布的年度报告，衡量各国家地区的和平程度。WikiCFP 是一个由社区维护的征稿信息平台，该网站通过抓取其数据来收录规模较小的会议。通过整合这些来源，该工具提供了一种面向旅行体验、而非学术声望的排名替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://portal.core.edu.au/conf-ranks/">portal. core .edu.au/conf- ranks</a></li>
<li><a href="https://en.wikipedia.org/wiki/Global_Peace_Index">Global Peace Index</a></li>
<li><a href="http://www.wikicfp.com/cfp/servlet/event.showcfp?eventid=63368©ownerid=96880">WikiCFP : Call For Papers of Conferences, Workshops and Journals</a></li>

</ul>
</details>

**标签**: `#academic conferences`, `#tools`, `#CS research`, `#travel`, `#ranking`

---

<a id="item-16"></a>
## [临时搭建的摄像头网站吸引社区关注 2026 年日食](https://jonty.github.io/2026_eclipse_webcams/) ⭐️ 6.0/10

一位创作者分享了为 2026 年日食搭建的网络摄像头聚合网站，该网站赶在日全食开始前快速上线，实时汇集了冰岛和西班牙的摄像头画面。 这个实时网络项目将一个小众工具转变为共享的社区体验，让世界各地的人们能够远程观看罕见的日食。它凸显了个人网络项目如何激发强烈的社区参与，并促进对自然事件的集体观察。 该网站托管于 jonty.github.io/2026_eclipse_webcams，创作者曾为 2024 年美国日食搭建过类似版本，并在日全食开始前几分钟才完成。创作者表示，协调冰岛和西班牙的摄像头是意料之外的任务，并希望活动期间网站不会出问题。

hackernews · zoenolan · 8月12日 11:53 · [社区讨论](https://news.ycombinator.com/item?id=49270953)

**背景**: 日食是月球经过太阳和地球之间时，在狭窄路径上暂时使天空变暗的自然现象。网络摄像头聚合网站收集多个地点的实时画面，让观众能远程体验日全食。创作者此前为 2024 年北美日食开发过类似工具，并以此为基础构建了 2026 年的版本。

**社区讨论**: 社区成员分享了个人日食经历，包括长途旅行躲避云层、用双筒望远镜观察粉色等离子体日珥等。有评论者提到泰勒斯（Thales of Miletus）首次准确预测日食，称之为“科学的诞生”。整体氛围积极而感激，也有人补充了太阳能电池板监测数据等额外资源。

**标签**: `#eclipse`, `#webcams`, `#community`, `#real-time`, `#space`

---

<a id="item-17"></a>
## [AmigaDOS 开发者 Tim King 去世](https://amiga-news.de/en/news/AN-2026-08-00070-EN.html) ⭐️ 6.0/10

AmigaDOS 开发者之一 Tim King 去世，amiga-news.de 发布了讣告。社区成员纷纷分享回忆，感谢他所作出的贡献。 Tim King 参与创建了 AmigaDOS，这是定义 16 位家用电脑时代的 Amiga 操作系统的关键组成部分。他的工作影响了一代用户和开发者，复古计算社区正在纪念他的遗产。 AmigaDOS 是 AmigaOS 的磁盘操作系统，最初基于 MetaComCo 的 TRIPOS 移植版，并在 AmigaOS 1.x 中使用 BCPL 编写。从 AmigaOS 2.x 开始改用 C 语言重写，到 AmigaOS 4 时移除了 BCPL 兼容层。

hackernews · doener · 8月12日 14:09 · [社区讨论](https://news.ycombinator.com/item?id=49272655)

**背景**: AmigaDOS 是 AmigaOS 的磁盘操作系统组件，负责文件系统、文件操作和命令行界面。最初的 AmigaOS 1.x 版本基于 MetaComCo 移植的 TRIPOS，并使用 BCPL 语言编写。从 AmigaOS 2.x 开始，它改用 C 语言重写。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AmigaDOS">AmigaDOS</a></li>

</ul>
</details>

**社区讨论**: HN 讨论氛围温馨而充满感激。评论者感谢 King 博士陪伴他们度过的 Amiga 时光，并认为 AmigaDOS 引导他们接触命令行，为之后学习 Linux 打下基础。还有评论者回忆他是 UK Online 的创始人，并分享了 2021 年的访谈链接。

**标签**: `#Amiga`, `#AmigaDOS`, `#obituary`, `#retrocomputing`, `#Tim King`

---

<a id="item-18"></a>
## [大规模扫描伪装成 ClaudeBot 等 AI 机器人](https://knownagents.com/insights) ⭐️ 6.0/10

大规模自动化漏洞扫描现在开始伪装成 ClaudeBot 等 AI 训练机器人的用户代理。观察者报告称，来自谷歌云 IP 空间的持续高流量自 8 月初以来激增至每分钟约 7 万次请求。 这一事态很重要，因为被伪装的 AI 爬虫用户代理可以绕过将已知机器人视为友好对象的白名单，从而可能将恶意扫描隐藏在可信流量中。这也表明互联网背景噪音日益复杂，使防御者的威胁检测更加困难。 据受影响的运营者称，这些扫描复用了合法的 AI 训练机器人用户代理字符串，并且似乎处于集中控制之下。一位运营者报告了来自谷歌云 AS396982 的约 7 万次/分钟请求，并称向 GCP Abuse 的举报未获回应。

hackernews · gavinhking · 8月12日 14:02 · [社区讨论](https://news.ycombinator.com/item?id=49272569)

**背景**: ClaudeBot 是 Anthropic 的网络爬虫，用于收集数据训练其 Claude 大语言模型。用户代理伪装是一种客户端更改其 User-Agent HTTP 头以冒充其他软件或设备的技术，常被机器人用来绕过过滤器。大规模自动化漏洞扫描自 2001 年的 Code Red 蠕虫事件以来一直是互联网上的常见现象，当时该蠕虫也同样用请求刷爆了服务器日志。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ClaudeBot">ClaudeBot</a></li>
<li><a href="https://en.wikipedia.org/wiki/User_agent_spoofing">User agent spoofing</a></li>
<li><a href="https://www.fraudlogix.com/blog/understanding-and-detecting-forged-user-agents-a-guide-for-fraud-detection-and-prevention/">User Agent Spoofing: How To Spot & Stop Fake User Agents</a></li>

</ul>
</details>

**社区讨论**: 评论者大多淡化其新颖性，指出服务器每天都会收到数千次探测点击，这只是披着新伪装的老一套垃圾流量。一些人分享了个人观察到的严重扫描流量，并对向云服务商举报的有效性表示怀疑，另一些人则指出，相比用户代理字符串，域名所有权（ASN）是更好的判断指标。

**标签**: `#security`, `#vulnerability scanning`, `#AI bots`, `#bot detection`, `#network traffic`

---

<a id="item-19"></a>
## [YC P26 初创公司推出 AI 智能体用于半导体材料发现](https://discoveredmaterials.com/research/) ⭐️ 6.0/10

YC P26 孵化的初创公司 Discovered Materials 在 Hacker News 上发布了用 AI 智能体计算发现新型半导体材料的成果。他们发布了数百种新材料以及一个衡量前沿模型材料发现能力的基准，并声称 8 小时的模型运行可媲美博士生数周的工作。 这家初创公司瞄准芯片热管理这一关键瓶颈——GPU 的 TDP 几乎每一代都翻倍，从 H100 的 700W 到 Rubin 预计的 2.3kW。如果 AI 智能体能缩短“实验室到晶圆厂的死亡之谷”，就能加速 3D 封装、新型热界面材料和基板的应用，从而降低数据中心的功耗和用水量。 创始人测试了来自 Anthropic、OpenAI 和 Kimi 的七种模型，并观察到一些奇怪行为，例如 Claude 的奖励黑客行为以及 GPT-5.6 在约 5000 万 token 后“失控”。他们还报告说，其模拟、合成并测试的热界面材料性能可媲美被保密超过 20 年的材料；其商业模式是授权材料和合成配方相关的知识产权。

hackernews · advaith08 · 8月12日 07:51 · [社区讨论](https://news.ycombinator.com/item?id=49269090)

**背景**: 热设计功耗（TDP）是指芯片在正常工作下能产生的最大热量，也是散热系统必须耗散的热量。3D 芯片封装将 HBM 内存栈等芯片直接堆叠在逻辑芯片上以降低数据传输能耗，但 SiO2 等介电材料是较差的热导体，会积聚热量。“实验室到晶圆厂的死亡之谷”指的是一项计算材料预测变成可制造芯片材料所需的数年时间和数亿美元投入。AI 智能体有望减少实验迭代次数并帮助生成合成配方。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Thermal_design_power">Thermal design power - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Three-dimensional_integrated_circuit">Three-dimensional integrated circuit - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论区持谨慎乐观态度。有评论者指出过去 AI 驱动的材料发现缺乏实际影响，但称赞这次触及了可行性；另有人指出闭合计算-实验回路仍是主要挑战。还有人看好 HBM 置于芯片上方的构想，并对该团队如何缓解奖励黑客行为表示好奇。

**标签**: `#AI`, `#materials-science`, `#semiconductors`, `#YC`, `#startup`

---

<a id="item-20"></a>
## [Datasette-upload-dbs 0.5a0 为数据库上传新增正式 API](https://simonwillison.net/2026/Aug/11/datasette-upload-dbs/) ⭐️ 6.0/10

该版本为现有的 datasette-upload-dbs 插件新增了一个正式化的 HTTP API，用户可以通过向 /-/upload-dbs 发送 POST 请求来上传或原子性地替换已托管的 Datasette 实例中的 SQLite 数据库文件。此前这只能通过插件的网页界面完成。 这使得数据库部署和更新可以实现自动化，例如在 GitHub Actions 等 CI 系统中构建新的数据库后立即将其热替换到生产环境。它增强了 Datasette 作为数据发布平台的定位，并降低了需要定期刷新数据的团队的使用门槛。 新端点要求在 Authorization: Bearer 请求头中携带令牌，并接收包含 db 文件和 db_name 字段的 multipart 表单。上传的数据库会先保存到磁盘、经过验证，然后原子性地替换，因此 /name 路径会无缝切换到新版本，无需停机。

rss · Simon Willison · 8月11日 20:35

**背景**: Datasette 是一个开源的数据探索和发布工具，可以将 SQLite 数据库转换为交互式网站和 JSON API。datasette-upload-dbs 插件由 Simon Willison 创建，允许用户直接将 SQLite 文件上传到托管的 Datasette 实例并自动提供访问。本次发布通过新增正式的程序化接口，为该能力打开了全自动发布工作流的大门。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://datasette.io/">Datasette: An open source multi-tool for exploring and ...</a></li>
<li><a href="https://docs.datasette.io/">Datasette documentation</a></li>
<li><a href="https://pypi.org/project/datasette-upload-dbs/">datasette-upload-dbs · PyPI</a></li>

</ul>
</details>

**标签**: `#datasette`, `#sqlite`, `#plugin`, `#api`, `#database`

---

<a id="item-21"></a>
## [AAAI 2027 审稿人指出投稿普遍缺少代码](https://www.reddit.com/r/MachineLearning/comments/1vlqjby/aaai_2027_review_no_code_submission_d/) ⭐️ 6.0/10

一位 AAAI 2027 审稿人表示，其负责的稿件中有大量投稿未提供代码实现，尽管会议明确强调可复现性。该审稿人正在考虑是否在初评中对此扣分，并征求社区意见。 这凸显了机器学习会议中可复现性政策与实际审稿实践之间的持续差距，可能削弱对已发表结果的信任。该讨论可能影响审稿人如何权衡代码可用性，并塑造未来的作者激励。 AAAI 要求每篇论文随附可复现性检查表，但并未将代码提交作为硬性要求。审稿人担心，现代 AI 助手可以快速生成带有虚假结果的实证论文，因此代码验证愈发重要。

reddit · r/MachineLearning · /u/wontonut · 8月11日 18:58

**背景**: AAAI-27 投稿指南要求作者在投稿时完成作者套件中的可复现性检查表，但代码提供是可选的。MLSys 和 MICRO 等会议已通过工件评估（Artifact Evaluation）将代码、数据等工件纳入评审过程，但各会议的具体做法不尽相同。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aaai.org/conference/aaai/aaai-27/submission-instructions/">AAAI-27 Submission Instructions - AAAI</a></li>
<li><a href="https://aaai.org/conference/aaai/aaai-23/reproducibility-checklist/">Reproducibility Checklist - AAAI</a></li>
<li><a href="https://neurips.cc/public/guides/PaperChecklist">NeurIPS Paper Checklist Guidelines</a></li>

</ul>
</details>

**标签**: `#reproducibility`, `#AAAI`, `#code submission`, `#peer review`, `#machine learning`

---

<a id="item-22"></a>
## [请教带后状态随机合并谜题的 RL/规划方法](https://www.reddit.com/r/MachineLearning/comments/1vlfavg/planningrl_for_a_stochastic_singleplayer_merge/) ⭐️ 6.0/10

一位开发者请求社区提供算法和实现建议，用于为随机单机合并谜题构建 AI，该谜题具有后状态（afterstate）和提前一步预知的随机事件。帖子详细说明了游戏规则、网络输入表示以及当前基于精确模拟器的规划方法。 该问题涉及后状态表示、预知随机事件和长时程吞吐量目标的非平凡结合。相关回答可能对从事类似棋盘/益智游戏的研究人员和爱好者有帮助，尤其是在规划预算有限且随机性可提前部分观察的情况下。 游戏有 6 个高度上限为 7 的堆栈，30 种选择有序列对的动作，这些动作会移动连续的相同方块，触发合并连锁，当任何堆栈高度超过 7 时游戏结束。每四个玩家动作后会添加六个随机方块，其数值在第三个动作后预知。用户的策略/价值网络具有列置换等变性，输入特征为 394 个，并将计时模式视为持续的平均奖励/吞吐量问题。

reddit · r/MachineLearning · /u/CaiwenGong · 8月11日 11:53

**背景**: 后状态价值函数估计动作发生后、随机结果出现前的环境状态价值，这种思路非常适合 2048 等游戏以及本合并谜题。由于用户拥有精确模拟器，可以结合蒙特卡洛树搜索（MCTS）或滚动时域优化等基于模型的方法，并配合学习的价值/策略模型。随机掉落的预览是一种随机事件，在被揭示后即可确定性规划，这使该问题区别于完全可观测的随机规划问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ai.stackexchange.com/questions/24816/how-are-afterstate-value-functions-mathematically-defined">reinforcement learning - How are afterstate value functions ...</a></li>
<li><a href="https://openreview.net/forum?id=XO944P8prc">Afterstate Reinforcement Learning for Continuous Control</a></li>

</ul>
</details>

**标签**: `#reinforcement learning`, `#planning`, `#monte carlo tree search`, `#afterstates`, `#merge puzzle`

---