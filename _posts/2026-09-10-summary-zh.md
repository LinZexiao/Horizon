---
layout: default
title: "Horizon Summary: 2026-09-10 (ZH)"
date: 2026-09-10
lang: zh
---

> 从 27 条内容中筛选出 13 条重要资讯。

---

1. [Calif Research 演示 WeWorm：AI 打造的微信通话零点击蠕虫](#item-1) ⭐️ 9.0/10
2. [OpenAI 宣称解决纳维-斯托克斯千年难题，却陷入优先权争议](#item-2) ⭐️ 9.0/10
3. [Shopify 将移动应用从 React Native 迁回 Swift 与 Kotlin 原生开发](#item-3) ⭐️ 8.0/10
4. [Forgejo 16.0.4 修复 16.0.3 及之前版本的严重远程代码执行漏洞](#item-4) ⭐️ 8.0/10
5. [微软将 Rust 提升为一级（Tier-1）语言](#item-5) ⭐️ 8.0/10
6. [布朗大学报告：硅谷正在改造军工复合体](#item-6) ⭐️ 8.0/10
7. [陶哲轩警告：AI 正在把数学开放问题当作不可再生资源开采](#item-7) ⭐️ 8.0/10
8. [Cognition 发布 SWE-2 编程模型，宣称以更低成本逼近前沿水平](#item-8) ⭐️ 7.0/10
9. [NASA 为火星研发的色彩处理技术被用于揭示地球上的褪色岩画](#item-9) ⭐️ 7.0/10
10. [PlanetScale 推出分片式 Postgres 产品 Neki，引发激烈争论](#item-10) ⭐️ 7.0/10
11. [348M 参数模型用 227 亿 token 训练，可完成 14 位数算术](#item-11) ⭐️ 7.0/10
12. [果蝇连接组学不会打乒乓，而审计过程才是真正的看点](#item-12) ⭐️ 7.0/10
13. [Sante 在 DiagnosisArena-MCQ 的 83.83 分只衡量选项选择能力](#item-13) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Calif Research 演示 WeWorm：AI 打造的微信通话零点击蠕虫](https://simonwillison.net/2026/Sep/10/calif-research/) ⭐️ 9.0/10

Calif Research 发布了一款名为 WeWorm 的演示程序，并称这是首个通过微信通话在 iOS 和 Android 上传播的零点击蠕虫。该团队表示，他们借助 AI 在约两天内找到了底层漏洞并写出首个远程代码执行（RCE）利用程序，随后又花了大约一周时间把它做成可自我传播的蠕虫。 如果这一说法成立，它同时在两个方面构成重要里程碑：一是针对一个用户规模远超十亿的通讯平台发起零点击、可自我传播的攻击；二是证明了 AI 辅助能把过去需要较大团队耗时数月完成的漏洞利用开发压缩到几天之内。这表明 AI 加速的漏洞发现与利用正从猜测走向实际可演示的能力，平台厂商不得不加快修补节奏，防守方也必须适应更短的攻击时间窗口。 根据该公告，受害者无需接听电话，也无需对手机做任何操作；即使接听，也只会听到一片安静，而漏洞利用依然成功——这是通话与消息处理栈中零点击漏洞的典型特征。该发布被明确描述为演示（demo）而非完整武器化版本，且未提及受影响的版本、CVE 编号或补丁信息，因此仅凭所引用的内容，这一说法尚未得到独立验证。

rss · Simon Willison · 9月10日 00:56

**背景**: 零点击漏洞利用是一类无需用户任何交互（例如点击链接或打开文件）即可入侵设备的攻击，因此比普通的钓鱼式攻击更难被发现和防御。微信由腾讯运营，是全球最大的即时通讯平台之一，其通话功能与其他 VoIP 及消息处理栈一样，会自动处理来自网络的数据，因而成为高价值攻击目标。AI 辅助漏洞发现利用机器学习和大型语言模型以人类难以企及的规模和速度扫描代码、依赖项与配置中的弱点；安全研究者越来越多地警告，这类能力不仅有利于防守方，也同样让攻击者受益。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.kaspersky.com/resource-center/definitions/what-is-zero-click-malware">Zero-Click Exploits - Kaspersky</a></li>
<li><a href="https://www.vulncheck.com/blog/ai-assisted-vulnerability-discovery?trk=article-ssr-frontend-pulse_little-text-block">The First CVE Wave: Signs That AI - Assisted Vulnerability Discovery ...</a></li>

</ul>
</details>

**标签**: `#ai-security-research`, `#cybersecurity`, `#malware`, `#zero-click-exploit`, `#WeChat`

---

<a id="item-2"></a>
## [OpenAI 宣称解决纳维-斯托克斯千年难题，却陷入优先权争议](https://simonwillison.net/2026/Sep/8/on-navier-stokes/) ⭐️ 9.0/10

2026 年 9 月 8 日，OpenAI 宣布其未发布的内部模型以约一万个智能体组成的集群，给出了纳维-斯托克斯存在性与光滑性问题的反例，并借助名为 GPT-6 Astra 的模型完成了 Lean 形式化验证；纳维-斯托克斯问题是七个千年大奖难题之一。但这一声明被优先权争议所笼罩：纽约大学数学家 Tristan Buckmaster 称他与 Anthropic 员工 Levent Alpöge 在近一年的工作后已于 8 月 15 日取得密切相关的结果（其间大量使用 Claude 与 Codex），而 OpenAI 是在得知他们的进展后才启动相应工作的。 如果该结果得到验证，这将是首次在 AI 深度参与下解决千年大奖难题，可能标志着数学研究范式的转变，也是对大规模智能体式 AI 用于科研的一次重大验证。同时，它把研究伦理、署名归属和训练数据来源等问题推到 AI 科研争论的中心，尤其是这场争议背后还有 Anthropic 与 OpenAI 的竞争关系。 OpenAI 称工作于 9 月 1 日启动，智能体在约 88 小时后的 9 月 5 日得出结果，Lean 形式化与验证又花费了 17 小时；仅在纳维-斯托克斯问题上，智能体就发送了 270 万条消息、消耗约 1300 亿输出 token（所有尝试过的问题合计 490 万条消息、3000 亿输出 token，按 GPT-6 Astra 的公开 API 价格计算约需 1500 万美元）。该反例尚未经外部数学家或克雷数学研究所验证，OpenAI 也表示不会申领 100 万美元奖金；据称所用方法建立在 Diego Córdoba 与 Luis Martínez-Zoroa 于 2023 年提出的爆破（blowup）技术之上。

rss · Simon Willison · 9月8日 23:55

**背景**: 纳维-斯托克斯方程是一组描述流体运动的偏微分方程；尽管它们在无数工程计算中被成功使用，但人们仍无法从解析上完全理解三维空间与时间中是否总存在光滑解，这一问题常与湍流联系在一起。2000 年，克雷数学研究所将“存在性与光滑性”问题列为七个千年大奖难题之一，每题对正确解答悬赏 100 万美元。目前唯一被官方解决的千年难题是庞加莱猜想，由格里戈里·佩雷尔曼解决，而他在 2010 年拒绝了该奖。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Navier-Stokes_existence_and_smoothness_problem">Navier-Stokes existence and smoothness problem</a></li>
<li><a href="https://en.wikipedia.org/wiki/Millennium_Prize_Problems">Millennium Prize Problems</a></li>
<li><a href="https://www.claymath.org/millennium-problems/">The Millennium Prize Problems - Clay Mathematics Institute</a></li>

</ul>
</details>

**社区讨论**: 评论区总体持怀疑态度：有人认为这就像一位人类合作者未经署名便发表基于研究者想法的成果，属于严重不道德；也有人主张两种情况可以并存——模型既可能把聊天数据吸收进潜在表示，也可能通过大规模可验证数学的强化学习发现真正新颖的技巧。还有人指出，在听说重大证明的传闻后立刻用一个仍在训练中的模型生成 3000 亿输出 token，时机令人生疑，感觉像是“平行构建”，尽管他们承认每一步单独看都有合理解释。

**标签**: `#AI-for-Mathematics`, `#Navier-Stokes`, `#Millennium-Prize`, `#OpenAI`, `#Research-Integrity`

---

<a id="item-3"></a>
## [Shopify 将移动应用从 React Native 迁回 Swift 与 Kotlin 原生开发](https://shopify.engineering/back-to-native) ⭐️ 8.0/10

Shopify 发布了一篇工程博客文章，宣布其移动应用将从 React Native 迁回完全原生的 iOS（Swift）与 Android（Kotlin）代码库。该消息在 Hacker News 上引发热议（651 分、437 条评论），讨论很快从这一单点决策扩展到 AI 生成代码时代“原生开发 vs 跨平台开发”的范式之争。 Shopify 是 React Native 最大的公开使用方之一，因此它的“回头”是一个颇具分量的行业信号，会被其他正在评估跨平台框架的公司拿来参考。讨论还显示，这一决策背后是更广泛的重新权衡：当 AI 代码生成让编写原生 Swift 和 Kotlin 的成本大幅下降时，React Native 原本“让 Web 开发者也能写移动应用”的核心优势正在被削弱。 这只是一家公司的工程决策，而非整个领域的突破，且原文本身并未给出具体的性能基准或迁移时间表。具体的数据点来自评论区：有开发者称借助 Codex 和 Maestro 测试工具，几乎在一夜之间就把一个 15 到 20 个页面的应用移植到了 iOS 和 Android 两端，随后又花几天时间做打磨完善。

hackernews · fnthawar2 · 9月10日 14:09 · [社区讨论](https://news.ycombinator.com/item?id=49643982)

**背景**: React Native 是 Meta（当时的 Facebook）推出的开源 UI 框架，允许开发者用 JavaScript/React 编写移动应用，同时仍以原生平台组件渲染界面；它支持 iOS、Android 等多个目标平台，Meta、微软和 Shopify 都曾使用它。它长期以来的卖点是代码复用——一套代码库，或者说一支 Web 开发团队，同时覆盖两大移动平台。Swift 是苹果用于 iOS/macOS 开发的编程语言，Kotlin 则是谷歌主推的 Android 开发语言，因此迁回原生意味着需要同时维护两套各自独立的平台代码库。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/React_Native">React Native</a></li>
<li><a href="https://reactnative.dev/">React Native</a></li>

</ul>
</details>

**社区讨论**: 评论整体情绪偏中性，主流观点是“视情况而定”。一条高赞评论把它描述为一条光谱：每家公司都处在某条分界线的两侧之一，一侧适合 Electron/React Native，另一侧则不适合，这只是一个在资源受限条件下的工程权衡，而非好坏分明的绝对判断。也有人认为，既然 AI 模型现在已能较好地生成原生 iOS/Android 代码，React Native“借用 Web 开发者”的理由基本不复存在；另有评论者分享了自己用 Codex 和 Maestro 一夜之间完成整个应用移植的一手经历；还有人对仅仅为了查询包裹就被迫下载 Shop 应用表达了用户角度的不满。

**标签**: `#React Native`, `#iOS/Android Native`, `#Mobile Engineering`, `#Cross-Platform Development`, `#AI Code Generation`

---

<a id="item-4"></a>
## [Forgejo 16.0.4 修复 16.0.3 及之前版本的严重远程代码执行漏洞](https://codeberg.org/forgejo/forgejo/src/branch/forgejo/release-notes-published/16.0.4.md) ⭐️ 8.0/10

Forgejo 发布了 16.0.4 版本，修复了一个影响 16.0.3 及更早版本的严重远程代码执行（RCE）漏洞。该修复对应 PR 14301，用于防止在基于模板仓库生成新仓库时，模板变量展开过程干扰 git 仓库初始化。 Forgejo 是被广泛使用的自托管 Git 代码托管平台，因此任何 RCE 漏洞都会使大量自管理实例及其代码面临风险，管理员应尽快升级。此次披露也凸显了 Forgejo 与其同源的 Gitea 之间的安全态势差异——Gitea 项目领导层表示其不受这两个问题影响。 该漏洞在从模板生成仓库的过程中被触发：Forgejo 会克隆模板仓库、删除 .git 目录、对 .forgejo/template 中列出的文件执行变量模板展开，然后重新初始化一个新的 git 仓库——此次修复对这一流程进行了加固。16.0.4 的发布说明包含两项安全修复，而 Codeberg 的访问速率限制一度导致说明页面难以打开，社区成员因此转贴了具体内容。

hackernews · weierstass · 9月10日 15:57 · [社区讨论](https://news.ycombinator.com/item?id=49645907)

**背景**: Forgejo 是用 Go 编写的开源自托管软件协同开发平台（forge），提供 Git 仓库托管以及问题跟踪、代码审查、Wiki 和 CI 等功能，由 Codeberg e.V. 治理，也是 Codeberg.org 背后的软件。Forgejo 最初是 Gitea 的社区治理分支，而 Gitea 本身又是 Gogs 的分支，因此两个项目共享大量代码，并经常被拿来比较安全状况。远程代码执行漏洞属于最严重的一类缺陷，因为攻击者可以在服务器上运行任意代码，而不仅仅是读取或篡改数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Forgejo">Forgejo</a></li>
<li><a href="https://forgejo.org/">Forgejo – Beyond coding. We forge.</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gitea">Gitea</a></li>

</ul>
</details>

**社区讨论**: 有评论者指出 Codeberg 的速率限制导致官方发布说明无法打开，并替其他人转贴了这两项修复内容。Gitea 项目领导层澄清 Gitea 对这两个问题均已具备防护，同时提醒不应指责报告安全问题的人；也有评论者认为，Forgejo 禁止 LLM 贡献的决定可能使其处于劣势，因为攻击者仍会利用 AI 来寻找漏洞。

**标签**: `#security`, `#vulnerability`, `#forgejo`, `#gitea`, `#self-hosted`

---

<a id="item-5"></a>
## [微软将 Rust 提升为一级（Tier-1）语言](https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/) ⭐️ 8.0/10

这是全球最大软件厂商之一对 Rust 的重要行业背书，也意味着所有同时在 C 和 C++ 工具链上有话语权的主流操作系统厂商，如今都为新项目的系统编程语言做了多元化布局。这也会进一步推动内存安全的行业趋势——微软此前曾表示，过去十年其产品漏洞中约 70% 属于 Rust 旨在消除的内存安全问题。 据社区讨论，最具体的技术消息是微软已将 Rust 工具链从 LLVM 切换到 MSVC 后端，使此前流传已久的 MSVC 集成传闻正式公开；但除"一级语言"这一认定外，官方披露的细节仍然有限。评论者还提到微软宣称的目标：到 2030 年借助自动化工具把 10 亿行代码转换为 Rust，宣传口径是"1 名工程师、1 个月、100 万行代码"，而这一目标的可行性受到广泛质疑。

hackernews · mmastrac · 9月10日 13:39 · [社区讨论](https://news.ycombinator.com/item?id=49643546)

**背景**: Rust 是一门系统级编程语言，最初由 Mozilla 创建，现由独立的 Rust 基金会维护，其最突出的特点是编译期内存安全：通过所有权和借用规则，无需垃圾回收即可避免缓冲区溢出、悬空指针等一整类缺陷。这里的"一级（Tier-1）"是微软内部的工程评级，用来描述某门语言在公司的构建、工具链和合规流程中受支持的程度，并非公开发布的产品。其背景是近年来政府与产业界共同推动的"远离 C/C++"运动——包括 2025 年 CISA 与 NSA 联合发布的内存安全语言指南——因为 C/C++ 不强制内存安全，是大量安全漏洞的根源。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/">Guest Post: Rust Is Tier-1 Language at Microsoft</a></li>
<li><a href="https://www.memorysafety.org/docs/memory-safety/">What is memory safety and why does it matter? - Prossimo Memory Safe Languages: Reducing Vulnerabilities in Modern ... Memory Safety: An Explainer - Center for Security and ... Memory Safe Languages: Reducing Vulnerabilities in Modern ... An Introduction to Memory Safety Concepts and Challenges Software Memory Safety</a></li>
<li><a href="https://www.cisa.gov/resources-tools/resources/memory-safe-languages-reducing-vulnerabilities-modern-software-development">Memory Safe Languages: Reducing Vulnerabilities in Modern ...</a></li>

</ul>
</details>

**社区讨论**: 整体情绪非常正面：评论者认为这表明 Rust 不再是"快速迭代、随时搞坏东西"的新生语言，而是能与 C++、C# 正面竞争的成熟选择，也比 Zig、Odin 这些更新的"更好的 C/C++"方案更完善。多人指出真正的头条是切换到 MSVC 后端；也有人从内存安全漏洞和微软庞大产品组合的角度解释其战略合理性。与此同时，一些评论对自动转换 10 亿行代码的目标持怀疑态度，并批评微软一边推 Rust 一边淘汰旧 Windows 硬件的做法。

**标签**: `#Rust`, `#Microsoft`, `#Systems Programming`, `#Memory Safety`, `#Language Ecosystems`

---

<a id="item-6"></a>
## [布朗大学报告：硅谷正在改造军工复合体](https://costsofwar.watson.brown.edu/paper/how-big-tech-and-silicon-valley-are-transforming-military-industrial-complex) ⭐️ 8.0/10

布朗大学“战争成本”（Costs of War）项目发布新报告，分析大型科技公司与硅谷企业正在如何改造军工复合体，并在 Hacker News 上引发了一场多达 267 条评论的讨论。讨论中提到的要点包括：旧金山初创公司 Keyhole 在 2003 年从 CIA 背景的风投机构 In-Q-Tel 获得种子投资，据称两周内美国军方与情报机构就已用其软件支持伊拉克战争，次年谷歌收购该公司并将其改名为 Google Earth。 报告挑战了“大型科技公司涉足国防只是近年新现象”的普遍看法，把这种关系追溯到半导体产业的最早期。其意义在于：它加剧了工程师与科技从业者围绕“共谋”问题持续进行的伦理争论，同时国防合同正成为大型云计算与人工智能公司重要且不断增长的收入来源。 该报告属于政策与历史分析，而非技术发布；其具体证据之一是 In-Q-Tel 投资 Keyhole 的案例，将 CIA 的种子资金与战时软件使用联系起来。相应的 Hacker News 讨论帖多为个人经历与观点，混杂历史论证、拒绝或辞去国防相关工作的自述，因此其中的说法应视为观点而非经过核实的事实。

hackernews · paimapi · 9月10日 15:47 · [社区讨论](https://news.ycombinator.com/item?id=49645754)

**背景**: “军工复合体”一词由美国总统艾森豪威尔在 1961 年的告别演说中推广开来，用来描述一国军队与其国防供应商之间紧密甚至可能危险的关系。布朗大学沃森国际与公共事务学院下属的“战争成本”项目，专门研究 9·11 之后历次战争在人员、经济和政治层面的代价。报告提到的 In-Q-Tel 是一家成立于 1999 年、由 CIA 支持的风险投资机构，专门投资那些技术可能服务于美国情报机构的初创公司。硅谷与国防的联系可追溯到 1950 年代，当时的仙童半导体（Fairchild Semiconductor）等早期芯片厂商就为“民兵”导弹等军事系统供应集成电路。

**社区讨论**: 评论者意见分歧明显：一些人认为硅谷从一开始就依赖美国国防部的资金，并以仙童半导体和谷歌的起源为例，还反问若这些公司当年拒绝为导弹系统制造芯片，世界是否会更好；另一些人则质疑企业是否就不该承接本国国防部的合同，或这种反对是否只针对美国。一位评论者表示自己因不满微软在以色列战争罪行中的“共谋”而辞去高薪工作，呼吁科技从业者抵制军工复合体；还有多位参与者分享了报告中的有趣发现，例如 Keyhole 在被改名为 Google Earth 之前曾获得 In-Q-Tel 的种子投资。

**标签**: `#military-industrial-complex`, `#silicon-valley`, `#defense-contracts`, `#tech-ethics`, `#policy`

---

<a id="item-7"></a>
## [陶哲轩警告：AI 正在把数学开放问题当作不可再生资源开采](https://simonwillison.net/2026/Sep/9/terence-tao/) ⭐️ 8.0/10

陶哲轩（Terence Tao）在 Mastodon 上发文指出，优质且富有成果的数学开放问题正被以“不可再生”的方式开采；如今只要传出某人在研究某个问题的风声，就可能引发大量由 AI 驱动的攻关，在原研究项目尚未充分发展之前就把它“铲平”。他由此得出结论：当前的激励机制可能促使数学家不再向更广泛的学术共同体分享有前景的研究方向。 如果研究者为了避免被 AI 辅助的攻关抢先而不再公开分享有前景的方向，这将逆转数百年的开放科学传统，并可能对数学以及其他依赖公开问题清单的领域造成长期严重损害。这一警告把 AI 日益增强的数学能力重新定义为对科研社会基础设施的威胁，而不仅仅是一种生产力工具。 陶哲轩的核心观点是，开放问题就像一种不可再生资源：好的问题稀缺、产生缓慢，一旦大量参与者蜂拥而至就很容易被耗尽。值得注意的是，他表示触发这股 AI 辅助攻关浪潮的不只是实际的研究工作，甚至仅仅是某人正在研究某个问题的传闻，这意味着保密动机可能在非常早期的阶段就已出现。

rss · Simon Willison · 9月9日 00:20

**背景**: 在数学中，开放问题是整个学科共享的前沿——研究者公开提出他们认为有价值的问题与猜想，其他人再在其基础上继续推进，这一规范已推动学科发展数百年。近年来的 AI 系统在数学推理与搜索方面能力不断增强，一旦目标问题被公开，就能迅速探索与之相关的大量结果空间。陶哲轩是菲尔兹奖得主，也是研究 AI 在数学中所起作用的最有影响力的声音之一，他此前就曾撰文讨论 AI 可能耗尽可入手的开放问题供给。

**标签**: `#ai-ethics`, `#open-science`, `#mathematics`, `#research-culture`, `#ai-impact`

---

<a id="item-8"></a>
## [Cognition 发布 SWE-2 编程模型，宣称以更低成本逼近前沿水平](https://cognition.com/blog/swe-2) ⭐️ 7.0/10

打造 Devin 编程智能体的公司 Cognition 发布了 SWE-2，称其为该公司迄今最先进的编程模型。官方表示 SWE-2 在 FrontierCode 1.1 Main 1 上取得 50.0% 的成绩，距离 Fable 5.1 仅差一个百分点，而成本低 64%，在主要评测上最高可便宜 70%。 此次发布加剧了编程模型市场的竞争。Cognition 主打「单位成本的能力」而非单纯的绝对前沿性能，直接挑战 Anthropic 的 Fable 5.1 与 OpenAI 的 GPT-6 Astra。若其成本优势成立，可能会对整个企业日益依赖的智能体编程工具领域的定价形成压力。 Cognition 称其首次将强化学习扩展到数万亿参数规模，基于 SWE-1.7 的训练基础设施与配方，并说明 SWE-2 是在 Kimi K3 基础上做后训练得到的。在效率方面，SWE-2 medium 据称中位数 18 步就做出首次真正的代码修改，而 SWE-1.7 需要 48 步（此前因在简单任务上过度探索而受到用户批评）；不过该模型的评测成绩跨度很大，Terminal Bench 2.1 上为 92.8%，而 Terminal Bench 4 上仅 27.3%。

hackernews · seelos · 9月10日 15:29 · [社区讨论](https://news.ycombinator.com/item?id=49645443)

**背景**: Cognition 是以 Devin 闻名的 AI 实验室，Devin 是最早被广泛报道的自主编程智能体之一，而 SWE-2 是其 SWE-1.7 模型的继任者。FrontierCode、Terminal Bench 等基准是用于横向比较编程模型的标准测试，其中 Terminal Bench 4 是在本次发布前几周才刚刚推出的新版本。对比对象包括 Anthropic 于 2026 年 9 月发布、面向企业、拥有 100 万 token 上下文窗口的 Fable 5.1，以及 OpenAI 于 2026 年 9 月 3 日以限量预览形式亮相的 GPT-6 Astra。模型权重是否开放以及训练数据来源，已成为开源与闭源模型之争的核心争议点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cognition.com/blog/swe-2">Introducing SWE-2: Pushing the Pareto Frontier | Cognition</a></li>
<li><a href="https://llm-stats.com/models/claude-fable-5-1">Claude Fable 5.1 Benchmarks, Pricing & Context Window</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-6_Astra">GPT-6 Astra - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论者普遍持怀疑态度：最大的争议点是 SWE-2 在 Terminal Bench 2.1 上 92.8% 与 Terminal Bench 4 上 27.3% 之间的巨大落差，被解读为衡量该模型「有多会刷榜」的指标。也有人援引 Cognition 早前 Upwork 演示引发的争议，认为其性能宣称应打折扣；还有人质疑为何要选择闭源权重模型而非 DeepSeek Flash 4.1，并讨论在别家模型（Kimi K3）上做后训练的弊端。也有评论持更积极看法，认为经过强化学习调优的 K3 能达到 Fable 5 级别的能力本身就是个好兆头。

**标签**: `#AI/ML`, `#coding-agents`, `#LLM-benchmarks`, `#open-weights`, `#model-release`

---

<a id="item-9"></a>
## [NASA 为火星研发的色彩处理技术被用于揭示地球上的褪色岩画](https://gizmodo.com/this-nasa-color-trick-was-meant-for-mars-now-its-unveiling-rock-art-on-earth-2000809844) ⭐️ 7.0/10

根据 NASA Spinoff 的一篇专题报道，NASA 最初为凸显火星图像中细微色彩差异而研发的一种图像处理技术，如今被改造用于揭示地球上已经褪色的岩画。这种方法名为去相关拉伸（decorrelation stretch），目前被用于处理那些图案已褪色到几乎无法辨认的古代岩刻与岩绘照片。 这件事是航天机构技术外溢的一个典型案例：为研究另一颗行星而开发的技术，反过来服务于地球上的考古学与文化遗产保护。如果它能够稳定地凸显出微弱的颜料与矿物反差，研究人员就能以非破坏性的方式记录那些正在风化、肉眼几乎看不见的脆弱岩画。 去相关拉伸的原理是通过数学方法消除图像各颜色通道之间的相关性，并重新拉伸其方差，从而最大化色彩分离度、让微弱特征更易分辨；它通常作用于混合了可见光与红外波段的伪彩色合成图。类似效果在普通软件中也能近似实现——有评论者指出，在 GIMP 中可将图像分解为 LAB 通道，对 A/B 色度图层做自动色阶，再重新合成——不过这类激进的增强也可能放大噪点，解读时需谨慎。

hackernews · gumby · 9月10日 15:29 · [社区讨论](https://news.ycombinator.com/item?id=49645437)

**背景**: 火星轨道器和漫游车等航天器会在包括红外在内的多个波段拍摄图像，而这些波段超出了人眼的感知范围；把这些波段合成为“伪彩色”图像后，画面呈现的颜色与普通照片不同，却能暴露出真彩色下看不见的差异。去相关拉伸正是处理这类多光谱数据的标准增强算法，在 MATLAB、ENVI 和 GIMP 等工具中都有实现。岩画会因数百年的风化而褪色，因此增强微弱的颜料或矿物反差，可以让已经消失或极淡的图案重新变得可读。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Decorrelation">Decorrelation - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/False_color">False color - Wikipedia</a></li>
<li><a href="https://www.mathworks.com/help/images/enhance-color-separation-using-decorrelation-stretching.html">Enhance Color Separation Using Decorrelation Stretching</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的读者总体反应积极，有人指出报道背后的 NASA Spinoff 长文有更多细节。多位评论者贡献了实操经验：一位分享了用 LAB 通道分解加自动色阶在 GIMP 中近似实现该效果的工作流；另一位讲述了自己在吴哥窟尝试多波段滤光成像却未能成功的经历（还因使用三脚架被警卫打断）；还有人感慨伪彩色合成图改变了自己对传感的认知——毕竟“植被是红色的，不是绿色的”。

**标签**: `#remote sensing`, `#archaeology`, `#image processing`, `#false color`, `#NASA spinoff`

---

<a id="item-10"></a>
## [PlanetScale 推出分片式 Postgres 产品 Neki，引发激烈争论](https://planetscale.com/blog/introducing-neki) ⭐️ 7.0/10

PlanetScale 推出了 Neki，一款由 Vitess 团队打造的分布式、分片式 Postgres 解决方案，其发布博客在 Hacker News 上获得 187 分和 96 条评论。Neki 被定位为让分片式 Postgres 变得人人可用的产品，但 PlanetScale 目前尚未将其开源。 这一发布之所以重要，是因为 PlanetScale 是数据库基础设施领域的重要厂商，其进军分片式 Postgres 领域表明整个行业正日益推动 Postgres 突破单节点限制进行扩展。这场争议也凸显了在 Supabase 等竞争对手提供开源替代方案的市场上，开源与专有数据库工具之间的更广泛辩论。 PlanetScale 表示 Neki 目前尚未开源，但一旦准备就绪并在真实生产工作负载中经过测试，就会作为开源项目发布。评论者还提出了 CAP 定理方面的担忧，认为最终一致性不适合许多高可用 Postgres 工作负载，并追问 Neki 如何解决这些权衡问题。

hackernews · simon_weber · 9月10日 15:43 · [社区讨论](https://news.ycombinator.com/item?id=49645686)

**背景**: Postgres 是一款广泛使用的开源关系型数据库，但它最初是为单机设计的，因此将其扩展至多台服务器（即所谓分片技术）十分困难，并催生了众多分支和第三方工具。分布式数据库必须在 CAP 定理所描述的一致性、可用性和分区容错之间进行权衡，这也是评论者质疑最终一致性的分片系统是否适合其工作负载的原因。PlanetScale 此前的业务建立在 Vitess 之上——这是最初由 Google 创建、用于 MySQL 的开源分片系统，这使得 Neki 的闭源性质成为一个对比焦点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://planetscale.com/neki">Neki — PlanetScale | Sharded Postgres by the Team Behind Vitess.</a></li>
<li><a href="https://neki.dev/">Sharded Postgres by PlanetScale | Neki</a></li>
<li><a href="https://pganalyze.com/blog/5mins-distributed-postgres">The different trade-offs of Distributed Postgres architectures</a></li>

</ul>
</details>

**社区讨论**: 整体情绪明显偏批判：一条高赞评论抱怨发布文章始终没有清楚说明 Neki 究竟是什么、用途是什么，另一条评论则肯定技术但称其 CEO 表现得像个“混蛋”。多位评论者将 Neki 的闭源状态与 Supabase 开源的 Multigres 进行不利对比，还有人追问在 CAP 定理约束下，最终一致性能否满足高可用 Postgres 工作负载的需求。

**标签**: `#postgres`, `#distributed-systems`, `#databases`, `#planetscale`, `#sharding`

---

<a id="item-11"></a>
## [348M 参数模型用 227 亿 token 训练，可完成 14 位数算术](https://www.reddit.com/r/MachineLearning/comments/1wc7hmu/i_trained_a_348m_model_trained_from_scratch_on/) ⭐️ 7.0/10

一位独立开发者发布了一个从零训练、使用 227 亿 token 的 348M 参数语言模型，随后经过微调，使其通过显式写出竖式过程来完成算术运算，在 GPT-3 的九个算术子任务上平均得分 99.4%。据称该模型在多项任务上超过了 GPT-3 175B 的少样本直接作答成绩，例如 4 位数加法为 100% 对 25.5%，2 位数乘法为 100% 对 29.2%；并且在作者把固定的位值名称列表从 6 个扩展到 19 个之后，其干净的加法能力上限从 8 位提升到 14 位。 这是一个引人注目的例证：语言模型的算术能力在很大程度上取决于训练数据和输出格式，而不是参数规模本身——一个比 GPT-3 175B 小约 500 倍的模型，在被训练成写出解题过程后，可以在竖式算术上大幅胜出。这也顺应了小型、任务专用语言模型的发展趋势，并进一步说明为什么逐步推理式的思维链生成已成为推理任务的标准做法。 这些提升范围有限：该模型在 GSM8K 应用题上仅得 4%，在 ASDiv 上为 16.5%，失败主要源于运算选择而非计算本身，同时它完全不会除法，4×4 乘法也是硬性障碍。此外它必须使用贪婪解码，因为采样会在推理链中途破坏竖式流程；作者还主动指出算术评测脚本对减法操作数进行了排序，因此减法成绩表并不能反映操作数顺序任意的情况。

reddit · r/MachineLearning · /u/nkthebass · 9月10日 03:28

**背景**: GPT-3 在 2020 年的原始论文中纳入了一组算术基准（2 至 5 位数加减法以及 2 位数乘法），并在少样本设置下评测，即提示中给出少量示例，模型必须在不借助计算器的情况下直接作答。Wei 等人在 2022 年提出的思维链提示则要求模型在给出最终答案前先产生中间推理步骤，从而显著提升多步任务的表现。这个项目把该思路用在训练阶段——用带进位和借位的竖式算术对模型进行微调——而不仅仅停留在提示层面；它同时表明分词与词表设计（例如每个数位是否有对应名称）可能在不被察觉的情况下限制模型的数值处理范围。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.promptingguide.ai/techniques/cot">Chain-of-Thought Prompting | Prompt Engineering Guide</a></li>
<li><a href="https://github.com/openai/gpt-3">GitHub - openai/gpt-3: GPT-3: Language Models are Few-Shot Learners · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Few-shot_learning">Few-shot learning</a></li>

</ul>
</details>

**标签**: `#small language models`, `#arithmetic reasoning`, `#chain-of-thought`, `#model training`, `#benchmarks`

---

<a id="item-12"></a>
## [果蝇连接组学不会打乒乓，而审计过程才是真正的看点](https://www.reddit.com/r/MachineLearning/comments/1wc67ci/i_tried_to_make_a_real_fly_connectome_learn_to/) ⭐️ 7.0/10

一位研究者尝试用多巴胺式可塑性，让新发布的 MaleCNS v1.0 果蝇连接组（基于真实电子显微镜重建的 16.6 万个神经元）的一小段真实子图学会打乒乓球，结果它根本没学会。对失败原因做审计后发现：一个 neuPrint 正则表达式 bug 静默地把两个完整神经元群体清零；最初的神经元选择中根本没有从光感受器通往下游的路径；四个运动神经元里有一半与任何感觉通路之间的突触数为零。 在一个被病毒式演示视频主导的领域里，这是一份罕见且有据可查的负面结果，它暗示若干高调的“果蝇大脑玩 Doom/Minecraft/Beat Saber”项目其实并未通过它们自己的验证门槛。它对计算神经科学和机器学习可复现性都有意义，因为这说明真正能区分“涌现行为”与“手工注入的兜底逻辑”的，是连接性审计，而不是游戏画面。 即便在重建流程之后，开启学习与关闭学习在多组随机种子下仍给出逐位完全相同的结果，而权重在底层确实在变化——原因是四个运动神经元中有两个没有任何感觉输入，却仅凭数组下标被分到了“球拍下移”组。最终出现的学习/非学习差异看起来更像是学习规则整体把系统压制得更安静（因为未击中多于击中，惩罚信号占主导），而不是任何技能层面的提升。

reddit · r/MachineLearning · /u/oPeraza2007 · 9月10日 02:28

**背景**: 连接组是大脑中全部神经元及其相互突触连接的完整图谱；MaleCNS v1.0 是一个成年雄性果蝇中枢神经系统数据集，包含约 16.6 万个通过电子显微镜重建的神经元。neuPrint 是研究者用来检索这些神经元及其连接关系的主要查询工具与 API，因此其匹配语义中的 bug 会静默污染任何下游模拟。多巴胺式可塑性是一种受生物启发的学习规则，用奖励或惩罚信号调制突触权重；而乒乓球被选作刻意严苛的测试环境，因为它每帧只给出一个命中或未命中的二值信号。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://male-cns.janelia.org/release/">Release Notes - MaleCNS connectome</a></li>
<li><a href="https://github.com/connectome-neuprint/neuPrint">GitHub - connectome-neuprint/neuPrint: tools for importing ...</a></li>
<li><a href="https://arxiv.org/html/2512.07194v1">Synchrony-Gated Plasticity with Dopamine Modulation for Spiking Neural ...</a></li>

</ul>
</details>

**标签**: `#connectomics`, `#computational neuroscience`, `#machine learning`, `#negative results`, `#neuromorphic computing`

---

<a id="item-13"></a>
## [Sante 在 DiagnosisArena-MCQ 的 83.83 分只衡量选项选择能力](https://www.reddit.com/r/MachineLearning/comments/1wbkxsa/what_santes_8383_on_diagnosisarenamcq_actually/) ⭐️ 6.0/10

Reddit 用户 /u/Expert_Coffee_203 撰文指出，Ant Ling 为 Ling-3.0-flash-Sante 在 DiagnosisArena-MCQ 上报出的 83.83 分，只反映模型在病例信息、检查和检验结果都已给出时，从四个候选诊断中挑选一个的能力。该帖还并列了此次发布中另外两项医学结果——MedXpertQA-Text 53.88 与 HealthBench Professional 45.73——并强调这三项结果都无法证明模型能无限制地生成鉴别诊断、判断还缺哪些病史，或决定下一步该做哪项检查。 基准分数常被当作模型临床能力的头条证据来引用，因此澄清这一分数只是受限的多选题任务结果，有助于开发者和采购方在为真实诊断流程选型时避免过度解读。这一区分对病例问答类应用尤为关键，因为此类应用的首要设计决策就是：由用户提供候选诊断，还是由模型自行生成候选诊断。 帖子指出，Sante 公布的图表没有提供足够的评分细节，无法判断所报的 HealthBench Professional 数值是长度调整后的还是未调整的，因此与其他已发布的 HBP 结果作比较前应先核实这一点；此外 HealthBench Professional 由医生按评分量表打分，并非百分比准确率，其定义涵盖诊疗咨询、写作/文书与医学研究等场景。

reddit · r/MachineLearning · /u/Expert_Coffee_203 · 9月9日 13:01

**背景**: DiagnosisArena 是一个专门评估大语言模型诊断推理能力的基准，其中包含多选题变体 DiagnosisArena-MCQ，以便与传统考试式基准进行对比。Ling-3.0-flash-Sante 是 InclusionAI（蚂蚁）推出的医学领域混合专家（MoE）模型，基于 Ling-3.0-Flash 构建，总参数量 1240 亿，但每个 token 仅激活约 51 亿参数，据报道其在上述多选题基准上超过若干更大的前沿模型。MedXpertQA-Text 是 MedXpertQA 的纯文本子集，后者是包含 4460 道题、覆盖 17 个专科和 11 个身体系统的专家级医学问答基准；而 HealthBench Professional 则衡量开放式临床对话，由医生撰写的评分量表来评判。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2505.14107">DiagnosisArena : Benchmarking Diagnostic Reasoning for Large...</a></li>
<li><a href="https://novita.ai/models/model-detail/inclusionai-ling-3.0-flash-sante">Ling 3 . 0 Flash Sante API & Playground | Novita AI</a></li>
<li><a href="https://github.com/TsinghuaC3I/MedXpertQA">GitHub - TsinghuaC3I/MedXpertQA: [ICML 2025] MedXpertQA: Benchmarking Expert-Level Medical Reasoning and Understanding · GitHub</a></li>

</ul>
</details>

**标签**: `#medical-ai`, `#benchmarking`, `#evaluation-methods`, `#LLM-reasoning`, `#machine-learning`

---