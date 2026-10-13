---
layout: default
title: "Horizon Summary: 2026-10-13 (EN)"
date: 2026-10-13
lang: en
---

> From 42 items, 12 important content pieces were selected

---

**Technology News**
1. [Hackers force defrost cycles in European supermarket fridges via legacy controllers](#item-tech-news-1) ⭐️ 8.0/10
2. [w1700k-sdr: Turning a WiFi 7 Router into a 320 Msps SDR Receiver](#item-tech-news-2) ⭐️ 8.0/10
3. [Python 3.15 arrives with explicit lazy imports and a built-in sampling profiler](#item-tech-news-3) ⭐️ 8.0/10
4. [Building a Modern Web App in C with Pledge and Chroot Hardening](#item-tech-news-4) ⭐️ 7.0/10
5. [OpenAI&\#x27;s Codex CLI installs a self-updating background daemon by default](#item-tech-news-5) ⭐️ 7.0/10
6. [Meta Announces Muse Wonder AI Model; Testers Question Benchmark Claims](#item-tech-news-6) ⭐️ 7.0/10
7. [Looped Diffusion Transformer reruns shared blocks per denoising step with tunable depth](#item-tech-news-7) ⭐️ 7.0/10
8. [learnc auto-tunes constants in unmodified C code for smaller JPEGs and better VAD](#item-tech-news-8) ⭐️ 7.0/10

**Financial News**
1. [Fed&\#x27;s Hammack says further rate hikes may be needed to prevent entrenched inflation mindset](#item-finance-news-1) ⭐️ 7.0/10
2. [China and EU Reach Consensus on Hybrid and Electric Vehicle Trade](#item-finance-news-2) ⭐️ 7.0/10
3. [China Cuts New Energy Vehicle Export VAT Rebate From 13% to 9%](#item-finance-news-3) ⭐️ 7.0/10
4. [New tax penalty rules take effect Nov 1, with employer social insurance arrears fined up to 3x](#item-finance-news-4) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Hackers force defrost cycles in European supermarket fridges via legacy controllers](https://www.tomshardware.com/tech-industry/cyber-security/unprecedented-cyberattack-cripples-supermarket-fridges-across-europe-as-hackers-activate-automatic-defrosting-delivery-and-store-prices-also-impacted-by-incident) ⭐️ 8.0/10

Hackers activated automatic defrost cycles in internet-connected supermarket refrigeration systems across Europe, forcing refrigerators to shut down at French retailers including Intermarché, which reported roughly 150 stores targeted, according to Tom&\#x27;s Hardware coverage citing Reuters, BBC, and Le Monde. The incident caused perishable food loss and disrupted deliveries and store pricing at affected locations. Reporting and community analysis point to end-of-support Danfoss refrigeration controllers — a device class for which Claroty researchers have previously published vulnerabilities — as the suspected weak point, though the exact attack path and attribution remain unconfirmed.

hackernews · Zeekaas · Oct 12, 12:16 · [Discussion](https://news.ycombinator.com/item?id=50055304)

**「Networked controllers and known Danfoss flaws」** Commercial refrigeration controllers like Danfoss&\#x27;s are commonly connected to the internet for remote management, and the vendor itself promotes connectivity so service engineers can diagnose faults or start defrost cycles without visiting stores. This attack surface had already been mapped by researchers: Claroty&\#x27;s Team82 disclosed vulnerabilities in the Danfoss AK-SM 800 A platform, including a hidden &quot;code-of-the-day&quot; authentication mechanism that could bypass login controls and enable remote code execution, and Danfoss subsequently published firmware to fix an authentication bypass in its AK-SM8xxA series cooler controllers.

**「Spoiled stock and pressure to retire vulnerable controllers」** The forced defrost cycles caused direct operational losses at affected stores — spoiled refrigerated food, disrupted deliveries, and price impacts — and reporting on the Intermarché incident additionally indicates that personal data of nearly 300,000 customers was stolen, with those customers advised to stay vigilant online in the coming weeks. For retailers, the actionable concern is exposure of internet-connected refrigeration controllers with publicly documented vulnerabilities: operators still running such legacy hardware face pressure to restrict or remove remote access and replace out-of-support equipment rather than continue relying on controllers they cannot patch.

**「Community discussion」** Commenters debated why commercial refrigeration is online at all: one argued that shift-work operations lack the budget for security reviews or replacing 15–20-year-old end-of-support gear such as the Danfoss SM800 and SC355, while another countered that vendors market remote access for avoiding service callouts and noted even hospital lab machines now require paid, internet-connected subscriptions to run tests. Another commenter pointed to a suspected similar incident affecting US military commissary freezers in August 2026 and asked whether the same group was involved, though that connection is speculative.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/claroty_team82-activity-7330549882962735105-h-MB">Danfoss fixes AK-SM8xxA Series cooler controllers vulnerability</a></li>
<li><a href="https://safetynews.au/story/refrigeration-controller-flaws-threaten-cold-chains">Refrigeration controller flaws threaten cold chains</a></li>
<li><a href="https://www.connexionfrance.com/news/intermarche-cyberattack-affects-nearly-300000-customers/806317">Intermarché cyberattack 2026 : Nearly 300,000 customers&#x27; data stolen...</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#OT security`, `#IoT`, `#critical infrastructure`, `#legacy systems`

---

<a id="item-tech-news-2"></a>
### [w1700k-sdr: Turning a WiFi 7 Router into a 320 Msps SDR Receiver](https://github.com/h0m3us3r/w1700k-sdr) ⭐️ 8.0/10

Developer h0m3us3r has published w1700k-sdr, an open-source project that turns a WiFi 7 router chipset into a software-defined radio receiver sampling at 320 megasamples per second. The project repurposes commodity router silicon into a wideband RF reception platform that would otherwise require expensive dedicated SDR hardware. It is a published, working demonstration rather than a vendor announcement, though the available material does not document supported bandwidths, sample formats, or operating limitations.

hackernews · djfergus · Oct 12, 12:41 · [Discussion](https://news.ycombinator.com/item?id=50055593)

**「Background」** A software-defined radio digitizes radio-frequency signals directly and processes the raw samples on a computer, but receivers sampling at hundreds of millions of samples per second have traditionally required dedicated, costly hardware. The enabler here is that Wi-Fi 7 chipsets such as the MediaTek MT7996 inside the Gemtek W1700K already contain high-speed converters that digitize the standard&\#x27;s wide 320 MHz channels, and the project simply taps that raw 14-bit sample stream — relayed by the router&\#x27;s Airoha AN7581 SoC over 10 GbE — instead of letting the chip process it into Wi-Fi frames.

**「A budget path to wideband SDR reception」** Hobbyists and RF experimenters gain a low-cost route to a 320 Msps wideband software-defined radio receiver by repurposing commodity WiFi 7 router hardware with the open-source w1700k-sdr project, a capability that normally requires expensive dedicated SDR equipment. Because the hack is tied to specific router chipsets, anyone hoping to replicate it should confirm their hardware uses compatible silicon before buying a router for this purpose.

**「Community reaction」** Commenters with SDR experience were enthusiastic while scoping the significance to their niche: aftbit said they know of no cheaper way to get a 320 Msps receiver at 5 GHz, and mikewarot, drawing on experience repairing service monitors, suggested that added fixed and switched attenuators, a 5 GHz low-pass filter, and an external up/down-converter mixer could push the setup toward service-monitor capability. Others noted the same developer previously built an SDR from an ESP32 Wi-Fi microcontroller \(published as eSpDR\), and thebeardisred argued that because it uses the same chipset, the approach should also work on the Banana Pi R4 router, which includes built-in PCIe for NVMe storage.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/h0m3us3r/w1700k-sdr">GitHub - h0m3us3r/w1700k-sdr</a></li>

</ul>
</details>

**Tags**: `#software-defined-radio`, `#hardware-hacking`, `#wifi-7`, `#rf`, `#open-source`

---

<a id="item-tech-news-3"></a>
### [Python 3.15 arrives with explicit lazy imports and a built-in sampling profiler](https://simonwillison.net/2026/Oct/12/python-3-15/) ⭐️ 8.0/10

Python 3.15.0 is released, with the official What&\#x27;s New guide curated by release manager Hugo van Kemenade. Its headline features are PEP 810 explicit lazy imports \(a \`lazy import \` statement defers loading the module until its symbols are first used\), PEP 798 unpacking in comprehensions such as \`\[\*sublist for sublist in lists\]\`, and a new low-overhead sampling profiler called Tachyon \(\`profiling.sampling\`\) that can attach to a running process by PID, joining the renamed tracing profiler \`profiling.tracing\` \(formerly \`cProfile\`\). Independent benchmarking by Miguel Grinberg against the 3.15.0rc3 release found performance mostly unchanged from 3.14, with the exception of the experimental JIT, which delivered a 1.2x speedup over the standard interpreter on a Fibonacci test—the first meaningful JIT gain he had observed. For open source maintainers such as Simon Willison, whose tools target every supported Python version, the release means dropping Python 3.10 support and finally being able to use Python 3.11 features.

rss · Simon Willison · Oct 12, 18:15

**「Background」** Python ships a new major version each year, and maintainers of libraries that support every currently supported version treat each release as the point to drop the oldest one, which is why Willison can say goodbye to Python 3.10 and start using 3.11 features as 3.15 lands. The lazy-import capability also builds on a familiar pain point rather than a new idea: before PEP 810, import statements ran eagerly, so Willison&\#x27;s LLM CLI plugin documentation had to recommend manual lazy-loading workarounds because simply installing plugins with heavy dependencies like sentence\_transformers added multiple seconds to every invocation of the llm command.

**「Python 3.10 is now unsupported, freeing maintainers to move forward」** Python 3.10 reached end of life on October 1, 2026—five years after its release—and now receives no fixes of any kind, including security patches, so projects still pinned to it will not get fixes for newly discovered vulnerabilities. The 3.15 release gives open source maintainers a concrete trigger to drop 3.10 from their support matrices, as Willison is doing, and to start requiring Python 3.11 features; teams that want PEP 810 explicit lazy imports or the built-in Tachyon sampling profiler must upgrade their own environments to 3.15 as well.

<details><summary>References</summary>
<ul>
<li><a href="https://endoflife.ai/article-python-310-eol">Python 3.10 End of Life: October 2026, When Security Fixes Stop</a></li>
<li><a href="https://end-of-life.org/python/3.10/">Python 3.10 End of Life – end-of-life.org</a></li>

</ul>
</details>

**Tags**: `#python`, `#language-features`, `#lazy-imports`, `#pep-810`, `#open-source`

---

<a id="item-tech-news-4"></a>
### [Building a Modern Web App in C with Pledge and Chroot Hardening](https://prophitt.me/writing/a-modern-web-app-in-c) ⭐️ 7.0/10

Developer prophittcorey published a write-up documenting how he built a modern web application in C, with particular attention to deployment and security hardening, including privilege dropping via pledge and chroot. This is a documented personal project rather than a shipped framework or product release, so the described capabilities reflect one developer&\#x27;s setup rather than an independently verified result. The post drew 426 points and 175 comments on Hacker News.

hackernews · prophittcorey · Oct 12, 16:13 · [Discussion](https://news.ycombinator.com/item?id=50058528)

**「Background」** Building a web application in C deliberately echoes the Common Gateway Interface \(CGI\) era of the 1990s, when web servers answered each request by launching a small compiled program, a pattern later refined by FastCGI to keep such binaries resident before most developers moved to long-running application servers in higher-level languages. The security posture described in the write-up relies on privilege dropping: chroot confines the process to a directory subtree, while OpenBSD&\#x27;s pledge restricts which system calls the process may invoke, so that a memory-safety bug in the C code cannot easily escalate into full control of the host.

**「Practical impact」** For developers maintaining small or self-hosted services, the write-up supplies a replicable pattern: a minimal C backend paired with OS-level sandboxing through pledge and chroot to limit the blast radius of any vulnerability. The trade-off surfaced in the comments is architectural: if the binary is invoked per request, as commenter brainless described the nginx setup, in-process state has to live elsewhere, so teams that need shared state would have to run a resident process or a FastCGI-style design instead.

**「Community discussion」** Commenters largely endorsed the approach with their own evidence: ramses0 called the post &\#x27;100% true and well-reasoned,&\#x27; highlighted its pledge/chroot privilege dropping, and noted that busybox ships built-in cgi-bin support, while assimpleaspossi reported running a FastCGI-based C ordering system commercially for some 22 years before its buyer migrated it to a Microsoft stack and ran into repeated problems. The main dissent came from brainless, who prefers resident backends with in-process state — Rust and SQLite with Tokio and Actix Web — over nginx spawning the binary on every request; these are individual experiences and preferences rather than established consensus.

**Tags**: `#C`, `#web-development`, `#systems-programming`, `#security`, `#technical-deep-dive`

---

<a id="item-tech-news-5"></a>
### [OpenAI&\#x27;s Codex CLI installs a self-updating background daemon by default](https://github.com/openai/codex/issues/48195) ⭐️ 7.0/10

OpenAI&\#x27;s Codex CLI installs a persistent, self-updating background daemon by default with no documented way to turn it off, according to GitHub issue \#48195 and a heavily discussed Hacker News thread. Commenters found it can currently be disabled through an undocumented setting — daemon\_auto\_start = false under the \[features\] section of ~/.codex/config.toml — or more forcibly by replacing the daemon&\#x27;s pid and lock files in ~/.codex with symlinks to /dev/null and marking them immutable with chattr +i. Users also reported concrete costs: roughly 12 GB of accumulated old versions on one machine, and auto-update bugs that randomly change repository permissions and leave .git read-only, interrupting long-running tasks. These are user reports from the issue and thread; the supplied material includes no official OpenAI response or documentation change.

hackernews · whimblepop · Oct 12, 18:29 · [Discussion](https://news.ycombinator.com/item?id=50060694)

**「Background」** Codex CLI v0.157.0 made daemon auto-start a stable default in late September 2026: since that release, simply opening an interactive codex session starts a persistent background process \(codex app-server --managed-daemon\), which is what prompted a September 25, 2026 GitHub issue asking that the behavior become opt-in. Coverage of the change notes the daemon updates itself roughly hourly and can kill active agent turns, and that enterprise deployments with strict process-isolation policies may need to disable it explicitly via configuration. The opt-out setting is inconsistently documented: a write-up on the release refers to an auto\_start = false key, while users in the current discussion point to a daemon\_auto\_start flag under \[features\] in ~/.codex/config.toml.

**「Practical impact and mitigations for Codex CLI users」** Developers running Codex CLI 0.157.0 \(installed via npm\) get a persistent, self-updating daemon without explicitly opting in, and users in the discussion report real costs from it: roughly 12GB of accumulated old versions consuming disk space, and auto-updates that reportedly corrupt repository permissions by making .git read-only and blocking work in progress. Until the project grants the request to make daemon\_auto\_start opt-in, developers can act now: set the undocumented flag daemon\_auto\_start = false under the \[features\] section of ~/.codex/config.toml, or delete the daemon&\#x27;s pid and lock files in ~/.codex and replace them with symlinks to /dev/null marked immutable with chattr +i as a filesystem-level guard.

**「Community discussion」** Commenters questioned whether an npm-installed CLI should spawn a daemon at all, with one user saying he would expect such behavior from a desktop client but finds it alarming in a package installed via NPM. Reactions to the harness itself split: one user reported about 12 GB of old versions on disk and called Codex worse than Claude Code &quot;on every metric,&quot; while another said he abandoned heavyweight harnesses for a minimal setup that lets the model rely on plain bash.

<details><summary>References</summary>
<ul>
<li><a href="https://codex.danielvaughan.com/2026/09/25/codex-cli-daemon-auto-start-stable-default-v0157/">Daemon Auto-Start Is Now the Stable Default in Codex CLI v0 ...</a></li>
<li><a href="https://github.com/openai/codex/issues/48195">CLI: make `daemon_auto_start` opt-in — a persistent, self ...</a></li>
<li><a href="https://elsolitario.org/en/2026/10/12/codex-cli-daemon-auto-start-opt-in-en/">Codex CLI Daemon: Why Users Want It Opt-In - elsolitario.org</a></li>
<li><a href="https://github.com/openai/codex/issues/48195">CLI : make ` daemon _auto_start` opt-in — a persistent, self-updating...</a></li>

</ul>
</details>

**Tags**: `#openai`, `#codex-cli`, `#developer-tools`, `#ai-coding-assistants`, `#software-supply-chain`

---

<a id="item-tech-news-6"></a>
### [Meta Announces Muse Wonder AI Model; Testers Question Benchmark Claims](https://research.meta.ai/blog/muse-wonder) ⭐️ 7.0/10

Meta announced Muse Wonder, a new AI model, in a post on its research blog, with a companion Muse Code developer site at dev.meta.ai; the available source material does not include the announcement&\#x27;s technical details, so the model&\#x27;s strong benchmark numbers remain Meta&\#x27;s claims rather than independently verified results. Early hands-on testing shared on Hacker News suggests real-world performance may lag those numbers: one tester&\#x27;s image-to-HTML comparison placed Muse Wonder \(high\) well below Opus 5.5 and closer to Sonnet- or Haiku-class output, with the tester speculating that the model&\#x27;s vision component underperformed. Commenters in the same thread referenced earlier Muse releases — Muse Spark 1.2 in August and Muse 1.3 in September — as comparison baselines, though those details come from community posts rather than the announcement itself.

hackernews · meetpateltech · Oct 12, 16:48 · [Discussion](https://news.ycombinator.com/item?id=50059115)

**「Background」** Meta introduced Muse Wonder and a larger Muse Wonder Full as its most capable models to date, stating that the series achieves state-of-the-art results across benchmarks for personal and professional agents, memory, and coding when compared with other frontier models in Meta&\#x27;s own evaluation suite. Third-party coverage describes it as the first Meta model in some time that appears competitive with the top models from Anthropic and OpenAI, with API details and early results from benchmark aggregators such as Artificial Analysis accompanying the launch. Because frontier-lab benchmark claims are typically self-reported, community testers routinely probe new releases with hands-on tasks, such as generating HTML from a design image, and grade the output against specific tiers of rival models like Anthropic&\#x27;s Claude family.

**「What developers should do」** Developers evaluating Muse Wonder should benchmark it on their own workloads rather than relying on published scores: one early community image-to-HTML comparison found its output closer to mid-tier Claude models \(Sonnet/Haiku-class\) than to Anthropic&\#x27;s top-tier Opus 5.5, despite the strong benchmark numbers reported for the model. Separately, a user reported that signing in through Meta&\#x27;s Muse Code site surfaced other people&\#x27;s account profiles in the login flow and made account settings inaccessible, so users may want to avoid linking their Meta accounts until the company confirms a fix. Muse Code is currently listed as live on Meta&\#x27;s Model API developer portal, which is where this sign-in flow is hosted.

**「Community reaction」** Hands-on reports drove much of the discussion: jjcm&\#x27;s image-to-HTML comparison put Muse Wonder closer to mid-tier Sonnet- or Haiku-level quality than to Opus 5.5 despite its benchmark numbers, while simonw ran comparative SVG &\#x27;pelican&\#x27; tests against the earlier Muse Spark 1.2 and Muse 1.3 releases. The most serious report came from a user who said the Muse Code login flow displayed other people&\#x27;s profiles in their authentication session, suggested Meta may be exposing profile and email data, and reported being unable to reach account settings to deactivate the account — a specific but unverified allegation.

<details><summary>References</summary>
<ul>
<li><a href="https://research.meta.ai/blog/muse-wonder">Muse Wonder | Meta AI Research</a></li>
<li><a href="https://about.fb.com/news/2026/10/introducing-muse-wonder-models/">Introducing Muse Wonder and Muse Wonder Full: Frontier Models ...</a></li>
<li><a href="https://www.agent-one.dev/blog/muse-wonder">Meta Muse Wonder: Benchmarks, Pricing, API, and How to Use It</a></li>
<li><a href="https://dev.meta.ai/">Meta Model API Developer Portal</a></li>

</ul>
</details>

**Tags**: `#artificial-intelligence`, `#meta`, `#large-language-models`, `#benchmarking`, `#model-release`

---

<a id="item-tech-news-7"></a>
### [Looped Diffusion Transformer reruns shared blocks per denoising step with tunable depth](https://www.reddit.com/r/MachineLearning/comments/1x49d61/looped_diffusion_transformer_the_same_blocks_run/) ⭐️ 7.0/10

The Looped Diffusion Transformer \(arXiv 2609.40305, September 30\) is a text-to-image architecture that runs a shared stack of transformer blocks multiple times inside each denoising step rather than scaling up the model, with loop depth selectable at sampling time and no retraining required. The authors state that naive looping does not reliably help and address it with deep supervision on every loop plus self-modulating attention; they report a 260M-parameter model beating a model 6.5x larger on several benchmarks with 4.9x less inference compute, though these benchmark numbers are the paper&\#x27;s own rather than independently measured. The B/16 code and weights are MIT-licensed \(weights on Hugging Face under sensenova\), and Reddit user /u/Fit-Ant2238 ran the released weights on an M5 Pro \(PyTorch MPS, fp32, 100 Euler steps, CFG 6.0, fixed seed per prompt\) across loop depths 1 to 4, finding that most quality change happens by depth 3, with depths 3 and 4 nearly identical on every prompt shown. On that machine, a single image took roughly 23 to 24 seconds at depth 1 and 43 to 47 seconds at depth 4.

reddit · r/MachineLearning · /u/Fit-Ant2238 · Oct 12, 18:13

**「Background」** Diffusion transformers \(DiTs\) generate images by iteratively denoising random noise over many steps, and the conventional way to improve their output quality is to enlarge the network, which raises compute cost at every step. The looped approach instead adapts an idea from looped and recurrent-depth language models, where the same layers are applied several times per forward pass and the iteration count is chosen at inference time, allowing compute to be traded for per-output refinement without retraining. The work discussed here is documented as arXiv paper 2609.40305, published on Sep 30, per its arXiv abstract page.

**「What it means for practitioners」** The MIT-licensed B/16 weights are available now, and the poster&\#x27;s hands-on testing points to a concrete tuning choice: since quality largely saturates by depth 3 while the model was trained at depth 4, sampling at depth 3 or below is a plausible compute saving, with the measured endpoints being about 23-24 seconds per image at depth 1 versus 43-47 at depth 4 on an M5 Pro. The 260M-beats-6.5x-larger benchmark comparisons remain author-reported and unverified, so they should be treated as claims until reproduced independently.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2609.40305">[ 2609 . 40305 ] Looped Diffusion Transformer</a></li>

</ul>
</details>

**Tags**: `#diffusion-models`, `#transformers`, `#efficient-inference`, `#text-to-image`, `#open-source`

---

<a id="item-tech-news-8"></a>
### [learnc auto-tunes constants in unmodified C code for smaller JPEGs and better VAD](https://www.reddit.com/r/MachineLearning/comments/1x4dlbm/learnc_fit_the_constants_in_existing_c_code_to/) ⭐️ 7.0/10

learnc, an MIT-licensed open-source tool, automatically tunes the named constants in unmodified C code against a score function the user writes in C, then rewrites the same file with the new values. On held-out data, the author reports that tuning the 128 quantization-table entries in stb\_image\_write.h on 12 Kodak images and testing on the other 12 yielded a 9.1% BD-rate improvement at equal SSIM — a result he states was checked independently with libjpeg and scikit-image — and beat mozjpeg&\#x27;s tables by 2.7%. Tuning every constant in Google&\#x27;s WebRTC voice activity detector \(vad\_core.c\) improved F1 from 0.810 to 0.859 on the LibriParty eval set. The post states clear limits: no JPEG gain below 1 bpp, and the approach fits tens to hundreds of constants rather than large weight sets.

reddit · r/MachineLearning · /u/keep\_up\_sharma · Oct 12, 20:51

**「Background」** JPEG encoders shrink images by dividing each block of DCT coefficients by quantization tables — in the standard configuration two fixed 8x8 arrays \(luminance and chrominance\) whose entries are hand-chosen constants rather than learned values, and rate-distortion optimization has long explored customizing these coefficients for better size-quality trade-offs. Mozilla&\#x27;s mozjpeg, a libjpeg-turbo patch intended as a drop-in, standard-compatible replacement, already ships redesigned quantization-table presets and trellis quantization for this purpose, making it a natural baseline for any table-tuning claim. On the audio side, Google&\#x27;s WebRTC voice activity detector likewise relies on fixed tuning constants in its vad\_core.c rather than a large set of learned weights.

**「What developers can do with it」** C developers maintaining code full of magic constants can try the tool directly, since the code is on GitHub under the MIT license and requires no changes to the target source beyond supplying a score function. Because tuned values are fit to specific data, teams should validate on their own workloads before shipping — the post itself notes JPEG tuning produced no gain below 1 bpp, and the reported numbers are author-run results pending broader independent adoption.

<details><summary>References</summary>
<ul>
<li><a href="https://salivity.github.io/jpeg/article/rate-distortion-optimization-in-jpeg-quantization">Rate-Distortion Optimization in JPEG Quantization - jpeg</a></li>
<li><a href="https://github.com/mozilla/mozjpeg">GitHub - mozilla/mozjpeg: Improved JPEG encoder. DCT and Quantization | mozilla/mozjpeg | DeepWiki JPEG Quantization Tables Explained: Why Quality 80 Isn&#x27;t ... Quantization Tables in JPEG Digital Forensics - jpeg Rate–distortion optimal evolutionary algorithm for JPEG ... Quantization Table Redesign for the JPEG Compression ...</a></li>
<li><a href="https://deepwiki.com/mozilla/mozjpeg/3.2-dct-and-quantization">DCT and Quantization | mozilla/mozjpeg | DeepWiki</a></li>

</ul>
</details>

**Tags**: `#autotuning`, `#C programming`, `#image compression`, `#voice activity detection`, `#open source tools`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Fed&\#x27;s Hammack says further rate hikes may be needed to prevent entrenched inflation mindset](https://www.cnbc.com/2026/10/12/beth-hammack-fed-inflation-policy.html) ⭐️ 7.0/10

Cleveland Fed President Beth Hammack, a voting member of the Fed&\#x27;s rate-setting committee, said Monday that a restrictive policy stance is appropriate and that smaller, faster rate adjustments are preferable to return inflation to the central bank&\#x27;s 2% goal. She noted headline PCE prices rose 3.4% in the year through August against that 2% target and warned that more than five years of above-target inflation risks entrenching an &\#x27;inflationary mindset&\#x27; in the economy.

rss · CNBC Finance · Oct 13, 02:58

**「Background」** The Fed raised its benchmark interest rate to 3.75%-4.00% at its September 2026 meeting, its first hike in three years, in response to stubbornly high inflation. Hammack is one of the rotating voters on the FOMC, the Fed&\#x27;s rate-setting committee, and the 2026 voting lineup adds officials known for favoring tighter policy.

**「Impact」** Households and businesses with floating-rate loans face higher borrowing costs if the Fed hikes again, an outcome traders currently price at nearly 88% odds for the December meeting versus about 78% for a hold at this month&\#x27;s meeting, according to CME&\#x27;s FedWatch tool.

<details><summary>References</summary>
<ul>
<li><a href="https://www.plus500.com/en-sz/newsandmarketinsights/understanding-fed-dissents-what-could-a-divided-fed-mean">Fed Dissents Explained: Navigating a Divided FOMC | Plus500</a></li>
<li><a href="https://www.usbank.com/investing/financial-perspectives/market-news/federal-reserve-interest-rate.html">Fed raises rates to 3.75%-4.00%, first hike since 2023 | U.S ...</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#inflation`, `#Beth Hammack`

---

<a id="item-finance-news-2"></a>
### [China and EU Reach Consensus on Hybrid and Electric Vehicle Trade](https://www.mofcom.gov.cn/xwfb/sjfzrfb/art/2026/art_4d502e1d49fd4480b39a6cfd0d752038.html) ⭐️ 7.0/10

China&\#x27;s Ministry of Commerce said the two sides reached multiple points of consensus under their trade and investment consultation mechanism, including that China&\#x27;s quota treatment will be no less favorable than the EU&\#x27;s other import sources, with the hybrid vehicle arrangement set upward from a 2025 baseline while preserving China&\#x27;s right to pursue WTO dispute settlement. On electric vehicles, the EU will continue advancing price-undertaking reviews and other review procedures for companies.

telegram · zaihuapd · Oct 12, 06:19

**「Background」** The consensus was reached under the China–EU trade and investment consultation mechanism and builds on the EU&\#x27;s anti-subsidy case against Chinese electric vehicles, where duties remain in place and &\#x27;price undertakings&\#x27;—automakers committing to a minimum import price in exchange for exemption from the duties—have been pursued as the main settlement route since 2024. The two sides also scheduled a ministerial video meeting for January 2027 and the mechanism&\#x27;s third plenary session for March 2027.

**「What it means for exporters」** Chinese automakers exporting hybrids and electric vehicles to the EU gain assured quota treatment no less favorable than other import sources, while the EU&\#x27;s continued review of price undertakings—the mechanism Chinese EV exporters already use—could shape the terms on which they avoid or reduce duties.

<details><summary>References</summary>
<ul>
<li><a href="https://www.zaobao.com.sg/news/china/story20261009-9813146">欧 盟 贸 易 专员： 中 国同意将 混 动 汽 车 对 欧 出口减半 | 联合早报</a></li>
<li><a href="https://www.21jingji.com/article/20241107/herald/91f8e13f10d2180221ee70c3d8dd61bd.html">21jingji.com/article/20241107/herald/91f8e13f10d2180221ee70c3d8dd...</a></li>
<li><a href="https://www.chinaautosupplier.com/show_article-87647.html">chinaautosupplier.com/show_article-87647.html</a></li>

</ul>
</details>

**Tags**: `#China-EU trade`, `#electric vehicles`, `#trade policy`, `#automotive industry`, `#Ministry of Commerce`

---

<a id="item-finance-news-3"></a>
### [China Cuts New Energy Vehicle Export VAT Rebate From 13% to 9%](https://www.news.cn/20261012/9709731f470b42f9a84825c2e4eb914b/c.html) ⭐️ 7.0/10

China&\#x27;s Ministry of Finance and State Taxation Administration announced on October 12 that, starting April 1, 2027, the VAT export rebate rate for new energy vehicles will drop from 13% to 9%, and export rebates for e-cigarette devices will be cancelled. The notice adds that consumption tax rebate and exemption policies for these products remain unchanged.

telegram · zaihuapd · Oct 12, 11:00

**「Background」** China&\#x27;s export tax rebate system refunds part of the value-added tax \(VAT\) paid on domestically made goods once they are shipped abroad; when the rebate rate is set below the full 13% VAT rate, the gap becomes an extra cost that the exporter must absorb.

**「Impact」** Chinese new energy vehicle exporters will receive 4 percentage points less in VAT refunded per exported vehicle starting in April 2027, raising their effective export costs unless absorbed into pricing.

**Tags**: `#fiscal policy`, `#export tax rebate`, `#new energy vehicles`, `#China`, `#trade`

---

<a id="item-finance-news-4"></a>
### [New tax penalty rules take effect Nov 1, with employer social insurance arrears fined up to 3x](https://fgk.chinatax.gov.cn/zcfgk/c100012/c5252754/content.html) ⭐️ 7.0/10

China&\#x27;s State Taxation Administration issued Announcement No. 20 of 2026, publishing the National Tax Administrative Penalty Discretion Benchmarks \(2026 edition\), effective November 1, 2026, which add employers&\#x27; overdue or underpaid social insurance contributions to punishable conduct, tiered by the amount owed and its share, with a maximum fine of 3 times the arrears. Penalties apply only if the employer still fails to pay after being ordered to pay within a set deadline; employers must also make up the arrears plus a daily late fee of 0.05% \(0.5 per ten thousand per day\), and conduct occurring before the effective date is generally handled under the rules then in force.

telegram · zaihuapd · Oct 13, 02:45

**「Background」** The State Taxation Administration had released this benchmark for public comment in July 2026 before issuing the final version, and China&\#x27;s Administrative Punishments Law authorizes agencies to formulate and publish such &quot;discretion benchmarks&quot; — guidelines that standardize how severely a given violation is penalized.

**「Who Is Affected」** Starting November 1, 2026, employers nationwide that still fail to pay social insurance contributions after being ordered to pay within a deadline can be fined up to three times the unpaid amount, on top of back payments and a daily late fee of 0.05%.

<details><summary>References</summary>
<ul>
<li><a href="https://paper.people.com.cn/rmrb/pc/attachement/202607/18/0378ed27-fe07-41dc-95b0-b5fb063d3b93.pdf">paper.people.com.cn/rmrb/pc/attachement/202607/18/0378ed27-fe07...</a></li>
<li><a href="https://npcobserver.com/wp-content/uploads/2023/09/2021-Administrative-Punishments-Law-Revision_Gazette.pdf">npcobserver.com/wp-content/uploads/2023/09/2021-Administrative...</a></li>

</ul>
</details>

**Tags**: `#税务处罚`, `#社保欠缴`, `#政策监管`, `#企业合规`, `#中国税务`

---