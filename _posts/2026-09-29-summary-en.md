---
layout: default
title: "Horizon Summary: 2026-09-29 (EN)"
date: 2026-09-29
lang: en
---

> From 43 items, 12 important content pieces were selected

---

**Technology News**
1. [Anthropic ships Claude Sonnet 5.5: faster, cheaper, now the claude.ai free-tier default](#item-tech-news-1) ⭐️ 8.0/10
2. [How Delhi Cut Electricity Distribution Losses from 50% to 5%](#item-tech-news-2) ⭐️ 7.0/10
3. [Research paper finds AI chat providers sharing conversation data with advertisers and trackers](#item-tech-news-3) ⭐️ 7.0/10
4. [London station facial recognition trial: 500,000 scans, no arrests, one false positive](#item-tech-news-4) ⭐️ 7.0/10
5. [Netherlands pilots NixOS-based ecosystem to replace Microsoft after US sanctions on ICC](#item-tech-news-5) ⭐️ 7.0/10
6. [SemiAnalysis Examines GLM-5.3 Sparse Attention&\#x27;s HBM Memory Impact](#item-tech-news-6) ⭐️ 7.0/10
7. [Free open-source book teaches ML performance engineering from silicon to agents](#item-tech-news-7) ⭐️ 7.0/10
8. [Kuaishou&\#x27;s Kling 4.0 to Launch in October with 4K HDR and 30-Second Clips](#item-tech-news-8) ⭐️ 7.0/10

**Financial News**
1. [AMD to Buy Fei-Fei Li&\#x27;s World Labs for $8.2 Billion](#item-finance-news-1) ⭐️ 8.0/10
2. [Trump&\#x27;s municipal bond holdings grow to as much as $1 billion](#item-finance-news-2) ⭐️ 7.0/10
3. [China Reportedly Sets New Criteria for Humanoid Robot IPOs](#item-finance-news-3) ⭐️ 7.0/10
4. [Oracle Invokes Force Majeure as New Mexico Stargate Data Center Hits Power-Approval Delays](#item-finance-news-4) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Anthropic ships Claude Sonnet 5.5: faster, cheaper, now the claude.ai free-tier default](https://simonwillison.net/2026/Sep/28/claude-sonnet-5-5/) ⭐️ 8.0/10

Anthropic has released Claude Sonnet 5.5, the second model in its Claude 5.5 family, available now across all platforms at the same price as Sonnet 5; the vendor claims it runs 30%+ faster and costs up to 30% less for most work, and reports a Terminal-Bench 4.0 agentic-coding score of 70.6% versus Sonnet 5&\#x27;s 10.3%. In hands-on testing, Simon Willison reproduced a bug Sonnet 5.5 shares with Opus 5.5: at &\#x27;max&\#x27; thinking effort the model consumed 128,000 tokens \(about $1.28\) and failed to produce his pelican SVG, while &\#x27;xhigh&\#x27; effort returned a decent result in 41 seconds for 5.74 cents, and the model otherwise appears nearly as strong as Opus 5.5 on some coding tasks. Notably, Sonnet 5.5 is now the model behind the free tier of claude.ai, which Willison argues makes Anthropic&\#x27;s free offering more capable than OpenAI&\#x27;s ChatGPT free tier, which runs Luna 5.6. It is also the first Sonnet with built-in cyber-safety fallback — a small share of high-risk requests automatically reroutes to Sonnet 5 or is blocked outright — while Haiku 5.5 remains an announced &\#x27;coming weeks&\#x27; release rather than a shipped model.

rss · Simon Willison · Sep 28, 22:07

**「Background」** Claude Sonnet is the mid-tier model in Anthropic&\#x27;s Claude lineup, sitting between the cheaper Haiku models and the more capable Opus tier, and Sonnet 5.5 succeeds Sonnet 5 at unchanged pricing. Willison evaluates new models with his recurring prompt asking for an SVG of pelicans riding a bicycle, and he had already documented this exact failure mode in Claude Opus 5.5 in a September 22, 2026 post: at &\#x27;max&\#x27; thinking effort the model consumes its full 128,000 thinking tokens and produces no output. The &\#x27;max&\#x27; thinking-effort setting is therefore an existing, known-buggy configuration across Anthropic&\#x27;s 5.5-family models rather than a new Sonnet-specific defect.

**「What it means for developers」** Teams can migrate from Sonnet 5 to Sonnet 5.5 as a drop-in change: the API keeps the same $2/$10 per-million-token pricing while Anthropic claims 30%+ faster generation and up to 30% lower cost for most work. One caveat worth acting on: Willison reproduced a bug shared with Opus 5.5 in which the &\#x27;max&\#x27; thinking effort setting consumed 128,000 tokens \(about $1.28\) and produced no output, so developers should avoid that setting or monitor spend until it is fixed. Additionally, because this is the first Sonnet tier to carry Anthropic&\#x27;s cyber safeguards, requests flagged for cybersecurity or frontier-model-development risk may fall back to Sonnet 5 or be blocked outright.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/claude-sonnet-5-5">Introducing Claude Sonnet 5.5 \ Anthropic</a></li>
<li><a href="https://www.marktechpost.com/2026/09/28/anthropic-releases-claude-sonnet-5-5-70-6-on-terminal-bench-4-0-at-the-same-2-10-price/">Anthropic Releases Claude Sonnet 5.5: 70.6% on Terminal-Bench ...</a></li>
<li><a href="https://thenextweb.com/news/sonnet-5-5-cyber-distillation">Anthropic releases Claude Sonnet 5.5 with the cyber ... - TNW</a></li>

</ul>
</details>

**Tags**: `#AI`, `#LLM`, `#Anthropic`, `#Claude`, `#model-release`

---

<a id="item-tech-news-2"></a>
### [How Delhi Cut Electricity Distribution Losses from 50% to 5%](https://spectrum.ieee.org/delhi-electricity-loss) ⭐️ 7.0/10

An IEEE Spectrum retrospective details how Delhi privatized and modernized its electricity distribution, cutting losses from about 50% of power to roughly 5% and largely ending the chronic unplanned outages known as load shedding. The piece is framed as a systems-engineering and policy case study of the transformation rather than a report of a new announcement or single technology. The loss reduction and reliability gains are as reported by the publication, which does not appear to rely on independently audited figures in the material supplied.

hackernews · rbanffy · Sep 29, 12:43 · [Discussion](https://news.ycombinator.com/item?id=49892245)

**「Background」** Delhi privatized its power distribution in 2002, handing operations to BSES and Tata Power with a mandate to cut losses that stood above 52% of purchased electricity at the time. These aggregate technical and commercial \(AT&amp;C\) losses combine physical grid losses with electricity lost to theft, meter tampering, and unbilled consumption, meaning roughly half the power flowing into the network went uncollected. Tata Power&\#x27;s Delhi subsidiary has since reported reducing its AT&amp;C losses from 53% in July 2002 to 5.54% in FY 2024-25, with a 6.3% figure recorded in 2023, crediting increasingly sophisticated metering among a broad set of interventions.

**「Impact」** For households and businesses in Tata Power&\#x27;s Delhi service area, the concrete consequence is dependable supply: the grid reliability index has risen from roughly 70 percent in 2002 to over 99.9 percent, reducing the practical need for the backup inverters, surge precautions, and dual wiring residents once used to cope with frequent unplanned outages. The reform model is also being replicated beyond Delhi: Tata Power reports it has applied the same distribution upgrades in Odisha with reduced AT&amp;C losses, though that claim comes from the company itself rather than an independent assessment.

**「Readers weigh in on what mattered most」** Commenters who experienced pre-reform Delhi argued the loss percentages understate the change, with one recalling outages several times a day and damaging surges when power returned, and contending that eliminating load shedding was the more revolutionary achievement. Others compared systems abroad, including a claim that Greek electricity bills pass losses to customers as a line item, which the commenter said removes utilities&\#x27; incentive to curb theft, while another pointed to Singapore&\#x27;s grid performance as the more interesting story in the article&\#x27;s data.

<details><summary>References</summary>
<ul>
<li><a href="https://spectrum.ieee.org/delhi-electricity-loss">How Delhi Cut Electricity Loss from 50 to 5 Percent - IEEE Spectrum</a></li>
<li><a href="https://timesofindia.indiatimes.com/city/delhi/from-50-losses-to-6-how-delhi-fixed-its-power-loses/articleshow/130121379.cms">From 50 % losses to 6%: How Delhi fixed its power loses | Delhi News</a></li>
<li><a href="https://grokipedia.com/page/Tata_Power_Delhi_Distribution_Limited">Tata Power Delhi Distribution Limited — Grokipedia</a></li>
<li><a href="https://spectrum.ieee.org/delhi-electricity-loss">How Delhi Cut Electricity Loss from 50 to 5 Percent - IEEE Spectrum</a></li>
<li><a href="https://www.linkedin.com/posts/tata-power_revolutionizing-electricity-distribution-activity-7363840902613602304-GKUb">Tata Power -led Odisha discoms improve electricity access... | LinkedIn</a></li>

</ul>
</details>

**Tags**: `#power-grid`, `#infrastructure`, `#energy`, `#india`, `#electrical-engineering`

---

<a id="item-tech-news-3"></a>
### [Research paper finds AI chat providers sharing conversation data with advertisers and trackers](https://jorgegarciaherrero.com/wp-content/interactivos/20260916-Prompt-like-a-butterfly-sting-like-a-tracker-%28clean%29.pdf) ⭐️ 7.0/10

A research paper titled &quot;Prompt Like a Butterfly, Sting Like a Tracker,&quot; shared on Hacker News on September 29, 2026, reports that multiple AI chat providers disclose conversation-derived artifacts — including conversation titles, prompts, and screenshots — to third-party advertisers and trackers, often alongside persistent identifiers that enable attribution to individual users. The paper further reports that some providers publicly expose conversation permalinks without access controls, meaning trackers that obtain a link can read the entire conversation. These are the findings of a measurement study documenting existing industry practices, not a vendor disclosure or regulatory finding, and the submission drew substantial engagement on Hacker News \(312 points, 102 comments at the time of the item\).

hackernews · damaru2 · Sep 29, 09:03 · [Discussion](https://news.ycombinator.com/item?id=49890226)

**「About the study」** The paper, titled &quot;Prompt like a Butterfly, Sting like a Tracker,&quot; is led by researcher Narseo Vallina-Rodríguez and his team and is credited to IMDEA Networks, based on measurements of AI chat services conducted in Spain in May 2026. It has been accepted after peer review at PoPETs 2027, described as a leading academic forum for privacy technologies. The behavior is not uniform across the industry: per the study, Copilot, DeepSeek, and Meta AI did not transmit web conversation data to third-party services during the measurement period.

**「Practical consequences for users and teams」** Users should treat chatbot conversations as attributable to them: the study measured 17 of 20 chatbots sharing data with at least one third party, three transmitting plaintext prompt and response snippets to Microsoft Clarity via session replay, and fifteen sending conversation URLs or chat identifiers to advertising, analytics, or social endpoints, often alongside persistent identifiers. Until providers change their tracker integrations and permalink controls, the actionable step is to keep sensitive personal or business material out of chat prompts, review each provider&\#x27;s tracking and sharing opt-outs, and restrict which assistants are permitted for confidential work. Switching providers alone does not eliminate exposure: even ChatGPT and Claude, which had stronger permalink access controls than Grok, still transmitted certain identifiers and conversation-related metadata to advertising and analytics providers.

**「Reader reactions」** Commenters contested the framing of the findings: drywater2 argued that &quot;leaking&quot; implies an accident, whereas routing conversation data to advertisers is an intentional business practice, and kdaniel\_03 drew a parallel to a recent dispute in which OpenAI reportedly acknowledged that de-identified product data from private Codex sessions may have improved its models, using it to argue that open models are the safer default. Separately, pbasista reported observing ChatGPT&\#x27;s web client periodically send unfinished prompts to a \`conversation/prepare\` endpoint before the user submits them, speculating that such partial text could be used to track users&\#x27; writing cadence and half-formed ideas.

<details><summary>References</summary>
<ul>
<li><a href="https://jorgegarciaherrero.com/en/prompt-like-a-butterfly-sting-like-a-tracker/">Infographic of the paper &quot; Prompt like a Butterfly , sting like a tracker &amp;quo...</a></li>
<li><a href="https://www.drweb.de/ki-chatbots-chatdaten-tracker-werbenetzwerke/">Geben KI- Chatbots Ihre Chatdaten an Werbenetzwerke weiter?</a></li>
<li><a href="https://arxiv.org/abs/2604.27438v1">Tracking Conversations: Measuring Content and Identity Exposure on AI ...</a></li>
<li><a href="https://grafa.com/en/news/crypto/ai-chatbot-data-leak-study">AI chatbots accused of leaking user data to ad trackers</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#ai-industry`, `#tracking`, `#chatbots`, `#security-research`

---

<a id="item-tech-news-4"></a>
### [London station facial recognition trial: 500,000 scans, no arrests, one false positive](https://www.theguardian.com/technology/2026/sep/29/trial-live-facial-recognition-cameras-london-stations-false-positive) ⭐️ 7.0/10

A UK trial of live facial recognition cameras at London rail stations scanned roughly 500,000 faces over several months, producing no arrests and a single false-positive match, The Guardian reported on September 29, 2026. The figures amount to a concrete empirical measurement of the technology&\#x27;s output in a busy transit environment: zero correct identifications leading to arrest, against one mistaken match. The sparse yield has sharpened debate over whether live facial recognition in public spaces delivers enough enforcement value to justify its privacy and civil-liberties costs.

hackernews · ilamont · Sep 29, 11:35 · [Discussion](https://news.ycombinator.com/item?id=49891480)

**「How live facial recognition works」** Live facial recognition \(LFR\) differs from ordinary CCTV: cameras scan the faces of people passing through an area in real time and compare them against a police watchlist, automatically generating an alert when a potential match appears. That real-time matching is why such trials are judged on counts of faces scanned and alert accuracy, and why an erroneous alert can lead to an innocent person being stopped in public. The results of this deployment surfaced through freedom-of-information requests, which showed the six-month trial cost over £320,000 and consumed almost 100 hours of police officers&\#x27; time.

**「Deployment expands despite empty results」** For London rail passengers and civil-liberties campaigners, the trial&\#x27;s outcome offers little documented operational justification for live facial recognition, yet the Met has announced plans to expand the technology into central London by Christmas, meaning commuters will face broader scanning that this trial&\#x27;s results do not yet support. The result fits a pattern: an earlier UK Home Office trial of live facial recognition on the Dublin–Holyhead route also scanned thousands of passengers and found no matches.

**「Reader debate」** Commenters questioned the trial&\#x27;s efficacy and even its reported scale: one calculated that 16 camera deployments running six months would have had to be inactive roughly 99% of the time to scan only 500,000 faces, noting that figure matches about two days of Liverpool Street station&\#x27;s daily footfall, while others asked what measurable return on investment such systems actually provide. A separate argument held that street cameras function less as crime prevention than as a signal to citizens that they are being watched, with one commenter comparing Western surveillance practices to China&\#x27;s.

<details><summary>References</summary>
<ul>
<li><a href="https://rocketnews.com/2026/09/trial-of-live-facial-recognition-in-london-stations-ends-with-a-false-positive-and-no-arrests/">Trial of live facial recognition in London stations ends with ...</a></li>
<li><a href="https://www.techmeme.com/260929/p16">Techmeme: FOI docs: UK police&#x27;s six-month live facial ...</a></li>
<li><a href="https://www.theguardian.com/technology/2026/sep/29/trial-live-facial-recognition-cameras-london-stations-false-positive">Trial of live facial recognition in London stations ... | The Guardian</a></li>
<li><a href="https://www.irishtimes.com/crime-law/2026/04/13/facial-recognition-trial-on-dublin-holyhead-route-scans-thousands-but-finds-no-matches/">Facial recognition trial on Dublin-Holyhead route scans thousands...</a></li>

</ul>
</details>

**Tags**: `#facial-recognition`, `#surveillance`, `#privacy`, `#civil-liberties`, `#AI-ethics`

---

<a id="item-tech-news-5"></a>
### [Netherlands pilots NixOS-based ecosystem to replace Microsoft after US sanctions on ICC](https://www.tomshardware.com/software/the-netherlands-is-rolling-alternative-nixos-based-software-ecosystem-after-u-s-sanctions-on-icc-took-microsoft-off-the-table-trial-programs-running-now-first-release-expected-at-end-of-2027) ⭐️ 7.0/10

The Netherlands is piloting a NixOS-based software ecosystem as an alternative to Microsoft products in government IT, with trial programs already running and a first release targeted for the end of 2027, according to Tom&\#x27;s Hardware. The stated motivation is the dependency risk exposed by US sanctions on International Criminal Court judges, which showed that US vendors could be compelled to cut off foreign institutions from basic services. The project remains at the trial stage, so its eventual scope and any timeline beyond the initial end-2027 release are not yet established.

hackernews · mywacaday · Sep 29, 11:44 · [Discussion](https://news.ycombinator.com/item?id=49891550)

**「The sanctions that exposed the dependency」** In 2025, the United States sanctioned the International Criminal Court&\#x27;s then-chief prosecutor, who lost access to his Microsoft email while his bank accounts were frozen, and US officials warned Dutch counterparts that sanctions could cut off the court&\#x27;s financial and IT services entirely. The project&\#x27;s leaders said it was precisely this sanctions risk — the realization that a US decision could revoke access to essential vendor services at any time — that pushed the Dutch government toward building its own open-source, NixOS-based platform.

**「Impact」** Dutch government bodies taking part in the trials would need to migrate workflows built on Windows and Microsoft services to the NixOS-based stack, making compatibility with existing documents and tools the key near-term test before the end-2027 first release. The sanctions episode also hands other governments a concrete, documented case for evaluating their own reliance on US technology vendors, though adoption decisions elsewhere remain speculative until the Dutch pilots produce results.

**「Community discussion」** The most concrete detail in the discussion came from a commenter who reported that ICC judges have been unable to access bank accounts or receive salary payments in their country of residence due to financial blockages triggered by the US sanctions. Others disagreed over the framing: one argued the effort amounts to a self-imposed sanction, claiming open-source replacements cost far less to run and support, while another suggested that moving off Windows 11 could be a blessing in disguise given businesses being pushed off Windows 10.

<details><summary>References</summary>
<ul>
<li><a href="https://www.thestack.technology/dutch-government-nixos-office-alternative/">Dutch government opts for NixOS as it moves off Office</a></li>
<li><a href="https://apnews.com/article/icc-trump-sanctions-eu-israel-netherlands-2c1cc314732f920c2de59396d3b556f6">The Dutch prepare for US sanctions against the International ...</a></li>
<li><a href="https://www.europesays.com/3271995/">The Netherlands Built a Nix-Basd Linux Desktop Because ...</a></li>

</ul>
</details>

**Tags**: `#digital-sovereignty`, `#nixos`, `#open-source`, `#government-it`, `#linux`

---

<a id="item-tech-news-6"></a>
### [SemiAnalysis Examines GLM-5.3 Sparse Attention&\#x27;s HBM Memory Impact](https://newsletter.semianalysis.com/p/sparse-savings-persistent-demand-inside-glm53) ⭐️ 7.0/10

SemiAnalysis published an analysis by Kimbo Chen on September 28, 2026 examining how GLM-5.3&\#x27;s sparse attention design affects HBM memory consumption during inference, covering KV cache offloading and related techniques named as HiSparse, DeepSeek Sparse Attention, IndexShare, and Single-rollout Asynchronous Optimization. The piece is an examination of serving-memory behavior — sparse attention reduces the per-token key/value data that the KV cache otherwise holds in high-bandwidth memory — rather than a new model, hardware, or product announcement. Only the article&\#x27;s title and topic keywords were supplied with this item, so its specific measurements, methodology, and conclusions could not be verified here, and nothing in this report should be read as an independently confirmed result about GLM-5.3&\#x27;s memory usage.

rss · Semianalysis · Sep 28, 19:26

**「Sparse attention and HBM memory」** In transformer inference, attention over long contexts requires storing a key-value \(KV\) cache of all previous tokens in high-bandwidth memory \(HBM\), making memory capacity and bandwidth major cost and performance constraints as context grows. Sparse-attention techniques such as DeepSeek Sparse Attention \(DSA\), used in Z.ai&\#x27;s GLM-5.3, reduce the memory bandwidth consumed during the attention computation by dynamically selecting only the top-k most relevant tokens, but because the initial token-selection step still requires access to the complete context history, these methods do not inherently eliminate primary memory capacity requirements.

**「HBM-to-DRAM KV cache tiering becomes a deployment decision」** For teams serving GLM-5.3-class models, sparse attention makes where the KV cache lives a first-class capacity decision rather than an HBM sizing afterthought. The SGLang team built HiSparse specifically to proactively offload KV cache entries from device HBM to host DRAM, and comparable offloading already ships in Nvidia&\#x27;s Dynamo, which tiers cache from GPU HBM through CPU DRAM and local SSD to networked storage. Operators adopting these designs face a measurable trade-off: cold KV cache left in HBM sacrifices concurrency, while offloading too deeply degrades latency, so tiering depth becomes a concrete tuning knob for serving economics.

<details><summary>References</summary>
<ul>
<li><a href="https://www.partgenie.ai/insights/how-glm5-3-sparse-attention-affects-hbm-memory-usage-2">How GLM-5.3 Sparse Attention and Hierarchical Memory Shape Accelerator ...</a></li>
<li><a href="https://www.polaris7.io/signals/glm-53-sparse-attention-impact-on-dram-memory-tam">GLM-5.3 Sparse Attention Impact on DRAM Memory TAM</a></li>
<li><a href="https://newsletter.semianalysis.com/p/sparse-savings-persistent-demand-inside-glm53">Inside GLM-5.3: How Sparse Attention Affects DRAM Memory TAM</a></li>
<li><a href="https://404kresearch.substack.com/p/the-ai-memory-demand-landscape-the">The AI Memory Demand Landscape: The HBM Bandwidth Wall, KV Cache Expansion, and SSD Tiering</a></li>
<li><a href="https://www.blocksandfiles.com/ai-ml/2026/03/30/nvidia-and-its-partners-kv-cache-extenders/5209284">Nvidia and its partners&#x27; KV Cache extenders</a></li>

</ul>
</details>

**Tags**: `#sparse-attention`, `#AI-inference`, `#HBM-memory`, `#KV-cache`, `#GLM-5.3`

---

<a id="item-tech-news-7"></a>
### [Free open-source book teaches ML performance engineering from silicon to agents](https://www.reddit.com/r/MachineLearning/comments/1wt6ns4/i_wrote_a_free_opensource_book_on_making_ml/) ⭐️ 7.0/10

Reddit user /u/SoloTiger\_ has released a free, open-source book titled &quot;How to Make Your Model Fast: A Systems View of Efficient Machine Learning, from Silicon to Agents,&quot; hosted on GitHub. Its core thesis is that reducing FLOPs does not necessarily make a model faster; readers first learn to use roofline analysis to determine whether a workload is compute-, bandwidth-, memory-, or system-bound before choosing an optimization. The material progresses from hardware and roofline analysis through kernels, compilers, quantization, pruning, vision, on-device LLMs, robotics, profiling, and serving, ending with applying the same bound analysis to agent workloads. This is a self-published announcement: the book is downloadable and the author is soliciting feedback and contributions, but its depth and accuracy have not been independently reviewed.

reddit · r/MachineLearning · /u/SoloTiger\_ · Sep 29, 10:35

**「Why fewer FLOPs doesn&\#x27;t mean faster models」** The book&\#x27;s starting point, roofline analysis, is a classic computer-architecture technique: by comparing a workload&\#x27;s arithmetic intensity \(operations per byte of data moved\) against a processor&\#x27;s compute and memory-bandwidth ceilings, it reveals whether performance is limited by computation or by data movement. That distinction underlies the author&\#x27;s premise that cutting FLOPs often fails to make a model faster, since optimizations such as quantization, pruning, and kernel tuning only pay off when aimed at the actual bottleneck. A v1.0 first-edition release on the project&\#x27;s GitHub repository shows the book is already published and readable free online, not merely announced.

**「Free access and open contribution」** ML practitioners optimizing inference can now read the full book at no cost from the GitHub repository usamahz/make-your-model-fast and apply its central workflow: using roofline analysis to determine whether a model is compute-, bandwidth-, memory-, or system-bound before deciding whether quantization, pruning, or kernel optimization is worth doing. The author explicitly solicits feedback and contributions from people working on ML systems, inference, compilers, and edge AI, giving early readers a direct route to shape the material. Because it is a self-published announcement whose depth is not yet independently verified, teams should benchmark its techniques against their own hardware and workloads before relying on them in production.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/usamahz/make-your-model-fast/releases/tag/v1.0">Release How to Make Your Model Fast, first edition · usamahz/make-your-model-fast</a></li>

</ul>
</details>

**Tags**: `#ml-systems`, `#performance-engineering`, `#inference-optimization`, `#quantization`, `#gpu-kernels`

---

<a id="item-tech-news-8"></a>
### [Kuaishou&\#x27;s Kling 4.0 to Launch in October with 4K HDR and 30-Second Clips](https://finance.sina.com.cn/stock/t/2026-09-28/doc-initmeau2827369.shtml) ⭐️ 7.0/10

Kuaishou&\#x27;s AI video team announced that Kling 4.0 will officially launch in October, while the lighter Kling 4.0 Flash variant has been open to a small group of users for early testing since September 28. According to the announcement, version 4.0 supports 4K and 1080p 10-bit HDR output, accepts up to 10 images, 5 video clips, and 7 subjects as reference inputs in a single generation, and can produce videos up to 30 seconds long. These are announced specifications from the company: the full release has not shipped yet, and only the Flash variant is available in limited preview, so real-world output quality has not been independently verified.

telegram · zaihuapd · Sep 29, 00:52

**「Background」** Creators with early access refer to the multi-image, multi-video, multi-subject input capability as &quot;Omni Reference&quot; and report that the full Kling 4.0 is considerably stronger than the Flash preview, particularly for dialogue-driven acting. The 10-bit HDR output is a departure from the usual standard for AI-generated video, which is typically 8-bit: 10-bit encodes 1,024 gradations versus 8-bit&\#x27;s 256, reducing banding in skies and color gradients once clips go through color correction.

**「Impact」** For creators using Kling for persona-driven or commerce video—a segment where 2026 model comparisons already rated Kling&\#x27;s portrait consistency and audio-visual sync highly—the ability to feed up to 10 images, 5 videos, and 7 subjects per generation directly targets multi-character and product-consistency workflows, while 4K/1080p 10-bit HDR output suits ad-grade delivery. Because only Kling 4.0 Flash is in limited preview as of September 28 and the full release is merely promised for October, production teams should benchmark it against early-2026 rivals such as ByteDance&\#x27;s Seedance v1.5 Pro and Google DeepMind&\#x27;s Veo 3.1 before standardizing on it.

<details><summary>References</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=b2jR0rOGEKQ">SPARE, a short film generated with the full version of Kling ... - YouTube</a></li>
<li><a href="https://www.drweb.de/kling-4-0-ki-video-30-sekunden-kuaishou/">Kling 4 . 0 : Was kann Kuaishous neues KI-Videomodell? | Dr. Web</a></li>
<li><a href="https://opencreator.io/zh/blog/ai-video-models-comparison-2026">主流AI 视频模型横向测评2026：Seedance、Veo、Sora、万相</a></li>
<li><a href="https://www.atlascloud.ai/blog/tips/seedance-vs-kling-vs-sora-vs-veo">Best Sora Alternatives in 2026: Seedance vs Kling vs Veo-Ultimate Head-to-Head Comparison - Atlas Cloud Blog</a></li>

</ul>
</details>

**Tags**: `#AI 视频生成`, `#可灵 Kling`, `#快手`, `#生成式 AI`, `#模型发布`

---

## Financial News

<a id="item-finance-news-1"></a>
### [AMD to Buy Fei-Fei Li&\#x27;s World Labs for $8.2 Billion](https://ir.amd.com/news-events/press-releases/detail/1299/amd-to-acquire-world-labs-to-advance-the-future-of-ai-compute) ⭐️ 8.0/10

AMD announced an $8.2 billion acquisition of World Labs, an AI startup founded by Fei-Fei Li that builds &quot;world models&quot; — technology designed to help AI understand and simulate the physical world, including generating simulated environments used to train robots. Li will join AMD as executive vice president and chief scientist, combining her company&\#x27;s model research with AMD&\#x27;s chips and computing platforms. The deal is expected to close by year-end, pending regulatory approval.

telegram · zaihuapd · Sep 29, 03:59

**「Background」** World Labs is an AI startup founded in 2024 by Fei-Fei Li — a former Google Cloud AI chief widely called the &quot;Godmother of AI&quot; — who serves as its CEO, and it has raised roughly $1 billion to build world models, AI systems that understand and simulate the physical world.

**「Why it matters」** The acquisition intensifies competition in the AI chip market, where AMD is directly countering Nvidia&\#x27;s push into world models and robotics simulation, and could influence which platforms robotics developers rely on for simulated training environments.

<details><summary>References</summary>
<ul>
<li><a href="https://aifunding.me/insights/world-labs-deep-dive">World Labs : How a High-Growth AI Pioneer Is... | AI Funding</a></li>
<li><a href="https://grokipedia.com/page/world-labs">World Labs — Grokipedia</a></li>
<li><a href="https://cointelegraph.com/news/godmother-ai-world-labs-230-million-funding?trk=article-ssr-frontend-pulse_little-text-block">‘Godmother of AI ’ launches World Labs with $230M funding at...</a></li>
<li><a href="https://www.linkedin.com/news/story/amd-targets-physical-ai-with-82b-world-labs-acquisition-7608652/">AMD targets physical AI with $8.2B World Labs acquisition | LinkedIn</a></li>
<li><a href="https://www.androguider.com/2026/09/amd-to-acquire-fei-fei-lis-world-labs.html">AMD to Acquire Fei-Fei Li’s World Labs for $8.2 Billion in Bold AI Bet</a></li>

</ul>
</details>

**Tags**: `#mergers-and-acquisitions`, `#AMD`, `#AI-compute`, `#world-models`, `#robotics`

---

<a id="item-finance-news-2"></a>
### [Trump&\#x27;s municipal bond holdings grow to as much as $1 billion](https://www.cnbc.com/2026/09/29/trump-municipal-bond-portfolio.html) ⭐️ 7.0/10

CNBC&\#x27;s analysis of President Trump&\#x27;s financial disclosures, most recently a July report made public on Sept. 22, 2026, finds his municipal bond holdings — debt issued by cities, hospitals, schools and utilities — have grown to more than 1,000 positions worth roughly $300 million to $1 billion. Many of the issuers are affected by decisions from his own administration, though CNBC found no evidence of trades made on advance knowledge of those decisions.

rss · CNBC Finance · Sep 29, 14:37

**「Background」** Municipal bonds are debt that cities, hospitals, schools and utilities issue to pay for public projects, and their repayment depends partly on federal grants and regulation. This situation raises questions because, unlike other federal employees, the president is exempt from the federal conflict-of-interest law that bars officials from official actions affecting their own financial interests.

**「Why it matters」** Cities, hospitals and utilities that depend on federal funding and regulation — including health systems exposed to roughly $900 billion in projected Medicaid cuts over a decade, according to KFF — now count the president among their creditors, and ethics experts note presidents are exempt from the conflict-of-interest rules that apply to other federal officials.

<details><summary>References</summary>
<ul>
<li><a href="https://factually.co/fact-checks/politics/federal-ethics-rules-president-family-commercial-crypto-products-c0156c">What federal ethics or conflict - of - interest rules appl...</a></li>
<li><a href="https://www.law.cornell.edu/uscode/text/18/208">18 U . S . Code § 208 - Acts affecting a personal financial interest</a></li>

</ul>
</details>

**Tags**: `#municipal bonds`, `#conflict of interest`, `#financial disclosures`, `#Trump administration`, `#public finance`

---

<a id="item-finance-news-3"></a>
### [China Reportedly Sets New Criteria for Humanoid Robot IPOs](https://www.cnbc.com/2026/09/29/china-criteria-humanoid-robot-ipos.html) ⭐️ 7.0/10

China&\#x27;s securities regulator has reportedly set three criteria for humanoid robot IPOs — sustainable revenue and commercial orders, narrowing losses, and core technology such as a robotic brain or hands — a bar that few or none of the country&\#x27;s more than 100 &\#x27;embodied AI&\#x27; startups can meet, according to three anonymous sources. At least two dozen humanoid-related companies have already filed to list in Hong Kong, though the CSRC did not respond to a request for comment and the Hong Kong exchange declined to comment.

rss · CNBC Finance · Sep 29, 07:19

**「Background」** Beijing has backed &quot;embodied AI&quot;—artificial intelligence embedded in physical robots—in its last two annual government work reports, and the sector now counts well over 100 domestic startups, though authorities have also warned of a bubble in the industry. The CSRC has previously used IPO approvals as a policy lever, imposing phased restrictions on new listings to balance investment and financing before its head signaled an easing of those curbs.

**「Impact」** If enforced, the rules could block public listings for startups across a sector that drew 47.09 billion yuan \(about $6.95 billion\) of investment in the second quarter, cutting off a funding route for founders and the government and private funds backing them.

<details><summary>References</summary>
<ul>
<li><a href="https://www.szftbz.com/blog/china-companies-fundraising-options-narrow-after-ipo-restrictions">China companies&#x27; fundraising options narrow after IPO restrictions</a></li>
<li><a href="https://www.scmp.com/business/china-business/article/3300050/china-may-ease-ipo-curbs-csrc-head-signals-policy-loosening-morgan-stanley-says">China may ease IPO curbs as CSRC head signals policy loosening...</a></li>

</ul>
</details>

**Tags**: `#China regulation`, `#humanoid robotics`, `#IPOs`, `#embodied AI`, `#CSRC`

---

<a id="item-finance-news-4"></a>
### [Oracle Invokes Force Majeure as New Mexico Stargate Data Center Hits Power-Approval Delays](https://www.bloomberg.com/news/articles/2026-09-24/oracle-cites-force-majeure-to-shield-itself-on-controversial-data-center) ⭐️ 7.0/10

Oracle has sent a force majeure notice to the developer of the Stargate &\#x27;Project Jupiter&\#x27; data center in New Mexico, seeking to defer some payments after environmental and power-supply approvals for the project&\#x27;s 2.45GW microgrid stalled, putting its targeted 2028 startup at risk. The news pushed the project&\#x27;s $18 billion syndicated loan to trade at a discount, adding to concern about construction timelines for giant AI data centers.

telegram · zaihuapd · Sep 29, 05:46

**「Background」** Force majeure is a contract clause that lets a party suspend obligations, such as payments, when events beyond its control—in this case delayed energy approvals tied to a gas pipeline—prevent a project from performing. Project Jupiter is a Stargate data center intended to serve OpenAI, and Oracle&\#x27;s notice went to Blue Owl, the developer and financing counterparty behind the project&\#x27;s lease.

**「Who is affected」** The banks holding the $18 billion syndicated loan \(debt shared among multiple lenders\) for Project Jupiter are directly hit: the loan has stalled in distribution and is quoted at 89–91 cents on the dollar, cutting its market value to roughly $16–16.4 billion as investors question the project&\#x27;s timeline.

<details><summary>References</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=mNozPwLvJIY">Oracle Is Paying for a Data Center It Can&#x27;t Use - YouTube</a></li>
<li><a href="https://best-ai.org/ai-news/oracle-triggers-force-majeure-on-245-gw-stargate-data-center-in-new-mexico-over-energy-supply-delays-gm2tsb">Oracle Triggers Force Majeure on 2 . 45 - GW Stargate Data Center in...</a></li>
<li><a href="https://digg.com/tech/oxyjjcs1">Oracle reportedly sends notice to delay Project Jupiter payments if it...</a></li>
<li><a href="https://finance.biggo.com/news/aa2b00f9-d885-40e0-92db-6fd9f55ffe63">Oracle&#x27;s $18 Billion AI Loan Sells at a Discount, Banks Forced to Swallow a Hot Potato — BigGo Finance</a></li>
<li><a href="https://allweatherfinance.com/oracles-18-billion-ai-loan-is-being-sold-at-a-discount-highlighting-the-pressure-on-its-ai-financing-chain/">Oracle&#x27;s $18 billion AI loan is being sold at a discount, highlighting the pressure on its AI financing chain.</a></li>

</ul>
</details>

**Tags**: `#AI数据中心`, `#甲骨文`, `#星际之门`, `#不可抗力`, `#银团贷款`

---