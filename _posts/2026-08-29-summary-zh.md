---
layout: default
title: "Horizon Summary: 2026-08-29 (ZH)"
date: 2026-08-29
lang: zh
---

> 从 19 条内容中筛选出 10 条重要资讯。

---

1. [在 RP2350 微控制器上实现微型潜流 Transformer 生成 128x128 人脸图像](#item-1) ⭐️ 9.0/10
2. [腾讯开源 Hy4 预览版：770B 参数 MoE 大模型](#item-2) ⭐️ 8.0/10
3. [AI 代理可将漏洞传言在几分钟内变成实际攻击](#item-3) ⭐️ 8.0/10
4. [百年老算法 SPC 击败 SOTA 时间序列异常检测](#item-4) ⭐️ 8.0/10
5. [美国国土安全部借鲜为人知的传票法秘密获取记者与非营利组织记录](#item-5) ⭐️ 7.0/10
6. [好文化胜过 AI：论生产力秘诀](#item-6) ⭐️ 7.0/10
7. [三星 PIM 存内计算技术：加速 AI 但面临质疑](#item-7) ⭐️ 7.0/10
8. [3.1 万条逐小时 LLM 基准：跨日波动约为日内 3 倍](#item-8) ⭐️ 7.0/10
9. [统计/概率 ML 研究者考虑转投 AISTATS 和 UAI，因顶级会议被 LLM 主导](#item-9) ⭐️ 7.0/10
10. [Reddit 热议：到底什么才算世界模型？](#item-10) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [在 RP2350 微控制器上实现微型潜流 Transformer 生成 128x128 人脸图像](https://www.reddit.com/r/MachineLearning/comments/1w10tax/i_implemented_a_very_tiny_image_generation_model/) ⭐️ 9.0/10

一位开发者在 RP2350 微控制器上实现了一个 240 万至 400 万参数的潜流变换器（latent flow transformer）模型，量化为 int8，约 20 秒即可生成 128×128 的人脸图像。该模型完全在设备端运行，输出可通过显示器显示或经 USB 传输。 这证明了基于变换器的图像生成可以在超低功耗微控制器上运行，挑战了这类模型必须依赖 GPU 或云服务器的传统认知。它为隐私保护、离线运行的嵌入式边缘 AI 应用（如设备端生成艺术、智能传感器或辅助设备）开辟了可能性。 该模型包含 12 层，采用 AdaLN-Zero 条件化，支持无分类器引导（CFG），并利用 ReLU²激活的稀疏性跳过部分计算。推理引擎通过 DMA 从闪存流式加载权重，同时计算前一层，从而在 RP2350 约 520KB 的 SRAM 内运行。

reddit · r/MachineLearning · /u/cpldcpu · 8月28日 19:48

**背景**: 潜流变换器（Latent Flow Transformer, LFT）通过流匹配训练学习到的传输算子来压缩多个层，用单个轻量变换替代沉重的残差堆叠。AdaLN-Zero（自适应 LayerNorm 零初始化）是扩散变换器中使用的条件化机制，通过对特定分支进行零初始化以稳定训练；而 ReLU²激活在稀疏语言模型中被证明具有极佳的稀疏性与性能权衡。RP2350 是一款双核 Cortex-M33 微控制器，拥有约 520KB RAM，常用于爱好者与物联网项目。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2505.14513">Abstract page for arXiv paper 2505.14513: Latent Flow Transformer</a></li>
<li><a href="https://arxiv.org/abs/2402.03804">[2402.03804] ReLU$^2$ Wins: Discovering Efficient Activation Functions for Sparse LLMs</a></li>
<li><a href="https://arxiv.org/html/2608.09438">Unveiling the Secret of AdaLN - Zero in Diffusion Transformer</a></li>

</ul>
</details>

**标签**: `#edge AI`, `#microcontrollers`, `#efficient inference`, `#transformer`, `#image generation`

---

<a id="item-2"></a>
## [腾讯开源 Hy4 预览版：770B 参数 MoE 大模型](https://www.tencent.com/tencent-releases-and-open-sources-tencent-hy4-preview/) ⭐️ 8.0/10

腾讯发布并开源了 Hy4 预览版，这是一款全新的 MoE 旗舰大语言模型，总参数量 770B，激活参数 49B。该模型已在 OpenRouter 上迅速走红，数天内处理了数万亿 token。 这是中国最大科技公司之一在开源 AI 领域的重要发布，将具有前沿能力的模型带入开源生态。其低缓存成本与强劲性能可能加速开源模型的采用，并加剧与 GLM 等其他提供商的竞争。 该模型采用混合专家（MoE）架构，总参数 770B，每个 token 激活 49B 参数，上下文窗口超过 100 万 token。值得注意的是，腾讯表示 Hy4 预览版通过提出方案并迭代结果参与了自己的开发过程，形成了早期递归自我改进循环。

hackernews · shenli3514 · 8月29日 19:33 · [社区讨论](https://news.ycombinator.com/item?id=49492632)

**背景**: Hy4 预览版是腾讯 Hy 系列大语言模型的继任者，由腾讯 Hy 团队开发。OpenRouter 是一个统一 API 平台，开发者可通过单一端点访问多种 AI 模型，该模型在 OpenRouter 的快速采用突显了市场对强大开源模型的需求。关于递归自我改进的说法，呼应了业界对模型辅助 AI 研究与开发日益增长的兴趣。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tencent.com/tencent-releases-and-open-sources-tencent-hy4-preview/">Tencent Releases and Open-Sources Tencent Hy4 preview</a></li>
<li><a href="https://github.com/Tencent-Hunyuan/Hy4-preview">GitHub - Tencent-Hunyuan/Hy4-preview</a></li>
<li><a href="https://hy.tencent.ai/research/hy4-preview?langVersion=en">Introducing Hy4 preview - Tencent Hy</a></li>

</ul>
</details>

**社区讨论**: 评论者指出 Hy4 在 OpenRouter 上‘惊人的人气’，数天内处理了数万亿 token，且缓存成本仅 5%，低于通常的 10%-20%。有人对递归自我改进的说法表示怀疑，也有人基于前代 Hy3 的使用体验称赞其通用智能体质量。还有评论者批评了发布中图表的呈现方式。

**标签**: `#AI`, `#Open Source`, `#Tencent`, `#LLM`, `#Model Release`

---

<a id="item-3"></a>
## [AI 代理可将漏洞传言在几分钟内变成实际攻击](https://simonwillison.net/2026/Aug/28/just-a-rumour-of-a-bug/) ⭐️ 8.0/10

剑桥大学教授、OCaml 编译器核心维护者 Anil Madhavapeddy 报告称，OCaml 的安全补丁在分享后几分钟内就会遭到利用尝试。他还演示了自己的 AI 代理能够找出这些漏洞，并在 Claude Fable 拒绝任务时切换到了 DeepSeek V4 Pro。 这表明 AI 代理几乎能瞬间将漏洞传言转化为实际攻击，打破了传统的负责任披露时间线。开源维护者正被激增的漏洞报告淹没，亟需新的安全流程。 探测针对的是百分号编码的遍历序列，这是一种经典的路径穿越攻击模式。rclone 维护者 Nick Craig-Wood 证实，过去一个月收到了 40 多份安全漏洞报告（而项目前十年总共约 20 份），GitHub 的 CVE 分配时间也从 2–3 天延长到了 3–4 周。

rss · Simon Willison · 8月28日 22:12

**背景**: OCaml 是一种通用、多范式的编程语言，以安全性著称，常用于静态分析和形式化方法。百分号编码（URL 编码）是 URI 中编码任意数据的方法，像 %2e%2e 这样的编码遍历序列可用于绕过过滤器。传统上，安全研究人员会给维护者一段禁运期，以便在公开披露前修复漏洞，但 AI 驱动的自动化探测使这种做法难以为继。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OCaml_programming_language">OCaml programming language</a></li>
<li><a href="https://en.wikipedia.org/wiki/Percent-encoding">Percent-encoding - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek_(product)">DeepSeek (product)</a></li>

</ul>
</details>

**社区讨论**: 在 Hacker News 的评论中，rclone 维护者 Nick Craig-Wood 证实了同样的现象，指出安全漏洞报告激增，其中约 75% 需要实际关注。他还表示，尽管 AI 工具有助于分类，但庞大的数量消耗了大量时间，而 CVE 分配延迟导致发布版本变更日志中只能标注“CVE-PENDING”。

**标签**: `#security`, `#AI agents`, `#open source`, `#automated exploitation`, `#OCaml`

---

<a id="item-4"></a>
## [百年老算法 SPC 击败 SOTA 时间序列异常检测](https://www.reddit.com/r/MachineLearning/comments/1w1wt1s/you_can_beat_sota_time_series_anomaly_detection/) ⭐️ 8.0/10

著名研究者 Eamonn Keogh 在 Reddit 上发帖，展示了一种简单的、有百年历史的统计过程控制（SPC）方法在 TSB-AD-M 时间序列异常检测基准的某些序列上能够取得完美结果，优于最先进（SOTA）方法。他认为这表明当前 TSAD 基准的意义值得怀疑。 这一发现挑战了时间序列异常检测领域标准评估实践的有效性。它表明近年来宣称的许多进展可能只是过于简单的基准造成的假象，因此需要更严格、更具挑战性的评估数据集。 展示的示例来自 TSB-AD-M 基准中的一条 ECG 信号，Keogh 指出许多“TAO”序列用 SPC 解决起来更加容易。他并未声称已解决基准过于简单的问题，但表示自己已完成大部分工作来引入更具挑战性的 TSAD 问题，例如雪橇犬、金枪鱼、燃料电池和智能制造等数据集。

reddit · r/MachineLearning · /u/eamonnkeogh · 8月29日 20:16

**背景**: TSB-AD-M 是由 Paparrizos 等人创建的广泛使用的时间序列异常检测算法评估基准套件，包含来自不同领域、具有多种异常类型且带标注的时间序列。统计过程控制（SPC）是一种经典的质量控制方法，利用控制图监控过程是否保持在预期范围内，简单的 SPC 规则也可以用于时间序列来标记异常点。Keogh 的帖子正是利用这一简单基线来论证 TSB-AD-M 基准“过于简单”，无法支撑有意义的进展声明。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/TheDatumOrg/TSB-AD">GitHub - thedatumorg/TSB-AD: Time-Series Anomaly Detection ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Statistical_process_control">Statistical process control</a></li>

</ul>
</details>

**标签**: `#time-series`, `#anomaly-detection`, `#benchmarks`, `#research-critique`, `#statistical-process-control`

---

<a id="item-5"></a>
## [美国国土安全部借鲜为人知的传票法秘密获取记者与非营利组织记录](https://www.theguardian.com/us-news/2026/aug/29/trump-dhs-1509-summons-records-journalists-nonprofits) ⭐️ 7.0/10

美国国土安全部（DHS）一直援引第 1509 条行政传票，秘密获取记者、非营利组织和工会的通信记录。在数起案件中，DHS 在法院提出质疑后、法官尚未裁决其合法性之前，主动撤回了传票。 这种做法使执法部门能够绕过司法监督，引发了对美国宪法第四修正案和新闻自由的严重关切。同时，它迫使科技和电信公司在缺乏法院命令的情况下，决定是否遵从有争议的政府要求。 在一桩案例中，T-Mobile 向政府提供了某记者六个月的电话记录，包含超过 1 万通通话和短信，且未告知当事人。据报道，谷歌则没有遵从类似要求。DHS 在面临法律挑战后撤回传票，可能是一种刻意避免不利法院裁决的策略。

hackernews · firefax · 8月29日 18:44 · [社区讨论](https://news.ycombinator.com/item?id=49492219)

**背景**: 行政传票是由联邦机构在未经法院事先批准的情况下发出的传票。与司法传票或大陪审团传票不同，行政传票不需要法院命令，但只能通过法院行动来强制执行。自“911”袭击以来，美国国会大幅扩大了这一权限，使 DHS 等机构获得了广泛的调查权力。批评者认为这绕过了传统的搜查令要求并违反宪法第四修正案，而支持者则视其为高效的调查工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Administrative_subpoena">Administrative subpoena</a></li>
<li><a href="https://www.justice.gov/archives/jm/criminal-resource-manual-408-definitions-judicial-subpoena-administrative-summons-and-formal">Justice Manual | 408. Definitions of Judicial Subpoena, Administrative Summons and Formal Written Request. | United States Department of Justice</a></li>

</ul>
</details>

**社区讨论**: 社区评论者对企业常常服从此类传票表示不满，有人指出 T-Mobile 屈服了而谷歌没有。还有人建议记者自行托管电子邮件服务以摆脱中心化系统，并提到了 tmailplus。此外也有对当前政治气候的讽刺评论，以及关于获取个人 IP 地址段需要暴露大量个人信息的困难。

**标签**: `#privacy`, `#surveillance`, `#law`, `#journalism`, `#civil liberties`

---

<a id="item-6"></a>
## [好文化胜过 AI：论生产力秘诀](https://newsletter.eng-leadership.com/p/good-culture-is-the-biggest-productivity) ⭐️ 7.0/10

一篇观点文章认为，强大的团队文化比采用 AI 更能驱动生产力。此文发表于工程领导力通讯，并在 Hacker News 上引发了热烈讨论，评论者补充了更多细节。 这一及时的辩论挑战了当前以 AI 为中心的生产力叙事，敦促领导者将文化作为基础杠杆优先考虑。它影响着工程管理者在痴迷技术的行业中如何分配时间、预算和注意力。 评论者引用了现实案例：一个由“负责人”组成的团队将 Jira 工单自动转为 PR，结果令人灰心且毫无成效。相反，一个 20 人、技能平平但彼此喜欢且流动率极低的团队，成为某位首席工程师见过的最具生产力的团队。

hackernews · gpi · 8月29日 17:19 · [社区讨论](https://news.ycombinator.com/item?id=49491568)

**背景**: 关于生产力的讨论往往聚焦于采用 AI 等新工具。然而，这一论点认为心理安全感、信任和一致性能够产生任何工具都无法匹敌的复利式增益。文化还决定了 AI 是否被自下而上地采用并有效使用，正如一位评论者所指出的。这与工程管理和组织健康的更广泛讨论相关联。

**社区讨论**: 总体情绪是赞同论文观点，但评论者补充了细微差别。有人指出 AI 会加速功能失调，让你更快地到达错误的地方，而好的文化则能加速成功。另有人指出部署 AI 比创造好文化更容易，还有几位强调，在鼓励主动性的文化中，自下而上推动 AI 采用效果最佳。

**标签**: `#company culture`, `#productivity`, `#AI`, `#engineering management`

---

<a id="item-7"></a>
## [三星 PIM 存内计算技术：加速 AI 但面临质疑](https://chipsandcheese.com/p/hot-chips-2026-samsungs-processing) ⭐️ 7.0/10

三星在 Hot Chips 2026 上展示了其存内处理（PIM）技术，包括 LPDDR5X-PIM，声称 AI 推理性能比标准 LPDDR5X 快 3.01 倍，带宽提升 8 倍。该方案将计算逻辑直接嵌入 DRAM，让部分计算在数据所在地完成。 PIM 直接针对限制 AI 加速器性能和能效的“存储墙”，通过减少数据搬运来改善。若被广泛采用，可能重塑 AI 硬件与软件的设计方式，但仍面临生态和可编程性方面的重大挑战。 该实现是在 DRAM 单元旁加入一个小型逻辑单元，支持基本的内存内计算。三星表示，通过将部分数据计算从主 AI 加速器卸载到内存中，可以降低能耗和数据传输开销，但依赖专用内存也可能带来新的限制。

hackernews · ingve · 8月29日 06:06 · [社区讨论](https://news.ycombinator.com/item?id=49487341)

**背景**: 传统冯·诺依曼架构将内存与处理器分离，数据必须在两者之间搬运，形成所谓“存储墙”瓶颈。存内处理（PIM）将计算嵌入或靠近内存，三星自 2021 年起就通过 AMD 加速器中的 HBM-PIM 进行试点，现在又将其扩展到 LPDDR5X。这一概念在学术界已被探讨数十年，但实际落地仍然有限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://semiconductor.samsung.com/news-events/tech-blog/hbm-pim-cutting-edge-memory-technology-to-accelerate-next-generation-ai/">HBM-PIM: Cutting-edge memory technology to accelerate next-generation AI | Samsung Semiconductor Global</a></li>
<li><a href="https://www.tomshardware.com/pc-components/dram/hot-chips-2026-samsung-makes-lpddr5x-smart-with-logic-unit-in-memory-lpddr5x-pim-is-3-01x-faster-than-lpddr5x-in-ai-inference-with-8x-the-bandwidth">Hot Chips 2026: Samsung makes LPDDR5X smart with logic unit in memory — LPDDR5X-PIM is 3.01x faster than LPDDR5X in AI inference with 8x the bandwidth | Tom's Hardware</a></li>
<li><a href="https://www.mk.co.kr/en/it/12136338">Samsung Electronics has proposed "PIM (Processing In Memory)" as a new solution to artificial intell.. - MK</a></li>

</ul>
</details>

**社区讨论**: 评论者指出这类构想历史悠久，可追溯到 1980 年代，并对实际落地表示怀疑，因为每年有大量创新加速器最终未能商用。也有人认为该方案对软件开发者限制很大，并质疑矩阵乘法能否在内存内高效利用计算，因为数据移动依然不可避免。

**标签**: `#hardware`, `#processing-in-memory`, `#semiconductors`, `#AI`, `#computer-architecture`

---

<a id="item-8"></a>
## [3.1 万条逐小时 LLM 基准：跨日波动约为日内 3 倍](https://www.reddit.com/r/MachineLearning/comments/1w1jp1j/i_analyzed_31352_hourly_llm_benchmark_scores/) ⭐️ 7.0/10

一项基于 31,352 个逐小时 LLM 基准分数的分析显示，日内分数波动为 2.8 分，而日间波动为 8.4 分，后者约为前者的 3 倍。作者据此构建了开源系统 AIStupidLevel，用于持续评估和漂移检测，并公开了实时仪表盘。 这项分析揭示了生产环境中的 LLM API 模型并非静态：由于提供商更新或配置变化，模型性能会随时间漂移，而常规单次评测无法捕捉这些变化。AIStupidLevel 在可用性、错误率、延迟和成本之外增加了“模型能力”可观测性，有助于开发者检测性能劣化并做出更可靠的路由决策。 评测使用归一化的 0-100 综合分数，涵盖编程、推理、工具调用和 canary 任务；每项任务执行 5 次并聚合成中位数。漂移检测基于每日中位数和顺序变点检测（CUSUM），只有超过历史方差和最小效应阈值的变化才被判定为劣化或恢复。目前该系统已积累 169,858 次基准运行、104,458 个分数、81 个历史模型标识符，覆盖 6 个活跃提供商。

reddit · r/MachineLearning · /u/ionutvi · 8月29日 11:08

**背景**: 大多数 LLM 评测只在单一时间点测量一次，隐含地把模型当作静态系统。实际上，托管式 API 模型会被提供商更新或重新配置，且每次生成结果具有随机性，因此分数会在小时和日之间波动。AIStupidLevel 是一个开源持续评测系统，它反复运行标准化的编程、推理、工具调用和 canary（金丝雀）任务，利用多次运行的聚合值，并通过变点检测把随机噪声与持续性漂移区分开来。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/AIStupidLevel">AIStupidLevel (AI Stupid Level) - Hugging Face</a></li>
<li><a href="https://israynotarray.com/en/ai/2026/06/16/aistupidlevel-llm-degradation-monitor/">Is AI Getting Quietly Dumber? AIStupidLevel: A 24-Hour Watchdog for LLM ...</a></li>
<li><a href="https://studioplatforms.eu/products/aistupidlevel">AI Training Data & Benchmarking Platform | AIStupidLevel.info</a></li>

</ul>
</details>

**标签**: `#LLM`, `#benchmark`, `#evaluation`, `#stability`, `#time-series`

---

<a id="item-9"></a>
## [统计/概率 ML 研究者考虑转投 AISTATS 和 UAI，因顶级会议被 LLM 主导](https://www.reddit.com/r/MachineLearning/comments/1w0kipf/where_to_submit_statprob_ml_d/) ⭐️ 7.0/10

一位统计与概率机器学习研究者在 Reddit 上表示，ICLR、NeurIPS 等顶级会议已被 LLM 和智能体相关论文主导，因此正在考虑将 AISTATS 和 UAI 作为替代投稿场所。 这反映出更广泛的生态变化：非 LLM 的机器学习研究可能不再在最高知名度的会议上找到自然归属，可能会重塑职业激励，以及严格的统计 ML 工作在哪里发表和讨论。 作者 u/didimoney 提到 Arnaud Doucet、Aapo Hyvärinen、Christian Naesseth 和 Stefano Ermon 等学者，并指出这些资深研究者仍在顶会发表。AISTATS 2025 将于 2025 年 5 月 3-5 日在泰国迈考举行，UAI 则自称是不确定性 AI 领域的首要会议。

reddit · r/MachineLearning · /u/didimoney · 8月28日 08:16

**背景**: ICLR 和 NeurIPS 是最负盛名的机器学习会议之一，近年来其录用论文和研讨会越来越被大语言模型（LLM）和智能体 AI（agentic AI）主题主导。AISTATS 是计算机科学、人工智能、机器学习和统计学交叉领域的会议，而 UAI（人工智能不确定性会议）则聚焦于不确定性下的知识表示、学习和推理。两者通常被认为是统计/概率 ML 领域的强会议，但知名度不如顶会。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aistats.org/aistats2025/">Home| Artificial Intelligence and Statistics Conference</a></li>
<li><a href="https://www.auai.org/uai2025/">uai2025 - auai.org</a></li>
<li><a href="https://virtual.aistats.org/Conferences/2025">2025 Conference</a></li>

</ul>
</details>

**标签**: `#ML research`, `#academic publishing`, `#statistical ML`, `#ICLR`, `#NeurIPS`

---

<a id="item-10"></a>
## [Reddit 热议：到底什么才算世界模型？](https://www.reddit.com/r/MachineLearning/comments/1w16jwj/wtf_is_a_world_model_d/) ⭐️ 6.0/10

一位用户在 r/MachineLearning 上发起了一个概念性讨论，询问什么才算世界模型，并质疑物理引擎、模拟器、游戏世界模型、数字孪生以及基于机器学习的流体模拟器是否符合这一定义。该帖子凸显了该领域定义上的模糊性，但并未提出新的技术发现。 世界模型是一个快速发展的研究领域，尤其是在视频生成和强化学习中，但其精确定义仍存在争议。学界如何在“学习到的世界模型”与“经典模拟器”之间划清界限，可能会影响研究目标、评估方式以及对试图理解或模拟现实世界的 AI 系统的预期。 该用户引用了一个定义，要求世界模型“基于学习到的表征运行，而非仅仅依赖手工编写的物理规则”，这意味着物理对应物是可选的，但也引出了关于机器学习加速物理模拟的更多问题。帖子还询问该术语是否应仅限于旨在建模整个真实世界的模型，这样就会排除游戏专用或任务专用的模拟器。

reddit · r/MachineLearning · /u/neutrino_boy · 8月28日 23:37

**背景**: 在人工智能领域，世界模型通常被理解为一种系统，它学习环境的内部表征，并能够预测或模拟环境的未来状态，常用于强化学习和规划。最近所谓的“世界模型”很多是视频生成系统，能够生成合理的后续帧，但该术语也涵盖更广泛的物理现实模拟工作，例如 Genie 3 和 World Labs 等项目。因此研究者提出了一种功能性分类，区分“帧生成模型”和“真正的模拟器”。Reddit 用户所描述的模糊性，正是当前研究界关于“仅靠模拟是否就算理解”这一争论的体现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/World_model_(artificial_intelligence)">World model (artificial intelligence) - Wikipedia</a></li>
<li><a href="https://arstechnica.com/ai/2026/07/simulating-everything-sort-of-the-promise-and-limits-of-world-models/">Simulating everything, sort of: The promise and limits of world models - Ars Technica</a></li>
<li><a href="https://drfeifei.substack.com/p/a-functional-taxonomy-of-world-models">A Functional Taxonomy of World Models - Dr. Fei-Fei Li</a></li>

</ul>
</details>

**标签**: `#world models`, `#machine learning`, `#reinforcement learning`, `#AI definitions`, `#conceptual`

---