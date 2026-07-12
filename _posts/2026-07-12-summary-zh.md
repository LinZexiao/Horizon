---
layout: default
title: "Horizon Summary: 2026-07-12 (ZH)"
date: 2026-07-12
lang: zh
---

> 从 28 条内容中筛选出 9 条重要资讯。

---

1. [Claude Code 每次提示消耗 3.3 万 tokens，OpenCode 仅 7 千](#item-1) ⭐️ 8.0/10
2. [爱尔兰数据中心消耗全国 23%的电力](#item-2) ⭐️ 8.0/10
3. [陶哲轩利用 LLM 编码代理创建可视化工具](#item-3) ⭐️ 8.0/10
4. [热爱 LLM，拒绝炒作](#item-4) ⭐️ 8.0/10
5. [Chromium 148 的 Math.tanh 允许操作系统指纹识别](#item-5) ⭐️ 7.0/10
6. [Anthropic 因计算限制延长 Claude Fable 5 可用时间](#item-6) ⭐️ 6.0/10
7. [Zer0Fit：将 Google TabFM 和 TimesFM 封装为 MCP 服务器](#item-7) ⭐️ 6.0/10
8. [基于上下文的神经网络线性映射观点](#item-8) ⭐️ 6.0/10
9. [ACL 会议接收流程：ARR 审稿机制解析](#item-9) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Claude Code 每次提示消耗 3.3 万 tokens，OpenCode 仅 7 千](https://systima.ai/blog/claude-code-vs-opencode-token-overhead) ⭐️ 8.0/10

一项实证对比发现，Claude Code 在读取用户提示之前就已发送约 3.3 万 tokens，而 OpenCode 仅发送约 7 千 tokens——由于低效的缓存策略和框架代币使用，前者开销约为后者的 4.7 倍。 这种代币低效会显著增加使用 Claude Code 的开发者的成本，尤其是对于大型或频繁的任务，并引发对 Anthropic 设计动机的质疑。这些发现对实践者在选择编程智能体工具和优化 LLM 使用方面具有实际指导意义。 该研究记录了每个工具与 Anthropic 端点之间的所有请求，测量了处理首个用户提示之前的 token 数量。作者指出，Claude Code 的开销并非来自提示本身，而是源于其缓存策略和框架代币使用方式。

hackernews · systima · 7月12日 18:25 · [社区讨论](https://news.ycombinator.com/item?id=48883275)

**背景**: 像 Claude Code 和 OpenCode 这样的编程智能体工具利用大语言模型自主编辑代码、运行命令并与代码库交互。它们依赖系统提示和框架逻辑，在处理任何用户输入之前就会消耗 tokens。代币效率直接影响成本和速度，因此成为开发者的关键指标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://opencode.ai/docs/models/">Models | OpenCode</a></li>

</ul>
</details>

**社区讨论**: 社区评论指出 Claude Code 中的子智能体会快速消耗预算，有用户提到单个任务竟启动 7 个子智能体。有人猜测 Anthropic 可能有财务动机来增加 token 使用量，而另一些人指出提示精简和工具质量比原始 token 数量更重要。

**标签**: `#agentic coding`, `#token efficiency`, `#Claude Code`, `#OpenCode`, `#LLM tooling`

---

<a id="item-2"></a>
## [爱尔兰数据中心消耗全国 23%的电力](https://www.theregister.com/on-prem/2026/07/11/irish-datacenters-now-guzzle-23-of-the-countrys-electricity/5270013) ⭐️ 8.0/10

据最新报道，爱尔兰数据中心目前已占该国总电力消耗的 23%，凸显出科技行业能源需求的急剧增长。 这一高占比引发了对家庭和企业能源成本的担忧，也对爱尔兰在支持数字基础设施增长的同时实现可再生能源目标的能力提出了挑战。 23%这一数字较往年显著增长，同时伴随电价上涨，居民电价已升至约每千瓦时 35 欧分。

hackernews · Bender · 7月12日 20:16 · [社区讨论](https://news.ycombinator.com/item?id=48884322)

**背景**: 数据中心对于云计算、流媒体和人工智能工作负载至关重要，但服务器和冷却系统消耗大量电力。由于优惠的企业税率和熟练的劳动力，爱尔兰已成为大型科技公司的枢纽，导致数据中心在该岛快速集中。

**社区讨论**: 评论者对电价上涨表示不满，有人将其与加州等其他地区进行比较。另一些人认为核能或其他政策可以缓解能源压力，同时普遍对政府优先事项及绿色替代方案的 affordability 表示怀疑。

**标签**: `#data centers`, `#energy consumption`, `#Ireland`, `#sustainability`, `#infrastructure`

---

<a id="item-3"></a>
## [陶哲轩利用 LLM 编码代理创建可视化工具](https://terrytao.wordpress.com/2026/07/11/old-and-new-apps-via-modern-coding-agents/) ⭐️ 8.0/10

菲尔兹奖得主陶哲轩发表博客文章，展示他如何利用现代编码代理（LLM）快速构建用于研究和教学的交互式可视化工具。 这展示了 LLM 编码代理在传统软件开发之外的实用价值，尤其是在教育和研究领域，并凸显了非传统领域对定制软件的巨大潜在需求。 陶哲轩指出，虽然 LLM 生成的补充内容对其论文并非至关重要，但此类可视化工具的负面影响风险是可接受的。该博客文章在热门聚合网站上获得 391 分和 111 条评论，显示出社区的高度关注。

hackernews · subset · 7月12日 11:09 · [社区讨论](https://news.ycombinator.com/item?id=48880170)

**背景**: 编码代理是一种 AI 工具，可以从自然语言提示生成代码，通常使用 GPT-4 或 Claude 等大型语言模型（LLM）。它们允许快速原型开发，包括交互式可视化，而无需深厚的编程专业知识。陶哲轩是著名数学家，他的认可为该方法增添了可信度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zencoder.ai/blog/best-free-ai-agents-for-coding">8 Best Free AI Agents for Coding To Try in 2026</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍赞同陶哲轩的平衡观点，指出该工具对教育和原型开发非常有用。有人幽默地将陶使用编码代理比作厨师发现微波炉食品。其他人则强调，在传统科技领域之外存在无限的软件潜在需求。

**标签**: `#LLM`, `#coding agents`, `#education`, `#software development`, `#visualization`

---

<a id="item-4"></a>
## [热爱 LLM，拒绝炒作](https://geohot.github.io//blog/jekyll/update/2026/07/12/i-love-llms.html) ⭐️ 8.0/10

George Hotz 发表博客文章，批评 LLM 炒作与实际创造价值之间的脱节，认为前沿实验室可能无法捕获其创造的价值。 这一批评呼应了日益增长的观点：尽管投入巨大，LLM 的经济价值可能流向用户和开源社区，而非构建它们的公司。它挑战了前沿 AI 实验室的估值，并凸显了向去中心化、定制化 AI 解决方案的转变。 文章强调，LLM 带来的生产力提升更多体现在私有的、一次性软件中，而非公共创新；社区评论中提出了‘随心所欲’时代的说法。一些评论者指出，像 Claude Sonnet 4 和 Opus 4.5 这样的新模型正在改变看法，但关于 AGI 时间线的不确定性依然存在。

hackernews · therepanic · 7月12日 18:31 · [社区讨论](https://news.ycombinator.com/item?id=48883343)

**背景**: 前沿 AI 实验室（如 OpenAI、Anthropic、Google DeepMind）是竞相构建最先进 AI 模型的公司。它们筹集了数十亿美元，现在对使用其最佳模型收取订阅费。然而，开源替代方案以及个人为特定需求定制 AI 的能力正在增长，引发了关于价值捕获和开源未来的问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.forbes.com/sites/josipamajic/2026/07/02/karp-says-frontier-ai-labs-are-stealing-enterprise-value-and-vcs-are-listening/">Karp Says Frontier AI Labs Are Stealing Enterprise ... - Forbes</a></li>
<li><a href="https://www.linkedin.com/pulse/frontier-ai-labs-what-building-why-transformation-leaders-kumar-gbuge/">Frontier AI Labs: What They Are Building — and Why ...</a></li>

</ul>
</details>

**社区讨论**: 社区讨论非常活跃，热门评论者认同价值捕获的论点。一位评论者指出，在当前订阅价格下，前沿模型对许多人来说是‘无需大脑’的选择；另一位则提出了‘随心所欲’时代的概念，即分叉和定制开源项目比以往任何时候都更容易。一些人表达了对开源未来的担忧，而另一些人则报告说新模型正在加速进步，使时间线变得不确定。

**标签**: `#LLMs`, `#AI hype`, `#open source`, `#productivity`, `#frontier labs`

---

<a id="item-5"></a>
## [Chromium 148 的 Math.tanh 允许操作系统指纹识别](https://scrapfly.dev/posts/browser-math-os-fingerprint/) ⭐️ 7.0/10

Chromium 148（V8 14.8.57）将 Math.tanh 的实现改为使用 std::tanh，后者调用宿主操作系统的数学库，产生的浮点结果在不同操作系统间存在差异，可用于识别底层操作系统。 这种新型指纹识别技术影响所有 Chromium 用户，可被反爬虫系统用于检测操作系统不匹配，损害隐私并增加浏览器伪装难度。 仅 Chrome 148 及更高版本（Chrome 148、149、150）受影响；早期版本不受影响。除了操作系统，该技术还可通过实现变化指纹识别浏览器版本范围。

hackernews · joahnn_s · 7月12日 21:12 · [社区讨论](https://news.ycombinator.com/item?id=48884853)

**背景**: 浮点运算结果因不同操作系统的数学库实现而异。浏览器指纹识别利用这些微小差异来识别用户。Math.tanh 是一种超越函数，其精度因平台而异，成为操作系统检测的信号。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://scrapfly.dev/posts/browser-math-os-fingerprint/">Your Browser Does Math Differently on Every OS, and Anti-Bot Systems Read the Bits · scrapfly.dev</a></li>
<li><a href="https://neoprint.dev/guide/collectors/math.html">Math Fingerprinting — neoprint | Open-Source Browser ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Floating-point_arithmetic">Floating-point arithmetic - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论指出该技术还可指纹识别浏览器版本范围而不仅是操作系统。有人批评文章来源 scrapfly 有自身利益，也有人建议使用正确舍入的超越函数作为修复方案。有用户希望 EFF 的 Cover Your Tracks 工具能包含这一信号。

**标签**: `#privacy`, `#fingerprinting`, `#browser`, `#Chromium`, `#security`

---

<a id="item-6"></a>
## [Anthropic 因计算限制延长 Claude Fable 5 可用时间](https://simonwillison.net/2026/Jul/12/bump/#atom-everything) ⭐️ 6.0/10

Anthropic 宣布将所有付费计划中 Claude Fable 5 的访问权限延长至 2026 年 7 月 19 日，并保持 Claude Code 每周速率限制提高 50%。与此同时，OpenAI 取消了 Plus、Business 和 Pro 计划中 GPT-5.6 Sol 的使用限制。 这一对比凸显了 AI 模型访问策略的差异：Anthropic 因计算限制谨慎延长，而 OpenAI 则激进取消限制。Fable 可用性的不确定性可能促使用户转向 OpenAI 的 GPT-5.6 Sol，从而改变市场格局。 在 Claude Max 计划中，用户最多可将每周使用限制的一半用于 Fable 5，之后可使用使用积分或切换模型。OpenAI 的 GPT-5.6 Sol 据称属于“Fable/Mythos 级别”模型，其效率改进将减少用量消耗。

rss · Simon Willison · 7月12日 21:20

**背景**: Claude Fable 5 是 Anthropic 于 2026 年 6 月发布的最强模型，适用于高要求编程和视觉任务。GPT-5.6 Sol 是 OpenAI 的最新前沿模型，专注于网络安全和长周期任务。两者均代表尖端 AI，但访问策略不同：Anthropic 因计算限制限制 Fable，而 OpenAI 取消限制以吸引用户。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://openai.com/index/previewing-gpt-5-6-sol/">Previewing GPT - 5 . 6 Sol : a next-generation model | OpenAI</a></li>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>

</ul>
</details>

**标签**: `#AI`, `#Anthropic`, `#Claude Fable 5`, `#GPT-5.6`, `#model access`

---

<a id="item-7"></a>
## [Zer0Fit：将 Google TabFM 和 TimesFM 封装为 MCP 服务器](https://www.reddit.com/r/MachineLearning/comments/1uue8cc/zer0fit_i_took_googles_new_tabfm_timesfm_ml/) ⭐️ 6.0/10

一位研究生发布了 Zer0Fit，这是一个将 Google 的 TabFM（表格基础模型）和 TimesFM（时间序列基础模型）封装到单个 Docker 容器中的 MCP 服务器，支持通过本地 LLM 进行零样本机器学习任务。该项目支持 CSV 输入，并在 Iris 和加州房价等经典数据集上进行了测试，准确率达 94.7%，回归 R²为 0.91。 Zer0Fit 降低了非专家执行分类、回归和预测等 ML 任务的门槛，无需手动训练或调参。通过 MCP 集成 Google 基础模型，它在 Open WebUI 等聊天界面中弥合了传统 ML 与生成式 AI 之间的鸿沟。 该服务器仅支持 CUDA，至少需要 16GB 显存，并通过 5 分钟 TTL 动态加载/卸载模型以释放内存。目前支持 CSV 文件，计划支持 XLS、XLSX、JSON 和 JSONL。由于依赖 PyTorch，不支持 Mac。

reddit · r/MachineLearning · /u/Porespellar · 7月12日 12:32

**背景**: TabFM 和 TimesFM 是 Google Research 分别针对表格数据和时间序列预测推出的零样本基础模型。它们在大规模合成数据上预训练，无需针对特定任务微调即可执行任务。Model Context Protocol（MCP）由 Anthropic 提出，是一种开放标准，允许 LLM 与外部工具和数据源连接，实现无缝集成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://research.google/blog/introducing-tabfm-a-zero-shot-foundation-model-for-tabular-data/">Introducing TabFM : A zero-shot foundation model for tabular data</a></li>
<li><a href="https://github.com/google-research/timesfm">GitHub - google -research/ timesfm : TimesFM ( Time Series...)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>

</ul>
</details>

**标签**: `#MCP`, `#TabFM`, `#TimesFM`, `#zero-shot`, `#foundation models`

---

<a id="item-8"></a>
## [基于上下文的神经网络线性映射观点](https://www.reddit.com/r/MachineLearning/comments/1uu2p63/context_and_average_best_linear_mappings_d/) ⭐️ 6.0/10

作者提出了一种神经网络的新视角，将每一层解释为基于输入上下文的平均最佳线性映射，并在 Archive.org 上提供了详细文档支持。 这一理论重构可能简化对神经网络信息处理方式的理解，有望带来更具可解释性的模型和新的架构见解。 该视角将每一层的输出视为输入特征经上下文相关系数加权后的线性组合，再对所有可能的上下文取平均。该概念在 Archive.org 上公开的文档中有详细解释。

reddit · r/MachineLearning · /u/oatmealcraving · 7月12日 02:18

**背景**: 在数学中，线性映射是向量空间之间保持向量加法和标量乘法的函数。神经网络通常使用非线性激活函数，但在特定上下文中将层表示为线性映射可以简化分析。这项工作建立在神经网络中上下文相关处理的思想上，该思想在持续学习和可解释 AI 等领域已有研究。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Linear_map">Linear map - Wikipedia</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#neural networks`, `#linear mappings`, `#context`

---

<a id="item-9"></a>
## [ACL 会议接收流程：ARR 审稿机制解析](https://www.reddit.com/r/MachineLearning/comments/1ut5krb/how_does_acl_conferences_acceptance_work_d/) ⭐️ 6.0/10

一位研究者询问*ACL 会议在已有 ARR 审稿和元审稿的情况下如何决定接收，指出分数与结果并不总是一致。社区解释称，会议会综合考虑所有审稿意见、元审稿和投稿 Track，并采用分级决策系统（主会、Findings、拒稿）。 这场讨论澄清了 NLP 研究人员常感困惑的接收流程，减少误解并设定合理预期，同时也凸显了 Findings Track 作为边缘论文中间地带的作用。 接收决策不仅基于总分数；会议会评估全部审稿意见、元审稿和论文的投稿 Track。排序从 Accept-Main 到 Reject，Findings Track 的论文被视同主会论文但无口头报告。

reddit · r/MachineLearning · /u/Happy_Today_3288 · 7月11日 00:47

**背景**: ACL Rolling Review (ARR) 是一个为计算语言学会议设立的集中审稿平台。论文在获得审稿人和行动编辑的元审稿后，被转发至具体会议做最终决策。会议程序委员会查看所有审稿意见和元审稿，并采用多级结果系统（主会、Findings、拒稿）。Findings 论文会发表在 ACL Anthology 但无口头报告。该系统旨在简化多个会议的审稿流程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aclrollingreview.org/">ACL Rolling Review – A peer review platform for the Association for...</a></li>
<li><a href="https://gist.github.com/antonisa/2158dee79179c7c49304ef353887bfa0">Conference Decisions · GitHub</a></li>
<li><a href="https://kinit.sk/quality-of-acl-findings-analysis-of-citations/">Quality of ACL “Findings”: analysis of citations - KInIT</a></li>

</ul>
</details>

**标签**: `#ACL`, `#conference acceptance`, `#NLP`, `#paper review`, `#meta-review`

---