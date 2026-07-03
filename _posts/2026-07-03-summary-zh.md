---
layout: default
title: "Horizon Summary: 2026-07-03 (ZH)"
date: 2026-07-03
lang: zh
---

> 从 29 条内容中筛选出 15 条重要资讯。

---

1. [CDD 仅从 logits 恢复微调原始数据](#item-1) ⭐️ 9.0/10
2. [欧盟议会间谍软件调查员遭 Pegasus 黑客攻击](#item-2) ⭐️ 8.0/10
3. [本地运行大模型硬件成本指南](#item-3) ⭐️ 8.0/10
4. [Current AI 发布开源 AI 差距地图](#item-4) ⭐️ 8.0/10
5. [Josh Comeau 报告课程销量因 AI 下降 50% 以上](#item-5) ⭐️ 8.0/10
6. [针对开放权重模型，微调抵抗是否有意义？](#item-6) ⭐️ 8.0/10
7. [Costco：反亚马逊的零售模式](#item-7) ⭐️ 7.0/10
8. [工厂也可以只是一个房间](#item-8) ⭐️ 7.0/10
9. [llm-coding-agent 0.1a0：编码助手的早期 Alpha 版本](#item-9) ⭐️ 7.0/10
10. [理解以参与：避免 AI 代理带来的认知负债](#item-10) ⭐️ 7.0/10
11. [H64LM：基于 PyTorch 从零构建的 2.49 亿参数混合专家 Transformer](#item-11) ⭐️ 7.0/10
12. [博士生寻求提升机器学习数学基础的书籍推荐](#item-12) ⭐️ 7.0/10
13. [让 AI 代理自行判断以降低成本](#item-13) ⭐️ 6.0/10
14. [使用 DSPy 优化 Datasette Agent 的 SQL 提示](#item-14) ⭐️ 6.0/10
15. [机器学习顶会如何评选最佳论文、口头报告和亮点展示](#item-15) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [CDD 仅从 logits 恢复微调原始数据](https://www.reddit.com/r/MachineLearning/comments/1umn2dk/contrastive_decoding_diffing_cdd_recovering/) ⭐️ 9.0/10

研究人员提出了对比解码差分（CDD）方法，这是一种灰盒方法，仅通过 logit 访问即可从大语言模型中恢复逐字的微调数据，无需模型权重或激活。CDD 在四个模型家族的 20 个模型对上，有 19 个达到了 4+/5 的逐字恢复得分，超过了之前白盒的激活差异透镜（ADL）方法，后者从未超过 3/5。 这项工作对 LLM 的安全性和透明度具有重大意义，因为它表明即使只暴露 logits 的黑盒模型也能提取微调数据。它还突显了一个潜在的隐私风险：LLM 生成的合成数据可能会嵌入伪影（如虚构人物'Dr. Elena Rodriguez'），这些伪影可以在不同的微调任务中被恢复。 CDD 使用单一默认配置，无需逐个校准或选择层，直接对比基础模型和微调模型的 logits。一个意外的发现是，在四个不相关的微调领域中，恢复出的文本中反复出现同一个虚构人物'Dr. Elena Rodriguez'，这源于 Claude Sonnet 3.6 在生成合成科学家姓名时的偏好。

reddit · r/MachineLearning · /u/CebulkaZapiekana · 7月3日 19:01

**背景**: 模型差分是比较两个版本模型差异的任务，常用于检测微调或数据投毒。对比解码是一种通过最大化强模型和弱模型在 log 概率上的加权差异来放大差异的技术。先前的激活差异透镜（ADL）方法需要完全权重访问才能通过激活差异检测微调痕迹，这促使了 CDD 作为更实用的灰盒替代方案的开发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2510.13900">Narrow Finetuning Leaves Clearly Readable Traces in Activation ...</a></li>
<li><a href="https://arxiv.org/abs/2309.09117">[2309.09117] Contrastive Decoding Improves Reasoning in Large Language Models</a></li>
<li><a href="https://www.emergentmind.com/topics/model-diffing">Model Diffing : Techniques & Applications</a></li>

</ul>
</details>

**标签**: `#model-diffing`, `#contrastive-decoding`, `#llm-security`, `#finetuning`, `#logit-analysis`

---

<a id="item-2"></a>
## [欧盟议会间谍软件调查员遭 Pegasus 黑客攻击](https://citizenlab.ca/research/member-of-committee-investigating-spyware-hacked-with-pegasus/) ⭐️ 8.0/10

公民实验室的法医分析证实，正在调查间谍软件的欧洲议会议员斯泰利奥斯·库洛格卢（Stelios Kouloglou）的 iPhone 在 2022 年和 2023 年多次被 Pegasus 间谍软件成功感染。 这一事件凸显了当议会调查人员本身成为商业间谍软件目标时对民主监督的威胁，可能危及对监控滥用行为的敏感调查。 感染发生在 2022 年 10 月 21 日左右以及 2023 年 3 月 6 日至 7 日，有证据将第一次感染与针对俄罗斯和白俄罗斯流亡记者的行动联系起来，表明这是一个在多个欧洲国家拥有授权的 Pegasus 客户所为。

hackernews · ledoge · 7月3日 20:38 · [社区讨论](https://news.ycombinator.com/item?id=48779683)

**背景**: Pegasus 是由 NSO Group 开发的间谍软件，设计用于对移动设备进行隐蔽远程安装。它被宣传用于预防犯罪和恐怖主义，但被广泛用于监视记者、活动家和政治人物。Citizen Lab 是领先的网络监督机构，调查此类监控威胁。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pegasus_(spyware)">Pegasus (spyware)</a></li>

</ul>
</details>

**社区讨论**: 评论者对 NSO 员工仍能旅行而不被逮捕表示愤慨，质疑议会设备如何能同时被泄露个人医疗和政府数据，并提到希腊的类似丑闻暗示国内 Pegasus 使用有政府参与。

**标签**: `#cybersecurity`, `#Pegasus`, `#spyware`, `#European Parliament`, `#surveillance`

---

<a id="item-3"></a>
## [本地运行大模型硬件成本指南](https://github.com/jamesob/local-llm) ⭐️ 8.0/10

Jamesob 发布了一份详细指南，介绍了本地运行最先进大语言模型的硬件配置和成本，涵盖从预算级到极致的方案。 这很重要，因为它提供了本地大模型推理的 realistic 成本分析，帮助爱好者和专业人士在昂贵的硬件投资上做出明智决策。 指南包括一个 4 万美元的配置（实际成本 5-5.5 万美元），使用 4 块单价 1.2 万美元的 GPU，以及一个更易获得的 2 块 RTX 3090 配置（48GB 显存），可运行 Qwen3.6-27B。

hackernews · livestyle · 7月3日 15:03 · [社区讨论](https://news.ycombinator.com/item?id=48775921)

**背景**: 大型语言模型（LLM）推理需要大量显存和计算能力。本地运行可避免 API 成本和隐私问题，但需要昂贵的硬件，通常涉及多块高端 GPU 和量化技术。

**社区讨论**: 评论者警告不要低估成本，并指出云托管可能比购买硬件更便宜。一些人建议统一内存架构，如 48GB 的 M5 MacBook Pro，作为成本效益的折中方案。

**标签**: `#LLM`, `#local inference`, `#hardware`, `#GPU`, `#cost`

---

<a id="item-4"></a>
## [Current AI 发布开源 AI 差距地图](https://simonwillison.net/2026/Jul/3/open-source-ai-gap-map/#atom-everything) ⭐️ 8.0/10

非营利组织 Current AI（2025 年成立）发布了开源 AI 差距地图 v0.1，收录了来自 228 个组织的 421 个开源 AI 产品，包括 266 个软件工具、85 个模型、50 个数据集和 20 个硬件项目。 该地图提供了对开源 AI 生态系统的关键可见性，帮助开发者和组织识别差距和资源。它获得了 4 亿美元的承诺资金支持，表明对开源 AI 的强力支持。 底层数据以 MIT 许可证在 GitHub 上发布，包含 1,184 个 YAML 文件和脚本。此外，该项目跟踪了 16,185 个 GitHub 仓库，可通过 Datasette Lite 进行探索。

rss · Simon Willison · 7月3日 22:04

**背景**: Current AI 是一个全球非营利合作伙伴关系，于 2025 年在巴黎人工智能行动峰会上启动，旨在构建人工智能的公共选项。差距地图将开源 AI 产品分为三个层面：模型组件、产品/用户体验和基础设施，共 14 个类别。该项目还包括 24,400 个未分类的长尾工件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jul/3/open-source-ai-gap-map/">Open Source AI Gap Map | Simon Willison’s Weblog</a></li>

</ul>
</details>

**标签**: `#open source`, `#AI`, `#ecosystem mapping`, `#non-profit`, `#tools`

---

<a id="item-5"></a>
## [Josh Comeau 报告课程销量因 AI 下降 50% 以上](https://simonwillison.net/2026/Jul/3/josh-w-comeau/#atom-everything) ⭐️ 8.0/10

Josh W. Comeau 报告称，他的第三门课程销量仅为正常水平的约三分之一，现有课程销售额较去年下降 50% 以上。 这凸显了开发者教育市场的重大转变：AI 导致的就业不确定性和 LLM 作为免费辅导工具的普及，减少了对付费课程的需求，威胁到独立课程创作者的生计。 Comeau 指出，许多人因担心开发者工作可能很快消失而不愿投入时间和金钱学习新技能；即使他们想学习，LLM 也能提供个性化辅导，从而降低了购买付费课程的动机。

rss · Simon Willison · 7月3日 21:25

**背景**: Josh W. Comeau 是 Web 开发社区知名教育者，制作了广受欢迎的 CSS 和 React 互动课程。像 ChatGPT 这样的大型语言模型（LLM）的兴起，使学习者能够获得即时、个性化的答案，可能取代传统的在线课程。这一转变正在影响许多此前依赖广告收入或课程销售的内容创作者。

**标签**: `#AI`, `#Online Education`, `#Developer Economy`, `#LLMs`, `#Course Creation`

---

<a id="item-6"></a>
## [针对开放权重模型，微调抵抗是否有意义？](https://www.reddit.com/r/MachineLearning/comments/1um9bs7/what_does_safe_ai_look_like_d/) ⭐️ 8.0/10

Reddit 上的一场讨论质疑了研究防御开放权重大语言模型在发布后因微调而削弱安全行为的意义，认为有决心的用户可以轻易绕过这些防御措施。 这场辩论凸显了 AI 安全中的一个根本挑战：如果安全训练可以被轻易解除，那么对开放权重模型进行安全训练是否值得，这将影响模型发布策略和治理。 该帖子特别指出，新模型的‘无审查’变体很快出现，并询问即使无法完美预防，增加攻击者成本或使安全移除变得不那么可靠是否有价值。

reddit · r/MachineLearning · /u/Aaron_Rock · 7月3日 09:07

**背景**: 开放权重大语言模型（LLMs）的参数公开可用，任何人都可以对它们进行微调。安全对齐（如拒绝行为）可能通过微调被削弱，即使使用无害数据。研究表明，‘LLM 的拒绝行为由一个单一方向介导’，这表明安全机制可能脆弱且容易被移除。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/your-llms-safety-guardrails-hang-single-thread-avinash-dubey-nvbtc">Your LLM's Safety Guardrails? They Hang by a Single Thread.</a></li>
<li><a href="https://arxiv.org/abs/2601.10141">[2601.10141] Understanding and Preserving Safety in Fine-Tuned LLMs</a></li>
<li><a href="https://arxiv.org/pdf/2409.18169">Harmful Fine-tuning Attacks and Defenses for Large Language Models: A Survey</a></li>

</ul>
</details>

**社区讨论**: 新闻中没有提供社区评论；但帖子本身邀请讨论威胁模型和实际收益，可能引发关于微调抵抗效用的不同观点。

**标签**: `#AI Safety`, `#Large Language Models`, `#Fine-tuning`, `#Open-source`, `#Model Governance`

---

<a id="item-7"></a>
## [Costco：反亚马逊的零售模式](https://phenomenalworld.org/analysis/the-anti-amazon/) ⭐️ 7.0/10

文章分析了 Costco 的仓储模式如何刻意避免亚马逊家庭配送系统的物流复杂性，引发了关于工程和商业哲学的深入讨论。 这很重要，因为它凸显了零售物流和商业模式中的基本权衡，为工程师和商业策略师提供了宝贵的见解。 Costco 采用会员制仓储模式，顾客亲自开车到店并自行运输商品，避免了“最后一英里”配送问题。该文章评分 7.0/10，并有 230 条评论。

hackernews · bookofjoe · 7月3日 15:14 · [社区讨论](https://news.ycombinator.com/item?id=48776044)

**背景**: Costco 是一家仅限会员的仓储式量贩店，以低价销售大包装商品，依赖顾客自行运输而非送货上门。相比之下，亚马逊专注于单个商品的家庭配送，需要复杂的物流体系。文章对比了这两种零售模式，探讨它们各自的权衡。

**社区讨论**: 评论扩展了文章观点：gwbas1c 讨论了个人驾车与配送卡车之间的成本结构差异；Backslasher 引用了一句关于智者避开问题的谚语；pupppet 称赞 Costco 是美国伟大的象征；khurs 提供了英国视角，提及会员资格和非食品商品；furyofantares 指出 Costco 也通过 Instacart 提供当日配送，部分反驳了文章论点。

**标签**: `#business-models`, `#logistics`, `#retail`, `#engineering-philosophy`

---

<a id="item-8"></a>
## [工厂也可以只是一个房间](https://interconnected.org/home/2026/07/03/factories) ⭐️ 7.0/10

interconnected.org 上的一篇文章探讨了工厂可以简化成一个房间的理念，引发了社区关于制造本质的讨论。 这一观点挑战了关于制造所需复杂性和规模的现代假设，可能激发更易获得和本地化的生产。 该文章评分 7.0/10，参与度高（175 分，72 条评论），包含读者关于小规模制造亲身经历的个人轶事。

hackernews · arbesman · 7月3日 15:13 · [社区讨论](https://news.ycombinator.com/item?id=48776035)

**背景**: “工厂”的概念通常让人联想到大型自动化流水线。然而，文章认为，工厂的核心只是一个人们制造东西的空间，可以简单到一个房间。这与创客运动和小规模制造的理念一致。

**社区讨论**: 评论反映了怀旧和实践洞察的混合。ChuckMcM 指出我们与“你可以做到”的心态渐行渐远，而 rm445 分享了一个采用最简工厂方法的公司难以为继的警示故事。simonbarker87 深情回忆经营小工厂的经历，legitster 则将快餐厨房比作高效的工厂。

**标签**: `#manufacturing`, `#makers`, `#philosophy`, `#technology`, `#simplicity`

---

<a id="item-9"></a>
## [llm-coding-agent 0.1a0：编码助手的早期 Alpha 版本](https://simonwillison.net/2026/Jul/2/llm-coding-agent/#atom-everything) ⭐️ 7.0/10

Simon Willison 发布了 llm-coding-agent 的 0.1a0 版本，这是一个基于他的 LLM 库构建的早期 alpha 编码助手。它使用 Anthropic 的 Claude Code 开发，提供了读取、编辑文件和执行命令的工具。 此版本展示了 Simon Willison 的 LLM 库如何演变为一个代理框架，使得创建实用的编码助手成为可能。它降低了开发者使用熟悉的 Python CLI 尝试 AI 辅助编码工作流的门槛。 该代理实现了五个工具：edit_file、execute_command、list_files、read_file 和 search_files。用户可以通过 `uvx --prerelease=allow --with llm-coding-agent llm code` 运行它，并且它支持带有 CodingAgent 类的 Python API。

rss · Simon Willison · 7月2日 19:33

**背景**: Simon Willison 的 LLM 库是一个 CLI 工具和 Python 库，用于访问来自多个提供商的的大型语言模型。它最近演变为支持代理能力。Claude Code 是 Anthropic 的代理编码工具，可以读取代码库、编辑文件和运行命令。此版本是结合这些技术的早期实验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/simonw/llm">GitHub - simonw/llm: Access large language models from the command-line · GitHub</a></li>
<li><a href="https://code.claude.com/docs/en/overview">Overview - Claude Code Docs</a></li>

</ul>
</details>

**标签**: `#coding agent`, `#LLM`, `#Python`, `#agent framework`

---

<a id="item-10"></a>
## [理解以参与：避免 AI 代理带来的认知负债](https://simonwillison.net/2026/Jul/2/understand-to-participate/#atom-everything) ⭐️ 7.0/10

Geoffrey Litt 在 AIE 大会上提出了“理解以参与”的概念，认为开发者必须保持对代码的深入理解，以避免在与编码代理协作时产生认知负债。 这一观点凸显了随着 AI 编码代理能力增强而日益凸显的挑战：开发者可能失去流畅性以及积极参与项目的能力，导致长期脆弱性。它强调了需要在人机协作中保持开发者的自主权和代码理解能力。 Litt 在 AIE 上的演讲是 300 多场录制会议之一，Twitter 上有其演讲的线程版。认知负债指的是开发者对代码的理解与代码实际状态之间日益扩大的差距，尤其在 AI 生成大规模变更时更为明显。

rss · Simon Willison · 7月2日 17:07

**背景**: 认知负债是一个术语，用于描述当开发者缺乏对代码（尤其是 AI 生成的代码）的清晰理解时积累的精神负担，这使得维护和改进软件变得更加困难。编码代理是能够自主编写、重构和调试代码的 AI 助手，在软件开发中越来越常用。挑战在于利用这些工具的同时，不牺牲开发者推理和指导代码库的能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mathiesen.dev/writing/cognitive-debt">Cognitive Debt | Jarle Mathiesen</a></li>
<li><a href="https://www.artofsm.art/t/feeling-lost-in-your-codebase-5-tips-to-tackle-ai-induced-cognitive-debt/16929">Feeling lost in your codebase? 5 tips to tackle AI-induced cognitive debt</a></li>

</ul>
</details>

**标签**: `#AI-assisted coding`, `#cognitive debt`, `#human-AI collaboration`, `#software development`

---

<a id="item-11"></a>
## [H64LM：基于 PyTorch 从零构建的 2.49 亿参数混合专家 Transformer](https://www.reddit.com/r/MachineLearning/comments/1umqfd2/h64lm_a_249mparameter_mixtureofexperts/) ⭐️ 7.0/10

一位开发者从零使用 PyTorch 构建了 H64LM，一个 2.49 亿参数的混合专家（MoE）Transformer，实现了注意力机制、MoE 路由和训练循环等核心组件，未依赖高级框架。该模型采用分组查询注意力、8 个专家和 Top-2 路由，并包含辅助路由损失。 该项目通过提供现代技术（如 MoE、GQA 和 SwiGLU）的动手实现，为理解 LLM 内部机制提供了教育资源。它帮助学习者在理论和实践之间架起桥梁，而不依赖黑盒框架。 该模型在 WikiText-103 子集上验证，最佳验证困惑度约 40.5，但在第 10 个 epoch 后过拟合。已知局限包括仅支持 batch size 为 1 的生成，以及使用 DataParallel 而非真正的 DDP。

reddit · r/MachineLearning · /u/Loose_Literature6090 · 7月3日 21:18

**背景**: Transformer 是一种使用自注意力机制处理序列数据的神经网络架构，是现代 LLM 的基础。混合专家（MoE）通过将输入路由到不同的“专家”子网络来提高模型容量，而分组查询注意力（GQA）通过跨查询组共享键值头来平衡效率和质量。SwiGLU 是 LLaMA 等模型中使用的激活函数，结合了 Swish 和门控线性单元，可能提升性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Grouped-query_attention">Grouped-query attention</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://medium.com/@s_boudefel/exploring-swiglu-the-activation-function-powering-modern-llms-9697f88221e7">Exploring SwiGLU : The Activation Function Powering Modern LLMs | by Selssabil | Medium</a></li>

</ul>
</details>

**标签**: `#Transformer`, `#Mixture-of-Experts`, `#PyTorch`, `#LLM`, `#Deep Learning`

---

<a id="item-12"></a>
## [博士生寻求提升机器学习数学基础的书籍推荐](https://www.reddit.com/r/MachineLearning/comments/1ulmy9g/booksresources_to_improve_mathematical/) ⭐️ 7.0/10

一名机器学习方向的中后期博士生在 Reddit 上发帖，请求推荐书籍和资源以加强其在线性代数、概率论和泛函分析方面的数学基础。 这凸显了机器学习研究人员中一个常见挑战：他们往往边学边用数学，需要夯实基础以进行更深入的研究。该帖子及其评论可以为许多处于类似情况的人提供精选资源。 该学生特别提到考虑使用《Linear Algebra Done Right》学习线性代数，使用《A Primer on RKHS》学习泛函分析，并寻求概率论和其他泛函分析资源的推荐。他们还提到了 Pat Kidger 的 'Just-Know-Stuff' 列表作为潜在指南。

reddit · r/MachineLearning · /u/mvreich · 7月2日 16:24

**背景**: 扎实的数学基础对于推进机器学习研究至关重要，尤其是在核方法和统计学习理论等领域。再生核希尔伯特空间 (RKHS) 是泛函分析中的一个关键概念，广泛应用于许多机器学习算法。书籍和在线讲座等资源可以帮助研究人员填补知识空白。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Reproducing_kernel_Hilbert_space">Reproducing kernel Hilbert space - Wikipedia</a></li>
<li><a href="https://jonathan-hui.medium.com/reproducing-kernel-hilbert-space-for-machine-learning-8de67b6b5377">Reproducing Kernel Hilbert Space for Machine Learning | by Jonathan Hui | Medium</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#mathematics`, `#linear algebra`, `#probability theory`, `#functional analysis`

---

<a id="item-13"></a>
## [让 AI 代理自行判断以降低成本](https://simonwillison.net/2026/Jul/3/judgement/#atom-everything) ⭐️ 6.0/10

这种方法显著降低了 AI 编码助手的令牌消耗和成本，使其在日常使用中更加经济。它将优化负担从手动提示工程转移到模型自身的判断上，从而能更好地适应各种任务。 Simon Willison 在 Claude Code 中使用了提示词“对于所有编码任务，请自行判断并选择合适的低功耗模型在子代理中运行”，这创建了一个记忆文件，规定了何时将工作委托给 Sonnet 或 Haiku 模型。初步结果显示 Fable 的令牌消耗明显放缓。

rss · Simon Willison · 7月3日 18:51

**背景**: Claude Code 是 Anthropic 开发的 AI 编码助手，使用 Fable 等高能力大语言模型帮助开发者编写和编辑代码。它按令牌收费，对于每个任务都使用顶级模型很快就会变得昂贵。将简单的编码任务委托给更小、更便宜的模型（如 Sonnet 或 Haiku）是一种已知的优化策略，但传统上需要手动配置。这个技巧利用模型自身的判断来自动化这种委托。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://navant.github.io/posts/claude-code-token-optimisation-cheat-sheet/">Claude Code – Token Optimisation Cheat Sheet | techaways</a></li>

</ul>
</details>

**标签**: `#AI`, `#coding assistants`, `#Claude Code`, `#agent workflows`, `#optimization`

---

<a id="item-14"></a>
## [使用 DSPy 优化 Datasette Agent 的 SQL 提示](https://simonwillison.net/2026/Jul/2/dspy-datasette-agent-prompts/#atom-everything) ⭐️ 6.0/10

Simon Willison 使用 DSPy 框架评估并改进了 Datasette Agent 的 SQL 查询生成系统提示，发现了因缺少模式细节导致的列名猜测等具体问题。 这展示了一种实用的自动化提示优化方法，可提升生成可执行 SQL 的 AI 工具的可靠性，并减少易出错的手动调优。 Fable 5 使用 GPT-4.1 mini 和 nano，建议在模式列表中包含列名，并软化避免调用 describe_table 的建议，以防止错误的列猜测和重试循环。

rss · Simon Willison · 7月2日 18:25

**背景**: DSPy 是斯坦福 NLP 团队开发的开源 Python 框架，允许开发者以声明式方式编程 LLM，通过评估驱动循环优化提示。Datasette Agent 是 Datasette 的 AI 助手，能够自动编写并运行 SQL 查询以回答用户的数据问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/DSPy">DSPy</a></li>
<li><a href="https://agent.datasette.io/">Datasette Agent : an AI assistant for Datasette to help explore and...</a></li>
<li><a href="https://github.com/datasette/datasette-agent">GitHub - datasette / datasette - agent : An LLM-powered agent for...</a></li>

</ul>
</details>

**标签**: `#DSPy`, `#Datasette Agent`, `#prompt engineering`, `#SQL`, `#AI agents`

---

<a id="item-15"></a>
## [机器学习顶会如何评选最佳论文、口头报告和亮点展示](https://www.reddit.com/r/MachineLearning/comments/1ulnstb/how_papers_are_selected_for_best_paper_oral_or/) ⭐️ 6.0/10

一位 Reddit 用户发帖详细询问机器学习顶会（如 CVPR、NeurIPS）评选最佳论文、口头报告和亮点展示的流程，引发了社区关于领域主席、高级领域主席和奖项委员会角色的讨论。 了解评选标准和流程有助于研究人员优化投稿策略，并对顶级会议的认可形成合理预期，这对职业发展至关重要。 流程通常涉及领域主席、高级领域主席和一个单独的奖项委员会；决策基于评审分数、创新性和讨论，通常依据评审版本而非最终定稿。

reddit · r/MachineLearning · /u/National-Resident244 · 7月2日 16:55

**背景**: 在 NeurIPS 和 CVPR 等会议上，论文首先由多位评审人评审。领域主席（AC）监督评审并推荐决定。高级领域主席（SAC）处理冲突并最终确定接受/拒绝。对于特殊称号，奖项委员会或项目主席从高分论文中评选，通常经过额外讨论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://neurips.cc/Conferences/2025/SAC-Guidelines">NeurIPS 2025 SAC Guidelines</a></li>
<li><a href="https://cvpr.thecvf.com/Conferences/2026/SACGuides">CVPR 2026 SAC Guide</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#conferences`, `#paper selection`, `#CVPR`, `#NeurIPS`

---