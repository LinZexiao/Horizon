---
layout: default
title: "Horizon Summary: 2026-09-10 (EN)"
date: 2026-09-10
lang: en
---

> From 27 items, 13 important content pieces were selected

---

1. [Calif Research demos WeWorm, an AI-built zero-click WeChat call worm](#item-1) ⭐️ 9.0/10
2. [OpenAI Claims Navier–Stokes Millennium Prize Solution Amid Priority Dispute](#item-2) ⭐️ 9.0/10
3. [Shopify moves its mobile app from React Native back to native Swift and Kotlin](#item-3) ⭐️ 8.0/10
4. [Forgejo 16.0.4 Fixes Critical RCE in Versions Up to 16.0.3](#item-4) ⭐️ 8.0/10
5. [Microsoft Elevates Rust to Tier-1 Language](#item-5) ⭐️ 8.0/10
6. [Brown Report: Silicon Valley Deepens the Military-Industrial Complex](#item-6) ⭐️ 8.0/10
7. [Terence Tao Warns AI Is Mining Math's Open Problems Dry](#item-7) ⭐️ 8.0/10
8. [Cognition launches SWE-2 coding model, claiming near-frontier performance at lower cost](#item-8) ⭐️ 7.0/10
9. [NASA Mars Color Technique Adapted to Reveal Faded Rock Art on Earth](#item-9) ⭐️ 7.0/10
10. [PlanetScale launches Neki, a sharded Postgres, to heated debate](#item-10) ⭐️ 7.0/10
11. [348M model trained on 22.7B tokens handles 14-digit arithmetic](#item-11) ⭐️ 7.0/10
12. [Fly connectome fails to learn Pong, and the audit is the real story](#item-12) ⭐️ 7.0/10
13. [Sante's 83.83 on DiagnosisArena-MCQ Measures Only Answer Selection](#item-13) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Calif Research demos WeWorm, an AI-built zero-click WeChat call worm](https://simonwillison.net/2026/Sep/10/calif-research/) ⭐️ 9.0/10

Calif Research released a demo of WeWorm, which it describes as the first zero-click worm to spread through WeChat calls across both iOS and Android. The team says that, working with AI, it found the underlying bug and wrote the first remote code execution (RCE) exploit in roughly two days, then spent about one more week turning that exploit into a self-spreading worm. If the claim holds up, this is a significant milestone on two fronts at once: a zero-click, self-propagating attack against a messaging platform used by well over a billion people, and a demonstration that AI assistance can compress exploit development that once took a large team months into a matter of days. It signals that AI-accelerated vulnerability discovery and exploitation is moving from speculation into practical, demonstrated capability, which raises the pressure on platform vendors to patch faster and on defenders to assume shorter attack timelines. According to the announcement, the victim does not need to answer the call or interact with the phone at all, and even answering yields silence while the exploit still succeeds — behavior typical of zero-click vulnerabilities in call and messaging stacks. The release is explicitly described as a demo rather than a full weaponized release, and no affected versions, CVE identifiers, or patches are mentioned, so the claim has not been independently verified from the quoted material.

rss · Simon Willison · Sep 10, 00:56

**Background**: A zero-click exploit is a class of attack that compromises a device without any user interaction, such as tapping a link or opening a file, which makes it far harder to detect and defend against than ordinary phishing-style attacks. WeChat, operated by Tencent, is one of the world's largest messaging platforms, and its call feature — like other VoIP and messaging stacks — is a high-value target because it processes data from the network automatically. AI-assisted vulnerability discovery uses machine learning and large language models to scan code, dependencies, and configurations for weaknesses at a scale and speed humans cannot match; security researchers have increasingly warned that attackers benefit from these same capabilities, not just defenders.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kaspersky.com/resource-center/definitions/what-is-zero-click-malware">Zero-Click Exploits - Kaspersky</a></li>
<li><a href="https://www.vulncheck.com/blog/ai-assisted-vulnerability-discovery?trk=article-ssr-frontend-pulse_little-text-block">The First CVE Wave: Signs That AI - Assisted Vulnerability Discovery ...</a></li>

</ul>
</details>

**Tags**: `#ai-security-research`, `#cybersecurity`, `#malware`, `#zero-click-exploit`, `#WeChat`

---

<a id="item-2"></a>
## [OpenAI Claims Navier–Stokes Millennium Prize Solution Amid Priority Dispute](https://simonwillison.net/2026/Sep/8/on-navier-stokes/) ⭐️ 9.0/10

OpenAI announced on September 8, 2026 that an unreleased internal model, run as a swarm of roughly 10,000 agents, produced a counterexample resolving the Navier–Stokes existence and smoothness problem, one of the seven Millennium Prize Problems, together with a Lean formalization verified by a model called GPT-6 Astra. The claim is overshadowed by a priority dispute: NYU mathematician Tristan Buckmaster says he and Anthropic employee Levent Alpöge reached closely related results on August 15 after nearly a year of work using Claude and Codex, and that OpenAI only started its effort after learning of their progress. If verified, this would be the first Millennium Prize Problem resolved with substantial AI involvement, marking a possible paradigm shift in how mathematics is done and a major validation of large-scale agentic AI for research. It also thrusts questions of research ethics, attribution, and training-data provenance into the center of the AI-for-science debate, especially given the Anthropic–OpenAI rivalry behind the dispute. OpenAI says the effort began on September 1, that the agents reached the resolution on September 5 after about 88 hours, and that Lean formalization and verification took another 17 hours; the agents sent 2.7 million messages and used roughly 130 billion output tokens on Navier–Stokes alone (4.9 million messages and 300 billion output tokens across all attempted problems, which at public GPT-6 Astra API prices would cost about $15 million). The counterexample is unverified by external mathematicians or the Clay Mathematics Institute, and OpenAI stated it would not claim the $1 million prize; the method reportedly builds on a 2023 blowup-technique approach by Diego Córdoba and Luis Martínez-Zoroa.

rss · Simon Willison · Sep 8, 23:55

**Background**: The Navier–Stokes equations are a system of partial differential equations describing how fluids move; while they are used successfully in countless engineering computations, there is no complete analytical understanding of whether smooth solutions always exist in three-dimensional space and time, a question often linked to turbulence. In 2000 the Clay Mathematics Institute named the existence and smoothness problem as one of seven Millennium Prize Problems, each carrying a $1 million award for a correct solution. As of now the only officially solved Millennium problem is the Poincaré conjecture, solved by Grigori Perelman, who declined the prize in 2010.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Navier-Stokes_existence_and_smoothness_problem">Navier-Stokes existence and smoothness problem</a></li>
<li><a href="https://en.wikipedia.org/wiki/Millennium_Prize_Problems">Millennium Prize Problems</a></li>
<li><a href="https://www.claymath.org/millennium-problems/">The Millennium Prize Problems - Clay Mathematics Institute</a></li>

</ul>
</details>

**Discussion**: Commenters are largely skeptical: one draws an analogy to an unethical human collaborator publishing work based on researchers' ideas without attribution, while another argues both can be true — that a model may absorb chat data into its latent representations and still discover genuinely novel techniques through massive RL on verifiable math. Others note the suspicious timing of generating 300 billion output tokens from a still-in-training model right after rumors of a major proof surfaced, describing it as feeling like 'parallel construction', though they concede each individual step has a plausible explanation.

**Tags**: `#AI-for-Mathematics`, `#Navier-Stokes`, `#Millennium-Prize`, `#OpenAI`, `#Research-Integrity`

---

<a id="item-3"></a>
## [Shopify moves its mobile app from React Native back to native Swift and Kotlin](https://shopify.engineering/back-to-native) ⭐️ 8.0/10

Shopify published an engineering post announcing that it is migrating its mobile app away from React Native and back to fully native iOS (Swift) and Android (Kotlin) codebases. The announcement drew a large Hacker News discussion (651 points, 437 comments) that quickly broadened into a debate about native versus cross-platform development in an era of AI-generated code. Shopify is one of the largest public users of React Native, so reversing that choice is a notable industry data point that other companies weighing cross-platform frameworks will likely cite. The discussion suggests the decision is part of a wider recalculation: as AI code generation makes writing native Swift and Kotlin far cheaper, React Native's original advantage of letting web developers ship mobile apps is weakening. The write-up is a single company's engineering decision rather than a field-wide breakthrough, and the source content itself contains no published benchmarks or timeline details. Commenters supplied the concrete anecdotal data instead: one developer reported porting a 15–20 screen app to both iOS and Android essentially overnight using Codex plus the Maestro testing tool, then spending a few days polishing.

hackernews · fnthawar2 · Sep 10, 14:09 · [Discussion](https://news.ycombinator.com/item?id=49643982)

**Background**: React Native is an open-source UI framework created by Meta (then Facebook) that lets developers write mobile apps in JavaScript/React while still rendering with native platform components; it supports iOS, Android and other targets and has been used by Meta, Microsoft and Shopify. Its long-standing pitch is code reuse — one codebase, or at least one team of web developers, serving both mobile platforms. Swift is Apple's language for iOS/macOS development and Kotlin is Google's preferred language for Android, so a move back to native means maintaining two separate platform-specific codebases.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/React_Native">React Native</a></li>
<li><a href="https://reactnative.dev/">React Native</a></li>

</ul>
</details>

**Discussion**: Sentiment was mixed but leaned toward "it depends." One top comment framed it as a spectrum — every company sits somewhere along a line dividing cases where Electron/React Native makes sense from those where it does not, and it is simply a resource-constrained engineering tradeoff rather than a matter of absolutes. Others argued that because AI models now generate native iOS/Android code well, React Native's "leverage your web devs" rationale has largely evaporated, while another commenter shared firsthand experience of porting an entire app overnight with Codex and Maestro; a fourth voiced a user-side complaint about being pushed into the Shop app just to track a package.

**Tags**: `#React Native`, `#iOS/Android Native`, `#Mobile Engineering`, `#Cross-Platform Development`, `#AI Code Generation`

---

<a id="item-4"></a>
## [Forgejo 16.0.4 Fixes Critical RCE in Versions Up to 16.0.3](https://codeberg.org/forgejo/forgejo/src/branch/forgejo/release-notes-published/16.0.4.md) ⭐️ 8.0/10

Forgejo released version 16.0.4, which patches a critical remote code execution (RCE) vulnerability affecting all versions up to and including 16.0.3. The fix, tracked as PR 14301, prevents template expansion from interfering with git repository initialization when a new repository is generated from a template repository. Forgejo is a widely used self-hosted Git forge, so any RCE flaw puts countless self-managed instances and their code at risk, and administrators are urged to upgrade immediately. The disclosure also highlights the security dynamics between Forgejo and its upstream-adjacent sibling Gitea, which project leadership says is not affected by either issue. The vulnerability is triggered during repository generation from a template: Forgejo clones the template repo, removes the .git folder, performs variable template expansion on files listed in .forgejo/template, and then re-initializes a new git repository — a sequence the fix now hardens. The 16.0.4 release notes contain two security fixes, and Codeberg rate limits initially made the notes hard to load, prompting community members to repost the details.

hackernews · weierstass · Sep 10, 15:57 · [Discussion](https://news.ycombinator.com/item?id=49645907)

**Background**: Forgejo is an open-source, self-hosted software forge written in Go that provides Git repository hosting along with issue tracking, code review, wikis, and CI features; it is governed by Codeberg e.V. and is the software behind Codeberg.org. Forgejo originated as a community-governed fork of Gitea, which itself is a fork of Gogs, so the two projects share a large amount of code and frequently compare security posture. A remote code execution vulnerability is one of the most severe classes of flaw, since an attacker can run arbitrary code on the server rather than merely read or alter data.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Forgejo">Forgejo</a></li>
<li><a href="https://forgejo.org/">Forgejo – Beyond coding. We forge.</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gitea">Gitea</a></li>

</ul>
</details>

**Discussion**: Commenters noted that Codeberg rate limits made the official release notes unreadable and reposted the two fixes for others. Gitea project leadership clarified that Gitea is protected against both issues while cautioning against shaming anyone who reports security bugs, and one commenter argued that Forgejo's decision to disallow LLM contributions may leave it at a disadvantage since attackers still use AI to find vulnerabilities.

**Tags**: `#security`, `#vulnerability`, `#forgejo`, `#gitea`, `#self-hosted`

---

<a id="item-5"></a>
## [Microsoft Elevates Rust to Tier-1 Language](https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/) ⭐️ 8.0/10

Microsoft has granted Rust "Tier-1 language" engineering status internally, giving product teams a paved path from local development to production — covering secure toolchain builds, productive developer tooling, quality workflows, deep platform integration and compliance. The designation, described in a guest post published by the Rust Foundation, signals that Rust is now a core language for Microsoft's own systems and security-critical work rather than an experimental option. This is a significant industry validation of Rust from one of the world's largest software vendors, and it means every major OS vendor that also influences C and C++ tooling has now diversified its systems-programming options for greenfield work. It also strengthens the broader memory-safety push, since Microsoft has previously attributed roughly 70% of its product vulnerabilities over the past decade to memory-safety issues that Rust is designed to prevent. According to the community discussion, the most concrete technical news is that Microsoft has moved its Rust toolchain onto MSVC's backend instead of LLVM, making long-rumored MSVC integration public; official details beyond the tier-1 designation remain limited. Commenters also point to Microsoft's stated goal of converting 1 billion lines of code to Rust by 2030 through automated tooling billed as "1 engineer, 1 month, 1 million lines of code," a target whose feasibility is widely questioned.

hackernews · mmastrac · Sep 10, 13:39 · [Discussion](https://news.ycombinator.com/item?id=49643546)

**Background**: Rust is a systems programming language, originally created at Mozilla and now stewarded by the independent Rust Foundation, whose standout feature is compile-time memory safety: its ownership and borrowing rules prevent classes of bugs such as buffer overflows and dangling pointers without a garbage collector. "Tier-1" here is a Microsoft-internal engineering status describing how well a language is supported across the company's build, tooling, and compliance pipelines, not a public product release. The context is a broad government- and industry-led campaign — including a 2025 CISA/NSA joint guide on memory-safe languages — to move critical software away from C and C++, which do not enforce memory safety and are the root of a large share of security vulnerabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/">Guest Post: Rust Is Tier-1 Language at Microsoft</a></li>
<li><a href="https://www.memorysafety.org/docs/memory-safety/">What is memory safety and why does it matter? - Prossimo Memory Safe Languages: Reducing Vulnerabilities in Modern ... Memory Safety: An Explainer - Center for Security and ... Memory Safe Languages: Reducing Vulnerabilities in Modern ... An Introduction to Memory Safety Concepts and Challenges Software Memory Safety</a></li>
<li><a href="https://www.cisa.gov/resources-tools/resources/memory-safe-languages-reducing-vulnerabilities-modern-software-development">Memory Safe Languages: Reducing Vulnerabilities in Modern ...</a></li>

</ul>
</details>

**Discussion**: Overall sentiment is strongly positive: commenters see the move as proof that Rust is no longer a "fledgling language that moves fast and breaks things" but a mature competitor to C++ and C#, and more polished than newer "better C/C++" efforts like Zig and Odin. Several highlight the MSVC backend switch as the real headline, and one explains the strategic logic via memory-safety CVEs and Microsoft's product portfolio; others are skeptical of the automated 1-billion-line conversion goal and criticize Microsoft's simultaneous push to retire legacy Windows hardware.

**Tags**: `#Rust`, `#Microsoft`, `#Systems Programming`, `#Memory Safety`, `#Language Ecosystems`

---

<a id="item-6"></a>
## [Brown Report: Silicon Valley Deepens the Military-Industrial Complex](https://costsofwar.watson.brown.edu/paper/how-big-tech-and-silicon-valley-are-transforming-military-industrial-complex) ⭐️ 8.0/10

A new paper from Brown University's Costs of War project examines how Big Tech and Silicon Valley firms are transforming the military-industrial complex, and it sparked a 267-comment debate on Hacker News. Discussion highlights include the claim that Keyhole, a San Francisco startup, received seed funding in 2003 from the CIA-backed venture firm In-Q-Tel, and that within two weeks military and intelligence agencies were reportedly using its software to support the US war in Iraq before Google acquired it in 2004 and renamed it Google Earth. The report challenges the common assumption that Big Tech's engagement with the defense sector is a recent phenomenon, tracing the relationship back to the earliest days of the semiconductor industry. It matters because it fuels an ongoing ethical debate among engineers and tech workers about complicity, and because defense contracts are becoming a significant and growing revenue source for major cloud and AI companies. The paper is a policy and historical analysis rather than a technical announcement, and its concrete evidence includes the In-Q-Tel–Keyhole case linking CIA seed money to wartime software use. The supporting Hacker News thread is largely anecdotal, mixing historical arguments with personal accounts of refusing or quitting defense-related work, so claims in the discussion should be treated as viewpoints rather than verified findings.

hackernews · paimapi · Sep 10, 15:47 · [Discussion](https://news.ycombinator.com/item?id=49645754)

**Background**: The term "military-industrial complex" was popularized by US President Dwight D. Eisenhower in his 1961 farewell address to describe the close relationship between a nation's armed forces and the defense industry that supplies them. Brown University's Costs of War project, part of the Watson Institute for International and Public Affairs, studies the human, economic, and political costs of the post-9/11 wars. In-Q-Tel, cited in the report, is a CIA-backed venture capital firm founded in 1999 that invests in startups whose technology could serve US intelligence agencies. Silicon Valley's defense ties date back to the 1950s, when Fairchild Semiconductor and other early chipmakers sold integrated circuits for military systems such as the Minuteman missile.

**Discussion**: Commenters were divided: some argued that Silicon Valley has been funded by the Department of Defense from the start — citing Fairchild Semiconductor and Google's origins — and asked whether the world would have been better off if those firms had refused military chip contracts, while others questioned whether any company should reject its own government's defense contracts or whether the objection applies only to the United States. One commenter said they quit a high-paying job at Microsoft over what they described as complicity in Israeli war crimes, urging tech workers to push back against the military-industrial complex, and several participants shared notable findings from the report, such as the In-Q-Tel seed funding behind Keyhole before it became Google Earth.

**Tags**: `#military-industrial-complex`, `#silicon-valley`, `#defense-contracts`, `#tech-ethics`, `#policy`

---

<a id="item-7"></a>
## [Terence Tao Warns AI Is Mining Math's Open Problems Dry](https://simonwillison.net/2026/Sep/9/terence-tao/) ⭐️ 8.0/10

Terence Tao posted on Mastodon that the pool of good, fruitful open mathematical problems is being mined in a "non-renewable fashion," and that even the rumor of someone working on a problem can now trigger a massive amount of AI-powered effort to solve and "flatten" it before the original research project matures. He concludes that incentives may now push mathematicians to stop sharing promising research directions with the broader community at all. If researchers stop publicly sharing promising directions to avoid being scooped by AI-assisted efforts, it would reverse centuries of open-science tradition and could do serious long-term damage to mathematics and other fields that depend on openly shared problem lists. The warning reframes AI's growing mathematical capability as a threat to the social infrastructure of research, not just a productivity tool. Tao's key point is that open problems function like a non-renewable resource: good problems are scarce, slow to generate, and easily exhausted once many actors converge on them. Notably, he says it is not only actual work but the mere rumor of someone working on a problem that can trigger the flood of AI-assisted effort, meaning secrecy incentives may kick in at a very early stage.

rss · Simon Willison · Sep 9, 00:20

**Background**: In mathematics, open problems are the shared frontier of the field — researchers publicly announce the questions and conjectures they find promising, and others build on them, a norm that has driven progress for centuries. Recent AI systems have become increasingly capable at mathematical reasoning and search, capable of quickly exploring large spaces of related results once a target problem becomes known. Tao, a Fields Medalist and one of the most prominent voices on AI's role in mathematics, has previously written about how AI could exhaust the supply of approachable open problems.

**Tags**: `#ai-ethics`, `#open-science`, `#mathematics`, `#research-culture`, `#ai-impact`

---

<a id="item-8"></a>
## [Cognition launches SWE-2 coding model, claiming near-frontier performance at lower cost](https://cognition.com/blog/swe-2) ⭐️ 7.0/10

Cognition, the company behind the Devin coding agent, released SWE-2, which it calls its most advanced coding model yet. The company says SWE-2 scores 50.0% on FrontierCode 1.1 Main 1 — within one point of Fable 5.1 — while being 64% cheaper, or up to 70% lower cost on leading evals. The release intensifies competition in the coding-model market, where Cognition is positioning on capability-per-dollar rather than raw frontier performance, directly challenging Anthropic's Fable 5.1 and OpenAI's GPT-6 Astra. If the cost claims hold up, it could pressure pricing across the agentic coding tool segment that enterprises increasingly rely on. Cognition says it scaled reinforcement learning to the multi-trillion-parameter regime for the first time, building on the SWE-1.7 training infrastructure, and that SWE-2 is post-trained from Kimi K3. On efficiency, SWE-2 medium reportedly makes its first real code edit after a median of 18 steps versus 48 for SWE-1.7, which had drawn complaints about over-exploring simple tasks; the model's benchmark spread, however, ranges from 92.8% on Terminal Bench 2.1 to just 27.3% on Terminal Bench 4.

hackernews · seelos · Sep 10, 15:29 · [Discussion](https://news.ycombinator.com/item?id=49645443)

**Background**: Cognition is the AI lab known for Devin, one of the first widely publicized autonomous coding agents, and SWE-2 is the successor to its SWE-1.7 model. Benchmark scores such as FrontierCode and Terminal Bench are standardized tests used to compare coding models, and Terminal Bench 4 is a newer version released only weeks before this launch. The comparison points are Anthropic's Fable 5.1, an enterprise-focused model released in September 2026 with a 1M-token context window, and OpenAI's GPT-6 Astra, which debuted as a limited preview on September 3, 2026. Weights availability and training-data provenance have become central points of contention in the open-versus-closed model debate.

<details><summary>References</summary>
<ul>
<li><a href="https://cognition.com/blog/swe-2">Introducing SWE-2: Pushing the Pareto Frontier | Cognition</a></li>
<li><a href="https://llm-stats.com/models/claude-fable-5-1">Claude Fable 5.1 Benchmarks, Pricing & Context Window</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-6_Astra">GPT-6 Astra - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters were largely skeptical: the top point of contention was the gulf between SWE-2's 92.8% on Terminal Bench 2.1 and 27.3% on Terminal Bench 4, framed as a measure of "how benchmaxxed" the model is. Others cited Cognition's earlier Upwork demo controversy as reason to discount performance claims, questioned why anyone would choose a closed-weight model over DeepSeek Flash 4.1, and debated the drawbacks of post-training on another lab's model (Kimi K3). One commenter took the more positive view that an RL-tuned K3 reaching Fable 5-level capability is itself a promising sign.

**Tags**: `#AI/ML`, `#coding-agents`, `#LLM-benchmarks`, `#open-weights`, `#model-release`

---

<a id="item-9"></a>
## [NASA Mars Color Technique Adapted to Reveal Faded Rock Art on Earth](https://gizmodo.com/this-nasa-color-trick-was-meant-for-mars-now-its-unveiling-rock-art-on-earth-2000809844) ⭐️ 7.0/10

An image-processing technique that NASA originally developed to bring out subtle color differences in Mars imagery is now being adapted to reveal faded rock art on Earth, according to a NASA Spinoff feature. The method, known as decorrelation stretch, is being applied to photographs of ancient petroglyphs and pictographs whose markings have faded to the point of near-invisibility. The story is a striking example of a space-agency spinoff: technology built to study another planet is feeding back into archaeology and cultural-heritage preservation on Earth. If it can reliably bring out faint pigment and mineral contrasts, it gives researchers a non-destructive way to document fragile rock art that is weathering away and may be invisible to the naked eye. Decorrelation stretching works by mathematically removing the correlation between an image's color channels and re-stretching their variances, which maximizes color separation and makes faint features easier to distinguish; it is typically applied to false-color composites that mix visible and infrared bands. The same effect can be approximated in ordinary software — one commenter notes GIMP can decompose an image into LAB channels, auto-level the A/B chroma layers, and recompose — though such aggressive enhancement can also amplify noise and must be interpreted with care.

hackernews · gumby · Sep 10, 15:29 · [Discussion](https://news.ycombinator.com/item?id=49645437)

**Background**: Spacecraft such as Mars orbiters and rovers capture images in several wavelength bands, including infrared, which lie outside what human eyes can see; combining those bands into a 'false color' composite renders the scene in colors that differ from a normal photograph and can expose differences invisible in true color. Decorrelation stretch is a standard enhancement algorithm for such multispectral data, available in tools like MATLAB, ENVI and GIMP. Rock art fades over centuries through weathering, so enhancing subtle pigment or mineral contrasts can make vanished or faint markings readable again.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Decorrelation">Decorrelation - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/False_color">False color - Wikipedia</a></li>
<li><a href="https://www.mathworks.com/help/images/enhance-color-separation-using-decorrelation-stretching.html">Enhance Color Separation Using Decorrelation Stretching</a></li>

</ul>
</details>

**Discussion**: Hacker News readers were broadly positive, with one pointing to the expanded NASA Spinoff article behind the story for more detail. Several commenters added hands-on value: one shared a GIMP workflow for approximating the effect via LAB channel decomposition and auto-leveling, another recounted trying multispectral bandpass imaging at Angkor Wat (unsuccessfully, and interrupted by guards), and a third reflected that false-color composites changed how they think about sensing, since 'vegetation is red, not green.'

**Tags**: `#remote sensing`, `#archaeology`, `#image processing`, `#false color`, `#NASA spinoff`

---

<a id="item-10"></a>
## [PlanetScale launches Neki, a sharded Postgres, to heated debate](https://planetscale.com/blog/introducing-neki) ⭐️ 7.0/10

PlanetScale introduced Neki, a distributed and sharded Postgres solution built by the team behind Vitess, as announced in a blog post that drew 187 points and 96 comments on Hacker News. The launch positioned Neki as a way to make sharded Postgres accessible, though PlanetScale has not yet open-sourced it. The launch matters because Planetscale is a major database infrastructure vendor, and its entry into the sharded Postgres space signals growing industry momentum toward scaling Postgres beyond single-node limits. The controversy also highlights a broader debate about open-source versus proprietary database tooling in a market where competitors like Supabase offer open alternatives. PlanetScale states that Neki is not yet open source but will be released as an open-source project once it is ready and tested in real production workloads. Commenters also raised CAP theorem concerns about eventual consistency being unsuitable for many high-availability Postgres workloads, asking whether Neki addresses those tradeoffs.

hackernews · simon_weber · Sep 10, 15:43 · [Discussion](https://news.ycombinator.com/item?id=49645686)

**Background**: Postgres is a widely used open-source relational database, but it was originally designed for a single machine, so scaling it across many servers — a technique called sharding — is difficult and has spawned numerous forks and third-party tools. Distributed databases must balance the CAP theorem tradeoffs among consistency, availability, and partition tolerance, which is why commenters question whether an eventually consistent sharded system fits their workloads. PlanetScale previously built its business on Vitess, an open-source sharding system for MySQL originally created at Google, making the proprietary nature of Neki a point of comparison.

<details><summary>References</summary>
<ul>
<li><a href="https://planetscale.com/neki">Neki — PlanetScale | Sharded Postgres by the Team Behind Vitess.</a></li>
<li><a href="https://neki.dev/">Sharded Postgres by PlanetScale | Neki</a></li>
<li><a href="https://pganalyze.com/blog/5mins-distributed-postgres">The different trade-offs of Distributed Postgres architectures</a></li>

</ul>
</details>

**Discussion**: Sentiment was notably critical: one top comment complained the launch post never clearly explained what Neki actually is or what it is for, while another defended the tech but called the CEO an 'asshole.' Several commenters contrasted Neki's closed-source status unfavorably with Supabase's open-source Multigres, and others pressed on whether eventual consistency can satisfy HA Postgres workloads given CAP theorem constraints.

**Tags**: `#postgres`, `#distributed-systems`, `#databases`, `#planetscale`, `#sharding`

---

<a id="item-11"></a>
## [348M model trained on 22.7B tokens handles 14-digit arithmetic](https://www.reddit.com/r/MachineLearning/comments/1wc7hmu/i_trained_a_348m_model_trained_from_scratch_on/) ⭐️ 7.0/10

An independent developer released a 348M-parameter language model trained from scratch on 22.7B tokens and then fine-tuned to solve arithmetic by explicitly showing worked columns, reporting a 99.4% average across nine GPT-3 arithmetic sub-tasks. The model reportedly beats GPT-3 175B's few-shot direct-answer scores on several tasks — for example 100% vs 25.5% on 4-digit addition and 100% vs 29.2% on 2-digit multiplication — and, after the author expanded a fixed list of place-value names from 6 to 19 entries, its clean addition ceiling rose from 8 digits to 14. It is a striking demonstration that arithmetic ability in language models is largely a question of training data and output format rather than raw parameter count, since a model roughly 500 times smaller than GPT-3 175B can dominate it on column arithmetic when it is trained to show its work. This supports the broader trend toward small, task-specialized language models and reinforces why chain-of-thought style step-by-step generation has become a standard technique for reasoning tasks. The gains are narrow: the model scores only 4% on GSM8K word problems and 16.5% on ASDiv, with failures driven by operation selection rather than calculation, and it cannot do division at all or 4x4 multiplication. It also requires greedy decoding because sampling corrupts the column routine mid-chain, and the author flags that the arithmetic harness orders subtraction operands, meaning the subtraction table does not reflect unordered operand inputs.

reddit · r/MachineLearning · /u/nkthebass · Sep 10, 03:28

**Background**: GPT-3's original 2020 paper included a set of arithmetic benchmarks (2- to 5-digit addition, subtraction and 2-digit multiplication) evaluated in few-shot settings, where the model is given a handful of examples in the prompt and must answer directly without a calculator. Chain-of-thought prompting, introduced by Wei et al. in 2022, instead asks a model to produce intermediate reasoning steps before the final answer, which markedly improves performance on multi-step tasks. This project applies that idea at the training stage — the model is fine-tuned on worked column arithmetic with carries and borrows — rather than only at the prompt level, and it also illustrates how tokenization and vocabulary choice, such as the availability of names for each place value, can silently cap a model's numeric range.

<details><summary>References</summary>
<ul>
<li><a href="https://www.promptingguide.ai/techniques/cot">Chain-of-Thought Prompting | Prompt Engineering Guide</a></li>
<li><a href="https://github.com/openai/gpt-3">GitHub - openai/gpt-3: GPT-3: Language Models are Few-Shot Learners · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Few-shot_learning">Few-shot learning</a></li>

</ul>
</details>

**Tags**: `#small language models`, `#arithmetic reasoning`, `#chain-of-thought`, `#model training`, `#benchmarks`

---

<a id="item-12"></a>
## [Fly connectome fails to learn Pong, and the audit is the real story](https://www.reddit.com/r/MachineLearning/comments/1wc67ci/i_tried_to_make_a_real_fly_connectome_learn_to/) ⭐️ 7.0/10

A researcher tried to train a small real subgraph of the newly released MaleCNS v1.0 fly connectome (166k neurons from real EM reconstruction) to play Pong using dopamine-style plasticity, and it failed to learn. Auditing the failure surfaced a neuPrint regex bug that silently zeroed out two entire neuron populations, a selection with no path from photoreceptors to downstream circuits, and four motor neurons half of which had zero synapses from any sensory pathway. This is a rare, well-documented negative result in a field currently dominated by viral demo clips, and it suggests that several high-profile 'fly brain plays Doom/Minecraft/Beat Saber' projects have not actually passed their own validation gates. It matters for computational neuroscience and ML reproducibility because it shows that connectivity audits, not gameplay footage, are what distinguish real emergent behavior from hand-injected fallbacks. Even after rebuilding the pipeline, learning-on and learning-off runs produced bit-for-bit identical results across multiple seeds while weights verifiably changed, because two of four motor neurons had zero sensory input and had been assigned to the 'paddle down' group purely by array index. The eventual divergence looked like the learning rule globally quieting the system — punishment dominated since misses outnumbered hits — rather than any skill improvement.

reddit · r/MachineLearning · /u/oPeraza2007 · Sep 10, 02:28

**Background**: Connectomes are complete maps of the neurons in a brain and the synapses between them; the MaleCNS v1.0 release is a male adult fly central nervous system dataset with about 166,000 neurons reconstructed from electron microscopy. neuPrint is the query tool and API most researchers use to search these neurons and their connectivity, so bugs in its matching semantics can silently corrupt any downstream simulation. Dopamine-style plasticity is a biologically inspired learning rule in which reward or punishment signals modulate synaptic weights, and Pong is used here as a deliberately unforgiving test because it yields only a binary hit-or-miss signal each frame.

<details><summary>References</summary>
<ul>
<li><a href="https://male-cns.janelia.org/release/">Release Notes - MaleCNS connectome</a></li>
<li><a href="https://github.com/connectome-neuprint/neuPrint">GitHub - connectome-neuprint/neuPrint: tools for importing ...</a></li>
<li><a href="https://arxiv.org/html/2512.07194v1">Synchrony-Gated Plasticity with Dopamine Modulation for Spiking Neural ...</a></li>

</ul>
</details>

**Tags**: `#connectomics`, `#computational neuroscience`, `#machine learning`, `#negative results`, `#neuromorphic computing`

---

<a id="item-13"></a>
## [Sante's 83.83 on DiagnosisArena-MCQ Measures Only Answer Selection](https://www.reddit.com/r/MachineLearning/comments/1wbkxsa/what_santes_8383_on_diagnosisarenamcq_actually/) ⭐️ 6.0/10

A Reddit analysis by /u/Expert_Coffee_203 argues that the 83.83 score Ant Ling reports for Ling-3.0-flash-Sante on DiagnosisArena-MCQ only reflects the model's ability to pick one of four supplied diagnoses when case information, examinations and test results are already provided. The post also lists the release's two other medical results — MedXpertQA-Text 53.88 and HealthBench Professional 45.73 — and stresses that none of the three demonstrates unrestricted differential generation, missing-history detection or next-investigation planning. Benchmark numbers are frequently quoted as headline evidence of clinical competence, so clarifying that this one is a constrained multiple-choice task helps developers and buyers avoid over-reading it when choosing a model for real diagnostic workflows. The distinction is especially consequential for case-answering applications, where the first design decision is whether users supply the candidate diagnoses or expect the model to construct them. The post notes that the published Sante chart does not give enough scoring detail to tell whether the reported HealthBench Professional value is length-adjusted or unadjusted, so any comparison against another published HBP number should verify that first; HealthBench Professional is also rubric-graded by physicians rather than a percentage-accuracy metric, and its definition covers care consultation, writing/documentation and medical research.

reddit · r/MachineLearning · /u/Expert_Coffee_203 · Sep 9, 13:01

**Background**: DiagnosisArena is a benchmark designed to evaluate diagnostic reasoning in large language models, and it includes a multiple-choice variant (DiagnosisArena-MCQ) so results can be compared with traditional exam-style benchmarks. Ling-3.0-flash-Sante is a health- and medicine-focused Mixture-of-Experts model from InclusionAI (Ant), built on Ling-3.0-Flash with 124 billion total parameters but only about 5.1 billion activated per token, and it is reported to outperform several larger frontier models on this MCQ benchmark. MedXpertQA-Text is the text-only subset of MedXpertQA, a board-level medical QA benchmark of 4,460 questions spanning 17 specialties and 11 body systems, while HealthBench Professional measures open-ended clinical chat judged against physician-written rubrics.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2505.14107">DiagnosisArena : Benchmarking Diagnostic Reasoning for Large...</a></li>
<li><a href="https://novita.ai/models/model-detail/inclusionai-ling-3.0-flash-sante">Ling 3 . 0 Flash Sante API & Playground | Novita AI</a></li>
<li><a href="https://github.com/TsinghuaC3I/MedXpertQA">GitHub - TsinghuaC3I/MedXpertQA: [ICML 2025] MedXpertQA: Benchmarking Expert-Level Medical Reasoning and Understanding · GitHub</a></li>

</ul>
</details>

**Tags**: `#medical-ai`, `#benchmarking`, `#evaluation-methods`, `#LLM-reasoning`, `#machine-learning`

---