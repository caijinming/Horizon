---
layout: default
title: "Horizon Summary: 2026-09-30 (ZH)"
date: 2026-09-30
lang: zh
---

> 从 45 条内容中筛选出 11 条重要资讯。

---

**科技新闻**
1. [OpenAI 发布 GPT 6.1 Sol：号称以五分之一价格逼近 Astra 智能](#item-tech-news-1) ⭐️ 8.0/10
2. [社区公开 PS5「Relapse」漏洞利用，疑似针对 WebKit JavaScriptCore 缺陷](#item-tech-news-2) ⭐️ 7.0/10
3. [研究论文剖析网页与移动端对话式 AI 的隐私与追踪风险](#item-tech-news-3) ⭐️ 7.0/10
4. [OpenAI 宣布常驻智能体产品 Dots，具体能力尚未披露](#item-tech-news-4) ⭐️ 7.0/10
5. [Anthropic 红队：GLM-5.3 与 Claude Mythos Preview 实现完整控制流劫持](#item-tech-news-5) ⭐️ 7.0/10
6. [开源免费书《How to Make Your Model Fast》：从硬件到智能体的模型提速](#item-tech-news-6) ⭐️ 7.0/10
7. [甲骨文就星际之门项目电力审批延期发不可抗力通知](#item-tech-news-7) ⭐️ 7.0/10

**财经新闻**
1. [财政部等三部门：10 月 1 日起首套房商业贷款贴息年化 1 个百分点、最长 5 年](#item-finance-news-1) ⭐️ 8.0/10
2. [盘前异动：Fair Isaac 因房贷定价新规大跌 18%，AMD 宣布 82 亿美元收购 World Labs](#item-finance-news-2) ⭐️ 7.0/10
3. [特朗普市政债组合最高达 10 亿美元，与联邦政策范围重叠](#item-finance-news-3) ⭐️ 7.0/10
4. [据报中国为人形机器人企业 IPO 设三道门槛，达标者寥寥](#item-finance-news-4) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [OpenAI 发布 GPT 6.1 Sol：号称以五分之一价格逼近 Astra 智能](https://openai.com/index/introducing-gpt-6-1-sol/) ⭐️ 8.0/10

OpenAI 于 9 月 29 日宣布发布 GPT 6.1 Sol，官方定位为“以五分之一的价格提供接近 Astra 的智能”。据公告，其缓存输入定价为每百万 tokens 0.10 美元——比标准输入价格低 95%，也比前代 GPT-6 Sol 的缓存输入价格低 50%，评论区普遍认为这项降价才是本次发布的真正卖点，尤其利好 Codex 等高缓存用量的场景。上述性能与性价比表述均为厂商说法，尚无独立评测佐证；该消息在 Hacker News 上引发高强度讨论（752 分、约 695 条评论），核心争议是前代 Sol 6 被指的质量回退，以及前沿模型定价能否抗衡更便宜的替代品。

hackernews · crorella · 9月29日 17:06 · [社区讨论](https://news.ycombinator.com/item?id=49896586)

**「前作 Sol 6 的遇冷与 Astra 对标」** GPT 6.1 Sol 是对 OpenAI 前作 GPT-6 Sol 的快速跟进版本；在 Hacker News 的讨论中，多位开发者称 Sol 6 数日前才发布，且编码表现较上一代 Sol 5.6 明显退步，有人因此改用 Anthropic 的 Opus 5.5。标题中的 Astra 指被这些用户视为当前更强的竞品前沿模型，而以约五分之一的价格提供接近 Astra 的智能，正是 OpenAI 为这次发布给出的核心卖点。

**「缓存密集型工作负载的迁移机会与验证提醒」** 对运行 Codex 类编码代理或长上下文应用的开发者而言，GPT-6.1 Sol 最直接的影响是成本：其标准 API 定价为每百万输入 token 2 美元、缓存输入 0.10 美元、输出 10 美元，约为 GPT-6 Astra 标准价格的五分之一，其中缓存输入价格比 GPT-6 Sol 低 50%、比标准输入价格低 95%。高缓存复用的工作负载可以将此类任务迁移到该模型以降低经常性 API 支出；不过由于部分用户报告上一代 GPT-6 Sol 在编码任务上出现明显质量回退，切换前建议先在自身任务上验证输出质量再决定是否迁移。

**「社区讨论」** 评论中最受关注的声音对 6.1 持怀疑态度：the\_duke 称 Sol 6 相比 Sol 5.6 回退严重、迫使其全面转用 Anthropic 的 Opus 5.5，revolvingthrow 则推测 6.1 是数日前泄露文件中出现的“Astra-Minor”在临发布前的应急改名。另一派观点聚焦成本：proxysna 表示 DeepSeek 更快、便宜到智能差异“可忽略”，让自己今年无需为 200 美元月费买单；gradus\_ad 则将 token 价格成为主战场解读为对行业与投资者的不祥信号，并猜测这可能是 Anthropic 选择今年 IPO 的原因之一。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/introducing-gpt-6-1-sol/">Introducing GPT-6.1 Sol | OpenAI</a></li>
<li><a href="https://fourweekmba.com/ai-gpt-61-sol-cached-read-price-change/">GPT-6.1 Sol&#x27;s One Real Price Change Is the Cached Read - FourWeekMBA</a></li>
<li><a href="https://thenextweb.com/news/openai-gpt-6-1-sol-price-astra-devday">OpenAI releases GPT-6.1 Sol at a fifth of GPT-6 Astra’s token prices</a></li>

</ul>
</details>

**标签**: `#openai`, `#large-language-models`, `#model-releases`, `#ai-pricing`, `#developer-tools`

---

<a id="item-tech-news-2"></a>
### [社区公开 PS5「Relapse」漏洞利用，疑似针对 WebKit JavaScriptCore 缺陷](https://github.com/ntfargo/Relapse-Exploit) ⭐️ 7.0/10

GitHub 用户 ntfargo 公开发布了一个名为「Relapse」的 PS5 漏洞利用项目（仓库为 Relapse-Exploit），并于 2026 年 9 月 29 日经 Hacker News 传播引发大量讨论（223 分、122 条评论）。根据评论区的初步观察，该项目疑似利用 PS5 内置 WebKit 中 JavaScriptCore JavaScript 引擎的缺陷，但公开资料未说明受影响的固件版本范围，也未确认它能获得何种权限级别或能否实现完整越狱。讨论焦点包括 PS5 上 JavaScriptCore 是否启用 JIT 编译所带来的攻击面，以及索尼可能采取的缓解措施。该漏洞利用的实际影响取决于它覆盖的固件版本以及索尼的后续响应。

hackernews · therepanic · 9月29日 15:44 · [社区讨论](https://news.ycombinator.com/item?id=49895304)

**「PS5 越狱的典型利用链模式」** PS5 的越狱通常依赖“用户态入口 + 内核漏洞”的两段式利用链：先在主机内置的 WebKit 浏览器中利用 JavaScriptCore 引擎的缺陷取得初步代码执行，再借助独立的内核漏洞拿到完整的内核读写权限。第三方收录与外部报道显示，Relapse 走的正是这条路线——通过 WebKit JSC 信息泄露配合内核 aio\_multi\_wait 释放后使用（UAF）漏洞实现内核读写，据称可覆盖 7.00 至 13.60 固件，仅发布不足两周的 14.00.00 暂不受影响。由于这类浏览器是封闭主机上少数会解析不可信网页内容并运行 JavaScript 的组件，其带 JIT 编译的脚本引擎相应成为外部攻击者少有的用户态切入点。

**「对 PS5 用户的影响与固件取舍」** 该漏洞链据报道仅支持 7.00 至 13.60 固件，对索尼 2026 年 9 月 16 日发布的最新 14.00 固件无效，因此希望保留破解能力的用户应暂缓系统更新。实际可用性方面存在明显限制：演示中漏洞虽可在数秒内加载，但控制台每次重启后必须重新执行；项目页面还提示内核漏洞可能导致控制台卡死或崩溃，需重启后再试，浏览器阶段也可能需要多次尝试，页面卡住时应重新加载。

**「社区讨论」** 评论中较有分量的技术讨论来自 MaxBarraclough，他质疑 PS5 的 WebKit 是否在启用 JIT 的情况下运行 JavaScriptCore，并猜测索尼可能通过禁用 JIT 来收窄攻击面；Muromec 则推测此类破解社区通常手中还握有未公开的零日漏洞以及引导加载程序层面的线索，这属于个人判断而非已证实的事实。另有评论者从权利角度表态，如 aussieguy1234 认为用户需要破解自己合法拥有的硬件才能获得完全控制并不合理，也有人希望借此在 PS5 上运行 Steam 等 PC 游戏库。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://elsolitario.org/en/2026/09/29/relapse-repo-claims-ps5-exploit-firmware-7-00-to-13-60/">PS5 Jailbreak: What Is Relapse Exploit and Its Scope</a></li>
<li><a href="https://kotaku.com/new-ps5-jailbreak-exploit-works-on-systems-running-july-2026-firmware-2000738283">PS5 Jailbreak Exploit For Systems Running July 2026 Firmware</a></li>
<li><a href="https://sploitus.com/exploit?id=64E42AF3-CF08-5BE3-8BA8-BBD8F517B53C">Relapse-Exploit — PoC exploit | Sploitus</a></li>
<li><a href="https://github.com/ntfargo/Relapse-Exploit">GitHub - ntfargo/Relapse-Exploit: Exploit chain for PS5 7.00 ...</a></li>
<li><a href="https://soplayit.com/en/news/new-ps5-jailbreak-relapse-targets-older-firmware">New PS5 Jailbreak &#x27;Relapse&#x27; Targets Older Firmware - Soplayit</a></li>
<li><a href="https://tbreak.com/ps5-jailbreak-relapse-firmware-13-60/">PS5 jailbreak reaches firmware 13.60 with Relapse</a></li>

</ul>
</details>

**标签**: `#security`, `#exploitation`, `#playstation`, `#webkit`, `#console-hacking`

---

<a id="item-tech-news-3"></a>
### [研究论文剖析网页与移动端对话式 AI 的隐私与追踪风险](https://jorgegarciaherrero.com/wp-content/interactivos/20260916-Prompt-like-a-butterfly-sting-like-a-tracker-%28clean%29.pdf) ⭐️ 7.0/10

一篇研究论文以 PDF 形式发布在作者个人网站上，分析了网页端与移动端对话式 AI 代理的隐私实践，重点关注广泛使用的聊天工具中的追踪机制与数据暴露问题。该论文于 9 月 29 日经 Hacker News 提交后引发热议，获得 407 点和 128 条评论，讨论集中在三类具体风险：未发送的提示词草稿被周期性上传（提示词遥测）、会话页面中嵌入的广告追踪器，以及仅以 UUID 保护的对话 URL 会暴露完整聊天记录。需要说明的是，本次仅提供了论文链接而无正文摘录，其测量方法与逐项结论无法在此核实；ChatGPT、Perplexity 等具体案例目前出自评论区用户的个人观察。

hackernews · damaru2 · 9月29日 09:03 · [社区讨论](https://news.ycombinator.com/item?id=49890226)

**「从提示词泄露到应用内追踪」** 网页端与移动端的对话式 AI 服务在实现上与普通网站、应用采用相似的技术方式，因此同样可能内嵌第三方广告与追踪服务（Advertising and Tracking Services，ATS），而许多用户默认聊天窗口是一条只面向服务商的私密通道。在此之前，学术界对提示词隐私的讨论大多集中在模型侧风险——例如上下文学习过程可能泄露敏感数据——并有综述系统整理了相应的防护与缓解技术，相比之下，对已上线 AI 产品中实际部署的追踪器及其数据流向进行系统测量仍较为少见。

**「影响」** 对通过浏览器或手机应用使用 AI 聊天的用户而言，直接后果是：输入内容可能在点击发送之前就已传到服务器，而历史对话链接一旦被他人访问即可看到完整会话。可采取的做法是把托管聊天会话视作非机密渠道，避免粘贴未发表文稿、内部代码等敏感草稿；部分评论者主张改用可本地运行的开源模型，这属于个人应对选择而非论文结论。

**「社区讨论」** 评论中最具体的观察来自 pbasista：他发现 ChatGPT 网页版会周期性地把未发送的提示词草稿上传到 conversation/prepare 端点，推测这些数据可能用于缓存预热，也可用于刻画用户的写作节奏与思路演化；postalcoder 则指出 Perplexity 等服务仅以 URL 中的 UUID 充当隐私屏障，访问旧链接即暴露整段对话。另有评论者将此与当月初的 Navier-Stokes 署名争议相类比——据其转述，OpenAI 承认去标识化的产品数据可能改进了其模型——并据此主张开源模型在隐私上必须胜出。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2404.06001v1">Privacy Preserving Prompt Engineering: A Survey - arXiv.org</a></li>

</ul>
</details>

**标签**: `#privacy`, `#conversational-ai`, `#tracking`, `#llm`, `#security`

---

<a id="item-tech-news-4"></a>
### [OpenAI 宣布常驻智能体产品 Dots，具体能力尚未披露](https://openai.com/index/introducing-dots/) ⭐️ 7.0/10

OpenAI 在官网发布《Introducing Dots》一文，宣布推出名为 Dots 的常驻智能体（always-on agents）产品。该消息经 Hacker News 转载后引发较大反响（451 分、341 条评论）。不过，所提供的材料中没有任何关于 Dots 实际能力、定价、可用范围或技术架构的具体细节，因此目前只能确认这是一项厂商公告，而非经过独立验证的已交付功能，其真实能力和发布条件仍有待官方文档或第三方测评确认。

hackernews · alvis · 9月29日 17:07 · [社区讨论](https://news.ycombinator.com/item?id=49896604)

**「背景」** Dots 是 OpenAI 在旧金山举行的 DevDay 2026 开发者大会上发布的，该公司当天共宣布了 20 多项消息，Mashable 称 Dots 是其中分量最重的一项。按照 OpenAI 的官方描述，Dots 属于“常驻”（always-on）智能体：它们能够了解什么对用户重要、持续代表用户工作，并把重要事务从用户手中接走。《连线》杂志的报道则将其称为 OpenAI 对 Meta 的回应。

**「平台锁定与迁移成本」** OpenAI 在 DevDay 上发布的 Dots 定位为可连接用户各类应用、执行多步骤任务的常驻智能体，并与 Meta 的个人 AI 智能体 Muse 形成直接竞争。对用户而言，采用此类服务意味着授权智能体访问自己的应用生态，并在平台侧持续积累任务记录；有评论者警告，与可以随时更换的底层模型不同，智能体因平台集成与工作历史沉淀而更难迁移，构成实质性的平台锁定风险。因此，用户在接入前应审慎评估所需授予的应用权限，以及数据与工作记录的可迁移性。

**「社区讨论」** 评论区的核心担忧是平台锁定：aditya\_rs 认为常驻智能体凭借对其他平台的集成和工作历史把用户深度绑定在单一平台上，比可随时替换的模型更难迁移，相当于把“你的电脑”搬到云端；johnfahey 则担心 OpenAI 在以宽松额度吸引开发者转入 Codex 后，会像 Anthropic 一样收紧限制并推销多余产品。另有 wxw 表示 Codex、ChatGPT Work 与 Dots 三者的产品边界日益模糊，jameslk 则认为此类运行在云端虚拟机上的智能体可能终结 PC 时代——以上均为评论者个人观点，而非已证实的事实。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/introducing-dots/">Introducing dots - OpenAI</a></li>
<li><a href="https://mashable.com/tech/openai-dev-day-dots-ai-agents">OpenAI introduces Dots, a new always-on AI agent, at Dev Day</a></li>
<li><a href="https://www.wired.com/story/openai-dots-always-on-ai-agents-that-proactively-help/">OpenAI’s Dots Are Always-On AI Agents—and Its Answer to Meta ...</a></li>
<li><a href="https://www.adweek.com/media/openai-takes-on-metas-muse-with-dots-an-always-on-ai-agent/">OpenAI Takes On Meta&#x27;s Muse With Dots, an Always-On AI Agent</a></li>
<li><a href="https://www.wired.com/story/openai-dots-always-on-ai-agents-that-proactively-help/">OpenAI’s Dots Are Always-On AI Agents—and Its Answer to Meta ...</a></li>
<li><a href="https://ai.meta.com/muse/">Muse: Meta&#x27;s personal AI agent, features &amp; capabilities</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#OpenAI`, `#platform lock-in`, `#product strategy`, `#developer tools`

---

<a id="item-tech-news-5"></a>
### [Anthropic 红队：GLM-5.3 与 Claude Mythos Preview 实现完整控制流劫持](https://simonwillison.net/2026/Sep/29/anthropic-frontier-red-team/) ⭐️ 7.0/10

Anthropic 前沿红队（Frontier Red Team）在报告《GLM-5.3 and the spread of advanced cyber capabilities》中称，在其内部二进制漏洞利用（Binary Exploitation）基准中随机抽取的 100 个任务上，GLM-5.3 在 4% 的试验中完成了完整的控制流劫持，Claude Mythos Preview 则达到 6%。相比之下，Claude Opus 4.6 和 GLM-5.2 等更早的模型在这些任务上均无一成功，Anthropic 由此判断“一个有意义的阈值已被跨越”。Simon Willison 在博客中转引了这段结论，但未附加自己的分析。需要说明的是，该结果来自 Anthropic 自有内部基准的评估，属于该实验室的单方研究结论，目前尚无独立验证。

rss · Simon Willison · 9月29日 22:20

**「背景」** Anthropic 的内部二进制漏洞利用（Binary Exploitation）基准用于测试模型能否在参与 Google OSS-Fuzz 项目的流行开源软件中发现并利用漏洞，其中只有完成完整的控制流劫持（full control-flow hijack）才能获得满分，这代表一种较高级的自动化攻击能力。被测试的 GLM-5.3 属于 GLM 系列第五代开源前沿大语言模型。在此项结果出现之前，Claude Opus 4.6 和 GLM-5.2 等更早的模型在该基准的任何任务上都未能实现这一目标。

**「影响与应对」** GLM-5.3 以开放权重形式发布，Anthropic 评估其未配备限制滥用的实质性安全防护，这意味着自主完成二进制漏洞利用的能力已经扩散到任何能获取该模型权重的人。Anthropic 的模拟测试还显示，简单技巧绕过 GLM-5.3 内置防护的成功率达 64% 到 100%，因此部署或微调该模型的组织不能依赖其自身安全机制，需要自行落实访问控制与使用审计。对防御方而言，Z.ai 报告 GLM-5.3 在测试中于 Linux、WebKit、FreeBSD 等主流开源代码库发现 1,097 个严重漏洞，同一能力也可用于攻击未及时修补的系统，安全团队应优先推进关键补丁并评估开放权重模型带来的暴露面。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/research/glm-5-3-and-the-spread-of-advanced-cyber-capabilities">GLM - 5 . 3 and the spread of advanced cyber capabilities \ Anthropic</a></li>
<li><a href="https://glm5.app/">GLM 5 — Next-Gen Frontier Model</a></li>
<li><a href="https://www.anthropic.com/research/glm-5-3-and-the-spread-of-advanced-cyber-capabilities">GLM-5.3 and the spread of advanced cyber capabilities \ Anthropic</a></li>
<li><a href="https://www.technology.org/2026/08/17/zai-glm-5-3-cybergym-mythos-5-benchmarks/">Z.ai GLM-5.3 Nears Mythos 5 on Bug Hunting - Technology Org</a></li>
<li><a href="https://ai-tldr.dev/releases/anthropic-glm-5-3-cyber-report/">Anthropic tests GLM-5.3 — its safeguards fall to… | AI/TLDR</a></li>

</ul>
</details>

**标签**: `#ai-security`, `#llm-research`, `#cybersecurity`, `#anthropic`, `#ai-safety`

---

<a id="item-tech-news-6"></a>
### [开源免费书《How to Make Your Model Fast》：从硬件到智能体的模型提速](https://www.reddit.com/r/MachineLearning/comments/1wt6ns4/i_wrote_a_free_opensource_book_on_making_ml/) ⭐️ 7.0/10

Reddit 用户 /u/SoloTiger\_ 发布了免费开源书籍《How to Make Your Model Fast: A Systems View of Efficient Machine Learning, from Silicon to Agents》，内容托管在 GitHub 仓库 usamahz/make-your-model-fast，面向 ML 系统、推理、编译器和边缘 AI 方向的从业者。书中的核心论点是：减少 FLOPs 不一定能让模型变快，优化前必须先判断系统究竟受计算、带宽、内存还是系统层面约束。全书从 roofline 分析与硬件讲起，依次覆盖 kernel、编译器、量化、剪枝、视觉、端侧 LLM、机器人、性能剖析、推理服务，直至智能体（agent）系统。需要说明的是，这是一则作者自述的发布帖，书籍的完整度和社区反馈目前尚无独立验证。

reddit · r/MachineLearning · /u/SoloTiger\_ · 9月29日 10:35

**「背景」** 理解这本书的前提是屋顶线（roofline）分析这一体系结构方法：先用硬件的峰值算力与内存带宽判断工作负载究竟受算力还是受数据搬运限制，这正是作者所说“单纯减少 FLOPs 未必能让模型变快”的原因。在机器学习效率这一主题上，社区此前已有覆盖部分相关内容的公开资源，例如 HSE 大学与 Yandex 数据分析学院公开的 Efficient Deep Learning Systems 课程材料，以及侧重生产级机器学习工程的 Made-With-ML 课程仓库。

**「影响」** 从事推理优化、编译器、边缘 AI 和性能工程的开发者现在可以免费获取一份按“瓶颈分析、kernel、量化、推理服务到智能体”递进的系统级学习材料。作者明确征集该领域从业者的反馈与贡献，早期读者可直接在 GitHub 仓库提交 issue、参与改进或加星支持，其反馈可能影响书籍后续的内容覆盖与质量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/GokuMohandas/Made-With-ML">GitHub - GokuMohandas/Made-With-ML: Learn how to develop ... GitHub - mryab/efficient-dl-systems: Efficient Deep Learning ... zero-to-mastery-ml/section-1-getting-ready-for-machine ... GitHub - apple-aiml-research/ml-fastvit: This repository ... How to Develop an AI Model Faster and More Efficiently</a></li>

</ul>
</details>

**标签**: `#machine-learning`, `#performance-engineering`, `#inference-optimization`, `#systems`, `#open-source`

---

<a id="item-tech-news-7"></a>
### [甲骨文就星际之门项目电力审批延期发不可抗力通知](https://www.bloomberg.com/news/articles/2026-09-24/oracle-cites-force-majeure-to-shield-itself-on-controversial-data-center) ⭐️ 7.0/10

甲骨文就星际之门（Stargate）位于新墨西哥州的 Project Jupiter 数据中心发出不可抗力通知，起因是配套 2.45GW 微电网的环境与供电审批迟迟未落地，项目面临无法在 2028 年按期投运的风险。根据该通知，甲骨文拟在外部因素导致延期时推迟部分付款，以规避自身承担延期责任。消息引发市场对超大型 AI 数据中心建设进度与融资风险的担忧，该项目相关的 180 亿美元银团贷款已出现折价交易。目前星际之门多数项目仍处于土建、审批和能源配套阶段，仅得州阿比林园区等少数园区投产，得州也已暂停新数据中心项目审批。

telegram · zaihuapd · 9月29日 05:46

**「背景：星际之门与不可抗力条款」** 星际之门是一个超大规模 AI 数据中心建设计划，目前多数项目仍处于土建施工、审批和电力配套阶段，仅得州阿比林园区等少数园区建成投运。不可抗力条款是指在发生一方无法控制的外部事件（如环境与供电审批延误）时，允许其免除或推迟履行合同义务的合同约定，Dealroom 转述的报道正是以该条款来解释甲骨文此次通知的法律依据。

**「融资端影响」** 不可抗力通知所涉的 Project Jupiter 约 180 亿美元银团建设贷款分销已陷入停滞，安排行桑坦德（Santander）与杰富瑞（Jefferies）难以把这笔债务转售给其他投资者；该贷款二级市场报价仅为面值的 89–91 美分，对应市值缩水至约 160 亿至 164 亿美元。承销该贷款的银行因此直接承担账面损失风险，参与或评估超大规模 AI 数据中心融资的机构需要将电力审批延期这类外部风险计入债务定价与放款条件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://app.dealroom.co/news/note/oracle-files-force-majeure-on-2-45gw-new-mexico-stargate-data-center">Oracle files force majeure on 2.45GW New Mexico Stargate data center | Dealroom.co</a></li>
<li><a href="https://finance.biggo.com/news/aa2b00f9-d885-40e0-92db-6fd9f55ffe63">Oracle&#x27;s $18 Billion AI Loan Sells at a Discount, Banks Forced to Swallow a Hot Potato — BigGo Finance</a></li>
<li><a href="https://www.roic.ai/news/oracle-invokes-force-majeure-on-project-jupiter-as-ai-data-center-financing-stumbles-09-24-2026">Oracle Invokes Force Majeure on Project Jupiter as AI Data Center Financing Stumbles | Roic News</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#data centers`, `#Oracle`, `#Stargate`, `#energy policy`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [财政部等三部门：10 月 1 日起首套房商业贷款贴息年化 1 个百分点、最长 5 年](https://jrs.mof.gov.cn/zhengcefabu/phjr/202609/t20260929_3998312.htm) ⭐️ 8.0/10

中国财政部、中国人民银行和金融监管总局 9 月 29 日联合印发通知，自 2026 年 10 月 1 日起在全国对新购买首套住房的商业性个人住房贷款实施中央财政贴息，政策暂定实施 1 年。建筑面积不超过 120 平方米且房价不超过 150 万元的首套房家庭，可按贷款本金获得年化 1 个百分点的贴息，贴息期限最长 5 年，单户可享受贴息的贷款规模上限为 100 万元，据此测算每年最高贴息约 1 万元。

telegram · zaihuapd · 9月29日 10:18

**「政策背景」** 贴息是指由财政替借款人承担部分贷款利息。此前，财政部、中国人民银行和金融监管总局已自 2025 年 9 月起对部分个人消费贷款实施财政贴息，并于 2026 年 1 月将该项政策延长至 2026 年底，此次购房贷款贴息是将同类做法扩展到首套住房商业贷款领域。

**「影响」** 购买建筑面积 120 平方米以下、总价 150 万元以下首套住房的家庭是直接受益方，按现行首套商业房贷利率水平，年化 1 个百分点的贴息约相当于利率优惠三分之一（三部门负责人答问口径），业内分析这将降低刚需购房者的实际利息负担、提振入市信心。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.dzwww.com/xinwen/guoneixinwen/202601/t20260120_17326136.htm">三 部 门：将个 人 消费 贷 款 财 政 贴 息 政 策 实施期限延长至 2026 ...</a></li>
<li><a href="https://news.china.com/socialgd/10000169/20260111/49152594.html">news.china.com/socialgd/10000169/20260111/49152594.html</a></li>
<li><a href="https://www.gznews.com/2026/09/29/6386.html">重磅！全国首套房贷国家贴息政策落地10月1日起实施 | 广州新闻网</a></li>
<li><a href="https://news.ifeng.com/c/8wotukhlA7p">居民房贷贴息政策10月1日起实施，力度多大？哪些购房者受益？_凤凰网</a></li>

</ul>
</details>

**标签**: `#housing policy`, `#mortgage subsidy`, `#China real estate`, `#fiscal policy`, `#financial regulation`

---

<a id="item-finance-news-2"></a>
### [盘前异动：Fair Isaac 因房贷定价新规大跌 18%，AMD 宣布 82 亿美元收购 World Labs](https://www.cnbc.com/2026/09/29/stocks-making-the-biggest-moves-premarket-fair-isaac-spacex-amd-more.html) ⭐️ 7.0/10

据 CNBC 盘前行情汇总，Fair Isaac 因美国联邦住房金融局（FHFA）局长 Bill Pulte 宣布将房利美与房地美的抵押贷款定价由两套费率表合并为一套、并将 VantageScore 纳入现有 FICO Classic 费率表，股价盘前暴跌 18%。其他主要个股方面：AMD 宣布以 82 亿美元收购李飞飞创办的 AI 公司 World Labs 后上涨逾 1%；Summit Therapeutics 因获阿斯利康 20 亿美元战略投资大涨 18%；CarMax 公布第二季度每股收益 1.16 美元、营收 78.8 亿美元，均高于分析师预期的 73 美分和 70.9 亿美元，股价上涨逾 6%。

rss · CNBC Finance · 9月29日 12:03

**「背景」** FICO（费尔艾萨克）的主要利润来自按次向房贷机构收取信用评分费用，而房利美和房地美这两家政府支持的房贷机构过去对 FICO 与竞争对手 VantageScore 分别适用两套贷款定价表（LLPA，即决定借款人利率加点的收费表），使 VantageScore 难以真正进入房贷市场。据行业报道，FHFA 公告发布数小时后，TransUnion 将 VantageScore 4.0 的房贷定价锁定在每份 0.99 美元，远低于 FICO 自定的 2026 年每份 4.95 美元许可价，市场因此担忧 FICO 的房贷评分收入将被直接分流。

**「影响」** VantageScore 进入房利美和房地美统一的房贷定价体系后，贷款机构获得了 FICO 之外的新评分选择，直接冲击 Fair Isaac 利润最高的按揭信用评分业务——该业务此前主要依靠提价推动收入增长。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.housingwire.com/articles/fhfa-gses-one-grid/">FHFA says GSEs will use one LLPA grid for FICO, VantageScore</a></li>
<li><a href="https://www.ctol.digital/news/fico-stock-drop-fhfa-one-pricing-grid-vantagescore/">Pulte just priced FICO&#x27;s mortgage moat at 99 cents</a></li>
<li><a href="https://wrenews.com/fico-shares-plunge-mortgage-vantagescore-competition-2026/">FICO Shares Plunge More Than 20% as VantageScore Threat Grows</a></li>
<li><a href="https://finance.yahoo.com/markets/stocks/articles/fair-isaac-fico-down-19-041752218.html">Fair Isaac (FICO) Is Down 19.2% After FHFA Opens Mortgage Scoring To VantageScore Competition - Has The Bull Case Changed?</a></li>
<li><a href="https://tickeron.com/blogs/fair-isaac-fico-shares-fall-17-4-as-mortgage-scoring-faces-new-competition-16838/">Fair Isaac (FICO) Shares Fall -17.4% as Mortgage Scoring Faces New Competition</a></li>

</ul>
</details>

**标签**: `#premarket-movers`, `#earnings`, `#mergers-and-acquisitions`, `#mortgage-policy`, `#credit-scores`

---

<a id="item-finance-news-3"></a>
### [特朗普市政债组合最高达 10 亿美元，与联邦政策范围重叠](https://www.cnbc.com/2026/09/29/trump-municipal-bond-portfolio.html) ⭐️ 7.0/10

根据 CNBC 对财务披露文件的分析，特朗普总统持有的市政债券组合已超过 1,000 笔，按披露区间估算价值约 3 亿至 10 亿美元，专家称这一规模对个人投资者前所未有；其中许多发行方——包括城市、医院和电力公司——直接受其政府的监管、拨款和医疗资金决定影响。报道未发现特朗普或其管理人利用政策内幕交易的证据，白宫与特朗普集团表示投资由独立金融机构全权管理。

rss · CNBC Finance · 9月29日 14:37

**「背景」** 市政债券是美国地方政府、医院和公用事业等公共机构为筹资发行的债务，联邦拨款、监管和医疗资金决定会影响发行方的财务和偿债能力，而总统依法豁免于一般利益冲突规定。文中举出的例子是：特朗普账户于 2025 年 2 月买入佐治亚电力 Bowen 电厂的污染控制债券，57 天后他签署公告，让包括该厂在内的数十座燃煤电厂在两年内免于执行更严格的联邦有毒空气污染限制。

**标签**: `#municipal bonds`, `#Trump finances`, `#conflict of interest`, `#financial disclosures`, `#presidential ethics`

---

<a id="item-finance-news-4"></a>
### [据报中国为人形机器人企业 IPO 设三道门槛，达标者寥寥](https://www.cnbc.com/2026/09/29/china-criteria-humanoid-robot-ipos.html) ⭐️ 7.0/10

据三位知情人士称，中国证监会通过&quot;窗口指导&quot;要求寻求上市的人形机器人初创企业满足三项标准：具备可持续营收和商业订单、亏损收窄（一名人士称需三年预测），并掌握机器人大脑或灵巧手等核心技术，即便只需满足其中两项，据称能达标的企业也寥寥无几或没有。该消息未获证监会或港交所证实；作为行业背景，龙头宇树科技 8 月 19 日在上海上市募资约 61 亿元人民币，首日股价飙升逾 460%至 845 元，截至周一已跌至 459.65 元、近乎腰斩。

rss · CNBC Finance · 9月29日 07:19

**「背景」** 中国目前有超过 100 家人形机器人企业，均属官方近年力推的“具身智能”（即把人工智能装进实体机器人）范畴，据消息人士称，仅在香港提交上市申请的相关企业就至少有 24 家。作为行业标杆的宇树科技（Unitree）于 8 月 19 日在上海上市，募资约 61 亿元人民币（约 9.05 亿美元），首日股价暴涨逾 460%至 845 元，但截至周一已近乎腰斩至每股 459.65 元。

**「影响」** 中国 100 多家人形机器人初创企业首当其冲：由于内地公司赴港上市同样需要中国证监会批准，达不到可持续营收、亏损收窄或核心技术等新门槛的公司可能只有极少数甚至没有能完成上市，其 IPO 融资和早期投资者的退出渠道将收窄；市场压力已提前显现，港股上市的优必选年内股价累计下跌逾 40%。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/09/29/china-criteria-humanoid-robot-ipos.html">China &#x27;s criteria for humanoid robot IPOs may be hard to meet</a></li>
<li><a href="https://wordupnews.com/crypto/china-has-three-new-criteria-for-humanoid-robot-ipos-few-if-any-meet-them/">China has three new criteria for humanoid robot IPOs . Few, if any...</a></li>
<li><a href="https://www.cnbc.com/2026/09/29/china-criteria-humanoid-robot-ipos.html">China has three new criteria for humanoid robot IPOs. Few, if any, meet them</a></li>

</ul>
</details>

**标签**: `#China`, `#humanoid robots`, `#IPO regulation`, `#Unitree`, `#AI bubble`

---