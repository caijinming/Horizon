---
layout: default
title: "Horizon Summary: 2026-10-10 (ZH)"
date: 2026-10-10
lang: zh
---

> 从 43 条内容中筛选出 5 条重要资讯。

---

**科技新闻**
1. [Cloudflare 收购 Deno：运行时将获一年维护后停止开发](#item-tech-news-1) ⭐️ 9.0/10
2. [Oxide Computer 宣布 4.45 亿美元 D 轮融资](#item-tech-news-2) ⭐️ 7.0/10
3. [JetBrains 发布开源编程模型 Mellum 2.1](#item-tech-news-3) ⭐️ 7.0/10
4. [Telegram Desktop 7.2.9 修复一键窃取任意文件漏洞](#item-tech-news-4) ⭐️ 7.0/10

**科技博客**
1. [软件的“半人马时代”可能延续数十年](#item-tech-blog-1) ⭐️ 5.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Cloudflare 收购 Deno：运行时将获一年维护后停止开发](https://deno.com/blog/cloudflare) ⭐️ 9.0/10

Cloudflare 宣布收购 JavaScript 运行时 Deno，Deno 官方博客确认了这一消息。根据公告，Cloudflare 将在未来一年内以每月发布的频率为 Deno 运行时提供缺陷修复和安全更新，一年之后将结束对运行时的开发。Deno 项目本身将保持开源，官方欢迎愿意继续开发的其他团队接手。对已基于 Deno 构建项目的开发者而言，这意味着约一年的维护缓冲期，而非长期支持承诺。

hackernews · ilreb · 10月9日 13:03 · [社区讨论](https://news.ycombinator.com/item?id=50019911)

**「背景」** Deno 由 Node.js 的原始创造者 Ryan Dahl 推出，是一款以安全沙箱机制著称的 JavaScript/TypeScript 运行时，旨在从底层重新设计 Node.js 的开发体验。收购方 Cloudflare 是一家提供 CDN、网络安全与 DDoS 防护等服务的互联网基础设施公司，其自有的 Workers 平台同样用于运行 JavaScript 代码，与 Deno 在运行时生态中的定位相近。

**「迁移期限与兼容性影响」** 使用 Deno Deploy 的开发者面临六个月的关停窗口，需在此期间完成迁移，付费客户可获得向 Cloudflare Workers 迁移的支持；Deno 运行时本身仅再提供一年的月度错误修复与安全更新，此后除非社区接手，否则不再有官方维护。依赖 JSR 注册表和 rusty\_v8 的项目短期影响较小——Cloudflare 承诺 JSR 继续运营且基础设施迁至 Cloudflare，并将继续维护 rusty\_v8、推进其集成到 workerd，但这些属于厂商公布的计划而非已交付的能力，受影响团队应尽早评估迁移路径，避免把长期规划建立在一年的维护期之上。

**「社区讨论」** 评论区的失望情绪集中在对运行时前景的影响上：有开发者称 Deno 是自己最喜爱的 JS 运行时，并希望 Cloudflare 的 workerd 至少能吸收 Deno 的安全沙箱机制作为补偿；另一位曾深度投入 Deno 生态的开发者则认为，项目在转向优先兼容 npm、功能面持续膨胀后就已偏离初衷，融资压力使其放弃了从第一性原理重建 Node 的愿景。也有评论者将此次交易定性为实质上的&quot;收编式招聘&quot;（acquihire），并把它列入近年开发者工具持续被大型公司收购整合的趋势清单中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cloudflare">Cloudflare - Wikipedia</a></li>
<li><a href="https://thenewstack.io/cloudflare-acquires-deno-ryan-dahl/">Cloudflare acquires Node.js creator’s startup that... - The New Stack</a></li>
<li><a href="https://deno.com/blog/cloudflare">Deno is joining Cloudflare | Deno</a></li>
<li><a href="https://deno.com/blog/cloudflare">Deno is joining Cloudflare | Deno</a></li>
<li><a href="https://azeemhassni.com/blog/wire-deno-joins-cloudflare-deploy-shuts-down/">Deno team joins Cloudflare, Deno Deploy shuts down in six ...</a></li>

</ul>
</details>

**标签**: `#cloudflare`, `#deno`, `#javascript`, `#runtimes`, `#acquisition`

---

<a id="item-tech-news-2"></a>
### [Oxide Computer 宣布 4.45 亿美元 D 轮融资](https://oxide.computer/blog/our-445m-series-d) ⭐️ 7.0/10

Oxide Computer 于 2026 年 10 月 9 日在公司博客宣布完成 4.45 亿美元的 D 轮融资。该公司以向企业交付单机架式（rack-scale）本地部署服务器系统闻名，并长期以开源方式发布其固件与软件栈，在系统与开源社区中口碑颇高。此次属于融资公告而非已交付的产品或经独立验证的能力；现有公开材料未披露投资方、估值或资金用途等具体细节。该消息在 Hacker News 上引发了较大规模的讨论。

hackernews · ahlCVA · 10月9日 13:12 · [社区讨论](https://news.ycombinator.com/item?id=50020014)

**「Oxide 的业务与上一轮融资」** Oxide Computer 成立于 2019 年，总部位于加州 Emeryville，主营业务是将机架级集成服务器硬件与开源软件打包销售，作为本地部署（on-premises）云的替代方案。该公司此前一轮融资是由 Thomas Tull 旗下 USIT 领投的 2 亿美元 C 轮，本次 4.45 亿美元的 D 轮规模为其两倍以上；据第三方融资数据统计，其四轮融资累计披露金额约 7.42 亿美元。

**「影响」** 对评估本地部署基础设施的组织而言，这轮融资的直接意义在于 Oxide 的机架级整机柜系统有望扩大生产与交付规模：其上一轮 C 轮融资为 2 亿美元、同样投向机架级本地云，本轮 4.45 亿美元的规模翻了一倍多，可能增强其兼具数据驻留与成本可控的类云方案的供货能力。Oxide 机架定位为在本地运行 AI、HPC、关键任务及通用工作负载，并提供云端式弹性与统一管控，且已有劳伦斯利弗莫尔国家实验室等实际部署。正在规划本地化云环境的组织可将该整机柜方案纳入采购评估范围，同时关注其后续产能与交付安排。

**「社区讨论」** 评论区总体对 Oxide 表示支持，有评论称其是业内少有的&quot;以正确理由融资&quot;的公司；但也存在不同声音：一位评论者（activexray）抱怨其招聘流程耗时过长且长期没有反馈直至被拒；另一位（arpinum）质疑为何选择股权融资而非用贸易融资覆盖客户订单，并猜测公司可能是在向 AMD 等供应商锁定未来订单——这属于个人推测而非已证实的信息；还有人（thatsabadlook）批评公司在社交媒体上过度强调 AI 话题，认为这有损其品牌形象。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://fundediq.co/oxide-computer-company-oxide-computer-funding/">Oxide Computer Company: Funding , Investors &amp; Team... | FundedIQ</a></li>
<li><a href="https://aiweekly.co/alerts/oxide-computer-discloses-445m-funding-round-in-sec-form-d">Oxide Computer discloses $ 445 M funding round in SEC... | AI Weekly</a></li>
<li><a href="https://oxide.computer/">Oxide Computer Company</a></li>
<li><a href="https://trustpost.org/oxide-computer-series-c-funding-data-center-2026/">Oxide Computer Series C: $200M Funds Rack - Scale Cloud ...</a></li>
<li><a href="https://thenewstack.io/oxide-computer-installs-on-premises-servers-for-lawrence-livermore/">Oxide Computer Installs On - Premises Servers for... - The New Stack</a></li>

</ul>
</details>

**标签**: `#hardware`, `#funding`, `#datacenter`, `#infrastructure`, `#open-source`

---

<a id="item-tech-news-3"></a>
### [JetBrains 发布开源编程模型 Mellum 2.1](https://blog.jetbrains.com/ai/2026/10/mellum2-1-gets-to-work-a-fast-open-model-for-coding-agents/) ⭐️ 7.0/10

JetBrains 发布了开源编程模型 Mellum 2.1，模型权重已以 Apache 2.0 许可在 Hugging Face 上提供。该模型采用 12B 参数的混合专家（MoE）架构，每次推理仅激活 2.5B 参数，并通过真实环境中的强化学习进行训练。JetBrains 表示，该模型能够探索代码库、编辑文件并检查修改结果，主要面向在本地运行编程代理（coding agents）的开发者场景。

telegram · zaihuapd · 10月9日 07:30

**「背景」** Mellum 最初是 JetBrains 的代码补全模型，2026 年 6 月发布的 Mellum2 在此基础上扩展为一个面向低延迟文本与代码工作负载的开源 12B 混合专家模型。Mellum2.1 可视为 Mellum2 Thinking 的后续版本，其 12B 总参数、2.5B 激活参数的架构保持不变，本轮工作几乎全部投入在后训练阶段，尤其是强化学习。

**「对开发者的影响」** 对于希望在自有硬件上运行编程代理的开发者和企业，Mellum2.1 以 Apache 2.0 许可在 Hugging Face 开放权重，意味着可以自由下载、微调并商用部署，无需依赖云端 API 或支付许可费用。由于该模型每个 token 仅激活 2.5B 参数，推理计算量得到有效控制，适合在本地硬件上驱动编程代理和快速子代理。实际部署前应先核对本机显存与硬件适配情况，再决定是否纳入现有的代理式编码工作流。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/blog/JetBrains/mellum2-launch">Introducing Mellum2: A 12B Mixture-of-Experts Model by JetBrains</a></li>
<li><a href="https://huggingface.co/JetBrains/Mellum2.1-12B-A2.5B-Thinking">JetBrains/Mellum2.1-12B-A2.5B-Thinking · Hugging Face</a></li>
<li><a href="https://blog.jetbrains.com/ai/2026/10/mellum2-1-gets-to-work-a-fast-open-model-for-coding-agents/">Mellum2.1 Gets to Work: A Fast Open Model for Coding Agents</a></li>
<li><a href="https://www.aimastery.page/news/jetbrains-mellum2-1-12b-moe-coding-agent">JetBrains Mellum2.1: 2.5B Active Params Reach 47 SWE-bench ...</a></li>
<li><a href="https://www.madebyagents.com/models/mellum2-1">Mellum2.1: Local VRAM and Hardware Fit - madebyagents.com</a></li>

</ul>
</details>

**标签**: `#open-source-models`, `#coding-agents`, `#JetBrains`, `#machine-learning`, `#developer-tools`

---

<a id="item-tech-news-4"></a>
### [Telegram Desktop 7.2.9 修复一键窃取任意文件漏洞](https://telegram.me/zaihuapd/44307) ⭐️ 7.0/10

Telegram Desktop 7.2.9 之前的版本被曝存在严重漏洞（CVE-2026-107181）：用户点击恶意 tg:// 链接后，攻击者可在无需任何确认的情况下悄悄窃取任意文件。据该报道援引 OpenNET 的说法，漏洞根源在于链接中的分号未经转义、被当作独立的 IPC 命令执行，配合 interpret: 处理器可读取文档、浏览器会话、SSH 密钥、加密钱包等敏感文件。官方已在 7.2.9 版本中修复此漏洞，受影响用户应尽快升级，并警惕来历不明的 tg:// 链接、启用本地密码作为防护。

telegram · zaihuapd · 10月9日 09:51

**「背景」** tg:// 是 Telegram 的自定义 URL 协议：点击这类链接时，操作系统会把请求转交给本机正在运行的 Telegram Desktop 客户端，由客户端通过 IPC（进程间通信）接口解析并执行其中的命令，来源提及的 interpret: 处理器即用于解释执行指令。这种仅凭一个链接即可触发客户端本地操作的机制，要求对链接参数做严格的转义与校验，否则一段文本就可能被拆分、拼接成多条独立命令。

**「影响与应对」** 对仍在运行 7.2.9 之前版本 Telegram Desktop 的用户而言，风险直接且现实：漏洞数据库已将该问题标记为在野利用（exploited in the wild），远程攻击者可借助含未转义分号的 tg:// 链接注入 OPEN: 记录、触达 interpret: 处理器，利用 Core::Sandbox 中的 IPC 记录分隔符注入，在无任何确认的情况下窃取 SSH 私钥、浏览器会话、加密钱包等本地文件。受影响用户应立即升级到 7.2.9；在完成升级前避免点击来源不明的 tg:// 链接，并可按官方建议启用本地密码（local passcode）作为额外缓解措施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://securityvulnerability.io/vulnerability/CVE-2026-107181">CVE - 2026 - 107181 : IPC Record-Separation Injection Vulnerability in...</a></li>
<li><a href="https://dbu.gs/vulnerability/PT-2026-107506">CVE - 2026 - 107181 — Telegram Telegram Desktop | dbugs</a></li>
<li><a href="https://packages.altlinux.org/en/vuln/CVE-2026-107181">ALT Linux - All branches - Vulnerability CVE - 2026 - 107181 - Information</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#telegram-desktop`, `#arbitrary-file-read`, `#CVE-2026-107181`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [软件的“半人马时代”可能延续数十年](https://seangoedecke.com/softwares-centaur-age-may-last-decades/) ⭐️ 5.0/10

rss · Sean Goedecke · 10月10日 00:00

**「背景」** 作者将 2022 年以来的软件工程称为“半人马时代”：人类工程师与 AI 编程系统搭档，效果好于任何一方单独作战，正如人机组合曾主导国际象棋约二十年。真正的问题是，软件的这一时代会同样长久，还是更快终结。

**「方案」** 作者沿时间线梳理工具演进：GitHub Copilot 起初是 AI 自动补全，与 GPT-4 等模型对话是下一次升级；2024 年 Cursor 的 agent 模式与 2025 年初的 Claude Code 让编程智能体兴起，早期仍需密切监督。据作者个人经验，2025 年 11 月 Claude Opus 4.5 发布后的智能体已可靠到可完全无人监督运行，输出仍需人工审查，但错误更多是对齐层面的——不合组织的技术价值观、局部过度或不足设计——而非常规 bug。他据此断言：无辅助的工程师已不可能胜过人机组合，无人监督的智能体也尚未做到，半人马暂时占优。至于时长，他列举彼此抵消的因素：棋类问题更简单、更适用自我对弈；软件更有利可图、投入资金高出多个数量级；“解决”软件反而会扩大工作总量；通用 AI 的外溢效应可能冲击经济与岗位；编织业中人与织框的组合曾延续两百年；而技术变革又在加速。作者承认结果无法真正预知，只能默认参照最相近的棋类先例，估计还能延续十年到二十年。据此他建议：不要转行，拒绝成为半人马是注定失败之路；要持续思考人类剩余价值何在——2023 年靠技术专长，他认为如今正转向对齐（也有人主张“品味”，但难以非循环地定义）。

**「启示」** 作者的结论是：全面自动化的幽灵可能在远方盘旋数十年，足以容纳一份完整长度的职业生涯；工程师应基于行业当下的运作方式顺势成为半人马，而不是为尚未到来的末日提前恐慌跳船。

**标签**: `#ai-coding-agents`, `#llm`, `#software-engineering-careers`, `#automation`, `#centaur-analogy`

---