---
layout: default
title: "Horizon Summary: 2026-09-25 (ZH)"
date: 2026-09-25
lang: zh
---

> 从 37 条内容中筛选出 8 条重要资讯。

---

1. [F-Droid 2.0 发布：开源 Android 应用商店迎来重大改版](#item-1) ⭐️ 9.0/10
2. [DHH 在 Rails World 2026 主题演讲：AI 时代开发者将成“创造者”](#item-2) ⭐️ 8.0/10
3. [Apple 撤下 ADP，英国 iCloud 用户被拆成两级加密](#item-3) ⭐️ 8.0/10
4. [Show HN：Bastardica 滥用 OpenType 连字把不搭的字体混在一起](#item-4) ⭐️ 7.0/10
5. [Dynomight 探讨：肝脏为何再生能力如此特殊](#item-5) ⭐️ 7.0/10
6. [Google 发布 Gemini 3.8 TTS 模型：2000+ 音色与 30 秒声音克隆](#item-6) ⭐️ 7.0/10
7. [arXiv 获 1720 万美元慈善资助，启动独立非营利组织转型](#item-7) ⭐️ 7.0/10
8. [Whiteboard（YC W26）：面向人机协作的开源可视化架构 IDE](#item-8) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [F-Droid 2.0 发布：开源 Android 应用商店迎来重大改版](https://f-droid.org/2026/09/24/f-droid-2.0-a-new-chapter-for-android-freedom.html) ⭐️ 9.0/10

F-Droid 于 2026 年 9 月 24 日发布 2.0 版本，对这一开源 Android 应用商店进行了重大改版，引入了全新设计的用户界面和重构的软件源（repo）管理机制，同时逐步淘汰长期被诟病的 F-Droid Privileged Extension（FPE）。该版本引发了社区热烈讨论，相关帖子获得 918 个赞和 261 条评论。 F-Droid 是自由开源（FOSS）Android 应用最主流的分发渠道，因此 2.0 的重新发布会影响所有在 Google Play 生态之外安装应用的用户。此次改版意义尤为重大，因为 Google 已开始推行更严格的应用安装验证规则，可能压缩第三方应用商店的生存空间，使得 F-Droid 的未来可行性成为人们关注的焦点。 该版本的重点是新视觉设计和更顺畅的软件源管理，并逐步弃用 FPE——这是一个特权辅助组件，许多用户（尤其在 LineageOS 等第三方 ROM 上）反映其难以配置。讨论中用户还指出了细节问题，例如官方截图中出现文字换行错误，“Syncthing-Fork”被断行得十分尴尬，并抱怨新界面在各区块和可点击元素之间缺乏视觉区分。

hackernews · daveoc64 · 9月24日 15:26 · [社区讨论](https://news.ycombinator.com/item?id=49831968)

**背景**: F-Droid 是一个面向 Android 的自由开源应用仓库，只分发源代码公开的应用，是社区运营的 Google Play 替代方案。软件源（repo）是 F-Droid 客户端获取应用元数据和 APK 文件的来源，因此源管理是用户体验的核心环节，F-Droid 的服务端工具也可用于搭建自定义或第三方源。FPE 之所以存在，是因为 Android 通常要求每次安装应用都由用户确认，而这个特权扩展可以让 F-Droid 客户端在已 root 或使用第三方 ROM 的设备上静默安装与更新应用。与此同时，Google 正在收紧 Android 生态：自 2026 年 3 月起，认证设备上的应用安装验证逐步推行，2026 年 9 月起在巴西、印尼、新加坡和泰国开始强制执行，并计划于 2027 年全球推广。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://f-droid.org/">F-Droid - Free and Open Source Android App Repository</a></li>
<li><a href="https://f-droid.org/docs/">Docs | F-Droid - Free and Open Source Android App Repository</a></li>
<li><a href="https://pixelunion.eu/blog/2026/03/google-closing-android-ecosystem/">Google Is Closing Android: And Taking Your Freedom With It | PixelUnion - Free your photos from American tech platforms</a></li>

</ul>
</details>

**社区讨论**: 社区情绪褒贬不一：用户普遍欢迎此次改版以及 FPE 的淘汰，一位 GrapheneOS 用户表示自己正是因为 F-Droid 界面糟糕、特权扩展难以配置才转用了第三方客户端 Droid-ify。也有人尖锐批评新设计缺乏视觉层次、可点击性和滚动提示不清晰，并且宣传截图中出现了明显的文字换行错误。另一个反复出现的担忧是：当 Google 明年的安装验证封锁措施生效后，F-Droid 将何去何从。

**标签**: `#F-Droid`, `#Android`, `#Open Source`, `#App Store`, `#UI/UX`

---

<a id="item-2"></a>
## [DHH 在 Rails World 2026 主题演讲：AI 时代开发者将成“创造者”](https://www.youtube.com/watch?v=vDjW_dRyKXY) ⭐️ 8.0/10

Ruby on Rails 的创造者 David Heinemeier Hansson（DHH）在 Rails World 2026 大会上发表了开场主题演讲，围绕 AI 描绘软件开发的未来，并提出开发者正从“写代码的人”转变为“创造事物的人（maker）”。演讲还讨论了在 AI 能够直接生成应用代码的当下，Rails 等成熟框架为何依然具有持续的相关性。 这场主题演讲之所以引发开发者社区的强烈反响，是因为它主张 AI 将重塑大多数程序员日常工作的实质内容，而不仅仅是加快写代码的速度。作为框架创造者在旗舰社区大会上的发言，它也反映出主流 Web 开发生态正如何围绕 AI 工具重新定位自身。 有评论者指出，DHH 的论述更多是从 Rails 的开发者和使用者视角出发，而不是从框架维护者、守护者的角度出发，一些人认为这对该项目而言是不太乐观的信号。讨论中还提到了 37Signals 正在进行的 Rust 重写工作，以及设计良好的测试套件在决定 AI 辅助重写能否成功方面所起的作用。

hackernews · an0malous · 9月23日 15:33 · [社区讨论](https://news.ycombinator.com/item?id=49817680)

**背景**: Rails World 是 Ruby on Rails 的官方年度大会。Rails 是 DHH 于 2004 年从自己的公司 Basecamp（37Signals）中提炼出来的开源 Web 框架，并因“约定优于配置”等理念而广受欢迎。Rails 常用于 CRUD 类 Web 应用（即基于数据库、执行创建、读取、更新、删除记录的应用），以让小团队快速交付产品而著称。DHH 也以对软件与行业趋势直言不讳、观点鲜明而闻名，因此他的主题演讲常常成为更大范围讨论的参照点。

**社区讨论**: Hacker News 上的评论者大体认同 AI 将给开发者带来实实在在的变化，但许多人对 DHH 的论述框架提出质疑：一位坐在前排的参会者表示现场气氛“远非末日论”，多数工程师仍是在维护客户愿意付费的系统、扮演“修补者（mender）”的角色；也有人反问，既然可以直接使用 AI，为什么还要用开发者“创造”的应用。数位评论者为 Rails 在 CRUD 场景中的价值辩护，认为其强约定特性使其特别适合 AI 生成的代码；还有评论者把 Rust 重写的成功率与既有测试套件的质量联系起来。

**标签**: `#Rails`, `#Ruby on Rails`, `#AI`, `#Keynote`, `#Software Development`

---

<a id="item-3"></a>
## [Apple 撤下 ADP，英国 iCloud 用户被拆成两级加密](https://macanorak.com/two-tier-encryption-in-the-uk/) ⭐️ 8.0/10

在英国政府发出的一项保密法律命令之后，Apple 撤下了面向英国 iCloud 用户的“高级数据保护”（ADP），英国账户因此无法再开启这项可选的点对点加密，原本受其覆盖的 iCloud 备份、照片、备忘录和 iCloud Drive 也随之失去保护。macanorak 的这篇分析将结果概括为“两级加密”体制：两台完全相同的 Apple 设备，仅因机主身处英国境内或境外，就获得不同等级的保护。 此事的先例意义在于：一个政府可以在从未公开承认相关命令的情况下，迫使一家全球性平台在整个国家范围内撤回点对点加密功能，这等于鼓励其他政府提出同样要求。它同时削弱了 Apple 自 2015 年以来一直使用的信任论据——即“无法解密就无法交出数据”——因为对许多英国账户而言，Apple 又重新掌握了密钥。 在英国，包括 iCloud 钥匙串和健康数据在内的大约 14 类 iCloud 数据默认仍是点对点加密的，而开启 ADP 本可将这一数字提高到约 23 类。回退到“标准数据保护”的那些类别——iCloud 备份、照片、备忘录、iCloud Drive 等——恰恰是 Apple 持有密钥、因而可以响应合法法律程序的类别；也有评论者指出，即使在名义上未受影响的类别中，英国用户的加密密钥在常见使用方式下仍可能被暴露。

hackernews · ReturnoftheHack · 9月24日 10:39 · [社区讨论](https://news.ycombinator.com/item?id=49828731)

**背景**: iCloud 数据在传输和存储时都会加密，但默认情况下 Apple 掌握着大多数类别的解密密钥，这意味着它技术上能够访问这些数据，并在法律强制要求时交出去。Apple 于 2022 年 12 月 7 日推出的“高级数据保护”是一项可选设置，它把几乎所有 iCloud 类别切换到点对点加密，使只有用户自己的设备持有密钥。英国的这道命令依据的是 2016 年《调查权力法》下的“技术能力通知”，该机制可以要求企业构建或维持拦截能力，而在本案中，这意味着必须改变 ADP 所依赖的架构。Apple 既没有构建这种能力，也没有在英国彻底放弃加密，而是选择对英国用户下架该功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://macanorak.com/two-tier-encryption-in-the-uk/">Two-Tier Encryption in the UK - macanorak.com</a></li>
<li><a href="https://mjtsai.com/blog/2026/09/22/two-tier-encryption-in-the-uk/">Michael Tsai - Blog - Two-Tier Encryption in the UK</a></li>
<li><a href="https://www.gov.uk/government/publications/notices-regime-code-of-practice/notices-regime-code-of-practice-accessible">Notices regime code of practice (accessible) - GOV.UK</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍把“两级加密”解读为“多绕了几步的后门”，不少人怀疑一个更不安全的等级不可能只局限于“别人”。也有人对技术表述提出修正，指出那 14 个默认类别并非完全不受影响，英国用户的加密密钥在常见使用场景下仍可能泄露；另一个反复出现的主题是，Apple 在 2015 年有与 FBI 硬碰硬的胆量，如今却显得不那么愿意抵抗，还有人主张 Apple 应当退出英国市场，或干脆切断对英国政府客户的服务。

**标签**: `#encryption`, `#privacy`, `#Apple`, `#UK-policy`, `#end-to-end-encryption`

---

<a id="item-4"></a>
## [Show HN：Bastardica 滥用 OpenType 连字把不搭的字体混在一起](https://bastardica.mitpit.com/) ⭐️ 7.0/10

Bastardica 是一个新的浏览器端工具（bastardica.mitpit.com），它故意滥用 OpenType 的连字替换机制，把一款字体的字形塞进另一款字体里，从而生成诸如 Times New Bastard 这类刻意“诡异”的混搭字体。它完全在浏览器中运行编译为 WebAssembly 的 Python，因此无需服务器往返就能快速处理并生成修改后的字体。 这个项目在 Hacker News 上获得了很强的社区认可（469 分、64 条评论），说明即便是一个玩笑性质的工具，也能成为展示“在客户端用 WebAssembly 跑 Python”的有力演示。它还凸显出 OpenType 的替换特性——平时用于讲究的排版——可以被改造成创意编程的媒介，同时给设计师提供了一个动手玩排版梗的玩具。 技术上讲，这个手法依赖 OpenType 的连字特性（liga 及相关替换查找表），把普通的字符序列映射到来自另一款字体的字形上，因此输出的是一个标准 OpenType 文件，安装到哪里就能在哪里显示这种混搭效果。由于 Python 被编译为 WASM，所有字体处理都在浏览器本地完成，既不需要把字体上传到服务器，也降低了延迟；代价则是 WASM 包体积和浏览器内存开销。

hackernews · MitPitt · 9月23日 22:53 · [社区讨论](https://news.ycombinator.com/item?id=49823738)

**背景**: OpenType 是微软和 Adobe 开发的现代跨平台字体格式，它支持的高级排版表远超简单的字形轮廓。连字（ligature）就是其中一项特性：用查找表把两个或多个字符替换成一个组合字形，最常见的例子有 'fi'、'fl' 和 'ffl'。WebAssembly（Wasm）是一种可移植的二进制指令格式，能让 C、C++、Rust 乃至如今的 Python 等语言在浏览器中以接近原生的速度运行；Pyodide、py2wasm 等项目让用这种方式运行 Python 变得切实可行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Fonts/OpenType_fonts">OpenType font features - CSS | MDN - MDN Web Docs Usage example</a></li>
<li><a href="https://github.com/pyodide/pyodide">GitHub - pyodide/pyodide: Pyodide is a Python distribution ... Waspy - Python to WebAssembly Compiler Running Python in the Browser with WebAssembly GitHub - wasmerio/wasmer-python: WebAssembly runtime for ... Python to WebAssembly: Unleashing New Possibilities in Web ... Python WebAssembly: Unleashing Python's Power on the Web</a></li>
<li><a href="https://wasmer.io/posts/py2wasm-a-python-to-wasm-compiler">Announcing py2wasm: A Python to Wasm compiler - Blog · Wasmer</a></li>

</ul>
</details>

**社区讨论**: 评论区热烈地交流各种字体恶作剧的点子：一位设计师描述自己如何仔细调整垂直缩放与偏移，让 Papyrus 与 Comic Sans 在视觉上对齐；另一位则建议把 Helvetica 和 Arial 每隔一两个字符混用，好让设计师精神崩溃。还有人提到了自我审查字体 Paranoia Sans，并提出可以用连字把一个词渲染成另一个词，比如让 “red” 显示为 “green”，此外还有人调侃一款故意把字距做得很糟的 Arial 变体。

**标签**: `#typography`, `#OpenType`, `#WebAssembly`, `#creative-coding`, `#Show HN`

---

<a id="item-5"></a>
## [Dynomight 探讨：肝脏为何再生能力如此特殊](https://dynomight.substack.com/p/liver) ⭐️ 7.0/10

科学博客 Dynomight 发表了一篇文章，探讨为什么肝脏的再生能力远强于人体其他器官，作者认为答案在于进化压力和人体伤口愈合的优先次序，而非某种独特的生物学奇迹。该文在 Hacker News 上引发热烈讨论（约 237 分、151 条评论），评论者质疑了作者的若干进化论论断，并补充了亲身经历的肝移植案例。 理解肝脏为何能再生、而其他器官基本不能，具有直接的临床意义：它是劈离式肝移植（split-liver transplantation）的基础——一个供体肝脏被分成两半，各自在不同受者体内重新生长；这也影响着研究者对心脏、肾脏等器官再生医学的思考方向。这篇文章还体现了科学传播的一种普遍模式：一篇论证扎实的博客文章，能够引出正式论文中少见的专家反例和患者亲身经历。 文章将肝脏视为一个异类：它主要依靠现有肝细胞的增殖来再生，而非依赖专门的干细胞库，并权衡了瘢痕形成与完美修复之间的取舍。评论者提出了反例：目前已知没有任何成年蝾螈能再生被完全摘除的眼睛；被切断的蝾螈只会死亡，而不像涡虫（planarian）那样再生；墨西哥钝口螈（axolotl）能再生肢体，却并非所有结构都能再生。

hackernews · jbotz · 9月24日 16:23 · [社区讨论](https://news.ycombinator.com/item?id=49832938)

**背景**: Dynomight 是一个广受欢迎的匿名科学与统计博客，以篇幅长、考据细、常带幽默的深度文章著称。肝脏再生是有充分文献记载的现象：在手术切除最多约三分之二的肝脏后，剩余组织会在数周内增生扩大，这正是活体供肝移植和劈离式肝移植得以实现的原因。相比之下，人体大多数器官——心脏、肾脏和中枢神经系统——愈合时主要形成瘢痕组织；生物学家通常将此解释为快速可靠的伤口闭合与完整组织重建之间的一种取舍。文章采用的进化压力框架，把再生视为只有在生存收益超过其代谢成本与致癌风险时才会演化出来的性状。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dynomight.substack.com/archive">Archive - DYNOMIGHT INTERNET NEWSLETTER</a></li>
<li><a href="https://en.wikipedia.org/wiki/Wound_healing">Wound healing - Wikipedia</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC12717721/">Liver regeneration : unraveling the molecular mechanisms and...</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认同这篇文章写得异常出色，有人感谢作者写出了“像是真人写的”文章；但也有不少人质疑其进化推理：一位评论者认为人体大部分器官不能再生只是因为缺乏选择压力，并指出蝾螈的再生能力其实存在明显局限；另一位则强烈反对“人类被过度调校为修复皮肤和血液”的说法，指出伤口愈合能力受损会导致严重的术后并发症和死亡。一位肝移植受者分享了自己的亲身经历：他接受了供体肝脏的一半，新肝脏在数月内便重新生长，而另一叶则移植给了一名儿童受者。

**标签**: `#biology`, `#regeneration`, `#evolution`, `#medicine`, `#science-communication`

---

<a id="item-6"></a>
## [Google 发布 Gemini 3.8 TTS 模型：2000+ 音色与 30 秒声音克隆](https://simonwillison.net/2026/Sep/23/gemini-tts-playground/) ⭐️ 7.0/10

Google 发布了两款新的 Gemini 文本转语音模型 gemini-3.8-flash-tts 和 gemini-3.8-flash-lite-tts，提供超过 2000 种音色的音色库，并支持仅用 30 秒的音频样本（用户拥有使用权的嗓音）创建自定义声音。Simon Willison 同步发布了一个自带 API Key 的浏览器 Playground，他借助 GPT-6 Astra 以“vibe coding”方式完成开发，界面中可加载 2089 种音色。 仅需一段短样本即可完成声音克隆，再加上庞大的音色库和多说话人对话能力，大幅降低了开发者在主流云 API 之上构建有声书、播客、游戏对白和无障碍工具的门槛。这也把生产级合成语音进一步推向“商品化”，加剧了与专业 TTS 厂商的竞争，并再次引发关于声音克隆授权与滥用的担忧。 该 API 的一个显著能力是能轻松定义多角色之间的完整对话，每个角色都可指定独立音色和表达风格指令。在 Willison 的测试中，用 gemini-3.8-flash-tts 生成 1 分 18 秒的音频耗时约 20 秒、花费 2.74 美分；这个 Playground 之所以能运行，是因为底层 Gemini API 采用了开放的 CORS 策略，API Key 仅保存在页面内存中，绝不会写入浏览器存储。

rss · Simon Willison · 9月23日 17:12

**背景**: 文本转语音（TTS）系统把书面文字转换为语音音频，而现代神经 TTS 模型还能控制音色身份、情绪和说话风格。声音克隆是一种复制特定人声的 AI 技术，使得该声音可以说出其本人从未说过的话；它可用于有声书制作，也能帮助因疾病失去声音的人，但同时也是音频深度伪造的一种形式，会被用于诈骗和虚假信息传播。CORS（跨源资源共享）是一种 Web 机制，允许某个域名下的网页调用另一个域名上的 API，这正是第三方浏览器 Playground 无需代理服务器就能直接访问 Google Gemini 接口的原因。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Voice_cloning">Voice cloning</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Guides/CORS">Cross-Origin Resource Sharing (CORS) - HTTP | MDN</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-6_Astra">GPT-6 Astra</a></li>

</ul>
</details>

**标签**: `#text-to-speech`, `#Gemini`, `#voice-cloning`, `#AI models`, `#developer tools`

---

<a id="item-7"></a>
## [arXiv 获 1720 万美元慈善资助，启动独立非营利组织转型](https://www.reddit.com/r/MachineLearning/comments/1wox8kt/arxiv_receives_multiyear_philanthropic/) ⭐️ 7.0/10

arXiv 宣布获得来自 Simons Foundation International、XTX Markets 和 Siegel Family Endowment 的多年度慈善资助，总额达 1720 万美元，资助周期为三至五年。这笔资金旨在支持 arXiv 作为独立非营利组织正式启动运营，从而脱离此前由康奈尔大学代管的架构。 arXiv 是物理学、数学和计算机科学领域事实上的预印本平台，当今大量人工智能与机器学习研究在通过同行评审之前都先发布于此，因此它的财务稳定性直接影响全球研究界获取新成果的速度。获得多年期资金并转型为独立非营利组织，降低了单一大学预算压力可能冲击这一关键开放获取科研基础设施的风险。 这笔承诺总额为 1720 万美元，覆盖三到五年，来自三家资助方——Simons Foundation International、算法交易公司 XTX Markets 以及 Siegel Family Endowment。消息发布在 arXiv 官方博客上，定位是支持 arXiv 向独立非营利治理模式过渡，而非资助某项具体的新技术功能。

reddit · r/MachineLearning · /u/Nunki08 · 9月24日 09:43

**背景**: arXiv 是一个免费、开放获取的预印本平台，1991 年诞生于洛斯阿拉莫斯国家实验室，后来由康奈尔大学托管；研究者可以在正式同行评审和期刊发表之前，先把论文公开挂出。它已成为物理学、数学和计算机科学预印本的默认发布地，近年来在人工智能和机器学习领域的增长尤为迅速。要维持这样大规模的服务，需要服务器、内容审核和人员的持续投入，因此多年期慈善承诺比一次性捐赠更为重要。捐赠方之一的 XTX Markets 是一家总部位于伦敦的算法交易公司，成立于 2015 年，利用机器学习技术为金融市场做价格预测。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.itsoc.org/publications/arxiv/arxiv-faq">ArXiV FAQ | IEEE Information Theory Society</a></li>
<li><a href="https://www.xtxmarkets.com/">Home | XTX Markets</a></li>
<li><a href="https://otio.ai/blog/what-is-arxiv-preprint">What Is Arxiv Preprint + How to Submit There — Otio Blog</a></li>

</ul>
</details>

**标签**: `#arXiv`, `#open access`, `#research infrastructure`, `#philanthropy`, `#academic publishing`

---

<a id="item-8"></a>
## [Whiteboard（YC W26）：面向人机协作的开源可视化架构 IDE](https://github.com/devdotfast/whiteboard) ⭐️ 6.0/10

由 Sid、Alex、Ketan 和 Milan 四人组成的团队发布了 Whiteboard，这是一款以 MIT 许可证开源发布的桌面应用，人类与 AI 编码智能体可以在共享的可视化画布上共同设计软件架构。该应用通过一套 agent SDK 接入 Claude Code、Codex 等现有智能体，让它们能在应用内画布上绘制图表并讲解自己的工作过程。 该发布在 Hacker News 上获得了 188 分和 79 条评论，有评论者预测“由智能体实时绘制的图表”将在一年内成为主流工作方式。它瞄准了智能体编程的一个真实痛点：团队合并 AI 生成的 PR 的速度远超自己理解代码的速度，从而不断累积创始人所称的“认知债务”。 Whiteboard 构建在 CodeOSS（VS Code 的开源内核）之上，因此继承了 LSP 支持和 VSCode 快捷键；它还包含一个用 Rust 编写的、基于 AST 的语义 diff 查看器，会把新增的大型函数概括为伪代码，并折叠单元测试和文档改动，且可通过 WASM 插件系统扩展。值得注意的局限是：该应用目前无法编辑文件，这引发了关于“IDE”这一称谓是否准确的争论；此外它目前仅支持 macOS，不过所有功能将始终保持可自托管。

hackernews · sidharthkmenon · 9月24日 17:21 · [社区讨论](https://news.ycombinator.com/item?id=49833867)

**背景**: CodeOSS 是微软 Visual Studio Code 所基于的开源代码库，为第三方应用提供了现成的编辑器基础和语言服务器（LSP）支持。Claude Code 是 Anthropic 的智能体编程工具，能读取代码库、编辑文件并运行命令；Codex 则是 OpenAI 的 AI 编程智能体，于 2025 年 4 月以 CLI 形式发布。Whiteboard 让这些通常只在文本中工作的智能体，通过向共享画布绘图来可视化地表达自己的方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.linuxadictos.com/code-oss-vscodium-or-visual-studio-code-what-should-i-install-on-linux.html">Code OSS , VSCodium or Visual Studio Code: what should you install...</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_Codex_(AI_agent)">OpenAI Codex (AI agent) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 整体反响积极且富有建设性：评论者 bbor 称赞“假手绘动画＋图表流式生成”的模式将在 12 个月内普及，他起初抱怨仅支持 macOS，随后又公开更正了自己的说法。其他人指出无法编辑文件让“IDE”这一称谓站不住脚，并请求支持链接和评论 GitHub PR；评论者 2001zhaozhao 则认为，在高层次架构工作上，它比编码智能体现有的“Plan Mode”更可视化、更好用。

**标签**: `#AI agents`, `#developer tools`, `#open source`, `#software architecture`, `#Show HN`

---