---
layout: default
title: "Horizon Summary: 2026-07-11 (EN)"
date: 2026-07-11
lang: en
---

> From 25 items, 9 important content pieces were selected

---

1. [Nvidia, CoreWeave, Nebius: Inside the GPU Boom's Circular Financing](#item-1) ⭐️ 8.0/10
2. [Scaling PgBouncer to 4x Throughput with SO_REUSEPORT and Peering](#item-2) ⭐️ 8.0/10
3. [Prefer SQLite STRICT tables for data integrity](#item-3) ⭐️ 7.0/10
4. [Female rower beats male record in solo California-Hawaii crossing](#item-4) ⭐️ 7.0/10
5. [Nilay Patel: AR Glasses Inevitably Invade Privacy](#item-5) ⭐️ 7.0/10
6. [Why no per-author submission limit in ML research?](#item-6) ⭐️ 7.0/10
7. [Ant: New JavaScript Runtime and Ecosystem Sparks Debate](#item-7) ⭐️ 6.0/10
8. [Learn by Rebuilding Redis, Git, and a Database from Scratch](#item-8) ⭐️ 6.0/10
9. [Seeking better alternatives to HPSv3 for human preference prediction](#item-9) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Nvidia, CoreWeave, Nebius: Inside the GPU Boom's Circular Financing](https://io-fund.com/ai-stocks/nvidia-coreweave-nebius-circular-financing-gpu-boom) ⭐️ 8.0/10

The article reveals how Nvidia, CoreWeave, and Nebius are entangled in a circular financing loop, where Nvidia invests in CoreWeave and Nebius, which then spend heavily on Nvidia's GPUs, fueling the AI infrastructure boom. This analysis matters because it exposes the financial mechanics behind the massive GPU buildout, raising questions about sustainability and profitability. If the circular flow breaks, it could trigger a correction in the AI hardware market. Nvidia invested $2 billion in CoreWeave for a 9% equity stake, yet CoreWeave plans $35 billion in capital expenditure in 2026 alone, meaning Nvidia's investment covers only a fraction. This pattern also involves Nebius, another AI cloud provider.

hackernews · adletbalzhanov · Jul 11, 17:21 · [Discussion](https://news.ycombinator.com/item?id=48873836)

**Background**: Circular financing is a loop where an investor provides capital to a company, which then uses that capital to purchase the investor's products. In the AI sector, this has become common: large tech firms invest in AI startups, which then spend the money on cloud services or hardware from the investors. Nvidia's GPU dominance makes it a key player in such arrangements.

<details><summary>References</summary>
<ul>
<li><a href="https://builtin.com/articles/ai-circular-financing">How Circular Financing Is Fueling the AI Boom | Built In</a></li>
<li><a href="https://blogs.cuit.columbia.edu/gjb2124/circular-financing/">The Hidden Risk in AI's Circular Financing Ecosystem</a></li>
<li><a href="https://en.wikipedia.org/wiki/CoreWeave">CoreWeave</a></li>

</ul>
</details>

**Discussion**: Commenters debate whether the financing is truly circular, noting that Nvidia's $2 billion investment is only 5.7% of CoreWeave's annual CapEx. Others question the long-term profitability of such builds, while one reminds that Nebius originated from Yandex, highlighting geopolitical connections.

**Tags**: `#Nvidia`, `#GPU`, `#cloud computing`, `#financing`, `#AI infrastructure`

---

<a id="item-2"></a>
## [Scaling PgBouncer to 4x Throughput with SO_REUSEPORT and Peering](https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres) ⭐️ 8.0/10

The ClickHouse team achieved a 4x throughput increase for PgBouncer, a PostgreSQL connection pooler, by leveraging the SO_REUSEPORT socket option and enabling PgBouncer's built-in peering feature. This optimization allows PgBouncer to handle significantly more connections per machine without additional hardware, which is critical for scaling PostgreSQL workloads in high-traffic environments. SO_REUSEPORT allows multiple processes to bind to the same port, distributing incoming connections across them, while peering enables cancel requests to be forwarded between processes if they land on the wrong one.

hackernews · saisrirampur · Jul 11, 15:28 · [Discussion](https://news.ycombinator.com/item?id=48872874)

**Background**: PgBouncer is a lightweight connection pooler for PostgreSQL, commonly used to manage database connections. Traditionally, running multiple PgBouncer instances required separate ports or complex load balancing. SO_REUSEPORT is a Linux socket option (since kernel 3.9) that enables multiple sockets to share the same port, simplifying horizontal scaling of server processes.

<details><summary>References</summary>
<ul>
<li><a href="https://lwn.net/Articles/542629/">The SO_REUSEPORT socket option [LWN.net]</a></li>
<li><a href="https://postgrespro.com/docs/postgrespro/current/pgbouncer">Postgres Pro Standard : Documentation: 18: pgbouncer</a></li>

</ul>
</details>

**Discussion**: Community members discussed alternative tools like Odyssey and pgdog, and inquired about the simplicity of setting up peering in PgBouncer. Some noted that running PgBouncer in Kubernetes already made multi-process deployment straightforward.

**Tags**: `#pgbouncer`, `#performance`, `#postgresql`, `#connection pooling`, `#scaling`

---

<a id="item-3"></a>
## [Prefer SQLite STRICT tables for data integrity](https://evanhahn.com/prefer-strict-tables-in-sqlite/) ⭐️ 7.0/10

The article argues that developers should use SQLite's STRICT tables mode to enforce column types and improve data integrity, rather than relying on the default flexible typing. This matters because STRICT tables address a common criticism of SQLite—its lack of type enforcement—making it more suitable for applications requiring robust data integrity, while still benefiting from SQLite's simplicity. STRICT tables, available since SQLite 3.37.0, must be explicitly declared per table; they enforce strict type checks but do not support all data types like DATE, which may require storing dates as TEXT or INTEGER.

hackernews · ingve · Jul 11, 17:33 · [Discussion](https://news.ycombinator.com/item?id=48873940)

**Background**: SQLite is known for its flexible typing, where column data types are merely hints; any value can be inserted into any column regardless of declared type. This design is intentional, as documented in the 'Flexible Typing' philosophy, but can cause subtle bugs when the same database is accessed by multiple applications or when migrating schema. STRICT tables provide an opt-in alternative that rejects type mismatches at insertion time, aligning with traditional SQL expectations.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sqlite.org/stricttables.html">STRICT Tables</a></li>
<li><a href="https://antonz.org/sqlite-strict-tables/">STRICT tables in SQLite</a></li>

</ul>
</details>

**Discussion**: Community comments show a divide: some developers strongly prefer STRICT as the default for better data integrity, while others defend SQLite's flexible typing based on its use cases (e.g., embedded, single-application). Notable points include that STRICT tables lack date support and that the SQLite team has stated rigid type enforcement may not always be beneficial.

**Tags**: `#SQLite`, `#data integrity`, `#database schemas`, `#type enforcement`, `#software engineering best practices`

---

<a id="item-4"></a>
## [Female rower beats male record in solo California-Hawaii crossing](https://www.theguardian.com/us-news/2026/jul/04/california-hawaii-rowing-solo-journey) ⭐️ 7.0/10

A female rower completed the fastest solo crossing from California to Hawaii, beating the previous male record by six days. This achievement highlights the extraordinary physical and mental endurance required for solo ocean crossings and challenges gender stereotypes in extreme endurance feats. The rower, Kelsey Pfendler, took 44 days to cover approximately 2,400 nautical miles, surpassing the previous male record by six days. Her boat was 21 feet long and 5.5 feet wide, designed for self-sufficiency.

hackernews · speckx · Jul 11, 17:03 · [Discussion](https://news.ycombinator.com/item?id=48873692)

**Background**: Solo ocean rowing is among the most demanding endurance challenges, requiring months of preparation and extreme resilience. Rowers face treacherous waves, isolation, and the need to carry all supplies. The California to Hawaii route is a classic but difficult crossing due to prevailing winds and currents.

**Discussion**: Commenters expressed awe at the mental and physical endurance required, with one noting the difficulty even on short crossings. Another highlighted that Kelsey is the fastest human to make the crossing, beating the male record. There was also curiosity about the boat design and logistics.

**Tags**: `#rowing`, `#endurance`, `#ocean crossing`, `#human achievement`, `#record`

---

<a id="item-5"></a>
## [Nilay Patel: AR Glasses Inevitably Invade Privacy](https://simonwillison.net/2026/Jul/10/nilay-patel/#atom-everything) ⭐️ 7.0/10

Nilay Patel argued on The Vergecast that augmented reality glasses require always-on cameras and cloud processing, making privacy invasion inevitable, and questioned whether the societal cost is worth it. This argument challenges the prevailing optimism about AR as the next computing platform, highlighting a fundamental ethical trade-off that could shape product design and regulation. Patel notes that no chip small enough to fit in a glasses stem can handle real-time video processing locally, so data must be sent to the cloud, or the device must be bulky like Apple Vision Pro.

rss · Simon Willison · Jul 10, 17:05

**Background**: Augmented reality glasses overlay digital information onto the real world. They require cameras to capture the user's view and powerful processors to analyze and render graphics in real time. Current hardware limitations force either cloud processing (raising privacy concerns) or bulky designs. Cloud-based face recognition for AR glasses is already an active research area.

<details><summary>References</summary>
<ul>
<li><a href="https://ieeexplore.ieee.org/document/10322211/">Cloud-Based Face Recognition for Augmented Reality Glasses | IEEE Conference Publication | IEEE Xplore</a></li>
<li><a href="https://www.researchgate.net/publication/391142373_Energy_Efficient_ARVR_Edge_Processing_Architecture_and_Optimization">(PDF) Energy Efficient AR /VR Edge Processing : Architecture and...</a></li>

</ul>
</details>

**Tags**: `#augmented reality`, `#privacy`, `#cloud computing`, `#technology ethics`, `#hardware limitations`

---

<a id="item-6"></a>
## [Why no per-author submission limit in ML research?](https://www.reddit.com/r/MachineLearning/comments/1usq43t/why_doesnt_the_ml_research_community_limit_the/) ⭐️ 7.0/10

A Reddit post questions why the ML research community does not limit submissions per author to manage review workload, citing successful examples from security (CCS) and computer architecture (DAC) conferences. This issue directly impacts review quality in ML conferences like those using ACL Rolling Review (ARR), where high submission volumes strain reviewers. Limiting submissions per author could improve review quality and reduce reviewer burnout. The post notes that other fields have successfully used per-author limits for years, e.g., ACM CCS in security and DAC in architecture. The ML community's cultural resistance may stem from its emphasis on rapid iteration and open submission.

reddit · r/MachineLearning · /u/alafaya101 · Jul 10, 14:59

**Background**: ACL Rolling Review (ARR) is a peer review platform for computational linguistics and NLP that has seen skyrocketing submission numbers, leading to reviewer overload. In fields like security, conferences like CCS limit each author to a small number of submissions (e.g., 2-3) to keep the review process manageable. The post questions why similar policies are not adopted in ML, which often suffers from low review quality due to excessive submissions.

<details><summary>References</summary>
<ul>
<li><a href="http://aclrollingreview.org/cfp">CALL FOR PAPERS – ACL Rolling Review – A peer review platform for the Association for Computational Linguistics</a></li>
<li><a href="https://dl.acm.org/doi/proceedings/10.1145/2810103?preflayout=flat">Proceedings of the 22nd ACM SIGSAC Conference on Computer and...</a></li>

</ul>
</details>

**Tags**: `#ML research`, `#peer review`, `#submission policies`, `#community discussion`

---

<a id="item-7"></a>
## [Ant: New JavaScript Runtime and Ecosystem Sparks Debate](https://antjs.org/) ⭐️ 6.0/10

Ant is a new JavaScript runtime built from scratch with its own engine, along with a package manager, package registry, deployment platform, and desktop app framework. It aims to be a coherent alternative to existing JavaScript stacks while maintaining compatibility. If successful, Ant could offer a lightweight, integrated ecosystem that challenges established runtimes like Node.js, Deno, and Bun. However, community skepticism about its origins and trustworthiness may hinder adoption. Ant is a single 9 MB binary that supports npm packages, TypeScript, VM-isolated sandboxing, and WebAssembly. It also introduces a new package registry at ants.land and an Electron-like desktop app builder called Ant Desktop.

hackernews · theMackabu · Jul 11, 20:07 · [Discussion](https://news.ycombinator.com/item?id=48875377)

**Background**: A JavaScript runtime executes JavaScript code outside a browser, with popular examples being Node.js, Deno, and Bun. Building a runtime from scratch is a massive undertaking, typically requiring a team of engineers over years. Ant claims to be built from scratch, but community members have pointed out that it originally used AGPL-licensed code from the Elk engine, raising concerns about transparency and licensing.

<details><summary>References</summary>
<ul>
<li><a href="https://antjs.org/">Ant, a lightweight JavaScript runtime</a></li>
<li><a href="https://github.com/themackabu/ant/">GitHub - theMackabu/ant: javascript for 🐜's, a tiny runtime with big ambitions</a></li>
<li><a href="https://news.ycombinator.com/item?id=48875377">Show HN: Ant – A JavaScript runtime and ecosystem | Hacker News</a></li>

</ul>
</details>

**Discussion**: Community comments reveal mixed reactions: some question the 'from-scratch' claim after discovering it was based on an AGPL codebase (Elk), while others worry about the author's trustworthiness due to a broken company website and the use of a personal GitHub account. There are also concerns about naming conflict with Apache Ant, and skepticism about performance claims against mature runtimes.

**Tags**: `#JavaScript`, `#runtime`, `#ecosystem`, `#controversy`, `#open-source`

---

<a id="item-8"></a>
## [Learn by Rebuilding Redis, Git, and a Database from Scratch](https://shipthatcode.com/) ⭐️ 6.0/10

A new free website offers hands-on projects to rebuild Redis, Git, and a database from scratch, providing a practical approach to learning systems internals. This resource makes deep systems knowledge accessible for free, potentially lowering the barrier for developers to understand core infrastructure. However, concerns about originality and similarity to existing platforms like CodeCrafters may affect its impact. The projects cover three popular systems: Redis (in-memory data store), Git (version control), and a generic database. Users must sign up, though some report a 'rate limit exceeded' error.

hackernews · acley · Jul 11, 13:40 · [Discussion](https://news.ycombinator.com/item?id=48871973)

**Background**: Rebuilding well-known systems from scratch is a classic learning technique that helps developers understand complex internals. Platforms like CodeCrafters and books like 'Building Git' have popularized this approach, but this new resource is free.

**Discussion**: Comments question the originality, suggesting content may be cribbed from existing sources and laundered through LLMs. There is also skepticism about how it differs from CodeCrafters, though some appreciate it being free.

**Tags**: `#learning`, `#systems`, `#tutorial`, `#hands-on`

---

<a id="item-9"></a>
## [Seeking better alternatives to HPSv3 for human preference prediction](https://www.reddit.com/r/MachineLearning/comments/1utdj1f/predicting_human_preference_for_generated_image/) ⭐️ 6.0/10

The author of imagebench.ai tested HPSv3 for predicting human preference on generated image pairs and found limitations, then asked the community for better alternatives. Choosing the right human preference model is crucial for evaluating and improving text-to-image generation, as it directly impacts the quality of automated feedback. HPSv3 is built on a dataset of 1.08M text-image pairs and 1.17M pairwise comparisons, yet the author reports it has many limitations in practical use.

reddit · r/MachineLearning · /u/dh7net · Jul 11, 07:36

**Background**: Human preference scores are automated metrics trained on human annotations to judge the quality of AI-generated images. HPSv3 is the latest in a series of such models, but no single model is perfect. Alternatives include PickScore, HPSv2, and VisionReward, each with different strengths.

<details><summary>References</summary>
<ul>
<li><a href="https://mizzenai.github.io/HPSv3.project/">HPSv 3 : Towards Wide-Spectrum Human Preference Score</a></li>
<li><a href="https://arxiv.org/html/2508.03789v2">HPSv 3 : Towards Wide-Spectrum Human Preference Score</a></li>

</ul>
</details>

**Tags**: `#image generation`, `#human preference`, `#evaluation`, `#HPSv3`, `#machine learning`

---