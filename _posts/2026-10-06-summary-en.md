---
layout: default
title: "Horizon Summary: 2026-10-06 (EN)"
date: 2026-10-06
lang: en
---

> From 37 items, 12 important content pieces were selected

---

**Technology News**
1. [vLLM v0.31.0 ships Blackwell-optimized DeepSeek-V4.1-Flash path and fast-restart preload CLI](#item-tech-news-1) ⭐️ 8.0/10
2. [Reflection AI releases Beam, a 501B-parameter open-weight sparse MoE model](#item-tech-news-2) ⭐️ 8.0/10
3. [Cloudflare launches Web Search API for AI agent developers](#item-tech-news-3) ⭐️ 7.0/10
4. [Anthropic reported a woman&\#x27;s Claude diary entry to police, leading to a felony charge](#item-tech-news-4) ⭐️ 7.0/10
5. [Stratechery: Apple&\#x27;s Privacy Model May Lose AI-Native Users to Meta&\#x27;s Muse](#item-tech-news-5) ⭐️ 7.0/10
6. [Qualcomm reportedly licenses patents on Huawei&\#x27;s LogicFolding chip technology](#item-tech-news-6) ⭐️ 7.0/10
7. [Gigafish: 3.9B Chess Positions Distilled from Stockfish Released on Hugging Face](#item-tech-news-7) ⭐️ 7.0/10
8. [Yandex Music reports single transformer Sona replaced its multi-stage recommender in A/B test](#item-tech-news-8) ⭐️ 7.0/10
9. [Quad9 Refuses French Piracy Blocks, Risks €580,000 Daily Fine](#item-tech-news-9) ⭐️ 7.0/10
10. [OpenAI to Add Invisible Watermarks to Some EU ChatGPT and Codex Text Outputs](#item-tech-news-10) ⭐️ 7.0/10

**Financial News**
1. [Brazilian Stocks Jump as Flávio Bolsonaro Becomes Heavy Runoff Favorite](#item-finance-news-1) ⭐️ 8.0/10
2. [Gas-Only Cars Fall Below Half of Global New-Car Sales for the First Time](#item-finance-news-2) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [vLLM v0.31.0 ships Blackwell-optimized DeepSeek-V4.1-Flash path and fast-restart preload CLI](https://github.com/vllm-project/vllm/releases/tag/v0.31.0) ⭐️ 8.0/10

vLLM v0.31.0 is out, aggregating 717 commits from 307 contributors \(96 of them new\), with Python wheels and Docker images for CUDA 13.0/12.9, ROCm, CPU, and Intel XPU. Per the release notes, the headline work is DeepSeek-V4.1-Flash serving on Blackwell \(SM100\) GPUs, where FlashMLA mega attention paired with the NVFP4 compressed KV cache is now the SM100 default, alongside DeepGEMM sparse MQA indexer logits, a Mega-Gate kernel fusing the gate GEMM with expert selection, and several fused MXFP8 paths. For operators, a new \`vllm preload\` CLI runs a weight-cache daemon that keeps post-quantized weights resident in GPU memory across engine restarts \(now with data parallelism, MTP draft-model support, and a /health endpoint\), and experimental \`vllm snapshot create/restore\` commands use CRIU to restore a fully initialized TP1 engine. Upgraders face breaking changes: \`tokenizer\_mode=&quot;slow&quot;\` is removed, per-request multimodal kwargs are rejected unless \`--trust-request-mm-kwargs\` is set, \`quantization=&quot;fp8&quot;\` is replaced by the \`fp8\_per\_tensor\` shorthand, and XPU graphs are enabled by default.

github · khluu · Oct 5, 06:44

**「Background」** vLLM is an open-source engine for serving large language models, and its releases aggregate many community contributions — v0.31.0 alone bundles 717 commits from 307 contributors, 96 of them first-time. The headline performance work targets DeepSeek-V4.1-Flash on NVIDIA&\#x27;s SM100/Blackwell data-center GPUs, where an NVFP4 compressed KV cache shrinks the memory needed to hold conversation context and fused Mixture-of-Experts \(MoE\) kernels cut per-step kernel and data-movement overhead during decoding.

**「Upgrade actions and compatibility notes」** Teams upgrading to v0.31.0 should audit launch scripts and client payloads first: per-request \`mm\_processor\_kwargs\` and \`media\_io\_kwargs\` are now rejected unless the server sets \`--trust-request-mm-kwargs\`, \`tokenizer\_mode=&quot;slow&quot;\` and the AllSpark INT8 W8A16 backend are removed, online \`quantization=&quot;fp8&quot;\` is replaced by the \`fp8\_per\_tensor\` shorthand, and XPU graphs are enabled by default with the \`VLLM\_XPU\_ENABLE\_XPU\_GRAPH\` flag removed. Operators serving DeepSeek-V4.1-Flash on NVIDIA Blackwell \(SM100\) get FlashMLA mega attention with the NVFP4 compressed KV cache as the new default without extra configuration, and can shorten engine restarts by running the new \`vllm preload\` weight-cache daemon.

<details><summary>References</summary>
<ul>
<li><a href="https://localmodelwatch.tsuchitsuchi.com/en/2026/10/05/vllm-v0310-released/">vLLM v0.31.0 Released: Fast Restart and Hardware Optimization</a></li>

</ul>
</details>

**Tags**: `#vllm`, `#llm-inference`, `#gpu-optimization`, `#quantization`, `#open-source`

---

<a id="item-tech-news-2"></a>
### [Reflection AI releases Beam, a 501B-parameter open-weight sparse MoE model](https://reflection.ai/blog/introducing-beam) ⭐️ 8.0/10

Reflection AI has released Beam, an open-weight sparse Mixture-of-Experts language model with 501 billion total parameters and 23 billion active parameters, pretrained on 23.8 trillion tokens and built for coding, reasoning, and agentic workloads. The company states its pretraining matches or outperforms similar-sized open base models and that it made major investments in reinforcement learning on top, but these are vendor claims and have not been independently verified. Among the vendor-reported results is a &\#x27;Land or Water&\#x27; grid-puzzle generalization demo, which the blog says is days old and therefore absent from training data, where Beam reportedly achieved 95.5% coverage, placing it between Opus 5 \(92.5%\) and a model referred to as Fable.

hackernews · Philpax · Oct 5, 19:16 · [Discussion](https://news.ycombinator.com/item?id=49969183)

**「Background」** Beam is Reflection AI&\#x27;s first open-weight model, introduced on October 5, 2026, and positioned as a Western counterpart to the Chinese systems that have so far defined frontier-scale open-weight releases. It uses a sparse Mixture-of-Experts architecture, meaning only 23 billion of its 501 billion total parameters activate per token, letting the model carry far more capacity than its per-token compute suggests. The text-only model is available for download and targets coding, reasoning, and agentic workloads.

**「Impact」** For teams that self-host or fine-tune open-weight models, Beam adds a Western frontier-scale option for coding and agentic workloads, but its serving economics warrant scrutiny: a community comparison with DeepSeek V4.1 Flash noted that Beam keeps 23 billion parameters active at both prefill and decode, versus DeepSeek&\#x27;s 8–16 billion, implying higher per-token compute for would-be hosters. Reflection&\#x27;s own scorecard places Beam near or ahead of some open models on selected coding tests and behind others, and the company&\#x27;s compute comparison excludes several costs of serving the model — so organizations evaluating it should benchmark against their incumbent models on real workloads and account for full serving costs before switching.

**「Community discussion」** Commenter wren6991 compiled a spec comparison against DeepSeek V4.1 Flash, showing comparable total size \(501B vs 552B parameters\) but higher active parameters \(23B vs 8B prefill / 16B decode\), fewer pretraining tokens \(28T vs 45T by the commenter&\#x27;s figures\), and no n-gram/PLE component versus DeepSeek&\#x27;s 196B. NorwegianDude argued Western open-weight releases still trail smaller free Chinese models, while Ariarule expressed skepticism about the vendor&\#x27;s claim that a days-old viral puzzle could not have appeared in Beam&\#x27;s training data — these are commenters&\#x27; opinions and figures, not established results.

<details><summary>References</summary>
<ul>
<li><a href="https://pollar.news/en/event/reflection-debuts-beam-ai">Reflection AI unveils 501-billion-parameter Beam model to rival...</a></li>
<li><a href="https://www.unite.ai/reflection-ai-unveils-beam-a-501b-parameter-open-weight-model/">Reflection AI Unveils Beam , a 501 B -Parameter Open-Weight Model</a></li>
<li><a href="https://cellcog.ai/blog/reflection-beam-open-weight-model/">Reflection Beam : 501 B Open-Weight Model , Benchmarks | CellCog</a></li>
<li><a href="https://runtimewire.com/article/reflection-ai-beam-open-weight-model">Reflection publishes Beam benchmark scores ahead of its ...</a></li>
<li><a href="https://techcrunch.com/2026/10/05/reflection-debuts-beam-a-open-weight-ai-model-to-rival-chinese-models-at-lower-compute-cost/">Reflection debuts Beam, an open-weight AI model to rival ...</a></li>

</ul>
</details>

**Tags**: `#open-weight models`, `#large language models`, `#mixture-of-experts`, `#reinforcement learning`, `#AI industry`

---

<a id="item-tech-news-3"></a>
### [Cloudflare launches Web Search API for AI agent developers](https://developers.cloudflare.com/changelog/post/2026-10-02-introducing-web-search-api/) ⭐️ 7.0/10

Cloudflare has launched a Web Search API, announced in a changelog post dated October 2, 2026, aimed at developers and builders of AI agents that need search grounding. The launch drew a large Hacker News discussion \(491 points, 223 comments\) that focused on licensing limits around storing or resyndicating search results, price comparisons with alternatives such as Google Gemini&\#x27;s bundled search access and Jina&\#x27;s search API, and criticism of Cloudflare&\#x27;s dual role as both a bot blocker and a paid gatekeeper for &\#x27;verified&\#x27; bots. Because the changelog text itself was not available for this item, specifics such as the API&\#x27;s pricing, quotas, and data-retention terms remain unconfirmed.

hackernews · tosh · Oct 5, 10:47 · [Discussion](https://news.ycombinator.com/item?id=49963171)

**「Background」** Grounding is the practice of feeding an AI model live web results so its answers reflect current information, and developers typically do this by calling a hosted search API from inside an agent pipeline. Cloudflare already operates AI Gateway, a proxy layer through which developers route model inference traffic, and the new API extends that gateway with search from three third-party providers — Ceramic.ai, Exa, and Linkup — rather than a Cloudflare-built search index. The documentation also describes the crawling standards these providers follow, positioning the product around compliant crawling of live web data.

**「What agent builders should weigh before adopting it」** Before committing to the API, agent developers should check whether its terms of service allow storing or resyndicating search results: Hacker News commenter simonw argued that such restrictions would block common features like a &quot;share transcript&quot; button, and noted the relevant licensing language is typically buried deep in the terms. Cost is the other deciding factor — commenters flagged cheaper or bundled alternatives, including Jina&\#x27;s search API, which also returns page content as markdown, and Google&\#x27;s Gemini Flash Lite 2.5, which reportedly still provides existing users 1,000 free searches per day. Some developers also questioned adding Cloudflare as an intermediary at all, pointing to its dual role as both a bot-blocking gatekeeper and a paid verifier of bots.

**「Community discussion」** In the Hacker News thread, simonw argued that the decisive question for any search API is whether its terms allow storing and resyndicating results, since restrictions there would curtail agent features like a &\#x27;share transcript&\#x27; button. Commenters iphonecorridor and jerrygoyal pointed to cheaper or more generous alternatives, including Gemini Flash Lite 2.5&\#x27;s free 1,000 Google searches per day and Jina&\#x27;s API, which also returns page content as markdown, while binarymax and denkmoon questioned why Cloudflare should sit between developers and search providers, with denkmoon characterizing the API as the profit step after blocking other bots&\#x27; page access.

<details><summary>References</summary>
<ul>
<li><a href="https://developers.cloudflare.com/web-search/">Overview · Cloudflare Web Search API docs</a></li>
<li><a href="https://developers.cloudflare.com/web-search/about/">About Web Search API - Cloudflare Docs</a></li>
<li><a href="https://blog.cloudflare.com/introducing-web-search-api/">Introducing Web Search API via AI Gateway | Cloudflare Blog</a></li>

</ul>
</details>

**Tags**: `#cloudflare`, `#search-api`, `#ai-agents`, `#developer-tools`, `#web-crawling`

---

<a id="item-tech-news-4"></a>
### [Anthropic reported a woman&\#x27;s Claude diary entry to police, leading to a felony charge](https://www.techspot.com/news/114091-florida-woman-used-claude-diary-anthropic-reported-shoot.html) ⭐️ 7.0/10

Anthropic reported a Florida woman&\#x27;s Claude diary entry, which contained threats, to local police, and she now faces a felony charge under Florida&\#x27;s written-threat statute, according to the report. The case stands out because the transcript reached law enforcement through the vendor&\#x27;s own review rather than a subpoena or leak, sharpening debate over whether LLM conversations carry any expectation of privacy and how vendors balance user trust against the risk of not reporting violent threats. The available material does not establish details such as the exact wording of the threats, the charging documents, or whether Anthropic has publicly commented on the case.

hackernews · emptybits · Oct 5, 05:37 · [Discussion](https://news.ycombinator.com/item?id=49961057)

**「Background」** Conversations with AI chatbots such as Claude are often used as private journals, but they remain subject to the company&\#x27;s own review processes: per WINK News reporting cited by Tom&\#x27;s Hardware, Anthropic&\#x27;s human review team examined the woman&\#x27;s &\#x27;diary&\#x27; entries and passed the threatening statements to law enforcement. Tom&\#x27;s Hardware notes this is at least the third such AI chatbot conversation to reach police since August, suggesting an emerging pattern of AI companies escalating threatening user chats. The defendant, identified by Decrypt as Carli Michelle Heller of Bonita Springs, was charged under Florida&\#x27;s written-threat statute, a law written before AI chatbots existed, and how it applies to model transcripts remains an open legal question.

**「Claude conversations can end up as police evidence」** The practical consequence for Claude users is that flagged chat transcripts can be reviewed by Anthropic and handed to law enforcement, and the content itself can support criminal charges — in this case a felony under Florida&\#x27;s written-threat statute. According to Tom&\#x27;s Hardware, this is at least the third Claude conversation to reach police since August, so reporting user threats appears to be a repeat practice rather than a one-off decision. Users who treat chatbots as private journals should assume those entries are potentially readable by the provider and reportable to authorities, and can consult Anthropic&\#x27;s Privacy Center for how conversations are handled.

**「Community debate」** Commenters disputed whether Florida Statute 836.10 — quoted in the thread as covering threats sent or posted &quot;in a manner in which another person may view it&quot; — can apply to a diary entry never intended for other eyes, and one skeptic of the charge nonetheless thought Anthropic was right to alert police. Another defended the company&\#x27;s decision as a damned-if-you-do dilemma, recalling headlines in which, the commenter said, OpenAI failed to report a shooter, while others argued the episode shows chat logs are surveilled corporate records rather than private confidences, with one recommending self-hosted open-source models for sensitive writing.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/tech-industry/artificial-intelligence/anthropic-reports-florida-womans-claude-diary-threat-to-shoot-up-sheriffs-office-felony-charge-follows-its-at-least-the-third-such-conversation-to-reach-police-since-august">Anthropic reports Florida woman ’s Claude ‘ diary ’ threat to shoot up...</a></li>
<li><a href="https://decrypt.co/380119/florida-woman-claude-diary-anthropic-reported-police">A Florida Woman Used Claude as a Diary . An Anthropic ... - Decrypt</a></li>
<li><a href="https://www.techspot.com/news/114091-florida-woman-used-claude-diary-anthropic-reported-shoot.html">Florida woman used Claude as a diary , then Anthropic reported an...</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/artificial-intelligence/anthropic-reports-florida-womans-claude-diary-threat-to-shoot-up-sheriffs-office-felony-charge-follows-its-at-least-the-third-such-conversation-to-reach-police-since-august">Anthropic reports Florida woman’s Claude ‘diary... | Tom&#x27;s Hardware</a></li>
<li><a href="https://privacy.claude.com/">Home | Anthropic Privacy Center</a></li>

</ul>
</details>

**Tags**: `#AI privacy`, `#Anthropic`, `#legal issues`, `#LLM policy`, `#surveillance`

---

<a id="item-tech-news-5"></a>
### [Stratechery: Apple&\#x27;s Privacy Model May Lose AI-Native Users to Meta&\#x27;s Muse](https://stratechery.com/2026/apple-and-a-hackers-future/) ⭐️ 7.0/10

A Stratechery analysis by Ben Thompson argues that Apple&\#x27;s privacy-centric permissions model, including full-disk-access grants, may cost the company relevance as users choose platforms based on how well general-purpose AI agents run on them. The piece focuses on Meta&\#x27;s general-purpose agent Muse, and Thompson writes that he can, &quot;for the first time,&quot; envision a future where he doesn&\#x27;t buy Apple by default. This is strategic commentary rather than a shipped capability or measured result, and it lands amid an active privacy controversy: an excerpt quoted in the discussion cites a recent full-disk-access announcement and columnist Jason Aten&\#x27;s report that Muse sent him an unsolicited notification referencing a private Apple Messages thread he never granted the agent permission to read.

hackernews · maguay · Oct 5, 10:05 · [Discussion](https://news.ycombinator.com/item?id=49962857)

**「Apple&\#x27;s TCC permissions model」** Apple&\#x27;s macOS security model rests on a permissions framework known as Transparency, Consent, and Control, which requires users to explicitly grant sensitive capabilities such as full-disk access before an app can read files across the machine. Thompson&\#x27;s argument grew out of a concrete episode in which an AI agent running on his Mac detected and helped remediate a macOS vulnerability, prompting his framing that &quot;the thing about AI, however, particularly agents, is that they make anyone a hacker&quot; — the lens through which he sees Apple&\#x27;s restrictive design philosophy colliding with an agentic computing future.

**「What It Means for Mac Users」** Apple has tightened macOS Full Disk Access to require explicit consent, citing AI-agent risks after Meta&\#x27;s Muse reportedly surfaced a columnist&\#x27;s private Apple Messages exchange even though he had never enabled that permission. The actionable takeaway for users is to treat full-disk access — normally granted to backup software, as one commenter noted — as a deliberate decision rather than a setup default when installing agents like Muse. The tension cuts both ways: these restrictions may limit what agents can do on macOS, which is exactly the trade-off Thompson argues could lead AI-native users to stop buying Apple by default, though that remains his projection rather than a measured shift in purchasing.

**「Community Discussion」** Several commenters argued that giving full-disk access to Meta software on a primary computer would effectively end privacy protections, and one also faulted Thompson for leaving VNC/Apple Remote Desktop open to the internet with no filtering — exactly the exposure Apple&\#x27;s protections exist to guard against. Others engaged with the platform-choice thesis itself: one agreed that Apple&\#x27;s roughly three-to-four-year default upgrade cycle is no longer guaranteed, while another countered that Apple has always imperfectly tried to do the right thing.

<details><summary>References</summary>
<ul>
<li><a href="https://stratechery.com/2026/apple-and-a-hackers-future/">Apple and a Hacker’s Future – Stratechery by Ben Thompson</a></li>
<li><a href="https://app.sandhill.io/posts/apple-and-a-hacker-s-future">Apple and a Hacker’s Future - SandHill.io</a></li>
<li><a href="https://www.implicator.ai/apple-will-require-explicit-consent-for-mac-full-disk-access-citing-ai-agent-risks/">Apple Tightens Mac Full Disk Access Over AI Agent Risks</a></li>
<li><a href="https://techgig.com/news/cybersecurity/apple-changes-macos-privacy-settings-to-curb-ai-agent-abuse/134683396">Apple changes macOS privacy settings to curb AI agent abuse</a></li>
<li><a href="https://www.purevpn.com/blog/apple-announces-new-mac-privacy-controls-amid-meta-muse-scrutiny/">Apple Announces New Mac Privacy Controls Amid Meta Muse Scrutiny</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#AI agents`, `#Meta`, `#privacy`, `#platform strategy`

---

<a id="item-tech-news-6"></a>
### [Qualcomm reportedly licenses patents on Huawei&\#x27;s LogicFolding chip technology](https://www.bloomberg.com/news/articles/2026-10-05/qualcomm-licenses-patents-on-huawei-s-logicfolding-chip-tech) ⭐️ 7.0/10

A Bloomberg report published October 5, 2026 says Qualcomm has taken licenses to Huawei&\#x27;s LogicFolding chip patents, and Huawei&\#x27;s own newsroom published an announcement of a broad patent agreement between the two companies. The deal is notable because it inverts the more common direction of semiconductor IP flow, in which US chipmakers license their technology to Chinese firms; here a leading US chip designer is reportedly paying for patents developed by Huawei. The submission itself offers little technical depth on what LogicFolding covers, and the terms of the agreement — including payment direction and size — are not disclosed in the available material.

hackernews · 0xedb · Oct 5, 07:46 · [Discussion](https://news.ycombinator.com/item?id=49961861)

**「Entity List context and the deal&\#x27;s actual scope」** Huawei has been on the US Commerce Department&\#x27;s Entity List since 2019, a designation that generally restricts US companies from transactions with it without a government license, which is why any direct patent arrangement between Qualcomm and Huawei draws export-control scrutiny. Per the companies&\#x27; joint announcements, the arrangement is broader than the LogicFolding patents alone: it is a multi-year, broad patent license agreement with cross-licenses spanning both firms&\#x27; portfolios in 5G, compute, AI, and networking, and also includes Qualcomm&\#x27;s purchase of certain Huawei US patents in those areas.

**「Entity List compliance gates similar IP deals」** Qualcomm&\#x27;s agreement — a multi-year cross-license spanning 5G, compute, AI, and networking patents, plus Qualcomm&\#x27;s purchase of certain Huawei U.S. patents — demonstrates that IP transactions with an Entity List company can be structured, giving other U.S. firms a concrete template for deals where the usual IP flow is reversed. Any company pursuing a similar arrangement must still conduct a defensible export-control review covering Huawei&\#x27;s exact Entity List entry, the applicable EAR provisions, and the Huawei Foreign-Produced Direct Product rule, since a single name search cannot establish the regulatory scope of the transaction.

**「Community discussion」** The most pointed question in the comments came from a reader asking how Qualcomm can enter a patent agreement with Huawei while Huawei remains on the US Entity List — a legality concern the report does not appear to address. Other commenters relayed an explicitly unverified claim that Huawei will net revenue from Qualcomm, framing it as a shift from buyer of Western IP to technology licensor, and one described LogicFolding as a multi-layer wafer approach whose shorter inter-layer signal paths reduce overall heat; these are reader claims, not confirmed deal terms.

<details><summary>References</summary>
<ul>
<li><a href="https://www.qualcomm.com/news/releases/2026/10/huawei-and-qualcomm-announce-broad-patent-license-agreement">Huawei and Qualcomm Announce Broad Patent License Agreement</a></li>
<li><a href="https://www.huawei.com/en/news/2026/10/qualcomm-broad-patent-agreement">Huawei and Qualcomm Announce Broad Patent License Agreement</a></li>
<li><a href="https://getembargo.com/blog/huawei-bis-entity-list-history">Huawei BIS Entity List: Timeline, FDPR &amp; Screening (2026)</a></li>
<li><a href="https://www.qualcomm.com/news/releases/2026/10/huawei-and-qualcomm-announce-broad-patent-license-agreement">Huawei and Qualcomm Announce Broad Patent License Agreement</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#patents`, `#huawei`, `#qualcomm`, `#geopolitics`

---

<a id="item-tech-news-7"></a>
### [Gigafish: 3.9B Chess Positions Distilled from Stockfish Released on Hugging Face](https://www.reddit.com/r/MachineLearning/comments/1wxz5qq/distilling_stockfish_on_a_billion_positions_full/) ⭐️ 7.0/10

A machine learning practitioner distilled Stockfish&\#x27;s depth-limited value function into ResNet and vision transformer \(ViT\) models trained on 1 billion chess positions and released the full 3.9-billion-position Gigafish dataset on Hugging Face \(gigafish-3.8b-d10\), built from positions spanning 37 months of Lichess games. The author held search depth constant so each training label approximates the value of the search tree beneath it, testing the hypothesis that a network reproducing that evaluation quickly enough could compete with Stockfish&\#x27;s small NNUE network — a stated goal, not a demonstrated result in the post. On training dynamics, the ViT was slow to learn the board while a CNN progressed much faster early on due to its geometric inductive biases, and the author reports the best results from combining the two architectures.

reddit · r/MachineLearning · /u/microscope1024 · Oct 5, 04:11

**「Background」** Stockfish evaluates chess positions by running a depth-limited search and scoring leaf nodes with NNUE, a very small neural network chosen for its speed. The distillation premise behind this project is that a depth-limited value function implicitly approximates the search tree beneath it, so a model trained to reproduce those evaluations could substitute for the search itself with a single network pass. Because the target was a fixed depth rather than the engine&\#x27;s full variable-depth search, the student model receives a consistent signal to imitate.

**「What practitioners can do with it」** Chess-AI and ML researchers can now train or benchmark board-evaluation models against 3.9 billion Stockfish-labeled positions without running expensive depth-limited searches themselves, since the full Gigafish dataset \(depth-10 evaluations built from 37 months of Lichess games\) is downloadable on Hugging Face. For teams doing similar distillation work, the author&\#x27;s blog notes that loss continued decreasing for the entire training run, a concrete signal that scaling data volume still pays off rather than treating current dataset sizes as sufficient.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.lukesalamone.com/posts/distilling-stockfish/">Distilling Stockfish with One Billion Positions :: Luke Salamone &#x27;s Blog</a></li>

</ul>
</details>

**Tags**: `#machine-learning`, `#knowledge-distillation`, `#chess-ai`, `#vision-transformer`, `#open-datasets`

---

<a id="item-tech-news-8"></a>
### [Yandex Music reports single transformer Sona replaced its multi-stage recommender in A/B test](https://www.reddit.com/r/MachineLearning/comments/1wy4qxm/sona_one_transformer_replaced_our_15_candidate/) ⭐️ 7.0/10

Engineers on Yandex Music report that Sona, a single end-to-end transformer, replaced the service&\#x27;s production recommender pipeline — 15+ candidate generators, a pre-ranker, and a ranker — in an A/B test, though it has not yet rolled out to full traffic. The model reads up to 8,192 user events, which its History Compression scheme splits into 6,144 older and 2,048 recent events linked through cross-attention and one full-history self-attention layer, with a 7-layer stack then running only on the recent block — a design the team says roughly halves inference cost versus full attention. The decoder and a Ranking Module share one encoder pass per request, and candidate items come out of beam search as Semantic IDs that are scored immediately. In the team&\#x27;s 7-day A/B test on smart speakers \(15% of users per arm\), Sona reportedly delivered +4.53% Active Users and +6.30% Total Listening Time over the production control, both significant at p &lt; 0.01; these self-reported results accompany an arXiv paper \(2608.11015\) rather than independent verification, and catalog coverage came in lower than the production stack&\#x27;s, with a long-term A/B test now underway.

reddit · r/MachineLearning · /u/SettingAccording8986 · Oct 5, 10:07

**「From cascade to single model」** Traditional production recommenders run as multi-stage cascades: many candidate generators propose items, then separate pre-ranking and ranking models order them, and large industrial systems can run dozens of specialized ranking models, each tuned to a single goal such as a click. Sona follows the broader shift, inspired by large language models, toward single end-to-end models that absorb work once split across specialized components. The model&\#x27;s design and ablations are documented in a public arXiv technical report \(2608.11015, revised August 12, 2026\).

**「Pipeline consolidation looks viable, but the coverage gap sets the condition」** Yandex&\#x27;s seven-day live experiment on smart speakers gives recommendation engineers a production datapoint that a single generative transformer can outperform a full cascade — +4.53% Active Users and +6.30% Total Listening Time at p&lt;0.01 — making it reasonable for teams maintaining multi-stage retrieval-and-ranking stacks to test consolidation rather than treat specialized candidate generators as required. The concrete compatibility concern is that Sona&\#x27;s catalog coverage is lower than the production stack&\#x27;s, a regression Yandex has not yet explained and is still investigating while a long-term A/B runs before any full-traffic rollout, so teams replicating this approach should measure catalog coverage alongside engagement metrics rather than judge success on listening time alone.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2608.11015">Sona Technical Report</a></li>
<li><a href="https://gist.github.com/AnthonyAlcaraz/1e483abbf10a66f0592dc9d20a204bf8">Agentic AI changes how fast recommender ... - 2026-09-11 · GitHub</a></li>
<li><a href="https://www.marktechpost.com/2026/10/05/yandex-introduces-sona-a-single-generative-recommender-that-replaces-entire-recommendation-cascade/">Yandex Introduces Sona: A Single Generative Recommender That...</a></li>
<li><a href="https://korshunov.ai/en/article/31318-yandex-replaces-15-stage-recommendation-cascade-with-single-generative-sona/">Yandex replaces 15+ stage recommendation cascade with single ...</a></li>

</ul>
</details>

**Tags**: `#recommender-systems`, `#transformers`, `#generative-models`, `#production-ml`, `#sequence-modeling`

---

<a id="item-tech-news-9"></a>
### [Quad9 Refuses French Piracy Blocks, Risks €580,000 Daily Fine](https://torrentfreak.com/dns-resolver-quad9-rejects-french-piracy-blocks-weighs-exit-as-bein-seeks-up-to-e580k-a-day/) ⭐️ 7.0/10

Swiss non-profit DNS resolver Quad9 is refusing to enforce French court-ordered blocks on 58 domains accused of carrying pirated beIN Sports streams, and beIN is seeking penalties of €10,000 per domain per day — up to €580,000 daily. The Paris court heard the case last Thursday and is expected to rule within three weeks. Quad9 says it has never blocked a domain and, because it collects no user data, cannot apply blocks to French users only; it would have to block worldwide or exit the French market. The resolver also called the French law passed in July, which allows domains to be blacklisted automatically in real time, &quot;reckless and dangerous.&quot;

telegram · zaihuapd · Oct 5, 08:05

**「Why a global DNS resolver cannot block France alone」** Quad9 is a Swiss non-profit that operates a public recursive DNS resolver for users worldwide; because it deliberately collects no user data, it cannot restrict a court-ordered block to French visitors, so blocking the 58 domains beIN Sports targets would either apply globally or amount to leaving the French market. The broadcaster is pressing the Paris court for €10,000 per domain per day across those piracy domains, with the case heard last Thursday and a decision expected within about three weeks. The dispute unfolds under France&\#x27;s tightened enforcement regime, including a law passed in July that allows domains to be added to blocklists automatically and in real time — a mechanism Quad9 has called &\#x27;reckless and dangerous&\#x27;.

**「Impact」** Both of Quad9&\#x27;s stated options land directly on users: complying with the order would block all 58 beIN Sports domains for every user of the resolver worldwide, since Quad9 says it collects no user data that would let it limit enforcement to France, while refusing points toward the non-profit exiting the French market. If the court rules against it, French users of the recursive resolver — the servers that receive client DNS queries and resolve domain names to IP addresses — would need to repoint their devices at a different DNS provider.

<details><summary>References</summary>
<ul>
<li><a href="https://torrentfreak.com/dns-resolver-quad9-rejects-french-piracy-blocks-weighs-exit-as-bein-seeks-up-to-e580k-a-day/">DNS Resolver Quad 9 Rejects French Piracy Blocks ... * TorrentFreak</a></li>
<li><a href="https://vpnlab.io/en/quad9-france-exit-bein-piracy-blocking-fines-2026-2654">Quad 9 may quit France over beIN &#x27;s piracy block fines</a></li>
<li><a href="https://dnschecker.org/">DNS Checker - DNS Check Propagation Tool</a></li>

</ul>
</details>

**Tags**: `#DNS`, `#internet-governance`, `#censorship`, `#privacy`, `#copyright-enforcement`

---

<a id="item-tech-news-10"></a>
### [OpenAI to Add Invisible Watermarks to Some EU ChatGPT and Codex Text Outputs](https://openai.com/index/eu-text-provenance/) ⭐️ 7.0/10

OpenAI announced that, in the coming weeks, it will embed machine-readable invisible watermarks into qualifying ChatGPT and Codex text outputs in the EU to meet the EU AI Act&\#x27;s content transparency requirements. API users can also opt in to watermarking for some models, though it is disabled by default. In parallel, OpenAI is opening applications for researchers and professional institutions to access its text watermark detector. The rollout is an announced plan scoped to the EU, and the announcement does not specify the technique&\#x27;s robustness or false-positive behavior.

telegram · zaihuapd · Oct 5, 15:25

**「Regulatory context and the state of watermarking」** The EU AI Act obliges providers of generative AI systems to make generated text identifiable in a machine-readable way, and this watermarking rollout is OpenAI&\#x27;s measure to satisfy that transparency obligation. OpenAI characterizes text watermarking and detection as early technologies with significant limitations — it notes that editing generated text can make the invisible marks harder to detect — and says its phased approach reflects both the legal requirement and these technical constraints.

**「What this means for EU deployments」** The move addresses Article 50 of the EU AI Act, whose transparency rules have applied since 2 August 2026 and require AI-generated text to be disclosed as artificially generated. EU-facing organizations should note the asymmetry: consumer ChatGPT and Codex outputs will be watermarked automatically, but API watermarking is off by default, so API developers serving EU users may need to actively enable it to cover their own disclosure obligations.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/eu-text-provenance/">Our approach to EU text provenance rules - OpenAI</a></li>
<li><a href="https://techcrunch.com/2026/10/05/openai-will-start-watermarking-chatgpts-text-in-the-eu/">OpenAI will start watermarking ChatGPT’s text in the EU</a></li>
<li><a href="https://ai-act-service-desk.ec.europa.eu/en/ai-act/article-50">AI Act Service Desk - Article 50: Transparency obligations ...</a></li>
<li><a href="https://digital-strategy.ec.europa.eu/en/factpages/quick-facts-transparency-rules-ai-systems">Quick Facts: Transparency rules for AI systems | Shaping ...</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#AI watermarking`, `#EU AI Act`, `#ChatGPT`, `#content provenance`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Brazilian Stocks Jump as Flávio Bolsonaro Becomes Heavy Runoff Favorite](https://www.cnbc.com/2026/10/05/brazilian-stocks-jump-bolsonaro-now-heavy-favorite-to-win-presidency.html) ⭐️ 8.0/10

Brazilian stocks surged Monday after first-round election results — more than 47% of the vote for challenger Flávio Bolsonaro, son of former president Jair Bolsonaro, nearly 2 percentage points ahead of President Lula and better than polls had expected — made him the heavy favorite on prediction markets, with odds above 80% on Kalshi and 85% on Polymarket for the Oct. 25 runoff. The iShares MSCI Brazil ETF \(EWZ\) rose more than 12%, U.S.-listed Itau Unibanco gained 15%, Banco Bradesco jumped 19%, and the Bovespa index climbed 8%.

rss · CNBC Finance · Oct 5, 20:41

**「Background」** Brazil holds a runoff when no presidential candidate wins a first-round majority, with this year&\#x27;s decisive vote set for Oct. 25. Flávio Bolsonaro, a senator for Rio de Janeiro since 2019 and the eldest son of former president Jair Bolsonaro — whom Lula defeated in 2022 — has promised greater fiscal discipline, a stance investors favor given Brazil&\#x27;s government deficit of nearly 10% of GDP in June.

**「Impact」** Investors in Brazilian equities are pricing in the fiscal discipline Bolsonaro has promised — a contrast with a deficit running near 10% of GDP in June — but the actual policy outlook stays contingent on the Oct. 25 runoff vote.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Fl%C3%A1vio_Bolsonaro">Flávio Bolsonaro - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Brazil`, `#elections`, `#emerging-markets`, `#equity-markets`, `#political-risk`

---

<a id="item-finance-news-2"></a>
### [Gas-Only Cars Fall Below Half of Global New-Car Sales for the First Time](https://asia.nikkei.com/business/automobiles/gas-vehicles-fall-under-50-of-global-new-auto-sales-for-first-time) ⭐️ 7.0/10

Global sales of gasoline- and diesel-only vehicles — excluding hybrids and other electrified models — fell 10% year on year to 20.25 million in the first half of 2026, or 49% of new car sales, down 3 percentage points and below the 50% mark for the first time, Nikkei Asia reported. Pure electric vehicle sales rose 12% to 6.87 million, taking a 17% share, as growth in Europe offset declines in China and North America; Nikkei attributed the drop in gas-car demand partly to oil prices pushed higher by the Middle East conflict.

telegram · zaihuapd · Oct 6, 01:04

**「Background」** Pure gasoline cars — vehicles powered only by an internal combustion engine, with no hybrid or plug-in electric drive — had always made up the majority of global new car sales, while electric models grew from a small base. By 2025, roughly one in four new cars sold worldwide was electric, including over half of sales in China and nearly all in Norway.

**「Impact」** Automakers that still depend on combustion-only models face a shrinking share of global new-car demand as electric vehicles take a growing slice of sales.

<details><summary>References</summary>
<ul>
<li><a href="https://ourworldindata.org/electric-car-sales">Tracking global data on electric vehicles - Our World in Data</a></li>

</ul>
</details>

**Tags**: `#automotive industry`, `#electric vehicles`, `#global auto sales`, `#energy transition`, `#oil demand`

---