---
layout: default
title: "Horizon Summary: 2026-09-30 (EN)"
date: 2026-09-30
lang: en
---

> From 45 items, 11 important content pieces were selected

---

**Technology News**
1. [OpenAI announces GPT 6.1 Sol: near-Astra intelligence claim at one-fifth the price](#item-tech-news-1) ⭐️ 8.0/10
2. [Community Releases &\#x27;Relapse&\#x27; PS5 Exploit Reportedly Targeting WebKit JavaScriptCore](#item-tech-news-2) ⭐️ 7.0/10
3. [Privacy Paper Finds Tracking and Data Exposure in Conversational AI Agents](#item-tech-news-3) ⭐️ 7.0/10
4. [OpenAI announces Dots, an always-on agent offering](#item-tech-news-4) ⭐️ 7.0/10
5. [Anthropic: GLM-5.3 and Claude Mythos Preview Now Achieve Full Control Flow Hijacks](#item-tech-news-5) ⭐️ 7.0/10
6. [Free Open-Source Book Teaches ML Performance Engineering from Silicon to Agents](#item-tech-news-6) ⭐️ 7.0/10
7. [Oracle Issues Force Majeure Notice Over Stargate Data Center Power Delays](#item-tech-news-7) ⭐️ 7.0/10

**Financial News**
1. [China to Subsidize First-Home Commercial Mortgage Interest by 1 Point a Year From October 1](#item-finance-news-1) ⭐️ 8.0/10
2. [Fair Isaac sinks 18% premarket on mortgage pricing overhaul; AMD, CarMax also move](#item-finance-news-2) ⭐️ 7.0/10
3. [Trump&\#x27;s municipal bond portfolio grows to between $300 million and $1 billion](#item-finance-news-3) ⭐️ 7.0/10
4. [China reportedly sets three tough criteria for humanoid robot IPOs that few startups can meet](#item-finance-news-4) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [OpenAI announces GPT 6.1 Sol: near-Astra intelligence claim at one-fifth the price](https://openai.com/index/introducing-gpt-6-1-sol/) ⭐️ 8.0/10

OpenAI announced GPT 6.1 Sol, pitched as near-Astra intelligence for roughly a fifth of the price, with cached input priced at $0.10 per million tokens—95% below standard input pricing and 50% below the previous GPT-6 Sol&\#x27;s cached-input rate. These are OpenAI&\#x27;s own announcement claims; no independent benchmarks, pricing verification, or availability details appear in the available material. The release follows GPT-6 Sol, which many Hacker News commenters describe as a quality regression, leading them to read 6.1 as a corrective follow-up rather than a new frontier.

hackernews · crorella · Sep 29, 17:06 · [Discussion](https://news.ycombinator.com/item?id=49896586)

**「Context」** GPT 6.1 Sol follows OpenAI&\#x27;s GPT-6 Sol release by only a matter of days, and commenters describe that predecessor as a notable regression from Sol 5.6 that pushed some developers toward Anthropic&\#x27;s Opus 5.5 instead. The update also undercuts its predecessor on cost, with the announcement quoting cached input at $0.10 per million tokens—95% below standard input pricing and half of GPT-6 Sol&\#x27;s cached rate. The headline&\#x27;s &\#x27;near-Astra&\#x27; framing references the higher-priced Astra tier, which commenters characterize as capable in areas like vision but unreliable for coding.

**「Cached input pricing is the concrete saving for agent workloads」** Developers running context-heavy coding agents get the most direct benefit from the cached input rate of $0.10 per million tokens—95% below standard input pricing and 50% below GPT-6 Sol&\#x27;s cached rate—so Codex-style sessions that repeatedly re-read long context can roughly halve that cost component. With standard API prices at $2 per million input and $10 per million output tokens \(a fifth of GPT-6 Astra&\#x27;s rates\), teams can re-baseline their model budgets at DevDay adoption, but given community reports of quality regressions in GPT-6 Sol, benchmarking 6.1 on your own coding tasks before migrating from alternatives like Opus 5.5 is the prudent action.

**「Community reaction」** Skeptics dominated the thread: the\_duke reported switching to Opus 5.5 after Sol 6 regressed badly on coding compared with Sol 5.6, and revolvingthrow speculated that 6.1 is a hurried rename of the recently spotted &\#x27;Astra-Minor&\#x27; to compensate for an underwhelming Sol 6. On economics, minimaxir called the 50% cached-input cut the real headline for Codex users, proxysna argued DeepSeek&\#x27;s speed and what he considers a negligible intelligence gap already make $200/month frontier plans hard to justify, and gradus\_ad saw token price becoming the industry&\#x27;s main battleground—a trend he called ominous for investors.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/introducing-gpt-6-1-sol/">Introducing GPT-6.1 Sol | OpenAI</a></li>
<li><a href="https://fourweekmba.com/ai-gpt-61-sol-cached-read-price-change/">GPT-6.1 Sol&#x27;s One Real Price Change Is the Cached Read - FourWeekMBA</a></li>
<li><a href="https://thenextweb.com/news/openai-gpt-6-1-sol-price-astra-devday">OpenAI releases GPT-6.1 Sol at a fifth of GPT-6 Astra’s token prices</a></li>

</ul>
</details>

**Tags**: `#openai`, `#large-language-models`, `#model-releases`, `#ai-pricing`, `#developer-tools`

---

<a id="item-tech-news-2"></a>
### [Community Releases &\#x27;Relapse&\#x27; PS5 Exploit Reportedly Targeting WebKit JavaScriptCore](https://github.com/ntfargo/Relapse-Exploit) ⭐️ 7.0/10

A community-published PlayStation 5 exploit named Relapse has been released on GitHub \(ntfargo/Relapse-Exploit\), and the accompanying discussion indicates it reportedly leverages a bug in WebKit&\#x27;s JavaScriptCore JavaScript engine. The release drew 223 points and 122 comments on Hacker News, where conversation quickly turned to the console&\#x27;s browser attack surface and Sony&\#x27;s likely response. The item itself provides limited technical detail, so which firmware versions are affected, the reliability of the exploit, and whether Sony will patch or mitigate it remain unclear.

hackernews · therepanic · Sep 29, 15:44 · [Discussion](https://news.ycombinator.com/item?id=49895304)

**「Background」** PlayStation console jailbreaks typically start in the system&\#x27;s WebKit browser engine, where a memory-safety flaw in JavaScriptCore yields userland code execution that must then be paired with a kernel bug for full control of the machine. Reports on Relapse describe exactly that structure: WebKit JavaScriptCore info leaks chained to a use-after-free in the kernel&\#x27;s aio\_multi\_wait interface to gain kernel read/write, with claimed coverage of firmware 7.00 through 13.60 — every shipping version except the less-than-two-week-old 14.00.00.

**「Firmware window defines who benefits」** PS5 owners on firmware 7.00 through 13.60 can now run the Relapse chain from the console&\#x27;s browser to jailbreak their systems, but the exploit is non-persistent — it must be re-executed after every reboot, and the kernel stage can hang or panic the console, requiring a reboot before retrying. The compatibility window is already closing: Sony&\#x27;s firmware 14.00.00, released September 16, 2026, is reported to be immune, so users who want jailbreak access should stay on 13.60 or earlier and skip the update.

**「Community reaction」** Commenter MaxBarraclough questioned whether the PS5&\#x27;s WebKit runs JavaScriptCore with the JIT compiler enabled and speculated Sony could respond by disabling the JIT to narrow the attack surface, while Muromec argued that console-hacking communities typically hold back stashes of undisclosed zero-days rather than publishing everything. Other commenters framed the appeal of a jailbreak around running Steam PC games on the console, and aussieguy1234 criticized that owners must hack hardware they legally own to gain full control over it.

<details><summary>References</summary>
<ul>
<li><a href="https://elsolitario.org/en/2026/09/29/relapse-repo-claims-ps5-exploit-firmware-7-00-to-13-60/">PS5 Jailbreak: What Is Relapse Exploit and Its Scope</a></li>
<li><a href="https://kotaku.com/new-ps5-jailbreak-exploit-works-on-systems-running-july-2026-firmware-2000738283">PS5 Jailbreak Exploit For Systems Running July 2026 Firmware</a></li>
<li><a href="https://sploitus.com/exploit?id=64E42AF3-CF08-5BE3-8BA8-BBD8F517B53C">Relapse-Exploit — PoC exploit | Sploitus</a></li>
<li><a href="https://github.com/ntfargo/Relapse-Exploit">GitHub - ntfargo/Relapse-Exploit: Exploit chain for PS5 7.00 ...</a></li>
<li><a href="https://soplayit.com/en/news/new-ps5-jailbreak-relapse-targets-older-firmware">New PS5 Jailbreak &#x27;Relapse&#x27; Targets Older Firmware - Soplayit</a></li>
<li><a href="https://tbreak.com/ps5-jailbreak-relapse-firmware-13-60/">PS5 jailbreak reaches firmware 13.60 with Relapse</a></li>

</ul>
</details>

**Tags**: `#security`, `#exploitation`, `#playstation`, `#webkit`, `#console-hacking`

---

<a id="item-tech-news-3"></a>
### [Privacy Paper Finds Tracking and Data Exposure in Conversational AI Agents](https://jorgegarciaherrero.com/wp-content/interactivos/20260916-Prompt-like-a-butterfly-sting-like-a-tracker-%28clean%29.pdf) ⭐️ 7.0/10

A research paper analyzing privacy and tracking risks in widely used web and mobile conversational AI agents became one of Hacker News&\#x27;s more discussed items on September 29, 2026, drawing 407 points and 128 comments. Hosted under the title &quot;Prompt Like a Butterfly, Sting Like a Tracker&quot;, the paper examines how chatbot clients can expose user data, with the surrounding discussion centering on third-party ad trackers, telemetry that transmits prompt content, full conversations being reachable through their URLs, and leakage of conversation data into model training. It is an independent analysis of shipped apps rather than a vendor announcement, assessing tools that users routinely treat as private conversation partners.

hackernews · damaru2 · Sep 29, 09:03 · [Discussion](https://news.ycombinator.com/item?id=49890226)

**「Background」** Privacy research on conversational AI has so far centered on the prompt itself: multiple earlier studies examined how prompting and in-context learning can expose sensitive data and devised mitigation techniques against those risks. These assistants, however, are delivered through ordinary web and mobile apps, placing them inside the same ecosystem of third-party advertising and tracking services \(ATSes\) as any other consumer software — the exposure surface this analysis set out to measure.

**「Practical takeaway」** For users of web chat clients, the practical consequence is that neither the URL nor the send button guarantees privacy: commenters reported that a past Perplexity conversation URL exposes the full transcript to whoever holds it, and that ChatGPT&\#x27;s browser client transmits prompt text before submission. Readers who share conversation links or type drafts without sending them should treat both actions as potential disclosure of the full content.

**「Community discussion」** The most substantive reports came from pbasista, who observed ChatGPT&\#x27;s web client periodically sending unfinished prompts to a conversation/prepare endpoint — possibly for cache pre-warming, but also usable to profile writing cadence and evolving drafts — and postalcoder, who criticized services equating a UUID in the URL with privacy. kdaniel\_03 framed the problem through his account of a recent incident in which OpenAI said no one viewed private Codex sessions containing unpublished math drafts while acknowledging de-identified product data may have improved its models, concluding that open models &quot;have to win&quot;, and j4k0bfr speculated that trackers tied to direct competitors suggest rushed ad integrations driven by investor profitability pressure.

<details><summary>References</summary>
<ul>
<li><a href="https://jorgegarciaherrero.com/wp-content/interactivos/20260916-Prompt-like-a-butterfly-sting-like-a-tracker-%28clean%29.pdf">Prompt like a Butterfly, Sting like a Tracker: A Privacy ...</a></li>
<li><a href="https://arxiv.org/html/2404.06001v1">Privacy Preserving Prompt Engineering: A Survey - arXiv.org</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#conversational-ai`, `#tracking`, `#llm`, `#security`

---

<a id="item-tech-news-4"></a>
### [OpenAI announces Dots, an always-on agent offering](https://openai.com/index/introducing-dots/) ⭐️ 7.0/10

OpenAI has announced Dots, a product its announcement page describes as always-on agents, though the item supplied here contains no technical details about capabilities, pricing, or availability, so it remains an announced offering rather than an independently verified one. The launch drew substantial attention on Hacker News, where the discussion reached 451 points and 341 comments. Commenters focused less on demonstrated features and more on strategy questions, including platform lock-in, the future of Codex subscription limits, and how Dots overlaps with OpenAI&\#x27;s existing Codex and ChatGPT Work products.

hackernews · alvis · Sep 29, 17:07 · [Discussion](https://news.ycombinator.com/item?id=49896604)

**「From chatbots to always-on agents」** Always-on agents represent a shift from today&\#x27;s request-and-response chatbots: per OpenAI&\#x27;s launch page, Dots is built to learn what matters to a user and keep working on their behalf rather than answering one prompt at a time. The product was announced at OpenAI&\#x27;s DevDay 2026 conference in San Francisco as part of more than 20 announcements, and Wired&\#x27;s coverage positioned Dots as OpenAI&\#x27;s answer to Meta in the emerging always-on agent category—a rivalry commenters associate with Meta&\#x27;s Muse. Dots also enters an OpenAI lineup that commenters say already includes the Codex coding agent and ChatGPT Work, which is fueling debate over where one agent product ends and the next begins.

**「Lock-in trade-offs and a head-to-head with Muse」** Adopting Dots carries a portability cost for users: the agent works by connecting to a person&\#x27;s apps and handling multistep tasks, so integrations and work history accumulate on OpenAI&\#x27;s platform, and commenters argue this makes switching providers harder than swapping between interchangeable models — before granting access, users should weigh which apps and data they want tied to OpenAI. Dots is positioned as a direct answer to Meta&\#x27;s Muse, so early adopters must choose between two competing always-on agent ecosystems rather than converging on a single standard.

**「Hacker News reaction」** Commenter aditya\_rs argued that always-on agents create deeper lock-in than swappable models because accumulated integrations and work history make the service effectively &quot;your computer on the cloud,&quot; while johnfahey speculated OpenAI could tighten the generous Codex limits that drew users over from Claude, a pattern he attributed to Anthropic earlier. Others questioned the product&\#x27;s positioning: wxw found the boundaries between Codex, ChatGPT Work, and Dots increasingly blurry, and jameslk suggested that cloud-VM agents like Dots and Meta&\#x27;s Muse could hasten a shift away from the PC era — opinions that reflect skepticism rather than established facts about the product.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/introducing-dots/">Introducing dots - OpenAI</a></li>
<li><a href="https://mashable.com/tech/openai-dev-day-dots-ai-agents">OpenAI introduces Dots, a new always-on AI agent, at Dev Day</a></li>
<li><a href="https://www.wired.com/story/openai-dots-always-on-ai-agents-that-proactively-help/">OpenAI’s Dots Are Always-On AI Agents—and Its Answer to Meta ...</a></li>
<li><a href="https://www.adweek.com/media/openai-takes-on-metas-muse-with-dots-an-always-on-ai-agent/">OpenAI Takes On Meta&#x27;s Muse With Dots, an Always-On AI Agent</a></li>
<li><a href="https://www.wired.com/story/openai-dots-always-on-ai-agents-that-proactively-help/">OpenAI’s Dots Are Always-On AI Agents—and Its Answer to Meta ...</a></li>
<li><a href="https://ai.meta.com/muse/">Muse: Meta&#x27;s personal AI agent, features &amp; capabilities</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#OpenAI`, `#platform lock-in`, `#product strategy`, `#developer tools`

---

<a id="item-tech-news-5"></a>
### [Anthropic: GLM-5.3 and Claude Mythos Preview Now Achieve Full Control Flow Hijacks](https://simonwillison.net/2026/Sep/29/anthropic-frontier-red-team/) ⭐️ 7.0/10

Anthropic&\#x27;s Frontier Red Team reports that GLM-5.3 and Claude Mythos Preview can execute full control flow hijacks — redirecting a running program&\#x27;s execution, a core primitive of memory-corruption exploitation — on 100 randomly selected tasks from the lab&\#x27;s internal Binary Exploitation benchmark, with GLM-5.3 succeeding in 4% of trials and Claude Mythos Preview in 6%. According to the report, earlier models including Claude Opus 4.6 and GLM-5.2 did not succeed on any of the tasks, which the red team describes as a meaningful threshold having clearly been crossed. Simon Willison quote-posted the excerpt on his blog without adding analysis of his own, and the figures are Anthropic&\#x27;s own reported benchmark results rather than an independently measured capability.

rss · Simon Willison · Sep 29, 22:20

**「Background」** A control-flow hijack means forcing a running program down an attacker-chosen execution path, and the test behind the quoted figures is Anthropic&\#x27;s internal Binary Exploitation benchmark, which checks whether models can find and exploit vulnerabilities in popular open-source projects participating in Google&\#x27;s OSS-Fuzz program, awarding full credit only for a complete hijack. GLM-5.3 belongs to GLM, a fifth-generation frontier large-language-model family described as open-source, built on a Mixture-of-Experts architecture with 745B total parameters, 44B activated per inference, and a 200K-token context window.

**「Unguarded open weights make autonomous exploit development widely accessible」** Anthropic&\#x27;s report emphasizes that GLM-5.3 differs from other frontier models because it has been released as an open-weight model without meaningful safeguards against misuse, meaning the control flow hijack capability demonstrated in the benchmark is downloadable and locally runnable rather than gated behind a guarded API. In simulated tests, simple tricks bypassed GLM-5.3&\#x27;s safeguards 64% to 100% of the time, so organizations cannot count on vendor-side guardrails as a mitigating layer for this model. Security teams — particularly those maintaining open-source codebases, which Z.ai says GLM-5.3 already surfaced 1,097 critical vulnerabilities in during testing — should treat autonomous end-to-end exploit development as a readily available capability when updating threat models.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/research/glm-5-3-and-the-spread-of-advanced-cyber-capabilities">GLM - 5 . 3 and the spread of advanced cyber capabilities \ Anthropic</a></li>
<li><a href="https://glm5.app/">GLM 5 — Next-Gen Frontier Model</a></li>
<li><a href="https://www.anthropic.com/research/glm-5-3-and-the-spread-of-advanced-cyber-capabilities">GLM-5.3 and the spread of advanced cyber capabilities \ Anthropic</a></li>
<li><a href="https://www.technology.org/2026/08/17/zai-glm-5-3-cybergym-mythos-5-benchmarks/">Z.ai GLM-5.3 Nears Mythos 5 on Bug Hunting - Technology Org</a></li>
<li><a href="https://ai-tldr.dev/releases/anthropic-glm-5-3-cyber-report/">Anthropic tests GLM-5.3 — its safeguards fall to… | AI/TLDR</a></li>

</ul>
</details>

**Tags**: `#ai-security`, `#llm-research`, `#cybersecurity`, `#anthropic`, `#ai-safety`

---

<a id="item-tech-news-6"></a>
### [Free Open-Source Book Teaches ML Performance Engineering from Silicon to Agents](https://www.reddit.com/r/MachineLearning/comments/1wt6ns4/i_wrote_a_free_opensource_book_on_making_ml/) ⭐️ 7.0/10

A machine learning practitioner has released a free, open-source book, &quot;How to Make Your Model Fast: A Systems View of Efficient Machine Learning, from Silicon to Agents,&quot; hosted on GitHub. The book teaches performance engineering starting with roofline analysis and hardware, then progressing through kernels, compilers, quantization, pruning, vision, on-device LLMs, robotics, profiling, serving, and agent systems. Its central premise is that reducing FLOPs does not necessarily make a model faster; readers first learn to determine whether a workload is compute-, bandwidth-, memory-, or system-bound and which optimization will actually raise that limit. As a self-published work announced via Reddit, its completeness and accuracy have not been independently reviewed, and the author is actively soliciting feedback and contributions.

reddit · r/MachineLearning · /u/SoloTiger\_ · Sep 29, 10:35

**「Background」** ML performance engineering is the practice of diagnosing whether a model is compute-, bandwidth-, memory-, or system-bound before choosing optimizations such as quantization, pruning, or custom kernels, since cutting FLOPs alone does not guarantee faster execution. Until now, learning this material has meant piecing together scattered resources: course repositories such as the Efficient Deep Learning Systems course taught at HSE University and the Yandex School of Data Analysis, curated lists like the awesome-production-machine-learning repository that tracks new production ML libraries, and broader curricula such as Made-With-ML, whose lessons emphasize end-to-end MLOps practices like tracking, testing, serving, and orchestration rather than hardware-level bottleneck analysis.

**「Impact」** Engineers and researchers working on inference, ML systems, compilers, or edge AI can access the book at no cost on GitHub and use its bottleneck-analysis framing to decide whether quantization, pruning, or kernel optimization is worth pursuing for a given model and hardware combination. Because the project is open source, readers can also file issues, contribute content, or give the author feedback directly.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/EthicalML/awesome-production-machine-learning">GitHub - EthicalML/awesome-production-machine-learning: A ...</a></li>
<li><a href="https://github.com/GokuMohandas/Made-With-ML">GitHub - GokuMohandas/Made-With-ML: Learn how to develop ... GitHub - mryab/efficient-dl-systems: Efficient Deep Learning ... zero-to-mastery-ml/section-1-getting-ready-for-machine ... GitHub - apple-aiml-research/ml-fastvit: This repository ... How to Develop an AI Model Faster and More Efficiently</a></li>

</ul>
</details>

**Tags**: `#machine-learning`, `#performance-engineering`, `#inference-optimization`, `#systems`, `#open-source`

---

<a id="item-tech-news-7"></a>
### [Oracle Issues Force Majeure Notice Over Stargate Data Center Power Delays](https://www.bloomberg.com/news/articles/2026-09-24/oracle-cites-force-majeure-to-shield-itself-on-controversial-data-center) ⭐️ 7.0/10

Oracle has issued a force majeure notice to the developer of Project Jupiter, a Stargate data center in New Mexico, after environmental and power-supply approvals for the site&\#x27;s 2.45GW supporting microgrid stalled, putting its planned 2028 launch at risk; the notice is meant to let Oracle defer some payments if externally caused delays materialize. Per Bloomberg reporting relayed via the source, the project&\#x27;s $18 billion syndicated loan is now trading at a discount, reflecting market concern about hyperscale AI data center timelines and financing risk. Most Stargate sites remain in civil construction, permitting, and energy-infrastructure stages, with only a few facilities—such as the Abilene, Texas campus—operational. Texas has also suspended approvals for new data center projects.

telegram · zaihuapd · Sep 29, 05:46

**「Background」** A force majeure clause excuses a party from its contractual obligations when events outside its control prevent performance, and the reports of 24 September 2026 described Oracle&\#x27;s notice as invoking exactly that mechanism toward the Project Jupiter developer over the stalled approvals. The notice has teeth because Oracle is the paying customer for the New Mexico campus, committed to funding the developer, which is why an approval-driven delay gives it grounds to defer payments rather than keep paying for capacity that cannot start up on schedule.

**「Financing fallout hits lenders」** The force majeure notice has already produced a measurable financial consequence: the roughly $18 billion syndicated construction loan for Project Jupiter has stalled in distribution, with banks quoting the debt at 89–91 cents on the dollar, shrinking its market value to roughly $16–16.4 billion. Arranging banks including Santander and Jefferies are struggling to pass the exposure to other investors, giving lenders and AI data center developers a concrete signal that power and environmental approval timelines now need to be priced into financing terms.

<details><summary>References</summary>
<ul>
<li><a href="https://app.dealroom.co/news/note/oracle-files-force-majeure-on-2-45gw-new-mexico-stargate-data-center">Oracle files force majeure on 2.45GW New Mexico Stargate data center | Dealroom.co</a></li>
<li><a href="https://techcrunch.com/2026/09/24/oracle-sends-force-majeure-notice-on-its-new-mexico-stargate-data-center/">Oracle sends force majeure notice on its New Mexico Stargate data center | TechCrunch</a></li>
<li><a href="https://finance.biggo.com/news/aa2b00f9-d885-40e0-92db-6fd9f55ffe63">Oracle&#x27;s $18 Billion AI Loan Sells at a Discount, Banks Forced to Swallow a Hot Potato — BigGo Finance</a></li>
<li><a href="https://www.roic.ai/news/oracle-invokes-force-majeure-on-project-jupiter-as-ai-data-center-financing-stumbles-09-24-2026">Oracle Invokes Force Majeure on Project Jupiter as AI Data Center Financing Stumbles | Roic News</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#data centers`, `#Oracle`, `#Stargate`, `#energy policy`

---

## Financial News

<a id="item-finance-news-1"></a>
### [China to Subsidize First-Home Commercial Mortgage Interest by 1 Point a Year From October 1](https://jrs.mof.gov.cn/zhengcefabu/phjr/202609/t20260929_3998312.htm) ⭐️ 8.0/10

China&\#x27;s finance ministry, central bank, and banking regulator jointly announced on September 29 that, from October 1, 2026, families buying a first home with a new commercial mortgage will receive a central government subsidy covering 1 percentage point of the loan&\#x27;s annual interest for up to 5 years. Eligible homes must be 120 square meters or smaller and cost no more than 1.5 million yuan, the subsidized loan is capped at 1 million yuan per household—roughly 10,000 yuan in maximum yearly benefit—and the program is tentatively set to run for one year.

telegram · zaihuapd · Sep 29, 10:18

**「Background」** The housing measure follows the same three agencies&\#x27; personal consumption loan interest subsidy—where the government pays part of a borrower&\#x27;s loan interest directly—which was introduced in September 2025 and extended through the end of 2026.

**「Who benefits」** First-time buyers of homes no larger than 120 square meters and priced at 1.5 million yuan or less will effectively pay about one third less in commercial mortgage interest at current rate levels, capped at roughly 10,000 yuan per household per year for up to five years.

<details><summary>References</summary>
<ul>
<li><a href="https://www.dzwww.com/xinwen/guoneixinwen/202601/t20260120_17326136.htm">三 部 门：将个 人 消费 贷 款 财 政 贴 息 政 策 实施期限延长至 2026 ...</a></li>
<li><a href="https://news.china.com/socialgd/10000169/20260111/49152594.html">news.china.com/socialgd/10000169/20260111/49152594.html</a></li>
<li><a href="https://news.ifeng.com/c/8wotukhlA7p">居民房贷贴息政策10月1日起实施，力度多大？哪些购房者受益？_凤凰网</a></li>

</ul>
</details>

**Tags**: `#housing policy`, `#mortgage subsidy`, `#China real estate`, `#fiscal policy`, `#financial regulation`

---

<a id="item-finance-news-2"></a>
### [Fair Isaac sinks 18% premarket on mortgage pricing overhaul; AMD, CarMax also move](https://www.cnbc.com/2026/09/29/stocks-making-the-biggest-moves-premarket-fair-isaac-spacex-amd-more.html) ⭐️ 7.0/10

Fair Isaac shares plunged 18% in premarket trading after Federal Housing Finance Agency director Bill Pulte said Fannie Mae and Freddie Mac will replace their two mortgage pricing grids with one that adds VantageScore alongside the existing FICO Classic grid. Also before the open, AMD rose more than 1% on its $8.2 billion acquisition of AI firm World Labs, Summit Therapeutics surged 18% after a $2 billion AstraZeneca investment, and CarMax gained more than 6% after second-quarter earnings of $1.16 per share on $7.88 billion in revenue beat the 73 cents and $7.09 billion analysts expected.

rss · CNBC Finance · Sep 29, 12:03

**「Background」** Fannie Mae and Freddie Mac, the government-backed companies at the heart of U.S. mortgage finance, charge lenders fees through &\#x27;pricing grids&\#x27; — fee schedules tied to borrowers&\#x27; credit scores — and that role had belonged to FICO&\#x27;s Classic score alone. The FHFA&\#x27;s change puts the competing VantageScore on the same single grid, ending FICO&\#x27;s exclusive position in mortgage pricing.

**「Impact」** The FHFA&\#x27;s move to a single mortgage pricing grid that admits VantageScore puts direct competitive pressure on Fair Isaac&\#x27;s mortgage credit-scoring franchise — a segment where FICO has recently booked strong pricing-driven revenue growth and described as its most visible profit engine — hitting the company&\#x27;s investors and reshaping how lenders using Fannie Mae and Freddie Mac price home loans.

<details><summary>References</summary>
<ul>
<li><a href="https://wrenews.com/fannie-freddie-single-pricing-grid-vantagescore-fico-2026/">Fannie, Freddie Move to One Pricing Grid With VantageScore</a></li>
<li><a href="https://www.housingwire.com/articles/fhfa-gses-one-grid/">FHFA says GSEs will use one LLPA grid for FICO, VantageScore</a></li>
<li><a href="https://wrenews.com/fico-shares-plunge-mortgage-vantagescore-competition-2026/">FICO Shares Plunge More Than 20% as VantageScore Threat Grows</a></li>
<li><a href="https://finance.yahoo.com/markets/stocks/articles/fair-isaac-fico-down-19-041752218.html">Fair Isaac (FICO) Is Down 19.2% After FHFA Opens Mortgage Scoring To VantageScore Competition - Has The Bull Case Changed?</a></li>

</ul>
</details>

**Tags**: `#premarket-movers`, `#earnings`, `#mergers-and-acquisitions`, `#mortgage-policy`, `#credit-scores`

---

<a id="item-finance-news-3"></a>
### [Trump&\#x27;s municipal bond portfolio grows to between $300 million and $1 billion](https://www.cnbc.com/2026/09/29/trump-municipal-bond-portfolio.html) ⭐️ 7.0/10

A CNBC analysis of President Trump&\#x27;s financial disclosures found his portfolio of municipal bonds — debt issued by cities, hospitals, schools, and utilities — has grown to more than 1,000 positions worth between $300 million and $1 billion, a scale a University of Chicago municipal finance expert called unprecedented for an individual investor. Many of these borrowers are affected by his own administration&\#x27;s regulatory and funding decisions, though CNBC found no evidence he traded on advance knowledge of policy.

rss · CNBC Finance · Sep 29, 14:37

**「Context」** Presidents are exempt from the conflict-of-interest laws that bar other executive branch officials from holding such bonds, and the White House and Trump Organization say the accounts are run by outside managers with no input from Trump.

**「Who is affected」** Coal plants granted a two-year exemption from stricter pollution rules and hospitals facing Medicaid cuts projected by the nonpartisan group KFF at about $900 billion over a decade are among borrowers whose finances federal policy can move while Trump holds their debt.

**Tags**: `#municipal bonds`, `#Trump finances`, `#conflict of interest`, `#financial disclosures`, `#presidential ethics`

---

<a id="item-finance-news-4"></a>
### [China reportedly sets three tough criteria for humanoid robot IPOs that few startups can meet](https://www.cnbc.com/2026/09/29/china-criteria-humanoid-robot-ipos.html) ⭐️ 7.0/10

According to three anonymous sources, China&\#x27;s securities regulator has issued &quot;window guidance&quot; requiring humanoid robot IPO applicants to show sustainable revenue and commercial orders, narrowing losses \(with a three-year forecast\), and core technology such as robotic &quot;brains&quot; or hands — criteria that few, if any, of China&\#x27;s 100-plus startups can meet, and which the regulator has not publicly confirmed. The reported tightening follows Unitree&\#x27;s Aug. 19 Shanghai IPO, which raised about 6.1 billion yuan \($905 million\) and jumped more than 460% on debut before nearly halving to 459.65 yuan a share as of Monday.

rss · CNBC Finance · Sep 29, 07:19

**「Context」** Chinese regulators often steer companies through informal, non-public &quot;window guidance&quot; rather than published rules, and Beijing has backed &quot;embodied AI&quot; — artificial intelligence placed in physical robots — as a national priority while warning of a sector bubble. The tightened scrutiny follows Unitree&\#x27;s Shanghai IPO on Aug. 19, whose shares surged more than 460% before nearly halving, and Hong Kong&\#x27;s May 2025 decision to let tech companies file confidentially for IPOs, with mainland firms also needing CSRC approval to list there.

**「Impact」** The reported criteria directly threaten the IPO plans of China&\#x27;s 100-plus humanoid robot startups — at least two dozen of which have filed in Hong Kong — and narrow the public-listing exit route for the government and private funds backing them, since mainland companies need CSRC approval to list there.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/09/29/china-criteria-humanoid-robot-ipos.html">China &#x27;s criteria for humanoid robot IPOs may be hard to meet</a></li>

</ul>
</details>

**Tags**: `#China`, `#humanoid robots`, `#IPO regulation`, `#Unitree`, `#AI bubble`

---