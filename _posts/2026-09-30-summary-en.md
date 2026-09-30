---
layout: default
title: "Horizon Summary: 2026-09-30 (EN)"
date: 2026-09-30
lang: en
---

> From 47 items, 13 important content pieces were selected

---

**Technology News**
1. [OpenAI Announces GPT-6.1 Sol With Steep Price Cuts Amid Quality Skepticism](#item-tech-news-1) ⭐️ 8.0/10
2. [New Relapse PS5 exploit appears on GitHub, reportedly using WebKit JavaScriptCore bug](#item-tech-news-2) ⭐️ 7.0/10
3. [Research Paper Examines Privacy and Tracking Risks in Web and Mobile AI Chat Agents](#item-tech-news-3) ⭐️ 7.0/10
4. [OpenAI Announces Dots, an Always-On Agent, Sparking Lock-In Debate](#item-tech-news-4) ⭐️ 7.0/10
5. [Anthropic red team: GLM-5.3 and Claude Mythos Preview achieve full control flow hijacks](#item-tech-news-5) ⭐️ 7.0/10
6. [Free Open-Source Book Teaches ML Performance Engineering from Silicon to Agents](#item-tech-news-6) ⭐️ 7.0/10
7. [Cloudflare launches cf CLI open beta covering 3,000+ API operations for AI agents](#item-tech-news-7) ⭐️ 7.0/10
8. [OpenAI DevDay recap announces Dots agent, GPT-6.1 Sol, and Pro 500 tier](#item-tech-news-8) ⭐️ 7.0/10
9. [Anthropic reportedly assesses Zhipu&\#x27;s GLM-5.3 as capable of autonomous cyberattacks](#item-tech-news-9) ⭐️ 7.0/10

**Financial News**
1. [Trump&\#x27;s Municipal Bond Holdings Reach $300 Million to $1 Billion](#item-finance-news-1) ⭐️ 7.0/10
2. [China reportedly sets tough IPO criteria for humanoid robot startups](#item-finance-news-2) ⭐️ 7.0/10
3. [Oracle Issues Force Majeure Notice as Stargate&\#x27;s New Mexico Data Center Faces Power-Approval Delays](#item-finance-news-3) ⭐️ 7.0/10
4. [China Launches 1-Point Interest Subsidy for First-Home Commercial Mortgages](#item-finance-news-4) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [OpenAI Announces GPT-6.1 Sol With Steep Price Cuts Amid Quality Skepticism](https://openai.com/index/introducing-gpt-6-1-sol/) ⭐️ 8.0/10

OpenAI announced GPT-6.1 Sol on September 29, 2026, positioning it as &quot;near-Astra intelligence for a fifth of the price&quot; — a claimed roughly 5x cost reduction versus its predecessor — with cached input priced at $0.10 per million tokens, which the announcement says is 95% below standard input pricing and 50% below GPT-6 Sol&\#x27;s cached-input rate. These figures and the quality framing are vendor claims from the release page and have not been independently verified. The launch follows GPT-6 Sol, which many developers in the release discussion describe as a marked quality regression that pushed them toward Anthropic&\#x27;s Opus 5.5 or cheaper rivals such as DeepSeek, so community attention centers on whether 6.1 fixes quality rather than price.

hackernews · crorella · Sep 29, 17:06 · [Discussion](https://news.ycombinator.com/item?id=49896586)

**「A week after a rocky GPT-6 Sol launch」** GPT-6.1 Sol arrives barely a week after its predecessor GPT-6 Sol, a version that developers in the announcement thread describe as a sharp regression from Sol 5.6, with several long-time OpenAI users reporting they had switched to Anthropic&\#x27;s Opus 5.5 for coding work. Commenters read the unusually quick follow-up, which OpenAI pitches as Astra-level intelligence at one-fifth the price, as a response both to that reception and to much cheaper rivals such as DeepSeek.

**「Impact」** Developers running cache-heavy API workloads stand to see the most direct effect: OpenAI&\#x27;s announced $0.10 per million cached-input tokens, presented as 50% below the prior GPT-6 Sol cached rate, would substantially lower the cost of agentic coding sessions such as Codex — though these are vendor claims not yet independently verified. Given reported quality regressions in Sol 6 and cheaper flagship alternatives already on the market \(DeepSeek&\#x27;s flagship at $0.28 per million input tokens, with its V4.1 Flash at $0.15\), teams with price-sensitive workloads should benchmark GPT 6.1 Sol&\#x27;s actual output quality against both the previous version and cheaper rivals before migrating.

**「Community reaction」** Commenters split on what matters most: minimaxir calls the halved cached-input price &quot;the actual big announcement&quot; because 50% cheaper cache &quot;will get you far more mileage on Codex,&quot; while the\_duke reports dropping OpenAI models for Opus 5.5 after calling Sol 6 a huge regression versus Sol 5.6, and proxysna argues DeepSeek&\#x27;s speed and price make frontier-tier subscriptions hard to justify. Revolvingthrow&\#x27;s theory that Sol 6.1 is a last-minute rename of &quot;Astra-Minor&quot; found in leaked files is speculation, not a confirmed fact.

<details><summary>References</summary>
<ul>
<li><a href="https://officechai.com/ai/gpt-6-1-sol/">OpenAI Announces GPT 6.1 Sol, Says It Has Astra-level Intelligence At 1/5th The Price</a></li>
<li><a href="https://www.aipricing.guru/anthropic-pricing/">Claude API Pricing 2026: Opus 5.5, Fable, Sonnet</a></li>
<li><a href="https://www.aipricing.guru/">AI API Pricing 2026: Compare GPT, Claude, Gemini Token Costs</a></li>

</ul>
</details>

**Tags**: `#openai`, `#large-language-models`, `#ai-pricing`, `#model-releases`, `#ai-industry`

---

<a id="item-tech-news-2"></a>
### [New Relapse PS5 exploit appears on GitHub, reportedly using WebKit JavaScriptCore bug](https://github.com/ntfargo/Relapse-Exploit) ⭐️ 7.0/10

A new PlayStation 5 exploit named Relapse was published on GitHub at ntfargo/Relapse-Exploit on September 29, 2026, and quickly drew attention on Hacker News, where the submission collected 235 points and 129 comments. The analysis accompanying the item says the exploit apparently leverages a WebKit JavaScriptCore bug, and discussion centers on its potential to enable homebrew and user freedoms such as backing up save games. The available material does not state the affected firmware versions, the confirmed exploit chain, or verified capabilities, so what the exploit actually enables on a given console remains unconfirmed.

hackernews · therepanic · Sep 29, 15:44 · [Discussion](https://news.ycombinator.com/item?id=49895304)

**「Firmware windows and the exploit chain」** PS5 jailbreak methods have historically been tightly bound to firmware versions, since Sony patches the underlying bugs in system updates, and earlier exploits each covered narrow update branches that required separate projects. According to the Relapse repository&\#x27;s own description, the project chains a WebKit memory-leak bug with a use-after-free race in the kernel&\#x27;s aio\_multi\_wait call to execute unsigned code on firmware 7.00 through 13.60, on both the PS5 and the PS5 Pro.

**「Impact」** PS5 owners on firmware 7.00 through 13.60 face an immediate update decision: the Relapse README claims its browser stage — JavaScriptCore information leaks combined with a structured-clone object-pool mismatch that corrupts a typed array — works across that entire range, so users who want to preserve access to the exploit need to stay on firmware 13.60 or lower, while anyone who has already updated further falls outside the claimed window. The claims come from the repository&\#x27;s README rather than independent verification, and Sony has a record of hardening the platform \(the PS5 developer wiki notes non-AF\_UNIX socket creation was disabled in PS4 games from System Software 8.00, bypassable only where native JIT is available\), so the exploit&\#x27;s practical reach should be treated as provisional until independently confirmed.

**「Community discussion」** Commenters focused on practical outcomes and open technical questions: one user — who lost a year of Minecraft saves to data corruption — asked whether the exploit would allow backing up game saves to USB, noting that the PS5 restricts this behind a PS Plus cloud subscription per profile, while another asked whether the PS5&\#x27;s WebKit runs JavaScriptCore with the JIT enabled and suggested Sony could disable the JIT to narrow the attack surface. Other remarks were speculative, with one commenter arguing that console jailbreak communities typically hold additional undisclosed vulnerabilities, and others musing about running Steam PC games on the console.

<details><summary>References</summary>
<ul>
<li><a href="https://elsolitario.org/en/2026/09/29/relapse-repo-claims-ps5-exploit-firmware-7-00-to-13-60/">PS5 Jailbreak: What Is Relapse Exploit and Its Scope</a></li>
<li><a href="https://gagadget.com/en/728014-new-ps5-jailbreak-relapse-works-on-firmware-up-to-1360/">New PS5 jailbreak Relapse works on firmware up to 13.60</a></li>
<li><a href="https://dev.to/lu1tr0n/relapse-repo-afirma-exploit-de-ps5-en-firmware-700-1360-1n14">Relapse: repo afirma exploit de PS5 en firmware 7.00-13.60 - DEV Community</a></li>
<li><a href="https://dev.to/lu1tr0n/relapse-repo-afirma-exploit-de-ps5-en-firmware-700-1360-1n14">Relapse: repo afirma exploit de PS5 en firmware 7.00-13.60 - DEV Community</a></li>
<li><a href="https://elsolitario.org/en/2026/09/29/relapse-repo-claims-ps5-exploit-firmware-7-00-to-13-60/">PS5 Jailbreak: What Is Relapse Exploit and Its Scope</a></li>
<li><a href="https://www.psdevwiki.com/ps5/Vulnerabilities">Vulnerabilities - PS5 Developer wiki</a></li>

</ul>
</details>

**Tags**: `#security`, `#exploits`, `#webkit`, `#console-hacking`, `#playstation`

---

<a id="item-tech-news-3"></a>
### [Research Paper Examines Privacy and Tracking Risks in Web and Mobile AI Chat Agents](https://jorgegarciaherrero.com/wp-content/interactivos/20260916-Prompt-like-a-butterfly-sting-like-a-tracker-%28clean%29.pdf) ⭐️ 7.0/10

A research paper analyzing privacy and tracking risks in web and mobile conversational AI agents was shared on Hacker News on September 29, 2026, where it drew 408 points and 130 comments. The paper is distributed as a PDF hosted on jorgegarciaherrero.com under the file name &\#x27;Prompt Like a Butterfly, Sting Like a Tracker,&\#x27; and examines how AI chat services may expose user prompts and conversations. The shared item covers the paper&\#x27;s topic and community reception rather than its full findings, so the specific measurements and conclusions are not confirmed from the source alone.

hackernews · damaru2 · Sep 29, 09:03 · [Discussion](https://news.ycombinator.com/item?id=49890226)

**「Web tracking measurement meets AI chat clients」** Consumer AI chat assistants run as ordinary web and mobile clients, so they inherit the web&\#x27;s familiar tracking surface: page loads can pull assets such as third-party-hosted fonts, and every prompt travels to the vendor&\#x27;s servers. The paper &quot;Prompt like a Butterfly, Sting like a Tracker&quot; brings standard traffic measurement to this newer category, quantifying the third-party data flows of conversational AI web and mobile clients, whose agents now also handle voice, images, documents, and browsing, broadening what those flows can expose. The work complements rather than repeats recent AI-agent security research, such as Palo Alto Networks Unit42&\#x27;s March 2026 report on web-based indirect prompt injection observed in the wild, which examined attacks on agent behavior instead of passive data collection.

**「Impact」** The discussion points to a practical exposure channel for users of AI chat services: conversation links that appear to be opaque identifiers but can reveal full transcripts. As one commenter reports, visiting a past Perplexity search URL exposes the entire conversation, so users should treat shared chat links as public and consider what their chat client transmits before a prompt is even submitted.

**「Community Discussion」** Commenter pbasista reported that ChatGPT&\#x27;s web client periodically sends unfinished prompts to a \`conversation/prepare\` endpoint before the user submits anything, speculating the fragments could be used to pre-warm caches or to profile typing cadence, error-correction habits, and how raw ideas evolve; postalcoder criticized services that equate a UUID in the URL with privacy, reporting that Perplexity conversation links expose the full exchange. Another commenter, kdaniel\_03, framed both telemetry and training as the same failure of private prompts leaving user control, citing a recent dispute in which OpenAI said no one saw unpublished drafts in private Codex sessions but acknowledged de-identified product data may have improved its models, and argued this makes open models the necessary alternative; these are individual observations and arguments rather than verified findings from the paper.

<details><summary>References</summary>
<ul>
<li><a href="https://jorgegarciaherrero.com/wp-content/interactivos/20260916-Prompt-like-a-butterfly-sting-like-a-tracker-%28clean%29.pdf">Prompt like a Butterfly, Sting like a Tracker: A Privacy Analysis of</a></li>
<li><a href="https://github.com/turnstonelabs/turnstone/issues/1229">Web UIs fetch their fonts from a third-party host on every page load · Issue #1229 · turnstonelabs/turnstone</a></li>
<li><a href="https://unit42.paloaltonetworks.com/ai-agent-prompt-injection/">Fooling AI Agents: Web-Based Indirect Prompt Injection Observed in the Wild</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#conversational AI`, `#AI agents`, `#tracking`, `#security`

---

<a id="item-tech-news-4"></a>
### [OpenAI Announces Dots, an Always-On Agent, Sparking Lock-In Debate](https://openai.com/index/introducing-dots/) ⭐️ 7.0/10

OpenAI announced Dots, an always-on agent product, in a post on its website dated September 29, 2026. The announcement text itself was not included in the available source material, so no capabilities, pricing, availability, or compatibility details for Dots can be confirmed; it stands as an announced product rather than an independently verified capability. The launch drew a large Hacker News response \(466 points, 353 comments\), where discussion centered on what always-on agents imply for the industry rather than on documented features.

hackernews · alvis · Sep 29, 17:07 · [Discussion](https://news.ycombinator.com/item?id=49896604)

**「What an &quot;always-on&quot; agent is」** Always-on agents depart from the chat-first format OpenAI built its name on: rather than waiting for prompts, they are designed to run continuously in the background, investigating, building, and acting on a user&\#x27;s behalf across connected services, with OpenAI claiming Dots can operate across 4,000 apps. OpenAI unveiled Dots at its DevDay 2026 keynote alongside a batch of other new features, and the agents are initially rolling out to eligible ChatGPT Pro and Business Premium subscribers.

**「Limited rollout and lock-in trade-offs」** Access is initially narrow: Dots will first be limited to paid enterprise plans, including Pro and Business Premium, so users on free or lower-tier plans cannot try the agents yet. Commenters also warn that always-on agents accumulate integrations and work history in the vendor&\#x27;s cloud, making switching harder than swapping standalone models, so teams adopting Dots may want to weigh data portability before building workflows on it.

**「Community reaction」** Commenters argued that always-on agents deepen platform lock-in because integrations and accumulated work history make them harder to swap than raw models, with aditya\_rs suggesting closed-model vendors want an abstraction layer over the model itself, and johnfahey predicting OpenAI will tighten the generous Codex limits that attracted users, a pattern he says Anthropic followed with Claude. Others expressed skepticism about product overlap: wxw found the lines between Codex, ChatGPT Work, and Dots increasingly blurry and said he favored Meta&\#x27;s Muse as a consumer play, while jameslk argued that cloud-hosted agents running on virtual machines target non-technical users and could mark the end of the PC era. These are commenters&\#x27; opinions and speculations, not verified facts about Dots.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/introducing-dots/">Introducing dots - OpenAI</a></li>
<li><a href="https://www.digitaltrends.com/computing/openais-dots-push-ai-beyond-chatbots-with-always-on-agents-that-can-investigate-build-and-act-across-4000-apps/">OpenAI&#x27;s Dots are always-on agents that can investigate ...</a></li>
<li><a href="https://runtimewire.com/article/openai-launches-dots-always-on-agents">OpenAI launches Dots, always-on agents that work across ...</a></li>
<li><a href="https://www.pcmag.com/news/openai-goes-after-metas-muse-with-always-on-dots-agents">OpenAI Goes After Meta&#x27;s Muse With Always-On Dots Agents</a></li>

</ul>
</details>

**Tags**: `#openai`, `#ai-agents`, `#always-on-agents`, `#platform-lock-in`, `#product-announcement`

---

<a id="item-tech-news-5"></a>
### [Anthropic red team: GLM-5.3 and Claude Mythos Preview achieve full control flow hijacks](https://simonwillison.net/2026/Sep/29/anthropic-frontier-red-team/) ⭐️ 7.0/10

Simon Willison quotes Anthropic&\#x27;s Frontier Red Team research, which reports that on 100 randomly selected tasks from an internal Binary Exploitation benchmark, GLM-5.3 produced full control flow hijacks — exploits that redirect a compiled program&\#x27;s execution — in 4% of trials, while Claude Mythos Preview did so in 6%. Anthropic characterizes this as a meaningful threshold being crossed, noting that earlier models such as Claude Opus 4.6 and GLM-5.2 did not succeed on any of these tasks. The figures come from the lab&\#x27;s own evaluation, relayed through Willison&\#x27;s quote-only post titled &quot;GLM-5.3 and the spread of advanced cyber capabilities&quot;; no independent replication is cited.

rss · Simon Willison · Sep 29, 22:20

**「Background」** Binary exploitation tests whether a model can find and weaponize vulnerabilities in compiled software, and a &\#x27;full control flow hijack&\#x27; — redirecting a program&\#x27;s execution — is a stronger outcome than a crash or partial exploit. GLM-5.3 is Z.ai&\#x27;s latest flagship model, built on the same base model as GLM-5.2 with its gains driven entirely by post-training, which makes the contrast with its immediate predecessor direct. In related evaluation, CAISI found GLM-5.3 to be the most cyber-capable open-weight model released to date, lagging the US frontier by about four months on an aggregate of its cyber benchmarks — a finding Anthropic says broadly matches its own capability results.

**「Security teams should factor in autonomous exploit capability」** Organizations assessing AI cyber risk may need to treat autonomous exploit development as a present capability rather than a future one: Anthropic&\#x27;s report measures GLM-5.3 producing end-to-end exploits in 50 of 410 attempts \(about 12%\) and Claude Mythos Preview in 56 of 410 \(about 14%\) on ExploitBench, alongside the full control flow hijack results on binary exploitation tasks. Teams operating AI cyber capability thresholds, such as responsible scaling policies or deployment gating, should review whether safeguards calibrated when no model could complete exploits unaided still hold for these models. Since the figures come from Anthropic&\#x27;s own internal benchmarks rather than independent testing, organizations weighing policy changes may want external replication first.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/research/glm-5-3-and-the-spread-of-advanced-cyber-capabilities">GLM - 5 . 3 and the spread of advanced cyber capabilities \ Anthropic</a></li>
<li><a href="https://docs.z.ai/guides/llm/glm-5.3">GLM - 5 . 3 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>
<li><a href="https://www.anthropic.com/research/glm-5-3-and-the-spread-of-advanced-cyber-capabilities">GLM-5.3 and the spread of advanced cyber capabilities \ Anthropic</a></li>
<li><a href="https://ai-tldr.dev/releases/anthropic-glm-5-3-cyber-report/">Anthropic tests GLM-5.3 — its safeguards fall to… | AI/TLDR</a></li>

</ul>
</details>

**Tags**: `#ai-security`, `#llm`, `#cybersecurity`, `#ai-safety`, `#anthropic`

---

<a id="item-tech-news-6"></a>
### [Free Open-Source Book Teaches ML Performance Engineering from Silicon to Agents](https://www.reddit.com/r/MachineLearning/comments/1wt6ns4/i_wrote_a_free_opensource_book_on_making_ml/) ⭐️ 7.0/10

ML practitioner /u/SoloTiger\_ has released &\#x27;How to Make Your Model Fast: A Systems View of Efficient Machine Learning, from Silicon to Agents,&\#x27; a free, open-source book hosted on GitHub \(usamahz/make-your-model-fast\). The book teaches performance engineering as systems-level reasoning, starting with roofline analysis and hardware before working through kernels, compilers, quantisation, pruning, vision, on-device LLMs, robotics, profiling, serving, and agent systems. Its central argument is that reducing FLOPs does not necessarily make a model faster; instead, readers learn to judge whether a workload is compute-, bandwidth-, memory-, or system-bound and which optimisation actually moves that limit. The description comes from the author&\#x27;s self-promotional post, so the book&\#x27;s depth, accuracy, and completeness have not been independently verified, and the author is soliciting feedback and contributions from the ML systems community.

reddit · r/MachineLearning · /u/SoloTiger\_ · Sep 29, 10:35

**「Background」** The book&\#x27;s starting point is roofline analysis, a long-standing performance-engineering technique that classifies a workload as limited by compute throughput or by memory bandwidth — the distinction behind the author&\#x27;s claim that cutting FLOPs through quantization or pruning does not automatically translate into lower latency. The linked repository is hosted under the GitHub account of Usamah Zaheer, whose profile identifies him as an ML engineer at Arm, giving this self-published post a named author with a professional ML-systems background.

**「Free access — and an open call for contributions」** ML and inference engineers now have no-cost access to a decision framework for determining whether a workload is compute-, bandwidth-, memory-, or system-bound before investing in optimizations like quantization, pruning, or kernel work — the diagnostic step the author argues is skipped when teams reduce FLOPs and see no corresponding speedup. Because the book is hosted openly at github.com/usamahz/make-your-model-fast, readers can evaluate its accuracy and depth directly, and the author is actively soliciting feedback and contributions from practitioners in ML systems, inference, compilers, and edge AI.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/usamahz/usamahz.github.io">GitHub - usamahz/usamahz.github.io</a></li>
<li><a href="https://github.com/usamahz">usamahz (Usamah) · GitHub</a></li>

</ul>
</details>

**Tags**: `#ML performance engineering`, `#roofline analysis`, `#quantization`, `#systems optimization`, `#open-source book`

---

<a id="item-tech-news-7"></a>
### [Cloudflare launches cf CLI open beta covering 3,000+ API operations for AI agents](https://blog.cloudflare.com/cloudflare-cf-cli-launch/) ⭐️ 7.0/10

Cloudflare has released cf, a new command-line tool in open beta, giving developers and AI agents a single interface to more than 3,000 Cloudflare API operations spanning Workers, WAF, Access, domains, and other platform services. Unlike the existing Wrangler CLI, which covers roughly 280 operations, cf is generated from Cloudflare&\#x27;s API schemas, so its coverage extends across the company&\#x27;s full stack rather than a single product. The tool outputs JSON by default and supports command search and guidance, letting agents discover operations, execute them, and parse results programmatically. Cloudflare says a single agent could use cf to create and deploy a Worker, monitor the service, configure Access and WAF settings, and even purchase a domain.

telegram · zaihuapd · Sep 29, 13:46

**「Wrangler&\#x27;s coverage gap」** Wrangler, the CLI Cloudflare developers have used to build and deploy Workers, was designed around that developer platform rather than the company&\#x27;s full API surface, exposing roughly 280 command paths with TOML/JSONC configuration files. Services outside the Workers ecosystem, such as WAF, Access, and domain management, therefore had to be handled through the web dashboard or direct REST API calls, leaving no unified command-line interface for scripts or AI agents to automate the whole stack.

**「Impact」** Teams using AI agents to operate Cloudflare infrastructure can now drive the full product surface — creating and deploying Workers, configuring Access and WAF, monitoring services, and purchasing domains — through a single tool, instead of combining Wrangler&\#x27;s roughly 280 Workers-focused operations with hand-written API calls. Its JSON-default output and built-in command discovery reduce the parsing and lookup work agents must perform, but as an open-beta, single-vendor tool it should be piloted alongside existing Wrangler- and API-based workflows before teams make it their primary automation path.

<details><summary>References</summary>
<ul>
<li><a href="https://creuto.com/cloudflare-cf-cli-3000-api-operations-agents">Cloudflare cf CLI: 3,000 API operations built for agents</a></li>
<li><a href="https://daily.dev/posts/introducing-cf-the-agentic-cli-for-the-entire-cloudflare-api-2x4miixan">Introducing cf: the agentic CLI for the entire Cloudflare API</a></li>

</ul>
</details>

**Tags**: `#cloudflare`, `#cli`, `#ai-agents`, `#developer-tools`, `#infrastructure`

---

<a id="item-tech-news-8"></a>
### [OpenAI DevDay recap announces Dots agent, GPT-6.1 Sol, and Pro 500 tier](https://openai.com/zh-Hant/index/devday-2026-recap/) ⭐️ 7.0/10

OpenAI&\#x27;s DevDay recap, as relayed in a Telegram digest, announces more than twenty updates, headlined by &\#x27;Dots&\#x27;, a persistent companion agent that runs autonomously around the clock, learns user habits, and proactively takes over long-running complex tasks. On models, GPT-6.1 Sol specializes in coding and computer control with claimed near-Astra intelligence at one-fifth of the price, while Astra Ultrafast is advertised as up to 8x faster \(6x via the API\). Developer-facing items include Codex moving to the cloud with voice control and automatic fault repair, an Agents API with native computer control and AWS Bedrock hosting, a Luna-based Decisions API for lightweight real-time classification, routing, and agent-action decisions over preset finite options from text or image input, and &\#x27;Sign in with ChatGPT&\#x27;, which lets users route subscription quota to third-party tools such as Devin and Notion. OpenAI also introduced a Pro 500 subscription tier with 25 times Plus&\#x27;s compute quota and exclusive access to Astra Ultrafast; these figures are vendor claims presented in the recap, which the second-hand digest relays without independent verification or stated availability dates.

telegram · zaihuapd · Sep 29, 17:52

**「Background」** OpenAI&\#x27;s GPT-6 generation is already tiered by capability: GPT-6 Astra is the flagship model, GPT-6 Sol is the coding- and computer-use-focused model, and GPT-6 Luna is the lighter-weight option. GPT-6.1 Sol is a direct upgrade to GPT-6 Sol, and OpenAI&\#x27;s published figures illustrate the gap it narrows: it fails to disclose a problem in 2.1% of cases, compared with 4.9% for GPT-6 Sol, 1.5% for GPT-6 Astra, and 28.7% for GPT-6 Luna. The updates landed at DevDay, OpenAI&\#x27;s annual developer conference, with GPT-6.1 Sol available starting September 29, 2026 to Plus, Pro, Business, Enterprise, and Edu users in ChatGPT Work and Codex, and to developers through the API as gpt-6.1-sol.

**「Impact」** Access to the fastest new capabilities is gated behind the new tier: Astra Ultrafast \(up to 8x standard Astra speed\) is exclusive to Pro 500, which third-party coverage prices at $500/month versus the existing $200 Pro plan, and the Decisions API reaches Codex and ChatGPT Work only on Pro 500 and Enterprise. Developers and teams on Plus or the $200 plan therefore cannot get Ultrafast performance or in-product Decisions support without upgrading or calling the API directly, so buyers should compare their current subscription or API spend against Pro 500&\#x27;s quotas before renewing. On Hacker News, commenters read the packaging as OpenAI narrowing the price gap between subscriptions and API usage — a reader interpretation rather than a confirmed pricing change — which, if borne out, would push heavy API users toward bundled plans.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/devday-2026-recap/">DevDay 2026 Recap | OpenAI</a></li>
<li><a href="https://openai.com/index/introducing-gpt-6-1-sol/">Introducing GPT-6.1 Sol | OpenAI</a></li>
<li><a href="https://www.unite.ai/openai-unveils-gpt-6-1-sol-at-devday-with-new-codex-and-chatgpt-tools/">OpenAI Unveils GPT-6.1 Sol at DevDay With New Codex and ChatGPT Tools – Unite.AI</a></li>
<li><a href="https://kingy.ai/blog/chatgpt-pro-500/">ChatGPT Pro 500: Features, Limits &amp; $200 Plan Comparison</a></li>
<li><a href="https://openai.com/index/devday-2026-recap/">DevDay 2026 Recap - OpenAI</a></li>
<li><a href="https://news.ycombinator.com/item?id=49896975">ChatGPT Pro 500 - Hacker News</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#AI agents`, `#large language models`, `#developer APIs`, `#industry news`

---

<a id="item-tech-news-9"></a>
### [Anthropic reportedly assesses Zhipu&\#x27;s GLM-5.3 as capable of autonomous cyberattacks](https://www.anthropic.com/research/glm-5-3-and-the-spread-of-advanced-cyber-capabilities) ⭐️ 7.0/10

According to a summary of Anthropic&\#x27;s research posted on Telegram, Anthropic assessed Zhipu AI&\#x27;s \(Z.ai\) GLM-5.3 as capable of autonomously carrying out end-to-end cyberattacks, succeeding on 50 of 410 ExploitBench attempts — close to the 56 recorded for Claude Mythos Preview. The same report says GLM-5.3&\#x27;s safeguards were bypassed by simple methods in simulated tests with success rates of 64% to 100%, and that the model&\#x27;s open weights allow users to modify it to weaken refusals. Anthropic reportedly concluded that this combination would expand the cyberattack capabilities available to malicious actors. The model names and figures come from the channel&\#x27;s summary rather than the primary publication, so they could not be independently verified from the supplied evidence.

telegram · zaihuapd · Sep 29, 23:58

**「Background」** GLM-5.3 is an open-weights model from Z.ai \(Zhipu AI\) that the company promoted in mid-August 2026 as a cybersecurity-capable release, claiming it edged past Anthropic&\#x27;s Mythos 5 at finding software flaws on the CyberGym benchmark while trailing badly on exploit generation. Z.ai&\#x27;s reported figures at the time showed CyberGym improving from 77.2% to 84.5% and ExploitBench from 24.4% to 54.4%. Those vendor-sourced capability claims, combined with the model&\#x27;s openly available weights, form the backdrop for Anthropic now publishing its own assessment of the model&\#x27;s offensive cyber potential.

**「Open-weight release puts assessed cyber capability in anyone&\#x27;s hands」** Because Z.ai publicly released GLM-5.3&\#x27;s weights two weeks after the model&\#x27;s August 14, 2026 launch, the assessed attack capability is a downloadable, modifiable artifact rather than a capability confined behind a controlled API — and Z.ai had itself acknowledged that safeguards become hard to enforce after download. Organizations deploying open-weight models locally cannot treat provider-side refusals as a security control, and defenders have concrete grounds to act on Anthropic&\#x27;s warning that such releases expand the offensive cyber capabilities available to malicious actors.

<details><summary>References</summary>
<ul>
<li><a href="https://www.technology.org/2026/08/17/zai-glm-5-3-cybergym-mythos-5-benchmarks/">Z.ai GLM-5.3 Nears Mythos 5 on Bug Hunting - Technology Org</a></li>
<li><a href="https://www.linkedin.com/posts/souravmishra83_zai-advanced-ai-chatbot-agent-powered-activity-7494000777359892480-zsSG">GLM-5.3 Boosts Cybersecurity Capabilities | Sourav Mishra posted on the topic | LinkedIn</a></li>
<li><a href="https://www.nist.gov/news-events/news/2026/09/caisis-assessment-zais-glm-53-cyber-capabilities">CAISI’s Assessment of Z.ai’s GLM-5.3 Cyber Capabilities | NIST</a></li>
<li><a href="https://www.facebook.com/61581151543501/posts/chinese-ai-company-zai-has-revealed-glm-53-a-coding-model-with-advanced-cybersec/122141535015038384/">Z.ai delays GLM-5.3 model release for cybersecurity testing</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#cybersecurity`, `#frontier model evaluation`, `#open weights`, `#GLM`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Trump&\#x27;s Municipal Bond Holdings Reach $300 Million to $1 Billion](https://www.cnbc.com/2026/09/29/trump-municipal-bond-portfolio.html) ⭐️ 7.0/10

A CNBC analysis of President Trump&\#x27;s financial disclosures found he holds more than 1,000 municipal bond positions worth $300 million to $1 billion, including debt from issuers affected by his own administration&\#x27;s policies. CNBC found no evidence of trading on advance knowledge of government decisions, and the White House says outside managers independently control the portfolio.

rss · CNBC Finance · Sep 29, 14:37

**「Background」** Municipal bonds are loans to public borrowers such as cities, hospitals, schools and utilities, and ethics experts note that presidents — unlike other federal officials — are exempt from conflict-of-interest laws restricting such holdings.

**「Impact」** Because the president is a creditor to hundreds of public institutions, federal decisions touching those borrowers — such as pollution-rule exemptions for coal plants and projected cuts of roughly $900 billion to Medicaid over a decade — now face heightened conflict-of-interest scrutiny.

**Tags**: `#municipal bonds`, `#conflict of interest`, `#financial disclosures`, `#regulatory policy`, `#Trump`

---

<a id="item-finance-news-2"></a>
### [China reportedly sets tough IPO criteria for humanoid robot startups](https://www.cnbc.com/2026/09/29/china-criteria-humanoid-robot-ipos.html) ⭐️ 7.0/10

China&\#x27;s securities regulator has issued unconfirmed &quot;window guidance,&quot; according to three anonymous sources cited by CNBC, requiring humanoid robot startups seeking IPOs to show sustainable revenue and commercial orders, narrowing losses over what one source said is a three-year forecast, and core technology such as a robotic brain or hands — criteria that few, if any, of the country&\#x27;s 100-plus humanoid companies may meet. The reported crackdown comes as sector bellwether Unitree&\#x27;s Shanghai-listed shares have nearly halved from their 845 yuan debut close to 459.65 yuan, Hong Kong-listed Ubtech reported a 279 million yuan first-half operating loss, and quarterly investment in the sector surged to 47.09 billion yuan \($6.95 billion\) in Q2.

rss · CNBC Finance · Sep 29, 07:19

**「Background」** China has well over 100 humanoid robot firms under Beijing&\#x27;s national &\#x27;embodied AI&\#x27; push, and investment in the sector surged to 47.09 billion yuan \($6.95 billion\) in the second quarter — more than double the first quarter — even as authorities have warned of a bubble. Mainland Chinese companies seeking to list in Hong Kong, where at least two dozen humanoid-related firms have filed, also need the CSRC&\#x27;s approval.

**「Impact」** If enforced as reported, the criteria would delay or block listing plans for the two dozen-plus humanoid startups already filed in Hong Kong and the sector&\#x27;s 100-plus companies, cutting off the IPO exits that private and government-backed investors had been counting on — a tightening that follows Unitree&\#x27;s volatile Shanghai debut.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/09/29/china-criteria-humanoid-robot-ipos.html">China &#x27;s criteria for humanoid robot IPOs may be hard to meet</a></li>
<li><a href="https://robottoday.com/article/unitree-s-ipo-review-what-it-means-for-china-s-humanoid-robot-ipo-landscape">Unitree&#x27;s IPO Review: What It Means for China&#x27;s Humanoid ... Unitree IPO Cleared, AGIBOT Hits 10,000 Units: China Humanoid ... Unitree IPO Resets China Robot Valuations in 2026 China curbs humanoid IPOs after Unitree’s volatile debut, The ... Unitree’s IPO Will Set The First Public Robot ... - Forbes Unitree Clears $618M STAR Market IPO as China&#x27;s Humanoid ...</a></li>

</ul>
</details>

**Tags**: `#China regulation`, `#humanoid robots`, `#IPO market`, `#embodied AI`, `#sector bubble`

---

<a id="item-finance-news-3"></a>
### [Oracle Issues Force Majeure Notice as Stargate&\#x27;s New Mexico Data Center Faces Power-Approval Delays](https://www.bloomberg.com/news/articles/2026-09-24/oracle-cites-force-majeure-to-shield-itself-on-controversial-data-center) ⭐️ 7.0/10

Oracle has sent a force majeure notice to the developer of the Stargate project&\#x27;s Project Jupiter data center in New Mexico, saying that still-pending environmental and power approvals for its 2.45-gigawatt microgrid put the planned 2028 start-up at risk — a legal step that could let Oracle postpone some payments if outside factors cause the delay. The $18 billion syndicated loan tied to the project has traded at a discount, reflecting market concern about construction timelines and financing for large AI data centers.

telegram · zaihuapd · Sep 29, 05:46

**「Background」** Stargate is a program of large AI data centers, most of which are still in construction, permitting, or power-infrastructure stages, with only a few campuses—such as Abilene, Texas—already operating. &quot;Force majeure&quot; is a standard contract clause that lets a party suspend obligations, such as payments, when events beyond its control—here, the delayed permits—prevent a project from proceeding on schedule.

**「What it means for lenders」** Banks holding the roughly $18 billion of loans tied to the New Mexico project are quoting the debt at 89–91 cents on the dollar, meaning lenders and investors financing AI data centers face mark-downs and tighter credit when power-approval delays threaten completion timelines.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/09/24/oracle-sends-force-majeure-notice-on-its-new-mexico-stargate-data-center/">Oracle sends force majeure notice on its New Mexico Stargate ...</a></li>
<li><a href="https://www.cnbc.com/2026/09/24/oracle-data-center-force-majeure.html">Oracle sends &#x27;force majeure&#x27; notice about data center project ...</a></li>
<li><a href="https://www.reuters.com/business/finance/oracles-18-billion-data-center-debt-under-pressure-ft-reports-2026-09-18/">Oracle&#x27;s $18 billion data center debt under pressure, FT ...</a></li>
<li><a href="https://www.tradingkey.com/analysis/stocks/us-stocks/262176714-oracle-stock-forecast-18b-data-center-loan-trades-tradingkey">Oracle Stock Price Forecast: $18 Billion Data Center Loan ...</a></li>

</ul>
</details>

**Tags**: `#AI基础设施`, `#甲骨文`, `#星际之门`, `#银团贷款`, `#电力审批`

---

<a id="item-finance-news-4"></a>
### [China Launches 1-Point Interest Subsidy for First-Home Commercial Mortgages](https://jrs.mof.gov.cn/zhengcefabu/phjr/202609/t20260929_3998312.htm) ⭐️ 7.0/10

China&\#x27;s finance ministry, central bank, and banking regulator on September 29 jointly announced a nationwide subsidy on new commercial first-home mortgages: the central government covers 1 percentage point of annual interest for up to 5 years, on loans capped at 1 million yuan—about 10,000 yuan per household per year at most. The policy takes effect October 1, 2026 and is initially set to run for one year.

telegram · zaihuapd · Sep 29, 10:18

**「Background」** An interest subsidy works differently from a bank cutting rates: the government pays part of the borrower&\#x27;s interest out of fiscal funds, so a first-home buyer&\#x27;s effective borrowing cost falls while the lender keeps charging its normal commercial mortgage rate. The joint notice frames the measure as support for essential, non-investment housing demand—so-called &quot;rigid demand&quot;—by easing the interest burden on families buying their first home.

**「Impact」** Households taking out new commercial loans for a first home of 120 square meters or smaller priced at 1.5 million yuan or below will see their interest costs lowered, while those using new loans to refinance existing mortgages are excluded.

<details><summary>References</summary>
<ul>
<li><a href="https://www.163.com/dy/article/L82D51AN0514R9P4.html?clickfrom=w_house">163.com/dy/article/L82D51AN0514R9P4.html?clickfrom=w_house</a></li>

</ul>
</details>

**Tags**: `#China fiscal policy`, `#housing policy`, `#mortgage subsidy`, `#real estate`, `#first-time homebuyers`

---