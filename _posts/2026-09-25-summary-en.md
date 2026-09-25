---
layout: default
title: "Horizon Summary: 2026-09-25 (EN)"
date: 2026-09-25
lang: en
---

> From 37 items, 8 important content pieces were selected

---

1. [F-Droid 2.0 Released: Major Overhaul of the Open-Source Android App Store](#item-1) ⭐️ 9.0/10
2. [DHH's Rails World 2026 Keynote: Developers Becoming 'Makers' in the AI Era](#item-2) ⭐️ 8.0/10
3. [UK Splits iCloud Users Into Two Encryption Tiers as Apple Pulls ADP](#item-3) ⭐️ 8.0/10
4. [Show HN: Bastardica mixes mismatched fonts by abusing OpenType ligatures](#item-4) ⭐️ 7.0/10
5. [Dynomight Asks Why the Liver Regenerates So Unusually Well](#item-5) ⭐️ 7.0/10
6. [Google ships Gemini 3.8 TTS models with 2,000+ voices and 30-second voice cloning](#item-6) ⭐️ 7.0/10
7. [arXiv Secures $17.2M Philanthropic Backing to Become Independent Nonprofit](#item-7) ⭐️ 7.0/10
8. [Whiteboard (YC W26): Open-Source Visual IDE for Human-AI Architecture](#item-8) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [F-Droid 2.0 Released: Major Overhaul of the Open-Source Android App Store](https://f-droid.org/2026/09/24/f-droid-2.0-a-new-chapter-for-android-freedom.html) ⭐️ 9.0/10

F-Droid announced version 2.0 on September 24, 2026, a major overhaul of the open-source Android app store that introduces a redesigned user interface and reworked repository management, while phasing out the long-criticized F-Droid Privileged Extension (FPE). The release sparked heavy community discussion, with 918 upvotes and 261 comments on the news thread. F-Droid is the most widely used distribution channel for free and open-source (FOSS) Android apps, so its 2.0 relaunch affects anyone who installs apps outside the Google Play ecosystem. The redesign matters even more because Google has begun rolling out stricter app-install verification rules that could shrink the space for third-party stores, making F-Droid's future viability a live question. The release focuses on a new visual design and smoother repository management, and it moves away from the FPE — a privileged helper that many users found difficult to configure, particularly on custom ROMs like LineageOS. In the discussion, users also pointed out cosmetic issues such as a text-wrapping glitch in an official screenshot, where "Syncthing-Fork" was line-broken awkwardly, and complained that the new UI offers little visual differentiation between sections or tappable elements.

hackernews · daveoc64 · Sep 24, 15:26 · [Discussion](https://news.ycombinator.com/item?id=49831968)

**Background**: F-Droid is a free and open-source app repository for Android that only distributes apps with publicly available source code, making it a community-run alternative to Google Play. Repositories (repos) are the sources from which the F-Droid client fetches app metadata and APK files, so repo management is a core part of the user experience, and the F-Droid server tools can also be used to run custom or alternative repos. The FPE existed because Android normally requires user confirmation for every app installation; the privileged extension let the F-Droid client install and update apps silently on rooted or custom-ROM devices. Meanwhile, Google has been tightening Android's ecosystem: verification for app installs on certified devices has been rolling out since March 2026, with active enforcement starting in Brazil, Indonesia, Singapore and Thailand in September 2026 and a worldwide rollout planned for 2027.

<details><summary>References</summary>
<ul>
<li><a href="https://f-droid.org/">F-Droid - Free and Open Source Android App Repository</a></li>
<li><a href="https://f-droid.org/docs/">Docs | F-Droid - Free and Open Source Android App Repository</a></li>
<li><a href="https://pixelunion.eu/blog/2026/03/google-closing-android-ecosystem/">Google Is Closing Android: And Taking Your Freedom With It | PixelUnion - Free your photos from American tech platforms</a></li>

</ul>
</details>

**Discussion**: Sentiment is mixed: users welcome the overhaul and the phase-out of the FPE, with one GrapheneOS user noting they had switched to the third-party client Droid-ify precisely because F-Droid's UI was poor and the privileged extension was painful to configure. Others are sharply critical of the new design's lack of visual hierarchy, unclear tappability and scroll affordances, and an obvious text-wrapping error in a promotional screenshot. A recurring worry is what will happen to F-Droid once Google's install verification lockdown takes effect next year.

**Tags**: `#F-Droid`, `#Android`, `#Open Source`, `#App Store`, `#UI/UX`

---

<a id="item-2"></a>
## [DHH's Rails World 2026 Keynote: Developers Becoming 'Makers' in the AI Era](https://www.youtube.com/watch?v=vDjW_dRyKXY) ⭐️ 8.0/10

David Heinemeier Hansson (DHH), the creator of Ruby on Rails, delivered the opening keynote at Rails World 2026, framing the future of software development around AI and suggesting that developers are shifting from being coders to becoming 'makers of things.' The talk also addressed the ongoing relevance of established frameworks such as Rails at a moment when AI can generate application code directly. The keynote touched a nerve in the developer community because it argues that AI will reshape what most programmers actually do day to day, not just how quickly they write code. Coming from a framework creator at a flagship community event, it signals how mainstream web-development ecosystems are repositioning themselves in response to AI tooling. Commenters noted that DHH's framing came largely from the perspective of a developer and user of Rails rather than from someone responsible for stewarding the framework itself, which some read as a worrying signal for the project. The discussion also referenced 37Signals' ongoing Rust rewrites and the role of well-designed test suites in determining how successfully AI-assisted rewrites succeed.

hackernews · an0malous · Sep 23, 15:33 · [Discussion](https://news.ycombinator.com/item?id=49817680)

**Background**: Rails World is the official annual conference for Ruby on Rails, the open-source web framework DHH extracted from his company Basecamp (37Signals) in 2004 and later popularized through conventions like 'convention over configuration.' Rails is widely used for CRUD-style web applications — database-backed apps that create, read, update and delete records — and remains known for letting small teams ship products quickly. DHH is also known for outspoken, opinionated commentary on software and industry trends, so his keynotes often become reference points for broader debates.

**Discussion**: Hacker News commenters largely agreed that AI will force real changes on developers, though many disputed DHH's framing: one front-row attendee reported a 'far from doom and gloom' atmosphere where most engineers remain 'menders' maintaining systems customers pay for, while others asked why anyone would use the apps developers 'make' instead of going straight to AI. Several defended Rails' continued value for CRUD work, noting its strong conventions make it especially well suited to AI-generated code, and one commenter tied the success of Rust rewrites to the quality of existing test suites.

**Tags**: `#Rails`, `#Ruby on Rails`, `#AI`, `#Keynote`, `#Software Development`

---

<a id="item-3"></a>
## [UK Splits iCloud Users Into Two Encryption Tiers as Apple Pulls ADP](https://macanorak.com/two-tier-encryption-in-the-uk/) ⭐️ 8.0/10

Following a secret legal order from the UK government, Apple withdrew Advanced Data Protection (ADP) for iCloud users in the United Kingdom, so UK accounts can no longer enable the optional end-to-end encryption that covers iCloud Backups, Photos, Notes and iCloud Drive. The macanorak analysis frames the result as a "two-tier" regime in which two otherwise identical Apple devices receive different levels of protection depending on which side of the UK border their owner sits. The case sets a precedent that a single government can force a global platform to roll back an end-to-end encryption feature for an entire country without ever publicly acknowledging the order, which invites other governments to demand the same. It also erodes the trust argument Apple has used since 2015 — that it cannot hand over data it cannot decrypt — because for many UK accounts Apple now holds the keys again. Roughly 14 iCloud categories, including iCloud Keychain and Health data, remain end-to-end encrypted by default in the UK, while ADP would have raised that total to about 23 categories. The categories that revert to Standard Data Protection — iCloud Backup, Photos, Notes, iCloud Drive and others — are ones where Apple holds the keys and can therefore respond to lawful legal process, and commenters note that UK users' encryption secrets can still be exposed in ordinary usage patterns even for the nominally unaffected categories.

hackernews · ReturnoftheHack · Sep 24, 10:39 · [Discussion](https://news.ycombinator.com/item?id=49828731)

**Background**: iCloud data is encrypted in transit and at rest, but by default Apple holds the decryption keys for most categories, meaning it can technically access that data and hand it over when legally compelled. Advanced Data Protection, announced by Apple on December 7, 2022, is an opt-in setting that moves almost all iCloud categories to end-to-end encryption so that only the user's devices hold the keys. The UK order came in the form of a Technical Capability Notice under the Investigatory Powers Act 2016, a mechanism that can require a company to build or maintain interception capability and which, in this case, would have required changing the architecture ADP depended on. Rather than build such a capability or abandon encryption in the UK entirely, Apple removed the feature for UK users.

<details><summary>References</summary>
<ul>
<li><a href="https://macanorak.com/two-tier-encryption-in-the-uk/">Two-Tier Encryption in the UK - macanorak.com</a></li>
<li><a href="https://mjtsai.com/blog/2026/09/22/two-tier-encryption-in-the-uk/">Michael Tsai - Blog - Two-Tier Encryption in the UK</a></li>
<li><a href="https://www.gov.uk/government/publications/notices-regime-code-of-practice/notices-regime-code-of-practice-accessible">Notices regime code of practice (accessible) - GOV.UK</a></li>

</ul>
</details>

**Discussion**: Commenters broadly read "two-tier encryption" as a euphemism for a backdoor with extra steps, and several doubt that a less secure tier can be confined to "someone else." Others push back on technical framing, pointing out that the 14 default categories are not fully untouched and that UK users' encryption secrets can still leak in common usage, while a recurring theme is that Apple in 2015 had the appetite to fight the FBI and today appears less willing to resist, with some arguing Apple should exit the UK market or cut off UK government customers altogether.

**Tags**: `#encryption`, `#privacy`, `#Apple`, `#UK-policy`, `#end-to-end-encryption`

---

<a id="item-4"></a>
## [Show HN: Bastardica mixes mismatched fonts by abusing OpenType ligatures](https://bastardica.mitpit.com/) ⭐️ 7.0/10

Bastardica is a new client-side web tool (bastardica.mitpit.com) that deliberately abuses OpenType ligature substitution to swap glyphs from one font into another, producing intentionally "cursed" typographic mashups like Times New Bastard. It runs Python loaded into WebAssembly entirely in the browser, which lets it process and generate the modified font quickly without any server round-trip. The project earned strong community validation on Hacker News (469 points, 64 comments), showing that even a joke tool can be a compelling demo of running Python client-side via WebAssembly. It also highlights how OpenType's substitution features — normally used for tasteful typography — can be repurposed as a creative-coding medium, and it gave designers a hands-on toy for typography in-jokes. Technically, the trick relies on OpenType ligature features (the liga and related substitution lookups) to map ordinary character sequences to glyphs drawn from a different font, so the output font is a normal OpenType file that renders the mashup anywhere it is installed. Because Python is compiled to WASM, all font manipulation happens locally in the browser, which avoids uploading fonts to a server and cuts latency; the tradeoff is the WASM payload size and browser memory overhead.

hackernews · MitPitt · Sep 23, 22:53 · [Discussion](https://news.ycombinator.com/item?id=49823738)

**Background**: OpenType is the modern cross-platform font format developed by Microsoft and Adobe, and it supports advanced layout tables that go far beyond simple glyph outlines. Ligatures are one such feature: lookups that replace two or more characters with a single combined glyph, most familiarly 'fi', 'fl' and 'ffl'. WebAssembly (Wasm) is a portable binary instruction format that lets languages like C, C++, Rust and now Python run at near-native speed in the browser; projects such as Pyodide and py2wasm make it practical to run Python this way.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Fonts/OpenType_fonts">OpenType font features - CSS | MDN - MDN Web Docs Usage example</a></li>
<li><a href="https://github.com/pyodide/pyodide">GitHub - pyodide/pyodide: Pyodide is a Python distribution ... Waspy - Python to WebAssembly Compiler Running Python in the Browser with WebAssembly GitHub - wasmerio/wasmer-python: WebAssembly runtime for ... Python to WebAssembly: Unleashing New Possibilities in Web ... Python WebAssembly: Unleashing Python's Power on the Web</a></li>
<li><a href="https://wasmer.io/posts/py2wasm-a-python-to-wasm-compiler">Announcing py2wasm: A Python to Wasm compiler - Blog · Wasmer</a></li>

</ul>
</details>

**Discussion**: Commenters enthusiastically traded font-prank ideas: one designer described carefully tuning vertical scale and offset so Papyrus and Comic Sans optically align, while another suggested mixing Helvetica and Arial every second or third character to induce a designer's nervous breakdown. Others pointed to a self-censoring font (Paranoia Sans) and proposed ligatures that render a word as a different word, e.g. making "red" display as "green", plus a joke about an Arial variant with intentionally bad kerning.

**Tags**: `#typography`, `#OpenType`, `#WebAssembly`, `#creative-coding`, `#Show HN`

---

<a id="item-5"></a>
## [Dynomight Asks Why the Liver Regenerates So Unusually Well](https://dynomight.substack.com/p/liver) ⭐️ 7.0/10

The science blog Dynomight published an essay asking why the liver regenerates so much more effectively than other human organs, arguing the answer lies in evolutionary pressure and the body's wound-healing priorities rather than any unique biological magic. The post drew a large Hacker News discussion (roughly 237 points and 151 comments), where commenters challenged several of the author's evolutionary claims and added firsthand transplant experiences. Understanding why the liver regenerates and other organs largely do not has direct clinical stakes: it underpins split-liver transplantation, where one donor liver is divided and each half regrows in a different recipient, and it shapes how researchers think about regenerative medicine for the heart, kidney and other organs. The piece also illustrates a broader pattern in science communication, where a well-argued blog post can surface expert counterexamples and lived patient experience that formal papers rarely capture. The essay frames the liver as an outlier that regrows mainly through proliferation of existing hepatocytes rather than relying on a dedicated stem-cell pool, and it weighs trade-offs such as scarring versus perfect repair. Commenters pushed back with counterexamples: no known adult salamander can regenerate an entirely removed eye, a chopped salamander simply dies rather than regenerating like a planarian worm, and axolotls can regrow limbs but not every structure.

hackernews · jbotz · Sep 24, 16:23 · [Discussion](https://news.ycombinator.com/item?id=49832938)

**Background**: Dynomight is a widely read pseudonymous science and statistics blog known for long, careful, often humorous deep-dives. Liver regeneration is a well-documented phenomenon: after surgical removal of up to roughly two-thirds of the organ, the remaining tissue expands within weeks, which is why living-donor and split-liver transplants are possible. By contrast, most human organs — the heart, kidneys, and central nervous system — heal largely by forming scar tissue, a process biologists generally explain as a trade-off between fast, robust wound closure and full tissue reconstruction. The evolutionary-pressure framing used in the post treats regeneration as a trait that only evolves when the survival benefit outweighs its metabolic and cancer-related costs.

<details><summary>References</summary>
<ul>
<li><a href="https://dynomight.substack.com/archive">Archive - DYNOMIGHT INTERNET NEWSLETTER</a></li>
<li><a href="https://en.wikipedia.org/wiki/Wound_healing">Wound healing - Wikipedia</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC12717721/">Liver regeneration : unraveling the molecular mechanisms and...</a></li>

</ul>
</details>

**Discussion**: Commenters largely agreed the post was unusually well written, with one thanking the author for an article that 'felt written by a human being,' but several disputed its evolutionary reasoning: one argued most of the body fails to regenerate simply for lack of selective pressure and noted that salamander regeneration has real limits, while another strongly rejected the idea that humans are 'overtuned' for skin and blood repair, pointing out that impaired wound healing causes major post-surgical complications and mortality. A transplant recipient shared a firsthand account of receiving half of a donor liver, noting the organ regrew within months and that the other lobe went to a child recipient.

**Tags**: `#biology`, `#regeneration`, `#evolution`, `#medicine`, `#science-communication`

---

<a id="item-6"></a>
## [Google ships Gemini 3.8 TTS models with 2,000+ voices and 30-second voice cloning](https://simonwillison.net/2026/Sep/23/gemini-tts-playground/) ⭐️ 7.0/10

Google released two new Gemini text-to-speech models, gemini-3.8-flash-tts and gemini-3.8-flash-lite-tts, offering a library of over 2,000 voices plus custom voice creation from just a 30-second audio sample of a voice the user has rights to use. Simon Willison simultaneously published a bring-your-own-key browser playground for the models, which he vibe coded with GPT-6 Astra and which loads 2,089 voices in its catalog. Built-in voice cloning from a short sample, combined with a large curated voice library and multi-speaker dialogue support, lowers the barrier for developers building audiobooks, podcasts, game dialogue and accessibility tools directly on top of a major cloud API. It also pushes production-grade synthetic speech further into commodity territory, intensifying competition with dedicated TTS vendors and raising familiar concerns about consent and misuse of cloned voices. A notable API capability is that it makes it easy to define a full conversation between multiple characters, each with its own voice and delivery-style instructions. In Willison's test, generating 1 minute 18 seconds of audio with gemini-3.8-flash-tts took about 20 seconds and cost 2.74 cents, and the playground works only because the underlying Gemini API has an open CORS policy; the API key stays in the page's memory and is never written to browser storage.

rss · Simon Willison · Sep 23, 17:12

**Background**: Text-to-speech (TTS) systems convert written text into spoken audio, and modern neural TTS models add controls over voice identity, emotion and speaking style. Voice cloning is an AI technique that replicates a specific person's voice so it can speak words they never actually said; while useful for audiobooks and for people who have lost their voices, it is also a form of audio deepfake used in scams and misinformation. CORS (Cross-Origin Resource Sharing) is the web mechanism that lets a page on one domain call an API on another domain, which is why a third-party browser playground can talk to Google's Gemini endpoints directly without a proxy server.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Voice_cloning">Voice cloning</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Guides/CORS">Cross-Origin Resource Sharing (CORS) - HTTP | MDN</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-6_Astra">GPT-6 Astra</a></li>

</ul>
</details>

**Tags**: `#text-to-speech`, `#Gemini`, `#voice-cloning`, `#AI models`, `#developer tools`

---

<a id="item-7"></a>
## [arXiv Secures $17.2M Philanthropic Backing to Become Independent Nonprofit](https://www.reddit.com/r/MachineLearning/comments/1wox8kt/arxiv_receives_multiyear_philanthropic/) ⭐️ 7.0/10

arXiv announced multiyear philanthropic commitments totaling $17.2 million from Simons Foundation International, XTX Markets, and Siegel Family Endowment, spanning three to five years. The funding is intended to support arXiv's launch as an independent nonprofit organization, moving it out from under Cornell University's administrative umbrella. arXiv is the de facto preprint server for physics, mathematics, and computer science, and a large share of modern AI and machine learning research appears there before peer review, so its financial stability directly affects how quickly the global research community can access new work. Securing multiyear funding and independent nonprofit status reduces the risk that a single university's budget pressures could disrupt a critical piece of open-access scientific infrastructure. The commitment totals $17.2 million over three to five years and comes from three funders — Simons Foundation International, the algorithmic trading firm XTX Markets, and Siegel Family Endowment. The announcement was made on the official arXiv blog and framed as supporting arXiv's transition to independent nonprofit governance rather than funding a specific new technical feature.

reddit · r/MachineLearning · /u/Nunki08 · Sep 24, 09:43

**Background**: arXiv is a free, open-access preprint server launched in 1991 at Los Alamos National Laboratory and later hosted at Cornell University; it lets researchers post papers publicly before formal peer review and journal publication. It has become the default venue for physics, mathematics, and computer science preprints, and in recent years it has grown especially fast in AI and machine learning. Running such a service at scale requires sustained funding for servers, moderation, and staff, which is why multiyear philanthropic commitments matter more than one-off donations. XTX Markets, one of the donors, is a London-based algorithmic trading firm founded in 2015 that uses machine learning for price forecasting across financial markets.

<details><summary>References</summary>
<ul>
<li><a href="https://www.itsoc.org/publications/arxiv/arxiv-faq">ArXiV FAQ | IEEE Information Theory Society</a></li>
<li><a href="https://www.xtxmarkets.com/">Home | XTX Markets</a></li>
<li><a href="https://otio.ai/blog/what-is-arxiv-preprint">What Is Arxiv Preprint + How to Submit There — Otio Blog</a></li>

</ul>
</details>

**Tags**: `#arXiv`, `#open access`, `#research infrastructure`, `#philanthropy`, `#academic publishing`

---

<a id="item-8"></a>
## [Whiteboard (YC W26): Open-Source Visual IDE for Human-AI Architecture](https://github.com/devdotfast/whiteboard) ⭐️ 6.0/10

A team of four developers (Sid, Alex, Ketan, and Milan) launched Whiteboard, an MIT-licensed open-source desktop app where humans and AI coding agents architect software together on a shared visual canvas. The app plugs into existing agents like Claude Code and Codex via an agent SDK that lets them draw diagrams and narrate their work on an in-app canvas. The launch drew 188 points and 79 comments on Hacker News, with commenters predicting that streaming, agent-drawn diagrams will become a standard way of working within a year. It targets a real pain point in agentic coding: teams shipping lots of AI-generated PRs faster than they can understand them, accumulating what the founders call "cognitive debt." Whiteboard is built on top of CodeOSS (the open-source core of VS Code), so it inherits LSP support and VSCode keybindings, and it includes a Rust-written AST-aware semantic diff viewer that summarizes large added functions as pseudocode and hides test or doc changes, extendable via a WASM plugin system. Notable limitations: the app currently cannot edit files, prompting debate over whether the "IDE" label is accurate, and it is macOS-only for now, though everything will remain self-hostable.

hackernews · sidharthkmenon · Sep 24, 17:21 · [Discussion](https://news.ycombinator.com/item?id=49833867)

**Background**: CodeOSS is the open-source repository that Microsoft's Visual Studio Code is built from, giving third-party apps a ready-made editor foundation with language-server (LSP) support. Claude Code is Anthropic's agentic coding tool that reads a codebase, edits files, and runs commands, while Codex is OpenAI's AI coding agent, released as a CLI in April 2025. Whiteboard lets these agents, which normally work only in text, express their plans visually by drawing to a shared canvas.

<details><summary>References</summary>
<ul>
<li><a href="https://en.linuxadictos.com/code-oss-vscodium-or-visual-studio-code-what-should-i-install-on-linux.html">Code OSS , VSCodium or Visual Studio Code: what should you install...</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_Codex_(AI_agent)">OpenAI Codex (AI agent) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Sentiment was largely positive and constructive: commenter bbor praised the "fake pen drawing animations + streaming diagrams" pattern as something that will be everywhere in 12 months, initially complained about the macOS-only limitation, then publicly corrected themselves. Others noted the inability to edit files challenges the "IDE" label, requested GitHub PR linking/commenting, and commenter 2001zhaozhao argued it is a better, more visual alternative to coding agents' current "Plan Mode" for high-level architecture work.

**Tags**: `#AI agents`, `#developer tools`, `#open source`, `#software architecture`, `#Show HN`

---