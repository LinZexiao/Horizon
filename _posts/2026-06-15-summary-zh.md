---
layout: default
title: "Horizon Summary: 2026-06-15 (ZH)"
date: 2026-06-15
lang: zh
---

> 从 24 条内容中筛选出 16 条重要资讯。

---

1. [Pyodide 314.0 支持将 WASM 轮子发布到 PyPI](#item-1) ⭐️ 9.0/10
2. [美国政府要求 Anthropic 暂停 Fable 5 和 Mythos 5 的访问](#item-2) ⭐️ 9.0/10
3. [Kage：将网站转为离线单二进制存档](#item-3) ⭐️ 8.0/10
4. [里约热内卢‘自主研发’大语言模型被揭露为现有模型的合并](#item-4) ⭐️ 8.0/10
5. [批评将 Anthropic 比作末日装置公司](#item-5) ⭐️ 8.0/10
6. [形式化方法与编程的未来](#item-6) ⭐️ 8.0/10
7. [为何 AI 不会取代软件工程师](#item-7) ⭐️ 8.0/10
8. [将 SQLite 结果列映射回源表.列](#item-8) ⭐️ 8.0/10
9. [开源知识图谱管道结合混合检索提升 LLM 推理能力](#item-9) ⭐️ 8.0/10
10. [连贯上下文悄然改变 LLM 内部状态，安全系统视而不见](#item-10) ⭐️ 8.0/10
11. [验证税：工具使用型 LLM 代理的安全性与成功率权衡](#item-11) ⭐️ 8.0/10
12. [使用 ncnn 的 C++ PaddleOCR 实现，支持 v3 到 v6 模型](#item-12) ⭐️ 7.0/10
13. [兼容 Caddy 的 Zeroserve 性能提升但缺少关键功能](#item-13) ⭐️ 6.0/10
14. [免费双语机器学习笔记本课程寻求反馈](#item-14) ⭐️ 6.0/10
15. [异常检测与分类在癌症类似物识别中的对比](#item-15) ⭐️ 6.0/10
16. [MDP 无导数优化器在 MNIST 上超越 Adam](#item-16) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Pyodide 314.0 支持将 WASM 轮子发布到 PyPI](https://simonwillison.net/2026/Jun/13/publishing-wasm-wheels/#atom-everything) ⭐️ 9.0/10

这消除了 Pyodide 生态系统中的一个主要瓶颈，减轻了核心维护者的负担，并使社区能够为基于浏览器的环境分发 Python 包。这符合通过 WebAssembly 使 Python 在浏览器中完全可用的更广泛趋势。 该支持基于 PEP 783 中定义的 PyEmscripten 平台，相应的 PyPI 变更于 4 月 21 日通过 PR #19804 落地。Simon Willison 通过发布一个 luau-wasm 包演示了此工作流，该包可在 Pyodide 内运行类似 Lua 的语言。

rss · Simon Willison · 6月13日 23:55

**背景**: Pyodide 是一个基于 WebAssembly、面向浏览器和 Node.js 的 Python 发行版，使 Python 代码能在客户端运行。在此之前，分发包含针对 WASM 编译的 C 或 Rust 扩展的 Python 包需要手动托管，且无法通过 PyPI 实现。PEP 783 标准化了这些轮子的平台标签，使其与 PyPI 的集成成为可能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/13/publishing-wasm-wheels/">Publishing WASM wheels to PyPI for use with Pyodide</a></li>
<li><a href="https://pyodide.org/">Pyodide — Version 314.0.0</a></li>
<li><a href="https://peps.python.org/pep-0783/">PEP 783 – Emscripten Packaging | peps .python.org</a></li>

</ul>
</details>

**标签**: `#Pyodide`, `#WebAssembly`, `#PyPI`, `#Python`, `#WASM`

---

<a id="item-2"></a>
## [美国政府要求 Anthropic 暂停 Fable 5 和 Mythos 5 的访问](https://simonwillison.net/2026/Jun/13/us-government-directive-to-suspend-access/#atom-everything) ⭐️ 9.0/10

美国政府于 2026 年 6 月 12 日向 Anthropic 发布出口管制指令，以国家安全为由，要求暂停对 Fable 5 和 Mythos 5 AI 模型的所有访问，原因是一项发现的越狱方法。Anthropic 已遵守命令，立即为所有客户（包括外籍员工）禁用访问权限。 此次前所未有的政府干预标志着 AI 政策的重大转变，可能为先进 AI 模型的国家安全审查开创先例。它引发了关于模型安全性、监管过度以及前沿 AI 能力开放访问未来的关键问题。 所谓的越狱涉及要求模型审查特定代码库并修复软件缺陷，Anthropic 认为该技术并非其模型独有，且防御者在日常安全工作中也会使用。根据 Simon Willison 的 API 测试，Fable 5 的访问于 2026 年 6 月 12 日太平洋时间下午 6:59 被切断。

rss · Simon Willison · 6月13日 01:01

**背景**: Claude Fable 5 和 Claude Mythos 5 是 Anthropic 于 2026 年 6 月发布的先进大型语言模型。Mythos 5 属于“Mythos 级”模型，专为安全研究和自主编码设计；Fable 5 则优化用于前沿物理研究，具有 100 万 token 的上下文窗口。这两个模型共享相同的基础模型，代表了 AI 能力的重大飞跃，在某些基准测试中超越了 GPT-5.5 等先前模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mashable.com/tech/anthropic-claude-fable-5-vs-openai-gpt-5-5">Claude Fable 5 vs GPT 5.5: Is this why the Trump admin... | Mashable</a></li>
<li><a href="https://9to5mac.com/2026/06/12/anthropic-pulls-claude-mythos-5-and-claude-fable-5-following-us-government-directive/">Anthropic pulls Claude Mythos 5 and Claude Fable... - 9to 5 Mac</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#government regulation`, `#model security`, `#Anthropic`, `#national security`

---

<a id="item-3"></a>
## [Kage：将网站转为离线单二进制存档](https://github.com/tamnd/kage) ⭐️ 8.0/10

Kage 是一款新的开源工具，它通过驱动真实浏览器抓取网页并移除 JavaScript，将任意网站克隆成一个离线可浏览的单一二进制文件。 这简化了网站存档和离线访问，无需完整服务器配置即可轻松分享或保存复杂网站。 该工具使用无头浏览器抓取动态内容，但生成的静态网站需要通过内置 HTTP 服务器来访问，无法直接从文件系统打开。

hackernews · tamnd · 6月14日 17:25 · [社区讨论](https://news.ycombinator.com/item?id=48529990)

**背景**: 传统的“另存为”方法对于现代 JavaScript 密集型网站会生成不完整的存档。Kage（影，意为“影子”）则驱动真实浏览器，按用户所见抓取页面，然后使其静态化，保留视觉结构且无需依赖项。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/tamnd/kage">GitHub - tamnd/kage: Shadow any website for offline viewing, with the JavaScript stripped out · GitHub</a></li>
<li><a href="https://kage.tamnd.com/">kage</a></li>

</ul>
</details>

**社区讨论**: 用户报告了 HTTP 站点的 DNS 解析失败 bug。其他人讨论了离线公司 Wiki 和 AI 原型存档等用例，并建议改进以支持无服务器的 HTML 文件输出。

**标签**: `#offline`, `#website mirroring`, `#tool`, `#archiving`, `#productivity`

---

<a id="item-4"></a>
## [里约热内卢‘自主研发’大语言模型被揭露为现有模型的合并](https://github.com/nex-agi/Nex-N2/issues/4) ⭐️ 8.0/10

社区调查发现，里约热内卢市政府发布的 Rio-3.5-Open-397B 模型并非自主微调，而是 Nex-N2 Pro 和 Qwen3.5 的加权合并，且未进行适当归属说明。 此事件凸显了 AI 模型发布中透明度和适当归属的必要性，特别是公共机构，并引发了关于该领域未公开模型合并现象的担忧。 Rio 模型中每个权重张量在所有层上大约都是 Nex 和 Qwen 的 0.6/0.4 混合，该模型被声称是超越同类开源模型的微调版本，但未提及合并操作。

hackernews · unrvl22 · 6月14日 15:37 · [社区讨论](https://news.ycombinator.com/item?id=48528371)

**背景**: 模型合并是一种将共享相同基础架构的多个模型的权重合并为一个模型的技术，通常无需重新训练。它可以提升性能，但需要适当披露以尊重原创者的工作。此次事件是开源 AI 伦理实践更广泛讨论的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mychen76.medium.com/the-art-of-model-blending-and-moerges-bac7f3749ab7">LLM Model Merging . In this article, I will share my views | Medium</a></li>
<li><a href="https://arxiv.org/html/2408.07666v5">Model Merging in LLMs, MLLMs, and Beyond: Methods, Theories...</a></li>

</ul>
</details>

**社区讨论**: 社区评论反应不一：有人推测可能出于技术原因（如未包含蒸馏步骤），而另一些人则批评缺乏归属，并怀疑这是常见做法。一位评论者指出，权重的简单线性组合反而提升了性能而未退化。

**标签**: `#LLM`, `#model attribution`, `#open source`, `#ethics`, `#community investigation`

---

<a id="item-5"></a>
## [批评将 Anthropic 比作末日装置公司](https://www.verysane.ai/p/did-anthropic-ask-for-this) ⭐️ 8.0/10

一篇批评文章将 Anthropic 比作末日装置公司，指责这家 AI 安全公司从它所警告的技术中获利，存在虚伪行为。 这一批评可能削弱 Anthropic 在 AI 安全领域的公信力，影响公众信任以及对其伦理主张的监管审查。 文章用末日装置公司的类比——一边警告风险，一边靠销售装置获利——来突出 Anthropic 作为安全倡导者和 AI 开发者的双重角色中存在的矛盾。

hackernews · ad8e · 6月14日 22:23 · [社区讨论](https://news.ycombinator.com/item?id=48533504)

**背景**: Anthropic 是一家由前 OpenAI 员工创立的 AI 研究公司，高度重视安全与伦理。该公司在开发 Claude 等强大 AI 模型的同时倡导监管。本文质疑这种双重角色是否自相矛盾，引发了关于傲慢与伦理定位的讨论。

**社区讨论**: 评论者意见不一：一些同意批评，指出傲慢和自利；另一些则为 Anthropic 辩护，认为对生存风险的真诚信念为其行为提供了正当理由。还有讨论涉及政府影响以及 AI 监管的政治环境。

**标签**: `#AI safety`, `#Anthropic`, `#ethics`, `#tech criticism`, `#hubris`

---

<a id="item-6"></a>
## [形式化方法与编程的未来](https://blog.janestreet.com/formal-methods-at-jane-street-index/?from_theconsensus=1) ⭐️ 8.0/10

Jane Street 探讨将形式化方法整合到编程中，认为随着 AI 生成更多代码，人类的价值将转向验证和证明辅助。 这一观点凸显了软件工程向严格验证的潜在转变，这可以提高可靠性和安全性，尤其是在关键系统中。 博客文章讨论了使用证明助手和 SAT 求解器等形式化方法，并指出最困难的部分是人类建议引理和引导证明的任务。

hackernews · eatonphil · 6月14日 12:35 · [社区讨论](https://news.ycombinator.com/item?id=48526633)

**背景**: 形式化方法是用于规范和验证软件/硬件系统的数学严格技术。像 Coq 或 Isabelle 这样的证明助手支持交互式定理证明，由人类引导证明搜索。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Formal_methods">Formal methods</a></li>
<li><a href="https://en.wikipedia.org/wiki/Proof_assistant">Proof assistant</a></li>

</ul>
</details>

**社区讨论**: 来自专家（如 'Animats'）的评论描述了证明自动化的历史经验，指出简单部分由 SAT 求解器处理，而更难的证明需要人类指导。另一位评论者 'winwang' 分享了在 Scala 3 中使用表达性类型进行编译时证明，这有助于防止 AI 生成代码的质量问题。

**标签**: `#formal methods`, `#programming languages`, `#AI verification`, `#software reliability`, `#Hacker News`

---

<a id="item-7"></a>
## [为何 AI 不会取代软件工程师](https://simonwillison.net/2026/Jun/14/why-ai-hasnt-replaced-software-engineers/#atom-everything) ⭐️ 8.0/10

Arvind Narayanan 和 Sayash Kapoor 发表文章，引用纽约 WARN 法案数据——首年没有一家公司报告 AI 相关裁员——论证 AI 不会导致软件工程师大规模失业。 这直接反驳了 AI 将很快自动化软件工程工作的流行说法，为开发人员提供了基于证据的 reassurance，并影响了关于 AI 经济影响的讨论。 文章指出 AI 无法替代的三个真正瓶颈：决定构建什么、验证交付成果，以及对代码库、业务和环境的深度人类理解。

rss · Simon Willison · 6月14日 23:54

**背景**: 像 GitHub Copilot 这样的 AI 编码助手发展迅速，引发了软件工程师可能被取代的担忧。然而，专业软件工程远不止输入代码，还需要复杂的推理、沟通和问责。

**标签**: `#AI`, `#software engineering`, `#job automation`, `#economy`

---

<a id="item-8"></a>
## [将 SQLite 结果列映射回源表.列](https://simonwillison.net/2026/Jun/13/sqlite-column-provenance/#atom-everything) ⭐️ 8.0/10

Simon Willison 研究了如何以编程方式将 SQL 查询结果列映射回 SQLite 中的源表和列，他使用 Claude Code（Opus 4.8）探索了多种解决方案，包括 apsw、通过 ctypes 访问 sqlite3_column_table_name() 函数以及分析 EXPLAIN 输出。 这项工作可以使 Datasette 能够为 SQL 查询结果添加列来源信息，从而改进数据分析和调试体验。利用 AI 辅助编码解决具体技术问题，展示了数据库工具开发的新方法。 Claude Code 确定了三种有前景的方法：使用 apsw 库、通过 Python ctypes 直接调用 SQLite C 函数 sqlite3_column_table_name()、以及解析 EXPLAIN 输出来推断列来源。该研究托管在 simonw/research 的公共 GitHub 仓库中。

rss · Simon Willison · 6月13日 23:05

**背景**: Datasette 是一个用于探索和发布数据的开源工具，常与 SQLite 搭配使用。列来源是指追踪每个结果值来自哪个表和列，SQLite 的 Python 绑定并未直接提供此功能。SQLite C API 提供了 sqlite3_column_table_name() 函数，但 Python 没有暴露它。Claude Code 是 Anthropic 的代理式编码工具，能够读取代码库并执行命令。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/13/sqlite-column-provenance/">Research: Mapping SQLite result columns back to their source...</a></li>
<li><a href="https://code.claude.com/docs/en/overview">Overview - Claude Code Docs</a></li>

</ul>
</details>

**标签**: `#SQLite`, `#Datasette`, `#Query Parsing`, `#AI-Assisted Coding`

---

<a id="item-9"></a>
## [开源知识图谱管道结合混合检索提升 LLM 推理能力](https://www.reddit.com/r/MachineLearning/comments/1u5yyyl/i_built_an_opensource_knowledge_graph_pipeline/) ⭐️ 8.0/10

一位开发者发布了一个开源全栈管道，可从原始文本构建知识图谱、检测主题社区，并使用混合检索（稠密向量 + BM25）解决“中间丢失”问题，改进 LLM 的多跳推理能力。 它解决了标准向量检索中因片段断开导致多跳查询失败的关键缺陷。通过融合图遍历与混合搜索，该管道使 LLM 能够进行多步推理，这对问答系统和文档分析等应用至关重要。 管道使用 spaCy 提取实体，NetworkX 配合贪心模块度进行社区检测，并为每个社区生成 LLM 摘要。检索结合了稠密向量搜索和 BM25，通过倒数排名融合（RRF）合并，再由交叉编码器重新排序。

reddit · r/MachineLearning · /u/Future_Caregiver_643 · 6月14日 22:38

**背景**: 标准的 RAG（检索增强生成）系统在处理需要连接不同文本片段事实的多跳问题时常常遇到困难。知识图谱明确表示实体及其关系，通过图遍历可以桥接不连续的片段。混合检索结合了稠密（语义）和稀疏（词汇）搜索，覆盖了语义漂移和精确关键词匹配，提高了检索质量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://neo4j.com/blog/genai/knowledge-graph-llm-multi-hop-reasoning/">How to improve multi-hop reasoning with knowledge graphs and LLMs - Graph Database & Analytics</a></li>
<li><a href="https://sabankara.medium.com/why-we-should-upgrade-classical-rag-with-hybrid-sparse-dense-retrieval-and-reranking-2b991d4bb95f">Why We Should “Upgrade” Classical RAG with Hybrid ( Sparse ...)</a></li>
<li><a href="https://www.aidoczh.com/networkx/reference/algorithms/generated/networkx.algorithms.community.modularity_max.greedy_modularity_communities.html">greedy_modularity_communities — NetworkX 3.4rc0.dev0 documentation</a></li>

</ul>
</details>

**标签**: `#knowledge graph`, `#LLM`, `#hybrid retrieval`, `#open-source`, `#NLP`

---

<a id="item-10"></a>
## [连贯上下文悄然改变 LLM 内部状态，安全系统视而不见](https://www.reddit.com/r/MachineLearning/comments/1u5xnxg/coherent_context_can_silently_shift_llms_into_a/) ⭐️ 8.0/10

一位独立研究者发现，提供连贯密集的文本作为上下文可以改变 LLM 的内部状态（隐藏状态和残差流轨迹），而不改变其表面输出，这种改变不会被当前的 RLHF 或输出分类器等安全过滤器检测到。 这一发现揭示了当前 LLM 对齐方法存在根本性盲点——它们只监控最终输出；这表明安全措施必须发展到持续监控隐藏状态，因为仅凭连贯的上下文就能悄然绕过它们。 实验主要在开源模型 Gemma-3-12B-IT 上进行，使用了隐藏状态几何、残差流轨迹、对比控制、SAE 读数以及教师强制 KL 散度。目标文本并非直接的越狱提示，而是建立特定话语模式的密集连贯文本。

reddit · r/MachineLearning · /u/PresentSituation8736 · 6月14日 21:42

**背景**: 大型语言模型通过堆叠的 Transformer 层处理文本，每层向跨 token 的'残差流'添加信息，残差流携带隐藏状态。机械可解释性研究这些内部状态以理解模型如何推理。当前的安全对齐方法（如 RLHF 和输出分类器）仅检查最终生成的文本，忽略了内部表示空间——其中不同的状态模式可能早已活跃。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://paperdive.ai/concepts/residual-stream.html">Residual Stream · AI Papers: A Deep Dive</a></li>
<li><a href="https://medium.com/@khayyam.h/understanding-and-controlling-llm-internal-representations-87c939957b25">Understanding and controlling LLM internal representations | by Khayyam H. | Medium</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#mechanistic interpretability`, `#LLM alignment`, `#representation space`, `#hidden states`

---

<a id="item-11"></a>
## [验证税：工具使用型 LLM 代理的安全性与成功率权衡](https://www.reddit.com/r/MachineLearning/comments/1u58mkq/the_verifier_tax_horizondependent_safetysuccess/) ⭐️ 8.0/10

在 ACM CAIS 2026 上发表的一篇论文引入了“验证税”概念，即工具使用型 LLM 代理中随任务长度变化的安全性与成功率之间的权衡，并提出了一种两层验证架构以减少不安全完成。 这项研究正式化了 LLM 代理安全评估中的一个关键陷阱，表明验证可以减少不安全成功，但随着任务长度增加也会降低任务完成率。这可能重塑代理评估的设计和报告方式。 论文在τ-bench 工具使用场景上进行评估，采用两层架构：先进行确定性策略/工具检查，再使用基于 LLM 的验证器进行上下文安全检查。验证税量化了安全性与成功率之间的权衡，且随任务长度增加而恶化。

reddit · r/MachineLearning · /u/AccomplishedLeg1508 · 6月14日 02:09

**背景**: 工具使用型 LLM 代理可能完成任务但违反安全策略，产生“不安全成功”。标准基准通常将完成视为成功而不检查安全性，从而掩盖了这种风险。τ-bench 是一个用于现实世界领域中工具-代理-用户交互的基准，提供航班改签、行李处理等场景。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/sierra-research/tau2-bench">GitHub - sierra-research/tau2-bench: τ-Bench: A Benchmark for Tool-Agent-User Interaction in Real-World Domains · GitHub</a></li>
<li><a href="https://www.preprints.org/manuscript/202604.1029">AgentVerify: Compositional Formal Verification of AI Agent Safety Properties via LTL Model Checking[v1] | Preprints.org</a></li>

</ul>
</details>

**标签**: `#LLM Agents`, `#AI Safety`, `#Verification`, `#Tool Use`, `#Evaluation`

---

<a id="item-12"></a>
## [使用 ncnn 的 C++ PaddleOCR 实现，支持 v3 到 v6 模型](https://www.reddit.com/r/MachineLearning/comments/1u4hy2x/paddleocr_v3v4v5v6_implemented_in_c_with_ncnn_p/) ⭐️ 7.0/10

一位开发者发布了基于 ncnn 推理框架的 PaddleOCR C++ 开源实现，现已支持 PP-OCR v3 到最新的 v6 模型。该实现替代了官方 Paddle C++ 运行时（体积大且复杂），提供了更轻量、更快速的替代方案。 该项目简化了在移动或边缘设备上工作的开发者的 OCR 部署，在这些场景中轻量级推理至关重要。它减少了依赖负担并提高了推理速度，使最先进的 OCR 在资源受限环境中更易用。 该实现使用了 ncnn，一个专为移动平台设计的高性能神经网络推理框架，支持大多数常见 CNN 网络。仓库包含对多个 PaddleOCR 模型版本（v3 到 v6）的支持，使用户能够根据准确率和速度需求选择最佳模型。

reddit · r/MachineLearning · /u/Knok0932 · 6月13日 05:06

**背景**: PaddleOCR 是百度 PaddlePaddle 开发的开源 OCR 工具包，支持超过 100 种语言。官方 Paddle C++ 推理运行时依赖较多，部署复杂。ncnn 是一个专为移动和嵌入式系统优化的轻量级推理框架，性能更快且集成更简单。该项目通过提供基于 ncnn 的 C++ 实现，填补了高效 OCR 推理的空白。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/PaddlePaddle/PaddleOCR">GitHub - PaddlePaddle/PaddleOCR: Turn any PDF or image document into structured data for your AI. A powerful, lightweight OCR toolkit that bridges the gap between images/PDFs and LLMs. Supports 100+ languages. · GitHub</a></li>
<li><a href="https://sourceforge.net/projects/ncnn.mirror/files/20260526/ncnn-20260526-windows-vs2022-shared.zip/download">Download ncnn -20260526-windows-vs2022-shared.zip ( ncnn )</a></li>

</ul>
</details>

**标签**: `#PaddleOCR`, `#OCR`, `#ncnn`, `#C++`, `#deployment`

---

<a id="item-13"></a>
## [兼容 Caddy 的 Zeroserve 性能提升但缺少关键功能](https://su3.io/posts/zeroserve-caddy-compat) ⭐️ 6.0/10

基于 eBPF 的 Web 服务器 Zeroserve 已与 Caddy 集成，与基准 Caddy 相比，吞吐量提升 3 倍，延迟降低 70%。 尽管性能提升令人印象深刻，但缺少 ACME 协议支持和插件兼容性限制了实际部署，突显了现代 Web 服务器在速度与功能完备性之间的权衡。 Zeroserve 使用 io_uring 进行异步 I/O，但一些资料指出这对网络安全存在风险；此外，与 Caddy 的兼容性缺少自动 TLS 证书管理等核心功能以及许多 Caddy 插件。

hackernews · losfair · 6月14日 13:43 · [社区讨论](https://news.ycombinator.com/item?id=48527145)

**背景**: Caddy 是一种流行的 Web 服务器，以通过 ACME 协议自动管理 HTTPS 而闻名。Zeroserve 是一种零配置、可通过 eBPF 脚本编程的 Web 服务器，旨在利用 io_uring 实现高性能。io_uring 是一种 Linux 内核接口，用于异步 I/O，相比传统方法开销更低，但可能带来安全风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://su3.io/posts/introducing-zeroserve">zeroserve : a zero -config web server you can script with eBPF</a></li>
<li><a href="https://en.wikipedia.org/wiki/Io_uring">Io uring</a></li>
<li><a href="https://en.wikipedia.org/wiki/ACME_protocol">ACME protocol</a></li>

</ul>
</details>

**社区讨论**: 评论反应不一：一些用户对性能数字感到兴奋，但多位用户指出缺少 ACME 支持是一个致命缺陷。还提到了 io_uring 的安全隐患以及有限的 Caddy 兼容性（缺少插件）。

**标签**: `#performance`, `#web server`, `#Caddy`, `#io_uring`, `#networking`

---

<a id="item-14"></a>
## [免费双语机器学习笔记本课程寻求反馈](https://www.reddit.com/r/MachineLearning/comments/1u4zbld/im_building_a_free_bilingual_machinelearning/) ⭐️ 6.0/10

一位开发者发布了一个开源的英波双语机器学习教程仓库，使用 Jupyter 笔记本格式，并正在征求社区对课程结构、覆盖范围和实用性的反馈。 这一举措可以降低波斯语学习者获得高质量实践性机器学习教育的门槛，并且社区驱动的方式有助于确保内容满足真实学习需求。 该仓库涵盖机器学习工作流程、数据清洗、回归、分类、树模型、聚类、时间序列、异常检测、责任型机器学习和 MLOps，并提供英波双语并行的笔记本。

reddit · r/MachineLearning · /u/abolfazl1363 · 6月13日 19:07

**背景**: Jupyter 笔记本是广泛用于教学和机器学习原型的交互式文档。双语教育资源对非英语母语者来说很珍贵但稀少，可以让学习者在用母语掌握技术概念的同时学习英语术语。MLOps 是一套在生产中部署和维护机器学习模型的实践，而责任型机器学习关注伦理、公平性和透明度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/MLOps">MLOps</a></li>
<li><a href="https://hildeweerts.github.io/responsiblemachinelearning/">An Introduction to Responsible Machine Learning — An Introduction...</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#education`, `#Jupyter notebooks`, `#bilingual`, `#open source`

---

<a id="item-15"></a>
## [异常检测与分类在癌症类似物识别中的对比](https://www.reddit.com/r/MachineLearning/comments/1u4obgy/anomaly_detection_vs_classification_for_visually/) ⭐️ 6.0/10

一位 Reddit 用户提问：当阴性样本（类似物）在视觉和形态上与癌症非常相似时，检测癌症应使用异常检测还是监督分类。该问题突显了医学机器学习中的一个方法学困境。 这个问题直击医学影像 AI 的关键挑战：良性类似物可能导致误诊或漏诊。异常检测与分类的选择会影响模型性能、鲁棒性和临床采纳。 用户特别描述了癌症与类似物非常相似的场景，这对两种方法都是难题。该问题未包含实验结果，而是寻求社区的理论和实践建议。

reddit · r/MachineLearning · /u/DryHat3296 · 6月13日 11:18

**背景**: 在癌症诊断中，“类似物”是指在影像上看起来像癌症的良性病变，通常需要高级检测来区分。异常检测将目标类视为分布内，其余视为分布外；监督分类则明确学习类别间的决策边界。选择取决于数据可用性、类别相似度和临床需求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://incitefulmed.com/resources/guides/gallbladder-bile-duct-cancer-diagnosis-guide/biliary-cancer-symptoms-mimics/">Biliary Cancer : Symptoms & Warning Signs | Inciteful Med Resources</a></li>
<li><a href="https://stats.stackexchange.com/questions/562650/imbalanced-classification-vs-anomaly-detection/592677">machine learning - Imbalanced classification vs anomaly detection ...</a></li>

</ul>
</details>

**标签**: `#anomaly detection`, `#classification`, `#medical imaging`, `#machine learning`

---

<a id="item-16"></a>
## [MDP 无导数优化器在 MNIST 上超越 Adam](https://www.reddit.com/r/MachineLearning/comments/1u4fc16/derivativefree_neural_network_optimization_mnist/) ⭐️ 6.0/10

一种名为 MDP 的无导数优化方法在 MNIST 上使用小型 784-32-10 神经网络达到了 93.4%的测试准确率，在不使用梯度的情况下超过了 Adam 的 91.7%。 这一结果表明，在特定神经网络任务中，无导数优化可以与基于梯度的方法竞争，从而在梯度无法获取或计算成本高昂时提供一种替代方案。 优化过程在 25,450 维参数空间上进行了 1,000,000 次函数评估，直接最小化 5,000 张训练图像的交叉熵损失。MDP 最终损失为 0.0004083，验证准确率为 93.7%，而 Adam 的损失为 0.002945，验证准确率为 91.8%。

reddit · r/MachineLearning · /u/Mis4318 · 6月13日 02:51

**背景**: 无导数优化（DFO）方法仅依赖函数评估来优化目标函数，无需使用梯度信息。它们在梯度不可用、有噪声或计算昂贵时非常有用，但通常在高维问题上表现不佳。这项工作表明，DFO 可以在简单的神经网络任务上扩展到超过 25,000 个参数。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.academia.edu/145050332/Two_derivative_free_optimization_algorithms_for_mesh_quality_improvement">(PDF) Two derivative - free optimization algorithms for mesh quality...</a></li>
<li><a href="https://vdoc.pub/documents/introduction-to-derivative-free-optimization-22tajmri9rtg">Introduction To Derivative - free Optimization [PDF] [22tajmri9rtg]</a></li>
<li><a href="https://optimization-online.org/wp-content/uploads/2026/01/Riemannian_optimization_with_finite-difference_gradient.pdf">Riemannian optimization with finite-difference gradient</a></li>

</ul>
</details>

**标签**: `#derivative-free optimization`, `#neural networks`, `#MNIST`, `#optimization`, `#MDP`

---