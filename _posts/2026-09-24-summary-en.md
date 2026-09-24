---
layout: default
title: "Horizon Summary: 2026-09-24 (EN)"
date: 2026-09-24
lang: en
---

> From 31 items, 15 important content pieces were selected

---

1. [Qualcomm Brings Linux Support to Snapdragon X2 Laptops](#item-1) ⭐️ 8.0/10
2. [Essay: LLM tokens may soon cost less than a grep call](#item-2) ⭐️ 8.0/10
3. [Claude Opus 5.5, GPT-6 Sol/Luna launch as model prices halve](#item-3) ⭐️ 8.0/10
4. [Xiaomi releases MiMo-V2.6 multimodal models, trained with $3.5M RL](#item-4) ⭐️ 8.0/10
5. [Anthropic says Claude found CRISPR-like enzyme system in raw DNA](#item-5) ⭐️ 7.0/10
6. [VSCode Remote-SSH Agent Ships Itself Over SSH, Enabling Reverse Code Execution](#item-6) ⭐️ 7.0/10
7. [Google launches Gemini 3.8 text-to-speech with 30-second voice cloning](#item-7) ⭐️ 7.0/10
8. [Radicle discloses unencrypted, unauthenticated node traffic exposing private repos](#item-8) ⭐️ 7.0/10
9. [Complex KDA Extends Kimi Delta Attention's Expressivity to Orthogonal DPLR Matrices](#item-9) ⭐️ 7.0/10
10. [Qonto launches QontoFAQ benchmark to curb retrieval benchmaxxing](#item-10) ⭐️ 7.0/10
11. [Meta Unveils $1,300 VR Glasses With Narrower Field of View Than Quest 3](#item-11) ⭐️ 6.0/10
12. [Italy's parliament votes to pave way for return to nuclear energy](#item-12) ⭐️ 6.0/10
13. [Raymond Chen Recounts the History of Windows Scroll Bar Shortcuts](#item-13) ⭐️ 6.0/10
14. [llm 0.36 adds GPT-6 Sol and Luna, plus conversation-support plugin flag](#item-14) ⭐️ 6.0/10
15. [Templar simulates stage skipping for pipeline-parallel fault tolerance](#item-15) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Qualcomm Brings Linux Support to Snapdragon X2 Laptops](https://www.qualcomm.com/news/onq/2026/09/snapdragon-summit-agentic-ai-pcs-linux) ⭐️ 8.0/10

Qualcomm announced at its Snapdragon Summit that Linux support is coming to Snapdragon X2 Series laptops, including upstreaming core drivers for the Hexagon NPU and Adreno GPU. Early enablement is already appearing beyond Linux itself, with the first OpenBSD/arm64 commits for these machines and confirmation that ARM EL2 (and therefore KVM virtualization) now works, unlike on previous generations. Lack of usable Linux support was one of the biggest blockers keeping developers and enthusiasts away from Snapdragon X laptops, so upstreaming the NPU and GPU drivers could make Qualcomm's ARM64 notebooks a genuine alternative to Apple Silicon for Linux users and give OEMs a path to ship Linux preinstalled. It also matters for the wider ARM laptop ecosystem, since open mainline drivers reduce the fragmentation that has historically slowed ARM-on-Linux adoption. OpenBSD developer Tobias Heider (tobhe@), who also works for Canonical, has already committed the first OpenBSD/arm64 pieces for Snapdragon X2 Elite laptops, getting USB, keyboard and touchpad working in ACPI mode on the HP EliteBook X G2q, and has demoed Ubuntu with ARM EL2 functioning, which implies KVM support. Early Geekbench comparisons place the Snapdragon X2 Elite Extreme X2E-96-100 not far behind Apple's M5 Pro, though the drivers are still upstream work in progress rather than finished, shipping code.

hackernews · aaronday · Sep 23, 22:38 · [Discussion](https://news.ycombinator.com/item?id=49823582)

**Background**: Snapdragon X Series are Qualcomm's ARM64 chips for laptops, built around an Oryon CPU plus a Hexagon NPU (a specialized accelerator for on-device AI inference) and an Adreno GPU. "Upstreaming" means contributing driver code to the mainline Linux kernel and other core projects so that support ships automatically with future distributions, instead of living in a vendor-specific, semi-proprietary fork. OpenBSD is a security-focused, freely licensed Unix-like operating system whose developers often pioneer new ARM hardware support; KVM is the Linux kernel's built-in virtualization layer, which requires ARM's EL2 exception level to run virtual machines.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Neural_processing_unit">Neural processing unit - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Upstream_(software_development)">Upstream (software development) - Wikipedia</a></li>
<li><a href="https://www.openbsd.org/">OpenBSD</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion is largely enthusiastic and optimistic: commenters describe this as huge, note that missing Linux support previously pushed them away from Snapdragon X laptops, and praise Qualcomm for upstreaming open drivers rather than shipping a semi-proprietary solution like ChromeOS device support. Several people highlight that Snapdragon X2 is the closest competition Apple's M-series has in the laptop space, arguably ahead of Intel and AMD, while a recurring concern is that the original X Elite was also promised good Linux support and it never materialized, so people want to see this actually ship.

**Tags**: `#Linux`, `#ARM`, `#Qualcomm`, `#Snapdragon X2`, `#Open Source`

---

<a id="item-2"></a>
## [Essay: LLM tokens may soon cost less than a grep call](https://jyn.dev/tokens-too-cheap-to-meter/) ⭐️ 8.0/10

A blog post on jyn.dev titled "Tokens too cheap to meter" argues that LLM inference costs are falling so fast that a single model call may soon become cheaper than running a conventional tool call such as grep. In the discussion, readers note the author's claim that a call to a model like "GPT-5.6 Luna" is currently only about 4-5 orders of magnitude more expensive than a grep invocation, and that at the present rate of improvement that gap could close. If model calls really do become cheaper than trivial local tools, the design calculus for AI agents changes: developers would stop optimizing around which operations are expensive and start treating inference as a nearly free primitive. It also puts pressure on the business models of AI providers, who are spending enormous sums on infrastructure in the expectation that future profits will justify it. The core comparison is deliberately rough — a 4-5 order-of-magnitude cost gap between a model call and grep is an estimate, not a benchmark, and it says nothing about the quality or reliability of the output relative to a deterministic tool. Commenters also point out that the essay treats the continued decline of per-call costs almost as a given, without modeling what happens when efficiency gains slow.

hackernews · teoruiz · Sep 23, 09:21 · [Discussion](https://news.ycombinator.com/item?id=49813482)

**Background**: Large language models process text as tokens — units produced by a tokenizer that may correspond to a whole word, part of a word, or punctuation — and API providers bill by the token, so token price is the basic unit of LLM economics. Tool calling (also called function calling) is the mechanism that lets a model invoke external functions, databases, or command-line utilities such as grep, which is a standard Unix search tool for matching text patterns in files. The phrase "too cheap to meter" comes from a 1954 speech by Lewis Strauss, then chairman of the US Atomic Energy Commission, predicting that nuclear power would make electricity essentially free to consumers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.geeksforgeeks.org/artificial-intelligence/tokens-and-context-windows-in-llms/">Tokens and Context Windows in LLMs - GeeksforGeeks</a></li>
<li><a href="https://www.ibm.com/think/topics/tool-calling">What Is Tool Calling? | IBM</a></li>

</ul>
</details>

**Discussion**: The Hacker News thread (229 upvotes, 179 comments) is broadly admiring of the essay but skeptical of its extrapolation: one commenter invokes Stein's Law ("if something cannot go on forever, it will stop") to argue these efficiency gains will not continue indefinitely. Others criticize the piece for glossing over business-model viability, given the scale of infrastructure investment, and several draw the historical parallel to nuclear power's unfulfilled "too cheap to meter" promise, noting their electricity bills were in fact metered and large. A separate complaint targets the ubiquitous Artificial Analysis cost/performance charts that underlie such comparisons.

**Tags**: `#LLM economics`, `#AI infrastructure`, `#cost trends`, `#Hacker News discussion`, `#AGI business models`

---

<a id="item-3"></a>
## [Claude Opus 5.5, GPT-6 Sol/Luna launch as model prices halve](https://simonwillison.net/2026/Sep/22/opus-and-sol-and-luna/) ⭐️ 8.0/10

Within roughly 48 hours, xAI released Grok 4.7, Xiaomi released MiMo v2.6 Flash/Pro, Anthropic released Claude Opus 5.5, and OpenAI released GPT-6 Sol and GPT-6 Luna about an hour later. Simon Willison's first impressions highlight that GPT-6 Luna costs $0.10/M input and $0.50/M output — half the price of GPT-5.6 Luna — while GPT-6 Sol matches GPT-5.6 Terra's pricing at $2/M input and $10/M output. This cluster of releases signals an escalating price war among frontier labs: comparable capability is now available at roughly half the previous cost, which directly lowers the cost base for anyone building applications on LLM APIs. It also compresses the market for older tiers — with GPT-6 Sol priced the same as GPT-5.6 Terra, the author notes any remaining reason to use Terra has evaporated. The comparison is even starker because GPT-5.6 had a scheduled 25% price increase for November, so GPT-6 is half the price of the promotional pricing of those models; at $0.10/$0.50, GPT-6 Luna is among the cheapest models OpenAI has ever shipped, beaten only by the weaker GPT-4.1 Nano and GPT-5 Nano. Grok 4.7 at $2/$6 is now roughly matched on input and only somewhat ahead on output versus GPT-6 Sol, while Claude Opus 5.5 sits at the higher $4/$20 tier.

rss · Simon Willison · Sep 22, 23:46

**Background**: Simon Willison is a well-known practitioner-blogger who evaluates new LLM releases quickly and pragmatically, often using his informal "pelican riding a bicycle" SVG prompt as a qualitative sanity check alongside formal benchmarks. Frontier model pricing is quoted per million tokens (input, cached input, and output), and caching discounts and promotional rates can shift effective costs substantially, which is why a headline price cut is a major practical event for API consumers. The pelican test has become a widely recognized informal benchmark that labs are occasionally accused of optimizing for.

<details><summary>References</summary>
<ul>
<li><a href="https://x.ai/news/grok-4-7">Introducing Grok 4.7 | SpaceXAI</a></li>
<li><a href="https://mimo.xiaomi.com/mimo-v2-6">MiMo-V2.6 | Xiaomi</a></li>
<li><a href="https://simonwillison.net/2026/Jul/16/kimi-k3/">Kimi K3, and what we can still learn from the pelican benchmark</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#OpenAI`, `#Anthropic`, `#model-releases`, `#pricing`

---

<a id="item-4"></a>
## [Xiaomi releases MiMo-V2.6 multimodal models, trained with $3.5M RL](https://www.reddit.com/r/MachineLearning/comments/1wn36d4/xiaomi_releases_mimov26_frontier_intelligence_all/) ⭐️ 8.0/10

Xiaomi released the MiMo-V2.6 family, a line of multimodal "frontier" models, and disclosed that the total reinforcement learning training cost was only $3.5M. The release ships with a live public benchmark dashboard, and the models have already gone live on OpenRouter. If the reported numbers hold up, MiMo-V2.6 shows that a hardware and consumer-electronics company can reach the front of the open-weight pack for a fraction of what Western labs spend, intensifying price and capability pressure across the open-source LLM ecosystem. The explicit disclosure of RL training cost is also unusual transparency that gives researchers a real data point for estimating post-training budgets. The flagship MiMo-V2.6-Pro is a 1T+ parameter model aimed at agentic coding, research, and long-horizon tasks, while MiMo-V2.6-Flash is an open-source 309B Mixture-of-Experts model with only 15B active parameters. Pro reportedly scores 46.32 on the Artificial Analysis Intelligence Index — the highest of any open-weight model, ahead of Kimi K3 and Qwen3.8 Max — and Xiaomi's own materials show it being used to design a new metal-organic framework (MOF) for adsorbing PFAS "forever chemicals".

reddit · r/MachineLearning · /u/we_are_mammals · Sep 22, 07:56

**Background**: "Multimodal" means the model handles more than text — typically images and other input types as well. Reinforcement learning (RL) post-training is the stage after pre-training where a model is optimized against reward signals rather than raw text prediction, and it is widely considered the main driver of recent reasoning and agentic gains; the $3.5M figure covers only this stage, not pre-training. Mixture-of-Experts (MoE) is an architecture that routes each token to a small subset of parameters, so a 309B-parameter model can run at roughly 15B active parameters, cutting inference cost. The Artificial Analysis Intelligence Index is an aggregated public leaderboard score, and the Reddit discussion uses "benchmaxxing" as slang for aggressively optimizing models for such benchmarks.

<details><summary>References</summary>
<ul>
<li><a href="https://mimo.xiaomi.com/mimo-v2-6">MiMo - V 2 . 6 | Xiaomi</a></li>
<li><a href="https://www.linkedin.com/posts/openrouter_xiaomi-mimo-v26-is-live-on-openrouter-three-activity-7507908531761610754-Y3hU">Xiaomi MiMo - V 2 . 6 is live on OpenRouter. Three new models from...</a></li>
<li><a href="https://www.youtube.com/watch?v=WWYH-Lw-i2g">Xiaomi MiMo - V 2 . 6 Is INSANE… Open-Source AI Just... - YouTube</a></li>

</ul>
</details>

**Tags**: `#AI/ML`, `#Large Language Models`, `#Multimodal AI`, `#Model Release`, `#Reinforcement Learning`

---

<a id="item-5"></a>
## [Anthropic says Claude found CRISPR-like enzyme system in raw DNA](https://www.anthropic.com/news/claude-discovers-novel-enzyme-system) ⭐️ 7.0/10

Anthropic reports that its Claude model, working as an agent on raw genomic sequence, identified a previously undescribed tandem repeat array sitting next to a reverse transcriptase gene, forming a CRISPR-like system the preprint calls an ART array. The arrays carry roughly 3 to 21 copies of a short non-coding repeat, echoing the guide-storage layout of CRISPR. If it holds up, this is a high-profile demonstration of an AI agent contributing to a genuine biological finding, which intensifies the debate over how much autonomy and credit AI systems deserve in science. It also hints at a potentially new class of programmable nucleic-acid-targeting systems, though any therapeutic relevance is far off. The core of the finding is a known retron-like reverse transcriptase; the novelty lies in the previously undescribed repeat arrangement around it rather than in the enzyme itself, and the work is a preprint that has not been peer-reviewed. Commenters also stress that for CRISPR-based therapeutics the main bottleneck remains delivery, not nuclease efficiency or targeting coverage.

hackernews · raahelb · Sep 23, 18:06 · [Discussion](https://news.ycombinator.com/item?id=49820134)

**Background**: CRISPR-Cas systems give bacteria adaptive immunity: a Cas nuclease is guided by short RNA spacers stored in a repeat array, letting it cut matching DNA. Reverse transcriptases (RTs) are enzymes that copy RNA back into DNA, and some CRISPR-Cas systems are known to be associated with RTs — sometimes fused to Cas1 — which may let RNA-derived spacers be written into the array. LLM agents are AI systems that pair a language model with planning, memory and tools so they can carry out multi-step tasks such as scanning sequence data.

<details><summary>References</summary>
<ul>
<li><a href="https://thenextweb.com/news/anthropic-claude-enzyme-system-crispr-like-repeats">Anthropic says Claude found a new enzyme system with CRISPR - like ...</a></li>
<li><a href="https://www.nature.com/articles/s41598-017-07828-y">The Reverse Transcriptases Associated with CRISPR-Cas Systems | Scientific Reports</a></li>
<li><a href="https://www.promptingguide.ai/research/llm-agents">LLM Agents | Prompt Engineering Guide</a></li>

</ul>
</details>

**Discussion**: Top commenters are skeptical of the framing, arguing the finding centers on a known retron-like reverse transcriptase and that a sober description would be "Claude identified a previously undescribed genomic arrangement around a known reverse transcriptase — not all that sexy." Others enjoy reliving the discovery through the agent's own transcript quotes, while some press Anthropic to clarify whether it is selling human-agent collaboration or autonomous discovery, and a few veer into dark jokes about dual-use risks.

**Tags**: `#AI for science`, `#CRISPR`, `#LLM agents`, `#genomics`, `#Anthropic`

---

<a id="item-6"></a>
## [VSCode Remote-SSH Agent Ships Itself Over SSH, Enabling Reverse Code Execution](https://fly.io/blog/vscode-ssh-wtf/) ⭐️ 7.0/10

Fly.io published a deep-dive blog post titled "VSCode's SSH Agent Is Bananas" that analyzes how the VS Code Remote-SSH extension bootstraps its server binary over the SSH tunnel itself and, in doing so, opens a bidirectional code-execution channel between the remote host and the local machine. The post triggered a 115-point Hacker News discussion in which practitioners debated whether this is a genuine security hazard or simply the expected behavior of a remote development tool. The analysis spotlights an under-examined security surface in one of the most widely used developer tools, since developers who point Remote-SSH at production servers or shared machines may not realize the extension grants the remote host a channel back into their local environment. It feeds into the broader industry conversation about how much implicit trust remote development tooling should be given by default. The behavior is architectural rather than a bug: VS Code ships its server component over SSH/SFTP partly because remote machines cannot be assumed to have outbound internet access, making the tunnel the natural bootstrap path. Commenters argue the more serious risk is the inverse direction — a compromised remote host abusing the channel to run arbitrary code on the local machine.

hackernews · Rapzid · Sep 23, 21:01 · [Discussion](https://news.ycombinator.com/item?id=49822555)

**Background**: VS Code Remote-SSH is an official extension that lets you open a folder on any remote machine, VM, or container with a running SSH server and use VS Code's full feature set locally, which requires installing a VS Code Server component on the remote host. Because SSH allows additional channels to be multiplexed over a single connection, tools can forward traffic and requests in both directions — the same mechanism used by SSH agent forwarding to reuse local keys on a remote server. Fly.io's post examines what that bidirectional capability means when the component being tunnelled is a tool designed to edit files and execute commands.

<details><summary>References</summary>
<ul>
<li><a href="https://code.visualstudio.com/docs/remote/ssh">Remote Development using SSH</a></li>
<li><a href="https://code.visualstudio.com/docs/remote/vscode-server">Visual Studio Code Server</a></li>
<li><a href="https://docs.github.com/en/authentication/connecting-to-github-with-ssh/using-ssh-agent-forwarding">Using SSH agent forwarding - GitHub Docs</a></li>

</ul>
</details>

**Discussion**: The Hacker News thread largely pushed back on the framing: several commenters argued that tunneling and remote command execution are inherent to the feature set, and that installing such a tool on production servers is the user's own mistake. The most substantive counterpoint came from a commenter noting that the inbound direction is fine, but a compromised remote gaining control of the local machine is not, while another questioned whether the same reverse-execution risk applies to VSCodium's extensions.

**Tags**: `#vscode`, `#ssh`, `#security`, `#remote-development`, `#developer-tools`

---

<a id="item-7"></a>
## [Google launches Gemini 3.8 text-to-speech with 30-second voice cloning](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-8-text-to-speech/) ⭐️ 7.0/10

Google released Gemini 3.8 text-to-speech, a new model that can recreate consistent vocal profiles from just a 30-second audio sample of your own voice or a voice you have the rights to use. The release ships with built-in consent verification, SynthID watermarking, and C2PA credentials intended to protect both developers and the vocal talent whose voices are cloned. Google had previously held back voice cloning capabilities out of abuse concerns, so shipping it now signals that cloning has become a commodity feature rather than a withheld research demo. It affects developers building audiobooks, assistants, and localization pipelines, as well as anyone whose voice could now be replicated from a short sample. Safety comes from consent verification plus two provenance mechanisms: SynthID watermarking embedded in the generated audio and C2PA content credentials attached to outputs. However, availability is inconsistent across Google's consumer, prosumer, and cloud platforms, and the underlying models do not always expose the same input and output modalities on each — for example, Omni Flash reportedly offers video and text input on consumer and prosumer tiers but video-only output on GCP.

hackernews · swolpers · Sep 23, 15:29 · [Discussion](https://news.ycombinator.com/item?id=49817615)

**Background**: Text-to-speech (TTS) systems convert written text into spoken audio, and voice cloning is the AI technique that lets such a system imitate a specific person's voice so it can say things they never actually said. Because cloned audio can be used in scams, phishing, and misinformation, the technology is often described as audio deepfake, and providers increasingly pair it with provenance signals — SynthID is Google's imperceptible watermark for AI-generated content, while C2PA credentials are an industry standard for recording how a piece of media was created and edited.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Voice_cloning">Voice cloning</a></li>
<li><a href="https://grokipedia.com/page/Voice_cloning">Voice cloning</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters were substantive and largely critical of Google's rollout consistency: one noted the lack of alignment across consumer, prosumer, and cloud platforms, where even capabilities differ, making the feature unusable for organizations that disable consumer tiers. Others observed that voice cloning is now widely available, so Google is no longer hesitant to ship it, and a developer showcased KeenLore, a locally hosted audiobook web app using Gemma 4 that reports 97.2% quotation-attribution accuracy (485/499 quotes) with no cloud costs.

**Tags**: `#Gemini`, `#text-to-speech`, `#voice cloning`, `#Google AI`, `#Hacker News`

---

<a id="item-8"></a>
## [Radicle discloses unencrypted, unauthenticated node traffic exposing private repos](https://radicle.dev/2026/09/23/disclosure-of-vulnerability-in-network-protocol) ⭐️ 7.0/10

On 2026-09-23 Radicle published a disclosure stating that every version of its peer-to-peer code collaboration protocol released to date sends node-to-node traffic without encryption or authentication, so private repositories can travel the network in cleartext. The flaw was reported by Konstantinos Maninakis on 2026-06-24, and until a security update ships the only advised mitigation is to stop using private repositories over the network. This is a serious blow to a decentralized code-hosting platform whose core value proposition is cryptographic identity and user sovereignty over code, and it directly undermines trust for anyone who hosted private repositories on Radicle. The roughly three-month gap between report and public disclosure, combined with a mitigation that amounts to "stop using the affected feature," also raises broader questions about the project's security engineering and disclosure process. The advisory says all Radicle versions released so far are affected, and while Signed References still authenticate repository contents and can detect objects being modified in transit, they do not stop an attacker positioned on the network path from reading the traffic. No patch was available at the time of disclosure.

hackernews · lostmsu · Sep 23, 15:23 · [Discussion](https://news.ycombinator.com/item?id=49817524)

**Background**: Radicle is a peer-to-peer alternative to centralized forges such as GitHub: each user runs a node identified by a public key, nodes discover each other through a custom gossip protocol, and Git is used to replicate repository data between peers. Because the design is built around cryptographic identities and signed artifacts, users reasonably assumed that transport between nodes was protected as well. When transport is neither encrypted nor authenticated, anyone who can observe the network path — an ISP, a hosting provider, a Wi-Fi operator — can read repository data in transit, which is exactly why comparable systems such as Amazon OpenSearch Service offer TLS for node-to-node traffic.

<details><summary>References</summary>
<ul>
<li><a href="https://radicle.dev/2026/09/23/disclosure-of-vulnerability-in-network-protocol">Disclosure of Vulnerability in the Network Protocol</a></li>
<li><a href="https://maninak.com/blog/radicle-cleartext-transport-vulnerability/">Vulnerability disclosure: Radicle nodes send private ...</a></li>
<li><a href="https://radicle.dev/guides/protocol">Radicle Protocol Guide</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters were largely harsh: several asked how a project built on cryptographic identities could overlook encrypting and authenticating node traffic, and criticized the three-month delay given that the only workaround is to stop using private repos and assume they are compromised. Others said the incident confirms long-standing doubts about the project — its ties to crypto/DAO circles and its curl-pipe-to-shell install — with one calling the whole affair "amateur hour."

**Tags**: `#security`, `#decentralization`, `#vulnerability-disclosure`, `#networking`, `#radicle`

---

<a id="item-9"></a>
## [Complex KDA Extends Kimi Delta Attention's Expressivity to Orthogonal DPLR Matrices](https://www.reddit.com/r/MachineLearning/comments/1wn5uv9/understanding_and_enhancing_kimi_delta_attention_r/) ⭐️ 7.0/10

A new paper, "Complex KDA: Understanding and Enhancing the Expressivity of Kimi Delta Attention" (arXiv 2609.24797, by Julien Siems and 10 co-authors), introduces "Complex KDA" (CKDA), a variant of Kimi Delta Attention that widens the diagonal gate range to [-1, 1] and the delta-rule learning rate to [0, 2]. The authors prove this single-step formulation can express any orthogonal diagonal-plus-rank-one matrix and can track the S3, S4 and A5 groups (but not S5), with experiments showing CKDA learns S3 and S4, gives promising audio-continuation results, and trains stably while staying competitive with standard KDA on language modeling. Linear attention mechanisms such as KDA are central to the push for efficient long-context models that beat full attention, so a result showing that a modest change in gate and learning-rate ranges unlocks richer state transitions — without increasing the rank or cost of the recurrent update — directly informs how expressive these layers can be at equal compute. It also clarifies the theoretical limits of the delta-rule family used in architectures like Kimi Linear and Gated DeltaNet, which matters for anyone designing hybrid linear/full-attention models or evaluating their state-tracking abilities. Prior work showed that modeling a 2D rotation with the delta rule requires composing two transitions in one recurrent update, which raises the rank and the update cost; CKDA instead uses KDA's full diagonal gate as a reflection so that a rotation can be carried out in a single step, at the price of extending the gate range to [-1, 1] and the learning rate to [0, 2]. The key limitation is that the construction provably cannot track S5, so the expressivity gain over orthogonal diagonal-plus-rank-one matrices remains bounded.

reddit · r/MachineLearning · /u/Yossarian_1234 · Sep 22, 10:34

**Background**: Kimi Delta Attention (KDA) was introduced with Kimi Linear, a hybrid linear-attention architecture that interleaves KDA layers with Multi-Head Latent Attention and, under fair comparisons, outperforms full attention while cutting KV-cache usage substantially. KDA itself refines Gated DeltaNet by replacing scalar decay with per-channel (fine-grained diagonal) gating, giving more precise control over a fixed-size recurrent memory. These models belong to the delta-rule linear-attention family, which behaves like a linear-time RNN with a low-rank correction to its memory updates. Group-tracking tasks based on the symmetric groups S3, S4 and S5 are a standard probe for whether a recurrent model can represent non-commutative state composition, which is exactly where diagonal linear updates tend to fall short.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2609.24797">[2609.24797] Complex KDA : Understanding and Enhancing the...</a></li>
<li><a href="https://arxiv.org/abs/2510.26692">[2510.26692] Kimi Linear: An Expressive, Efficient Attention ... KDA (Kimi Delta Attention) | fla-org/flash-linear-attention ... GitHub - hwilner/kimi-delta-attention: Educational ... Linear Attention: Kimi Delta Attention | Jianyu Huang [2609.24797] Complex KDA: Understanding and Enhancing the ... GitHub - MoonshotAI/Kimi-Linear Kimi Delta Attention: Delta‐Rule Linear Mechanism</a></li>
<li><a href="https://arxiv.org/abs/2412.06464">[2412.06464] Gated Delta Networks: Improving Mamba2 with Delta Rule</a></li>

</ul>
</details>

**Tags**: `#attention-mechanisms`, `#linear-attention`, `#deep-learning-theory`, `#expressivity`, `#sequence-modeling`

---

<a id="item-10"></a>
## [Qonto launches QontoFAQ benchmark to curb retrieval benchmaxxing](https://www.reddit.com/r/MachineLearning/comments/1wn9xqk/qontofaq_a_better_information_retrieval_benchmark/) ⭐️ 7.0/10

Qonto introduced QontoFAQ, a new information retrieval benchmark plus an accompanying evaluation metric designed to measure embedding models by how well they surface the document that actually answers a product question. The release includes a Medium article explaining the approach, a public benchmarking dataset, and open-source code on GitHub (qonto/qonto-faq-benchmark). Most popular retrieval benchmarks are static and can be gamed, so models increasingly look strong on leaderboards while failing on real search needs; tying the metric to answer-finding relevance aims to close that gap. Anyone choosing or shipping embedding models for search, RAG, or support-document retrieval — including teams evaluating models on BEIR-style suites — could benefit from a benchmark aligned with an actual user objective. The stated motivation is that existing retrieval benchmarks feel “benchmaxxed,” so Qonto designed a metric intended to scale more proportionally with document relevance and built a dedicated dataset around product FAQ queries. The contribution is narrow by design — it targets one specific retrieval objective (finding the article that answers a product question) rather than general-purpose retrieval, so results are not directly comparable to broad multi-task suites like BEIR.

reddit · r/MachineLearning · /u/espadrine · Sep 22, 13:45

**Background**: Information retrieval systems are typically evaluated with measures such as precision, recall, and nDCG over curated test collections, and embedding models are the component that turns text into vectors so semantically similar documents can be matched. Benchmarks like BEIR popularized cross-domain, zero-shot evaluation of these models, but leaderboard pressure has led to “benchmaxxing” — tuning specifically to score well rather than to help end users. QontoFAQ sits in this lineage, arguing that a benchmark should be defined by the retrieval task's real purpose, in this case answering customer product questions from a knowledge base.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Evaluation_measures_(information_retrieval)">Evaluation measures (information retrieval) - Wikipedia</a></li>
<li><a href="https://zilliz.com/glossary/beir">Benchmarking IR Information Retrieval (BEIR) - Zilliz</a></li>
<li><a href="https://www.pinecone.io/learn/series/rag/embedding-models-rundown/">Choosing an Embedding Model | Pinecone</a></li>

</ul>
</details>

**Tags**: `#Information Retrieval`, `#Benchmark`, `#Embedding Models`, `#Evaluation Metrics`, `#NLP`

---

<a id="item-11"></a>
## [Meta Unveils $1,300 VR Glasses With Narrower Field of View Than Quest 3](https://www.meta.com/vr-glasses/) ⭐️ 6.0/10

Meta announced a new pair of VR glasses priced at $1,300, which feature a field of view of only 70° × 66° — noticeably narrower than the Quest 3's 103° × 96° — and have drawn heavy discussion on Hacker News (166 points, 117 comments). The device was shown alongside a new Beat Saber title and other game logos, though availability details for existing Quest 3 or PCVR users remain unclear. The launch highlights a strategic tension for Meta: the company is charging a premium, flagship-level price while offering a substantially narrower field of view than its cheaper Quest 3, which risks alienating the enthusiast VR community that has driven its ecosystem. It also revives long-running debates about the tradeoffs between headset size, comfort, and immersion, and about whether Meta's mandatory ID verification and data practices are pushing loyal users away. The 70° × 66° field of view is roughly two-thirds of the Quest 3's horizontal coverage, and commenters note that even the Quest 3's 103° × 96° can feel like looking through binoculars; lower FOV generally reduces immersion and can increase discomfort. The $1,300 price point is more than double the $599.99 Quest 3 512GB, and reviewers question whether text rendering is sharp enough for the productivity use cases Meta promotes.

hackernews · polymorph1sm · Sep 23, 23:47 · [Discussion](https://news.ycombinator.com/item?id=49824268)

**Background**: Field of view (FOV) describes how much of the visual world a headset's lenses and displays can present at once, and it is one of the biggest factors in how immersive and comfortable a VR headset feels. Meta's Quest 3, launched in 2023 starting at $499.99 for the 128GB model and $599.99 for 512GB, is a standalone headset running Meta Horizon OS (an Android AOSP derivative) that can run games natively or stream them from a PC over USB-C or Wi-Fi. Meta has also required users to link a Facebook/Meta account and, in some cases, verify identity with a government-issued ID, a policy that has been widely criticized.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Meta_Quest_3">Meta Quest 3 - Wikipedia</a></li>
<li><a href="https://theimmersivetech.com/field-of-view-for-vr-headset/">Field of View for VR Headset: Explained | The Immersive Tech</a></li>

</ul>
</details>

**Discussion**: Commenters were largely skeptical: several long-time Quest owners said the narrower FOV and $1,300 price give them no reason to upgrade, and some argued Meta should stop marketing such devices for productivity given the text clarity limits. A recurring theme was distrust of Meta itself — one user said they would never upload their state-issued ID to keep using their headset, calling the company's practices "unacceptable and user-hostile." Others were puzzled by the apparent pivot away from the transparent AR glasses direction (Ray-Ban Display, Orion) suggested by the imagery.

**Tags**: `#VR/AR`, `#Meta`, `#hardware`, `#privacy`, `#consumer-tech`

---

<a id="item-12"></a>
## [Italy's parliament votes to pave way for return to nuclear energy](https://apnews.com/article/italy-nuclear-chernobyl-4891b6b7c7791ae84db6b0bf0f7cf567) ⭐️ 6.0/10

Italy's parliament voted to create a legal and regulatory framework that would allow the country to produce nuclear power again, with the government focusing on small modular reactors (SMRs) and other advanced technologies rather than the large traditional reactors of the past. The legislation itself does not authorize the construction of any reactor; it only establishes the regulatory foundation that future projects would need before being proposed, assessed and approved. Italy was one of the few European countries to fully abandon nuclear power, so a parliamentary vote to build a regulatory path back is a notable reversal in national energy policy, changing the investment landscape for utilities and SMR vendors. It also feeds into a broader European debate about energy security, decarbonization and the rising electricity demand from data centers and AI, where SMRs are being pitched as an on-site power source. By definition SMRs are reactors rated below roughly 300 MWe that use modular, factory-built designs with passive safety features, intended to cut construction cost and time versus large light-water reactors; the Italian law stops short of naming any design, site or financing plan. A key open question flagged in the legislation's coverage is how reactors would be financed in a grid increasingly dominated by solar power.

hackernews · geox · Sep 23, 17:06 · [Discussion](https://news.ycombinator.com/item?id=49819221)

**Background**: Italy shut down its nuclear plants and voted to abandon nuclear energy in a 1987 referendum held just after the Chernobyl disaster, and a 2011 referendum rejected a planned revival, so the country has since depended heavily on natural gas and electricity imports. Small modular reactors (SMRs) are an emerging class of fission reactors with electrical output typically between about 10 and 300 MWe per module, designed to be built in factories and shipped to sites, with many designs offering passive safety systems that need no external power or human action in an emergency. SMRs have drawn strong interest from technology companies such as Google and Microsoft as a way to power data centers for AI workloads.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Small_modular_reactor">Small modular reactor</a></li>
<li><a href="https://www.iaea.org/newscenter/news/what-are-small-modular-reactors-smrs">What are Small Modular Reactors (SMRs)? | IAEA</a></li>
<li><a href="https://www.eia.gov/todayinenergy/detail.php?id=67584">Small modular reactors and microreactors under development in ...</a></li>

</ul>
</details>

**Discussion**: Commenters were divided: an Italian reader welcomed the move, arguing the 1987 referendum that banned nuclear power was a gut reaction to Chernobyl rather than a reasoned choice, and another called the law a "giant step" for SMRs and hoped for more NATO energy collaboration. The sharpest skepticism came from users who noted that SMR proposals rarely publish honest full-lifecycle cost and decommissioning accounting and may exist to attract investor or government money, and from a commenter who regretted that nuclear debate has become part of the culture wars and doubted that reactors could find financing in a solar-dominated grid.

**Tags**: `#nuclear energy`, `#Italy`, `#SMRs`, `#energy policy`, `#Hacker News`

---

<a id="item-13"></a>
## [Raymond Chen Recounts the History of Windows Scroll Bar Shortcuts](https://devblogs.microsoft.com/oldnewthing/20260922-00/?p=112719/) ⭐️ 6.0/10

In a September 2026 installment of Microsoft's Old New Thing blog, Windows veteran Raymond Chen traced the history and design rationale behind the shortcut behaviors of Win32 scroll bars. The post triggered a wide-ranging Hacker News discussion about how modern frameworks have abandoned those long-standing conventions. Scroll bars are one of the oldest and most universal GUI controls, so the loss of their carefully designed interaction model affects virtually every desktop and web user. The piece highlights a broader trend in which framework authors reinvent common controls with less rigor, quietly eroding cross-application consistency. Chen is a longtime Microsoft engineer whose Old New Thing blog is a canonical source on why Windows behaves the way it does, and his posts typically explain small quirks that trace back to compatibility or design decisions from the 1980s and 1990s. Commenters noted that analogous behaviors still exist elsewhere in inconsistent forms — for example, in GTK clicking the trough jumps to that position, Shift+click pages up or down, and middle-click behavior varies between Firefox and LibreOffice.

hackernews · tybulewicz · Sep 23, 18:02 · [Discussion](https://news.ycombinator.com/item?id=49820065)

**Background**: A Win32 scroll bar traditionally supports several distinct mouse actions: clicking the arrow buttons scrolls one line, clicking the empty trough scrolls one page, and dragging the thumb moves continuously — a scheme invented to give mouse users capabilities that keyboard keys like Page Up and Page Down cannot replicate. Modern software frequently replaces these native controls with custom or CSS-styled scroll bars, which behave differently or drop features entirely. Raymond Chen's Old New Thing is a long-running Microsoft developer blog devoted to Windows history and API archaeology.

<details><summary>References</summary>
<ul>
<li><a href="https://support.microsoft.com/en-us/accessibility/windows/keyboard-shortcuts-in-windows">Keyboard shortcuts in Windows | Microsoft Support</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Scrollbars_styling">CSS scrollbars styling - CSS | MDN</a></li>
<li><a href="https://www.w3schools.com/howto/howto_css_custom_scrollbar.asp">How To Create a Custom Scrollbar</a></li>

</ul>
</details>

**Discussion**: Commenters largely agreed with the article's implicit lament: many argued that custom framework scroll bars are carelessly implemented and behave worse than the Win32 originals, with some missing the era of consistent UX across applications. One widely echoed view was that clicking the trough should jump to that position by default, since Page Up/Page Down already cover paging and no keyboard key can replicate 'scroll here'. Others complained about ultrathin or hidden web scroll bars and shared workarounds such as Firefox's layout.css.scrollbar-width-thin.disabled setting, while one commenter catalogued the inconsistent click, Shift+click and middle-click behaviors across GTK, Firefox, LibreOffice and Inkscape.

**Tags**: `#Windows`, `#UI/UX`, `#scrollbars`, `#software history`, `#HCI`

---

<a id="item-14"></a>
## [llm 0.36 adds GPT-6 Sol and Luna, plus conversation-support plugin flag](https://simonwillison.net/2026/Sep/22/llm/) ⭐️ 6.0/10

llm 0.36, Simon Willison's CLI tool for accessing large language models, adds two new OpenAI model aliases — gpt-6-sol for GPT-6 Sol and gpt-6-luna for GPT-6 Luna — along with bug fixes from five new contributors. The release also lets model plugins declare supports_conversation = False, causing LLM to raise llm.ConversationNotSupported when single-turn-only models receive assistant or tool history, and llm chat to reject them before a session starts. This keeps llm current with OpenAI's newest GPT-6 family tiers, so users can access the cheaper Sol and Luna models without waiting for third-party tooling to catch up. The supports_conversation flag is a small but meaningful extensibility improvement: it lets plugin authors model real-world API limitations explicitly instead of relying on undocumented failures, which matters for classification and scoring plugins like the new llm-typesafe. The new flag is enforced in two places: LLM raises llm.ConversationNotSupported when such a model is given assistant or tool history, and llm chat refuses the model up front. The first plugin to adopt it is llm-typesafe, and the release also wraps reasoning traces in llm logs Markdown output inside <details><summary> tags so long chain-of-thought text can be collapsed.

rss · Simon Willison · Sep 22, 18:48

**Background**: llm is a command-line tool and Python library by Simon Willison for running prompts against models from OpenAI, Anthropic, Google and others, with a plugin system for adding new providers or models. GPT-6 Sol and GPT-6 Luna were released on September 22, 2026 as mid-tier and fast, low-cost members of OpenAI's GPT-6 family, sitting below the flagship GPT-6 Astra. Some models — particularly specialized classifiers and scorers — only accept a single prompt and cannot handle multi-turn conversation history, which previously caused confusing errors when used through chat interfaces.

<details><summary>References</summary>
<ul>
<li><a href="https://openrouter.ai/openai/gpt-6-sol">GPT - 6 Sol - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://openrouter.ai/openai/gpt-6-luna">GPT - 6 Luna - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://pypi.org/project/llm-typesafe/">Use TypeSafe classification and scoring models with LLM</a></li>

</ul>
</details>

**Tags**: `#llm`, `#OpenAI`, `#release`, `#CLI`, `#plugins`

---

<a id="item-15"></a>
## [Templar simulates stage skipping for pipeline-parallel fault tolerance](https://www.reddit.com/r/MachineLearning/comments/1wnd5ys/simulating_fault_tolerance_with_stage_skipping_in/) ⭐️ 6.0/10

Templar published new work on fault tolerance in Crucible, its distributed pre-training platform, simulating a "stage skipping" scheme in which activations and gradients bypass a failed inner pipeline stage for several steps so healthy workers continue processing tokens instead of waiting for recovery. In simulations using a 178M model with eight replicas and four stages per replica, at a 1% per-replica failure probability per global step, validation loss stayed close to the no-failure baseline even though each outage removed a stage for six global steps. If the approach holds up beyond simulation, it could let large-scale pre-training runs tolerate unreliable hardware such as spot instances and transiently failing workers, reducing idle time and cost when a single stage goes down. This matters to ML systems engineers building and operating distributed training infrastructure, where pipeline stalls caused by one failed worker can otherwise waste the throughput of an entire pipeline. The authors are explicit that this is a simulation of the learning effects of stage failures, not a measurement of physical worker replacement or production cost savings, and the results are on a relatively small 178M model. Fixed projections shared across layers further improved robustness when pipeline compression was used, which the authors suggest may align representations across stage boundaries and make bypasses less disruptive — but they note this alignment explanation remains a hypothesis.

reddit · r/MachineLearning · /u/covenant_ai · Sep 22, 15:47

**Background**: Pipeline parallelism splits a model's layers across multiple workers into stages, with each stage passing activations forward and gradients backward to its neighbors, so the loss of any inner stage normally stalls the whole pipeline. Crucible combines data-parallel replicas (each holding a full copy of the model split across stages) with pipeline parallelism, uses SparseLoCo to exchange compressed pseudo-gradient updates between replicas, and applies pipeline compression to cut the communication across stage boundaries. Stage skipping builds on this setup by temporarily rerouting the forward and backward passes around an unavailable stage instead of pausing training.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tplr.ai/publications/blog/skipping-stages-with-fixed-projections">Fault tolerance in low-bandwidth model parallelism: exploring ...</a></li>
<li><a href="https://arxiv.org/html/2508.15706v1">Communication Efficient LLM Pre-training with SparseLoCo</a></li>

</ul>
</details>

**Tags**: `#distributed-training`, `#fault-tolerance`, `#pipeline-parallelism`, `#ml-systems`, `#large-scale-training`

---