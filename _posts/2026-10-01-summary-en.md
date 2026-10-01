---
layout: default
title: "Horizon Summary: 2026-10-01 (EN)"
date: 2026-10-01
lang: en
---

> From 41 items, 12 important content pieces were selected

---

**Technology News**
1. [Google announces Gemini 4 Argon frontier model, broad availability still pending](#item-tech-news-1) ⭐️ 9.0/10
2. [EDG publishes its long-proprietary C++ compiler front-end on GitHub](#item-tech-news-2) ⭐️ 8.0/10
3. [Survey by 32 Researchers Spans Tokenization Algorithms, Security, and Alternatives](#item-tech-news-3) ⭐️ 7.0/10
4. [CO2Jump: Training-Free Sampler Improves Text-Image Consistency in Joint Generation](#item-tech-news-4) ⭐️ 7.0/10
5. [DeepSeek reportedly open-sources Huawei Ascend ports of its core AI stack](#item-tech-news-5) ⭐️ 7.0/10
6. [Cloudflare announces plan to become a public certificate authority](#item-tech-news-6) ⭐️ 7.0/10
7. [Baseten Enables Kimi K3 in OpenAI Codex, Billed to Existing OpenAI Commitments](#item-tech-news-7) ⭐️ 7.0/10
8. [Reddit to End RSS Feeds and Close Public API, Citing AI Bot Abuse](#item-tech-news-8) ⭐️ 7.0/10
9. [OpenAI says it disrupted model distillation campaign tied to Moonshot-affiliated individuals](#item-tech-news-9) ⭐️ 7.0/10

**Financial News**
1. [Kalshi, Polymarket trading volumes on some products raise questions amid massive growth](#item-finance-news-1) ⭐️ 7.0/10
2. [China warns of &\#x27;firm response&\#x27; if EU restricts Chinese businesses](#item-finance-news-2) ⭐️ 7.0/10
3. [China reportedly tightens IPO criteria for humanoid robot startups](#item-finance-news-3) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Google announces Gemini 4 Argon frontier model, broad availability still pending](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-argon/) ⭐️ 9.0/10

Google announced Gemini 4 Argon, its next-generation frontier AI model, headlining agentic capabilities — announcement text quoted in the discussion claims Argon agents are already migrating C/C++ codebases to Rust across Google. Availability is the caveat: Google says it is still gathering feedback from early testers and iterating on guardrails before opening Argon to developers, enterprises, and consumers &\#x27;as soon as possible.&\#x27; The excerpted announcement includes no benchmarks, pricing, or release dates, so the capability claims remain unverified vendor statements at this stage.

hackernews · bradleyg223 · Sep 30, 20:04 · [Discussion](https://news.ycombinator.com/item?id=49913571)

**「Background」** Gemini 4 Argon is the newest entry in Google&\#x27;s Gemini model family, introduced on September 30, 2026 by Koray Kavukcuoglu, SVP of Google DeepMind, as a frontier model for long-horizon work such as real-world software engineering, legal and financial knowledge work, and cyber defense. Although coverage describes it as Alphabet&\#x27;s most advanced model yet, Google&\#x27;s announcement frames it as &quot;rolling out soon&quot; rather than a broadly shipped release, with reporting noting the model reaches cybersecurity teams before developers.

**「Limited release leaves most developers waiting」** Gemini 4 Argon is not broadly usable yet: Google unveiled it to a small group of cybersecurity partners and says it will gather early-tester feedback on guardrails before making the model available to developers, enterprises, and consumers, so most teams cannot access or evaluate it today. Its claimed benchmark lead over Anthropic&\#x27;s Claude Opus 5.5, Claude Fable 5.1, and OpenAI&\#x27;s GPT-6 Astra comes from Google&\#x27;s own published benchmarks, so organizations selecting models for software development, professional knowledge work, or cybersecurity operations should treat the performance claims as unverified until broader access or independent testing arrives.

**「Community Discussion」** Commenters flagged the staged rollout — one quipped that Google still can&\#x27;t shake its &\#x27;can&\#x27;t release a model&\#x27; reputation — and debated what the release signals for competition: one argued this year&\#x27;s repeated lead changes among labs disprove Dario Amodei&\#x27;s winner-take-all &\#x27;concentrating&\#x27; thesis, with AI capacity spreading across hyperscalers, neoclouds, startups, and both GPU and ASIC vendors, while another urged developers to keep models and providers replaceable since frontier labs keep leapfrogging each other. Separately, one user recounted an earlier Gemini model autonomously debugging a GPU driver and authoring an LD\_PRELOAD shim to get ROCm llama.cpp running, offered as anecdotal evidence of rapid agentic progress.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-argon/">Introducing Gemini 4 Argon - The Keyword</a></li>
<li><a href="https://www.datacamp.com/blog/gemini-4-argon">Gemini 4 Argon: Benchmarks, Pricing, and Access | DataCamp</a></li>
<li><a href="https://www.cnbc.com/2026/09/30/google-gemini-4-argon-ai.html">Google rolls out Gemini 4 Argon, its most advanced model - CNBC</a></li>
<li><a href="https://venturebeat.com/technology/google-unveils-gemini-4-argon-retaking-benchmark-lead-over-openai-and-anthropic-but-in-limited-release">Google unveils Gemini 4 Argon, retaking benchmark lead over ...</a></li>
<li><a href="https://www.trendingtopics.eu/gemini-4-argon-google-anthropic-openai/">Google Finally Brings Gemini 4 Into the Fight Against ...</a></li>
<li><a href="https://www.axios.com/2026/09/30/google-gemini-4">Google unveils Gemini 4, long-awaited answer to OpenAI and ...</a></li>

</ul>
</details>

**Tags**: `#artificial-intelligence`, `#google`, `#large-language-models`, `#gemini`, `#ai-industry`

---

<a id="item-tech-news-2"></a>
### [EDG publishes its long-proprietary C++ compiler front-end on GitHub](https://edgcpp.org/#transition) ⭐️ 8.0/10

Edison Design Group \(EDG\) has made the source code of its long-proprietary C++ compiler front-end publicly available on GitHub at github.com/edgcpp/compiler, with an announcement and documentation hosted at edgcpp.org. Hacker News commenters identify the license as Apache-2.0 WITH LLVM-exception, and one notes the repository&\#x27;s commit history reaches back to 1990, an unusual amount of preserved history for an open-sourcing. Commenters report that EDG the company is winding down, citing the firm&\#x27;s Wikipedia article and a Herb Sutter trip report, which suggests the release accompanies that transition and leaves long-term maintenance uncertain. The front-end has long been embedded in commercial C++ tooling, most visibly powering Visual C++&\#x27;s IntelliSense rather than Microsoft&\#x27;s own compiler front-end.

hackernews · iandinwoodie · Sep 30, 19:26 · [Discussion](https://news.ycombinator.com/item?id=49913192)

**「Background」** Edison Design Group \(EDG\) developed and licensed its C++ front end as proprietary code for roughly 30 years, building a reputation as one of the most respected and widely used compiler front ends in the industry. Its most visible embedding is inside Microsoft Visual C++, where IntelliSense completion reportedly runs on the EDG front end rather than Microsoft&\#x27;s own compiler front end — a detail commenters point to when explaining why the release matters to the C++ tooling ecosystem.

**「Impact」** Tool vendors and compiler developers who previously needed a commercial license to embed EDG&\#x27;s front-end can now inspect, modify, and redistribute the code under Apache 2.0 with the LLVM exception, with community contributions accepted under The C++ Alliance&\#x27;s stewardship as the project&\#x27;s nonprofit home. Projects that build on EDG-based tooling should review the license terms for compatibility, and, given community reports that the company is winding down, weigh that continued maintenance now rests with the C++ Alliance and outside contributors rather than the original vendor.

**「Community Discussion」** Commenter jabl argued the announcement omits the likely driving context: that EDG the company is winding down, citing the firm&\#x27;s Wikipedia entry and a Herb Sutter trip report as their references. Others weighed what the release enables: badsectoracula wondered whether EDG&\#x27;s source-to-source compilation could transpile C++ libraries into other languages such as Free Pascal, vintagedave recalled that Visual C++ uses the EDG front-end for IntelliSense, and trebligdivad highlighted the unusual in-repo history stretching back to 1990.

<details><summary>References</summary>
<ul>
<li><a href="https://techplanet.today/post/edg-c-front-end-goes-open-source-a-historic-moment-for-the-c-community">EDG C++ Front-End Goes Open Source: A Historic Moment for the ...</a></li>
<li><a href="https://edgcpp.org/">Open Source Transition · EDGCPP</a></li>
<li><a href="https://www.phoronix.com/news/EDG-CPP-Open-Sourced">EDG C/ C++ Front - End Open -Sourced - Phoronix</a></li>

</ul>
</details>

**Tags**: `#C++`, `#compilers`, `#open-source`, `#developer-tools`, `#programming-languages`

---

<a id="item-tech-news-3"></a>
### [Survey by 32 Researchers Spans Tokenization Algorithms, Security, and Alternatives](https://www.reddit.com/r/MachineLearning/comments/1wuccjf/tokenization_a_survey_for_modern_nlp_r/) ⭐️ 7.0/10

A group of 32 self-described tokenizer researchers has released a survey that its authors call the most comprehensive overview of tokenization in modern NLP, compiled over roughly eight months. The paper covers tokenization algorithms, evaluation, multilinguality, encodings, and theory, as well as potential replacements such as latent and visual tokenization, plus adjacent topics including constrained generation, token healing, and tokenizer security. The announcement is a self-submission on r/MachineLearning by one of the authors, linking to alphaXiv, so the breadth and authorship claims come from the post itself and have not been independently verified.

reddit · r/MachineLearning · /u/mcmcmcmcmcmcmcmcmc\_ · Sep 30, 18:13

**「From documented gap to comprehensive survey」** Tokenization is the stage of language modeling that converts raw text into the discrete units—typically subwords produced by algorithms such as byte-pair encoding—that models read and generate, and its design choices shape vocabulary size, multilingual coverage, and downstream model behavior. Efforts to consolidate the field predate this survey: a February 2025 systematic review of discrete tokenizers on arXiv noted that a comprehensive survey dedicated to them was still &quot;conspicuously absent&quot; from the literature, and set out to fill that gap with a review of their design principles, applications, and challenges.

**「Impact」** Practitioners building or auditing LLM pipelines—particularly for multilingual workloads or security-sensitive deployments—get a single reference for tokenizer design, evaluation, and known attack surfaces, which the authors argue is otherwise scattered and understudied. A concrete use is to consult it as a checklist when selecting or reviewing a tokenizer, while treating it as a reference survey rather than independently reviewed findings.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2502.12448v1">From Principles to Applications: A Comprehensive Survey of ...</a></li>

</ul>
</details>

**Tags**: `#tokenization`, `#NLP`, `#large language models`, `#survey`, `#machine learning`

---

<a id="item-tech-news-4"></a>
### [CO2Jump: Training-Free Sampler Improves Text-Image Consistency in Joint Generation](https://www.reddit.com/r/MachineLearning/comments/1wtyl5m/concurrent_image_understanding_and_generation/) ⭐️ 7.0/10

Researchers from Google, Google DeepMind, and Stony Brook University have posted a paper claiming NeurIPS 2026 acceptance that introduces CO2Jump, a training-free self-correcting sampler for coupled Markov jump processes in joint text-image models. The sampler uses text confidence and cross-modal attention to guide image updates during sampling, and allows low-confidence image tokens to be re-masked and regenerated so earlier decisions can be revised, all with a single model forward pass per denoising step and no training beyond the task-specific fine-tuning applied equally to compared methods. Evaluation covers image editing, maze solving, and nonogram puzzles using three newly introduced datasets \(JEdit-1M, JMaze-200K, JNono-200K\), where joint accuracy requires both the textual answer and the generated image to be correct. The authors report that across 8 to 512 sampling steps, CO2Jump was the only sampler compared that improved monotonically on both editing quality and grounding, though results were obtained on task-specific fine-tuned models and constrained benchmarks rather than general-purpose generation.

reddit · r/MachineLearning · /u/Upstairs\_Theme2785 · Sep 30, 07:28

**「Background」** CO2Jump sits within masked discrete diffusion, a class of generative models that build outputs from masked tokens and can flip low-confidence tokens back to a masked state during sampling; the paper&\#x27;s own background section identifies masked diffusion models and remasking as the technical foundation for its self-correcting approach. The work also reflects a newer research framing that treats multimodal output as a single unified stochastic process, allowing a model to perform image understanding and generation concurrently rather than as separate stages, which is what gives rise to the text-image consistency problem the sampler addresses.

**「Why it matters」** For researchers working on discrete diffusion and Markov jump process models, CO2Jump offers a drop-in sampling method that targets text-image consistency without additional training, making it testable against existing fine-tuned checkpoints. The three released datasets provide constrained tasks where correctness of both modalities can be verified automatically, and the authors are soliciting suggestions for additional tasks with jointly evaluable text-image consistency.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/papers/2607.13188.md">huggingface.co/ papers /2607.13188.md</a></li>
<li><a href="https://www.alphaxiv.org/abs/2607.13188">Concurrent Image Understanding and Generation ... | alphaXiv</a></li>

</ul>
</details>

**Tags**: `#machine-learning`, `#generative-models`, `#multimodal`, `#discrete-diffusion`, `#sampling-methods`

---

<a id="item-tech-news-5"></a>
### [DeepSeek reportedly open-sources Huawei Ascend ports of its core AI stack](https://mp.weixin.qq.com/s/X41mKH4Ds-VXUAnK6M8Eww) ⭐️ 7.0/10

DeepSeek reportedly released open-source Huawei Ascend versions of its core AI infrastructure components on September 30, 2026, giving developers building on Ascend NPUs ports of components that previously existed for the company&\#x27;s NVIDIA platform. The listed projects are TileLang compiler tooling, TileKernels, DeepGEMM Ascend, DeepEP Ascend, FlashMLA, and DeepSelect, spanning a high-level kernel language toolchain, compute libraries, and distributed communication libraries. DeepSeek claims the components reach performance close to hardware limits in multiple tests, and it describes an ongoing joint effort with Huawei on a 128-card supernode solution for the Ascend 950 rather than a completed deployment. The account comes from a brief single-source aggregator post with no repository links or benchmarks attached, so neither the release itself nor the near-hardware-limit performance figures have been independently verified.

telegram · zaihuapd · Sep 30, 03:09

**「DeepSeek&\#x27;s open-source infrastructure stack」** DeepSeek&\#x27;s model efficiency has rested on a suite of open-source kernel and communication libraries originally built for NVIDIA GPUs: DeepGEMM for matrix multiplication, DeepEP for large-scale expert-parallel communication, FlashMLA attention kernels, and supporting tooling such as TileLang. The FlashMLA repository describes the library as powering inference of the DeepSeek-V4.1 model on both NVIDIA GPUs and Huawei Ascend NPUs, and the newly published DeepGEMM-Ascend port is stated to be fully API-compatible with the original while supporting BF16, FP8, and FP4 GEMM operations. In other words, the Ascend releases are ports of the same toolkit DeepSeek previously shipped for NVIDIA hardware, reworked for a different chip architecture rather than entirely new software.

**「Impact」** Teams deploying DeepSeek models on Huawei Ascend hardware can now adopt the same open-source optimization stack—DeepGEMM, DeepEP, FlashMLA, and TileLang tooling—that DeepSeek maintains for its NVIDIA platform, addressing the CUDA-to-CANN porting costs that third-party comparisons highlight as a key trade-off when weighing Ascend against NVIDIA GPUs. The near-hardware-limit performance figures are DeepSeek&\#x27;s own claims rather than independently benchmarked results, and the Ascend 950 128-card supernode is work in progress with Huawei rather than a shipped product, so operators should benchmark these ports on their own clusters before committing production inference workloads.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/deepseek-ai/DeepGEMM-Ascend">GitHub - deepseek-ai/DeepGEMM-Ascend: DeepGEMM-Ascend: clean ...</a></li>
<li><a href="https://github.com/deepseek-ai/FlashMLA">GitHub - deepseek-ai/FlashMLA: FlashMLA: Efficient Multi-head ...</a></li>
<li><a href="https://startupfortune.com/deepseek-open-sources-chip-tools-that-could-let-huawei-replace-nvidia-in-china/">DeepSeek open sources chip tools that could let Huawei ...</a></li>
<li><a href="https://www.spheron.network/blog/huawei-ascend-950-vs-nvidia-b300-b200-llm-inference-2026/">Huawei Ascend 950 vs NVIDIA B300 and B200 for LLM Inference ...</a></li>

</ul>
</details>

**Tags**: `#deepseek`, `#huawei-ascend`, `#ai-infrastructure`, `#open-source`, `#ai-hardware`

---

<a id="item-tech-news-6"></a>
### [Cloudflare announces plan to become a public certificate authority](https://blog.cloudflare.com/cloudflare-certificate-authority/) ⭐️ 7.0/10

Cloudflare has announced plans to become a public certificate authority, applying to join the Chrome, Apple, Microsoft, and Mozilla root certificate programs and signing an agreement with GlobalSign to acquire a widely trusted root certificate. No certificates have been issued yet, so this is an announced plan rather than a live signing capability, and admission to each trust store still awaits the respective programs&\#x27; review. The new CA is expected to prioritize ACME for automated issuance and renewal, with production-grade Merkle Tree Certificates \(MTC\) planned for the first quarter of 2027 as part of a push toward post-quantum-ready TLS.

telegram · zaihuapd · Sep 30, 06:26

**「Background」** Web browsers and operating systems decide which certificate authorities devices trust by default through root programs, run separately by Chrome, Apple, Microsoft, and Mozilla, and a newly generated root normally spends years in audits and gradual inclusion before most existing devices accept it. That is what makes Cloudflare&\#x27;s agreement to acquire an already-trusted root notable: the root in question is reported to date back to 2012 under GlobalSign, so certificates chained to it could be trusted on currently deployed devices rather than waiting for a fresh root to be admitted \[tool-2-2\]. For day-to-day issuance, the new CA will lean on ACME, the automation protocol that lets web servers request and renew TLS certificates programmatically instead of through manual certificate signing requests.

**「What this means for operators」** Once Cloudflare&\#x27;s acquired root is accepted into the Chrome, Apple, Microsoft, and Mozilla root programs, site operators gain an additional ACME-automated source of publicly trusted TLS certificates backed by a major infrastructure provider. Until those applications are approved and issuance actually begins, certificates from the new CA will not be trusted by clients, so organizations should not plan migrations away from their current CAs yet; the concrete milestone to watch is Cloudflare&\#x27;s stated target of issuing production Merkle Tree Certificates in Q1 2027 for post-quantum readiness.

<details><summary>References</summary>
<ul>
<li><a href="https://ppc.land/cloudflare-targets-q1-2027-for-its-first-quantum-safe-web-certificates/">Cloudflare targets Q1 2027 for its first quantum-safe web certificates</a></li>
<li><a href="https://quantumcomputingreport.com/cloudflare-launches-public-certificate-authority-to-secure-the-web-against-quantum-threats/">Cloudflare Launches Public Certificate Authority to Secure the Web ...</a></li>
<li><a href="https://www.voicendata.com/security/cloudflare-public-certificate-authority-expands-web-pki-12596095">Cloudflare Public Certificate Authority Expands Web PKI</a></li>

</ul>
</details>

**Tags**: `#Cloudflare`, `#certificate-authority`, `#PKI`, `#TLS`, `#post-quantum`

---

<a id="item-tech-news-7"></a>
### [Baseten Enables Kimi K3 in OpenAI Codex, Billed to Existing OpenAI Commitments](https://36kr.com/newsflashes/4005691489112198) ⭐️ 7.0/10

US AI infrastructure company Baseten announced that enterprise users can use the Chinese open-source model Kimi K3 inside OpenAI&\#x27;s Codex coding tool, with usage fees billed directly against the enterprise&\#x27;s existing OpenAI procurement commitment, so no new supplier procurement process is required. According to the 36Kr newsflash, this places Kimi K3 in OpenAI&\#x27;s mainstream enterprise payment and settlement channel, which the report describes as a first for a Chinese open-source model. The item is a short, single-source newsflash relayed via Telegram with no technical details or independent verification, so specifics such as how Baseten routes the calls and which Codex features support the model remain unconfirmed.

telegram · zaihuapd · Sep 30, 11:23

**「OpenAI enterprise billing and Kimi K3」** OpenAI&\#x27;s Codex is the company&\#x27;s programming tool used by enterprise customers, whose usage is billed against pre-negotiated OpenAI purchasing commitments rather than requiring per-vendor contracts. Kimi K3 is an open-source large language model developed by China&\#x27;s Moonshot AI, which enterprises would ordinarily have to adopt through a separate vendor agreement and procurement process outside their OpenAI spending relationship. Until now, that enterprise billing channel covered only OpenAI&\#x27;s own models, so a third-party model like Kimi K3 becoming payable through it is what makes this development notable.

**「Impact on enterprise AI procurement」** Organizations that already hold OpenAI purchase commitments can run Kimi K3 inside Codex, OpenAI&\#x27;s coding agent, with Baseten billing usage against their existing commitment, removing the separate vendor contract and procurement cycle that trialing a Chinese open-source model would normally require. The integration aligns with OpenAI&\#x27;s recent opening of its billing rails to outside consumption, as the company has begun letting third-party applications draw on ChatGPT subscription quota, but the report is a single unverified newsflash, so teams should confirm availability and billing mechanics with Baseten before routing production coding workloads.

<details><summary>References</summary>
<ul>
<li><a href="https://technode.com/2026/09/30/kimi-k3-enters-openais-enterprise-codex-channel-and-billing-system/">Kimi K3 enters OpenAI’s enterprise Codex channel and billing ...</a></li>
<li><a href="https://www.techflowpost.com/en-US/newsletter/138394">Kimi K3 Integrates with OpenAI Codex Enterprise Channel ...</a></li>
<li><a href="https://github.com/openai/codex">GitHub - openai / codex : Lightweight coding agent that runs in your...</a></li>
<li><a href="https://www.163.com/tech/article/L82GG47Q00097U7T.html?clickfrom=w_yw_tech">OpenAI 凌晨大上新！新助手迎战Muse：你关机，它接着干</a></li>

</ul>
</details>

**Tags**: `#大模型生态`, `#开源模型`, `#企业 AI 采购`, `#OpenAI Codex`, `#模型互操作性`

---

<a id="item-tech-news-8"></a>
### [Reddit to End RSS Feeds and Close Public API, Citing AI Bot Abuse](https://techcrunch.com/2026/09/30/reddit-is-killing-rss-feeds-ending-public-api-access-because-of-ai-bots/) ⭐️ 7.0/10

Reddit has announced it will discontinue RSS feed support on November 13, 2026, and shut down public API access by March 2027, saying the feeds have become a common channel for large-scale scraping and automated abuse, especially by AI bots. The company is urging moderators to move to Discord Relay and telling third-party app and bot developers they must complete registration by January 12, 2027, or lose API access. The announcement was reported by TechCrunch; this item is a secondhand repost of that report, so the dates and requirements have not been independently verified here. If carried out as announced, third-party clients, bots, and moderation tooling that depend on feeds or the open API will need to migrate or register before the stated deadlines.

telegram · zaihuapd · Oct 1, 00:27

**「What RSS and Reddit&\#x27;s public API provide」** RSS \(Really Simple Syndication/Rich Site Summary\) is a web feed format that lets users and applications access updates to a website in a standardized way, and Reddit has exposed RSS feeds for its content. Reddit&\#x27;s public API separately allowed programmatic access to its conversations, which tools relied on including social listening products, research tools, and AI products such as AI assistants. These two mechanisms are the long-standing integration points that Reddit now plans to close.

**「Migration deadlines for developers and moderators」** Third-party app and bot developers must complete registration by January 12, 2027 to preserve API access for approved apps and bots until the shutdown, and moderators who rely on RSS channels for their own alerts are advised to review their setups and move workflows to the Discord Relay Devvit app before November 13 to avoid disruption. Some breakage appears unavoidable: Reddit has acknowledged there is no full replacement for certain RSS uses, and readers who depend on Old Reddit, which relies on these interfaces, are among those affected.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/09/30/reddit-is-killing-rss-feeds-ending-public-api-access-because-of-ai-bots/">Reddit is killing RSS feeds and ending public API ... | TechCrunch</a></li>
<li><a href="https://tech.slashdot.org/story/26/09/30/1841213/reddit-is-killing-rss-feeds-ending-public-api-access">Reddit Is Killing RSS Feeds , Ending Public API Access - Slashdot</a></li>
<li><a href="https://techbeat.co/story/reddit-ends-rss-feeds-and-public-api-as-ai-data-revenue-grows">Reddit Ends RSS Feeds and Public API as AI Data Revenue Grows</a></li>
<li><a href="https://mashable.com/tech/reddit-rss-feeds-public-api-shutdown-ai-scraping">Reddit is shutting down RSS and public API access. Blame AI.</a></li>
<li><a href="https://tech.yahoo.com/social-media/articles/reddit-killing-rss-feeds-ending-174500068.html">Reddit is killing RSS feeds and ending public API access ...</a></li>

</ul>
</details>

**Tags**: `#reddit`, `#api`, `#rss`, `#developer-ecosystem`, `#ai-bots`

---

<a id="item-tech-news-9"></a>
### [OpenAI says it disrupted model distillation campaign tied to Moonshot-affiliated individuals](https://openai.com/index/disrupting-a-coordinated-model-distillation-campaign/) ⭐️ 7.0/10

OpenAI says it disrupted a coordinated model distillation campaign that used manipulated interactions to extract protected reasoning content, and it attributes the core activity to individuals associated with Moonshot AI, the developer of Kimi. According to the company&\#x27;s account, the activity first appeared in early July 2026, peaked on July 24-25 with roughly 16,000 requests from more than 4,000 users, and conduct involving over 15,000 users had been disrupted by July 28. OpenAI says it shared its findings with industry and government through Frontier Model Forum channels. The attribution rests on OpenAI&\#x27;s own claim: it competes directly with Moonshot, the figures do not reconcile as reported \(more than 4,000 users making 16,000 requests versus more than 15,000 users disrupted, with no explanation of the gap\), and no independent verification or technical detail has been published.

telegram · zaihuapd · Oct 1, 01:18

**「Background」** Distillation is the practice of training one AI model on another&\#x27;s outputs, and OpenAI uses the term &quot;adversarial distillation&quot; for the systematic, unauthorized use of a model&\#x27;s outputs or reasoning to train, reproduce, or improve another model. OpenAI&\#x27;s reasoning models keep their raw chain-of-thought hidden from users largely to prevent this kind of copying, and reporting on the incident describes a &quot;novel&quot; encryption bypass as the technique used to extract that protected reasoning. Moonshot AI is the Chinese developer of the Kimi model family, including the Kimi K3 model, and a direct rival of OpenAI, which frames how the company&\#x27;s attribution claim will be assessed.

**「Enforcement risk for extraction practices and sharper scrutiny of Chinese open-source models」** For developers and organizations, the immediate consequence is enforcement risk: OpenAI says it disrupted activity tied to more than 15,000 users before July 28, so anyone running bulk or automated collection of protected reasoning outputs through its API faces account termination, and indicators shared through Frontier Model Forum channels let other providers apply similar detection to their own platforms. The public attribution also raises the stakes in an ongoing dispute, since American AI companies and the US government have already accused Chinese firms such as Moonshot AI of &\#x27;systematic&\#x27; distillation attacks, and Kimi&\#x27;s free or low-cost open-source models sit at the center of that competitive tension — though the link to Moonshot-affiliated individuals remains OpenAI&\#x27;s own claim, not an independently verified finding.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/disrupting-a-coordinated-model-distillation-campaign/">Disrupting a coordinated model-distillation campaign | OpenAI</a></li>
<li><a href="https://cyberscoop.com/openai-moonshot-ai-model-distillation-attack/">OpenAI reveals ‘novel’ encryption bypass used in distillation ...</a></li>
<li><a href="https://wccftech.com/moonshot-ai-of-kimi-k3-fame-tried-to-crack-openais-encrypted-reasoning-through-16000-requests-bolstering-trump-administrations-distillation-claims/">Moonshot AI Of Kimi K3 Fame Tried To Crack OpenAI ... - Wccftech</a></li>
<li><a href="https://cryptobriefing.com/openai-disrupts-moonshot-ai-kimi-extraction/">OpenAI disrupts extraction attempts linked to Moonshot AI&#x27;s Kimi</a></li>
<li><a href="https://cyberscoop.com/openai-moonshot-ai-model-distillation-attack/">OpenAI reveals ‘novel’ encryption bypass used in distillation ...</a></li>
<li><a href="https://www.cnbc.com/2026/10/01/openai-chinas-moonshot-ai-kimi.html">OpenAI links China’s Moonshot AI to extraction attempt - CNBC</a></li>

</ul>
</details>

**Tags**: `#AI security`, `#model distillation`, `#OpenAI`, `#Moonshot AI \(Kimi\)`, `#industry competition`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Kalshi, Polymarket trading volumes on some products raise questions amid massive growth](https://www.cnbc.com/2026/09/30/kalshi-polymarket-trading-volume-scrutiny.html) ⭐️ 7.0/10

CNBC reports that unusual trading volume patterns on Kalshi and Polymarket are fueling concerns about potentially inflated or wash-traded volumes at a time when both platforms command multibillion-dollar valuations, face reported CFTC scrutiny, and are reportedly exploring public listings.

rss · CNBC Finance · Sep 30, 21:09

**Tags**: `#prediction-markets`, `#trading-volumes`, `#wash-trading-concerns`, `#CFTC-scrutiny`, `#IPO-valuations`

---

<a id="item-finance-news-2"></a>
### [China warns of &\#x27;firm response&\#x27; if EU restricts Chinese businesses](https://www.cnbc.com/2026/09/30/china-warns-europe-increases-trade-pressure.html) ⭐️ 7.0/10

China&\#x27;s commerce ministry warned it will &quot;respond firmly&quot; if the EU restricts Chinese businesses or products, saying such moves during ongoing trade talks would &quot;seriously undermine mutual trust&quot; ahead of high-level meetings in Beijing next week. The warning responds to proposals that are not yet policy: a Germany-France paper urging the European Commission to develop a US &\#x27;301&\#x27;-style tool that one official said could cut China off from the EU market within 24 hours, as Brussels presses to shrink the world&\#x27;s largest bilateral trade deficit by October; EU-China trade in goods and services totaled 880 billion euros \(nearly $1 trillion\) last year.

rss · CNBC Finance · Sep 30, 03:39

**「Background」** A &\#x27;301-style&\#x27; tool would let Brussels unilaterally and quickly restrict Chinese goods or market access, mirroring a U.S. trade-law mechanism, whereas the EU currently relies on slower remedies such as anti-dumping cases. The warning lands mid-negotiation: the EU has given Beijing until October to deliver &\#x27;concrete results&\#x27; toward shrinking the world&\#x27;s largest bilateral trade deficit or face &\#x27;harsher measures,&\#x27; per EU Trade Commissioner Maroš Šefčovič.

**「Who could be affected」** European businesses that import or make electrical equipment and machinery—the top two product groups in EU-China trade, which ran a €103 billion deficit in Q2 2026—face higher costs and market-access risk if Brussels restricts Chinese goods and Beijing carries out its retaliation threat.

<details><summary>References</summary>
<ul>
<li><a href="https://www.firstpost.com/business/china-eu-trade-tensions-section-301-trade-tool-beijing-eu-trade-policy-14049259.html">China warns of ‘resolute response’ as EU weighs US-style ...</a></li>
<li><a href="https://vanovertveldt.com/wp-content/uploads/2026/06/study-eu_china_parliament_report.pdf">The impact of EU-China tariff escalation and retaliation</a></li>
<li><a href="https://ec.europa.eu/eurostat/statistics-explained/SEPDF/cache/55157.pdf">EU trade with China - latest developments Statistics Explained</a></li>

</ul>
</details>

**Tags**: `#China-EU trade`, `#trade tensions`, `#retaliation threat`, `#trade policy`, `#tariffs`

---

<a id="item-finance-news-3"></a>
### [China reportedly tightens IPO criteria for humanoid robot startups](https://www.cnbc.com/2026/09/29/china-criteria-humanoid-robot-ipos.html) ⭐️ 7.0/10

China&\#x27;s securities regulator has reportedly set three new criteria for humanoid robot IPOs — sustainable revenue with commercial orders, narrowing losses backed by a three-year forecast, and core technology such as a robotic brain or hands — and sources familiar with the matter say few or none of the sector&\#x27;s applicants may qualify.

rss · CNBC Finance · Sep 30, 02:50

**「Background」** The regulator has not confirmed the unpublished &quot;window guidance,&quot; which comes as China&\#x27;s 100-plus humanoid startups drew 47.09 billion yuan \($6.95 billion\) in investment in the second quarter, more than double the first quarter. Unitree, the sector&\#x27;s flagship, raised about 6.1 billion yuan in its August Shanghai IPO, but its shares have since nearly halved.

**「Impact」** Humanoid startups pursuing Hong Kong listings and their early-stage investors could be shut out of public markets, since mainland companies need the CSRC&\#x27;s approval to list there.

**Tags**: `#China regulation`, `#humanoid robots`, `#IPO`, `#CSRC`, `#AI sector`

---