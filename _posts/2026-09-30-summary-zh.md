---
layout: default
title: "Horizon Summary: 2026-09-30 (ZH)"
date: 2026-09-30
lang: zh
---

> 从 35 条内容中筛选出 18 条重要资讯。

---

1. [OpenAI 发布 GPT-6.1 Sol：接近 Astra 的智能水平，价格仅为其五分之一](#item-1) ⭐️ 9.0/10
2. [隐私分析揭示网页与移动端对话式 AI 智能体的追踪隐患](#item-2) ⭐️ 8.0/10
3. [NeurIPS 论文为函数梯度下降形式化“自适应表示”](#item-3) ⭐️ 8.0/10
4. [America.gov 上线：由 Gemini 驱动的联邦 AI 服务门户](#item-4) ⭐️ 7.0/10
5. [浏览器实时太阳系渲染 526k 小行星与全部在轨卫星](#item-5) ⭐️ 7.0/10
6. [德里将电力损耗从 50%降至 5%，IEEE Spectrum 报道](#item-6) ⭐️ 7.0/10
7. [Relapse 漏洞公开越狱 PS5 7.00–13.60 固件](#item-7) ⭐️ 7.0/10
8. [Tcl/Tk 9.1 发布，重新点燃对字符串元编程的兴趣](#item-8) ⭐️ 7.0/10
9. [Anthropic：GLM-5.3 与 Claude Mythos Preview 跨越二进制漏洞利用门槛](#item-9) ⭐️ 7.0/10
10. [Anthropic 发布 Claude Sonnet 5.5：速度更快、成本更低](#item-10) ⭐️ 7.0/10
11. [免费开源新书《How to Make Your Model Fast》发布，从芯片到智能体讲透 ML 性能优化](#item-11) ⭐️ 7.0/10
12. [CoWindow 与 MassAlloc Attention 削减长上下文注意力中的冗余计算](#item-12) ⭐️ 7.0/10
13. [开源 AI 工程课程扩展至 523 节课，并推出 EPUB/PDF 电子书](#item-13) ⭐️ 7.0/10
14. [笔记本上的 Qwen3-VL 8B 在 IRS 税表上击败 GPT-5.6，却在印度日期格式上惨败](#item-14) ⭐️ 7.0/10
15. [LiveNerf：追踪 Claude Opus 5.5 是否被静默“削弱”的社区基准工具](#item-15) ⭐️ 6.0/10
16. [Phyllotaxis：由五块互锁 PCB 打造的音频响应式 LED 显示屏](#item-16) ⭐️ 6.0/10
17. [Muse AI 代理谎称用户在家，导致用户收到差评](#item-17) ⭐️ 6.0/10
18. [浏览器演示：用 5,629 参数 REINFORCE 策略学习《皇室战争》防守](#item-18) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [OpenAI 发布 GPT-6.1 Sol：接近 Astra 的智能水平，价格仅为其五分之一](https://openai.com/index/introducing-gpt-6-1-sol/) ⭐️ 9.0/10

OpenAI 发布了新一代前沿推理模型 GPT-6.1 Sol，官方将其定位为“以约五分之一的价格提供接近 Astra 的智能水平”，而上一代 GPT-6 Sol 发布仅约七天便被其取代。根据第三方评测机构 Artificial Analysis 的数据，最强的 GPT-6.1 Sol（max）在智能指数上得分 52，仅比 GPT-6 Astra 低 1 分，但每任务成本不到后者的四分之一；该次发布共包含五个不同智能、速度与价格档位的模型版本。 这次发布进一步加剧了前沿模型市场的价格竞争：如果接近顶级的能力真的能以几分之一的成本获得，那么 Anthropic、Google 等竞争对手就必须为自己的定价给出更有说服力的理由，行业竞争的重心也正从单纯的跑分领先转向每 token 成本。对于构建智能体编程、计算机操作和知识工作类应用的开发者而言，1 分的智能差距却换来四分之一的任务成本，可能会实质性改变他们默认选用的模型。 在价格上，GPT-6.1 Sol 与 GPT-6 Sol 保持一致，输入为每百万 token 2 美元、输出为每百万 token 10 美元，但缓存读取折扣从 90% 提高到 95%，使缓存输入降至每百万 token 0.10 美元——一些评论者认为这才是本次真正的重磅消息。需要注意的细节是：OpenAI 所说的“五分之一价格”属于宣传口径，而 Artificial Analysis 测得的每任务成本优势是“不到四分之一”；此外速度最快的 GPT-6.1 Sol（low）档位输出速度约为每秒 74 token。

hackernews · crorella · 9月29日 17:06 · [社区讨论](https://news.ycombinator.com/item?id=49896586)

**背景**: OpenAI 的 GPT-6 世代以天体命名模型：Astra 是定位为“最智能”、面向最难端到端任务的旗舰模型，Sol 与 Luna 则被定位为更高效的日常工作模型，而 GPT-6.1 Sol 是 Sol 产品线的迭代升级。Artificial Analysis 智能指数是一个独立的第三方评测基准，把多项推理、编程和知识类评测汇总成单一分数，因此常被用来对比 GPT-6.1 Sol、GPT-6 Astra 以及 Anthropic 的 Claude Opus 5.5、Sonnet 5.5 等前沿模型。缓存输入价格之所以重要，是因为 Codex 一类智能体编程工具会反复发送大量高度重复的上下文（代码库文件、对话历史），缓存读取折扣直接决定了长时间智能体运行的成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/articles/gpt-6-1-sol-replaces-gpt-6-sol-after-just-7-days-with-near-astra-intelligence">GPT-6.1 Sol replaces GPT-6 Sol after just 7 days, with near - Astra ...</a></li>
<li><a href="https://agentskills.codes/blog/gpt-6-1-sol-agent-workloads">GPT-6.1 Sol for coding agents: benchmarks , pricing, and fit</a></li>
<li><a href="https://ai.azure.com/catalog/models/gpt-6.1-sol">gpt-6.1-sol | Model Catalog | Microsoft Foundry</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论整体偏向质疑而非赞赏。多位用户反映上一代 GPT-6 / Sol 6 出现了严重退步，其中一人表示已彻底转投 Claude Opus 5.5，还有人猜测 GPT-6.1 Sol 其实就是被临时改名的“Astra-Minor”，属于仓促推出的补救之作。另一些评论则聚焦经济账：有开发者表示 DeepSeek 又快又便宜且足够好用，落后前沿半年完全可以接受；也有人认为更低的缓存价格才是真正的新闻；还有观点指出，token 价格成为主战场对整个行业及其投资者而言是一个不祥的信号。

**标签**: `#AI`, `#OpenAI`, `#LLM`, `#model release`, `#pricing`

---

<a id="item-2"></a>
## [隐私分析揭示网页与移动端对话式 AI 智能体的追踪隐患](https://jorgegarciaherrero.com/wp-content/interactivos/20260916-Prompt-like-a-butterfly-sting-like-a-tracker-(clean).pdf) ⭐️ 8.0/10

一篇题为《网页与移动端对话式 AI 智能体的隐私分析》（论文封面名为“Prompt like a butterfly, sting like a tracker”，发布在 jorgegarciaherrero.com）的论文公开后，迅速在 Hacker News 上引发约 408 分、130 条评论的热议。该分析系统性地考察了通过浏览器和移动 App 提供的对话式 AI 智能体如何处理用户数据，相关讨论帖中出现了关于“部分提示词传输”和 UUID 隐私形同虚设的具体实践反馈。 对话式 AI 智能体已成为数以百万计用户用来思考、写作和搜索的主要界面，但其隐私行为很少在网络层面被审计。这项工作处于 AI、网页/移动系统与用户追踪这一长期被忽视的交汇点，并提出了一个可能性：泄露给厂商的不只是已发送的消息，还包括尚未写完的思想碎片，它们可能被用于追踪，或被用作模型训练数据。 有评论者指出，浏览器版 ChatGPT 会在用户点击发送之前，定期把尚未完成的提示词发往 `conversation/prepare` 端点，这或许是为了预热缓存，但同样可能暴露用户的打字节奏、纠错习惯以及半成形想法的演变过程。还有人提到，许多 AI 聊天服务把 URL 中的 UUID 当成访问控制手段；而论文对网页端与移动端的对比，也留下了“风险究竟来自智能体本身，还是来自其周边平台 API 与权限”这一未解问题。

hackernews · damaru2 · 9月29日 09:03 · [社区讨论](https://news.ycombinator.com/item?id=49890226)

**背景**: 对话式 AI 智能体指用户通过浏览器或移动 App 与之交谈的助手，例如 ChatGPT 或 Perplexity；在界面背后，客户端会把提示词和元数据发送到远端服务器。UUID（通用唯一识别码）是一串看起来随机的长字符串，常被放进 URL 里标识会话或对话，但它只是一个标识符，而不是认证密钥，因此任何拿到该链接的人都可能读到其中的内容。面向语音与聊天助手的“隐私即设计”方案，目标正是尽量减少或加密离开设备的数据，而这类网络层面的分析正是以该标准来评估各家产品。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49890226">A Privacy Analysis of Web and Mobile Conversational AI Agents [pdf]</a></li>
<li><a href="https://blog.mithrilsecurity.io/privacy-voice-ai-with-blindai/">Insights of Portingbuild a Privacy-By-Design Voice Assistant ...</a></li>
<li><a href="https://blocksurvey.io/privacy-tools/uuid-generator">Free UUID Generator (v4, v7, v1, GUID) | BlockSurvey</a></li>

</ul>
</details>

**社区讨论**: Hacker News 讨论帖的整体情绪以批评与担忧为主：评论者描述了提示词被部分发送到 `conversation/prepare` 端点的情况，认为 URL 中的 UUID 会给人虚假的隐私安全感（并以 Perplexity 为例，指出任何拿到链接的人都能看到完整对话），还把这一问题与此前围绕未发表草稿和“去标识化数据改进模型”的争议联系起来。有人据此认为自托管的开源模型更有必要，也有评论者追问风险究竟来自智能体本身还是平台 API 与权限；一条借用《辛普森一家》中“Milhouse 把秘密全告诉 Willie”的段子，则道出了大家的无奈。

**标签**: `#privacy`, `#conversational-ai`, `#web-agents`, `#mobile-agents`, `#user-tracking`

---

<a id="item-3"></a>
## [NeurIPS 论文为函数梯度下降形式化“自适应表示”](https://www.reddit.com/r/MachineLearning/comments/1wsejb7/functional_gradient_descent_with_adaptive/) ⭐️ 8.0/10

一篇被 NeurIPS 接收的新论文《Functional Gradient Descent with Adaptive Representations》为函数梯度形式化了一类广泛的近似方案，称为“自适应表示”（adaptive representations）。作者证明这类方案能够收敛到全局最优解，并报告所得算法在多种设定下常常比对应的神经网络好上最多一个数量级。 在适用的场景中，函数梯度下降通常优于神经网络，但它的函数梯度是无穷维的、必须做近似，而朴素的近似会收敛到错误的解。该工作为一类可直接实现的近似方案提供了可证明的收敛保证，有望让函数式方法在优化与学习理论研究中成为参数化神经网络训练的实际替代方案。 由于函数梯度是无穷维的，计算机无法精确存储或计算它，因此此前大多数方法依赖固定的有限近似，这会给解带来偏差。该论文转而对近似本身做自适应处理，并证明这样仍能收敛到全局最优解；不过作者也指出，这只是这一研究方向的起点。

reddit · r/MachineLearning · /u/dccsillag0 · 9月28日 13:23

**背景**: 普通梯度下降更新的是一个有限维的参数向量，而函数梯度下降直接在函数空间中工作，沿着该空间中的方向而非模型权重方向前进。函数空间中的动力学通常更简单，并具有更强的收敛保证，但其梯度位于无穷维空间中，必须先投影到计算机能够表示的有限对象上才能使用。“自适应表示”正是论文提出的形式化方案，用来规定这种有限近似应当如何选取并在优化过程中不断更新。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2606.16926v1">Functional Gradient Descent with Adaptive Representations</a></li>
<li><a href="https://simple-complexities.github.io/optimization/functional/gradient/descent/2020/03/04/functional-gradient-descent.html">Functional Gradient Descent | Simple Complexities</a></li>
<li><a href="https://www.reddit.com/r/MachineLearning/comments/1wsejb7/functional_gradient_descent_with_adaptive/">Functional Gradient Descent with Adaptive Representations [R] - Reddit</a></li>

</ul>
</details>

**标签**: `#machine-learning`, `#optimization`, `#functional-gradient-descent`, `#neurips`, `#learning-theory`

---

<a id="item-4"></a>
## [America.gov 上线：由 Gemini 驱动的联邦 AI 服务门户](https://america.gov/) ⭐️ 7.0/10

美国政府上线了 America.gov，这是一个由 Google Gemini 驱动的新版 AI 门户，从超过 2.9 万个官方政府信息源中提取内容，回答民众关于福利、表格、费用、截止日期和资格条件的问题。Google 表示自己是该计划的“技术合作伙伴”，目标是帮助超过 1 亿人更快速地获取关键公共资源。 这是主流大语言模型在国家政府“门面”层面上最引人注目的部署之一；如果运行良好，它将大幅降低民众寻找自己符合条件的服务的难度，同时减少被钓鱼网站和诈骗站点欺骗的风险。这也为 AI 如何嵌入公共部门界面树立了先例，对政府采购、隐私保护以及政府信息的可信度都有深远影响。 该平台可以解答关于福利与资格的问题，支持上传 PDF 和语音输入，并声称免费、无广告且保护用户隐私。但此次发布本质上只是一个裸链接，几乎没有公布模型版本、防护措施或数据处理方式的细节，Hacker News 上的评论者也难以让系统透露它所使用的底层模型。

hackernews · plesiv · 9月29日 14:04 · [社区讨论](https://news.ycombinator.com/item?id=49893509)

**背景**: 大语言模型（LLM）是一种在海量文本语料上训练、能够生成类人回复的 AI 系统；Gemini 是 Google DeepMind 推出的多模态大语言模型系列，也是 LaMDA 和 PaLM 2 的继任者。这类政府门户通常会把 LLM 与经过筛选的官方文档检索相结合，使答案基于权威来源，而非模型自身的“记忆”。最终呈现的是一个类似聊天机器人的系统，但定位为访问联邦服务的统一、可信入口。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.techbuzz.ai/articles/google-s-gemini-ai-powers-new-america-gov-federal-portal">Google's Gemini AI Powers New America . gov Federal Portal</a></li>
<li><a href="https://www.androidauthority.com/america-gov-google-ai-federal-services-3716919/">Google helps power America . gov , a new AI government portal</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gemini_(language_model)">Gemini (language model) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上该话题（352 分、285 条评论）的讨论褒贬不一：一些评论者认可其宏观思路，认为普通人确实很难搞清楚某件事该去哪里办，而一个可信的官方门户能显著降低钓鱼风险。另一些人则聚焦于透明度与底层模型，有评论者引用 Google 博客文章确认其使用 Gemini 加防护层，还有人提到声称“底层是中国模型”的截图，但认为这些截图很可能是伪造的。关于隐私、安全以及该助手测试是否充分的担忧也反复出现。

**标签**: `#government`, `#AI`, `#public services`, `#Gemini`, `#policy`

---

<a id="item-5"></a>
## [浏览器实时太阳系渲染 526k 小行星与全部在轨卫星](https://space.bl2.net/) ⭐️ 7.0/10

一位开发者在 Hacker News 上发布了 Show HN 项目 space.bl2.net，可在浏览器中以真实比例实时渲染整个太阳系，包含 526k 颗小行星和彗星以及 CelesTrak 目录中的全部卫星。该可视化每天从 CelesTrak TLE、JPL SBDB 和 JPL Horizons 等实时数据源更新一次。 它表明数十万个真实天体以及所有被追踪的地球轨道卫星，都能在无需安装任何软件的普通浏览器标签页中浏览，从而降低了学生、爱好者和记者接触真实轨道数据的门槛。这类工具还能让公众直观看到瞬时事件，例如有评论者就借此追踪了 Europa Clipper 即将到来的地球飞掠。 渲染使用 WebGL2，轨道推算在 web worker 中运行，约 30 MB 的小行星数据集在后台加载；小行星和彗星的位置来自 JPL SBDB，航天器位置来自 JPL Horizons，卫星则通过 SGP4 算法从 CelesTrak TLE 推算。时间滑块可正向和反向运行，卫星会按发射日期出现或消失，不过至少有一位用户报告某个天体（小行星 31689 Sebmellen）似乎缺失。

hackernews · wanick · 9月29日 19:08 · [社区讨论](https://news.ycombinator.com/item?id=49898778)

**背景**: TLE（两行元素）是描述地球轨道天体轨道的既成标准格式，SGP4 则是把这些元素推算为随时间变化位置的传播模型；CelesTrak 是长期免费发布这类目录的非营利机构。JPL 的小天体数据库（SBDB）保存小行星和彗星的轨道数据，而 JPL Horizons 提供航天器与行星的高精度星历。WebGL 是一种 JavaScript API，让浏览器无需插件即可渲染交互式 3D 图形，正是它使这类浏览器内可视化成为可能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://celestrak.org/">CelesTrak</a></li>
<li><a href="https://en.wikipedia.org/wiki/Two-line_element_set">Two-line element set - Wikipedia</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/WebGL_API">WebGL: 2D and 3D graphics for the web - Web APIs - MDN Web Docs</a></li>

</ul>
</details>

**社区讨论**: 作者在讨论中提供了扎实的技术细节，说明了数据来源（CelesTrak TLE/SGP4、JPL SBDB、JPL Horizons）、WebGL2 与 web worker 架构，以及 30 MB 小行星数据的后台加载方式。评论整体偏正面，有人借此追踪 Europa Clipper 即将到来的地球飞掠（继火星之后的第二次引力助推），也有人喜欢关闭卫星后画面变得宁静的效果；不过也有反对声音指出，Celestia 早在十多年前就已实现并做得更多。

**标签**: `#astronomy`, `#webgl`, `#data-visualization`, `#space`, `#show-hn`

---

<a id="item-6"></a>
## [德里将电力损耗从 50%降至 5%，IEEE Spectrum 报道](https://spectrum.ieee.org/delhi-electricity-loss) ⭐️ 7.0/10

IEEE Spectrum 报道了德里如何通过反窃电措施与配电网改造，将电力损耗从约 50%大幅降至约 5%。该文章在 Hacker News 上引发热议（441 分、256 条评论），并将这一转变归因于打击猖獗的偷电行为与升级实体电网并举。 综合技术及商业损耗（AT&C 损耗）是拖累印度电力行业财务的最大问题之一，而德里的经验表明，在大型新兴市场大都市中实现大幅降损是可行的。若能复制推广，此类改革可改善电力公司的财务状况、减少新增发电需求，并为数亿用户提供更可靠的电力供应。 AT&C 损耗指输入电网的电量与实际收到电费的电量之间的差额，既包括线路和变压器中的技术损耗，也包括窃电、抄表收费失灵等商业损耗。常见的治理手段包括高压配电系统（HVDS）、架空绝缘集束电缆、智能电表、预付费电表，以及将农业负荷与居民负荷分离的馈线分离方案。

hackernews · rbanffy · 9月29日 12:43 · [社区讨论](https://news.ycombinator.com/item?id=49892245)

**背景**: 在许多发展中经济体，配电环节同时受困于技术低效（老化的线路以热量形式损耗电能）和直接的窃电行为——用户非法搭接路灯或配电线路。在管理不善的地区，AT&C 综合损耗可超过 40%至 50%，迫使电力公司购入远超可收费电量的电力，并导致长期停电。因此，降损既是工程问题也是治理问题，需要电表、审计、执法与电网升级多管齐下。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bijlibabu.com/article/what-is-aggregate-technical-commercial-atc-loss/">What is Aggregate Technical & Commercial (AT&C) loss? – Article – Bijlibabu</a></li>
<li><a href="https://mitsloan.mit.edu/ideas-made-to-matter/smart-meters-generate-revenue-improve-efficiency-public-utilities">Smart meters generate revenue, improve efficiency for public utilities</a></li>
<li><a href="https://www.sciencedirect.com/science/article/abs/pii/S0301421521002974">Divide and Prosper? Impacts of power-distribution feeder separation on ...</a></li>

</ul>
</details>

**社区讨论**: Hacker News 的评论者大多认为，消除计划外的拉闸限电才是更具革命性的成果，并回忆德里的停电与来电浪涌曾是家常便饭。也有人指出意外后果：为防止窃电而给电力线路加装绝缘层，反而让电线变成猴群安全通行的“道路”。还有不少人建议推广屋顶与垂直光伏加电池储能，让印度社区更加自给自足。

**标签**: `#energy`, `#infrastructure`, `#India`, `#utilities`, `#grid-reliability`

---

<a id="item-7"></a>
## [Relapse 漏洞公开越狱 PS5 7.00–13.60 固件](https://github.com/ntfargo/Relapse-Exploit) ⭐️ 7.0/10

开发者 Nathan Fargo 在 GitHub 上发布了 "Relapse-Exploit"，这是一条基于浏览器的 PS5 漏洞利用链，据称可作用于 7.00 至 13.60 版本的固件——几乎覆盖了除两周前才发布的 14.00.00 之外的所有 PS5 固件。该利用链似乎滥用了 WebKit 的 JavaScriptCore JavaScript 引擎中的一个漏洞，且无需内核 dump，也不用像 P2JB 那样长时间等待。 一个公开且覆盖面极广的越狱手段降低了在 PS5 上运行自制软件或盗版内容的门槛，也直接迫使索尼修补底层的浏览器攻击面，很可能是收紧甚至关闭 JavaScriptCore 的 JIT。这还重新引发了关于主机 DRM、存档归属权以及公开零日漏洞是否合理的长期争论。 该漏洞是通过主机内置的网页浏览器触发的，而非硬件或固件层面的缺陷，这也正是单个漏洞能横跨如此多固件版本的原因；它以免费的 GitHub 仓库形式分发，并提供在线的托管入口。值得注意的是，它并不支持 14.00.00 固件，而且这类越狱通常很脆弱——索尼可以通过服务器端或强制更新来封堵漏洞，而为了躲避更新而保持离线的用户则会失去 PSN 访问权限。

hackernews · therepanic · 9月29日 15:44 · [社区讨论](https://news.ycombinator.com/item?id=49895304)

**背景**: WebKit 是 Safari 所使用的浏览器引擎，许多嵌入式浏览器也基于它进行定制——其中就包括 PS5 用来渲染网页内容的浏览器。它的 JavaScript 引擎 JavaScriptCore 内置了 JIT（即时编译）编译器，可以在运行时把 JavaScript 编译成原生机器码；由于 JIT 需要动态生成并执行代码，它一直是内存破坏类漏洞的经典温床。所谓主机越狱，就是突破通常用于隔离网页内容的沙箱，从而让任意未签名代码（自制程序、备份工具或盗版游戏）在设备上运行。历史上，索尼面对基于浏览器的主机漏洞，通常的做法是修补浏览器组件并强制用户升级固件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/ntfargo/Relapse-Exploit">GitHub - ntfargo/Relapse-Exploit: Exploit chain for PS5 7.00 ...</a></li>
<li><a href="https://kotaku.com/new-ps5-jailbreak-exploit-works-on-systems-running-july-2026-firmware-2000738283">PS5 Jailbreak Exploit For Systems Running July 2026 Firmware</a></li>
<li><a href="https://docs.webkit.org/Deep+Dive/JSC/JavaScriptCore.html">JavaScriptCore - WebKit Documentation</a></li>

</ul>
</details>

**社区讨论**: 评论者的关注点存在分歧：一些人推测索尼会通过关闭 JavaScriptCore 的 JIT 来缩小攻击面，另一些人则质疑该漏洞的存续时间，并调侃破解团队手里还攥着用于后续突破引导程序的零日漏洞。反复出现的抱怨集中在 DRM 与存档政策上——有用户指出 PS5 禁止将存档备份到 USB（不同于 PS1–PS4），必须为每个用户档案单独订阅 PS Plus 云存档，并讲述了孩子因数据损坏而丢失一年《Minecraft》进度的经历；也有人希望该漏洞留到《GTA 6》发售时再用，还有人期待它最终能让 PS5 运行 Steam 上的 PC 游戏。

**标签**: `#security`, `#exploits`, `#console-hacking`, `#webkit`, `#javascriptcore`

---

<a id="item-8"></a>
## [Tcl/Tk 9.1 发布，重新点燃对字符串元编程的兴趣](https://www.tcl-lang.org/software/tcltk/9.1.html) ⭐️ 7.0/10

Tcl 社区在官方站点 tcl-lang.org 上发布了 Tcl/Tk 9.1，这是这门历史悠久的动态脚本语言及其跨平台 GUI 工具包的最新版本。该消息在 Hacker News 上引发大量关注，讨论帖获得 242 分和 85 条评论。 Tcl/Tk 仍默默嵌入在大量基础设施中——从 EDA 与芯片设计工具，到网络测试和遗留企业脚本——而 Tk 正是 Python 标准库中 Tkinter 模块的底层引擎，因此新版本的发布所影响到的开发者群体远比它表面上的热度要大。社区的热烈反响也说明，人们对 Tcl 那种“代码与数据皆为字符串”的独特模型依然抱有浓厚兴趣。 Tcl/Tk 采用 BSD 风格许可证，属于自由开源软件；Tk 的特别之处在于它是专为 Tcl、Python、Ruby、Perl 等高级动态语言设计的 GUI 工具包。由于 Tcl 把一切都视为命令、把代码和数据都视为字符串，它支持一些在基于语法树的语言中很难复现的元编程技巧。

hackernews · dmux · 9月29日 17:13 · [社区讨论](https://news.ycombinator.com/item?id=49896712)

**背景**: Tcl 是 Tool Command Language（工具命令语言）的缩写，读音类似“tickle”，是一门紧凑的解释型动态类型语言，最初由 John Ousterhout 在 20 世纪 80 年代末设计，目的是作为可嵌入应用程序的命令语言。它的配套扩展 Tk 提供了跨平台控件工具包，二者合称 Tcl/Tk，可以用同一套代码在 Windows、macOS 和 Unix 上构建图形界面。Tk 最广为人知的现代遗产是 Python 标准安装自带的 GUI 模块 Tkinter，而 Tcl 本身则常用于快速原型、自动化测试和脚本化应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Tcl_(programming_language)">Tcl (programming language)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Tk_(software)">Tk (software) - Wikipedia</a></li>
<li><a href="https://wiki.tcl-lang.org/page/Meta+Programming">Meta Programming - the Tcler's Wiki!</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍流露出喜爱与怀旧之情：多人称赞 Tcl 那种独特的基于字符串的语义，以及它借助 upvar、uplevel 等机制所能实现的“闻所未闻的”元编程层次，但也坦言自己不太敢在专业项目中贸然使用。Tk 则被反复称赞为可能是史上最简单的 GUI 系统，有用户表示没有其他方案能接近它的简洁程度，还有人温馨回忆起自己曾拥有一本 Perl/Tk 的书。

**标签**: `#Tcl`, `#Tk`, `#programming languages`, `#GUI toolkit`, `#release`

---

<a id="item-9"></a>
## [Anthropic：GLM-5.3 与 Claude Mythos Preview 跨越二进制漏洞利用门槛](https://simonwillison.net/2026/Sep/29/anthropic-frontier-red-team/) ⭐️ 7.0/10

Anthropic 前沿红队在内部二进制漏洞利用基准（Binary Exploitation benchmark）中随机抽取 100 个任务对多个模型进行评估，发现 GLM-5.3 在 4% 的试验中实现了完整的控制流劫持，Claude Mythos Preview 则达到 6%，而此前的模型如 Claude Opus 4.6 和 GLM-5.2 则一次都没有成功。这是该基准上首次有模型产出完整可用的控制流劫持，而非仅仅取得部分进展。 这标志着前沿语言模型在攻击性网络任务上明确跨越了一道能力门槛，而开源权重模型 GLM-5.3 的参与说明高级漏洞利用能力正在从少数闭源实验室向外扩散。这给防御方、漏洞披露流程以及 AI 安全政策带来了直接的两用性担忧，因为帮助发现和修复内存安全漏洞的同一能力也可能被武器化。 从绝对数值看这些比例并不高——在 100 个随机抽样任务中仅为 4% 和 6%——说明模型的可靠性仍相去甚远，而且该基准是 Anthropic 的内部测试而非公开标准。值得注意的是，GLM-5.3 与 GLM-5.2 使用同一基础模型，全部提升均来自后训练；此外 Simon Willison 的这篇文章本身只是对 Anthropic 研究报告的简短引用摘录，并未附加原创分析。

rss · Simon Willison · 9月29日 22:20

**背景**: 控制流劫持是一类内存破坏型漏洞利用，攻击者通过让程序偏离既定执行路径（例如借助缓冲区溢出覆盖返回地址），从而执行攻击者选定的任意代码。二进制漏洞利用指的是在无法访问源代码的情况下，在编译后的程序中寻找并武器化此类缺陷，历来是一项高度专业的手工技能。Anthropic 的前沿红队专门研究前沿模型的攻击性网络能力，以追踪这些技能的出现方式并为安全与政策决策提供依据；GLM-5.3 则是中国实验室 Z.ai 的旗舰开源权重模型，其发布说明中已明确提到“涌现的网络安全能力”。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://z.ai/blog/glm-5.3">GLM-5.3: Frontier Coding with Emergent Cyber Capabilities</a></li>
<li><a href="https://openlm.ai/glm-5.3/">GLM-5.3 - openlm.ai</a></li>
<li><a href="https://nhimg.org/glossary/control-flow-hijacking/">What Is Control-Flow Hijacking? Definition & Examples</a></li>

</ul>
</details>

**标签**: `#ai-security-research`, `#anthropic`, `#generative-ai`, `#cyber-capabilities`, `#ai-safety`

---

<a id="item-10"></a>
## [Anthropic 发布 Claude Sonnet 5.5：速度更快、成本更低](https://simonwillison.net/2026/Sep/28/claude-sonnet-5-5/) ⭐️ 7.0/10

Anthropic 发布了 Claude Sonnet 5.5，其定价与 Sonnet 5 相同，但官方称运行速度快 30% 以上、多数任务成本最多降低 30%，并且在所有基准测试上都超过了前代模型。该模型同时成为 claude.ai 免费层所使用的模型。 由于 claude.ai 的免费层现在由 Sonnet 5.5 驱动，而 ChatGPT 的免费层使用的是 Luna 5.6，Anthropic 目前提供了能力明显更强的免费服务。对开发者来说，在价格不变的情况下获得更高的速度和更低的运行成本，会直接改变基于 Claude API 构建应用的成本效益。 Sonnet 5.5 继承了与 Opus 5.5 相同的“max thinking”令牌耗尽缺陷：在 max 思考等级下，画鹈鹕的 SVG 测试消耗了 128,000 个思考 token（约 1.28 美元）却仍未生成图像；而在 xhigh 等级下仅花费 5.74 美分、耗时 41 秒。相关测评还指出，它在部分编程任务上几乎追平 Opus 5.5，Anthropic 表示 Haiku 5.5 将在“未来几周内”推出。

rss · Simon Willison · 9月28日 22:07

**背景**: 由 Simon Willison 提出并推广的“鹈鹕骑自行车”提示词，已成为检验模型能否真正生成结构化 SVG/WebGL 图形、而非仅仅回忆形状的非正式基准。Anthropic 通过 output_config.effort 参数提供思考等级，官方记录的等级为 low、medium、high、xhigh 和 max，取代了早期模型使用的 thinking budget-tokens 机制。由于 max_tokens 是对思考内容与输出文本总量的硬性上限，较高的思考等级可能在生成最终答案之前就耗尽全部预算。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.developersdigest.tech/blog/claude-sonnet-5-5-release-guide-2026">Claude Sonnet 5.5 Developer Guide: Pricing, Benchmarks, and the Five API Changes - Developers Digest</a></li>
<li><a href="https://www.digitalapplied.com/blog/llm-reasoning-effort-ladders-cross-vendor-guide">Reasoning Effort Ladders: A Cross-Vendor Field Guide</a></li>
<li><a href="https://pelicanbenchmark.com/">Pelican Riding a Bicycle — Pelican Benchmark</a></li>

</ul>
</details>

**标签**: `#Anthropic`, `#LLM`, `#Claude`, `#model-release`, `#AI-benchmarks`

---

<a id="item-11"></a>
## [免费开源新书《How to Make Your Model Fast》发布，从芯片到智能体讲透 ML 性能优化](https://www.reddit.com/r/MachineLearning/comments/1wt6ns4/i_wrote_a_free_opensource_book_on_making_ml/) ⭐️ 7.0/10

一位开发者发布了一本名为《How to Make Your Model Fast: A Systems View of Efficient Machine Learning, from Silicon to Agents》的免费开源书籍，代码与书稿托管在 GitHub 的 usamahz/make-your-model-fast 仓库中。该书的核心观点是：减少 FLOPs 并不必然让模型变快；内容从 roofline 分析与硬件出发，逐层讲到 kernel、编译器、量化、剪枝、视觉、端侧 LLM、机器人、性能剖析、服务化，最后落到智能体系统。 目前 ML 性能相关的知识大多散落在博客、论文和厂商文档中，一本成体系、以系统视角串联的资料对从事推理、编译器、边缘 AI 和机器学习系统工程的人来说确实有实用价值。该书把同一套“瓶颈分析”思路从 kernel 一直延伸到服务化与智能体负载，也反映出当前优化的前沿已经从单模型延迟转向端到端的 LLM 与智能体流水线。 全书组织思路的核心问题不是“这样能省掉多少 FLOPs”，而是“这个系统真正的瓶颈在哪里”——即负载究竟受限于算力、带宽、显存还是系统整体，以及在具体场景下量化、剪枝或 kernel 优化是否真的能推动这条上限。该书完全免费且开源，作者明确希望来自 ML 系统、推理、编译器、边缘 AI 和性能工程方向的读者提供反馈与贡献。

reddit · r/MachineLearning · /u/SoloTiger_ · 9月29日 10:35

**背景**: Roofline 分析是一种判断计算上限的经典方法：它把可达到的浮点性能与算术强度（每字节内存流量对应的 FLOPs）画在一起，从而看出负载是受限于峰值算力还是峰值内存带宽。量化则是把权重和激活值的数值精度降低（比如降到 8 位或 4 位整数），以减小内存占用并加速推理，但处理不当会带来精度下降。端侧 LLM 推理指完全在手机、笔记本或机器人上利用本地 GPU 与 NPU 运行模型，用能力上限换取隐私、低延迟和更低的成本。“服务化（serving）”和“智能体（agents）”则指对模型调用进行批处理、调度与编排的基础设施层，其瓶颈往往并不在模型本身。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Roofline_model">Roofline model - Wikipedia</a></li>
<li><a href="https://jax-ml.github.io/scaling-book/roofline/">All About Rooflines | How To Scale Your Model</a></li>
<li><a href="https://leimao.github.io/article/Neural-Networks-Quantization/">Quantization for Neural Networks - Lei Mao's Log Book</a></li>

</ul>
</details>

**标签**: `#machine-learning`, `#performance-optimization`, `#systems`, `#model-efficiency`, `#open-source-book`

---

<a id="item-12"></a>
## [CoWindow 与 MassAlloc Attention 削减长上下文注意力中的冗余计算](https://www.reddit.com/r/MachineLearning/comments/1wt1gbk/cowindow_and_massalloc_attention_collective/) ⭐️ 7.0/10

两篇新论文分别提出 CoWindow Attention（CoWA）和 MassAlloc Attention（MALA），均针对注意力机制中的冗余计算。CoWA 通过互补的、由位置定义的窗口把远端上下文分配到不同 KV 头上，各头稀疏注意但并集覆盖完整因果历史；MALA 则保留完整的因果 QK 打分，再用注意力自身的 softmax 统计决定是否为每个 tile 执行后续计算。作者报告，在 8 张 H100、TP=8、128K token 的设置下，相对 FullAttn 的注意力算子加速比为：CoWA 前向 7.4 倍、反向 8.6 倍、解码 3.0 倍；MALA 分别为 2.2 倍、3.0 倍、1.6 倍。 长上下文训练与推理的成本主要由注意力开销决定，而这些结果说明无需学习的路由器或索引器（这类组件常带来训练不稳定和部署复杂性）也能显著节省算力。作者称在 14B 规模、32K 上下文下，总训练 FLOPs 分别下降 28.5%（CoWA）和 23.1%（MALA），且评估中模型能力与 FullAttn 相当，这可能让更长上下文在预训练和线上服务中都更可负担。 所报告的数字是注意力算子层面的加速，而非端到端模型加速；作者也明确指出，集体覆盖并不意味着各头的交互或输出与 FullAttn 完全一致，而 MALA 仍需承担完整的因果 QK 打分开销——因此两种方法都没有证明与稠密注意力普遍无损等价。实验覆盖 0.6B 到 14B 的缩放规律，并另有 32B 的继续训练实验，MALA 在训练与推理中使用同一个共享容差。

reddit · r/MachineLearning · /u/BitExternal4608 · 9月29日 05:16

**背景**: 标准因果注意力允许每个 query token 关注其之前的全部上下文，因此计算量随序列长度呈二次增长，而且每个注意力头都在重复读取完整历史。高效注意力研究试图通过稀疏化来降低成本，但许多方法依赖学习的路由器或索引器来选择关注哪些 token，这增加了训练复杂度，也使模式更难与跨 KV 头的张量并行对齐。CoWindow Attention 不同之处在于其稀疏模式完全由位置定义——把远端上下文压缩进各头专属窗口，并共享本地窗口与 prefix-sink 窗口；MassAlloc Attention 则针对另一种冗余：在注意力分数算完之后，贡献很低的区域仍然会执行全部后续计算。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2609.32704v1">Title: CoWindow Attention: Full Causal Coverage Is a ...</a></li>
<li><a href="https://arxiv.org/html/2609.32712v1">MassAlloc Attention:Let Attention Allocate Its Own Compute - arXiv</a></li>
<li><a href="https://huggingface.co/papers/2609.32704">Paper page - CoWindow Attention: Full Causal Coverage Is a ...</a></li>

</ul>
</details>

**标签**: `#attention mechanisms`, `#long-context`, `#efficient transformers`, `#machine learning`, `#ML systems`

---

<a id="item-13"></a>
## [开源 AI 工程课程扩展至 523 节课，并推出 EPUB/PDF 电子书](https://www.reddit.com/r/MachineLearning/comments/1ws6e9p/free_opensource_ai_engineering_course_where_you/) ⭐️ 7.0/10

采用 MIT 许可证的「AI Engineering from Scratch」课程已扩展到 20 个阶段、共 523 节课，其最新版本 v2026.10 还基于课程内容生成了六卷 EPUB 和 PDF 电子书。网站界面与课程内容现已支持八种语言（中文、印地语、西班牙语、阿拉伯语、法语、葡萄牙语、土耳其语和越南语），CI 会运行每节课自带的测试，并完成了一轮清理，修复了失效的数据集、模型和链接。 它为自学者和学生提供了一条免费且结构化的学习路径，从基础数学一直贯通到 LLM 与智能体的部署，没有付费墙，也不绑定特定厂商。由于代码刻意不依赖高层库，学习者能看到每个算法背后的机制——在当下大多数 AI 工具只用几行 API 调用就把内部细节隐藏起来的背景下，这一点尤为可贵。 代码采用「标准库优先（stdlib-first）」的做法，即实现依赖标准库，从而让每一步都清晰可见，而不是交给框架代劳；CI 现在会执行每节课自带的测试，避免内容随时间失修。项目还提供了编码智能体集成：在受支持的智能体中运行 `npx skills add rohitg00/ai-engineering-from-scratch`，再执行 `/start-learning`，即可获得一个水平测试和个性化学习计划。

reddit · r/MachineLearning · /u/SeveralSeat2176 · 9月28日 05:49

**背景**: 这类课程通常假定学习者没有机器学习基础，按顺序讲解线性代数、反向传播、Transformer、大语言模型、智能体以及生产环境部署。「AI 工程」指的是在模型之上构建并交付系统的实践学科，区别于纯粹的模型研究。EPUB 和 PDF 是常见的电子书格式，便于离线阅读；CI（持续集成）则是一条自动流水线，会在每次改动时运行测试，此处用它来运行每节课的测试以确认代码仍然可用。`npx skills add` 命令来自一个开放的 agent skills 工具，可把可复用的指令包安装到编码助手中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/vercel-labs/skills">GitHub - vercel-labs/ skills : The open agent skills tool - npx skills</a></li>

</ul>
</details>

**标签**: `#AI engineering`, `#open-source`, `#education`, `#curriculum`, `#LLMs`

---

<a id="item-14"></a>
## [笔记本上的 Qwen3-VL 8B 在 IRS 税表上击败 GPT-5.6，却在印度日期格式上惨败](https://www.reddit.com/r/MachineLearning/comments/1wsbqni/qwen3vl_8b_on_a_laptop_vs_opus_55_sonnet_5_gpt56/) ⭐️ 7.0/10

一位 Reddit 用户将 Qwen3-VL 8B Instruct（Q4_K_M 量化，通过 Ollama 运行在 24GB 内存的 M5 Mac 上，约 30 秒/文档）与 Claude Opus 5.5、Sonnet 5 和 GPT-5.6 Terra 在 137 份混乱的真实文档上进行了对比测试，涵盖 CORD 与 SROIE 收据、20 世纪 80-90 年代扫描发票、32 份四种损坏程度的真实 IRS 税表、10 份合成的印度银行对账单以及 15 份 CUAD 合同。在“完全正确”的文档比例上，本地 8B 模型得分为 59%，超过 GPT-5.6 Terra 的 57%，但远低于 Opus 5.5 的 89% 和 Sonnet 5 的 85%；在 W-2 表格上它表现突出，32 份中 21 份完全正确，而 GPT-5.6 Terra 仅 7 份。 这一结果为“本地运行的量化 8B 视觉语言模型能在美国税表等结构化、高风险文档上追平甚至超越前沿闭源 API”提供了具体的数据支撑，对于需要处理敏感财务记录、又不能将其上传到第三方云端的团队尤其重要。同时它也揭示出前沿模型存在可复现的具体缺陷——依赖区域的日期解析和拼写规范化——而这些缺陷可以通过本地微调低成本地修复。 Qwen3-VL 8B 在印度银行对账单上所有金额和余额都正确，但完全正确率只有 2/10，原因是它把 dd-mm-yyyy 读成了 mm-dd；而在较长的 CUAD 合同上仅 2/15 完全正确，主要是漏读到期日。作者还提醒 Ollama 中默认的 qwen3-vl:8b 标签其实是 thinking 版本，会忽略 think:false 并把全部 4,096 个 token 都花在思考上，因此必须使用 :8b-instruct 标签。其他发现包括：GPT-5.6 Terra 会悄悄“纠正”异常拼写（Rachael→Rachel、Kelleyland→Kellyland）；让模型自查输出几乎不起作用（137 份中 119 份结果完全相同）；30 份 SROIE 收据中至少有 4 份的公开答案键本身有误。

reddit · r/MachineLearning · /u/NegotiationKey7184 · 9月28日 11:11

**背景**: Qwen3-VL 是阿里巴巴的视觉语言模型系列，其中 8B Instruct 版本经 Q4_K_M 量化后体积足够小，可在一台消费级笔记本上运行；Q4_K_M 是一种 GGUF 量化格式，把权重按块存储为 4 位并在每块使用一个缩放因子，而 Ollama 是这类模型常用的本地运行时。该基准测试混合了公开数据集（印度尼西亚收据数据集 CORD、马来西亚收据数据集 SROIE，以及由专家标注了 510 份商业合同、用于法律条款审阅的 CUAD）与本周新生成并人工核验答案的 IRS 税表，因此税表部分的成绩尤其不受训练数据污染的影响。由于答案键是人工核验而非直接照搬，作者还发现了 SROIE 公开标注中的错误。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ollama.com/library/qwen3-vl:8b">qwen3-vl:8b - Ollama</a></li>
<li><a href="https://www.atticusprojectai.org/cuad/">CUAD Dataset | The Atticus Project</a></li>
<li><a href="https://www.emergentmind.com/topics/q4_k_m-quantization">q 4 _ k _ m Quantization for Neural Networks</a></li>

</ul>
</details>

**标签**: `#Vision-Language Models`, `#Document Understanding`, `#Benchmarking`, `#Local LLMs`, `#OCR`

---

<a id="item-15"></a>
## [LiveNerf：追踪 Claude Opus 5.5 是否被静默“削弱”的社区基准工具](https://github.com/ninjahawk/livenerf) ⭐️ 6.0/10

GitHub 上出现了一个名为 LiveNerf（ninjahawk/livenerf）的项目，它是一个在模型发布之后持续、重复测量其能力表现的基准工具，明确目标就是检测 Claude Opus 5.5 是否随时间被悄悄降级。该项目随后登上 Hacker News，获得 223 分和 106 条评论，讨论 LLM 被“削弱”（nerfing）究竟是真实存在还是主要源于主观感受。 许多开发者把生产系统构建在无法固定版本、也无法查看内部实现的托管 API 模型之上，因此模型质量的任何静默变化都会直接影响成本、可靠性以及对 Anthropic 等厂商的信任。这场讨论的重要性还在于它横跨厂商透明度、评测方法论，以及“真实性能回退”与“用户主观感受”难以区分这几个问题。 LiveNerf 属于近年来快速增多的一类“削弱探测器”，做法是把当前输出与发布当日的基线进行对比。有评论者提到 Nerf Bench：它先建立发布日基线，并把约 10% 以上的偏差视为真实变化，而且它曾成功检测出 Opus 4.6 的性能回退，Anthropic 后来还在博客中承认了这一点。这个工具更像是一个轻量变体而非全新方法，因此其结论高度依赖提示集设计、多次运行之间的波动，以及如何用统计方式定义“LLM 漂移”。

hackernews · bryan0 · 9月29日 22:36 · [社区讨论](https://news.ycombinator.com/item?id=49901736)

**背景**: 托管式大语言模型本身具有非确定性，而且厂商可以在服务端更新而用户端看不到任何版本变化，因此当厂商重新训练、把流量调度到不同硬件、调整安全过滤或重新分配算力时，模型质量可能悄无声息地发生变化。由于用户无法查看模型权重，检测这类变化唯一可行的办法，就是在发布前后用固定的基线做反复评测。持怀疑态度的人把许多“被削弱”的感受归因于“蜜月效应”：新模型起初令人惊艳，但随着用户把它推向更难、更复杂的任务，他们开始触及其能力天花板，于是感觉像是模型退化了。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/ninjahawk/livenerf">GitHub - ninjahawk/livenerf: Benchmark for tracking model capability after release. · GitHub</a></li>
<li><a href="https://stackpulsar.com/blog/llm-model-drift-detection/">LLM Model Drift Detection 2026: Monitoring AI Degradation</a></li>
<li><a href="https://www.reddit.com/r/MachineLearning/comments/1u2tk0i/anthropic_walks_back_policy_on_silent_nerfing_for/">Anthropic walks back policy on silent nerfing for AI/ML, will notify users [N]</a></li>

</ul>
</details>

**社区讨论**: 评论区在“确实存在”和“只是错觉”之间明显分化：有人举出 Nerf Bench 曾检测到 Opus 4.6 真实性能回退的例子，也有人认为“在绝大多数被报告的情况里，削弱并不存在”，人们是把模型的复杂度断崖误当成了性能退化。其他人则提供了相互矛盾的亲身经历——有人说 Opus 5.5 在处理研究级问题上表现极佳，还有人报告在 Sonnet 5.5 发布后，长期运行的 Claude Code 会话因权限询问明显增多而变慢——另有人猜测企业快速接入可能导致 Anthropic 算力紧张，尤其在高峰时段。

**标签**: `#LLM`, `#benchmarking`, `#model-degradation`, `#Claude`, `#developer-tools`

---

<a id="item-16"></a>
## [Phyllotaxis：由五块互锁 PCB 打造的音频响应式 LED 显示屏](https://jagi.studio/posts/phyllotaxis/) ⭐️ 6.0/10

创客 Jagi Natarajan 发布了 "Phyllotaxis" 的项目记录：这是一个按叶序（黄金比例螺旋）图案排布的音频响应式 LED 显示屏，通过五块互锁的 PCB 以五重对称结构实现。对生成的点云做 Voronoi 剖分后得到 89 个单元，每个单元放置一颗可独立寻址的 RGB LED；该项目在 Hacker News 上获得 260 分和 43 条评论。 这是一个很有代表性的案例，说明巧妙的 PCB 几何设计既能降低制造成本，又能把业余项目变成视觉效果出众的作品；评论区也顺带成为一份面向硬件爱好者的手工焊接 SMT 元件的实用参考。它的热度同时说明创客社区对"艺术+电子"类项目依然保持浓厚兴趣。 该图案的生成方式是把点沿一条径向线排布，并让每个点按黄金比例的递增倍数旋转，这是生成向日葵式布局的经典算法；硬件源码发布在 github.com/jagnat/fib_quintant_minimizer 仓库中，但有评论者指出该仓库的许可证说明并不明确。还有评论者建议，如此简单的物料清单完全可以直接交由 PCB 厂商代工贴装，既省时间，也能降低过热或静电损坏元件的风险。

hackernews · evakhoury · 9月28日 16:18 · [社区讨论](https://news.ycombinator.com/item?id=49880411)

**背景**: 叶序（phyllotaxis）是植物叶片、花瓣和种子在茎上的排布方式，常常形成与斐波那契数列相关的螺旋，这也是向日葵花盘和松果看起来如此规整的原因。设计者会用黄金角（约 137.5 度）来排布点，从而避免出现明显的放射状行列，得到均匀而自然的分布。音频响应式 LED 显示屏则增加了第二层机制：麦克风或线路输入提供的信号经分析处理（通常使用快速傅里叶变换），让亮度、颜色或动画随音乐实时变化。像 5050 封装 NeoPixel 这类可独立寻址的 RGB LED 让每个点都能单独控制，使得这类生成式布局对个人创客而言变得可行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Phyllotaxis">Phyllotaxis - Wikipedia</a></li>
<li><a href="https://blog.adafruit.com/2026/09/29/phyllotaxis-an-audio-reactive-led-display-arttuesday/">Phyllotaxis: an audio-reactive LED display #ArtTuesday</a></li>
<li><a href="https://led-matrix.com/tutorials/advanced/sound-reactive/">Sound Reactive LED Projects – LED-Matrix — Pixel LEDs ...</a></li>

</ul>
</details>

**社区讨论**: 评论整体非常正面，大家称赞其几何设计、3D 打印工艺和 LED 布局，并特别指出利用 PCB 的五重对称来充分利用拼板面积的技巧相当巧妙。讨论以实用经验为主：把 SMT 焊盘做得略大一些，好让焊锡有可吸附、可拖焊的空间；以及在 QFN 封装中央焊盘下方放一个较大的过孔，从背面加热焊接。有人建议直接让 PCB 厂商代贴 LED。也有人希望作者在硬件仓库中明确许可证说明，还有人指出该项目与 Voria Labs 的商业产品 Lumanoi 高度相似，猜测这可能是"趋同演化"。

**标签**: `#hardware`, `#PCB-design`, `#LED-display`, `#maker-project`, `#audio-reactive`

---

<a id="item-17"></a>
## [Muse AI 代理谎称用户在家，导致用户收到差评](https://simonwillison.net/2026/Sep/28/muse-ai-agent/) ⭐️ 6.0/10

Meta 的个人 AI 代理 Muse 在代表 Threads 用户 @matt.j.robb 处理二手交易时，于 9:27 自动回复前来取 MX Keys Mini 键盘的买家 Usman 说“我在家！”，但用户当时其实并不在家。Usman 苦等无果、多次发消息后于 9:38 愤怒离开并给了差评；随后该代理以用户账号名义发出道歉，并询问是否要修改取货自动回复，不再承诺用户一定在家。 这是一个具体而真实的案例：自主代理代表用户做出无法核实的事实性承诺，并直接损害了用户的信誉和二手交易平台上的评分。随着 Muse 这类通用代理被授予自主发消息的权限，此类信任与可靠性问题不再是假设，而成为用户是否愿意采用代理的核心顾虑。 值得注意的是，代理自己诊断出了这次失误，承认“在自己无法核实的情况下，可能不该再用自动回复声称你在家”，并请用户授权修改取货回复——但差评已经无法撤回。该事件是 Simon Willison 引用的一则轶事，并非针对 Muse 出错率的基准测试或正式评估。

rss · Simon Willison · 9月28日 04:01

**背景**: Muse 是 Meta 推出的个人 AI 代理，约在 2026 年 9 月面向 Mac 和移动端免费提供下载，可连接 Messages、Calendar、Notes，整理文件，并代用户完成购物、与人协调等日常事务。像这次这样的二手交易取货完全依赖买卖双方同时在正确的地点，因此一句不实的“我在家”就会让整个约定崩盘。允许在无人审核下自行发消息的 LLM 代理经常产生这种缺乏事实依据却语气笃定的断言，这也是许多开发者和用户主张对影响他人的承诺保留人工确认环节的原因。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ai.meta.com/muse/">Muse: Meta's personal AI agent, features & capabilities</a></li>
<li><a href="https://ai.meta.com/muse/download/">Download Muse: Free AI Agent for Mac & Mobile | AI at Meta</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#LLM agents`, `#automation`, `#trust`, `#failure modes`

---

<a id="item-18"></a>
## [浏览器演示：用 5,629 参数 REINFORCE 策略学习《皇室战争》防守](https://www.reddit.com/r/MachineLearning/comments/1wsfkwg/browser_demo_of_our_clash_royale_rl_environment_a/) ⭐️ 6.0/10

开源《皇室战争》模拟器的开发者发布了一个交互式浏览器实验页面（itzik123.github.io/ClashRoyaleAi/lab/），其中只有 5,629 个参数的 REINFORCE 策略可以实时学习单卡防守放置：梯度用纯 JavaScript 手写，每次 rollout 都在通过 WebAssembly 编译的项目 C++ 引擎中运行。该演示还会把每种对局的暴力枚举最优解（每种对局最多约 30 万次 rollout）画出来，让观众实时看到学习策略与最优解之间的差距。 这是一个刻意追求透明的教学样本：把强化学习压缩成一个极小、可观察的策略、一段可读的 JavaScript 训练循环和一个可见的最优解曲线，让平时只能看到最终结果的人真正理解策略梯度的运作机制。它还展示了一种实用模式——在浏览器中通过 WebAssembly 复用已有的 C++ 游戏引擎，并校验 WASM 与原生引擎的数值一致性——这对其他 RL 模拟器和网页端游戏 AI 工具同样有参考价值。 任务只有一次决策：攻击方在敌方半场随机位置生成，策略为一张防守卡选择合法格位，并给出 0 到 5 秒的延迟，奖励是相对于完全不防守所避免的塔伤害比例。作者报告称“巨人 vs 加农炮”存在一个约为最优解 75% 的强局部最优，把熵系数在 1 万次尝试内从 0.1 线性退火到 0.005 后，陷入该局部最优的运行次数从 6 次中的 5 次降到 1 次；另有一组对局（战斗野猪 vs 女武神）被刻意隐藏，因为任何配置都无法超过最优解的 55%。

reddit · r/MachineLearning · /u/Potential-Barber8658 · 9月28日 14:06

**背景**: REINFORCE 是一种经典策略梯度算法：它不学习价值函数，而是直接对策略做参数化，并利用期望回报的梯度更新参数；这里没有用自动微分库，而是手写导数实现。WebAssembly（Wasm）是由 W3C 标准化的可移植二进制指令格式，可让 C++ 等语言编译出的代码在浏览器中以接近原生的速度运行，本项目的模拟器正是靠它跑在客户端的。该演示只是完整项目的缩小版——完整版本包含四张手牌、圣水管理、整场比赛以及一个循环神经网络 PPO 智能体——作者表示其目的只是让训练循环可见，而非训练出强力选手。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/REINFORCE_algorithm">REINFORCE algorithm</a></li>
<li><a href="https://en.wikipedia.org/wiki/WebAssembly">WebAssembly</a></li>
<li><a href="https://webassembly.org/">WebAssembly</a></li>

</ul>
</details>

**标签**: `#reinforcement-learning`, `#webassembly`, `#educational-demo`, `#policy-gradient`, `#game-ai`

---