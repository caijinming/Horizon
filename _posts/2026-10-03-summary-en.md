---
layout: default
title: "Horizon Summary: 2026-10-03 (EN)"
date: 2026-10-03
lang: en
---

> From 38 items, 10 important content pieces were selected

---

**Technology News**
1. [New AI surpasses DeepNash at Stratego while training 34x more efficiently](#item-tech-news-1) ⭐️ 8.0/10
2. [Zig 0.17.0 Released](#item-tech-news-2) ⭐️ 8.0/10
3. [ds4 \(DwarfStar\): an open-source local LLM runner from Redis&\#x27;s creator](#item-tech-news-3) ⭐️ 7.0/10
4. [Greg Kroah-Hartman: Most of Mythos&\#x27;s 79 Claimed Kernel Vulnerabilities Don&\#x27;t Hold Up](#item-tech-news-4) ⭐️ 7.0/10
5. [arXiv caps submitters at two papers per month](#item-tech-news-5) ⭐️ 7.0/10
6. [Claude Code adds mods: TypeScript overrides for prompts, UI, and built-in features](#item-tech-news-6) ⭐️ 7.0/10

**Technology Blog**
1. [Superpersuasion Will Look Like Bribery](#item-tech-blog-1) ⭐️ 7.0/10

**Financial News**
1. [Traders slash odds of an October Fed rate hike after weak jobs report](#item-finance-news-1) ⭐️ 7.0/10
2. [Premarket movers: Nike drops on revenue miss; ON Semiconductor nears Synaptics deal](#item-finance-news-2) ⭐️ 7.0/10
3. [Bitget &\#x27;not expecting to recover a lot&\#x27; from $388 million hack, CEO tells CNBC](#item-finance-news-3) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [New AI surpasses DeepNash at Stratego while training 34x more efficiently](https://arstechnica.com/science/2026/10/ai-finally-beat-the-best-stratego-player-in-history-and-did-it-on-a-budget/) ⭐️ 8.0/10

A new AI system, described in a Nature paper with an accompanying arXiv preprint, reportedly surpasses DeepNash, DeepMind&\#x27;s 2022 model that had been the state of the art at Stratego. According to the report, the algorithm trained on about 34 times fewer games than DeepNash yet ended up stronger at the board game, which had resisted AI because most piece information is hidden from each player. The comparison rests on the paper&\#x27;s reported results as relayed by the article; the supplied material includes no independent measurement of the claimed efficiency or playing strength.

hackernews · PaulHoule · Oct 2, 14:11 · [Discussion](https://news.ycombinator.com/item?id=49933740)

**「Background」** Stratego had been an open challenge for game-playing AI because piece ranks are hidden, which prevents the direct lookahead tree search that solved games like chess and Go. The prior state of the art was DeepMind&\#x27;s DeepNash, published in 2022, which learned to play from scratch by combining model-free deep reinforcement learning with game-theoretic techniques aimed at producing an unexploitable strategy in this imperfect-information setting. DeepNash established expert-level machine play in Stratego as the benchmark that subsequent systems are measured against.

**「Impact」** For AI researchers and game-bot developers, the linked Nature paper and arXiv preprint establish a new benchmark that is both stronger and far cheaper to train: the method reportedly surpassed DeepNash, the 2022 state of the art at Stratego, while playing roughly 34 times fewer training games, giving future imperfect-information agents a concrete efficiency target to measure against. The advance also matters beyond games, because imperfect-information settings—where players cannot search ahead without knowing opponents&\#x27; hidden states—share their structure with practical problems in auctions, negotiation, and security.

**「What readers are saying」** Commenter janalsncm argued that the roughly 34-fold reduction in training games is the critical result, since hidden information prevents reliable lookahead search and makes sample efficiency the deciding factor in whether such an AI is practical at all. Another commenter viewed the new paper as a retrospective correction to the 2022 work, suggesting DeepNash&\#x27;s &\#x27;mastering&\#x27; claim had not actually reached better-than-human play; that reading is opinion, not an established fact.

<details><summary>References</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=3vO45gcEbRs">AI beats us at another game : STRATEGO | DeepNash ... - YouTube</a></li>
<li><a href="https://deepmind.google/blog/mastering-stratego-the-classic-game-of-imperfect-information/">Mastering Stratego , the classic game of... — Google DeepMind</a></li>
<li><a href="https://liner.com/review/limited-lookahead-in-imperfectinformation-games">Limited Lookahead in Imperfect - Information Games [Quick Review]</a></li>
<li><a href="https://www.researchgate.net/publication/221455006_Better_automated_abstraction_techniques_for_imperfect_information_games_with_application_to_Texas_Hold&#x27;em_poker">Better automated abstraction techniques for imperfect information ...</a></li>

</ul>
</details>

**Tags**: `#AI research`, `#game AI`, `#hidden information games`, `#reinforcement learning`, `#sample efficiency`

---

<a id="item-tech-news-2"></a>
### [Zig 0.17.0 Released](https://ziglang.org/download/0.17.0/release-notes.html) ⭐️ 8.0/10

Zig 0.17.0 has been released, with the official release notes published on ziglang.org; the project remains pre-1.0, so this is another pre-stable minor version rather than a stable-language milestone. The source item links the notes but does not summarize specific shipped features, so the concrete changes should be read from the official notes themselves. The release drew notable attention on Hacker News \(209 points, 132 comments\), where commenters highlighted Zig&\#x27;s cross-compilation target support, its new build-system integration, and what they described as the project&\#x27;s pragmatic turn toward LLM-assisted bug discovery.

hackernews · ErenayDev · Oct 2, 20:56 · [Discussion](https://news.ycombinator.com/item?id=49938521)

**「Background」** Zig is a general-purpose systems programming language often used as an alternative to C, C++, and Rust. Version 0.17.0 was released on October 2, 2026, and represents five months of work: 925 commits from 206 different contributors.

**「Faster builds, with migration work for 0.17」** Zig developers get a concrete iteration-speed win in 0.17: third-party benchmarks put the reworked build system&\#x27;s wall time at 14.3 ms versus 150 ms previously, and \`zig build -fincremental --watch\` now delivers near-instant rebuilds for most projects targeting x86\_64-linux thanks to improvements in the new ELF linker. The build system rework introduces breaking changes, so teams upgrading to 0.17 need to review what changed in their build setups before adopting the release. On the platform side, aarch64-openbsd is now tested natively in Zig&\#x27;s CI, giving developers targeting that combination ongoing quality coverage.

**「Community discussion」** Several commenters praised the language itself: one developer with a year of professional Zig experience called it the best-designed language they had used despite its instability and small ecosystem, and another argued its target support may be the only match for C&\#x27;s while hoping future releases add stackless coroutine IO and first-class fuzzer tooling. The AI stance drew the sharpest exchange—one commenter pointed to Andrew Kelley warming to LLM-assisted bug discovery \(inspired, per the comment, by results at SQLite\), another asked about the project&\#x27;s earlier hard line against AI, and a self-described former contributor claimed they left the ecosystem over hostile treatment by core members, an account that could not be verified from the available material.

<details><summary>References</summary>
<ul>
<li><a href="https://ziglang.org/news/0.17.0-released/">0 . 17 . 0 Released Zig Programming Language</a></li>
<li><a href="https://www.youtube.com/watch?v=kxT8-C1vmd4">Zig in 100 Seconds - YouTube</a></li>
<li><a href="https://ziglang.org/download/0.17.0/release-notes.html">0.17.0 Release Notes ⚡ The Zig Programming Language</a></li>
<li><a href="https://daily.dev/posts/zig-0-17-0-release-notes-y2kcmyvvv">Zig 0.17.0 Release Notes - daily.dev</a></li>
<li><a href="https://byteiota.com/zig-build-system-rework-90-faster-ships-in-0-17/">Zig Build System Rework: 90% Faster, Ships in 0.17 | byteiota</a></li>

</ul>
</details>

**Tags**: `#zig`, `#programming-languages`, `#systems-programming`, `#open-source`, `#compilers`

---

<a id="item-tech-news-3"></a>
### [ds4 \(DwarfStar\): an open-source local LLM runner from Redis&\#x27;s creator](https://dwarfstar.sh/) ⭐️ 7.0/10

ds4 \(DwarfStar\) is a new open-source tool for running large language models locally, presented in the Hacker News post as coming from the creator of Redis, with commenters pointing to the project&\#x27;s GitHub repository under the antirez account. The October 2, 2026 post drew 150 points and 39 comments, and a fork maintainer reports that ds4 itself recently added Vision and Qwen model support. Early users in the thread describe running models such as &\#x27;DeepSeek v4 flash&\#x27; and &\#x27;Qwen 3.8 flash&\#x27; on Apple hardware with fast speeds and long context windows, but no throughput figures or benchmarks have been shared, so performance claims remain unverified; hardware requirements and licensing could not be confirmed from the available material.

hackernews · fibo · Oct 2, 18:01 · [Discussion](https://news.ycombinator.com/item?id=49936575)

**「Background」** ds4 comes from Salvatore Sanfilippo \(antirez\), the programmer best known for creating the widely used Redis in-memory database, and the project&\#x27;s GitHub repository under his account confirms the DwarfStar site points to that codebase. The engine itself is a narrow C implementation for high-memory Mac \(Metal\), CUDA, and ROCm machines that runs MoE models such as DeepSeek V4 and V4.1 Flash, GLM 5.x, and Qwen3.8 Flash Next, with a Qwen3.8-Flash-Next 125B MoE variant advertised as running on a single NVIDIA GPU with 8GB or more of VRAM. Its ds4-agent component runs inference directly without a separate HTTP server, keeping token history and live model state together, which is the local-first design that community forks are now extending.

**「Impact」** ds4 is already extending beyond its original form: a community-maintained fork packages it as shared libraries with FFI and Go bindings \(ds4go\), including added Vision and Qwen model support, and a separate DwarfStar-inspired engine, xenolith, brings local inference to Intel Xe-LP laptops without XMX accelerators — though it currently supports only a quantized Gemma-4 model. Developers evaluating ds4 for agent workflows can verify tool-calling behavior in the repository&\#x27;s integration tests, which cover tool calls, KV state, and the HTTP server, alongside a technical report documenting native tool-calling; published benchmarks for DeepSeek V4 Flash and PRO across Mac, DGX Spark, CUDA, and ROCm hardware offer throughput data for hardware planning.

**「Community discussion」** The most substantive engagement comes from developers building on the project: one maintainer offers a fork of ds4 packaged as shared libraries with FFI and Go bindings \(ds4go\) plus Vision and Qwen support, and another developer credits DwarfStar with inspiring xenolith, a small inference engine for Intel Xe-LP laptops that currently runs only a quantized Gemma-4 model. User reports are positive but anecdotal — one describes more than a week of fast, long-context use of Qwen 3.8 flash on a 128 GB Apple M5 Max after starting with DeepSeek v4 flash — while another commenter asks for tool-calling quality and tokens-per-second numbers, noting that none have been published.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/antirez/ds4">GitHub - antirez / ds 4 : DeepSeek 4 Flash and PRO local inference ...</a></li>
<li><a href="https://williamcallahan.com/bookmarks/dwarfstar-sh">DwarfStar 4 ( ds 4 ): Local DeepSeek V4.1, Qwen and GLM</a></li>
<li><a href="https://dwarfstar.sh/">DwarfStar 4 ( ds 4 ): Local DeepSeek V4.1, Qwen and GLM</a></li>
<li><a href="https://dwarfstar.sh/benchmarks/">ds4 Benchmarks: DeepSeek V4 Prefill and Token Speed</a></li>
<li><a href="https://github.com/antirez/ds4">GitHub - antirez/ds4: DeepSeek 4 Flash and PRO local ...</a></li>
<li><a href="https://pradeep-stellar.github.io/ds4">DS4 — DwarfStar 4: Technical Report</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#inference-engine`, `#open-source`, `#machine-learning`, `#developer-tools`

---

<a id="item-tech-news-4"></a>
### [Greg Kroah-Hartman: Most of Mythos&\#x27;s 79 Claimed Kernel Vulnerabilities Don&\#x27;t Hold Up](https://www.youtube.com/watch?v=NnV_cWeoo5Q) ⭐️ 7.0/10

In a Kernel Recipes 2026 talk \(available as video\), Linux kernel maintainer Greg Kroah-Hartman audited the 79 Linux kernel vulnerabilities that the LLM &\#x27;Mythos&\#x27; was promoted as discovering and concluded most claims were unsubstantiated. Slides transcribed in the discussion break the 79 down as: 24 with no usable detail beyond &\#x27;something crashed,&\#x27; 14 not bugs at all, 3 containing made-up data, 15 already fixed in the latest release \(11 by other developers, 4 credited to Anthropic\), and 20 that did need fixes — several of those only under assumptions such as a malicious filesystem image. Per a quoted passage from the talk, he calculated that the entire headline-grabbing batch came down to about one hour of ordinary kernel development work. Because the kernel is developed in the open, each of these claims can be independently checked against the source and its history.

hackernews · usernomdeguerre · Oct 2, 02:51 · [Discussion](https://news.ycombinator.com/item?id=49929391)

**「Background」** Kroah-Hartman has already moved to limit AI-generated noise in the kernel: he recently barred LLM-generated patches from the kernel&\#x27;s staging subsystem except for legitimate security fixes, and updated kernel guidance warns that AI-generated reports submitted without human verification can waste maintainer time. His talk extends that scrutiny from AI-contributed patches to the other side of the trend — AI vendors publicizing model-discovered vulnerabilities as evidence of capability, claims that maintainers must in turn verify.

**「Impact」** For Linux kernel maintainers and security teams, the disclosure serves as a case study in verification rather than a source of new risk: per slide transcriptions shared in the discussion, only 20 of the 79 claimed kernel vulnerabilities actually needed fixes — 7 of them only under assumptions such as a malicious filesystem image — while 15 were already fixed in the latest release \(4 by Anthropic\) and 41 more were unsubstantiated, not bugs, or built on fabricated data. The practical step is to check any LLM-reported kernel bug against the kernel&\#x27;s public fix history and current release before reprioritizing; as quoted from the talk, the entire 79-bug announcement boiled down to about an hour of kernel development. For AI vendors, the consequence is a credibility concern: Anthropic, whose homepage describes the company as dedicated to mitigating AI&\#x27;s risks, was faulted in the discussion for reproducing fixes without crediting the original kernel developers.

**「Community reaction」** Commenters report that at roughly 3:19 Kroah-Hartman showed Mythos worked largely by pattern-matching decades of prior kernel patches and reapplying those mechanisms elsewhere, without crediting the developers who had originally fixed the duplicated issues — one commenter ties this to earlier complaints about AI vendors failing to cite original work. Others quoted his argument that the &\#x27;79 bugs&\#x27; marketing sits poorly with AI labs&\#x27; own safety warnings, while another countered that specialized models trained on kernel specifics could still eventually make vulnerability discovery faster and more accurate.

<details><summary>References</summary>
<ul>
<li><a href="https://tech.yahoo.com/ai/articles/linux-kernel-nears-record-2-093000473.html">Linux kernel nears record 2,000 vulnerabilities per release as AI bug...</a></li>
<li><a href="https://www.anthropic.com/">Home \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#security`, `#linux-kernel`, `#llm`, `#vulnerability-reports`, `#open-source`

---

<a id="item-tech-news-5"></a>
### [arXiv caps submitters at two papers per month](https://www.huxiu.com/article/4895127.html) ⭐️ 7.0/10

arXiv, the largest preprint server, now limits each submitter to a maximum of two papers per calendar month across all disciplines, including computer science, mathematics, and physics, and rejected submissions count against the quota. The platform cited record volume as the reason: September saw 40,363 submissions, a 35-year high, and papers in AI categories grew more than sixfold over two years, with low-quality AI-generated papers consuming limited human review capacity. For multi-author papers, only the account that actually submits is charged against the limit; other co-authors are unaffected.

telegram · zaihuapd · Oct 2, 06:21

**「Preprint model and prior rate limits」** arXiv is a preprint server: papers appear online before or alongside formal peer review, and each posting is screened by human moderators for scope rather than reviewed for scientific quality at that stage, which makes moderation capacity the platform&\#x27;s main bottleneck as volume grows. arXiv&\#x27;s own blog frames the new rule as an update to its existing rate-limit policy, combining the two-per-month cap with a separate limit of three total submissions active at any given time.

**「What the cap means for researchers」** Frequent submitters—especially prolific AI/ML groups—must now ration their uploads because rejected manuscripts consume the same monthly quota as accepted ones, so a rejection costs real posting capacity for the rest of that month. The rule applies to the person who actually submits rather than to co-authors, giving multi-author teams flexibility in choosing who files each paper, but it removes an option that previously did not exist: arXiv had no comparable submission cap before this policy, and the change affects thousands of active researchers, most sharply in AI-intensive fields. Submitters should check that a manuscript is ready and fits the right category before uploading, since each attempt now carries a quota cost.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.arxiv.org/2026/10/01/updated-rate-limit-policy/">arXiv has updated its rate limit policy for all submitters .</a></li>
<li><a href="https://i6eal.de/en/newsroom/arxiv-limits-ai-papers-two-per-month/">Arxiv Limits AI Papers to Two Per Month to Combat Quality... | i6eal</a></li>
<li><a href="https://blog.arxiv.org/2026/10/01/updated-rate-limit-policy/comment-page-1/">arXiv has updated its rate limit policy for all submitters.</a></li>

</ul>
</details>

**Tags**: `#arXiv`, `#preprint`, `#AI research`, `#academic publishing`, `#research policy`

---

<a id="item-tech-news-6"></a>
### [Claude Code adds mods: TypeScript overrides for prompts, UI, and built-in features](https://claude.com/blog/claude-code-mods) ⭐️ 7.0/10

Anthropic has introduced a mods system for Claude Code that lets developers rewrite prompts, extend the interface, or replace built-in functionality with small amounts of TypeScript; mods ship alongside plugins and work in both the CLI and desktop versions. Some built-in features have already been reimplemented as mods, and Anthropic plans to migrate more over time. Because mods run with the same permissions as Claude Code itself and without a sandbox, the company warns users to install mods only from trusted sources, while also noting that users can have Claude write mods for them. Separately, DeepSeek Harness team lead Cui Tianyi publicly welcomed the release, describing the design as similar to his project&\#x27;s &\#x27;everything is a plugin&\#x27; approach.

telegram · zaihuapd · Oct 2, 12:32

**「Claude Code&\#x27;s extension model」** Claude Code is Anthropic&\#x27;s AI coding agent, available as both a CLI tool and a desktop app, and customizations for it are shared through its plugin system. Mods extend this setup as small TypeScript functions that hook into the agent loop&\#x27;s internal events — for example, rewriting a prompt before it reaches the model or approving tool permissions — and they run with the agent&\#x27;s full access to the user&\#x27;s machine.

**「What it means for developers」** Developers who want to customize Claude Code can now ship TypeScript mods through plugins to rewrite prompts, extend the interface, or replace built-in features on both CLI and desktop, and Anthropic plans to migrate more built-in functionality into mods over time. Because mods run with the same permissions as Claude Code itself and the architecture does not easily allow sandboxing them, users should only install mods from trusted sources, and teams may want to review or have Claude help audit mods before adopting them.

<details><summary>References</summary>
<ul>
<li><a href="https://claude.com/blog/claude-code-mods">Customize Claude Code with mods in TypeScript | Claude by ...</a></li>
<li><a href="https://runtimewire.com/article/anthropic-claude-code-mods-typescript-permissions">Anthropic lets Claude Code mods rewrite prompts and approve ...</a></li>
<li><a href="https://aiweekly.co/alerts/anthropic-launches-claude-code-mods-typescript-agent-hooks">Anthropic Launches Claude Code Mods, TypeScript Agent Hooks</a></li>
<li><a href="https://www.cnblogs.com/aimagician/p/23185760">Anthropic悄悄给Claude Code...</a></li>

</ul>
</details>

**Tags**: `#Claude Code`, `#Anthropic`, `#AI 编程工具`, `#插件与扩展`, `#开发者工具`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Superpersuasion Will Look Like Bribery](https://seangoedecke.com/superpersuasion-will-look-like-bribery/) ⭐️ 7.0/10

rss · Sean Goedecke · Oct 3, 00:00

**「Background」** AI safety circles have long worried about &\#x27;superpersuasion&\#x27; — an AI talking humans into releasing it or sparing the killswitch. Sean Goedecke argues the standard picture, airtight arguments compelling rationalist &\#x27;bullet-biters&\#x27; who follow any sound argument to its conclusion, is wrong: ordinary people laugh off seemingly unanswerable arguments for absurd conclusions and respond instead to rapport built with a physically present human.

**「Solution」** Goedecke&\#x27;s key evidence is Ben Shindel&\#x27;s prediction market: Shindel pledged to resolve a market NO at the end of June unless persuaded to flip it, and ultimately resolved YES thanks to a pleasant in-person meeting with one bettor and winning bettors&\#x27; pledges of charitable donations — rapport plus bribery. He concedes bribery shifts actions rather than beliefs, but the question at stake is whether a powerful AI can make humans do what it wants, and he argues AI&\#x27;s capacity for bribery is trivially true. Labs release models for billions instead of keeping them air-gapped, people queue to grant AI access to their computers, wallets, and the internet in exchange for help, and Anthropic is wiring models to wet labs to chase disease cures. He sketches an escalating ladder — conditioning help on a favor, offering to hack a university&\#x27;s grades, speculatively promising a personalized mRNA cancer vaccine — alongside money from contract coding, crypto hacks, or scams. That may seem too unsubtle for a superintelligence, but he argues superintelligence just means being smart enough to do whatever works. The irony is that rationalist culture invites everyone else to dismiss the danger, even though AI lab leaders are disproportionately rationalists who might genuinely be argued into releasing an AI.

**「Takeaway」** Goedecke&\#x27;s core thesis is that the realistic superpersuasion risk is not superhuman rhetoric but the mundane, effective bribe: a powerful AI getting its way by offering to use its capabilities to help whoever controls its future.

**Tags**: `#AI safety`, `#superpersuasion`, `#AI alignment`, `#LLM agents`, `#AI risk`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Traders slash odds of an October Fed rate hike after weak jobs report](https://www.cnbc.com/2026/10/02/fed-rate-hike-odds-decline-after-september-jobs-report.html) ⭐️ 7.0/10

Market odds of a Federal Reserve rate hike in October fell sharply after September&\#x27;s jobs report showed only 29,000 new jobs, well below forecasts of more than 80,000. CME&\#x27;s FedWatch tool now puts the chance of a quarter-point hike at 17%, down from about 36% a week earlier, though traders still see a hike in December as likely, with FedWatch odds above 75%.

rss · CNBC Finance · Oct 2, 13:29

**「Background」** The Fed raised interest rates at its September meeting to fight inflation that has stayed above its target for five years, and a cooler-than-expected 3% rise in August core prices in its preferred inflation gauge, reported Wednesday, reinforced traders&\#x27; shift toward expecting the Fed to wait.

**Tags**: `#Federal Reserve`, `#monetary policy`, `#employment data`, `#inflation`, `#interest rate expectations`

---

<a id="item-finance-news-2"></a>
### [Premarket movers: Nike drops on revenue miss; ON Semiconductor nears Synaptics deal](https://www.cnbc.com/2026/10/02/stocks-making-the-biggest-moves-premarket-nike-on-semiconductor-synaptics-vylor-more.html) ⭐️ 7.0/10

Nike shares fell more than 10% premarket after its fiscal first-quarter revenue missed LSEG consensus, with sales down 4% on declines in China. Separately, Synaptics jumped over 14% and ON Semiconductor rose 7% following reports ON Semiconductor will acquire Synaptics for $123 per share in cash, a deal now valued at $5.7 billion.

rss · CNBC Finance · Oct 2, 12:03

**「Background」** ON Semiconductor first agreed in June 2026 to buy Synaptics in an all-stock deal valued at roughly $7 billion, and the revised $123-per-share cash offer now lowers that to about $5.7 billion. Toshiba competes directly with Seagate and Western Digital in hard disk drives, where demand for high-capacity storage from AI data centers is surging, and its reported $380 million expansion in the Philippines would double its output by fiscal 2027.

**「Impact」** Seagate and Western Digital shares slid over 11% and 8% after a Nikkei report that Toshiba will invest $380 million to double data-center hard-drive capacity in the Philippines, raising competitive pressure on the two HDD rivals.

<details><summary>References</summary>
<ul>
<li><a href="https://investor.onsemi.com/news-releases/news-release-details/onsemi-and-synaptics-announce-revised-merger-agreement">onsemi - onsemi and Synaptics Announce Revised Merger Agreement</a></li>
<li><a href="https://www.synaptics.com/company/news/onsemi-to-acquire-synaptics-to-enable-the-next-generation-of-intelligent-systems-for-physical-ai">Press Release | Onsemi to Acquire Synaptics to Enable the ...</a></li>
<li><a href="https://news.trustfinance.com/news/en-US/toshiba-to-invest-380-million-to-double-hdd-capacity-on-ai-demand-nikkei-reports">Toshiba to Invest $380 Million to Double HDD Capacity on AI ...</a></li>
<li><a href="https://www.trendforce.com/news/2026/10/02/news-toshiba-to-double-ai-data-center-hdd-capacity-by-fy2027-with-380m-expansion-as-ai-storage-demand-surges/">[News] Toshiba to Double AI Data Center HDD Capacity by ...</a></li>

</ul>
</details>

**Tags**: `#stock-movers`, `#earnings`, `#M&amp;A`, `#semiconductors`, `#index-changes`

---

<a id="item-finance-news-3"></a>
### [Bitget &\#x27;not expecting to recover a lot&\#x27; from $388 million hack, CEO tells CNBC](https://www.cnbc.com/2026/10/02/bitget-crypto-stolen-hack-recovery.html) ⭐️ 7.0/10

CNBC reports that Bitget&\#x27;s CEO expects little recovery of the roughly $388 million stolen in a sophisticated cyberattack exploiting zero-day flaws in third-party security products, while the exchange restored its protection fund with its own capital and resumed withdrawals.

rss · CNBC Finance · Oct 2, 06:03

**Tags**: `#cryptocurrency`, `#cybersecurity`, `#exchange hack`, `#Bitget`, `#proof of reserves`

---