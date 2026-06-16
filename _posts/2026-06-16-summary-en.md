---
layout: default
title: "Horizon Summary: 2026-06-16 (EN)"
date: 2026-06-16
lang: en
---

> From 39 items, 23 important content pieces were selected

---

1. [Neocortical Learning Framework Challenges Backpropagation](#item-1) ⭐️ 9.0/10
2. [Backdoor in LinkedIn job offer via malicious npm package](#item-2) ⭐️ 8.0/10
3. [Banned Book Library Stored in a Smart Light Bulb](#item-3) ⭐️ 8.0/10
4. [Iroh 1.0: Application-Layer P2P Networking Library Launches](#item-4) ⭐️ 8.0/10
5. [Users share success replacing Claude/GPT with local models for coding](#item-5) ⭐️ 8.0/10
6. [Hetzner Announces Major Price Increases Due to AI-Driven Hardware Costs](#item-6) ⭐️ 8.0/10
7. [Fox plans to acquire Roku](#item-7) ⭐️ 8.0/10
8. [TimescaleDB Hypercore Compression Up to 98%](#item-8) ⭐️ 8.0/10
9. [Salesforce Acquires Fin (formerly Intercom) for $3.6B](#item-9) ⭐️ 8.0/10
10. [Why AI hasn't replaced software engineers, and won't](#item-10) ⭐️ 8.0/10
11. [Homelab AI Dev Platform with Forgejo and Opencode](#item-11) ⭐️ 7.0/10
12. [US battery manufacturing output continues to break records](#item-12) ⭐️ 7.0/10
13. [Deep Dive into Commander Keen's Adaptive Tile Refresh](#item-13) ⭐️ 7.0/10
14. [Copper drug restores memory in Alzheimer's mice](#item-14) ⭐️ 7.0/10
15. [Cloudflare CAPTCHA Only on Search URLs with Ampersand](#item-15) ⭐️ 7.0/10
16. [Personality clashes led US govt to shut down Anthropic's models](#item-16) ⭐️ 7.0/10
17. [Open weights insufficient; open training frameworks like FeynRL needed](#item-17) ⭐️ 7.0/10
18. [Cleo: A 2B Model for Text-to-SQL with Unified Harness](#item-18) ⭐️ 7.0/10
19. [PrintGuard 2.0: Few-shot failure detector goes TFLite, runs in browser](#item-19) ⭐️ 7.0/10
20. [Developer's Nostalgic Ode to Computing](#item-20) ⭐️ 6.0/10
21. [LLMs Show Consistent Name Preferences Across Generated Sites](#item-21) ⭐️ 6.0/10
22. [Quant Firms Rush to Diamond Sponsor ICML 2026](#item-22) ⭐️ 6.0/10
23. [Biggest time sinks in embedded ML for sensor data](#item-23) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Neocortical Learning Framework Challenges Backpropagation](https://www.reddit.com/r/MachineLearning/comments/1u6x8al/how_the_brains_learn_r/) ⭐️ 9.0/10

A new framework for neocortical learning using error-driven predictive learning via temporal derivatives has been proposed, implemented in a spiking neural simulation called Axon, and claims to outperform backpropagation on challenging cognitive tasks. If validated, this could represent a paradigm shift in both AI and neuroscience by providing a biologically plausible learning algorithm that rivals the performance of backpropagation while being implementable in neural hardware. The framework claims to meet all three criteria (computational, algorithmic, implementational) and uses competitive kinase synaptic plasticity induction mechanisms. It was demonstrated on a range of cognitively motivated tasks, though the specific tasks and performance metrics are not detailed in the summary.

reddit · r/MachineLearning · /u/Terminator857 · Jun 15, 23:39

**Background**: The neocortex is the part of the brain responsible for higher-order functions like perception, language, and reasoning. Learning in the neocortex is believed to involve synaptic plasticity, where connections between neurons are strengthened or weakened based on activity. Error-driven predictive learning via temporal derivatives is an algorithm that adjusts predictions based on differences between expected and actual outcomes over time, similar to temporal difference learning in reinforcement learning. The Axon simulation framework is a spiking neural network simulator that models biological neurons more realistically than traditional artificial neural networks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Temporal_difference_learning">Temporal difference learning - Wikipedia</a></li>
<li><a href="https://elifesciences.org/articles/37836">Competition for synaptic building blocks shapes synaptic plasticity | eLife</a></li>

</ul>
</details>

**Tags**: `#neuroscience`, `#machine learning`, `#learning algorithms`, `#neocortex`, `#predictive learning`

---

<a id="item-2"></a>
## [Backdoor in LinkedIn job offer via malicious npm package](https://roman.pt/posts/linkedin-backdoor/) ⭐️ 8.0/10

A LinkedIn recruiter sent a job applicant a malicious GitHub repository where running npm install executed a backdoor through a postinstall script, disguised as a deprecated module issue. This attack highlights a sophisticated supply chain attack vector combining social engineering with npm lifecycle scripts, posing a serious threat to developers and organizations that rely on open-source dependencies. The backdoor was hidden in commented-out tests and executed via the npm prepare script, which runs automatically after npm install. The attacker targeted a crypto startup developer, and the payload communicated with a remote server.

hackernews · lwhsiao · Jun 15, 20:00 · [Discussion](https://news.ycombinator.com/item?id=48546294)

**Background**: npm lifecycle scripts like postinstall run automatically when a package is installed, making them a common attack vector for supply chain attacks. Similar attacks, including the widespread Shai-Hulud worm, have compromised thousands of npm packages by injecting malware via compromised maintainer accounts.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cisa.gov/news-events/alerts/2025/09/23/widespread-supply-chain-compromise-impacting-npm-ecosystem">Widespread Supply Chain Compromise Impacting npm Ecosystem</a></li>
<li><a href="https://medium.com/data-and-beyond/the-npm-install-that-handed-hackers-your-entire-system-in-1-1-seconds-39d6f713196d">The npm Install That Handed Hackers Your Entire System in... | Medium</a></li>

</ul>
</details>

**Discussion**: Commenters noted this is a criminal act and questioned the lack of a centralized reporting mechanism for cybercrime. One user shared a similar experience via email, possibly linked to North Korean threat actors.

**Tags**: `#security`, `#supply-chain-attack`, `#social-engineering`, `#npm`, `#linkedin`

---

<a id="item-3"></a>
## [Banned Book Library Stored in a Smart Light Bulb](https://www.richardosgood.com/posts/banned-book-library/) ⭐️ 8.0/10

A hacker has successfully stored a library of banned books inside a Wi-Fi smart light bulb, creating a portable and discreet repository for censored texts. The project uses an ESP8266-based smart bulb to host the files, which can be accessed over Wi-Fi without a traditional server. This project combines hardware hacking with free speech advocacy, offering a novel way to circumvent censorship by hiding information in everyday objects. It highlights both the potential for IoT devices as tools for activism and the ongoing debate about access to banned books. The smart bulb runs custom firmware that serves the book files via a Wi-Fi access point, with the entire library fitting within the bulb's limited storage. The project is open source and encourages further development, such as mesh networking for distributed access.

hackernews · sohkamyung · Jun 15, 22:37 · [Discussion](https://news.ycombinator.com/item?id=48547985)

**Background**: Smart light bulbs often contain microcontrollers like the ESP8266, which can run custom firmware and store data in flash memory. Security researchers have demonstrated that these bulbs can be hacked to install malicious firmware, but this project repurposes that capability for storing censored content. The ESP8266 is a low-cost Wi-Fi chip commonly used in IoT devices, capable of both serving web pages and storing files.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.checkpoint.com/security/the-dark-side-of-smart-lighting-check-point-research-shows-how-business-and-home-networks-can-be-hacked-from-a-lightbulb/">The Dark Side of Smart Lighting: Check Point Research Shows How Business and Home Networks Can Be Hacked from a Lightbulb - Check Point Blog</a></li>
<li><a href="https://randomnerdtutorials.com/visualize-esp32-esp8266-sensor-readings-from-anywhere/">Visualize ESP32/ ESP 8266 Sensor Readings... | Random Nerd Tutorials</a></li>

</ul>
</details>

**Discussion**: The community largely praised the project for its creativity and relevance to free speech, with some drawing parallels to earlier projects like PirateBox and LibraryBox. Commenters also discussed the potential for mesh networking to enhance resilience, while a few raised concerns about the specific selection of 'banned books' and the effectiveness of such tactics.

**Tags**: `#hardware hacking`, `#free speech`, `#smart light bulb`, `#banned books`, `#activism`

---

<a id="item-4"></a>
## [Iroh 1.0: Application-Layer P2P Networking Library Launches](https://www.iroh.computer/blog/v1) ⭐️ 8.0/10

The open-source project Iroh has released version 1.0, offering a library that simplifies establishing direct peer-to-peer connections at the application layer, similar to how Tailscale operates at the network layer. This release makes it significantly easier for app developers to embed peer-to-peer connectivity without requiring users to manage separate VPN accounts. It reduces the complexity of building distributed applications and could accelerate the adoption of decentralized networking. Iroh 1.0 natively supports IPv4, IPv6, and relay transports, and now also allows developers to implement custom transports for protocols like WebRTC or BLE. It uses cryptographic asymmetric keys, called 'dial keys', for peer identity and secure connectivity.

hackernews · chadfowler · Jun 15, 15:13 · [Discussion](https://news.ycombinator.com/item?id=48542480)

**Background**: Iroh is a networking library that establishes direct connections between two peers anywhere on the internet, automatically handling NAT traversal and transport selection. Often compared to Tailscale, Iroh operates at the application layer (layer 7) instead of the network layer (layer 3), making it embeddable directly into applications without needing a separate VPN. This approach lets app developers add peer-to-peer features without requiring users to create accounts or configure network settings.

<details><summary>References</summary>
<ul>
<li><a href="https://www.iroh.computer/">iroh</a></li>
<li><a href="https://www.iroh.computer/blog/comparing-iroh-and-libp2p">Comparing Iroh & Libp2p: Simplifying P2P Connectivity - Iroh</a></li>

</ul>
</details>

**Discussion**: Community members showed strong interest, with discussions focusing on custom transport support and comparisons to existing solutions. Developers clarified that Iroh now supports custom transports and uses cryptographic keys for identity. Some questioned the necessity of Iroh given IP and DNS, while others praised its potential for decentralized apps. A notable concern was insufficient documentation about the key mechanics and relay involvement.

**Tags**: `#networking`, `#p2p`, `#peer-to-peer`, `#tailscale`, `#iroh`

---

<a id="item-5"></a>
## [Users share success replacing Claude/GPT with local models for coding](https://news.ycombinator.com/item?id=48542100) ⭐️ 8.0/10

A Hacker News discussion reveals that many developers have successfully replaced cloud-based coding assistants like Claude and GPT with local models such as Qwen 3.6 and Gemma 4, achieving adequate performance for daily coding tasks while gaining privacy and cost benefits. This demonstrates that open-source local models have matured enough to serve as viable alternatives to frontier cloud models for many practical coding use cases, potentially reducing reliance on expensive subscriptions and improving data privacy. Users reported using setups like llama.cpp with Qwen3.6-35B running on a single RTX 3090 achieving over 150 tok/s, and Mac Studio with 128GB RAM running Qwen3.6 35b (with 3B active parameters). However, local models are noted to be less smart than frontier models like Claude Code or GPT Codex.

hackernews · cloudking · Jun 15, 14:46

**Background**: Large language models (LLMs) like Claude and GPT are typically accessed via cloud APIs. Local models are downloaded and run on the user's own hardware, offering privacy and offline capability but requiring sufficient computational resources. Qwen is a family of open-source LLMs from Alibaba Cloud, and Gemma is from Google DeepMind. Tokens per second (tok/s) measures how fast a model generates text.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>
<li><a href="https://ai.google.dev/gemma/docs">Gemma models overview | Google AI for Developers</a></li>
<li><a href="https://benchlm.ai/llm-speed">LLM Speed & Latency Comparison — Tokens/sec & Response Latency (2026)</a></li>

</ul>
</details>

**Discussion**: The discussion is overwhelmingly positive, with many users sharing detailed setups and performance numbers. Some note that while local models are not yet on par with the best cloud models, they are sufficient for most daily coding needs and offer significant privacy and cost advantages. A few commenters express skepticism about fully replacing cloud models, citing the opportunity cost of not using the latest models.

**Tags**: `#local-llm`, `#coding-assistant`, `#qwen`, `#gemma`, `#hpc`

---

<a id="item-6"></a>
## [Hetzner Announces Major Price Increases Due to AI-Driven Hardware Costs](https://docs.hetzner.com/general/infrastructure-and-availability/price-adjustment/#cloud-servers) ⭐️ 8.0/10

Hetzner has announced significant price increases for its server products, with some prices tripling, citing rising hardware costs driven by AI demand. This price adjustment reflects a broader industry trend where AI boom is straining hardware supply chains, impacting cloud hosting economics and potentially forcing customers to reconsider their providers. Specific price changes include up to 3x increases on some server models, and the adjustment applies across Hetzner's server product line including cloud servers.

hackernews · tuhtah · Jun 15, 13:19 · [Discussion](https://news.ycombinator.com/item?id=48540844)

**Background**: Hetzner is a German cloud hosting provider known for competitive pricing. Recent AI advancements have increased demand for GPUs and data center hardware, leading to shortages and higher costs across the industry.

**Discussion**: Community members expressed shock at the magnitude of increases, with one calling a 3x jump 'wild'. Some noted this was inevitable given Hetzner's previous low pricing relative to competitors, while others criticized AI boom for driving up costs without clear benefits.

**Tags**: `#cloud hosting`, `#pricing`, `#AI boom`, `#hardware scarcity`, `#Hetzner`

---

<a id="item-7"></a>
## [Fox plans to acquire Roku](https://www.wsj.com/business/deals/fox-roku-deal-f6e564f9) ⭐️ 8.0/10

Fox announced its intention to acquire Roku, a major streaming hardware platform, sparking concerns over content control and antitrust issues. This acquisition would give Fox direct access to 30-50% of US households' TV hardware, potentially compromising platform neutrality and market competition. Roku has historically been a service-agnostic platform but increasingly integrated ads and content, raising concerns about conflicts of interest if owned by a content provider like Fox.

hackernews · thm · Jun 15, 12:50 · [Discussion](https://news.ycombinator.com/item?id=48540499)

**Background**: Roku is a popular streaming device manufacturer and platform. Fox is a major media company with news and entertainment content. The deal could reshape the streaming landscape by combining hardware and content ownership.

**Discussion**: Commenters express strong pessimism, fearing loss of neutrality and increased control by Fox, with some already switching to alternatives like Nvidia Shield. There is concern that Fox should not be allowed to buy access to such a large user base.

**Tags**: `#acquisition`, `#Roku`, `#Fox`, `#streaming`, `#antitrust`

---

<a id="item-8"></a>
## [TimescaleDB Hypercore Compression Up to 98%](https://roszigit.com/en/blog/timescaledb-compression-hypercore) ⭐️ 8.0/10

A new article details how TimescaleDB's hypercore compression achieves up to 98% storage reduction for time-series data in PostgreSQL using columnar storage and advanced encoding techniques. This compression capability makes PostgreSQL significantly more efficient for storing massive time-series datasets, potentially reducing storage costs and improving I/O performance for IoT, monitoring, and analytics workloads. Hypercore is a hybrid row-columnar storage engine that uses segment-by and order-by configuration to optimize compression. It employs techniques like delta-of-delta encoding (inspired by Facebook's Gorilla) and dictionary encoding, with trade-offs in query performance for highly selective queries.

hackernews · lkanwoqwp · Jun 15, 17:29 · [Discussion](https://news.ycombinator.com/item?id=48544451)

**Background**: TimescaleDB is a PostgreSQL extension designed for time-series data. Traditional row-oriented databases store each row contiguously, which is inefficient for time-series because repeated timestamps and similar values across many rows compress poorly. Columnar storage groups values from the same column, enabling higher compression ratios through contiguous similar data.

<details><summary>References</summary>
<ul>
<li><a href="https://roszigit.com/en/blog/timescaledb-compression-hypercore">TimescaleDB Compression: Hypercore and Columnar Storage with up to 98% Ratio in PostgreSQL</a></li>
<li><a href="https://docs.tigerdata.com/use-timescale/latest/hypercore/">Tiger Data Documentation | Hypercore</a></li>
<li><a href="https://www.tigerdata.com/blog/building-columnar-compression-in-a-row-oriented-database">Columnar Compression for Large Databases | Tiger Data</a></li>

</ul>
</details>

**Discussion**: Community comments highlight performance trade-offs: users note that compression can slow down queries, especially with high selectivity, and compare TimescaleDB's approach to alternatives like deltaX and swinging-door compression. One commenter expresses skepticism about the 'up to 98%' claim, calling it 'dross' unless benchmarks are provided.

**Tags**: `#TimescaleDB`, `#PostgreSQL`, `#time-series`, `#compression`, `#database`

---

<a id="item-9"></a>
## [Salesforce Acquires Fin (formerly Intercom) for $3.6B](https://www.salesforce.com/news/press-releases/2026/06/15/salesforce-signs-definitive-agreement-to-acquire-fin/?bc=HL) ⭐️ 8.0/10

Salesforce has signed a definitive agreement to acquire Fin, the AI customer agent platform formerly known as Intercom, for approximately $3.6 billion. The acquisition aims to enhance Salesforce's Agentforce platform with Fin's autonomous agent technology. This acquisition intensifies competition in the AI customer service agent market, particularly against Sierra, co-founded by Salesforce's former co-CEO Bret Taylor. It also signals Salesforce's strategic move to prevent independent AI support platforms from becoming a control point outside its CRM ecosystem. Fin was rebranded from Intercom just a month ago, and the acquisition price is $3.6 billion. Salesforce plans to integrate Fin's technology into its existing Agentforce platform for building custom AI agents.

hackernews · colesantiago · Jun 15, 12:08 · [Discussion](https://news.ycombinator.com/item?id=48540126)

**Background**: Salesforce is the global leader in CRM (Customer Relationship Management). Fin (formerly Intercom) is an AI-powered customer agent platform that integrates with various business systems. The acquisition reflects the growing trend of large enterprises acquiring AI startups to bolster their AI capabilities, especially in customer service automation.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/06/15/salesforce-acquires-ai-customer-service-platform-fin-for-3-6b/">Salesforce acquires AI customer service platform Fin for $3 ...</a></li>
<li><a href="https://www.salesforce.com/news/press-releases/2026/06/15/salesforce-signs-definitive-agreement-to-acquire-fin/">Salesforce Signs Definitive Agreement to Acquire Fin</a></li>

</ul>
</details>

**Discussion**: Community comments show mixed reactions: some praise AI customer service when done right (e.g., Starlink), while others question the long-term viability of helpdesk companies like Intercom as businesses train their own AI agents. There is also speculation that the acquisition is a direct move to compete with Sierra, founded by Salesforce's ex-co-CEO Bret Taylor.

**Tags**: `#acquisition`, `#AI`, `#customer-service`, `#Salesforce`, `#CRM`

---

<a id="item-10"></a>
## [Why AI hasn't replaced software engineers, and won't](https://simonwillison.net/2026/Jun/14/why-ai-hasnt-replaced-software-engineers/#atom-everything) ⭐️ 8.0/10

Arvind Narayanan and Sayash Kapoor published an essay arguing that AI has not and will not cause mass unemployment for software engineers, citing data from New York WARN Act filings showing zero AI-related layoffs in the first year of mandatory disclosure. This analysis directly challenges the prevalent narrative that AI will eliminate software engineering jobs, providing empirical evidence to counter fear-driven predictions. It matters because software engineering is considered one of the most AI-exposed professions, yet the data shows no displacement. The essay identifies three real bottlenecks in software engineering that resist automation: deciding and specifying what to build, verifying and being accountable for deliverables, and deep human understanding of the codebase, business, and environment. AI can assist with the first two but cannot replace the third.

rss · Simon Willison · Jun 14, 23:54

**Background**: The WARN Act requires employers to provide advance notice of mass layoffs; New York added an AI disclosure checkbox in March 2025. The narrative that AI will replace software engineers stems from rapid advances in code-generating AI models like GPT-4 and Copilot. However, software engineering involves much more than writing code, including requirements gathering, debugging, and system design.

**Tags**: `#AI`, `#software engineering`, `#employment`, `#job displacement`, `#technology policy`

---

<a id="item-11"></a>
## [Homelab AI Dev Platform with Forgejo and Opencode](https://rsgm.dev/post/ai-dev-platform/) ⭐️ 7.0/10

A developer detailed their homelab AI development platform using Forgejo for Git hosting and opencode as an AI coding agent, sparking a rich discussion on similar self-hosted setups. This showcases a growing trend of developers self-hosting AI tools to create customized, private AI-assisted coding environments, reducing reliance on cloud services and increasing control over workflows. The setup combines Forgejo, a self-hosted Git forge, with opencode, an open-source AI coding agent; one commenter integrated opencode into Forgejo action runners to enable AI-driven code generation from issues.

hackernews · rsgm · Jun 15, 15:09 · [Discussion](https://news.ycombinator.com/item?id=48542433)

**Background**: Forgejo is a self-hosted, lightweight Git forge written in Go, offering features like issue tracking, code review, and CI/CD. Opencode is an open-source AI coding agent that can generate and edit code in the terminal or integrate into development workflows. Together, they enable developers to build a private, AI-powered development platform on their own hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Forgejo">Forgejo</a></li>
<li><a href="https://forgejo.org/">Forgejo – Beyond coding. We forge.</a></li>
<li><a href="https://grokipedia.com/page/OpenCode">OpenCode</a></li>

</ul>
</details>

**Discussion**: Commenters shared similar homelab setups and expressed enthusiasm, with some discussing challenges like managing AI context across multiple rounds of interaction. One user mentioned their domain was filtered by Quad9 DNS.

**Tags**: `#homelab`, `#AI`, `#development-platform`, `#forgejo`, `#opencode`

---

<a id="item-12"></a>
## [US battery manufacturing output continues to break records](https://fred.stlouisfed.org/series/IPG33591S) ⭐️ 7.0/10

US battery manufacturing output reached record levels in recent months, as indicated by the FRED series IPG33591S. This is significant because increasing domestic battery production is critical for the US supply chain and national security, especially for EVs and energy storage. However, as community comments show, the US still lags far behind China and Europe. The FRED series tracks output of storage batteries (NAICS 33591) and includes primary batteries, which may inflate figures for the EV battery segment. The record output marks a recovery from the COVID dip.

hackernews · epistasis · Jun 15, 20:28 · [Discussion](https://news.ycombinator.com/item?id=48546616)

**Background**: Battery manufacturing is a key industry for the transition to electric vehicles and renewable energy storage. The US has been investing in domestic production through the Inflation Reduction Act and other policies, but faces global competition.

**Discussion**: Comments highlight that US cell production capacity (70 GWh in 2025) is dwarfed by China (1755 GWh) and Europe (252 GWh). Some note the data may include primary batteries and question relevance to EVs, while others see it as a positive step for national security.

**Tags**: `#battery manufacturing`, `#energy storage`, `#manufacturing`, `#supply chain`, `#EV industry`

---

<a id="item-13"></a>
## [Deep Dive into Commander Keen's Adaptive Tile Refresh](https://forgottenbytes.net/commander_keen.html) ⭐️ 7.0/10

A detailed technical analysis of the Commander Keen game engine has been published, focusing on its innovative adaptive tile refresh technique that enabled smooth scrolling on early PC hardware. This analysis sheds light on a groundbreaking technique that allowed early PC games to compete with console graphics, demonstrating the ingenuity of id Software's developers. It is valuable for understanding the history of game engine optimization and retro programming. The adaptive tile refresh technique uses EGA hardware features to perform scrolling in hardware and minimizes redrawing by tracking moved graphical elements. The article also discusses the historical context of PC versus console hardware limitations.

hackernews · mfiguiere · Jun 15, 17:52 · [Discussion](https://news.ycombinator.com/item?id=48544781)

**Background**: In the early 1990s, PCs lacked dedicated sprite hardware like consoles such as the SNES, making smooth side-scrolling challenging. John Carmack of id Software developed adaptive tile refresh, which used EGA's hardware scrolling capabilities and only redrew changed tiles, enabling games like Commander Keen to run smoothly. This technique was a significant innovation that helped define the PC gaming experience of that era.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Adaptive_tile_refresh">Adaptive tile refresh</a></li>
<li><a href="https://fabiensanglard.net/ega/">Commander Keen's Adaptive Tile Refresh - Fabien Sanglard</a></li>
<li><a href="https://retrocomputing.stackexchange.com/questions/22175/what-is-adaptive-tile-refresh-in-the-context-of-commander-keen">What is 'Adaptive Tile Refresh' in the context of Commander Keen?</a></li>

</ul>
</details>

**Discussion**: Commenters praised the analysis and recommended the book 'Masters of Doom' for historical context. One user noted the comparison between PC and SNES hardware, while another pointed to similar analysis on Cosmodoc. Overall sentiment was positive and appreciative of the technical deep dive.

**Tags**: `#game engine`, `#retro gaming`, `#programming`, `#computer history`, `#id Software`

---

<a id="item-14"></a>
## [Copper drug restores memory in Alzheimer's mice](https://www.monash.edu/news/articles/copper-drug-restores-memory-and-clears-toxic-alzheimers-proteins) ⭐️ 7.0/10

Monash University researchers demonstrated that the copper-delivering compound Cu(ATSM) significantly reduced toxic amyloid-beta proteins and improved spatial memory in a mouse model of Alzheimer's disease, with Aβ42 levels dropping by 42% and spatial learning improving by 44%. This research offers a potential new therapeutic approach for Alzheimer's disease, which currently has limited effective treatments, and the drug's prior safety evaluation for other conditions could accelerate its path to human clinical trials. Cu(ATSM) increased the abundance of P-gp clearance pumps at the blood-brain barrier by 24.1%, restoring the brain's ability to clear amyloid-beta. The study was published in ACS Chemical Neuroscience.

hackernews · bookofjoe · Jun 15, 14:48 · [Discussion](https://news.ycombinator.com/item?id=48542132)

**Background**: Alzheimer's disease is characterized by accumulation of amyloid-beta plaques in the brain, which are thought to contribute to neurodegeneration. Copper homeostasis is known to be disrupted in Alzheimer's, and copper dysregulation can lead to oxidative stress and mitochondrial damage. Cu(ATSM) is a compound that delivers copper specifically to cells, potentially restoring copper balance and activating clearance mechanisms.

<details><summary>References</summary>
<ul>
<li><a href="https://medicalxpress.com/news/2026-06-copper-drug-memory-toxic-alzheimer.html">Copper drug restores memory and clears toxic Alzheimer's ...</a></li>
<li><a href="https://scienceblog.com/a-copper-drug-cleared-toxic-proteins-and-restored-memory-in-alzheimers-mice/">A Copper Drug Cleared Toxic Proteins and Restored Memory in ...</a></li>
<li><a href="https://www.drugtargetreview.com/copper-drug-cuatsm-reduces-alzheimers-proteins-by-42-percent-in-preclinical-study/2135715.article">Copper drug Cu (ATSM) reduces Alzheimer's proteins by 42 ...</a></li>

</ul>
</details>

**Discussion**: Community comments express skepticism about the amyloid hypothesis, with one user citing Derek Lowe's view that amyloid-targeted therapies have repeatedly failed. Others note that while the drug works in mice, human trials are needed, and one commenter shares a personal story about their mother's early-onset Alzheimer's, highlighting the disease's heterogeneity and the controversy over current treatments.

**Tags**: `#Alzheimer's`, `#drug discovery`, `#neuroscience`, `#amyloid-beta`, `#preclinical`

---

<a id="item-15"></a>
## [Cloudflare CAPTCHA Only on Search URLs with Ampersand](https://simonwillison.net/2026/Jun/16/captcha-on-at-least-one-ampersand/#atom-everything) ⭐️ 7.0/10

Simon Willison shared a Cloudflare WAF custom rule that restricts Managed Challenge to search URLs containing at least one ampersand, preventing CAPTCHA for simple single-term searches like /search/?q=term. This practical tip improves site usability by reducing unnecessary CAPTCHA prompts for legitimate single-term searches, which is a common annoyance for site visitors and can impact user experience. The rule expression uses the Cloudflare Rules language: (http.request.uri.path wildcard r"/search/*" and http.request.uri.query contains "&"). Simon initially tried Cloudflare's MCP with Claude Code but switched to the Cloudflare API as MCP could not edit the required rules.

rss · Simon Willison · Jun 16, 00:21

**Background**: Cloudflare's Managed Challenge is an alternative to traditional CAPTCHAs that uses various challenges to verify human visitors. It can be configured via Cloudflare's Web Application Firewall (WAF) custom rules, which use a specific expression syntax to match traffic. Simon Willison runs a faceted search engine on his site, which aggressive crawlers were hitting, prompting him to add a CAPTCHA rule that he later refined to only trigger on complex queries with multiple parameters (indicated by an ampersand).

<details><summary>References</summary>
<ul>
<li><a href="https://developers.cloudflare.com/cloudflare-challenges/">Challenges · Cloudflare challenges docs</a></li>
<li><a href="https://blog.cloudflare.com/end-cloudflare-captcha/">The end of the road for Cloudflare CAPTCHAs</a></li>
<li><a href="https://developers.cloudflare.com/waf/custom-rules/">Custom rules · Cloudflare Web Application Firewall (WAF) docs</a></li>

</ul>
</details>

**Tags**: `#Cloudflare`, `#CAPTCHA`, `#WAF`, `#Configuration`, `#Simon Willison`

---

<a id="item-16"></a>
## [Personality clashes led US govt to shut down Anthropic's models](https://simonwillison.net/2026/Jun/15/axios-clashes-anthropics/#atom-everything) ⭐️ 7.0/10

An Axios report reveals that personality clashes between Anthropic and US government officials, combined with export control enforcement, led to the suspension of access to Anthropic's Claude Fable and Claude Mythos models. This incident highlights the growing tension between frontier AI labs and government regulators over export controls and safety standards, potentially setting a precedent for future government intervention in AI model deployment. The US government classified a jailbreak of Claude Mythos as a 'potential narrow, non-universal jailbreak,' and Anthropic's Constitutional Classifiers have so far prevented a universal jailbreak. Anthropic's Frontier Red Team, led by Logan Graham, is meeting with the Commerce Department to discuss the situation.

rss · Simon Willison · Jun 15, 14:57

**Background**: Anthropic developed two advanced models: Claude Fable 5, a public version with safeguards, and Claude Mythos 5, a more powerful version with stronger safeguards restricted to certain users. The US government issued a directive to suspend access to these models under export control laws, citing potential national security risks from jailbreaks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://red.anthropic.com/">red.anthropic.com</a></li>

</ul>
</details>

**Discussion**: Simon Willison, commenting on the Axios piece, expresses skepticism about resolving the standoff, noting that perfect jailbreak resistance may be impossible. He also questions whether Anthropic has addressed universal adversarial attacks from 2023.

**Tags**: `#Anthropic`, `#AI safety`, `#export controls`, `#AI policy`, `#US government`

---

<a id="item-17"></a>
## [Open weights insufficient; open training frameworks like FeynRL needed](https://www.reddit.com/r/MachineLearning/comments/1u6p7k3/open_weights_are_not_enough_we_need_open_training/) ⭐️ 7.0/10

A Reddit user argues that open weights are insufficient and introduces FeynRL, an open-source framework for explicit, modifiable RL post-training of LLMs, VLMs, and agents. This matters because current RL post-training for LLMs suffers from hidden system details that hinder algorithmic research; open training frameworks could democratize and accelerate progress in this critical area. FeynRL is built to be explicit and modular, supporting SFT, DPO, and RL post-training with vllm and llm, and runs on single to multi-GPU and cluster configurations.

reddit · r/MachineLearning · /u/summerday10 · Jun 15, 18:37

**Background**: RL post-training is a technique that uses reinforcement learning to fine-tune large language models (LLMs) after initial supervised fine-tuning, improving alignment, reasoning, or task performance. Open weights mean the model parameters are publicly available, but without access to the training code and infrastructure, researchers cannot easily reproduce or modify the training process.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/FeynRL-project/FeynRL">GitHub - FeynRL -project/ FeynRL : RL-first post-training framework for...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Richard_Feynman">Richard Feynman</a></li>

</ul>
</details>

**Tags**: `#open-source AI`, `#reinforcement learning`, `#LLM training`, `#research frameworks`, `#machine learning`

---

<a id="item-18"></a>
## [Cleo: A 2B Model for Text-to-SQL with Unified Harness](https://www.reddit.com/r/MachineLearning/comments/1u6udpb/cleo_trying_to_fit_full_analyst_behavior_in_a_2b/) ⭐️ 7.0/10

Cleo is a fine-tuned Qwen3.5-2B-Base model for text-to-SQL, trained and evaluated within a unified harness that supports live execution search and co-design of system components. This shows that small 2B models can be effective for text-to-SQL when training and inference conditions are aligned, potentially reducing costs and making such systems more accessible for resource-constrained environments. The unified harness enables training on the same gather-repair-answer contract used at inference, and allows searching over candidate queries using live execution evidence rather than just model likelihood. The model, harness, and datasets are fully open-source.

reddit · r/MachineLearning · /u/Dreeseaw · Jun 15, 21:43

**Background**: Text-to-SQL systems convert natural language queries into SQL database queries. Large language models (LLMs) are often used for this, but large models (e.g., 7B+ parameters) are resource-intensive. Fine-tuning a smaller model like Qwen3.5-2B-Base can achieve competitive performance while being more efficient. A unified harness ensures that training, evaluation, and inference share the same structure, improving consistency and performance.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.5-2B-Base">Qwen/ Qwen 3 . 5 - 2 B - Base · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#text-to-SQL`, `#small language models`, `#fine-tuning`, `#open-source`, `#AI engineering`

---

<a id="item-19"></a>
## [PrintGuard 2.0: Few-shot failure detector goes TFLite, runs in browser](https://www.reddit.com/r/MachineLearning/comments/1u6e9zc/printguard_20_shufflenetv2_fewshot_prototypical/) ⭐️ 7.0/10

PrintGuard 2.0 is released as a complete rewrite that exports its ShuffleNetV2 + prototypical network model to a ≈5 MB TFLite model via LiteRT, enabling unmodified execution on CPython and in browsers via Pyodide. This demonstrates a practical deployment of few-shot learning on edge devices using a lightweight runtime, making advanced failure detection accessible to any FDM printer without cloud dependency. The model remains a ShuffleNetV2 encoder with nearest-prototype classification, but now uses LiteRT inference and includes per-printer sensitivity/threshold sliders that map directly to prototype distances.

reddit · r/MachineLearning · /u/oliverbravery · Jun 15, 11:47

**Background**: ShuffleNetV2 is an efficient CNN architecture designed for mobile devices, balancing speed and accuracy. Prototypical networks learn a metric space where classification is done by computing distances to class prototypes, enabling few-shot learning. LiteRT (formerly TensorFlow Lite) is Google's runtime for on-device ML. Pyodide allows running Python in the browser via WebAssembly.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/1807.11164">[1807.11164] ShuffleNet V2: Practical Guidelines for Efficient CNN Architecture Design</a></li>
<li><a href="https://arxiv.org/abs/1703.05175">[1703.05175] Prototypical Networks for Few-shot Learning</a></li>
<li><a href="https://developers.googleblog.com/en/tensorflow-lite-is-now-litert/">TensorFlow Lite is now LiteRT - Google Developers Blog</a></li>
<li><a href="https://github.com/google-ai-edge/litert">GitHub - google-ai-edge/LiteRT: LiteRT, successor to ...</a></li>

</ul>
</details>

**Tags**: `#few-shot learning`, `#edge AI`, `#TFLite`, `#3D printing`, `#fault detection`

---

<a id="item-20"></a>
## [Developer's Nostalgic Ode to Computing](https://michaelenger.com/blog/i-love-the-computer/) ⭐️ 6.0/10

A developer published a personal essay titled 'I Love the Computer' reflecting on the pure joy of tinkering with computers, contrasting it with the frustrations of the modern tech industry. The essay resonates deeply with many developers who share a similar nostalgia, highlighting a cultural tension between the intrinsic joy of computing and the commercialized tech industry, and sparking discussions about AI, retro computing, and gatekeeping. The essay is a thoughtful personal reflection with high community engagement (136 points, 87 comments), but it is not technically groundbreaking; the author expresses a love for computing that feels lost in today's industry.

hackernews · speckx · Jun 15, 20:14 · [Discussion](https://news.ycombinator.com/item?id=48546441)

**Background**: The essay draws on the nostalgia of early computing when tinkering was central, contrasting it with modern complexities like AI and corporate software. Many developers feel disconnected from the pure fun they once had.

**Discussion**: Comments are mixed: some agree wholeheartedly ('Breaking something, poking at it...'), while others critique the author for gatekeeping ('how gatekeepy this sentiment is'). Some praise AI as a useful tool, and one commenter mentions writing 6502 assembler for pure joy.

**Tags**: `#computing culture`, `#tinkering`, `#nostalgia`, `#hacker community`

---

<a id="item-21"></a>
## [LLMs Show Consistent Name Preferences Across Generated Sites](https://www.reddit.com/r/MachineLearning/comments/1u6mn3q/ai_language_models_have_favorite_names_and_we/) ⭐️ 6.0/10

Researchers discovered that large language models have model-specific and version-specific name preferences, such as 'Elena Vasquez' and 'Marcus Chen' often appearing together in Claude-generated content. These name ensembles appear across dozens of websites, with the same trios co-occurring with AI-generated faces. This finding reveals a subtle but pervasive bias in LLM outputs that can serve as a fingerprint for identifying AI-generated content. It also highlights how models' internal priors can lead to correlated hallucinations that may propagate across the web. The paper (arxiv 2606.02184) shows that LLMs produce correlated character ensembles—pairs and trios—whose co-occurrence rates far exceed chance. The researchers stumbled on this while developing a model diffing method called CDD (Concurrent Diffing of Distributions).

reddit · r/MachineLearning · /u/CebulkaZapiekana · Jun 15, 17:07

**Background**: Large language models (LLMs) like GPT-4 and Claude generate text based on patterns learned from vast datasets. They sometimes default to high-probability names or concepts, leading to consistent biases. The concept of 'correlated ensembles' refers to groups of names that reliably appear together across many independent generations, indicating an underlying prior in the model's parameters.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2606.02184">[2606.02184] The Ghost Couple: Correlated LLM Name Priors and Their ...</a></li>

</ul>
</details>

**Tags**: `#LLMs`, `#AI bias`, `#model behavior`, `#generated content`

---

<a id="item-22"></a>
## [Quant Firms Rush to Diamond Sponsor ICML 2026](https://www.reddit.com/r/MachineLearning/comments/1u64rse/quant_firms_at_icml_2026_d/) ⭐️ 6.0/10

A Reddit post highlights that multiple quantitative finance firms have signed on as Diamond sponsors for the International Conference on Machine Learning (ICML) 2026. This trend signals the deepening integration of machine learning into quantitative trading and finance, as these firms invest heavily in cutting-edge ML research and talent. ICML is one of the top-tier machine learning conferences; Diamond sponsorship is the highest level, offering premier visibility and access to top researchers.

reddit · r/MachineLearning · /u/Intrepid_Discount_67 · Jun 15, 03:09

**Background**: Quantitative finance firms use advanced mathematical models and algorithms to execute trades. They increasingly rely on machine learning for predictive modeling, risk management, and automated strategies. ICML attracts leading ML researchers, making it a prime venue for recruitment and collaboration.

**Tags**: `#machine learning`, `#quantitative finance`, `#conferences`, `#industry sponsorship`

---

<a id="item-23"></a>
## [Biggest time sinks in embedded ML for sensor data](https://www.reddit.com/r/MachineLearning/comments/1u6q97f/embeddededge_ml_folks_what_actually_eats_the_most/) ⭐️ 6.0/10

A Reddit discussion asks embedded ML practitioners which part of sensor-based projects costs the most time: data collection, cleaning/labeling, or deployment. Understanding the real bottlenecks in embedded ML workflows can guide tool development and help startups focus on the most impactful features. The author is building a hardware-agnostic, GenAI-native platform similar to Edge Impulse but targeted at time-series data, and wants feedback on potential features like automatic data quality checks and AI-assisted labeling.

reddit · r/MachineLearning · /u/No-Bug-4879 · Jun 15, 19:13

**Background**: Edge Impulse is a leading platform for developing and deploying machine learning on edge devices, including microcontrollers. Time-series sensor data (e.g., from accelerometers) is common in embedded ML, but collecting, cleaning, and labeling such data manually is often a major bottleneck. A GenAI-native approach means the platform is built from the ground up to leverage generative AI models, potentially automating many of these tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.edgeimpulse.com/">Edge Impulse - The Leading Edge AI Platform</a></li>
<li><a href="https://www.st.com/content/st_com/en/partner/partner-program/partnerpage/Edge_Impulse.html">Edge Impulse - STMicroelectronics - STMicroelectronics</a></li>
<li><a href="https://en.wikipedia.org/wiki/Generative_AI">Generative AI - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#embedded ML`, `#edge computing`, `#time series`, `#data labeling`, `#model deployment`

---