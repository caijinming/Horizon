---
layout: default
title: "Horizon Summary: 2026-10-10 (EN)"
date: 2026-10-10
lang: en
---

> From 43 items, 5 important content pieces were selected

---

**Technology News**
1. [Cloudflare acquires Deno, will end runtime development after one year of maintenance](#item-tech-news-1) ⭐️ 9.0/10
2. [Oxide Computer Announces $445M Series D Funding Round](#item-tech-news-2) ⭐️ 7.0/10
3. [JetBrains Releases Open-Source Coding Model Mellum 2.1](#item-tech-news-3) ⭐️ 7.0/10
4. [Telegram Desktop one-click flaw could silently steal files; fixed in 7.2.9](#item-tech-news-4) ⭐️ 7.0/10

**Technology Blog**
1. [Software&\#x27;s centaur age may last decades](#item-tech-blog-1) ⭐️ 5.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Cloudflare acquires Deno, will end runtime development after one year of maintenance](https://deno.com/blog/cloudflare) ⭐️ 9.0/10

Cloudflare announced it has acquired Deno, and per the announcement the Deno runtime will receive only one more year of support: monthly releases containing bug fixes and security updates, after which Cloudflare will end its development of the runtime. Deno will remain open source, and the company says it welcomes others who want to continue developing the project. This is an announced plan rather than a settled outcome — unless another party picks up development, the runtime will no longer be supported once that year ends. Developers and teams that built on Deno now have a defined maintenance window but an uncertain long-term future for the platform.

hackernews · ilreb · Oct 9, 13:03 · [Discussion](https://news.ycombinator.com/item?id=50019911)

**「Background」** Deno is a JavaScript runtime created by Ryan Dahl, the original creator of Node.js, and the company behind it also operated Deno Deploy, a hosting service that will shut down after six months, with migration support for paying customers moving to Cloudflare Workers. Cloudflare, the acquiring company, is an infrastructure provider whose core services include content delivery, cybersecurity, and DDoS mitigation. The JSR package registry tied to the Deno ecosystem will continue operating under Cloudflare, making it one piece of Deno infrastructure that outlasts the runtime&\#x27;s remaining year of maintenance.

**「Impact」** Developers running production workloads on Deno face a fixed timeline: Deno Deploy shuts down in six months and the runtime gets only one more year of monthly bug fix and security releases before active development ends, so teams should begin evaluating migration paths now. Cloudflare is offering migration support for paying customers moving to Cloudflare Workers, JSR will continue operating with its infrastructure moved to Cloudflare, and work continues on rusty\_v8 with the goal of integrating it into workerd — while the runtime&\#x27;s open-source status leaves any longer-term continuation to the community.

**「Community discussion」** In the Hacker News thread, developers who had invested in the Deno ecosystem described disappointment and migration concerns; one commenter who said he stopped building on Deno after npm compatibility became a priority argued the runtime had drifted from its original minimal vision, while another suggested a more accurate headline would be that &quot;Deno development effectively shut down via a Cloudflare acquihire.&quot; Others framed the deal as part of a broader wave of developer-tools acquisitions and expressed hope that Cloudflare&\#x27;s workerd would adopt Deno&\#x27;s security sandboxing mechanisms — hopes, not confirmed plans.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cloudflare">Cloudflare - Wikipedia</a></li>
<li><a href="https://thenewstack.io/cloudflare-acquires-deno-ryan-dahl/">Cloudflare acquires Node.js creator’s startup that... - The New Stack</a></li>
<li><a href="https://deno.com/blog/cloudflare">Deno is joining Cloudflare | Deno</a></li>
<li><a href="https://deno.com/blog/cloudflare">Deno is joining Cloudflare | Deno</a></li>
<li><a href="https://azeemhassni.com/blog/wire-deno-joins-cloudflare-deploy-shuts-down/">Deno team joins Cloudflare, Deno Deploy shuts down in six ...</a></li>

</ul>
</details>

**Tags**: `#cloudflare`, `#deno`, `#javascript`, `#runtimes`, `#acquisition`

---

<a id="item-tech-news-2"></a>
### [Oxide Computer Announces $445M Series D Funding Round](https://oxide.computer/blog/our-445m-series-d) ⭐️ 7.0/10

Oxide Computer, a maker of rack-scale server hardware built around open-source systems software, announced a $445 million Series D funding round in a post on its company blog. The announcement drew substantial discussion on Hacker News \(598 points, 268 comments\), where readers read it as a sign the company is moving toward scaled production of its rack-scale on-premises cloud systems. The round is an announced financing rather than a shipped capability or independently measured result, and details such as the investors, valuation, and stated use of proceeds were not included in the material available for this item.

hackernews · ahlCVA · Oct 9, 13:12 · [Discussion](https://news.ycombinator.com/item?id=50020014)

**「Background」** Oxide Computer, founded in 2019 and headquartered in Emeryville, California, sells rack-scale integrated server hardware combined with open-source software as an on-premises alternative to public cloud. According to an SEC Form D filing, the $445 million round is more than double the company&\#x27;s $200 million Series C led by Thomas Tull&\#x27;s USIT, and third-party funding trackers put Oxide&\#x27;s total raised across four rounds at roughly $742 million.

**「Impact」** Following the $200M Series C that funded Oxide&\#x27;s rack-scale on-premises cloud platform, this $445M Series D gives the company capital to scale production of racks that run AI, HPC, and mission-critical workloads with cloud-like elasticity, data residency, and cost control. Organizations considering on-premises deployments — as in the documented Lawrence Livermore installation — can treat Oxide as a better-capitalized supplier, lowering vendor-viability risk for multi-year hardware commitments.

**「What Readers Are Saying」** Several commenters praised Oxide&\#x27;s products and communications, but one reader questioned why the company raised equity instead of using trade finance to cover customer orders, speculating the round might be tied to locking in supply commitments from AMD and other suppliers. Others shared less flattering experiences and opinions: one described spending extensive time on a job application and waiting months for a rejection, and another argued that Oxide&\#x27;s AI-focused marketing devalues its brand image.

<details><summary>References</summary>
<ul>
<li><a href="https://fundediq.co/oxide-computer-company-oxide-computer-funding/">Oxide Computer Company: Funding , Investors &amp; Team... | FundedIQ</a></li>
<li><a href="https://aiweekly.co/alerts/oxide-computer-discloses-445m-funding-round-in-sec-form-d">Oxide Computer discloses $ 445 M funding round in SEC... | AI Weekly</a></li>
<li><a href="https://oxide.computer/">Oxide Computer Company</a></li>
<li><a href="https://trustpost.org/oxide-computer-series-c-funding-data-center-2026/">Oxide Computer Series C: $200M Funds Rack - Scale Cloud ...</a></li>
<li><a href="https://thenewstack.io/oxide-computer-installs-on-premises-servers-for-lawrence-livermore/">Oxide Computer Installs On - Premises Servers for... - The New Stack</a></li>

</ul>
</details>

**Tags**: `#hardware`, `#funding`, `#datacenter`, `#infrastructure`, `#open-source`

---

<a id="item-tech-news-3"></a>
### [JetBrains Releases Open-Source Coding Model Mellum 2.1](https://blog.jetbrains.com/ai/2026/10/mellum2-1-gets-to-work-a-fast-open-model-for-coding-agents/) ⭐️ 7.0/10

JetBrains has released Mellum 2.1, an open-source coding model under the Apache 2.0 license, with weights available on Hugging Face. The model uses a 12B-parameter mixture-of-experts architecture with only 2.5B active parameters and was trained via reinforcement learning in real environments. It is aimed at coding agents running locally, with capabilities that include exploring codebases, editing files, and checking modifications.

telegram · zaihuapd · Oct 9, 07:30

**「From Mellum to Mellum2.1」** The Mellum line began as a code completion model, and in June 2026 JetBrains expanded it with Mellum2, an open 12B mixture-of-experts model optimized for low-latency text-and-code workloads. Mellum2.1 is the successor to the Mellum2 Thinking version with an unchanged architecture — 12B total parameters and 2.5B active — with almost all of the new work going into post-training, primarily reinforcement learning. This release therefore refines an existing open model family rather than introducing a new one.

**「What it means for developers running local coding agents」** Developers building coding agents can now run a commercially usable model entirely on their own hardware: the Apache 2.0 license permits unrestricted commercial use and modification, while the mixture-of-experts design activating only 2.5B parameters per token keeps compute bounded enough for local execution rather than cloud API dependency. The concrete step is to pull the weights from Hugging Face and integrate Mellum2.1 into local agent runtimes, including as a fast sub-agent.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/blog/JetBrains/mellum2-launch">Introducing Mellum2: A 12B Mixture-of-Experts Model by JetBrains</a></li>
<li><a href="https://huggingface.co/JetBrains/Mellum2.1-12B-A2.5B-Thinking">JetBrains/Mellum2.1-12B-A2.5B-Thinking · Hugging Face</a></li>
<li><a href="https://blog.jetbrains.com/ai/2026/10/mellum2-1-gets-to-work-a-fast-open-model-for-coding-agents/">Mellum2.1 Gets to Work: A Fast Open Model for Coding Agents</a></li>
<li><a href="https://www.aimastery.page/news/jetbrains-mellum2-1-12b-moe-coding-agent">JetBrains Mellum2.1: 2.5B Active Params Reach 47 SWE-bench ...</a></li>
<li><a href="https://www.madebyagents.com/models/mellum2-1">Mellum2.1: Local VRAM and Hardware Fit - madebyagents.com</a></li>

</ul>
</details>

**Tags**: `#open-source-models`, `#coding-agents`, `#JetBrains`, `#machine-learning`, `#developer-tools`

---

<a id="item-tech-news-4"></a>
### [Telegram Desktop one-click flaw could silently steal files; fixed in 7.2.9](https://telegram.me/zaihuapd/44307) ⭐️ 7.0/10

Telegram Desktop versions below 7.2.9 reportedly contain a critical vulnerability, tracked as CVE-2026-107181, that lets a single click on a malicious tg:// link exfiltrate arbitrary files from the user&\#x27;s machine without any confirmation. The flaw stems from semicolons in links not being escaped, allowing them to be treated as separate IPC commands; combined with the interpret: handler, an attacker can reportedly steal documents, browser sessions, SSH keys, and cryptocurrency wallets. According to the report, which cites OpenNET, the fix has shipped in version 7.2.9, and users are advised to upgrade promptly, avoid suspicious tg:// links, and enable Telegram&\#x27;s local password protection.

telegram · zaihuapd · Oct 9, 09:51

**「Background」** tg:// links are deep links that launch Telegram Desktop the moment they are clicked in a browser, chat message, or document, so the app receives their contents with no confirmation step beyond the click itself. Internally, the client parses such input through an IPC command interface in which an interpret: handler executes application commands, meaning link text that is not properly escaped can reach a command-execution path instead of being treated as inert data.

**「Impact」** Telegram Desktop users on versions below 7.2.9 can have sensitive files such as SSH keys, browser session data, and crypto wallets silently taken with a single click on a malicious tg:// link, with no confirmation prompt or visible sign of access. Vulnerability trackers list CVE-2026-107181 as exploited in the wild, so anyone on an affected version should upgrade to 7.2.9 or later immediately, treat unsolicited tg:// links as hostile, and enable the local passcode as an added barrier against unauthorized file access.

<details><summary>References</summary>
<ul>
<li><a href="https://securityvulnerability.io/vulnerability/CVE-2026-107181">CVE - 2026 - 107181 : IPC Record-Separation Injection Vulnerability in...</a></li>
<li><a href="https://dbu.gs/vulnerability/PT-2026-107506">CVE - 2026 - 107181 — Telegram Telegram Desktop | dbugs</a></li>

</ul>
</details>

**Tags**: `#security`, `#vulnerability`, `#telegram-desktop`, `#arbitrary-file-read`, `#CVE-2026-107181`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Software&\#x27;s centaur age may last decades](https://seangoedecke.com/softwares-centaur-age-may-last-decades/) ⭐️ 5.0/10

rss · Sean Goedecke · Oct 10, 00:00

**「Background」** In chess, human-plus-AI &quot;centaur&quot; teams beat either humans or machines alone for roughly twenty years. The author argues software engineering is now in its own centaur age, and that how long this hybrid era lasts is the defining question for today&\#x27;s engineers.

**「Solution」** The author traces the arc from GitHub Copilot&\#x27;s 2022 autocomplete, through chat-based model help, to coding agents \(Cursor&\#x27;s agent mode in 2024, Claude Code in early 2025\). After Claude Opus 4.5&\#x27;s November 2025 release, he observes that agents are reliable enough to run unsupervised, but their failures now look like alignment mistakes rather than routine bugs — over- or under-engineering, mismatched technical values, misplaced priorities. His assessment: an unassisted engineer can no longer beat a centaur team, but neither can an unsupervised agent, since every impressive LLM result he has seen had a competent human in control. Predicting the era&\#x27;s length is hopeless in any rigorous sense, he argues: chess is simpler and amenable to self-play, but software is far more lucrative and funded; &quot;solving&quot; it would create more total work; generally-capable AI could disrupt software jobs indirectly; yet knitting&\#x27;s centaur age lasted two hundred years even as technology accelerated. Defaulting to chess&\#x27;s roughly twenty-year span, he advises engineers not to quit, to lean into the partnership, and to work out what human value remains — which he suspects is shifting from technical expertise toward alignment, though it&\#x27;s early days.

**「Takeaway」** The author&\#x27;s conclusion is that software&\#x27;s centaur age will plausibly last long enough to carry engineers through full careers, so the rational response is to become an effective centaur rather than panic — while candidly conceding the duration estimate rests on analogy and could prove wrong.

**Tags**: `#ai-coding-agents`, `#llm`, `#software-engineering-careers`, `#automation`, `#centaur-analogy`

---