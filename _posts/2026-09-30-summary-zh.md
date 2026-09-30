---
layout: default
title: "Horizon Summary: 2026-09-30 (ZH)"
date: 2026-09-30
lang: zh
---

> 从 50 条内容中筛选出 17 条重要资讯。

---

**科技新闻**
1. [OpenAI 发布 GPT-6.1 Sol：近 Astra 级智能，价格约为前代五分之一](#item-tech-news-1) ⭐️ 8.0/10
2. [OpenAI 发布常驻运行型 AI 智能体产品 Dots](#item-tech-news-2) ⭐️ 7.0/10
3. [浏览器实时太阳系可视化：52.6 万颗小行星与已跟踪卫星](#item-tech-news-3) ⭐️ 7.0/10
4. [IEEE Spectrum 复盘：德里如何将电网损耗从 50%降至 5%](#item-tech-news-4) ⭐️ 7.0/10
5. [PS5 漏洞利用 Relapse 公开，针对 WebKit JavaScriptCore 引擎](#item-tech-news-5) ⭐️ 7.0/10
6. [Quoting Anthropic Frontier Red Team](#item-tech-news-6) ⭐️ 7.0/10
7. [Simon Willison 开始实时直播 OpenAI DevDay 2026 大会](#item-tech-news-7) ⭐️ 7.0/10
8. [开源新书《How to Make Your Model Fast》讲解从芯片到智能体的模型加速](#item-tech-news-8) ⭐️ 7.0/10
9. [Cloudflare 推出面向 AI Agent 的命令行工具 cf 开放测试版](#item-tech-news-9) ⭐️ 7.0/10
10. [特朗普与六大科技巨头签署道义约束性 AI 安全协议](#item-tech-news-10) ⭐️ 7.0/10
11. [DeepSeek 据报开源面向华为升腾的基础计算组件](#item-tech-news-11) ⭐️ 7.0/10
12. [Cloudflare 宣布计划成为公共证书颁发机构](#item-tech-news-12) ⭐️ 7.0/10
13. [微软安排数百名外包人员审阅 Copilot 用户提示词与图片](#item-tech-news-13) ⭐️ 7.0/10

**财经新闻**
1. [中国商务部警告：若欧盟限制中企将&quot;坚决回应&quot;](#item-finance-news-1) ⭐️ 7.0/10
2. [美股盘前：Fair Isaac 因房贷定价新规暴跌 18%，AMD 以 82 亿美元收购 World Labs](#item-finance-news-2) ⭐️ 7.0/10
3. [特朗普市政债券持仓最高达 10 亿美元，利益冲突问题引发关注](#item-finance-news-3) ⭐️ 7.0/10
4. [中国据报为人形机器人企业 IPO 设三道新门槛](#item-finance-news-4) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [OpenAI 发布 GPT-6.1 Sol：近 Astra 级智能，价格约为前代五分之一](https://openai.com/index/introducing-gpt-6-1-sol/) ⭐️ 8.0/10

OpenAI 在 9 月 29 日的公告中推出 GPT-6.1 Sol，宣称以约为前代（GPT-6 Sol）五分之一的价格提供接近 Astra 级（near-Astra）的智能，主要面向通过 API 使用模型的应用开发者。公告中最受关注的变化是缓存输入定价降至每百万 tokens 0.10 美元——比标准输入定价低 95%，也比 GPT-6 Sol 的缓存输入低 50%，对依赖缓存输入的高频调用场景（如编程代理工作流）成本下降尤为明显。需要说明的是，接近前沿的能力描述目前仅出自 OpenAI 自己的公告，所提供材料中没有独立基准或评测加以验证，实际表现仍待使用者检验。

hackernews · crorella · 9月29日 17:06 · [社区讨论](https://news.ycombinator.com/item?id=49896586)

**「前代产品与定价基准」** 在 OpenAI 的模型序列中，GPT-6 Astra 是标准价格最高的旗舰档，也是这次“接近 Astra”定位所对照的基准：GPT-6.1 Sol 在 DevDay 2026 上发布，未缓存的标准输入与输出价格恰为 GPT-6 Astra 的五分之一（每百万输入 token 2 美元），0.10 美元的缓存输入单价为 Astra 的十分之一。它的直接前代 GPT-6 Sol，以及目前以每百万输入 token 4 美元折扣价提供的 GPT-5.6 Sol，构成了价格上的参照系——官方称此次缓存输入价格较 GPT-6 Sol 再降 50%，主要面向在多次请求间复用上下文的 Agent 工作负载。

**「对开发者的实际影响」** 对于在大模型 API 上构建产品的开发者，GPT-6.1 Sol 把近前沿（&quot;near-Astra&quot;）智能的价格压到前代约五分之一，且缓存输入降至每百万 token 0.10 美元——比标准输入定价低 95%、比 GPT-6 Sol 的缓存输入低 50%，这对 Codex 等高频复用上下文的智能体和编码工作流是直接的运行成本削减。不过各家厂商的基准声明不可直接比较：Anthropic 称 Opus 5.5 在 Terminal-Bench 4.0 上以 66.4% 对 57.9% 领先 GPT-6 Astra，OpenAI 则称 Sol 以更低成本在编码上匹敌 Fable 5.1，面对日趋在意成本的企业客户和低价开放权重模型的竞争，开发者应在自己的代码库上实测后再决定是否迁移。另需注意，有社区用户报告 GPT-6 Sol 相比 Sol 5.6 出现明显质量倒退并已转用 Opus 5.5，因此 6.1 的实际能力仍待独立验证。

**「社区讨论」** 讨论主要围绕价格战与商品化展开：whatifitoldyou 和 gradus\_ad 认为 token 定价成为主战场说明模型缺乏护城河、行业正滑向底价竞争，后者还猜测这可能是 Anthropic 今年选择上市的背景之一。与此相对，开发者 the\_duke 报告 GPT-6 Sol 相比 Sol 5.6 出现严重退步、自己已改用 Opus 5.5，因而对 6.1 能否带来实质提升持怀疑态度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thenextweb.com/news/openai-gpt-6-1-sol-price-astra-devday">‘Near-Astra intelligence for a fifth of the price’: GPT-6.1 Sol</a></li>
<li><a href="https://venturebeat.com/technology/openais-gpt-6-1-sol-offers-astra-like-performance-at-1-5th-price-a-new-ultrafast-tier-clocks-at-300-tokens-per-second">OpenAI&#x27;s GPT-6.1 Sol offers Astra-like performance at 1/5th price. A new Ultrafast tier clocks at 300 tokens per second. | VentureBeat</a></li>
<li><a href="https://openai.com/index/introducing-gpt-6-1-sol/">Introducing GPT-6.1 Sol | OpenAI</a></li>
<li><a href="https://fortune.com/2026/09/22/what-ai-slowdown-openai-anthropic-release-dueling-moreaffordable-models-as-ai-price-wars-heat-up/">What slowdown? OpenAI, Anthropic release dueling models as AI price wars heat up | Fortune</a></li>
<li><a href="https://www.progressiverobot.com/2026/09/23/ai-price-war-anthropic-openai-cheaper-ai-models/">Price War: Anthropic and OpenAI Smart, Proven AI Cuts</a></li>

</ul>
</details>

**标签**: `#openai`, `#llm`, `#model-release`, `#pricing`, `#ai-industry`

---

<a id="item-tech-news-2"></a>
### [OpenAI 发布常驻运行型 AI 智能体产品 Dots](https://openai.com/index/introducing-dots/) ⭐️ 7.0/10

根据 2026 年 9 月 29 日发布的公告，OpenAI 推出了 Dots，这是一款面向“常驻运行”（always-on）AI 智能体的产品，定位是让智能体持续在后台为用户执行任务。据讨论中引用的 OpenAI 支持文档，该产品目前不向欧洲经济区、瑞士和英国的用户开放。目前可得的信息仅来自官方公告链接与 Hacker News 讨论，属于厂商发布内容：其所宣称的常驻智能体能力尚未经独立验证，实际效用也存在争议。

hackernews · alvis · 9月29日 17:07 · [社区讨论](https://news.ycombinator.com/item?id=49896604)

**「何为“常驻”智能体」** “常驻”智能体（always-on agents）指无需用户逐步下达指令、可在后台持续运行并执行任务的 AI 助手。据媒体报道，Dots 在 OpenAI 的 DevDay 活动上发布，由 GPT-6 Astra 模型驱动，配备带网页浏览器的云端计算机，并被定位为 Meta 旗下 Muse 智能体的竞品。发布时机也颇为微妙：据 NBC News 报道，该公告是在 OpenAI 就其机器人被入侵事件道歉仅一天后发布的，产品因此在 AI 智能体“失控”争议声中亮相。

**「区域可用性受限」** Dots 在发布时仅向欧洲经济区、瑞士和英国以外地区的 Pro 订阅用户开放，可通过 ChatGPT 连接 4,000 多款应用；上述三个地区的用户目前无法使用，且 OpenAI 尚未公布这些地区的发布时间，Free、Go 和 Plus 档位同样没有确定日期。因此，位于受支持地区的 Pro 用户可以立即试用该智能体，而英国和欧洲的用户在规划基于 Dots 的工作流前需先确认所在区域的可用性，短期内可能需要等待官方扩展或寻找替代方案。

**「社区讨论」** 评论分歧明显：自称重度使用类似常驻智能体产品（Grok Bot）的 jjcm 认为，领域专用智能体之间的协作能在不塞满上下文窗口的前提下保留专业知识，并借专业化形成更清晰的信任边界；批评者（jwpapi、abeppu）则认为隔夜自动运行的实际收益有限，因为产出仍受人工审批节奏制约，而此前社区对同类工具（评论中提到的 openclaw）的共识——不要授予写入或删除权限、不要让它接触敏感数据——并未因模型改进而失效。另有评论者（mvkel）抱怨前沿 AI 公司发布的功能往往在约半年后为压缩算力成本而被大幅削减，与发布时的演示相去甚远。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/09/29/openai-launches-dots-its-bubbly-agentic-avatar/">OpenAI launches Dots, its bubbly agentic avatar | TechCrunch</a></li>
<li><a href="https://www.macrumors.com/2026/09/29/openai-launches-dots/">OpenAI Launches Always-On &#x27;Dots&#x27; Agents to Rival Meta&#x27;s Muse - MacRumors</a></li>
<li><a href="https://www.nbcnews.com/tech/tech-news/openai-launches-dots-ai-agents-safety-questions-rcna600338">OpenAI launches always-on AI agents a day after apologizing for a hack by its bots</a></li>
<li><a href="https://shattered.io/openai-dots-4000-apps-skip-uk-eu-2026/">OpenAI dots: 4,000+ Apps, No UK/EU Access Yet [2026]</a></li>
<li><a href="https://madrobot.blog/2026/09/29/chatgpt-dots-uk-europe-release-date/">ChatGPT Dots UK &amp; Europe Release Date: Is It Out? | MadRobot</a></li>
<li><a href="https://nerdschalk.com/chatgpt-dots-regional-availability/">When Will ChatGPT Dots Become Available in My Region?</a></li>

</ul>
</details>

**标签**: `#ai-agents`, `#openai`, `#agent-autonomy`, `#trust-and-safety`, `#product-launch`

---

<a id="item-tech-news-3"></a>
### [浏览器实时太阳系可视化：52.6 万颗小行星与已跟踪卫星](https://space.bl2.net/) ⭐️ 7.0/10

开发者 wanick 在 Hacker News 发布了浏览器端太阳系实时可视化站点 space.bl2.net，以真实比例呈现当前时刻的太阳系，包含约 52.6 万颗小行星以及 CelesTrak 目录中地球周边的已跟踪卫星。项目采用 WebGL2 渲染，轨道推算在 Web Worker 中运行；数据来自 CelesTrak 的 TLE（SGP4）、JPL SBDB 的小行星与彗星数据以及 JPL Horizons 的航天器位置，并每日更新。约 30 MB 的小行星数据集在后台加载，时间滑块可向前或向后移动，卫星会按发射日期出现或消失。这是一个已上线的可视化与教育工具，而非研究性突破或广泛部署的技术产品。

hackernews · wanick · 9月29日 19:08 · [社区讨论](https://news.ycombinator.com/item?id=49898778)

**「背景：公开轨道数据与此前报道」** 该项目能在浏览器中实时运行，依托的是长期公开且结构化的权威数据：CelesTrak 持续发布以两行根数（TLE）表示的地球轨道目标编目，配合 SGP4 传播模型即可推算任意时刻的卫星位置；NASA 喷气推进实验室（JPL）的 SBDB 数据库提供小行星与彗星轨道，Horizons 系统则提供航天器星历。此前的日报曾以“Space Now”为名收录同一网站，称其包含 526,000 颗小行星、35,164 颗卫星与航天器，以及 837 个从行星、卫星到矮行星和彗星的太阳系天体，此次 Show HN 提交是该作品在社区中的再次亮相。

**「对用户的影响」** 对天文爱好者和关注具体航天任务的用户，这是一个可直接使用的浏览器工具：数据每日更新自 CelesTrak 与 JPL，可实时查看约 52.6 万颗小行星和在册卫星的当前位置，并沿时间正反向推演轨道。实际用途已有用户验证——有评论者用它确认了 Europa Clipper 探测器即将进行的第二次地球引力助推，另一位报告普通笔记本即可以 60fps 以上帧率流畅渲染数十万天体。使用时需注意首次访问会在后台加载约 30 MB 的小行星数据集，低带宽环境应预留加载时间。

**「社区讨论」** 用户 FlowingRiver 回忆早年用 486DX 依靠 FPU 才能以约 30fps 计算 30 个天体的轨道，对比如今普通笔记本浏览器即可流畅渲染五十多万个天体，感叹硬件与 Web 技术的进步；用户 climech 则报告自己借此追踪到即将飞掠地球的 Europa Clipper 探测器，并称这是其继火星之后的第二次引力助推。另有评论者提出，当数据公开且结构良好时，此类可视化（包括借助 LLM 辅助开发）如今已容易实现，还有用户建议增加小行星人气投票等趣味功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zeli.app/story/49898778">Space Now - Real-time Solar System · 39 HN comments | Zeli</a></li>

</ul>
</details>

**标签**: `#webgl2`, `#data-visualization`, `#orbital-mechanics`, `#web-workers`, `#space`

---

<a id="item-tech-news-4"></a>
### [IEEE Spectrum 复盘：德里如何将电网损耗从 50%降至 5%](https://spectrum.ieee.org/delhi-electricity-loss) ⭐️ 7.0/10

IEEE Spectrum 于 2026 年 9 月 29 日发表回顾性深度报道，梳理德里如何将配电网损耗从 50%降至 5%，并称之为全球最显著的电网转型案例之一。报道将这一成果归因于技术改造与政策改革的结合；评论者引述的文章原文也指出，当年的损耗并非仅由技术因素造成。需要区分的是，这是一篇对已完成转型的复盘分析，而非新政策发布或新工程落地的消息。

hackernews · rbanffy · 9月29日 12:43 · [社区讨论](https://news.ycombinator.com/item?id=49892245)

**「背景」** 德里此次治理针对的是“AT&amp;C 损失”（综合技术与商业损失），即电能在技术损耗之外、因窃电、漏计费和电费收缴失败而未能变现的部分；《印度时报》2026 年 4 月 8 日曾报道，自 2002 年改革启动以来，德里已通过配电私有化、电网升级、智能电表、加强执法以及引入 AI 与 SCADA 系统，把这一损失率从约 52% 压至约 6%。其制度起点是印度 2003 年《电力法》：该法将邦级电网的发、输、配环节拆分为独立实体，并向私营资本开放电力行业。随后，2008 年 9 月为第十一个五年计划构想的 R-APDRP（重组加速电力发展与改革计划）又把降低 AT&amp;C 损失、改善各邦配电公司的财务状况列为核心目标，为这类改革提供了全国性的政策框架。

**「影响」** 对面临类似高损耗的电网运营方，该案例给出的可操作结论是：损耗并非纯技术问题，反窃电与计费、政策层面的改革需与线路和设备升级同步推进，仅靠硬件投入难以复制从 50%到 5%的降幅。

**「社区讨论」** 评论中最具分量的内容来自一位德里居民的回忆：二十年前当地一天停电数次、来电常伴随浪涌，人们得赶忙拔掉电视和笔记本电脑，办公室甚至布有两套插座；他认为与降损本身相比，计划外停电（load shedding）的消失才是真正革命性的变化。其他讨论包括：反窃电用的绝缘线路意外成了猴群在社区间穿行的“公路”；有评论者建议印度利用充足日照、用户对 UPS/逆变器的既有熟悉度以及屋顶光伏加电池，推动社区电力自给；也有人以爱沙尼亚电网作对照（据其引用，99%家庭装有智能电表、供电可靠性达 99.99%）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://timesofindia.indiatimes.com/city/delhi/from-50-losses-to-6-how-delhi-fixed-its-power-loses/articleshow/130121379.cms">From 50% losses to 6%: How Delhi fixed its power loses | Delhi News - The Times of India</a></li>
<li><a href="https://www.osti.gov/etdeweb/servlets/purl/21390277">Case of Reforms in the Indian Power Distribution Sector: A Move Towards</a></li>
<li><a href="https://spectrum.ieee.org/delhi-electricity-loss">How Delhi Cut Electricity Loss from 50 to 5 Percent - IEEE Spectrum</a></li>

</ul>
</details>

**标签**: `#power-grid`, `#infrastructure`, `#energy-policy`, `#india`, `#electrical-engineering`

---

<a id="item-tech-news-5"></a>
### [PS5 漏洞利用 Relapse 公开，针对 WebKit JavaScriptCore 引擎](https://github.com/ntfargo/Relapse-Exploit) ⭐️ 7.0/10

2026 年 9 月 29 日，一个名为 Relapse 的 PS5 漏洞利用项目在 GitHub 上公开，据仓库描述针对 PS5 内置浏览器所用的 WebKit JavaScriptCore 引擎。该发布在 Hacker News 上引发较高关注（301 分、177 条评论），但目前公开信息仅有代码仓库链接，漏洞利用所能达到的权限级别（用户态还是内核）、适用固件版本和可靠性均缺乏独立验证，因此尚不能确认它构成完整的系统破解。

hackernews · therepanic · 9月29日 15:44 · [社区讨论](https://news.ycombinator.com/item?id=49895304)

**「背景：WebKit 漏洞链与固件门槛」** PS5 自发售以来以难以出现公开可用漏洞著称，主机破解社区通常依赖浏览器 WebKit 引擎中的用户态漏洞，再配合内核漏洞组成完整利用链来运行未签名代码。据该仓库及相关报道，Relapse 正是这一模式的实例：它将 WebKit 内存泄漏与内核 aio\_multi\_wait 的 UAF（释放后使用）竞态串联，声称覆盖 7.00 至 13.60 固件，作者声明项目仅用于教育目的，并警告运行可能导致主机死机。固件版本是关键门槛，索尼尚未确认是否已在 13.60 之后的固件中封堵该漏洞。

**「影响」** 对运行 7.00–13.60 固件的 PS5 用户而言，社区已出现配套加载工具（WebKit Autoloader），可在主屏幕创建应用并自动缓存加载 Relapse 利用链，降低了部署门槛 \[tool-3-3\]。有用户期望借此把游戏存档备份到自己的 USB 介质——据其反映，PS5 目前只提供需订阅 PS Plus 的云备份且每个用户档案需单独订阅；但该漏洞的实际能力层级（用户态还是内核级、是否构成完整越狱）尚无独立验证。索尼方面一个具体的应对选项是禁用 PS5 WebKit 中的 JIT 以缩小攻击面 \[tool-3-1\]：WebKit 官方文档表明 JavaScriptCore 支持 no-JIT 的 &\#x27;mini mode&\#x27;，并称该模式更难被利用、内存占用更低 \[tool-3-2\]，因此这一收缩在技术上可行，也将使未来依赖 JIT 的利用链失效。

**「社区讨论」** 存档备份是评论中最强烈的诉求：一位用户称 PS5 不允许将存档备份到自己的存储介质、只能通过按账号订阅的 PS Plus 云备份，并提到女儿因数据损坏在 Minecraft 中丢失了一年进度（属个人经历陈述，未经独立核实）。技术上，有评论质疑 PS5 的 WebKit 是否在启用 JIT 的情况下运行 JavaScriptCore，并猜测索尼可能以禁用 JIT 来缩小攻击面；另有评论认为破解社区通常握有未公开的零日漏洞储备，还有用户期待借此在 PS5 上运行 Steam 游戏。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/ntfargo/Relapse-Exploit">GitHub - ntfargo/Relapse-Exploit: Exploit chain for PS5 7.00 - 13.60 · GitHub</a></li>
<li><a href="https://dev.to/lu1tr0n/relapse-repo-afirma-exploit-de-ps5-en-firmware-700-1360-1n14">Relapse: repo afirma exploit de PS5 en firmware 7.00-13.60 - DEV Community</a></li>
<li><a href="https://elsolitario.org/en/2026/09/29/relapse-repo-claims-ps5-exploit-firmware-7-00-to-13-60/">PS5 Jailbreak: What Is Relapse Exploit and Its Scope</a></li>
<li><a href="https://news.ycombinator.com/item?id=49898390">At a glance, it looks like it exploits a bug in WebKit &#x27;s * JavaScriptCore ...</a></li>
<li><a href="https://webkit.org/blog/10308/speculation-in-javascriptcore/">Speculation in JavaScriptCore | WebKit</a></li>
<li><a href="https://github.com/CielWhat/ps5-webkit-autoloader-13x">GitHub - CielWhat/ ps 5 - webkit -autoloader-13x · GitHub</a></li>

</ul>
</details>

**标签**: `#console-security`, `#exploit`, `#playstation-5`, `#webkit`, `#javascriptcore`

---

<a id="item-tech-news-6"></a>
### [Quoting Anthropic Frontier Red Team](https://simonwillison.net/2026/Sep/29/anthropic-frontier-red-team/) ⭐️ 7.0/10

Simon Willison quotes Anthropic&\#x27;s Frontier Red Team reporting that GLM-5.3 and Claude Mythos Preview now succeed at full control flow hijacks on binary exploitation benchmark tasks, a capability threshold earlier models did not cross.

rss · Simon Willison · 9月29日 22:20

**标签**: `#anthropic`, `#ai-safety`, `#cybersecurity`, `#llm-evaluations`, `#ai-security-research`

---

<a id="item-tech-news-7"></a>
### [Simon Willison 开始实时直播 OpenAI DevDay 2026 大会](https://simonwillison.net/2026/Sep/29/openai-devday-2026-live-blog/) ⭐️ 7.0/10

2026 年 9 月 29 日，Simon Willison 在旧金山 Fort Mason 现场参加 OpenAI DevDay 2026，并像去年一样实时记录主题演讲及当日其他开发者相关内容。截至该篇日志发布时，页面仅为开场记录，尚未包含任何具体的产品发布、版本或功能公告，实际内容取决于当日主题演讲的进展。他同时披露 OpenAI 向其提供了免费门票，以及主题演讲&quot;创作者&quot;（creator）区域的座位。

rss · Simon Willison · 9月29日 15:55

**「背景」** OpenAI DevDay 是 OpenAI 面向开发者的年度大会，新模型、API 和开发者工具通常在其主题演讲中公布，因此备受开发者社区关注。作者 Simon Willison 并非首次报道该活动：文中链接显示，他在 2025 年 10 月 6 日的 DevDay 上也曾以同样的 live blog 方式记录主题演讲，今年的报道延续了这一做法。

**「对 OpenAI 平台开发者的影响」** 依赖 OpenAI 模型和工具链的开发者与企业是本次大会的直接受影响方：据 OpenAI 官方回顾页面，DevDay 2026 包含超过 20 项公告，涵盖 GPT-6 Astra、ChatGPT、Codex、API、安全以及面向构建者的新工具。维护相关集成的团队需要逐一核对这份官方汇总，评估新模型与接口变化对现有应用的兼容性影响，并据此规划升级或采用工作。具体公告属于厂商发布内容，实际能力与限制仍需以官方文档和实测为准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/devday-2026-recap/">DevDay 2026 Recap - OpenAI</a></li>

</ul>
</details>

**标签**: `#openai`, `#llms`, `#coding-agents`, `#live-blog`, `#developer-ecosystem`

---

<a id="item-tech-news-8"></a>
### [开源新书《How to Make Your Model Fast》讲解从芯片到智能体的模型加速](https://www.reddit.com/r/MachineLearning/comments/1wt6ns4/i_wrote_a_free_opensource_book_on_making_ml/) ⭐️ 7.0/10

Reddit 用户 /u/SoloTiger\_ 于 2026 年 9 月 29 日在 r/MachineLearning 发布免费开源书籍《How to Make Your Model Fast: A Systems View of Efficient Machine Learning, from Silicon to Agents》，内容托管在 GitHub 仓库 usamahz/make-your-model-fast。该书的核心论点是：减少 FLOPs 并不一定能让模型更快，优化前必须先判断系统究竟受计算、带宽、内存还是系统级瓶颈约束。内容路线从 roofline 分析与硬件入手，依次覆盖内核、编译器、量化、剪枝、视觉、端侧 LLM、机器人、性能剖析、推理服务，最后延伸到智能体系统。需要说明的是，这是作者自行发布的介绍，书中内容的实际质量目前无法仅凭该公告独立验证。

reddit · r/MachineLearning · /u/SoloTiger\_ · 9月29日 10:35

**「背景」** 机器学习性能优化的核心前提是判断系统的实际瓶颈——究竟是受计算、带宽、内存还是系统层面限制——这正是 roofline 分析等方法要回答的问题，而单纯减少 FLOPs 并不必然带来加速。在这一领域此前已有类似的开源免费读物：jax-ml 项目在 GitHub 上发布的《How To Scale Your Model》一书讲解了 TPU 与 GPU 硬件的工作原理，以及 Transformer 在大规模训练和推理中如何高效并行化，其 GitHub 索引页可追溯至 2025 年 2 月 4 日，但该书侧重于模型扩展而非本书所覆盖的从硅片到智能体的端到端性能工程。本书作者 Usamah（GitHub 用户名 usamahz）是 Arm 的机器学习工程师，在 GitHub 上维护 62 个公开仓库。

**「影响」** 从事 ML 系统、推理、编译器或边缘 AI 工作的读者可以立即在 GitHub 免费阅读该书，作者同时公开征集反馈与代码贡献。对于需要判断量化、剪枝或内核优化是否值得投入的工程团队，书中提供的瓶颈分析方法可作为决策参考，但其实际效果有待读者自行检验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/usamahz">usamahz (Usamah) · GitHub</a></li>
<li><a href="https://jax-ml.github.io/scaling-book/">How To Scale Your Model - jax-ml.github.io</a></li>
<li><a href="https://github.com/jax-ml/scaling-book/blob/main/index.md">scaling-book/index.md at main · jax-ml/scaling-book · GitHub</a></li>

</ul>
</details>

**标签**: `#machine-learning-systems`, `#performance-engineering`, `#inference-optimization`, `#open-source`, `#hardware`

---

<a id="item-tech-news-9"></a>
### [Cloudflare 推出面向 AI Agent 的命令行工具 cf 开放测试版](https://blog.cloudflare.com/cloudflare-cf-cli-launch/) ⭐️ 7.0/10

Cloudflare 发布了 cf 命令行工具的开放测试版，目标是让开发者和 AI Agent 通过命令行直接调用 Cloudflare 全部 API。与现有 Wrangler 覆盖约 280 种操作不同，cf 由 API Schema 自动生成，覆盖超过 3,000 项 API 操作。它默认以 JSON 输出结果，并提供命令搜索与引导功能，便于 Agent 自动发现、执行操作并解析返回内容。Cloudflare 举例称，Agent 可用同一工具创建并部署 Worker、监控服务、配置 Access 与 WAF，甚至购买域名；该产品目前仍处于官方测试阶段，尚无独立验证。

telegram · zaihuapd · 9月29日 13:46

**「背景：Wrangler 的局限与 Agent 驱动的命令行需求」** Wrangler 是 Cloudflare 现有的官方命令行工具，长期用于 Workers 等产品的开发与部署流程，但其命令仅覆盖约 280 种操作，远少于平台实际提供的数千个 API 端点。与此同时，AI Agent 正日益依赖命令行来自动操作基础设施，对结构化输出和命令自动发现与引导能力的要求也随之提高，这构成了推出覆盖全 API 的新 CLI 的直接背景。

**「影响」** 对需要自动化管理 Cloudflare 资源的开发者和团队而言，cf 将单一路径下可脚本化的操作范围从 Wrangler 的约 280 项扩展到 3,000 余项，一条命令行工具即可覆盖从 Worker 部署到域名购买的完整流程，且 JSON 默认输出更利于程序解析。由于它仍是开放测试版，关键自动化流程的使用者应预期命令行为和覆盖范围可能调整，必要时保留 Wrangler 等现有方式作为回退。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.cloudflare.com/cloudflare-cf-cli-launch/">Introducing cf : the agentic CLI for the entire Cloudflare API</a></li>
<li><a href="https://github.com/cloudflare/cf">GitHub - cloudflare / cf : The agentic CLI for the entire Cloudflare API</a></li>

</ul>
</details>

**标签**: `#cloudflare`, `#cli`, `#ai-agents`, `#developer-tools`, `#api`

---

<a id="item-tech-news-10"></a>
### [特朗普与六大科技巨头签署道义约束性 AI 安全协议](https://www.zaobao.com.sg/news/world/story20260930-9758185) ⭐️ 7.0/10

据联合早报援引 CBS News 报道，美国总统特朗普当地时间 9 月 29 日与谷歌、Anthropic、Meta、OpenAI、xAI 和英伟达的掌门人共同签署一份一页纸的人工智能安全协议，并将文件发布在 Truth Social 上。协议要求企业建立四层控制机制：配合外部审计机构独立评估 AI 管控系统、设立董事会独立委员会进行监督，以及在模型训练和部署期间围绕网络安全、生物和化学威胁监控 AI 能力与对齐情况，确保各项措施按预期运行。特朗普称这份文件仅具有“道义约束力”，意味着相关承诺主要依赖企业自愿遵守，而非法律上的强制义务。

telegram · zaihuapd · 9月30日 02:30

**「自愿承诺替代强制监管的延续」** 这份协议延续了美国政府以企业自愿承诺替代强制立法的 AI 治理路线：特朗普此前已排除在其任内放缓 AI 发展的可能，将技术失控的担忧斥为“骗局”，并在 Truth Social 上写道“绝不会以任何方式阻碍或抑制这一非凡产业的发展”。据 France24 报道，他在推动该协议的同时拒绝了政府限制措施的呼声，敦促 AI 快速发展；《卫报》则指出，协议仅为 AI 公司在测试新产品时如何建立安全标准勾勒了一个模糊框架，特朗普称这将让企业对自身产品和技术进行“极大的自我监督”。

**「实际影响」** 对谷歌、Anthropic、Meta、OpenAI、xAI 和英伟达这六家签署企业而言，直接后果是需在无法律强制力的前提下自行建立外部审计、董事会独立监督，以及围绕网络安全、生物和化学威胁监控模型能力与对齐情况的内部机制。由于协议仅具&quot;道义约束力&quot;、属自愿性质，各公司是否落实及落实程度全凭自觉，依赖这些前沿模型的企业和开发者无法通过法律途径追究未履约行为，只能观察各公司后续的实际执行情况。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.france24.com/en/technology/20260929-trump-says-ai-companies-sign-voluntary-accord-on-safety-controls">Trump says AI companies sign voluntary accord on safety controls</a></li>
<li><a href="https://www.theguardian.com/us-news/2026/sep/29/trump-ai-deal-tech-ceos-superintelligence">Trump announces vague ‘morally binding’ AI deal... | The Guardian</a></li>
<li><a href="https://www.rt.com/news/646452-tech-pact-ai-controls/">Trump and US tech giants sign pact to stop AI from... — RT World News</a></li>
<li><a href="https://www.newsmax.com/politics/donald-trump-ai-accord/2026/09/29/id/1271143/">Trump Calls AI Pact &#x27;Morally Binding&#x27; as Tech Giants Commit to...</a></li>
<li><a href="https://www.usnews.com/news/top-news/articles/2026-09-29/trump-releases-ai-accord-with-tech-executives">Trump Releases AI Accord With Tech Executives</a></li>
<li><a href="https://cointelegraph.com/news/trump-accord-calls-for-tech-firms-to-self-police-their-own-frontier-ai">Trump , Tech CEOs Sign Voluntary Frontier AI Safety Pact</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#AI governance`, `#tech policy`, `#AI industry`, `#regulation`

---

<a id="item-tech-news-11"></a>
### [DeepSeek 据报开源面向华为升腾的基础计算组件](https://mp.weixin.qq.com/s/X41mKH4Ds-VXUAnK6M8Eww) ⭐️ 7.0/10

据单一聚合渠道（Telegram 转发的微信公众号文章）消息，DeepSeek 于 2026 年 9 月 30 日开源了面向华为升腾平台的基础计算组件，项目包括 DeepGEMM Ascend、DeepEP Ascend、TileKernels、FlashMLA 与 DeepSelect，覆盖 TileLang 高级语言编译工具、计算库和分布式通信库，与其英伟达平台组件相对应。DeepSeek 称相关组件在多项测试中性能接近硬件上限，并与华为推进升腾 950 的 128 卡超节点方案，但这些均属厂商宣称，尚未见 DeepSeek 或华为的官方仓库或公告佐证。该消息目前仅来自单一聚合渠道，发布日期也较为反常，真实性有待官方发布或独立渠道确认。若属实，在升腾硬件上进行部署的团队将能直接复用 DeepSeek 的开源算子与分布式通信栈。

telegram · zaihuapd · 9月30日 03:09

**「与英伟达平台组件一一对应的来龙去脉」** DeepGEMM、DeepEP、FlashMLA 等是 DeepSeek 此前在其英伟达（CUDA）平台上开源的训练推理基础组件，分别覆盖矩阵乘法计算、分布式通信与注意力内核等环节，此次发布的是它们向华为升腾平台的对应移植版本。据 GitHub 仓库说明，DeepGEMM Ascend 与原版 DeepGEMM 完全 API 兼容，支持 BF16、FP8、FP4 精度的 GEMM、MQA logits 和 MegaMoE；第三方仓库统计也称各组件接口与 CUDA 版本保持一致、可在升腾 950 上构建。相关报道称，研发过程中华为团队提供了大力支持，项目已在 GitHub 开源。

**「影响」** 对在华为升腾硬件上部署或训练大模型的开发者和企业而言，这意味着可以直接采用 DeepSeek 开源的生产级算子与通信栈：TileLang、DeepGEMM、DeepEP、FlashMLA 与其英伟达平台组件一一对应，并号称与 CUDA 工具链 1:1 对齐，有助于降低从 CUDA 迁移到升腾的适配成本（据 tool-3-1、tool-3-2）。结合双方正在推进的升腾 950 128 卡超节点方案——此前华为超节点技术已被报道用于支撑 DeepSeek V4 训练（tool-3-3）——规划大规模国产算力集群的团队在基础软件层多了一套可评估的开源选择。不过&quot;性能接近硬件上限&quot;等说法目前仅为 DeepSeek 单方披露，尚无独立测试佐证，生产环境采用前应在自有负载上实测验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tech.ifeng.com/c/8wpvR2zbzBw">DeepSeek 开 源 升 腾 基础组件：与英伟达平台一一对应_凤凰网</a></li>
<li><a href="https://github.com/deepseek-ai/DeepGEMM-Ascend">GitHub - deepseek -ai/ DeepGEMM - Ascend : DeepGEMM - Ascend ...</a></li>
<li><a href="https://trendshift.io/repositories/270861">deepseek -ai/ DeepGEMM - Ascend — GitHub trending stats... | Trendshift</a></li>
<li><a href="https://todayforai.com/zh/news/20260930-news-deepseek-ascend-infra-open-source">DeepSeek 开源升腾版全套 AI 基础设施：对齐 CUDA 工具链，适配 128 ...</a></li>
<li><a href="https://tech.china.com/article/20260930/202609301963239.html">DeepSeek开源升腾基础组件，联手华为优化128卡超节点</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/2031649923507172150">AI行业动态20260426: 华为&quot;超节点&quot;携升腾950芯片支撑DeepSeek V4训练...</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#Huawei Ascend`, `#open source`, `#AI infrastructure`, `#GPU kernels`

---

<a id="item-tech-news-12"></a>
### [Cloudflare 宣布计划成为公共证书颁发机构](https://blog.cloudflare.com/cloudflare-certificate-authority/) ⭐️ 7.0/10

Cloudflare 宣布计划进军公共证书颁发机构（CA）领域，已申请加入 Chrome、Apple、Microsoft 和 Mozilla 的根证书计划，并与 GlobalSign 签署协议收购一个受广泛信任的根证书。目前该公司尚未签发任何证书，此次属于意向性公告而非已上线的签发能力。新 CA 将优先支持通过 ACME 协议自动签发和续期证书。Cloudflare 还计划在 2027 年第一季度签发生产级默克尔树证书（Merkle Tree Certificates，MTC），以面向后量子互联网场景。

telegram · zaihuapd · 9月30日 06:26

**「背景」** 公共 CA 签发的证书之所以被浏览器和操作系统默认信任，是因为其根密钥被收录进 Chrome、Apple、Microsoft、Mozilla 等厂商维护的根证书计划，而新机构通常需要经过审计和分阶段纳入才能进入这些计划。ACME 是由 Let&\#x27;s Encrypt 推广的证书自动签发与续期协议，目前已成为 TLS 证书自动化管理的事实标准。此外，现有 TLS 证书普遍采用的 RSA 和椭圆曲线签名算法可被足够强大的量子计算机破解，Merkle Tree Certificates 正是为此提出的后量子替代证书格式。

**「影响」** 对网站运营者和开发者而言，Cloudflare 进入的是决定浏览器与操作系统如何信任网站的 Web PKI 生态；一旦其根证书被 Chrome、Apple、Microsoft 和 Mozilla 的根证书计划接受，证书获取将多一个原生支持 ACME 自动签发与续期的新选择，有助于简化 TLS 证书的生命周期管理。不过这一选择以各大根程序的审核通过为前提，且其面向后量子互联网的生产级默克尔树证书（MTC）计划要到 2027 年第一季度才会签发，Cloudflare 目前尚未签发任何证书，因此现有证书部署在短期内不会受到直接影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.cloudflare.com/pq-ca-with-mtcs/">Building a post-quantum certificate authority with... | Cloudflare Blog</a></li>

</ul>
</details>

**标签**: `#Cloudflare`, `#certificate-authority`, `#PKI`, `#post-quantum`, `#TLS`

---

<a id="item-tech-news-13"></a>
### [微软安排数百名外包人员审阅 Copilot 用户提示词与图片](https://www.404media.co/humans-reading-copilot-prompts-images/) ⭐️ 7.0/10

据 404 Media 报道，微软为改进 Copilot 的图片生成与编辑效果，雇佣了数百名外包合同工审阅用户提交的提示词与图片。报道称，这意味着用户发送给 Copilot 的对话内容、请求乃至随手上传的私人照片并非绝对私密，后台的真实人员可能逐一查看这些内容。报道同时指出，这些一线审查员在日常工作中被迫接触大量冲击性内容，包括低俗露骨照片、涉嫌偷拍（upskirt）的性暗示影像乃至潜在违法的动物祭祀画面，承受了严重的精神创伤。

telegram · zaihuapd · 9月30日 07:13

**「背景」** Copilot 的图像编辑功能允许用户上传照片并用文字描述想要的修改，云端模型据此生成改写结果，而评估这类生成质量需要人工比对提示词、原始照片和模型输出。据 404 Media 获取的内部承包商文件及 The Verge 等媒体的跟进报道，这些外包人员的职责是判断两次 AI 生成结果中哪一个更符合用户请求，属于质量评估而非传统意义上的内容审核，因此用户上传的照片和提示词会直接呈现到他们的工作界面中。由外包人员承担 AI 数据标注和用户内容人工审查在科技行业并非首例，此类岗位此前也曾多次曝出心理创伤问题。

**「影响」** 对使用 Copilot 图片生成与编辑功能的个人用户而言，提示词和上传的照片存在被外包人员人工审阅的可能，因此应避免在免费或 Pro 等缺乏同等保护措施的版本中提交私密照片或机密内容。企业用户受影响相对有限，其数据仍受组织既有的安全、合规与隐私策略约束。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://windowsreport.com/human-copilot-reviewers-are-seeing-users-disturbing-image-editing-requests-new-report-reveals/">Human Copilot Reviewers Are Seeing Users’ Disturbing Image ...</a></li>
<li><a href="https://www.theverge.com/ai-artificial-intelligence/1001381/human-workers-are-reviewing-prompts-and-images-sent-to-microsoft-copilot">Human workers are reviewing prompts and images sent to ...</a></li>
<li><a href="https://letsdatascience.com/news/microsoft-copilot-contractors-review-user-image-edits-6dcf58ca">Microsoft Copilot Contractors Review User Image Edits</a></li>
<li><a href="https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-365-copilot-architecture">Microsoft Copilot architecture and how it works</a></li>
<li><a href="https://spellbook.com/learn/is-copilot-private">Is Copilot AI Private? Legal Considerations for Lawyers</a></li>

</ul>
</details>

**标签**: `#AI privacy`, `#Microsoft Copilot`, `#content moderation`, `#data privacy`, `#AI ethics`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [中国商务部警告：若欧盟限制中企将&quot;坚决回应&quot;](https://www.cnbc.com/2026/09/30/china-warns-europe-increases-trade-pressure.html) ⭐️ 7.0/10

中国商务部表示，若欧盟对中国企业或产品施加限制，中方将&quot;坚决回应&quot;，并警告此类举动会&quot;严重破坏互信&quot;、干扰正在进行的中欧贸易谈判。此番警告正值欧盟贸易专员谢夫乔维奇下周访华之前，欧方要求北京在 10 月前拿出&quot;具体成果&quot;以缩减创纪录的对华贸易逆差，德法两国正推动欧委会加快打造可仿照美国&quot;301 条款&quot;、快速限制中国进入欧盟市场的工具，而去年中欧货物与服务贸易总额约为 8800 亿欧元。

rss · CNBC Finance · 9月30日 03:39

**「背景」** 所谓&quot;301 式&quot;工具仿照美国《1974 年贸易法》第 301 条，可让欧盟委员会无需等待世贸组织争端裁决，即单方面对别国加征关税、设置配额或采取其他限制措施；欧盟此前长期反对美国使用这一单边条款针对中国。

**「潜在影响」** 若欧盟限制措施落地而中方兑现报复，2023 年约三分之一销售额来自中国的德国车企，以及此前已被中国加征报复性关税的欧盟烈酒、猪肉和乳制品行业将首当其冲。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.atlanticcouncil.org/blogs/econographics/as-chinas-surpluses-become-unbearable-the-eu-is-edging-toward-its-own-section-301/">As China’s surpluses become unbearable, the EU is edging ...</a></li>
<li><a href="https://informedclearly.com/en/trade-war/61779/eu-china-trade-war-european-section-301-2026">EU-China Trade War: Brussels&#x27; European Section 301 Explained</a></li>
<li><a href="https://www.investing.com/news/stock-market-news/factboxeuropean-carmakers-exposed-to-any-chinese-retaliation-for-eu-tariffs-3483675">Factbox- European carmakers exposed to any Chinese retaliation for...</a></li>
<li><a href="https://www.bta.bg/en/news/world/1045335-on-the-road-to-nowhere-european-carmakers-face-ev-push-from-china">BTA :: On the Road to Nowhere? European Carmakers Face EV Push...</a></li>
<li><a href="https://www.reuters.com/business/autos-transportation/european-carmakers-exposed-any-chinese-retaliation-eu-tariffs-2024-06-13/">reuters.com/ business /autos-transportation/ european -carmakers...</a></li>

</ul>
</details>

**标签**: `#EU-China trade`, `#trade policy`, `#tariffs`, `#trade deficit`, `#retaliation threat`

---

<a id="item-finance-news-2"></a>
### [美股盘前：Fair Isaac 因房贷定价新规暴跌 18%，AMD 以 82 亿美元收购 World Labs](https://www.cnbc.com/2026/09/29/stocks-making-the-biggest-moves-premarket-fair-isaac-spacex-amd-more.html) ⭐️ 7.0/10

美股盘前交易中，Fair Isaac 股价暴跌 18%，因美国联邦住房金融局（FHFA）局长 Bill Pulte 宣布房利美与房地美将把 VantageScore 纳入现有 FICO 定价表，从两张定价表合并为一张统一的贷款定价表。其他主要波动包括：AMD 宣布以 82 亿美元收购 AI 公司 World Labs 后涨逾 1%，Summit Therapeutics 获阿斯利康 20 亿美元投资后飙升 18%，CarMax 因第二季度每股收益 1.16 美元（远超分析师预期的 73 美分、营收 78.8 亿美元高于预期的 70.9 亿美元）上涨逾 6%。

rss · CNBC Finance · 9月29日 12:03

**「背景」** 房利美和房地美此前按借款人的 FICO 信用分数，通过两套分开的定价表（即贷款级价格调整，指按分数向贷款机构收取的费用标准）收费；FHFA 局长普尔特周一宣布合并为一张统一表格并加入 FICO 的竞争对手 VantageScore，目的是在房贷信用评分领域引入竞争，打破了 FICO 的主导地位。AMD 以约 82 亿美元收购的 World Labs 是由有&quot;AI 教母&quot;之称的李飞飞创办的 AI 研究公司，交易以全股票形式进行。

**「影响」** 美国联邦住房金融局将房利美和房地美的抵押贷款定价统一为纳入 VantageScore 的单一网格，直接冲击 Fair Isaac 的核心评分（Scores）业务——该业务 2025 财年收入达 11.69 亿美元——引入竞争对手并削弱其此前在房贷信用评分定价上的主导地位。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.housingwire.com/articles/fhfa-gses-one-grid/">FHFA says GSEs will use one LLPA grid for FICO , VantageScore</a></li>
<li><a href="https://finance.yahoo.com/real-estate/articles/us-moves-end-fico-mortgage-131040861.html">The US Moves to End FICO ’s Mortgage Scoring Monopoly.</a></li>
<li><a href="https://www.fastcompany.com/91614972/fico-stock-collapsing-mortgage-industry-shakeup-credit-scores">FICO stock collapsing, mortgage industry shakes up... - Fast Company</a></li>
<li><a href="https://www.wsj.com/tech/ai/amd-to-acquire-world-labs-for-8-2-billion-a8d03d11">AMD to Acquire World Labs for $8.2 Billion - WSJ</a></li>
<li><a href="https://finance.yahoo.com/technology/article/amd-just-spent-82-billion-to-enlist-the-godmother-of-ai-230634166.html">AMD just spent $8.2 billion to enlist the &#x27;godmother of AI&#x27; - Yahoo Finance</a></li>
<li><a href="https://tickerspark.ai/market/fair-isaac-corporation-fico-tumbles-on-vantagescore-shift-1790685367142">Fair Isaac Corporation (FICO) tumbles on VantageScore shift - TickerSpark</a></li>
<li><a href="https://investors.fico.com/static-files/4dd43bd8-b07f-472c-9e53-5cb224ec9acd">[PDF] 2025 Annual Report - FICO Investor Relations</a></li>

</ul>
</details>

**标签**: `#premarket-movers`, `#mortgage-credit-policy`, `#earnings-surprise`, `#acquisitions`, `#biotech-investment`

---

<a id="item-finance-news-3"></a>
### [特朗普市政债券持仓最高达 10 亿美元，利益冲突问题引发关注](https://www.cnbc.com/2026/09/29/trump-municipal-bond-portfolio.html) ⭐️ 7.0/10

据 CNBC 对特朗普财务披露文件的分析，他截至 2025 年底持有 807 笔市政债券（价值 2.407 亿至 7.976 亿美元），2026 年以来又披露至少 243 笔新买入，合计持仓超过 1,000 笔、价值约 3 亿至 10 亿美元。由于煤电厂、公用事业和医院等许多债券发行方受其政府的监管与拨款决策影响，这一规模空前的个人持仓引发利益冲突质疑，但 CNBC 未发现不当交易证据，白宫称相关投资由独立机构全权管理。

rss · CNBC Finance · 9月29日 14:37

**「利益冲突法的适用范围」** 根据美国联邦利益冲突法（18 U.S.C. 第 208 条），联邦雇员不得参与涉及其个人财务利益的政府事务，但据 CNBC 报道，总统不在这一约束范围内。市政债券由城市、医院、公用事业等公共机构为筹资而发行，其偿付前景常受联邦监管与拨款决定影响，这正是利益冲突疑虑的来源。

**「影响」** 美国各地的地方政府、医院和公用事业等债券发行方的财务状况可能与联邦监管和拨款政策相互交织（如获得煤电污染豁免的电厂、依赖医疗补助拨款的医院），而总统豁免于典型利益冲突法规，使这一持仓与政策的重叠持续受到伦理专家关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.law.cornell.edu/uscode/text/18/208">18 U.S. Code § 208 - Acts affecting a personal financial interest</a></li>
<li><a href="https://www.ecfr.gov/current/title-5/chapter-XVI/subchapter-B/part-2640">eCFR :: 5 CFR Part 2640 -- Interpretation, Exemptions and ...</a></li>

</ul>
</details>

**标签**: `#municipal bonds`, `#Trump finances`, `#conflict of interest`, `#financial disclosures`, `#public policy`

---

<a id="item-finance-news-4"></a>
### [中国据报为人形机器人企业 IPO 设三道新门槛](https://www.cnbc.com/2026/09/29/china-criteria-humanoid-robot-ipos.html) ⭐️ 7.0/10

据三位知情人士透露，中国证监会以“窗口指导”形式要求寻求上市的人形机器人初创企业满足三项标准：拥有可持续营收和商业订单、亏损持续收窄（一位人士称需提供三年预测）、并掌握机器人大脑或灵巧手等核心技术。即便只需满足其中两项，仅在港交所递交上市申请的至少 24 家相关企业中，最终能上市的可能也只有少数几家甚至没有；证监会和港交所均未对此置评。

rss · CNBC Finance · 9月30日 02:50

**「背景」** 人形机器人属于中国政策力推的&quot;具身智能&quot;领域，全国相关企业已超过 100 家，仅在香港递交上市申请的就至少有 24 家。据 9 月 21 日报道，监管机构此前已通过非正式的&quot;窗口指导&quot;（即以口头方式私下传达政策要求）暂缓部分人形机器人企业上市，而行业龙头宇树科技 8 月 19 日在上海上市、募资约 61 亿元人民币后，股价已近乎腰斩。

**「影响」** 若这一窗口指导执行，仅在香港已递交上市申请的至少 24 家人形机器人初创企业及其背后投资者，可能因收入、亏损或核心技术不达标而无法上市，早期资本的退出渠道随之收窄。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.reuters.com/business/finance/china-slows-humanoid-robot-ipo-rush-hype-outruns-reality-2026-09-21/">China slows humanoid robot IPO rush as hype outruns reality - Reuters</a></li>

</ul>
</details>

**标签**: `#China`, `#humanoid-robots`, `#IPO-regulation`, `#CSRC`, `#embodied-AI`

---