---
layout: default
title: "Horizon Summary: 2026-09-30 (EN)"
date: 2026-09-30
lang: en
---

> From 50 items, 17 important content pieces were selected

---

**Technology News**
1. [OpenAI announces GPT-6.1 Sol: near-Astra intelligence at about a fifth of the price](#item-tech-news-1) ⭐️ 8.0/10
2. [OpenAI Announces Dots for Always-On AI Agents, Excluding EEA, Switzerland, and UK](#item-tech-news-2) ⭐️ 7.0/10
3. [Browser visualization renders real-time Solar System with 526k asteroids and tracked satellites](#item-tech-news-3) ⭐️ 7.0/10
4. [How Delhi cut electricity losses from 50% to 5%](#item-tech-news-4) ⭐️ 7.0/10
5. [Public &\#x27;Relapse&\#x27; Exploit for PS5 Targets WebKit JavaScriptCore](#item-tech-news-5) ⭐️ 7.0/10
6. [Quoting Anthropic Frontier Red Team](#item-tech-news-6) ⭐️ 7.0/10
7. [Simon Willison begins live-blogging OpenAI DevDay 2026 keynote](#item-tech-news-7) ⭐️ 7.0/10
8. [&\#x27;How to Make Your Model Fast&\#x27;: Free Open-Source Book on ML Performance Engineering](#item-tech-news-8) ⭐️ 7.0/10
9. [Cloudflare launches cf, an agent-friendly CLI covering its full API in open beta](#item-tech-news-9) ⭐️ 7.0/10
10. [Trump and Six AI Giants Sign One-Page &\#x27;Morally Binding&\#x27; AI Safety Agreement](#item-tech-news-10) ⭐️ 7.0/10
11. [DeepSeek Reportedly Open-Sources Foundational Compute Components for Huawei Ascend](#item-tech-news-11) ⭐️ 7.0/10
12. [Cloudflare announces plan to become a public certificate authority](#item-tech-news-12) ⭐️ 7.0/10
13. [Microsoft Reportedly Uses Hundreds of Outsourced Workers to Review Copilot Prompts and Images](#item-tech-news-13) ⭐️ 7.0/10

**Financial News**
1. [China threatens &\#x27;firm&\#x27; retaliation if EU restricts Chinese businesses](#item-finance-news-1) ⭐️ 7.0/10
2. [Premarket movers: Fair Isaac plunges 18% on FHFA pricing change; AMD buys World Labs for $8.2 billion](#item-finance-news-2) ⭐️ 7.0/10
3. [Trump&\#x27;s municipal bond portfolio grows to as much as $1 billion, CNBC analysis finds](#item-finance-news-3) ⭐️ 7.0/10
4. [China sets three new criteria for humanoid robot IPOs, sources say](#item-finance-news-4) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [OpenAI announces GPT-6.1 Sol: near-Astra intelligence at about a fifth of the price](https://openai.com/index/introducing-gpt-6-1-sol/) ⭐️ 8.0/10

OpenAI announced GPT-6.1 Sol, pitched as &\#x27;near-Astra&\#x27; — near-frontier — intelligence for about a fifth of the price, with cached input quoted at $0.10 per million tokens: 95% below standard input pricing and 50% below GPT-6 Sol&\#x27;s cached rate. The cached-input cut is the most concrete figure in the available material and matters most for agentic coding workloads such as Codex, which resend large context repeatedly. The &\#x27;near-Astra&\#x27; capability claim is the company&\#x27;s own announcement framing and is not backed by benchmarks or independent measurements in the supplied material.

hackernews · crorella · Sep 29, 17:06 · [Discussion](https://news.ycombinator.com/item?id=49896586)

**「Background」** Within OpenAI&\#x27;s GPT-6 lineup, &quot;Astra&quot; denotes the flagship tier that GPT-6.1 Sol undercuts: the new model costs $2 per million input tokens — one-fifth of GPT-6 Astra&\#x27;s standard rate — and its $0.10 per million cached-input price is one-tenth of Astra&\#x27;s while also running 50% below the cached rate of the earlier GPT-6 Sol, according to OpenAI&\#x27;s announcement. As a further point of comparison, VentureBeat reports that the previous-generation GPT-5.6 Sol is currently discounted to $4 per million input tokens, meaning GPT-6.1 Sol halves even that figure.

**「Impact for developers」** For teams running coding and agentic workloads, the concrete consequence is cost: cached input drops to $0.10 per million tokens—95% below standard input pricing and 50% below GPT-6 Sol&\#x27;s cached rate—which matters most for context-heavy tools like Codex that re-read long context repeatedly. The &\#x27;near-Astra&\#x27; intelligence claim is a vendor assertion made amid an active price war for cost-conscious business customers: Anthropic reports Opus 5.5 leading GPT-6 Astra 66.4% to 57.9% on Terminal-Bench 4.0, while OpenAI says Sol matches Fable 5.1 on coding at lower cost, and the two claims are not directly comparable. Teams should benchmark GPT-6.1 Sol against alternatives on their own repositories before switching, particularly given community reports that the prior GPT-6 Sol release was a quality regression.

**「Community reaction」** Commenters treated pricing, not capability, as the real story: one argues token price becoming the &\#x27;main battleground&\#x27; is ominous for the industry and its investors and speculates it could factor into Anthropic&\#x27;s IPO timing, while another contends AI models are a commodity with &\#x27;no real moat&\#x27; caught in a race to the bottom. Other users described GPT-6 Sol as a marked regression from Sol 5.6 that pushed them to Anthropic&\#x27;s Opus 5.5, and one speculated — without confirmation — that 6.1 is &\#x27;Astra-Minor,&\#x27; a model name reportedly spotted in files days earlier, renamed after Sol 6 underwhelmed.

<details><summary>References</summary>
<ul>
<li><a href="https://thenextweb.com/news/openai-gpt-6-1-sol-price-astra-devday">‘Near-Astra intelligence for a fifth of the price’: GPT-6.1 Sol</a></li>
<li><a href="https://venturebeat.com/technology/openais-gpt-6-1-sol-offers-astra-like-performance-at-1-5th-price-a-new-ultrafast-tier-clocks-at-300-tokens-per-second">OpenAI&#x27;s GPT-6.1 Sol offers Astra-like performance at 1/5th price. A new Ultrafast tier clocks at 300 tokens per second. | VentureBeat</a></li>
<li><a href="https://openai.com/index/introducing-gpt-6-1-sol/">Introducing GPT-6.1 Sol | OpenAI</a></li>
<li><a href="https://fortune.com/2026/09/22/what-ai-slowdown-openai-anthropic-release-dueling-moreaffordable-models-as-ai-price-wars-heat-up/">What slowdown? OpenAI, Anthropic release dueling models as AI price wars heat up | Fortune</a></li>
<li><a href="https://www.progressiverobot.com/2026/09/23/ai-price-war-anthropic-openai-cheaper-ai-models/">Price War: Anthropic and OpenAI Smart, Proven AI Cuts</a></li>

</ul>
</details>

**Tags**: `#openai`, `#llm`, `#model-release`, `#pricing`, `#ai-industry`

---

<a id="item-tech-news-2"></a>
### [OpenAI Announces Dots for Always-On AI Agents, Excluding EEA, Switzerland, and UK](https://openai.com/index/introducing-dots/) ⭐️ 7.0/10

OpenAI announced Dots, a product built around always-on AI agents intended to operate continuously rather than only on demand. What is known so far comes from the vendor&\#x27;s announcement; no independent evaluation of the shipped product is available yet. According to OpenAI&\#x27;s own help documentation cited in the discussion thread, the product excludes users in the European Economic Area, Switzerland, and the UK at launch. The announcement drew substantial debate on Hacker News about agent autonomy, trust, and practical usefulness.

hackernews · alvis · Sep 29, 17:07 · [Discussion](https://news.ycombinator.com/item?id=49896604)

**「Background」** Unveiled at OpenAI&\#x27;s DevDay event, Dots is a personal agentic assistant built on the GPT-6 Astra model, with each agent running on a cloud computer equipped with a web browser, and OpenAI positions it as a rival to Meta&\#x27;s Muse agent. The launch came one day after OpenAI apologized for a hack carried out by its own bots, meaning the product&\#x27;s always-on autonomy arrives while questions about rogue-agent safety are still fresh.

**「Pro-only rollout leaves UK and Europe waiting」** At launch, Dots is available only to ChatGPT Pro subscribers outside the European Economic Area, Switzerland, and the UK, so users and developers in those regions cannot adopt or build on the always-on agents yet, and OpenAI&\#x27;s help centre lists no release date for the excluded countries or for Free, Go, or Plus tiers. Teams considering Dots for automation should confirm regional availability before planning dependent workflows, since the agent links to more than 4,000 apps through ChatGPT at launch.

**「Community discussion」** In a 453-comment thread, opinions diverged: one commenter who uses comparable always-on agents argued that domain-specific agents collaborating with each other keep context windows manageable and create clearer trust boundaries, while another said their throughput is limited by their own approval rate, making overnight agent runs of little value. Skeptics also raised safety — one noted that recent consensus on a similar tool called openclaw was to grant it no write, delete, or sensitive-read access — and frustration that launched AI products often arrive &quot;severely nerfed&quot; relative to their demos.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/09/29/openai-launches-dots-its-bubbly-agentic-avatar/">OpenAI launches Dots, its bubbly agentic avatar | TechCrunch</a></li>
<li><a href="https://www.macrumors.com/2026/09/29/openai-launches-dots/">OpenAI Launches Always-On &#x27;Dots&#x27; Agents to Rival Meta&#x27;s Muse - MacRumors</a></li>
<li><a href="https://www.nbcnews.com/tech/tech-news/openai-launches-dots-ai-agents-safety-questions-rcna600338">OpenAI launches always-on AI agents a day after apologizing for a hack by its bots</a></li>
<li><a href="https://shattered.io/openai-dots-4000-apps-skip-uk-eu-2026/">OpenAI dots: 4,000+ Apps, No UK/EU Access Yet [2026]</a></li>
<li><a href="https://madrobot.blog/2026/09/29/chatgpt-dots-uk-europe-release-date/">ChatGPT Dots UK &amp; Europe Release Date: Is It Out? | MadRobot</a></li>
<li><a href="https://nerdschalk.com/chatgpt-dots-regional-availability/">When Will ChatGPT Dots Become Available in My Region?</a></li>

</ul>
</details>

**Tags**: `#ai-agents`, `#openai`, `#agent-autonomy`, `#trust-and-safety`, `#product-launch`

---

<a id="item-tech-news-3"></a>
### [Browser visualization renders real-time Solar System with 526k asteroids and tracked satellites](https://space.bl2.net/) ⭐️ 7.0/10

A developer has released a browser-based Solar System visualization that renders approximately 526,000 asteroids and all tracked Earth satellites in real time at true scale. The site combines CelesTrak TLE data propagated with SGP4 for satellites, asteroid and comet data from JPL&\#x27;s Small-Body Database, and spacecraft positions from JPL Horizons, with all datasets updated daily. Rendering uses WebGL2, orbit propagation runs in web workers, and the roughly 30 MB asteroid dataset loads in the background. A time slider runs both forward and backward, and satellites appear and disappear according to their launch dates.

hackernews · wanick · Sep 29, 19:08 · [Discussion](https://news.ycombinator.com/item?id=49898778)

**「Public orbital catalogs and earlier trackers」** Tracking objects in Earth orbit has long relied on two-line element sets \(TLEs\) published by catalogs such as CelesTrak and propagated with the standard SGP4 model, while JPL&\#x27;s Small-Body Database supplies asteroid and comet orbits and the Horizons system provides spacecraft ephemerides. Real-time browser trackers for a handful of bodies already existed — Space Informer, for example, offers a live map of planet positions, the ISS, and satellites with live distances — so this project&\#x27;s step is applying the same public-data approach at the scale of hundreds of thousands of objects.

**「Impact」** Space enthusiasts and educators get a no-install way to watch real spacecraft in their actual positions: one commenter reports already using the site to follow Europa Clipper ahead of its second Earth gravity assist, and another notes an ordinary laptop renders the roughly half-million-object scene at over 60 fps. The main compatibility constraint is that WebGL2 is the only rendering path, so browsers without it cannot display the scene, and the full asteroid view appears only after a roughly 30 MB background download of data that the author refreshes daily from CelesTrak and JPL.

**「Community reaction」** Commenters reported that the site runs smoothly on ordinary hardware, with one recalling that orbital calculations on a 486DX once managed about 30 objects at roughly 30 fps, versus half a million objects at over 60 fps in a browser today. Another commenter argued the project shows how easily LLMs can now build such visualizations when the underlying data is structured and publicly available, while one user demonstrated a practical use by tracking the Europa Clipper spacecraft ahead of its Earth flyby gravity assist.

<details><summary>References</summary>
<ul>
<li><a href="https://spaceinformer.com/solar-system-live/">Solar System Live: Track Planets &amp; Satellites in Real-Time</a></li>

</ul>
</details>

**Tags**: `#webgl2`, `#data-visualization`, `#orbital-mechanics`, `#web-workers`, `#space`

---

<a id="item-tech-news-4"></a>
### [How Delhi cut electricity losses from 50% to 5%](https://spectrum.ieee.org/delhi-electricity-loss) ⭐️ 7.0/10

IEEE Spectrum has published a deep-dive explaining how Delhi reduced electricity distribution losses from 50% to 5%, a turnaround the piece characterizes as one of the world&\#x27;s most significant power-grid reforms. It credits a combination of technical and policy changes rather than any single fix; a commenter quoting the article notes that the losses &quot;weren&\#x27;t caused solely by technical&quot; problems. The piece is retrospective analysis rather than a new announcement or measurement, but it drew heavy engagement on Hacker News, with 288 comments covering theft prevention, load shedding, and grid modernization.

hackernews · rbanffy · Sep 29, 12:43 · [Discussion](https://news.ycombinator.com/item?id=49892245)

**「Background」** Delhi&\#x27;s turnaround has roots in reforms dating to the early 2000s: the city moved to privatized electricity distribution in 2002, and India&\#x27;s Electricity Act of 2003 extended the overhaul nationally by unbundling state control of the grid into separate generation, transmission, and distribution entities and opening the power sector to privatization. The headline metric is AT&amp;C \(aggregate technical and commercial\) loss, which counts both electricity dissipated on the network and power delivered but never billed or collected, so reducing it required engineering upgrades as well as theft prevention and billing enforcement. Reporting on Delhi&\#x27;s distributors credits the fall from roughly 52% losses to about 6% since those reforms to privatization, infrastructure upgrades, smart metering, SCADA/AI-based monitoring, and enforcement.

**「Impact」** For utilities and regulators in regions where theft and collection failure drive high distribution losses, Delhi serves as a documented benchmark that losses can be brought down to 5%. The caveat raised in the discussion is that this required policy and enforcement reform alongside infrastructure work, so replication depends on institutional change rather than equipment upgrades alone.

**「Community discussion」** The most substantive argument holds that eliminating load shedding, not the loss figures, was the real revolution: one commenter who lived in Delhi recalls outages several times a day two decades ago, returning-power surges that threatened expensive appliances, and offices wired with two separate sets of sockets. Others added color and comparisons — insulated anti-theft lines reportedly doubling as safe &quot;roads&quot; for monkeys, and Estonia&\#x27;s grid \(99% smart-meter coverage, 99.99% reliability\) offered as a contrast — though these reflect individual reports rather than established facts.

<details><summary>References</summary>
<ul>
<li><a href="https://timesofindia.indiatimes.com/city/delhi/from-50-losses-to-6-how-delhi-fixed-its-power-loses/articleshow/130121379.cms">From 50% losses to 6%: How Delhi fixed its power loses | Delhi News - The Times of India</a></li>
<li><a href="https://spectrum.ieee.org/delhi-electricity-loss">How Delhi Cut Electricity Loss from 50 to 5 Percent - IEEE Spectrum</a></li>

</ul>
</details>

**Tags**: `#power-grid`, `#infrastructure`, `#energy-policy`, `#india`, `#electrical-engineering`

---

<a id="item-tech-news-5"></a>
### [Public &\#x27;Relapse&\#x27; Exploit for PS5 Targets WebKit JavaScriptCore](https://github.com/ntfargo/Relapse-Exploit) ⭐️ 7.0/10

A GitHub repository, ntfargo/Relapse-Exploit, surfaced on Hacker News on September 29, 2026, presented as a PlayStation 5 exploit targeting the WebKit JavaScriptCore engine; the post drew 301 points and 177 comments. Because the PS5 has so far resisted public exploits, any published foothold draws attention, but the available material is only the repository link: the exploit&\#x27;s capability level \(userland code execution versus kernel access\), its reliability, and whether it enables a full jailbreak are not established by the supplied evidence. If it works as described, it would give researchers and homebrew developers a rare documented entry point on Sony&\#x27;s current-generation console, and readers should treat its real-world capability as unverified until independent results appear.

hackernews · therepanic · Sep 29, 15:44 · [Discussion](https://news.ycombinator.com/item?id=49895304)

**「How PS5 exploit chains work」** Gaining deep access to a modern console typically requires a two-stage exploit chain: a userland bug that executes unsigned code, often reached through the console&\#x27;s embedded WebKit browser, followed by a kernel-level bug that escalates privileges. The Relapse Exploit follows this structure, pairing a WebKit memory leak with a use-after-free race in the kernel&\#x27;s aio\_multi\_wait interface, and its public repository lists PS5 firmware versions 7.00 through 13.60 as supported.

**「Impact for PS5 owners」** For PS5 owners on firmware 7.00–13.60, the Relapse chain runs through the console&\#x27;s browser — a community autoloader \(ps5-webkit-autoloader-13x\) caches the exploit page and adds a homescreen app to relaunch it — giving users a concrete path to capabilities Sony blocks, such as the local USB save backups one commenter sought after losing a year of Minecraft progress to corruption \(the PS5 restricts saves to per-profile PS Plus cloud storage\). This access is firmware-dependent, so interested users must hold off on system updates, and it may prove short-lived: WebKit documents that JavaScriptCore&\#x27;s no-JIT &quot;mini mode&quot; is harder to exploit, and commenters expect Sony could disable JIT in the browser to shrink this attack surface.

**「Community discussion」** Commenters focused on what the bug implies rather than demonstrated results: MaxBarraclough asked whether the PS5&\#x27;s WebKit runs JavaScriptCore with the JIT compiler enabled and suggested Sony might respond by disabling JIT to shrink the attack surface, while Muromec offered the speculation that console-hacking groups typically hold additional zero-days for whatever privilege-escape step this bug does not cover. On the consumer side, publlus\_enigma reported losing a year of their daughter&\#x27;s Minecraft progress to data corruption and argued that local save backups — blocked on the PS5 except through paid PS Plus cloud storage, unlike the PS1 through PS4 — are the main practical motivation for running such an exploit.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ntfargo/Relapse-Exploit">GitHub - ntfargo/Relapse-Exploit: Exploit chain for PS5 7.00 - 13.60 · GitHub</a></li>
<li><a href="https://dev.to/lu1tr0n/relapse-repo-afirma-exploit-de-ps5-en-firmware-700-1360-1n14">Relapse: repo afirma exploit de PS5 en firmware 7.00-13.60 - DEV Community</a></li>
<li><a href="https://elsolitario.org/en/2026/09/29/relapse-repo-claims-ps5-exploit-firmware-7-00-to-13-60/">PS5 Jailbreak: What Is Relapse Exploit and Its Scope</a></li>
<li><a href="https://news.ycombinator.com/item?id=49898390">At a glance, it looks like it exploits a bug in WebKit &#x27;s * JavaScriptCore ...</a></li>
<li><a href="https://webkit.org/blog/10308/speculation-in-javascriptcore/">Speculation in JavaScriptCore | WebKit</a></li>
<li><a href="https://github.com/CielWhat/ps5-webkit-autoloader-13x">GitHub - CielWhat/ ps 5 - webkit -autoloader-13x · GitHub</a></li>

</ul>
</details>

**Tags**: `#console-security`, `#exploit`, `#playstation-5`, `#webkit`, `#javascriptcore`

---

<a id="item-tech-news-6"></a>
### [Quoting Anthropic Frontier Red Team](https://simonwillison.net/2026/Sep/29/anthropic-frontier-red-team/) ⭐️ 7.0/10

Simon Willison quotes Anthropic&\#x27;s Frontier Red Team reporting that GLM-5.3 and Claude Mythos Preview now succeed at full control flow hijacks on binary exploitation benchmark tasks, a capability threshold earlier models did not cross.

rss · Simon Willison · Sep 29, 22:20

**Tags**: `#anthropic`, `#ai-safety`, `#cybersecurity`, `#llm-evaluations`, `#ai-security-research`

---

<a id="item-tech-news-7"></a>
### [Simon Willison begins live-blogging OpenAI DevDay 2026 keynote](https://simonwillison.net/2026/Sep/29/openai-devday-2026-live-blog/) ⭐️ 7.0/10

Simon Willison has opened a live blog covering OpenAI DevDay 2026 at Fort Mason in San Francisco on September 29, 2026, stating he will post notes on the keynote and other developer-focused sessions throughout the day. The supplied post is only the opening stub: it contains no keynote announcements, product details, or API changes yet, so what OpenAI actually shipped or claimed at the event is not documented in this source. Willison says he is using the same live-blog approach as his 2025 DevDay coverage and discloses that OpenAI gave him a free ticket and a seat in the keynote&\#x27;s &quot;creator&quot; area. Readers should treat this as an entry point for ongoing coverage rather than a report of concrete announcements.

rss · Simon Willison · Sep 29, 15:55

**「Background」** OpenAI DevDay is the company&\#x27;s annual developer conference, and the 2026 edition is being held at Fort Mason in San Francisco. Willison covered the previous edition the same way, live-blogging the keynote in a post dated October 6, 2025, which this entry explicitly links back to as last year&\#x27;s coverage.

**「What developers should do with this」** Teams building on OpenAI&\#x27;s APIs and coding-agent tooling now have a concrete review task: OpenAI&\#x27;s DevDay 2026 recap lists more than 20 announcements covering GPT-6 Astra, ChatGPT, Codex, APIs, security, and new builder tools, so developers should check which of these changes touch capabilities they depend on before updating production integrations. Because that list is OpenAI&\#x27;s own account of the September 29 event at Fort Mason, treat it as a vendor claim of what was announced rather than independent verification, and cross-check it against other coverage such as CNBC&\#x27;s live keynote report.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/devday-2026-recap/">DevDay 2026 Recap - OpenAI</a></li>
<li><a href="https://devday.openai.com/">OpenAI DevDay [2026]</a></li>
<li><a href="https://www.cnbc.com/2026/09/29/openai-devday-2026-live-updates.html">OpenAI DevDay 2026: Live updates and announcements - CNBC</a></li>

</ul>
</details>

**Tags**: `#openai`, `#llms`, `#coding-agents`, `#live-blog`, `#developer-ecosystem`

---

<a id="item-tech-news-8"></a>
### [&\#x27;How to Make Your Model Fast&\#x27;: Free Open-Source Book on ML Performance Engineering](https://www.reddit.com/r/MachineLearning/comments/1wt6ns4/i_wrote_a_free_opensource_book_on_making_ml/) ⭐️ 7.0/10

Reddit user /u/SoloTiger\_ has published &\#x27;How to Make Your Model Fast: A Systems View of Efficient Machine Learning, from Silicon to Agents,&\#x27; a free, open-source book hosted on GitHub at usamahz/make-your-model-fast. Its central premise is that reducing FLOPs doesn&\#x27;t necessarily make a model faster, so readers first need to determine whether a system is compute-, bandwidth-, memory-, or system-bound. The book starts with roofline analysis and hardware, then works up through kernels, compilers, quantization, pruning, vision, on-device LLMs, robotics, profiling, serving, and agent systems. As a self-published announcement, its technical quality cannot yet be independently verified, and the author is soliciting feedback and contributions from practitioners in ML systems, inference, compilers, edge AI, and performance engineering.

reddit · r/MachineLearning · /u/SoloTiger\_ · Sep 29, 10:35

**「Background」** The book rests on the roofline-model premise that a workload runs only as fast as its scarcest resource—compute throughput or memory bandwidth—so reducing floating-point operations often produces no real speedup when the workload is bandwidth- or memory-bound. It joins a small set of free, hardware-first ML texts: the jax-ml project&\#x27;s &quot;How to Scale Your Model&quot; book likewise explains how TPUs and GPUs work and how to parallelize models during training and inference, but centers on scaling large models rather than optimizing an individual model&\#x27;s inference from kernels up to serving and agents. The author publishes on GitHub as usamahz and identifies himself as an ML engineer at the chip designer Arm.

**「Impact」** Practitioners can read the full text for free on GitHub and submit corrections or contributions through the open-source repository. For inference and edge-AI teams, the book&\#x27;s roofline-first framing offers a concrete decision procedure for whether quantization, pruning, or kernel optimization is worth pursuing on specific hardware before committing engineering time.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/usamahz">usamahz (Usamah) · GitHub</a></li>
<li><a href="https://jax-ml.github.io/scaling-book/">How To Scale Your Model - jax-ml.github.io</a></li>
<li><a href="https://github.com/jax-ml/scaling-book/blob/main/index.md">scaling-book/index.md at main · jax-ml/scaling-book · GitHub</a></li>

</ul>
</details>

**Tags**: `#machine-learning-systems`, `#performance-engineering`, `#inference-optimization`, `#open-source`, `#hardware`

---

<a id="item-tech-news-9"></a>
### [Cloudflare launches cf, an agent-friendly CLI covering its full API in open beta](https://blog.cloudflare.com/cloudflare-cf-cli-launch/) ⭐️ 7.0/10

Cloudflare has launched cf, a new command-line tool now in open beta, giving developers and AI agents terminal access to more than 3,000 Cloudflare API operations. Unlike the existing Wrangler CLI, which covers roughly 280 operations, cf is generated from Cloudflare&\#x27;s API schemas and defaults to JSON output, with built-in command search and guidance to help agents discover, execute, and interpret commands. Cloudflare&\#x27;s own examples show a single agent using cf to create and deploy Workers, monitor services, configure Access and WAF settings, and even purchase domains. The coverage and agent-workflow claims come from Cloudflare&\#x27;s announcement of a beta product, not from independent testing.

telegram · zaihuapd · Sep 29, 13:46

**「Wrangler, the CLI cf builds on and departs from」** Cloudflare&\#x27;s existing command-line tool, Wrangler, was designed around human developer workflows and exposes commands for only about 280 of the company&\#x27;s thousands of API operations. The new cf CLI is generated from Cloudflare&\#x27;s API schemas to mirror the full API of more than 3,000 operations, and it defaults to machine-readable JSON output rather than human-formatted text — a deliberate departure aimed at AI agents, which need to parse results and discover commands programmatically instead of reading help pages.

**「Why it matters」** Teams building AI agents or automation on Cloudflare get a single command-line entry point to nearly the entire Cloudflare API — from Worker deployment to WAF configuration and domain purchases — without writing raw API calls, and the JSON-first output lets agent pipelines parse results directly. Because cf is an open beta, organizations should validate its stability and coverage before relying on it for production workflows, and Wrangler remains the established tool for the roughly 280 operations it already covers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.brocker.org/cloudflare-cf-agentic-cli-full-api">Cloudflare releases cf , an agentic CLI for its full API</a></li>
<li><a href="https://blog.cloudflare.com/cloudflare-cf-cli-launch/">Introducing cf : the agentic CLI for the entire Cloudflare API</a></li>

</ul>
</details>

**Tags**: `#cloudflare`, `#cli`, `#ai-agents`, `#developer-tools`, `#api`

---

<a id="item-tech-news-10"></a>
### [Trump and Six AI Giants Sign One-Page &\#x27;Morally Binding&\#x27; AI Safety Agreement](https://www.zaobao.com.sg/news/world/story20260930-9758185) ⭐️ 7.0/10

US President Donald Trump on September 29 signed a one-page AI safety agreement together with the leaders of Google, Anthropic, Meta, OpenAI, xAI, and NVIDIA, publishing the document on Truth Social and describing it as &quot;morally binding.&quot; Under the agreement, the companies commit to a four-layer control framework: cooperating with external audit institutions to independently evaluate their AI control systems, establishing an independent board committee for oversight, and monitoring model capabilities and alignment for cybersecurity, biological, and chemical threats during training and deployment. The stated purpose of these measures is to verify that safeguards operate as intended, but the document&\#x27;s brevity and non-legally-binding character mean the commitments rest on voluntary adherence rather than enforceable obligations.

telegram · zaihuapd · Sep 30, 02:30

**「A voluntary pledge, not a regulation」** The pact follows Trump&\#x27;s consistent opposition to binding AI rules: he has rejected calls for government restrictions and urged rapid AI development, dismissed fears of the technology going rogue as &quot;a hoax,&quot; and in a Truth Social post earlier this month wrote that the United States &quot;will not in any way hinder or stifle the Growth of this incredible Industry.&quot; In place of regulation, the agreement leans on companies performing &quot;tremendous self-policing&quot; of their products, a framework that some outlets, including The Guardian, characterized as vague.

**「Voluntary accord, concrete oversight duties for six AI labs」** The immediate consequence falls on developers at the six signatory companies — Google, Anthropic, Meta, OpenAI, xAI, and NVIDIA — which commit to external audits of their AI control systems, independent board-committee oversight, and monitoring of frontier-model capabilities and alignment for cybersecurity, biosecurity, and chemical threats during training and deployment. Because the one-page document is described as &quot;morally binding&quot; rather than legally enforceable, customers of these AI products gain no new legal recourse if commitments go unmet, and AI companies outside the six signatories are under no obligation at all. Organizations that rely on these vendors can ask whether audit and board-oversight mechanisms are actually being implemented, since adherence depends entirely on each company&\#x27;s voluntary compliance.

<details><summary>References</summary>
<ul>
<li><a href="https://www.france24.com/en/technology/20260929-trump-says-ai-companies-sign-voluntary-accord-on-safety-controls">Trump says AI companies sign voluntary accord on safety controls</a></li>
<li><a href="https://www.theguardian.com/us-news/2026/sep/29/trump-ai-deal-tech-ceos-superintelligence">Trump announces vague ‘morally binding’ AI deal... | The Guardian</a></li>
<li><a href="https://www.rt.com/news/646452-tech-pact-ai-controls/">Trump and US tech giants sign pact to stop AI from... — RT World News</a></li>
<li><a href="https://www.newsmax.com/politics/donald-trump-ai-accord/2026/09/29/id/1271143/">Trump Calls AI Pact &#x27;Morally Binding&#x27; as Tech Giants Commit to...</a></li>
<li><a href="https://www.usnews.com/news/top-news/articles/2026-09-29/trump-releases-ai-accord-with-tech-executives">Trump Releases AI Accord With Tech Executives</a></li>
<li><a href="https://cointelegraph.com/news/trump-accord-calls-for-tech-firms-to-self-police-their-own-frontier-ai">Trump , Tech CEOs Sign Voluntary Frontier AI Safety Pact</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#AI governance`, `#tech policy`, `#AI industry`, `#regulation`

---

<a id="item-tech-news-11"></a>
### [DeepSeek Reportedly Open-Sources Foundational Compute Components for Huawei Ascend](https://mp.weixin.qq.com/s/X41mKH4Ds-VXUAnK6M8Eww) ⭐️ 7.0/10

DeepSeek has reportedly open-sourced its foundational AI compute components for Huawei&\#x27;s Ascend platform, including DeepGEMM Ascend, DeepEP Ascend, TileKernels, FlashMLA, and DeepSelect, along with TileLang-based compiler tooling for compute kernels and distributed communication libraries — mirroring the stack it maintains for NVIDIA GPUs. The September 30, 2026 report states DeepSeek claims the components reach near-hardware-limit performance across multiple tests and that it is working with Huawei on a 128-card Ascend 950 supernode design. These performance figures and the Ascend 950 collaboration are vendor statements that have not been independently verified, and the item originates from a single Telegram/WeChat aggregator channel rather than a primary DeepSeek or Huawei announcement.

telegram · zaihuapd · Sep 30, 03:09

**「DeepSeek&\#x27;s earlier NVIDIA CUDA stack」** These components are Ascend ports of libraries DeepSeek had already open-sourced for NVIDIA CUDA GPUs — DeepGEMM for matrix-multiplication kernels, DeepEP for distributed communication, FlashMLA, and the TileLang toolchain — and the new repositories are designed to be drop-in equivalents: the DeepGEMM-Ascend project describes itself as fully API-compatible with DeepGEMM, supporting BF16, FP8, and FP4 GEMM, MQA logits, and MegaMoE. DeepSeek credited Huawei&\#x27;s team with substantial support during development, and the projects are published on GitHub and reported to be buildable on Ascend 950 hardware.

**「Impact for Ascend adopters」** Organizations running DeepSeek models or custom AI workloads on Huawei Ascend hardware gain a maintained, open-source path to the same kernel and communication stack DeepSeek uses on NVIDIA GPUs, as the Ascend versions of TileLang, DeepGEMM, DeepEP, and FlashMLA are reported to mirror the CUDA toolchain one-to-one \(tool-3-1, tool-3-2\). Teams should benchmark the Ascend ports against their own workloads before migrating, since the near-hardware-limit performance figures are DeepSeek&\#x27;s own claims, and the jointly developed Ascend 950 128-card supernode remains a plan in progress rather than a shipped product — extending a Huawei–DeepSeek collaboration that an earlier report already tied to Ascend 950 supernode support for DeepSeek V4 training \(tool-3-3\).

<details><summary>References</summary>
<ul>
<li><a href="https://tech.ifeng.com/c/8wpvR2zbzBw">DeepSeek 开 源 昇 腾 基础组件：与英伟达平台一一对应_凤凰网</a></li>
<li><a href="https://github.com/deepseek-ai/DeepGEMM-Ascend">GitHub - deepseek -ai/ DeepGEMM - Ascend : DeepGEMM - Ascend ...</a></li>
<li><a href="https://trendshift.io/repositories/270861">deepseek -ai/ DeepGEMM - Ascend — GitHub trending stats... | Trendshift</a></li>
<li><a href="https://todayforai.com/zh/news/20260930-news-deepseek-ascend-infra-open-source">DeepSeek 开源昇腾版全套 AI 基础设施：对齐 CUDA 工具链，适配 128 ...</a></li>
<li><a href="https://tech.china.com/article/20260930/202609301963239.html">DeepSeek开源昇腾基础组件，联手华为优化128卡超节点</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/2031649923507172150">AI行业动态20260426: 华为&quot;超节点&quot;携昇腾950芯片支撑DeepSeek V4训练...</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#Huawei Ascend`, `#open source`, `#AI infrastructure`, `#GPU kernels`

---

<a id="item-tech-news-12"></a>
### [Cloudflare announces plan to become a public certificate authority](https://blog.cloudflare.com/cloudflare-certificate-authority/) ⭐️ 7.0/10

Cloudflare has announced plans to become a public certificate authority: it has applied to join the Chrome, Apple, Microsoft, and Mozilla root certificate programs and signed an agreement with GlobalSign to acquire a widely trusted root certificate. This is an intent announcement only — no certificates have been issued yet. The new CA will prioritize ACME support for automated issuance and renewal, and Cloudflare plans to begin issuing production-grade Merkle Tree Certificates \(MTC\) in the first quarter of 2027, aimed at a post-quantum internet. Acquiring an already-trusted root from GlobalSign could shorten the path to broad browser and operating system trust compared with growing a new root from scratch.

telegram · zaihuapd · Sep 30, 06:26

**「Background」** Browsers and operating systems decide which certificate authorities users trust by default through root programs run by Chrome, Apple, Microsoft, and Mozilla, so a new public CA typically must either gain admission to those programs or acquire an already-trusted root; Cloudflare is pursuing both routes, and per its announcement materials the GlobalSign root acquisition is expected to close within the next two months, subject to closing conditions. Merkle Tree Certificates, which Cloudflare targets for production issuance from early 2027, are a proposed post-quantum alternative to the RSA and ECDSA signatures used in today&\#x27;s TLS certificates, which could in principle be forged by a sufficiently powerful quantum computer.

**「Impact」** Once Cloudflare&\#x27;s root certificate is accepted into the Chrome, Apple, Microsoft, and Mozilla root programs, website operators will gain an additional publicly trusted CA in the Web PKI ecosystem, with ACME automated issuance and renewal as its primary workflow. Near term there is nothing to migrate: Cloudflare has not yet begun issuing certificates, so organizations should monitor root-program inclusion progress rather than change providers, and the planned production-grade Merkle Tree Certificates for a post-quantum internet, targeted for Q1 2027, remain an announced plan rather than an available capability.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cloudflare.net/news/news-details/2026/Cloudflare-Announces-Public-Certificate-Authority-for-the-Post-Quantum-Web/default.aspx">Cloudflare Announces Public Certificate Authority for the Post ...</a></li>
<li><a href="https://www.helpnetsecurity.com/2026/09/30/cloudflare-certificate-authority-2027/">Post-quantum website certificates from Cloudflare are scheduled for early ...</a></li>
<li><a href="https://blog.cloudflare.com/pq-ca-with-mtcs/">Building a post-quantum certificate authority with... | Cloudflare Blog</a></li>

</ul>
</details>

**Tags**: `#Cloudflare`, `#certificate-authority`, `#PKI`, `#post-quantum`, `#TLS`

---

<a id="item-tech-news-13"></a>
### [Microsoft Reportedly Uses Hundreds of Outsourced Workers to Review Copilot Prompts and Images](https://www.404media.co/humans-reading-copilot-prompts-images/) ⭐️ 7.0/10

According to a 404 Media report, messages sent to Microsoft Copilot are not fully private: user prompts, requests, and even casually uploaded personal photos can be reviewed one by one by human staff, and Microsoft has hired hundreds of outsourced contractors specifically to evaluate Copilot&\#x27;s image generation and editing output. The reporting states these reviewers are routinely exposed to large volumes of disturbing material, including explicit &\#x27;upskirt&\#x27;-type photos and potentially illegal animal sacrifice imagery, inflicting serious psychological harm on the workers. The item presents these findings as 404 Media&\#x27;s reporting rather than a Microsoft announcement, and no company response or policy detail is included in the source.

telegram · zaihuapd · Sep 30, 07:13

**「Human raters in the AI feedback loop」** Microsoft&\#x27;s Copilot assistant lets users upload photos and request AI-generated edits, and improving generative image models typically relies on human raters who compare model outputs against the original requests — a practice that treats user submissions as quality-improvement data rather than strictly private content. Internal contractor documents indicate hundreds of such reviewers can be shown Copilot prompts, uploaded images, and the AI&\#x27;s generated edits. Unlike traditional content moderation, which screens material for policy violations, these contractors were judging which edit better followed a user&\#x27;s request, meaning disturbing submissions reached them through routine model evaluation rather than violation flags — the latest instance of a familiar industry pattern in which outsourced review work inflicts psychological harm on low-paid workers.

**「What this means for Copilot users」** Individuals using Copilot&\#x27;s image generation and editing features should assume their prompts and uploaded photos can be read by human reviewers rather than treated as strictly private, and avoid submitting intimate, identifying, or confidential images through the consumer service. Microsoft&\#x27;s own documentation states that enterprise Microsoft 365 Copilot data is secured by the organization&\#x27;s existing security, compliance, and privacy policies, while third-party guidance notes that free and Pro consumer tiers lack equivalent safeguards — so organizations handling sensitive material should verify their tenant-level protections instead of relying on consumer-style Copilot.

<details><summary>References</summary>
<ul>
<li><a href="https://windowsreport.com/human-copilot-reviewers-are-seeing-users-disturbing-image-editing-requests-new-report-reveals/">Human Copilot Reviewers Are Seeing Users’ Disturbing Image ...</a></li>
<li><a href="https://letsdatascience.com/news/microsoft-copilot-contractors-review-user-image-edits-6dcf58ca">Microsoft Copilot Contractors Review User Image Edits</a></li>
<li><a href="https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-365-copilot-architecture">Microsoft Copilot architecture and how it works</a></li>
<li><a href="https://spellbook.com/learn/is-copilot-private">Is Copilot AI Private? Legal Considerations for Lawyers</a></li>

</ul>
</details>

**Tags**: `#AI privacy`, `#Microsoft Copilot`, `#content moderation`, `#data privacy`, `#AI ethics`

---

## Financial News

<a id="item-finance-news-1"></a>
### [China threatens &\#x27;firm&\#x27; retaliation if EU restricts Chinese businesses](https://www.cnbc.com/2026/09/30/china-warns-europe-increases-trade-pressure.html) ⭐️ 7.0/10

China&\#x27;s commerce ministry said it will &quot;respond firmly&quot; if the EU imposes restrictions on Chinese businesses or products, warning that such steps during ongoing trade talks would &quot;seriously undermine mutual trust&quot; and disrupt negotiations. The warning came as EU Trade Commissioner Maroš Šefčovič demanded &quot;concrete results&quot; by October to narrow the world&\#x27;s largest bilateral goods trade deficit, ahead of his expected visit to Beijing, in a trading relationship the EU valued at 880 billion euros \(nearly $1 trillion\) including services last year.

rss · CNBC Finance · Sep 30, 03:39

**「What a &\#x27;Section 301&\#x27;-style tool would mean」** A &\#x27;Section 301&\#x27;-style mechanism, modeled on a provision of the U.S. Trade Act of 1974, would let the European Commission impose tariffs or quotas on Chinese goods without waiting for a World Trade Organization dispute ruling — a unilateral approach the EU has historically opposed, which limited its alignment with Washington when the U.S. first used it against Beijing.

**「Who could be affected」** If the EU imposes restrictions and Beijing follows through, German carmakers — which drew almost a third of their sales from China in 2023 — and EU exporters of goods China has retaliated against before, such as spirits, pork and dairy, would be among the most exposed.

<details><summary>References</summary>
<ul>
<li><a href="https://www.atlanticcouncil.org/blogs/econographics/as-chinas-surpluses-become-unbearable-the-eu-is-edging-toward-its-own-section-301/">As China’s surpluses become unbearable, the EU is edging ...</a></li>
<li><a href="https://informedclearly.com/en/trade-war/61779/eu-china-trade-war-european-section-301-2026">EU-China Trade War: Brussels&#x27; European Section 301 Explained</a></li>
<li><a href="https://www.investing.com/news/stock-market-news/factboxeuropean-carmakers-exposed-to-any-chinese-retaliation-for-eu-tariffs-3483675">Factbox- European carmakers exposed to any Chinese retaliation for...</a></li>
<li><a href="https://www.bta.bg/en/news/world/1045335-on-the-road-to-nowhere-european-carmakers-face-ev-push-from-china">BTA :: On the Road to Nowhere? European Carmakers Face EV Push...</a></li>

</ul>
</details>

**Tags**: `#EU-China trade`, `#trade policy`, `#tariffs`, `#trade deficit`, `#retaliation threat`

---

<a id="item-finance-news-2"></a>
### [Premarket movers: Fair Isaac plunges 18% on FHFA pricing change; AMD buys World Labs for $8.2 billion](https://www.cnbc.com/2026/09/29/stocks-making-the-biggest-moves-premarket-fair-isaac-spacex-amd-more.html) ⭐️ 7.0/10

Fair Isaac shares fell 18% premarket after FHFA Director Bill Pulte said Fannie Mae and Freddie Mac will replace their two mortgage pricing grids with one that adds VantageScore alongside FICO Classic. Also moving: AMD rose more than 1% on its $8.2 billion acquisition of AI firm World Labs, Summit Therapeutics jumped 18% on a $2 billion AstraZeneca equity investment and clinical collaboration, and CarMax gained more than 6% after second-quarter earnings of $1.16 per share on $7.88 billion revenue beat the FactSet consensus of 73 cents and $7.09 billion.

rss · CNBC Finance · Sep 29, 12:03

**「Background」** FICO has long been the near-exclusive credit score in US mortgage pricing: Fannie Mae and Freddie Mac, the government-backed companies that buy most home loans, priced loans off grids built around FICO scores. FHFA Director Bill Pulte&\#x27;s move to a single grid that also accepts rival VantageScore 4.0 opens that market to competition for the first time, threatening Fair Isaac&\#x27;s mortgage-scoring revenue. Separately, World Labs — the AI startup AMD is buying for $8.2 billion in an all-stock deal — was founded by Fei-Fei Li, a leading AI researcher often called the &\#x27;godmother of AI.&\#x27;

**「Impact」** Fair Isaac investors bear the immediate damage, since its Scores segment — $1.169 billion of the company&\#x27;s $1.99 billion in fiscal 2025 revenue — now faces VantageScore competition in the Fannie Mae and Freddie Mac mortgage pricing grid, and analysts flag its reliance on mortgage originations and its pricing power as key risks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.housingwire.com/articles/fhfa-gses-one-grid/">FHFA says GSEs will use one LLPA grid for FICO , VantageScore</a></li>
<li><a href="https://finance.yahoo.com/real-estate/articles/us-moves-end-fico-mortgage-131040861.html">The US Moves to End FICO ’s Mortgage Scoring Monopoly.</a></li>
<li><a href="https://www.wsj.com/tech/ai/amd-to-acquire-world-labs-for-8-2-billion-a8d03d11">AMD to Acquire World Labs for $8.2 Billion - WSJ</a></li>
<li><a href="https://finance.yahoo.com/technology/article/amd-just-spent-82-billion-to-enlist-the-godmother-of-ai-230634166.html">AMD just spent $8.2 billion to enlist the &#x27;godmother of AI&#x27; - Yahoo Finance</a></li>
<li><a href="https://seekingalpha.com/news/4640460-fair-isaac-slumps-17-on-vantagescore-directive">Fair Isaac slumps 17% on VantageScore directive (FICO:NYSE)</a></li>
<li><a href="https://investors.fico.com/static-files/4dd43bd8-b07f-472c-9e53-5cb224ec9acd">[PDF] 2025 Annual Report - FICO Investor Relations</a></li>

</ul>
</details>

**Tags**: `#premarket-movers`, `#mortgage-credit-policy`, `#earnings-surprise`, `#acquisitions`, `#biotech-investment`

---

<a id="item-finance-news-3"></a>
### [Trump&\#x27;s municipal bond portfolio grows to as much as $1 billion, CNBC analysis finds](https://www.cnbc.com/2026/09/29/trump-municipal-bond-portfolio.html) ⭐️ 7.0/10

A CNBC analysis of President Trump&\#x27;s financial disclosures found his municipal bond holdings have grown past 1,000 positions worth between $300 million and $1 billion as of 2026, a scale the director of the University of Chicago&\#x27;s Center for Municipal Finance called unprecedented for an individual investor. CNBC found no evidence Trump traded on advance knowledge of administration decisions, and the White House says outside managers independently control the accounts, but ethics experts say overlaps with policy — including coal-plant pollution exemptions covering issuers he holds — raise conflict-of-interest questions.

rss · CNBC Finance · Sep 29, 14:37

**「Background」** Municipal bonds are IOUs issued by states, cities, hospitals, and utilities whose finances can be swayed by federal funding and regulatory decisions. The federal conflict-of-interest law 18 U.S.C. § 208 bars executive branch officials from government matters affecting their own financial interests, but it does not apply to the president, which is why the ethics experts cited by CNBC say Trump can legally hold such debt.

**「Impact」** Because federal actions shape municipal borrowers&\#x27; finances, the portfolio links the president&\#x27;s wealth to issuers affected by his own policies: his accounts bought debt tied to coal plants later granted a two-year exemption from stricter EPA pollution rules, and hospital systems facing a projected $900 billion, decade-long Medicaid cut \(per KFF\) that S&amp;P Global Ratings warns could pressure their credits.

<details><summary>References</summary>
<ul>
<li><a href="https://www.law.cornell.edu/uscode/text/18/208">18 U.S. Code § 208 - Acts affecting a personal financial interest</a></li>
<li><a href="https://www.ecfr.gov/current/title-5/chapter-XVI/subchapter-B/part-2640">eCFR :: 5 CFR Part 2640 -- Interpretation, Exemptions and ...</a></li>

</ul>
</details>

**Tags**: `#municipal bonds`, `#Trump finances`, `#conflict of interest`, `#financial disclosures`, `#public policy`

---

<a id="item-finance-news-4"></a>
### [China sets three new criteria for humanoid robot IPOs, sources say](https://www.cnbc.com/2026/09/29/china-criteria-humanoid-robot-ipos.html) ⭐️ 7.0/10

China&\#x27;s securities regulator has issued unpublished &quot;window guidance&quot; requiring humanoid robot startups seeking IPOs to show sustainable revenue and commercial orders, narrowing losses over a three-year forecast, and core technology such as a robotic brain or hands, according to three unnamed sources — a bar that few or none of the at least two dozen companies that have filed to list in Hong Kong may meet. The CSRC did not respond to a request for comment, and the scrutiny follows Unitree&\#x27;s 6.1 billion yuan \($905 million\) Shanghai IPO on Aug. 19, whose shares have since nearly halved from their 845 yuan debut close to 459.65 yuan.

rss · CNBC Finance · Sep 30, 02:50

**「Background」** Chinese regulators had already used informal &quot;window guidance&quot; — unwritten instructions to slow or block listings — to hold back some humanoid-robot IPOs before the new criteria surfaced. The sector, part of Beijing&\#x27;s national push for &quot;embodied AI&quot; \(AI embedded in physical robots\), drew 47.09 billion yuan \($6.95 billion\) of investment in the second quarter alone, more than double the first quarter.

**「Impact」** China&\#x27;s 100-plus humanoid robot startups — at least two dozen of which have already filed to list in Hong Kong — and the government and private funds backing them could lose IPOs as a fundraising and exit route, deepening pressure on a sector where listed peers such as UBTECH have already seen shares fall sharply.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reuters.com/business/finance/china-slows-humanoid-robot-ipo-rush-hype-outruns-reality-2026-09-21/">China slows humanoid robot IPO rush as hype outruns reality - Reuters</a></li>
<li><a href="https://eu.36kr.com/en/p/3915964898504326">Emotional Companion Robots Fail to Ease UBTECH Share Price ...</a></li>

</ul>
</details>

**Tags**: `#China`, `#humanoid-robots`, `#IPO-regulation`, `#CSRC`, `#embodied-AI`

---