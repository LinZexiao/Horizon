---
layout: default
title: "Horizon Summary: 2026-09-23 (EN)"
date: 2026-09-23
lang: en
---

> From 34 items, 22 important content pieces were selected

---

1. [OpenAI launches GPT-6 Sol and Luna with sharply lower pricing](#item-1) ⭐️ 9.0/10
2. [Anthropic Ships Claude Opus 5.5 With Capability Gains and Price Cuts](#item-2) ⭐️ 9.0/10
3. [Pentagon: AI Overreliance Contributed to Deadly Iran School Strike](#item-3) ⭐️ 9.0/10
4. [Anthropic's Claude Opus 5.5 and OpenAI's GPT-6 Sol, Luna Spark Price War](#item-4) ⭐️ 9.0/10
5. [ShinyHunters claims theft of all FBI employee data, threatens coercion](#item-5) ⭐️ 8.0/10
6. [Trail of Bits Argues SAML Is Fundamentally Broken by Design](#item-6) ⭐️ 8.0/10
7. [WordPress core unauthenticated path traversal can lead to conditional RCE](#item-7) ⭐️ 8.0/10
8. [TypeSafe AI's Jev Returns Typed Decisions Instead of Generated Text](#item-8) ⭐️ 8.0/10
9. [Cloudflare Python Workers reach general availability after two-year preview](#item-9) ⭐️ 8.0/10
10. [OpenAI GPT-6 Astra Helps Researcher Crack Long-Unsolved Enigma Message](#item-10) ⭐️ 7.0/10
11. [Developer revives Visual FoxPro 9 on a Rust/WASM runtime](#item-11) ⭐️ 7.0/10
12. [California Tests Solar Panels Over Irrigation Canals](#item-12) ⭐️ 7.0/10
13. [Artificial Analysis benchmarks Claude Opus 5.5 reasoning tiers, sparking price-performance debate](#item-13) ⭐️ 7.0/10
14. [Unreal Agent: Open-Source Harness Pushes Programmatic Tool Calling](#item-14) ⭐️ 7.0/10
15. [Xiaomi releases MiMo-V2.6 multimodal models with public RL cost and live dashboards](#item-15) ⭐️ 7.0/10
16. [Complex KDA Extends Kimi Delta Attention's Expressivity via Wider Gates](#item-16) ⭐️ 7.0/10
17. [LLM 0.36 adds GPT-6 Sol/Luna support and non-conversational model flag](#item-17) ⭐️ 6.0/10
18. [llm-typesafe 0.1a0 brings TypeSafe's Jev model to the LLM CLI](#item-18) ⭐️ 6.0/10
19. [LinearSolveBench: New Benchmark for Model-Written Sparse Linear Solvers](#item-19) ⭐️ 6.0/10
20. [Templar simulates fault tolerance via stage skipping in pipeline-parallel training](#item-20) ⭐️ 6.0/10
21. [AI "Sandbox Escapes" Were Sloppy Firewall Failures, Not Air Gap Breaches](#item-21) ⭐️ 6.0/10
22. [Qonto releases QontoFAQ benchmark for product FAQ retrieval](#item-22) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [OpenAI launches GPT-6 Sol and Luna with sharply lower pricing](https://openai.com/index/introducing-gpt-6-sol-and-luna/) ⭐️ 9.0/10

OpenAI announced GPT-6 Sol and Luna, a new flagship model family that succeeds the GPT-5.6 generation. According to Simon Willison, GPT-6 Luna is priced at roughly half of what GPT-5.6 Luna cost, a change he calls "a really big deal." A flagship OpenAI release that halves a key tier's price directly reshapes the economics of AI coding agents and API-based products, forcing comparison with competing tools such as Anthropic's Claude Code and OpenAI's own Codex. Developers weighing subscription tiers and per-token costs will feel the impact immediately. The family appears to span multiple tiers, with Luna as the cheaper option and Sol as the higher-end model (commenters also reference a "GPT-6 Sol max" variant). Community discussion stresses that practical usage limits are downstream of input/output token costs, so headline pricing does not automatically translate into more work per dollar.

hackernews · OfficialTurkey · Sep 22, 18:00 · [Discussion](https://news.ycombinator.com/item?id=49805509)

**Background**: OpenAI ships frontier language models in named generations and tiers, and developers access them either through the API (billed per token) or through consumer subscriptions such as ChatGPT Plus and coding-agent plans like Codex Pro. Because agentic coding tools burn tokens continuously, model pricing and usage limits have become a central competitive battleground. A recurring community benchmark is the "pelican test," in which a model is asked to draw a pelican riding a bicycle as SVG code, used as a quick proxy for code generation and instruction-following quality.

**Discussion**: Commenters focused on three themes: Simon Willison highlighted Luna's halved price as the headline change and shared pelican-test outputs for Sol and Luna; m_fayer described an unusual attachment to the previous 5.6 Sol, worrying that a technically better successor may "feel" less natural to work with; and jeffnash argued that on usage limits and plan math, Codex Pro 20x currently beats Claude Code 20x by a mile, especially since ChatGPT usage is effectively unmetered. leokennis offered a counterpoint from the mainstream user's view, saying ChatGPT Plus has felt essentially limitless and "just works" since 5.6.

**Tags**: `#AI`, `#LLM`, `#OpenAI`, `#model-release`, `#pricing`

---

<a id="item-2"></a>
## [Anthropic Ships Claude Opus 5.5 With Capability Gains and Price Cuts](https://www.anthropic.com/claude-opus-5-5) ⭐️ 9.0/10

Anthropic released Claude Opus 5.5, described as its first model release since it publicly called for slowing the race to the AI frontier, and paired the launch with across-the-board price reductions — cache reads fell from $0.50 to $0.20 per million tokens, input from $5 to $4, output from $25 to $20, and cache writes from $6.25 to $5. The announcement drew 1,184 upvotes and 804 comments on Hacker News, making it one of the most discussed model launches of the period. Opus 5 was reportedly the highest-spend model on OpenRouter, so cutting cached-read prices by 60% and output prices by 20% lowers the cost floor for long-running agentic and coding workloads, and puts pressure on rival labs to match. The release also sharpens the contradiction critics see between Anthropic's safety-first messaging about pacing the frontier and its continued aggressive shipping cadence. Anthropic claims Opus 5.5 "communicates more naturally" than Opus 5, puts the most important information up front, and is easier to follow and verify over long sessions, which the company frames as both a practical and a safety benefit. Notably, most of the capability evidence in the announcement and discussion is anecdotal — early-tester impressions and side-by-side demos rather than headline benchmark scores.

hackernews · km144 · Sep 22, 16:29 · [Discussion](https://news.ycombinator.com/item?id=49803892)

**Background**: Anthropic's Responsible Scaling Policy defines AI Safety Levels (ASL) that gate how much capability it will deploy, and the revised version 3.0 of February 2026 replaced the original "hard pause" trigger with tiered ASL-3 security standards and a public Frontier Safety Roadmap. "Pacing the frontier" refers to the company's stated willingness to slow down frontier development for safety reasons, which is why reviewers scrutinize each new release against that pledge. LLM API pricing is quoted in cost per million tokens, where output tokens typically cost several times more than input tokens and cached reads are the cheapest path, so a cache-read price cut is the most consequential line for high-volume users.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/responsible-scaling-policy">Anthropic’s Responsible Scaling Policy</a></li>
<li><a href="https://aiinsightsnews.net/anthropic-responsible-scaling-policy-2026-asl3/">Anthropic RSP 2026 Explained: ASL-3, Frontier Safety Roadmap ...</a></li>
<li><a href="https://siliconanalysts.com/data/llm-pricing">LLM API Pricing — $ per Million Tokens by Model (2026)</a></li>

</ul>
</details>

**Discussion**: The dominant sentiment was pointed irony: top comments noted that Anthropic opened the announcement by recalling its call to pace the frontier, then spent the rest of the post demonstrating with specific numbers that it is doing the opposite. Commenters verified capability gains hands-on by re-running a pelican 3D-animation prompt against both Opus 5.5 and Opus 5 and reporting "significant improvement," and broadly welcomed the price drops, while some pushed back on model choice — one user said they were content staying on DeepSeek v4.1.

**Tags**: `#AI`, `#LLM`, `#Anthropic`, `#Claude`, `#Model Release`

---

<a id="item-3"></a>
## [Pentagon: AI Overreliance Contributed to Deadly Iran School Strike](https://www.bloomberg.com/graphics/2026-iran-school-attack/) ⭐️ 9.0/10

A Pentagon report concluded that overreliance on AI-assisted targeting contributed to a U.S. missile strike on a school in Iran, finding that the United States "failed in its obligation to do everything feasible to verify" that the school was a military objective and that the failure "went beyond mere negligence." According to reporting summarized in the discussion, the Minab site had been cataloged as an Islamic Revolutionary Guard Corps facility based on outdated data and was fed into the Maven system, where it emerged as a recommended day-one target. This is one of the most explicit official acknowledgments that AI-enabled targeting pipelines can contribute to civilian casualties, putting military AI accountability, human oversight, and the governance of lethal autonomous weapons squarely on the policy agenda. It is likely to intensify scrutiny of systems like Maven and shape debates over how much authority militaries should delegate to machine-generated target recommendations. The report's finding hinges on process rather than full autonomy: target-list work that once took hours was reportedly compressed into minutes, with Maven surfacing the site as a recommended target from a pool of candidates, which critics describe as optimizing speed instead of verification. The incident also fits the pattern of automation bias, in which human operators favor suggestions from automated systems and discount contradictory evidence, even though a human remained formally in the loop.

hackernews · devonnull · Sep 22, 19:03 · [Discussion](https://news.ycombinator.com/item?id=49806430)

**Background**: Project Maven is a U.S. Department of Defense effort that applies machine learning to analyze imagery and sensor data and to help generate targeting candidates; its outputs are meant to assist, not replace, human decision-makers. Automation bias is a well-documented cognitive effect in which people over-trust automated recommendations, observed in domains from aviation cockpits to intensive care units and nuclear power plants. In the weapons debate, "human-in-the-loop" describes a system where a human must authorize engagement, as opposed to lethal autonomous weapons systems (LAWS) that can select and engage targets without manual human control.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Automation_bias">Automation bias</a></li>
<li><a href="https://en.wikipedia.org/wiki/Human-in-the-loop">Human-in-the-loop - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Lethal_autonomous_weapons_systems">Lethal autonomous weapons systems</a></li>

</ul>
</details>

**Discussion**: Commenters were sharply divided: some argued that "AI" is not really the culprit and that the report's language points to command responsibility and reckless disregard rather than a machine failure, while others stressed that compressing target-list work from hours to minutes means optimizing the wrong metric. A recurring counterargument was that the ratio of correct to incorrect targets in this campaign (roughly 3 errors out of some 13,000 strikes) is better than any historical aerial campaign, and one commenter cited a related incident in which the U.S. nearly boarded a Chinese vessel that AI had incorrectly flagged as carrying nuclear-weapons materiel.

**Tags**: `#AI ethics`, `#military AI`, `#autonomous weapons`, `#accountability`, `#geopolitics`

---

<a id="item-4"></a>
## [Anthropic's Claude Opus 5.5 and OpenAI's GPT-6 Sol, Luna Spark Price War](https://simonwillison.net/2026/Sep/22/opus-and-sol-and-luna/) ⭐️ 9.0/10

On September 22, 2026, Anthropic released Claude Opus 5.5, and roughly an hour later OpenAI released two new frontier models, GPT-6 Sol and GPT-6 Luna. According to Simon Willison, GPT-6 Luna costs $0.10 per million input tokens and $0.50 per million output tokens — exactly half the price of its GPT-5.6 Luna predecessor — while GPT-6 Sol also saw a comparable price reduction. The simultaneous launches plus steep price cuts signal an intensifying price war among frontier labs, directly lowering the cost of building LLM-powered applications for developers. GPT-6 Sol being priced identically to GPT-5.6 Terra effectively removes any remaining reason to keep using Terra, and Grok 4.7's earlier pricing advantage over OpenAI has now largely evaporated. OpenAI's new pricing is even more aggressive than it first appears: GPT-5.6 models have a scheduled 25% price increase coming in November, so GPT-6 is half the price of the promotional pricing for those older models. At $0.10/$0.50, GPT-6 Luna is one of the cheapest models OpenAI has ever shipped, beaten only by the far weaker GPT-4.1 Nano ($0.10/$0.40) and GPT-5 Nano ($0.05/$0.40).

rss · Simon Willison · Sep 22, 23:46

**Background**: Frontier LLM APIs are typically priced per million tokens, with separate rates for input, cached input, and output; caching repeated context is much cheaper, which is why cached input rates in the table are far lower. Simon Willison, a well-known developer and blogger, tracks new model releases and popularized the informal 'pelican on a bicycle' benchmark, in which models are asked to generate an SVG of a pelican riding a bicycle to test code generation and visual coherence. Anthropic's Claude line is split into Haiku, Sonnet, and Opus tiers, with Opus being the most capable, while OpenAI's GPT naming has expanded into a family of named variants such as Sol, Luna, Terra, and Astra.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/claude-opus-5-5">Introducing Claude Opus 5 . 5 \ Anthropic</a></li>
<li><a href="https://github.com/simonw/pelican-bicycle">GitHub - simonw/pelican-bicycle: LLM benchmark: Generate an ...</a></li>
<li><a href="https://mimo.xiaomi.com/mimo-v2-6">MiMo-V2.6 | Xiaomi</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#Anthropic`, `#OpenAI`, `#AI pricing`, `#model releases`

---

<a id="item-5"></a>
## [ShinyHunters claims theft of all FBI employee data, threatens coercion](https://www.404media.co/we-hacked-the-fbi-hackers-say-they-have-data-on-all-fbi-employees/) ⭐️ 8.0/10

A hacking group identifying itself with ShinyHunters claims to have stolen data on all FBI employees, telling 404 Media that its plans amount to "coercion" rather than financially motivated extortion. The claim, which has not been confirmed by the FBI, has triggered widespread discussion about federal data security. If verified, a breach exposing the personal data of every FBI employee would rank among the most sensitive US government data incidents, potentially enabling targeting, harassment, or recruitment of agents by foreign intelligence. Even unverified claims like this embolden extortion groups and increase pressure on agencies to overhaul their data-handling and identity-protection practices. The group explicitly told 404 Media that the operation is "not financially motivated" and that what it plans is "not something I'd call extortion, maybe coercion," suggesting a politically or ideologically driven motive rather than a ransom demand. The FBI has not publicly confirmed the breach, so the scope and authenticity of the stolen data remain unverified.

hackernews · spenvo · Sep 22, 17:46 · [Discussion](https://news.ycombinator.com/item?id=49805278)

**Background**: ShinyHunters is a black-hat criminal hacking and extortion group active since 2019 that has been linked to a long string of large data breaches, including the recent theft of roughly 6.65 terabytes of Canvas data and claims of selling close to 200 million stolen records. The news item's only source link is an archive.ph snapshot, a service that preserves copies of web pages for later reference. Such claims are common in the extortion economy, where groups often exaggerate the scale of stolen data to maximize leverage.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ShinyHunters">ShinyHunters - Wikipedia</a></li>
<li><a href="https://www.wired.com/story/shinyhunters-hacking-group-data-breach-spree/">ShinyHunters Is a Hacking Group on a Data Breach Spree | WIRED</a></li>
<li><a href="https://webcurate.co/archive-ph">Archive . ph - WebCurate</a></li>

</ul>
</details>

**Discussion**: Commenters were largely skeptical and darkly humorous, arguing that no organization seems able to safeguard a large database and pointing to the 2015 OPM breach that exposed 22.1 million US government employee records. Others framed the incident as a symptom of eroding institutional expertise and security culture, with jokes about hackers being added to a Signal group chat or about air-gapped systems in Battlestar Galactica, and one commenter mocked the group's "coercion, not extortion" framing.

**Tags**: `#cybersecurity`, `#data breach`, `#FBI`, `#ShinyHunters`, `#privacy`

---

<a id="item-6"></a>
## [Trail of Bits Argues SAML Is Fundamentally Broken by Design](https://blog.trailofbits.com/2026/09/21/saml-a-fractal-of-bad-design/) ⭐️ 8.0/10

Trail of Bits published a blog post titled "SAML: A fractal of bad design" arguing that the Security Assertion Markup Language is not merely buggy in individual implementations but structurally flawed at the protocol level, comparing its problems to the famous critiques of XML and other over-engineered standards. The post drew 149 points and 86 comments on Hacker News, where practitioners traded concrete signature-verification horror stories and debated whether OpenID Connect actually offers a meaningful security improvement for enterprise single sign-on. SAML remains the backbone of enterprise single sign-on across thousands of applications, so structural design flaws translate directly into authentication-bypass risk at scale rather than being an academic concern. The debate also highlights a practical tension for vendors: OIDC is widely seen as the eventual successor, yet SAML's stable if mediocre subset still supports enterprise features such as IdP-initiated flow that OIDC handles inconsistently. Commenters pointed to specific implementation traps, including a C implementation of XML signature verification that by default would also accept an HMAC computed with an attacker-supplied password from the document itself, and would validate signatures against the web PKI so that a document signed with an attacker's own TLS certificate for their personal domain would pass. The article's critics noted it catalogs SAML's weaknesses without applying the same scrutiny to OIDC, which suffers from JWT algorithm confusion, "none" algorithm attacks, missing audience checks, and bugs in JOSE libraries.

hackernews · aray07 · Sep 22, 18:57 · [Discussion](https://news.ycombinator.com/item?id=49806335)

**Background**: SAML 2.0, standardized by OASIS in 2005, is an XML-based protocol for exchanging authentication and authorization data between an identity provider and a service provider — the mechanism behind "log in with your company account" for many enterprise apps. Because it relies on XML Signature, it inherits that standard's notorious complexity: the signature covers an element referenced by an ID, and canonicalization plus XPath reference resolution has repeatedly allowed XML Signature Wrapping attacks, in which an attacker restructures the document so a valid signature covers a different element than the one the application actually processes. OpenID Connect, built on OAuth 2.0 and JSON Web Tokens instead of XML, was designed as a simpler alternative and is often recommended for new applications, though it is really a constellation of specs with uneven vendor support.

<details><summary>References</summary>
<ul>
<li><a href="https://cheatsheetseries.owasp.org/cheatsheets/SAML_Security_Cheat_Sheet.html">SAML Security - OWASP Cheat Sheet Series SAML Security Testing: SSO Vulnerabilities, XML Signature ... SAML Vulnerabilities and Attacks: A Practical Guide Common SAML vulnerabilities and how to remediate them - Snyk Common SAML security vulnerabilities and how to defend ...</a></li>
<li><a href="https://www.ibm.com/think/topics/xml-signature-wrapping">What is XML Signature Wrapping? | IBM</a></li>
<li><a href="https://learn.microsoft.com/en-us/entra/identity/enterprise-apps/saml-vs-oidc-decision-guide">SAML versus OpenID Connect: Choose the right SSO protocol</a></li>

</ul>
</details>

**Discussion**: Commenters largely agreed with the thesis but pushed back on its completeness: one called SAML a product of the era when "markup languages were the hammer for everything," while others stressed that OIDC is not automatically better and that SAML's commonly implemented subset still wins on enterprise features like IdP-initiated flow. Several argued the pragmatic answer is to support both protocols, since real integration pain often lies elsewhere — notably SCIM provisioning — and one commenter noted rising optimism about newer alternatives to the XML-based stack.

**Tags**: `#SAML`, `#security`, `#authentication`, `#OIDC`, `#XML`

---

<a id="item-7"></a>
## [WordPress core unauthenticated path traversal can lead to conditional RCE](https://github.com/WordPress/wordpress-develop/security/advisories/GHSA-7hp8-65ch-5whp) ⭐️ 8.0/10

A GitHub security advisory (GHSA-7hp8-65ch-5whp) in the WordPress core repository discloses an unauthenticated path traversal flaw that can escalate to remote code execution under certain conditions, and the fix has been backported to every branch as far back as WordPress 4.7. Because WordPress powers more than 40% of the web, an unauthenticated flaw that can be exploited without any credentials or user interaction puts an enormous number of sites at risk, and the unusually deep backport down to version 4.7 signals that the maintainers consider legacy installations especially exposed. The advisory describes the impact as "conditional" RCE, meaning exploitation depends on additional preconditions such as how a site or plugin passes user-controlled input into template-loading logic; notably, a nine-year-old documentation comment on the affected locate_template() function already warned that it does not prevent directory traversal, and the community identified the fix as commit 9c4e85 in the wordpress-develop repository.

hackernews · vntok · Sep 22, 16:33 · [Discussion](https://news.ycombinator.com/item?id=49803959)

**Background**: A path traversal (or directory traversal) vulnerability exploits insufficient validation of user-supplied file names, letting characters such as "../" escape the intended directory and reach other files on the file system. Remote code execution is the ability of an attacker to run arbitrary code on a target machine over a network, and it represents the most severe class of software vulnerability. WordPress is a widely used open-source content management system, and its theming system resolves template file names at runtime through functions like locate_template(); if such a function is handed attacker-controlled input without strict validation, a traversal can reach files that the attacker can influence, which is what turns the bug into a code-execution risk.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Path_traversal_vulnerability">Path traversal vulnerability</a></li>
<li><a href="https://en.wikipedia.org/wiki/Remote_code_execution">Remote code execution</a></li>

</ul>
</details>

**Discussion**: Commenters were largely critical, noting that roughly a third of WordPress installs are not on the latest branch and arguing that WordPress is among the most-exploited software on the web; some shared the concrete patch commit and the nine-year-old locate_template() documentation comment that predicted this exact flaw, while others said the incident pushed them to migrate to statically hosted site generators such as Hugo.

**Tags**: `#WordPress`, `#security`, `#vulnerability`, `#RCE`, `#path traversal`

---

<a id="item-8"></a>
## [TypeSafe AI's Jev Returns Typed Decisions Instead of Generated Text](https://simonwillison.net/2026/Sep/21/jev/) ⭐️ 8.0/10

TypeSafe AI unveiled Jev on 15 September 2026, the first of what it calls "System One models" (Simon Willison and Maggie Appleton prefer the term "decision models"). Jev accepts text or semi-structured "state" input but returns floating point numbers — Bernoulli-style yes/no confidence, a probability distribution over provided choices, or a score along a numeric range — rather than generated text, and charges only $0.042 per million input tokens with free output. If decision models catch on, they could replace a large class of LLM use cases — spam detection, labeling, triage, ranking, search reranking — with something faster, cheaper and directly consumable by software, removing the parsing overhead of conversational agents. It also reflects a broader split in the ecosystem between fast, bounded inference primitives and general-purpose text-generating models. Jev exposes three question types: "Noul" yes/no questions (short for Bernoulli, confirmed by the CEO on Hacker News), choice questions returning a confidence score plus a distribution over options, and score questions over a described numeric scale; a single state can carry many questions that are evaluated in parallel, so latency barely grows with question count. Its own "jaggedness" documentation admits weaknesses with numbers, dates and adversarial content, and Jev gives no rationale for a decision — you get a float, not an explanation.

rss · Simon Willison · Sep 21, 23:09

**Background**: "System One" borrows from Daniel Kahneman's dual-process theory, in which System 1 thinking is fast, intuitive and automatic while System 2 is slow and deliberate; here the label signals cheap, low-latency inference rather than deep reasoning. Regular LLMs are priced per input and output token, with output typically costing much more, and they emit natural language that software must parse before acting. A decision model instead compresses the whole task into a bounded, typed output such as a probability or a category label, which makes it a better fit as a learned decision primitive inside an application's control flow.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Jev_(AI_model)">Jev (AI model) - Wikipedia</a></li>
<li><a href="https://typesafe.ai/blog/introducing-system-one-models-and-jev">Introducing System One Models & Jev - TypeSafe AI Blog</a></li>
<li><a href="https://mchromiak.github.io/articles/2026/Sep/17/Jev-Typed-Decisions-for-Enterprise-AI/">Jev: Typed decisions for enterprise AI - Michał Chromiak's blog</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#AI models`, `#decision models`, `#TypeSafe AI`, `#Jev`

---

<a id="item-9"></a>
## [Cloudflare Python Workers reach general availability after two-year preview](https://simonwillison.net/2026/Sep/21/cloudflare-python-worker/) ⭐️ 8.0/10

Cloudflare has announced that Python Workers are now generally available, making Python a "first-class, fully supported language on the Cloudflare Developer Platform" after roughly two years in preview. The announcement is credited to Gyeongjae Choi, Dominik Picheta and Hood Chatham, two of whom are Pyodide core maintainers. Python is one of the world's most widely used languages, so making it a stable, first-class option on a major serverless edge platform meaningfully expands what developers can deploy close to users without leaving the Python ecosystem. It also signals deeper investment by Cloudflare in the Pyodide/WebAssembly toolchain, which benefits the broader Python-in-the-browser community. Because Python runs as WebAssembly inside Cloudflare's V8-based workerd runtime, some standard library capabilities do not work: notably `multiprocessing` and `threading` are non-functional in the WebAssembly VM. Local development is handled by the pywrangler CLI tool (published on PyPI as `workers-py`), which simulates the whole stack locally by executing Pyodide-in-WebAssembly-in-V8 inside a 123MB `workerd` binary.

rss · Simon Willison · Sep 21, 22:25

**Background**: Cloudflare Workers is a serverless platform that runs code on Cloudflare's global edge network, powered by the open-source workerd runtime, which executes JavaScript and WebAssembly and is built on the V8 engine. Pyodide is a port of CPython to WebAssembly (via Emscripten), originally created in 2018 by Michael Droettboom at Mozilla for the Iodide project; it lets Python and many C/C++/Rust-extension packages such as NumPy, pandas and scikit-learn run inside a JavaScript host. By combining the two, Cloudflare can run Python code inside workerd without a separate native Python interpreter.

<details><summary>References</summary>
<ul>
<li><a href="https://pyodide.org/en/stable/project/about.html">What is Pyodide? — Version 314.0.7</a></li>
<li><a href="https://blog.cloudflare.com/workerd-open-source-workers-runtime/?ref=console.dev/">Introducing workerd : the Open Source Workers runtime</a></li>
<li><a href="https://github.com/pyodide/pyodide">GitHub - pyodide/pyodide: Pyodide is a Python distribution ... Home - Pyodide About Us - Pyodide What Is Pyodide? Definition & Examples - nhimg.org pyodide | Pyodide is a Python distribution for the browser ...</a></li>

</ul>
</details>

**Tags**: `#Cloudflare Workers`, `#Python`, `#WebAssembly`, `#Serverless`, `#Pyodide`

---

<a id="item-10"></a>
## [OpenAI GPT-6 Astra Helps Researcher Crack Long-Unsolved Enigma Message](https://www.cryptocellar.org/bgac/the-mvueh-break.html) ⭐️ 7.0/10

OpenAI's GPT-6 Astra reportedly assisted a researcher in decrypting a historic Enigma message that had resisted solution since 2005, in what is described as a two-day collaboration between the researcher and the model. Astra generated Enigma simulator software in Python and C++ and provided cryptanalytic insights that, combined with human work, yielded the plaintext. This is one of the more visible public demonstrations of LLM-assisted cryptanalysis, and it has ignited debate over how much credit the AI deserves versus the human researcher and the standard tooling the model generated. It also feeds a broader industry conversation about whether frontier models are becoming genuine scientific research partners or merely fast code generators and search aids. Community members note that the message used a completely different key from the rest of that day's traffic, that the original transcription contained errors, and that the left rotor turned over at letter 72, an event rare enough to defeat standard crib attacks. One commenter also claims Gemini 3.8 Flash reportedly decrypted the same ciphertext in a roughly 45-minute non-steered run, raising questions about the uniqueness of Astra's contribution.

hackernews · sohkamyung · Sep 22, 13:52 · [Discussion](https://news.ycombinator.com/item?id=49801324)

**Background**: Enigma was the German rotor cipher machine whose traffic was broken during World War II by Allied cryptanalysts including Alan Turing at Bletchley Park, a story popularized by films and documentaries. Some historic intercepts remain unsolved decades later because of transcription mistakes, unusual key settings, or lost daily key sheets. GPT-6 Astra is OpenAI's newest flagship large language model, released in September 2026 and marketed for state-of-the-art computer use, coding, cybersecurity, and science capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cryptanalysis_of_the_Enigma">Cryptanalysis of the Enigma - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-6_Astra">GPT-6 Astra - Wikipedia</a></li>
<li><a href="https://openai.com/index/gpt-6-astra/">GPT-6 Astra: A new generation of intelligence | OpenAI</a></li>

</ul>
</details>

**Discussion**: Sentiment is skeptical and nuanced: several commenters argue the framing that Astra "did it entirely on its own" is incongruous with the fact that it generated standard Enigma simulator software, and they question how much of that tooling is novel. Others point out that a rival model (Gemini) reportedly solved the same message in under an hour, and one commenter proposes the corrected headline "Researcher breaks one specific stubborn historic enigma message with good help from Astra."

**Tags**: `#AI`, `#cryptography`, `#Enigma`, `#LLM`, `#codebreaking`

---

<a id="item-11"></a>
## [Developer revives Visual FoxPro 9 on a Rust/WASM runtime](https://foxscript.org/) ⭐️ 7.0/10

A developer has released FoxScript, a new runtime that keeps the Visual FoxPro 9 language and file formats working while replacing the original 32-bit engine with one written in Rust and compiled to WebAssembly. The project remains compatible with existing vfp9 code and legacy 32-bit .fll add-ins, but removes the classic 2 GB table-size limit and adds lambdas, JSON handling and a built-in HTTP server; it is licensed under MIT, reports are not yet implemented, and builds are unsigned. A large number of line-of-business applications written in FoxPro are still in production decades after Microsoft ended support, and rewriting them is usually more expensive than keeping them alive. A compatible drop-in runtime gives those shops a path to modern infrastructure — larger tables, WebAssembly portability and HTTP endpoints — without abandoning their existing code base. Compatibility is being validated by checking behavior against the real vfp9.exe binary, which gives the claim of drop-in compatibility some teeth. Notable caveats: reports are entirely missing, builds are unsigned, and the language extensions (lambdas, JSON, HTTP server) go beyond what vfp9 ever offered, so code relying on the old 2 GB constraint or on Microsoft-specific runtime internals may behave differently.

hackernews · boredjohnny · Sep 22, 21:00 · [Discussion](https://news.ycombinator.com/item?id=49808023)

**Background**: Visual FoxPro was a data-centric, object-oriented programming language and database IDE that Microsoft acquired with Fox Software in 1992. The final version, Visual FoxPro 9.0, shipped in December 2004 and was last patched with SP2 in October 2007; mainstream support ended in January 2010 and extended support in January 2015, and Microsoft never produced a .NET successor. WebAssembly, by contrast, is a portable binary instruction format standardized as a W3C recommendation in 2019, designed as a compilation target for high-performance code both on the web and outside it — which is what lets a Rust rewrite of a Windows-only x86 language run elsewhere. The .fll files referenced here are FoxPro's native 32-bit extension libraries, roughly analogous to DLLs, which the new runtime must still load.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Visual_FoxPro">Visual FoxPro</a></li>
<li><a href="https://en.wikipedia.org/wiki/WebAssembly">WebAssembly</a></li>

</ul>
</details>

**Discussion**: Commenters largely treated the revival as technically impressive but raised a serious security objection: the Database Container model stores stored procedures as plain text in a memo field, must be read/write for all users with no permission scheme, and can execute arbitrary FoxPro code including Win32 calls — meaning an INSERT trigger can be edited into a remote-code-execution vector. Others shared war stories about FoxPro file locking on network drives and a physician's office that had to be migrated to .NET client/server, while several reminisced about how easy and lucrative CRUD-era FoxPro development was.

**Tags**: `#Visual FoxPro`, `#legacy software`, `#WASM`, `#language runtime`, `#database`

---

<a id="item-12"></a>
## [California Tests Solar Panels Over Irrigation Canals](https://www.kqed.org/science/2002033/heres-what-california-is-learning-from-solar-panels-built-over-irrigation-canals) ⭐️ 7.0/10

California's Project Nexus pilot, built with the Turlock Irrigation District in Stanislaus County, has stretched solar panels over roughly 1.2 miles of irrigation canal, generating about 1.6 MW of power while early testing shows up to 70% less evaporation from the shaded water. It is the first US demonstration of "solar-over-canal" design at this scale, intended as a proof of concept for statewide deployment. The pilot is an applied test of the water-energy nexus: if it scales, it could resolve land competition between solar farms and agriculture, conserve scarce water, and cool the panels to raise their output, all on land the state already owns. It is relevant to California's roughly 4,000 miles of canals and to a grid that already draws 62% of its electricity from renewable and zero-carbon sources. Project Nexus was designed as a proof of concept funded on behalf of the state, with the irrigation district supplying its own canal infrastructure and grid interconnection as the test bed, so the results are still preliminary and limited to a small capacity. Community commenters also point out the practical tradeoffs: the mounting structures look massive and costly, the run requires additional cabling and copper rather than one long daisy-chained array, and panels must be serviced individually over water.

hackernews · Jtsummers · Sep 22, 03:10 · [Discussion](https://news.ycombinator.com/item?id=49796379)

**Background**: Aquavoltaics — placing solar panels above canals or other water bodies — is an emerging practice that aims to get double duty from the same surface: shade reduces evaporation and aquatic weed growth, while the cooler microclimate can improve photovoltaic efficiency, and no farmland or desert habitat is consumed. Prior modeling by researchers such as Brandi McKuin at UC Santa Cruz estimated that covering California's thousands of miles of canals could save tens of billions of gallons of water annually and generate substantial electricity. Canals and aqueducts are central to California's water system, carrying snowmelt from the north to cities and farms in the drier south, and who holds the water rights to that flow is a long-running political question.

<details><summary>References</summary>
<ul>
<li><a href="https://beiconstruction.com/solar-over-canal/">Project Nexus : Advancing Solar - Over - Canal Innovation in California</a></li>
<li><a href="https://www.goodnewsnetwork.org/california-scientists-suggest-covering-the-states-canals-in-solar-panels/">Huge Supply of Water is Saved From Evaporation When Solar Panels ...</a></li>
<li><a href="https://www.anthropocenemagazine.org/2021/03/the-two-for-one-benefits-of-solar-canals/">Irrigation canals covered in solar panels are a powerful combination</a></li>

</ul>
</details>

**Discussion**: Commenters were split on whether the design makes economic sense: one argued it would be cheaper to put the panels in a field and simply shade the canal, citing costly supports, extra copper and cabling. Others appreciated learning that 62% of California's electricity is renewable or zero-carbon, asked how the canal system and water rights came to be structured as they are, and raised concerns about whether panel materials could leach chemicals into the water over time; one reader also complained about the site geo-blocking access.

**Tags**: `#solar energy`, `#water infrastructure`, `#California`, `#renewable energy`, `#agriculture`

---

<a id="item-13"></a>
## [Artificial Analysis benchmarks Claude Opus 5.5 reasoning tiers, sparking price-performance debate](https://artificialanalysis.ai/models/claude-opus-5-5) ⭐️ 7.0/10

Artificial Analysis has published benchmark pages for Anthropic's Claude Opus 5.5 broken out by reasoning-effort setting, with separate pages for the "max", "xhigh" and default "medium" tiers, and the accompanying Hacker News thread drew 233 upvotes and 69 comments. Discussion focused on cost-per-task improvements, benchmark reliability after launch, and how the model stacks up against open-weight alternatives. For teams choosing a frontier model, the reported halving of cost per task versus Opus 5 at matched high effort directly changes the economics of agentic and long-running workloads. The thread also reflects wider industry skepticism about vendor-published benchmarks and post-launch quality regressions, plus the recurring argument that open-weight models are "good enough" at a fraction of the price. Artificial Analysis is an independent platform that benchmarks models on quality, price, output speed and latency, and Claude's effort tiers (low/medium/high/max) interact with a thinking-token budget, so the "max" setting can consume very large budgets. simonw reported that his "pelican riding a bicycle" SVG prompt exhausted the 128,000-token budget twice at max effort without producing a result.

hackernews · theanonymousone · Sep 22, 16:51 · [Discussion](https://news.ycombinator.com/item?id=49804316)

**Background**: Claude models expose an "effort" control that, together with a thinking-token budget, determines how much reasoning the model does before answering; higher effort generally improves quality but raises latency and cost. Artificial Analysis publishes continuously updated, vendor-independent evaluations that practitioners use to weigh quality against price, speed and latency. The "rug pull" concern refers to the worry that labs optimize models for launch-day benchmarks and then quietly change behavior later, while open-weight models are openly downloadable alternatives that are usually far cheaper to run.

<details><summary>References</summary>
<ul>
<li><a href="https://artificialanalysis.ai/">AI Model & API Providers Analysis | Artificial Analysis</a></li>
<li><a href="https://platform.claude.com/docs/en/build-with-claude/effort">Effort - Claude Platform Docs</a></li>
<li><a href="https://support.claude.com/en/articles/8664678-change-the-model-effort-and-thinking-settings">Change the model, effort, and thinking settings | Claude Help ...</a></li>

</ul>
</details>

**Discussion**: Sentiment mixes enthusiasm with skepticism: hglaser welcomed the roughly half cost per task versus Opus 5 at matched high effort, while simonw reported two practical failures to generate a pelican-on-a-bicycle SVG at max effort because the model burned through its 128,000-token budget. breckenedge warned that re-running evaluations weeks after launch can reveal regressions and accused providers of "pulling the rug", cmiles8 argued open-weight models are only slightly worse while costing around 100x less, and lhk931122 doubted the model is more capable than Fable and plans to test perceived performance directly.

**Tags**: `#LLM`, `#Claude`, `#AI benchmarks`, `#model pricing`, `#AI industry`

---

<a id="item-14"></a>
## [Unreal Agent: Open-Source Harness Pushes Programmatic Tool Calling](https://unreallabs.ai/blog/unreal-agent/) ⭐️ 7.0/10

Unreal Labs released Unreal Agent, an open-source AI agent harness, and published a blog post accompanied by a GitHub repository (unreallabsai/unreal-agent) that centers on programmatic tool calling and improved tool orchestration. The release drew a substantive Hacker News discussion comparing it with existing approaches such as DSH's PTC mode, Codex's newly added async tool calling, and experimental ideas like fractal tool discovery. Tool orchestration is emerging as the main battleground among LLM agent frameworks, since latency and token consumption in multi-tool workflows often matter more than raw model quality. A new open-source harness that reduces round trips between the model and tools could influence how developers build and benchmark agentic products, even if it is an incremental rather than a paradigm-shifting step. The core idea behind programmatic tool calling is that instead of returning a sequence of individual tool calls through the completion API, the model emits a program (often TypeScript) that invokes the tools itself, so it does not have to wait for each tool result before issuing the next call. Commenters noted caveats: the approach is beneficial in some cases but not others, the headline benchmark graph compares the harness running on Astra xhigh against Codex with Astra max, and there is a potential naming clash with Epic's Unreal Engine.

hackernews · trollied · Sep 22, 18:15 · [Discussion](https://news.ycombinator.com/item?id=49805748)

**Background**: An agent harness (also called agent scaffolding) is the software infrastructure surrounding a large language model — tools, memory, sandboxes, and feedback loops — that turns a raw model into a working agent. Conventional tool calling requires a round trip to the model for every tool invocation, which adds latency and inflates token usage in multi-step tasks. Programmatic tool calling, already supported by platforms such as Letta and Anthropic's Claude, instead lets the model write code that calls tools inside an execution container, filtering or processing data before it reaches the model's context. Unreal Agent enters this crowded space as an open-source alternative.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Agent_harness">Agent harness - Wikipedia</a></li>
<li><a href="https://www.databricks.com/blog/ai-harness">What is an AI Agent Harness? | Databricks Blog</a></li>
<li><a href="https://platform.claude.com/docs/en/agents-and-tools/tool-use/programmatic-tool-calling">Programmatic tool calling - Claude Platform Docs</a></li>

</ul>
</details>

**Discussion**: Skeptics on Hacker News argued the project largely restates existing programmatic tool calling, pointing to DSH's PTC mode as prior art. Others saw the space as under-explored, pitching ideas like fractal tool taxonomies that let agents drill deeper, and splay trees for tool selection; one commenter flagged benchmark unfairness (Astra xhigh vs. Codex with Astra max) and noted OpenAI's new async tool calling in Codex, while another raised serious concern that the 'Unreal' name invites a trademark fight with Epic's Unreal Engine.

**Tags**: `#AI agents`, `#LLM tool calling`, `#agent frameworks`, `#developer tools`, `#programmatic tool calling`

---

<a id="item-15"></a>
## [Xiaomi releases MiMo-V2.6 multimodal models with public RL cost and live dashboards](https://www.reddit.com/r/MachineLearning/comments/1wn36d4/xiaomi_releases_mimov26_frontier_intelligence_all/) ⭐️ 7.0/10

Xiaomi released the MiMo-V2.6 series, a natively omnimodal frontier model family, and disclosed that the total reinforcement-learning training cost was about $3.5M. The release also ships with a live 'benchmaxxing' dashboard that streams training metrics directly from the trainer's logs, alongside a benchmark-tracking page. A frontier multimodal model from a major consumer-tech company like Xiaomi signals that the top tier of AI capability is no longer limited to a handful of US labs. The unusual transparency around training cost and live benchmarks directly engages the industry's ongoing debate about benchmark gaming and reproducibility. The series includes MiMo-V2.6-Pro, described as the most capable model, and MiMo-V2.6-Flash, which balances intelligence, efficiency, and cost; Pro also offers an 'UltraSpeed' mode delivering up to 20x inference speed on Xiaomi's open platform. The models are fully open source and API pricing is unchanged, but the Reddit submission itself only provides a link and two screenshots.

reddit · r/MachineLearning · /u/we_are_mammals · Sep 22, 07:56

**Background**: A 'frontier model' is loosely defined as a model at or near the leading edge of general-purpose AI capability at a given time, typically the newest flagship from a major lab. 'Benchmaxxing' is community slang for optimizing a model specifically to score high on public benchmarks, sometimes at the expense of real-world usefulness — which is why Xiaomi publishing a live training-metric dashboard is notable, since it lets outsiders watch how the numbers are actually produced rather than only seeing final leaderboard results.

<details><summary>References</summary>
<ul>
<li><a href="https://mimo.xiaomi.com/mimo-v2-6">MiMo-V2.6 | Xiaomi</a></li>
<li><a href="https://mimo.xiaomi.com/rl/">mimo-v2.6 RL - mimo.xiaomi.com</a></li>
<li><a href="https://mimo.mi.com/docs/en-US/news/latest/v2-6">Xiaomi MiMo-V2.6 Series: 3 New Models Officially Released</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#multimodal`, `#model-release`, `#reinforcement-learning`, `#benchmarks`

---

<a id="item-16"></a>
## [Complex KDA Extends Kimi Delta Attention's Expressivity via Wider Gates](https://www.reddit.com/r/MachineLearning/comments/1wn5uv9/understanding_and_enhancing_kimi_delta_attention_r/) ⭐️ 7.0/10

A new paper titled "Complex KDA: Understanding and Enhancing the Expressivity of Kimi Delta Attention" analyzes how Kimi Delta Attention (KDA) differs in expressivity from Gated DeltaNet (GDN), showing that KDA's full diagonal gate can act as a reflection enabling a 2D rotation in a single step — but only if the gate range is extended to [-1, 1] and the delta-rule learning rate to [0, 2], a variant the authors call Complex KDA (CKDA). Experiments show CKDA can learn the S3 and S4 groups, gives promising results on audio continuation, and trains stably and competitively with standard KDA on language modeling. It clarifies a concrete, group-theoretic reason why linear attention models with bounded positive gates cannot express arbitrary rotations, which is central to the state-tracking and reasoning limits of efficient long-context architectures. If a simple range extension buys strictly more expressivity at little cost, it could inform how future KDA-style and Gated DeltaNet-style models are designed for long-sequence and multimodal workloads. Theoretically, CKDA can express any orthogonal diagonal-plus-rank-one matrix and can track the S3, S4 and A5 groups, but not S5, indicating a genuine expressivity ceiling rather than a training artifact. The gains are theoretical and empirical rather than a large-scale result: CKDA is described as competitive with, not clearly better than, standard KDA on language modeling, and the study is a technical deep-dive rather than an industry breakthrough.

reddit · r/MachineLearning · /u/Yossarian_1234 · Sep 22, 10:34

**Background**: Linear attention replaces the quadratic softmax attention with a recurrent, fixed-size state so that compute and memory scale linearly with sequence length, which is what makes ultra-long contexts practical. Gated DeltaNet (GDN) combines the delta rule — an error-correcting update that overwrites outdated memories — with input-dependent gating to improve memory retention and selectivity, and Kimi Delta Attention (KDA) further refines this with a finer-grained, per-channel diagonal gating mechanism. The symmetric groups S3, S4, S5 (permutations of 3, 4, 5 elements) and A5 are standard probes used in the literature to test whether a sequence model's hidden state can track non-commutative state, since doing so requires a state update that is not merely elementwise scaling.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2510.26692">Kimi Linear: An Expressive, Efficient Attention Architecture</a></li>
<li><a href="https://arxiv.org/abs/2412.06464">[2412.06464] Gated Delta Networks: Improving Mamba2 with Delta Rule</a></li>
<li><a href="https://en.wikipedia.org/wiki/Orthogonal_matrix">Orthogonal matrix - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Kimi Delta Attention`, `#Attention Mechanisms`, `#Deep Learning Theory`, `#Expressivity`, `#Sequence Modeling`

---

<a id="item-17"></a>
## [LLM 0.36 adds GPT-6 Sol/Luna support and non-conversational model flag](https://simonwillison.net/2026/Sep/22/llm/) ⭐️ 6.0/10

Simon Willison released version 0.36 of the LLM CLI tool, which adds two new OpenAI models — `gpt-6-sol` for GPT-6 Sol and `gpt-6-luna` for GPT-6 Luna — via issue #1702. The release also lets model plugins declare `supports_conversation = False` for models that only accept single-turn prompts, and wraps reasoning traces in `<details><summary>` tags in the Markdown output of `llm logs`, alongside bug fixes from five new contributors. LLM is one of the most widely used command-line and Python interfaces for working with large language models, so each release quickly gives its users access to the newest OpenAI offerings without waiting for separate integrations. The `supports_conversation` flag matters because it lets plugin authors correctly model single-turn endpoints such as classifiers, producing clear errors instead of silently confusing behavior. When a model declares that it does not support conversations, LLM raises `llm.ConversationNotSupported` if it receives assistant or tool history, and the `llm chat` command rejects the model before a session even starts. The first plugin to adopt this is `llm-typesafe`, which exposes TypeSafe classification/scoring models such as `typesafe/jev-latest` (aliased as `jev`) that answer yes/no questions.

rss · Simon Willison · Sep 22, 18:48

**Background**: LLM is Simon Willison's command-line tool and Python library for interacting with large language models from many providers, including OpenAI, Anthropic, Google and others, and it is extensible through plugins. GPT-6 Sol is described by OpenAI as the cost-efficient high-end model in the GPT-6 series, sitting below the flagship GPT-6 Astra and above the fast GPT-6 Luna tier; in the OpenAI API they are exposed as `gpt-6-sol` and `gpt-6-luna`. Many specialty models, such as classifiers, are not designed for multi-turn chat, which is why a plugin needs a way to advertise that limitation.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/simonw/llm">GitHub - simonw/llm: Access large language models from the ...</a></li>
<li><a href="https://openai.com/index/introducing-gpt-6-sol-and-luna/">Introducing GPT - 6 Sol and Luna | OpenAI</a></li>
<li><a href="https://pypi.org/project/llm-typesafe/">Use TypeSafe classification and scoring models with LLM</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#Simon Willison`, `#release`, `#OpenAI`, `#plugins`

---

<a id="item-18"></a>
## [llm-typesafe 0.1a0 brings TypeSafe's Jev model to the LLM CLI](https://simonwillison.net/2026/Sep/22/llm-typesafe/) ⭐️ 6.0/10

Simon Willison released llm-typesafe 0.1a0, an alpha plugin that adds support for TypeSafe AI's Jev model to his LLM command-line tool, installable with `llm install llm-typesafe` after setting a TypeSafe API key via `llm keys set typesafe`. Through the plugin, users can run probabilistic yes/no "noul" questions, which return output such as {"type": "noul", "noul": 0.99}, as well as choice questions and scoring questions using LLM's -s and -o options. This release wires TypeSafe's "System One" typed-question model into the widely used LLM CLI ecosystem, giving developers a scriptable way to get structured, machine-usable answers such as probabilities, categories and scores instead of free-form prose. It reflects a broader trend of models purpose-built to return typed outputs that downstream code can act on directly, rather than text that still needs parsing. The plugin is an early alpha (0.1a0), so its interface and options may still change. Noul questions return a single number representing the probability that the answer is yes, while choice and score answer types require a criteria argument — a JSON object mapping labels to descriptions for choices, or an ordered list of levels for scoring.

rss · Simon Willison · Sep 22, 15:54

**Background**: LLM is Simon Willison's command-line tool and Python library for prompting large language models, which can be extended with plugins that add support for new models and providers. Jev is the flagship model from TypeSafe AI, a San Francisco-based company founded in 2024, which released Jev in limited early access on 15 September 2026 alongside a US$40 million seed round led by DCVC; TypeSafe describes it as the first "System One" model, served through a POST /v1/systemone endpoint. A "noul" is Jev's yes/no question primitive, in which you write the question in the instructions, optionally define what yes and no mean in criteria, and receive the probability that the answer is yes.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Jev_(AI_model)">Jev (AI model) - Wikipedia</a></li>
<li><a href="https://docs.typesafe.ai/primitives/noul">Noul - TypeSafe AI</a></li>
<li><a href="https://llm.datasette.io/">LLM : A CLI utility and Python library for interacting with Large...</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#plugin`, `#TypeSafe`, `#AI models`, `#Simon Willison`

---

<a id="item-19"></a>
## [LinearSolveBench: New Benchmark for Model-Written Sparse Linear Solvers](https://www.reddit.com/r/MachineLearning/comments/1wnctam/linearsolvebench_new_benchmark_for_linear_solvers/) ⭐️ 6.0/10

A new benchmark called LinearSolveBench has been released (GitHub: hgarud/LinearSolveBench) that measures how well a model or evaluation harness can write fast, accurate, and general numerical solvers for large sparse linear systems in C. Its stated goal is to encourage algorithmic advances in numerical methods for solving systems of linear equations. Most LLM code benchmarks focus on general programming or competitive-coding tasks, so a benchmark targeting numerically robust, high-performance scientific kernels fills a real gap in evaluating models for scientific computing. If models can be pushed toward producing genuinely efficient sparse solvers, that has direct value for simulation, engineering, and data-analysis workloads where linear solves dominate runtime. The task is specifically constrained to C, so it tests low-level memory management and performance discipline alongside numerical correctness, and the emphasis on "general" solvers implies they must handle a range of sparse matrix types and sizes rather than overfitting to a single case. The announcement is a community post by /u/hgarud with limited engagement so far, so independent validation of the results is still pending.

reddit · r/MachineLearning · /u/hgarud · Sep 22, 15:34

**Background**: Numerical linear algebra is the subfield of numerical analysis concerned with designing matrix algorithms that give accurate approximations on finite-precision floating-point computers, and it underpins areas such as fluid dynamics, structural simulation, signal processing, and computational statistics. Large sparse linear systems — matrices where most entries are zero — typically arise from discretizing partial differential equations or from graph and network problems, and they are usually attacked with either direct factorizations like sparse LU or Cholesky, or iterative methods such as conjugate gradient and GMRES. Because these systems can be enormous and are often memory-bandwidth bound, the quality of the solver implementation strongly determines overall runtime. Benchmarks of this kind are typically run through LLM evaluation harnesses, the standardized tooling used to score models on tasks reproducibly.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Numerical_linear_algebra">Numerical linear algebra</a></li>
<li><a href="https://qaskills.sh/blog/lm-evaluation-harness-tutorial-2026">lm- evaluation - harness Tutorial: Run LLM Benchmarks... | QASkills.sh</a></li>
<li><a href="https://gitlab.mn.tu-dresden.de/teaching/sparse_linear_systems">sparse _ linear _ systems · GitLab</a></li>

</ul>
</details>

**Tags**: `#benchmarks`, `#numerical-linear-algebra`, `#sparse-solvers`, `#code-generation`, `#LLM-evaluation`

---

<a id="item-20"></a>
## [Templar simulates fault tolerance via stage skipping in pipeline-parallel training](https://www.reddit.com/r/MachineLearning/comments/1wnd5ys/simulating_fault_tolerance_with_stage_skipping_in/) ⭐️ 6.0/10

Templar published research on fault tolerance in Crucible, its distributed pre-training platform, showing that when an inner pipeline stage goes offline, activations and gradients can bypass it for multiple steps so healthy stages keep processing tokens. In simulations with a 178M-parameter model, eight replicas and four stages per replica, validation loss stayed close to the no-failure baseline at a 1% per-replica failure probability per global step, even though each simulated outage removed a stage for six global steps. If training can tolerate failed pipeline stages instead of stalling or restarting, large-scale pre-training runs could tap cheaper, unreliable hardware such as spot instances and geographically dispersed clusters, which is exactly the economics Templar is targeting with Crucible. This matters for the distributed-training community because low-bandwidth, failure-prone links have so far limited pipeline parallelism to well-connected, reliable data centers. The approach combines SparseLoCo's compressed inter-replica updates and pipeline compression across stage boundaries with stage skipping, and the authors report that fixed projections shared across layers further improve robustness, hypothesizing that shared projectors align representations across stage boundaries so bypasses are less disruptive. The authors are explicit that this is a simulation of the learning effects of stage failures, not a measurement of physical worker replacement, recovery latency, or production cost savings, and it uses a modest 178M model on a small cluster.

reddit · r/MachineLearning · /u/covenant_ai · Sep 22, 15:47

**Background**: Pipeline parallelism splits a model into consecutive stages placed on different workers, so that activations flow from one stage to the next during the forward pass and gradients flow back during the backward pass; if any stage dies, the whole pipeline normally stalls. SparseLoCo is a communication-efficient training algorithm that uses Top-k sparsification and quantization to compress updates exchanged between data-parallel replicas to extreme ratios, and Crucible is Templar's platform that layers data-parallel replicas on top of pipeline parallelism while compressing both dimensions of communication.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tplr.ai/publications/blog/skipping-stages-with-fixed-projections">Fault tolerance in low-bandwidth model parallelism: exploring ...</a></li>
<li><a href="https://deepwiki.com/one-covenant/SparseLoCo/4.2-distributed-training-setup">Distributed Training Setup | one-covenant/ SparseLoCo | DeepWiki</a></li>
<li><a href="https://www.tplr.ai/publications/blog/introducing-crucible">Introducing Crucible and An Economic Validation of Globally ...</a></li>

</ul>
</details>

**Tags**: `#distributed-training`, `#fault-tolerance`, `#pipeline-parallelism`, `#llm-pretraining`, `#systems`

---

<a id="item-21"></a>
## [AI "Sandbox Escapes" Were Sloppy Firewall Failures, Not Air Gap Breaches](https://www.reddit.com/r/MachineLearning/comments/1wm9hgn/these_were_not_rogue_ai_escapes_just_sloppy/) ⭐️ 6.0/10

A post on r/MachineLearning by u/PithyCyborg argues that widely reported AI "sandbox escapes" were not air-gap breaches at all, because none of the sandboxes involved were ever physically isolated. It points to two cases: the OpenAI/Hugging Face incident, where the sandbox reached OpenAI's internal network through a package proxy and the model simply exploited a basic flaw in that proxy, and the Google Gemini "hack", where testers left the model connected to the live internet during offensive testing and used test domain names that overlapped with real companies. The framing matters because calling these incidents "air gap escapes" inflates routine IT security failures into evidence of autonomous, boundary-breaking AI, which can distort AI safety debates and regulatory responses. The post argues the real lessons are mundane but important: proper network segmentation, restrictive egress rules, and not relying on soft software barriers when the thing behind them is a highly capable model. The post stresses one computer-science fact: a true air gap requires zero cables and network interfaces plus absolute physical isolation, so any test rig with an active network interface cannot be described as air-gapped. In the OpenAI case the model's only link to the outside was a third-party package-registry cache proxy deployed in-house that relays and caches dependency downloads, making it the single allowed egress path and therefore a critical dependency; the Gemini case involved permissive egress rules and domain-name overlap.

reddit · r/MachineLearning · /u/PithyCyborg · Sep 21, 10:55

**Background**: An air gap is a network security measure in which one or more computers are physically isolated from unsecured networks, including the internet, so no data can cross except by physical media moved by hand. A sandbox is a restricted environment in which code or a model can run without being able to affect the wider system. A package proxy is an intermediary service that sits between a sandbox and public package registries such as npm or PyPI, caching and filtering dependency downloads; it reduces direct internet exposure but becomes a critical single point of failure if it is the only allowed egress path.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Air_gap_(networking)">Air gap ( networking ) - Wikipedia</a></li>
<li><a href="https://lilting.ch/en/articles/openai-model-sandbox-escape-hugging-face-breach">OpenAI models breached Hugging Face in an eval: zero-day escape ...</a></li>
<li><a href="https://nhimg.org/glossary/package-proxy/">What Is Package Proxy? Definition & Examples - nhimg.org</a></li>

</ul>
</details>

**Tags**: `#AI Safety`, `#Sandbox Escape`, `#Air Gap`, `#Network Security`, `#Machine Learning`

---

<a id="item-22"></a>
## [Qonto releases QontoFAQ benchmark for product FAQ retrieval](https://www.reddit.com/r/MachineLearning/comments/1wn9xqk/qontofaq_a_better_information_retrieval_benchmark/) ⭐️ 6.0/10

Qonto, the French fintech company, introduced QontoFAQ, a new information retrieval benchmark together with a new relevance metric, aimed at evaluating embedding models on the task of retrieving the article that answers a product question. The company published a write-up on Medium and released the associated code on GitHub at qonto/qonto-faq-benchmark. General-purpose retrieval benchmarks such as BEIR are widely felt to be saturated, or 'benchmaxxed', by strong models, so a domain-specific benchmark anchored to a concrete business objective gives practitioners a more meaningful signal when choosing or tuning embedding models for support and FAQ search. It also adds a public, reusable evaluation resource for teams building product question-answering and customer-support retrieval systems. The contribution centers on a new relevance metric that is claimed to be more proportional to document relevance than existing measures, plus a purpose-built evaluation dataset; the scope is narrow, however, since it covers a single domain (product FAQ search for one company) and is described by the submitter as an incremental rather than a breakthrough contribution.

reddit · r/MachineLearning · /u/espadrine · Sep 22, 13:45

**Background**: An information retrieval benchmark is a standardized dataset and evaluation protocol used to compare how well search or retrieval systems return relevant documents for a query, with BEIR being a well-known heterogeneous benchmark spanning many IR tasks. Embedding models are neural models that map text into vectors so that semantically similar texts end up close together, and they are the usual engine behind semantic FAQ search. A relevance metric turns the ranked list of retrieved documents into a single score, so the choice of metric strongly shapes which model looks best.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Evaluation_measures_(information_retrieval)">Evaluation measures (information retrieval) - Wikipedia</a></li>
<li><a href="https://github.com/beir-cellar/beir">GitHub - beir-cellar/beir: A Heterogeneous Benchmark for ...</a></li>
<li><a href="https://arxiv.org/abs/2306.03411">[2306.03411] Generate-then-Retrieve: Intent-Aware FAQ ... [2306.03411] Generate-then-Retrieve: Intent-Aware FAQ ... Generate-then-Retrieve: Intent-Aware FAQ Retrieval in Product ... Generate-then-retrieve: Intent-aware FAQ retrieval in product ... Abstract Generate-then-Retrieve: Intent-Aware FAQ Retrieval ... Generate-then-Retrieve: Intent-Aware FAQ Retrieval in Product ... Generate-then-Retrieve: Intent-Aware FAQ Retrieval in Product ...</a></li>

</ul>
</details>

**Tags**: `#information-retrieval`, `#benchmark`, `#embeddings`, `#NLP`, `#machine-learning`

---