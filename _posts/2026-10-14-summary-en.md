---
layout: default
title: "Horizon Summary: 2026-10-14 (EN)"
date: 2026-10-14
lang: en
---

> From 51 items, 12 important content pieces were selected

---

**Technology News**
1. [Google DeepMind launches Gemini 4 Argon with a robotics-focused variant](#item-tech-news-1) ⭐️ 9.0/10
2. [Anthropic replaces Git with custom Scion system as AI drives 30,000 daily merges](#item-tech-news-2) ⭐️ 8.0/10
3. [Apple announces HomeView smart display with A18 Secure Exclaves and no App Store](#item-tech-news-3) ⭐️ 7.0/10
4. [11-year-old soundness bug surfaces in Rust&\#x27;s borrow checker](#item-tech-news-4) ⭐️ 7.0/10
5. [Mozilla Pitches Firefox Enterprise to Businesses with Management and Security Controls](#item-tech-news-5) ⭐️ 7.0/10
6. [Apple ML Research Proposes Virtual GPU Cloud from Idle Apple Silicon Devices](#item-tech-news-6) ⭐️ 7.0/10
7. [Character.ai files for Chapter 11 as Disney moves to buy assets and hire CEO](#item-tech-news-7) ⭐️ 7.0/10

**Financial News**
1. [SFC suspends ChaPanda trading over suspected IPO fraud](#item-finance-news-1) ⭐️ 8.0/10
2. [JPMorgan Chase keeps outside AI agents blocked from transacting on customer accounts](#item-finance-news-2) ⭐️ 7.0/10
3. [Fed&\#x27;s Hammack says higher rates may be needed to keep inflation expectations anchored](#item-finance-news-3) ⭐️ 7.0/10
4. [Global Smartphone Shipments Fall 20% in Q3 2026; Apple Posts Record Q3 Share](#item-finance-news-4) ⭐️ 7.0/10
5. [LVMH Says Molly Tea Trademark Dispute Weighed on Q3 as Chinese Demand Fell 15%](#item-finance-news-5) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Google DeepMind launches Gemini 4 Argon with a robotics-focused variant](https://deepmind.google/models/gemini/) ⭐️ 9.0/10

Google DeepMind launched its Gemini 4 Argon model on October 13, 2026, with a companion &quot;Gemini 4 Argon for Robotics&quot; announcement submitted in a parallel thread. Pricing quoted from the launch post puts API access at an introductory rate of $2 per million input tokens and $10 per million output tokens, with cached input tokens 95% off; the standard price after the introductory period was not disclosed. Early Hacker News commenters report strong prose quality, structured reasoning, and a tendency to build interactive, tweakable simulations, but these are individual impressions — the supplied launch page contains no benchmarks or specifications, so the claimed improvements are not independently verified.

hackernews · 737max · Oct 13, 16:03 · [Discussion](https://news.ycombinator.com/item?id=50073879)

**「Background」** Gemini 4 Argon is the newest model in Google DeepMind&\#x27;s Gemini family of frontier large language models, announced alongside a separate Gemini 4 Argon for Robotics variant that the source links with the main release. Third-party guides compiled from Google&\#x27;s first-party materials describe a phased rollout through a program called the Fairwind Program, a 1-million-token output limit, and introductory pricing, while noting that some capabilities are still missing from the public API. The benchmark results published so far are figures reported by Google DeepMind itself on its own evaluation pages rather than independently measured, so the scale of the model&\#x27;s improvement remains vendor-claimed for now.

**「Impact」** Developers evaluating frontier APIs get a new option at an introductory price of $2 per million input tokens and $10 per million output tokens, with cached input tokens 95% discounted — but Google has not stated the post-introductory price or when it takes effect, so teams should not assume current rates will persist. Independent evaluations characterized the model as a competitive frontier entrant rather than a benchmark redefinition, reportedly placing first or tied in 13 of 18 standardized tests against GPT-6 Astra and Claude Opus 5.5, and one report says initial access ran through a controlled testing program rather than an immediate general release, so organizations should verify capability claims and availability on their own workloads before migrating.

**「Community Discussion」** Several commenters report favorable first experiences: svara calls the model &quot;a clear step change&quot; in clarity and logical structure, and postalcoder praises its writing quality when used via the API. Others criticized the rollout, with damsta objecting that the launch post buries the post-introductory pricing and I\_am\_tiberius describing payment failures and confusion across Google&\#x27;s AI Studio, Antigravity, and AI Ultra offerings.

<details><summary>References</summary>
<ul>
<li><a href="https://kingy.ai/blog/gemini-4-argon-specs-benchmarks-pricing/">Gemini 4 Argon : Specs , Benchmarks , Pricing ... - Kingy AI</a></li>
<li><a href="https://agentpedia.codes/blog/gemini-4-argon-complete-guide">Gemini 4 Argon : Complete Guide to Benchmarks , Pricing and...</a></li>
<li><a href="https://www.cometapi.com/models/google/gemini-4-argon/">Gemini 4 Argon API - Access Google Gemini 4 Argon at Best Price</a></li>
<li><a href="https://hypothesiswire.com/articles/google-s-gemini-4-argon-rejoins-the-frontier-but-independent-tests-temper-the-cl-4d79acc5">Gemini 4 Argon : Frontier Model Returns, But Independent Tests...</a></li>
<li><a href="https://aiarabai.com/en/google-gemini-4-argon/">Google Unveils Gemini 4 Argon , Its New Frontier AI Model</a></li>
<li><a href="https://www.remio.ai/post/gemini-4-argon-launches-behind-closed-doors-putting-googles-benchmark-lead-on-tr">Gemini 4 Argon Launches Behind Closed Doors, Putting...</a></li>

</ul>
</details>

**Tags**: `#artificial intelligence`, `#large language models`, `#Google DeepMind`, `#machine learning`, `#robotics`

---

<a id="item-tech-news-2"></a>
### [Anthropic replaces Git with custom Scion system as AI drives 30,000 daily merges](https://simonwillison.net/2026/Oct/13/redesigning-source-control-at-anthropic/) ⭐️ 8.0/10

Anthropic has replaced Git for its monorepo with Scion, a custom centralized source control system built by a seven-person team and migrated in five months, after the company&\#x27;s own engineering write-up reported merged changes growing from roughly 2,500 per day in May 2026 to over 30,000 per day by September. The scale strained Git&\#x27;s design: the main branch history alone is almost 100 GB, and the roughly 25 million daily CI checkouts would amount to over 600 PB of git traffic if fetched naively. Simon Willison reads Scion as a reinvention of centralized version control in the Subversion mold, paired with a new code review system called Antique that has largely replaced pull requests, and notes it deliberately lacks offline support because Claude — by far the heaviest user — is necessarily online. Annotating Anthropic&\#x27;s merge chart with 2026 model release dates, Willison speculates that the Fable/Mythos model class is a key factor in the acceleration, while cautioning that public release dates don&\#x27;t show when the models reached internal use.

rss · Simon Willison · Oct 13, 23:00

**「Background」** Git, the version control system Anthropic replaced, is a distributed design: every clone carries the project&\#x27;s full history, and its workflow assumes changes are authored, merged, and reviewed at a human pace. Anthropic had kept all of its code in a single Git-based monorepo, whose main-branch history alone had grown to nearly 100 GB. Simon Willison observes that the replacement, Scion, resembles a return to centralized version control along the lines of Subversion, in which history lives on a server rather than in each developer&\#x27;s copy.

**「Impact」** Engineering organizations scaling AI-assisted development now have a concrete benchmark for when Git&\#x27;s distributed model stops holding up: Anthropic hit the wall at roughly 100 GB of main-branch history, 25 million daily CI checkouts, and a jump from about 2,500 to over 30,000 merged changes per day, thresholds other teams can use to decide whether to evaluate centralized alternatives — such as the open-source Mega monorepo server or git-branchless high-velocity workflows — before committing to a custom five-month migration. The compatibility trade-off is also instructive: Scion shipped with no offline support because Claude, an always-online agent, is its heaviest user, a design choice teams whose human developers work locally or intermittently offline could not make as easily.

**「Community discussion」** In the Hacker News thread, one commenter argued Anthropic should have first questioned the monorepo itself — moving from &\#x27;monorepo makes merging easier&\#x27; to &\#x27;redesign version control because merging is too hard&\#x27; skips the middle question — while another likened Scion to Epic Games&\#x27; Lore, an SVN/Perforce-style centralized VCS with no production use outside the company, no support for non-text assets, and no code release. Others highlighted a passage quoted from Anthropic&\#x27;s write-up describing how an early internal Claude Mythos Preview snapshot rewrote the hand-written git-to-Scion ingestion pipeline to use 20x less memory and run 4x faster with no further instructions.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/gitmono-dev/mega">GitHub - gitmono-dev/mega: Mega is an open-source implementation...</a></li>
<li><a href="https://www.graphcanon.com/tools/arxanas-git-branchless">git -branchless - High-velocity monorepo - scale workflow for...</a></li>

</ul>
</details>

**Tags**: `#version-control`, `#git`, `#anthropic`, `#ai-assisted-development`, `#developer-tooling`

---

<a id="item-tech-news-3"></a>
### [Apple announces HomeView smart display with A18 Secure Exclaves and no App Store](https://www.apple.com/apple-homeview/) ⭐️ 7.0/10

Apple has announced HomeView, a smart-home display powered by an A18 chip containing &quot;Secure Exclaves&quot; that, according to Apple&\#x27;s product page, process camera and microphone feeds in a compartment inaccessible to the operating system and to Apple, allowing the device to recognize each user&\#x27;s face and voice without exposing the underlying audio and video. The announcement drew heavy Hacker News discussion, where commenters also flagged that the device offers no App Store support and no battery. The isolation claims come from Apple&\#x27;s own promotional page rather than independent testing, so they should be treated as vendor claims.

hackernews · etothet · Oct 13, 13:02 · [Discussion](https://news.ycombinator.com/item?id=50071017)

**「Background」** HomeView is Apple&\#x27;s first dedicated smart-home display: Macworld describes a 7-inch touchscreen device with speakers, a camera, and Siri AI designed to sit at the center of the connected home. Apple&\#x27;s announcement frames the product around entertainment, FaceTime calls, home monitoring, and hands-free voice automations, with face and voice recognition handled on-device. MacRumors reports the hub was introduced in October 2026 at $299 with Apple Intelligence support, covering a screen-based home-control category Apple had not previously addressed with its own hardware.

**「Impact」** For buyers, the immediate constraint raised in early discussion is that HomeView runs no third-party App Store apps, so households that rely on services like Messenger or Snapchat for video calls or Plexamp for music — examples one commenter gave — would need to verify that the built-in software covers their routines before replacing a mounted tablet. If Apple&\#x27;s description holds up, per-user face and voice recognition would be walled off from both the OS and Apple itself, a stronger isolation boundary than typical smart-home displays that process audio and video through the operating system.

**「Community discussion」** On Hacker News \(663 points, 779 comments\), a recurring argument held that HomeView&\#x27;s &quot;biggest competitor is an old iPad,&quot; which offers a battery, a mounting ecosystem, and App Store access the new display lacks. Other commenters called the Secure Exclaves camera and microphone isolation the most technically interesting part, and one argued the heavy cynicism is itself a sign the product will be a hit.

<details><summary>References</summary>
<ul>
<li><a href="https://www.apple.com/newsroom/2026/10/meet-apple-homeview-a-new-way-to-enjoy-entertainment-and-manage-the-home/">Meet Apple HomeView, a new way to enjoy entertainment and ...</a></li>
<li><a href="https://www.macworld.com/article/676817/new-homeview-homepod-mini-screen-rumours-release-date.html">Apple HomeView guide: Price, release date, features, and ...</a></li>
<li><a href="https://www.macrumors.com/roundup/apple-homeview/">Apple HomeView: Everything We Know | MacRumors</a></li>

</ul>
</details>

**Tags**: `#apple`, `#smart-home`, `#hardware`, `#security`, `#privacy`

---

<a id="item-tech-news-4"></a>
### [11-year-old soundness bug surfaces in Rust&\#x27;s borrow checker](https://github.com/rust-lang/rust/issues/164250) ⭐️ 7.0/10

A soundness bug that has existed in Rust&\#x27;s borrow checker for roughly 11 years was brought to broad attention via compiler issue rust-lang/rust\#164250, drawing 676 points and 375 comments on Hacker News. Because the compiler has been accepting code that Rust&\#x27;s existing lifetime rules already prohibit, commenters characterize the flaw as a compiler implementation bug rather than a defect in the type system itself, meaning a fix means making the compiler reject the code rather than changing lifetime rules. The finding carries weight for a language whose core promise is memory safety, and it is not an outlier: more than 100 issues are currently labeled unsound in the Rust repository, some of them long-standing. Whether real-world crates actually depend on the erroneous acceptance, and would stop compiling once the bug is fixed, remains an open question.

hackernews · formerly\_proven · Oct 13, 10:27 · [Discussion](https://news.ycombinator.com/item?id=50069499)

**「What soundness means in Rust」** Rust&\#x27;s type system is intended to guarantee that safe code—anything written without an \`unsafe\` block—cannot cause memory unsafety, so an &\#x27;unsoundness&\#x27; bug means the compiler wrongly accepts safe-looking code that can violate that guarantee. In this case, issue \#164250 lets an assignment through a covariant struct field bypass the struct&\#x27;s declared lifetime bounds, producing a use-after-free with no unsafe code anywhere, and the compiler has accepted the pattern since Rust 1.4.0 in 2015—roughly 4,001 days on stable, reproduced on 1.99.0.

**「Impact」** Because the flaw is in the compiler rather than Rust&\#x27;s type system, the expected fix is simply to make rustc reject code its lifetime rules already forbid, meaning any program that unknowingly relied on this unsoundness could stop compiling after a toolchain update — a compatibility risk maintainers should watch for when the patch lands. As commenters on the thread note, it is not yet known whether any real-world crates actually depend on the bug, and this issue is one of more than 100 already labeled unsound in Rust&\#x27;s tracker, though the upcoming trait solver is expected to unblock fixes for some of the others.

**「Community discussion」** GrantMoyer argues the bug should be easy to fix because the compiler should have been rejecting the affected code under Rust&\#x27;s existing lifetime rules all along, while weinzierl notes that over 100 unsound issues are already tracked and that the new trait solver may unblock fixes for some of them, though probably not this one. Eridrus contends such soundness bugs often circulate as gotchas without evidence of real-world impact, and says the revealing test will be whether fixing this one actually causes any crates to stop compiling.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/rust-lang/rust/issues/164250">11 year old unsoundness bugs found in Rust borrow checker</a></li>
<li><a href="https://braindetox.kr/en/posts/rust_borrow_checker_soundness_bugs_11_years_2026.html">Rust #164250: Borrow Checker Unsoundness Open Since 1.4</a></li>
<li><a href="https://www.solosoft.dev/post/rust-borrowck-covariant-field-assignment-unsoundness/">Rust Accepted This Safe-Looking Code for 4,001 Days ...</a></li>

</ul>
</details>

**Tags**: `#rust`, `#borrow-checker`, `#compiler-bugs`, `#type-systems`, `#memory-safety`

---

<a id="item-tech-news-5"></a>
### [Mozilla Pitches Firefox Enterprise to Businesses with Management and Security Controls](https://www.firefox.com/en-US/enterprise/) ⭐️ 7.0/10

Mozilla is publicizing Firefox Enterprise, an offering pitched at organizations that need centralized management and security controls when deploying Firefox, as the company seeks business adoption in a browser market dominated by Chrome. The Hacker News discussion \(645 points, 262 comments at posting\) treated the move as overdue: one commenter cited enterprise browser vendor Island&\#x27;s $400 million Series F raise at a $6.4 billion valuation as evidence of demand for capabilities such as data-loss prevention \(including blocking copy-paste of sensitive data into AI chat apps\) and VPN-less access to private intranet apps, while judging Mozilla very far behind in that race. Other commenters said large businesses commonly ban Firefox outright because it lacks such controls, which limits both its workplace presence and day-to-day testing by developers.

hackernews · recvonline · Oct 13, 12:00 · [Discussion](https://news.ycombinator.com/item?id=50070302)

**「Firefox&\#x27;s enterprise gap」** Managing browsers across a workplace typically requires centralized policy controls and data loss prevention \(DLP\), which lets IT departments restrict actions such as copying, downloading, or pasting sensitive data from managed devices. Firefox has trailed Chrome and Edge in providing these hooks, which is why several commenters in the discussion said their employers ban or restrict installing it on work machines. Mozilla has been building toward this capability: its bug tracker documents ongoing work on Firefox support for DLP products through the Content Analysis SDK, covering DLP-related prompts, warnings, and performance.

**「Impact」** Organizations that currently ban Firefox for lacking central management have a supported path to deploy it instead, since Firefox Enterprise provides enterprise policies and security controls such as data-loss prevention that address the stated reason many companies prohibit installation. IT teams considering a rollout should plan for user friction: commenters reporting firsthand IT experience say employees try to install Chrome regardless of approved software and submit help-desk tickets claiming their computer is broken or offline, so administrators may need to update both software-installation policies and support workflows alongside any managed Firefox deployment.

**「Community reaction」** Commenters split between seeing a large opportunity and explaining why enterprises currently exclude Firefox: one argued the enterprise browser market is proven by Island&\#x27;s fundraising while Mozilla lags badly, and others reported that their employers ban or are actively phasing out Firefox for lacking these controls. An IT worker added a practical caveat, predicting that even successful rollout would bring ticket queues full of non-technical users insisting their machines are broken because Chrome is not installed.

<details><summary>References</summary>
<ul>
<li><a href="https://bugzilla.mozilla.org/show_bug.cgi?id=1876616">1876616 - Figure out if we can use DLP as a signal for enterprise</a></li>

</ul>
</details>

**Tags**: `#firefox`, `#browsers`, `#mozilla`, `#enterprise-software`, `#open-source`

---

<a id="item-tech-news-6"></a>
### [Apple ML Research Proposes Virtual GPU Cloud from Idle Apple Silicon Devices](https://machinelearning.apple.com/research/distributed-gpu-cloud) ⭐️ 7.0/10

Apple&\#x27;s machine learning research group has published a proposal for a dynamic, distributed virtual GPU cloud that pools idle Apple Silicon devices into shared compute for AI workloads. The material is a research publication on Apple&\#x27;s Machine Learning Research site, not a product announcement, and no deployed service or availability timeline is indicated. With only the paper&\#x27;s page and community reaction supplied, its specific mechanisms and measured results remain unverified here.

hackernews · acossta · Oct 13, 12:26 · [Discussion](https://news.ycombinator.com/item?id=50070593)

**「Background」** Mac computers with Apple silicon already work as local AI machines: Apple&\#x27;s MLX library lets M1- and M2-based systems fine-tune large language models, including 7B-parameter ones, on-device at low cost. On the other side sits an established datacenter market where developers rent GPU capacity by the second on chips like the NVIDIA H100 and A100, billed across dedicated pods, serverless inference, or multi-node clusters. The proposal is therefore best understood as an attempt to pool that existing on-device capability from idle machines into a shared alternative to rented datacenter GPUs.

**「Impact」** Apple&\#x27;s paper is a research proposal rather than a shipped service, so its immediate relevance is as a blueprint: organizations with fleets of idle Apple Silicon Macs could run delay-tolerant inference — overnight batch jobs or analytics — on hardware they already own instead of renting data-center GPUs, an approach one commenter summarizes as running inference &quot;in the off-hours on the machines that you already have.&quot; Commercial precedent already exists for this model: distributed platforms that tap idle consumer PCs and GPUs for inference workloads have launched, potentially letting hardware owners earn money from unused capacity \(tool-3-1, tool-3-2\). Commenters flag the economics as the open question — distributing tasks to idle desktops can cost more in energy than sending them to data centers, where power is cheaper and hardware more efficient — so practical adoption would likely favor workloads that tolerate scheduling delays.

**「Community Discussion」** Commenters split on practicality: mcculley argued that, as with SETI@home-style projects, distributing work to idle devices can cost more in energy than running it in data centers with cheaper power and more efficient hardware, while tom1337 saw value in companies running non-urgent inference on machines they already own but considered the technique unremarkable. yardie defended the concept as consistent with Apple&\#x27;s established practice, citing Grand Central Dispatch, distributed Final Cut Pro rendering, and Xcode&\#x27;s distributed CI/CD as precedents for harvesting idle Mac capacity.

<details><summary>References</summary>
<ul>
<li><a href="https://www.runpod.io/pricing">GPU Cloud Pricing | Per-Second H100, A100, RTX | Runpod</a></li>
<li><a href="https://www.linkedin.com/posts/chemistry-ai-machine-learning-applications_ai-machinelearning-applesilicon-activity-7476599007901954048-Ql8_">Fine-tune 7B LLM on Apple Silicon with MLX | Chemistry AI... | LinkedIn</a></li>
<li><a href="https://www.linkedin.com/posts/techstrongsemi_rent-out-your-idle-pc-for-ai-inference-workloads-activity-7503172940423688193-IFJo">Distributed AI Platforms Tap Home Computers for Inference Workloads</a></li>
<li><a href="https://thetechdata.com/aieev-launches-air-cloud-distributed-ai-inference-on-idle-gpus/">AIEEV Launches Air Cloud: Distributed AI Inference On Idle GPUs</a></li>

</ul>
</details>

**Tags**: `#distributed-computing`, `#apple-silicon`, `#ai-infrastructure`, `#gpu-cloud`, `#machine-learning`

---

<a id="item-tech-news-7"></a>
### [Character.ai files for Chapter 11 as Disney moves to buy assets and hire CEO](https://blog.character.ai/an-update-on-character-ai/) ⭐️ 7.0/10

Character.ai has filed for voluntary Chapter 11 bankruptcy, with the company announcing the move on October 13, 2026, roughly five years after the interactive chatbot platform launched. Reporting linked from the announcement, including a Reuters story, indicates Disney has agreed to buy some of the company&\#x27;s assets for about $20 million, and a statement from Character.ai&\#x27;s blog quoted in the discussion says CEO Karandeep Anand is joining Disney in a newly created role as Senior Executive Vice President and Chief Technology Officer, to be followed by members of Character&\#x27;s technical team. The filing comes two years after Google spent over $2 billion in 2024 to hire back co-founders Noam Shazeer and Daniel De Freitas along with much of the company&\#x27;s talent, per the linked coverage, so the bankruptcy proceeding concerns the remaining company rather than the team that originally built it. Because the item supplies only headlines, links, and comments rather than full article text, the exact terms of the Disney transaction should be treated as reported rather than confirmed.

hackernews · nryoo · Oct 13, 07:28 · [Discussion](https://news.ycombinator.com/item?id=50068036)

**「Background」** Character.ai was effectively hollowed out in August 2024, when Google paid roughly $2.7 billion to license its technology and bring back co-founders Noam Shazeer and Daniel De Freitas along with a group of researchers — a deal structured as a licensing arrangement and hires rather than an acquisition, which commenters note let Google sidestep antitrust review. What remained was an independent company without its founding team, which per commenters kept roughly 86 Bay Area employees and spent about $1 million per month while banning underage users who made up much of its audience. The Chapter 11 filing, Disney&\#x27;s reported ~$20 million bid for assets, and CEO Karandeep Anand&\#x27;s move to Disney as Chief Technology Officer close out that two-year aftermath.

**「What it means for users」** Character.ai&\#x27;s roughly 20 million monthly active users — half of them Gen Z or younger, averaging 75 minutes a day across millions of listed characters — face the most direct consequences, and the announcements cited here include no stated option for exporting data or preserving custom characters once the reported $20 million sale of some assets to Disney proceeds. Any continuation of the technology looks set to happen inside Disney, which has hired CEO Karandeep Anand as its first CTO along with members of Character.ai&\#x27;s technical team; notably, Disney had earlier accused Character.ai of &quot;blatantly infringing&quot; its copyrights and demanded removal of Disney characters from the platform, so bots built on licensed IP now fall under the rights holder&\#x27;s direct control.

**「Community reaction」** Commenters largely treated the filing as a foregone epilogue rather than a surprise: one argued the company was effectively acquired in August 2024 and that the entity entering Chapter 11 is the shell left after Google&\#x27;s antitrust-structured deal paid shareholders $2.7 billion and the founding team departed, while another took a moral view, calling the AI companion business predatory and citing reported scandals and suicides as grounds for personal executive accountability. Others pointed to the post-deal operation&\#x27;s burn rate, with one comment citing roughly $1 million in monthly spending across 86 Bay Area employees at about $278,000 average base pay plus nearly $100,000 owed to DoorDash, and noting that a prior ban on minors — which the same commenter calls probably most of the userbase — had already hollowed out the service.

<details><summary>References</summary>
<ul>
<li><a href="https://character.ai/">character . ai | AI Chat, Reimagined–Your Words. Your World.</a></li>
<li><a href="https://prinsessa.com/staysocial/character-ai-statistics-2026-20-million-people-75-minutes-a-day/">Character . AI Statistics 2026: 20 Million People, 75... - Prinsessa</a></li>
<li><a href="https://variety.com/2026/biz/news/disney-cto-karandeep-anand-character-ai-1236866528/?bt_ee=HolODr8Li/n+9lff65v/HBpdl3sKxI3noTHdwcglNQbOKVOM3F5hH7Qa+0jduAUv&amp;bt_ts=1789747455067">Disney Hires First CTO: Karandeep Anand , Former CEO of...</a></li>

</ul>
</details>

**Tags**: `#ai-industry`, `#character-ai`, `#bankruptcy`, `#disney`, `#business`

---

## Financial News

<a id="item-finance-news-1"></a>
### [SFC suspends ChaPanda trading over suspected IPO fraud](https://apps.sfc.hk/edistributionWeb/gateway/TC/news-and-announcements/news/doc?refNo=26PR168) ⭐️ 8.0/10

Hong Kong&\#x27;s Securities and Futures Commission said on October 13 that it is investigating two groups suspected of an IPO fraud scheme that created a false appearance of demand in ChaPanda&\#x27;s \(02555\) listing, and directed the stock exchange to suspend trading in the shares from 9 a.m. that day. The SFC also restricted asset disposals in related accounts, with a cap of HK$4.379 billion for the first suspected group — the highest for a case of its kind — and said the investigation, which could later lead to compensation orders for affected investors, is ongoing.

telegram · zaihuapd · Oct 13, 10:15

**「Background」** ChaPanda, a bubble-tea chain, listed on the Hong Kong stock exchange in 2024 but fell below its offer price at debut and has lost about 46% in roughly a year, lagging tea rivals such as Mixue and Guming. The SFC, Hong Kong&\#x27;s securities regulator, can direct the exchange to halt trading and restrict account dealings while it investigates suspected IPO \(a company&\#x27;s first public share sale\) fraud — here, two groups allegedly creating a false appearance of demand.

**「Who is affected」** ChaPanda&\#x27;s existing shareholders and IPO subscribers cannot buy or sell shares while the suspension lasts, and investors harmed by the suspected scheme may later receive compensation if the SFC orders responsible parties to pay.

<details><summary>References</summary>
<ul>
<li><a href="https://cj.sina.com.cn/articles/view/5973732618/1640fed0a00101f6aq?finpagefr=p_103">cj.sina.com.cn/articles/view/5973732618/1640fed0a00101f6aq?...</a></li>
<li><a href="https://www.hstong.com/news/hk/detail/25040314122719089">hstong.com/news/hk/detail/25040314122719089</a></li>

</ul>
</details>

**Tags**: `#香港证监会`, `#茶百道`, `#IPO操纵`, `#停牌`, `#市场监管`

---

<a id="item-finance-news-2"></a>
### [JPMorgan Chase keeps outside AI agents blocked from transacting on customer accounts](https://www.cnbc.com/2026/10/13/jpmorgan-ai-agents-account-access.html) ⭐️ 7.0/10

JPMorgan Chase will continue blocking outside AI agents from transacting on customer accounts, with CEO Jamie Dimon citing risks from &quot;rogue agents&quot; on the bank&\#x27;s third-quarter earnings call Tuesday. The bank permits read-only data access through connectors like Plaid, has no timeline for allowing direct agent transactions, and is piloting its own internal tool, Smart Cash.

rss · CNBC Finance · Oct 13, 20:48

**「Background」** JPMorgan previously fought fintech data middlemen such as Plaid over charging for access to customer data, a dispute that similarly pitted the bank&\#x27;s security concerns against tech firms&\#x27; demands for access. The regulatory backdrop remains unsettled: the Consumer Financial Protection Bureau&\#x27;s 2024 &quot;open banking&quot; rule, which would let consumers share their bank data with third-party apps for free, has been enjoined by a federal court and is being rewritten by the CFPB, including whether banks can charge fees for data access.

**「Impact」** External AI assistants like Meta&\#x27;s Muse and Instinct remain limited to viewing balances rather than paying bills or moving money, which also limits the deposit-outflow risk to banks that economists such as Apollo&\#x27;s Torsten Slok have flagged from agents shifting cash to higher-yield accounts.

<details><summary>References</summary>
<ul>
<li><a href="https://openbankingtracker.com/guides/section-1033-status">Section 1033 Status &amp; Timeline (2026): Is the Open Banking ...</a></li>
<li><a href="https://www.privacylawnetwork.com/news/cfpb-personal-financial-data-rights-rule.html">CFPB Section 1033 Rule: Text, Injunction and Status</a></li>

</ul>
</details>

**Tags**: `#JPMorgan Chase`, `#AI agents`, `#open banking`, `#fintech`, `#banking policy`

---

<a id="item-finance-news-3"></a>
### [Fed&\#x27;s Hammack says higher rates may be needed to keep inflation expectations anchored](https://www.cnbc.com/2026/10/12/beth-hammack-fed-inflation-policy.html) ⭐️ 7.0/10

Cleveland Fed President Beth Hammack, a voting member of the rate-setting committee, said Monday that a restrictive policy stance and further interest rate hikes are likely needed to return inflation to the central bank&\#x27;s 2% goal, warning that prices running above target for more than five years risk entrenching an &quot;inflationary mindset.&quot; Traders currently price about an 88% chance of a hike at the Fed&\#x27;s December meeting, per CME&\#x27;s FedWatch tool, after the personal consumption expenditures price index rose 3.4% year over year in August versus the 2% target.

rss · CNBC Finance · Oct 13, 02:58

**「Recent Fed policy and Hammack&\#x27;s stance」** The Federal Reserve raised interest rates last month for the first time in three years, while inflation has stayed above the central bank&\#x27;s 2% target for more than five years. Hammack has consistently favored tighter policy, having dissented in favor of a rate hike at the Fed&\#x27;s July meeting.

**「Impact」** If the Fed follows through with another hike, households and businesses with loans tied to short-term interest rates would face higher borrowing costs, though officials have not yet committed to a December move.

<details><summary>References</summary>
<ul>
<li><a href="https://www.clevelandfed.org/collections/speeches/2026/sp-20260731-statement-regarding-july-fomc-meeting-vote">Statement from Federal Reserve Bank of Cleveland president ...</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#inflation`, `#Beth Hammack`

---

<a id="item-finance-news-4"></a>
### [Global Smartphone Shipments Fall 20% in Q3 2026; Apple Posts Record Q3 Share](https://counterpointresearch.com/en/insights/global-smartphone-shipments-hit-a-new-low-with-20-percent-yoy-decline-lowest-in-14-years) ⭐️ 7.0/10

Global smartphone shipments fell 20% year over year in Q3 2026 to their lowest third-quarter level since 2012, hit by memory chip shortages and rising prices, according to Counterpoint Research. Samsung led with a 23% share while Apple&\#x27;s 22% was its highest third-quarter share on record, and IDC data put Apple second in China at 17.8%, behind Huawei&\#x27;s 21%.

telegram · zaihuapd · Oct 13, 14:49

**「Background」** The downturn extends a contraction already under way: Counterpoint Research had reported that global smartphone shipments fell 11% year over year in Q2 2026, the weakest second quarter since 2013, with Apple the only vendor to grow and Samsung keeping the top spot.

**「Impact」** The chip shortage is directly squeezing phone makers and shoppers: Apple launched only the iPhone 18 Pro series in September with no base model, leaving retail channels with less new stock than a year earlier even as Pro models sold well in China.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/news/story/smartphone-shipments-hit-a-13-year-low-last-quarter-8372761/">Smartphone shipments hit a 13-year low last quarter | LinkedIn</a></li>
<li><a href="https://www.androidauthority.com/counterpoint-research-q2-2026-smartphone-shipment-report-3686931/">Samsung wins Q2, but the smartphone market is... - Android Authority</a></li>
<li><a href="https://www.silicon.co.uk/mobility/smartphones/smartphone-q2-2026-contraction-630649">Smartphone Shipments Sink 11 Percent Worldwide | Silicon UK</a></li>

</ul>
</details>

**Tags**: `#smartphone-market`, `#memory-chip-shortage`, `#Apple`, `#Samsung`, `#market-share`

---

<a id="item-finance-news-5"></a>
### [LVMH Says Molly Tea Trademark Dispute Weighed on Q3 as Chinese Demand Fell 15%](https://www.nbd.com.cn/articles/2026-10-13/4603294.html) ⭐️ 7.0/10

LVMH&\#x27;s third-quarter 2026 report showed organic growth slowing to 1% from 3% in the second quarter, as demand from Chinese customers fell 15% and organic revenue in its core fashion and leather goods division declined 5%. The group for the first time acknowledged that its trademark dispute with Chinese jasmine-tea chain Molly Tea \(茉莉奶白\) had a negative impact early in the quarter — an effect its CFO called hard to quantify precisely — while saying it will keep investing in China.

telegram · zaihuapd · Oct 13, 15:19

**「Background」** The dispute stems from Louis Vuitton, LVMH&\#x27;s flagship brand, winning a trademark infringement lawsuit against the Chinese tea chain Molly Tea \(茉莉奶白\) in Suzhou, after which the case escalated into a wider public debate over intellectual property and cultural ownership.

**「Impact」** LVMH is closely watched as a bellwether for Chinese luxury spending, and with Asia excluding Japan its only declining region this quarter, the results underscore the pressure weak Chinese demand is placing on the luxury industry&\#x27;s most important growth market.

<details><summary>References</summary>
<ul>
<li><a href="https://dibarti.com/lv-v-molly-tea">LV v. Molly Tea Debate: Is another Chinese business being... | Dibarti</a></li>
<li><a href="https://www.tiktok.com/discover/mollytea-sued">Mollytea Sued | TikTok</a></li>

</ul>
</details>

**Tags**: `#LVMH`, `#luxury sector`, `#China consumer demand`, `#Q3 earnings`, `#trademark dispute`

---