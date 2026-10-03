---
layout: default
title: "Horizon Summary: 2026-10-03 (ZH)"
date: 2026-10-03
lang: zh
---

> 从 38 条内容中筛选出 10 条重要资讯。

---

**科技新闻**
1. [新 AI 以约 34 倍训练效率攻克隐藏信息游戏 Stratego，超越 DeepNash](#item-tech-news-1) ⭐️ 8.0/10
2. [Zig 0.17.0 发布：社区关注语言设计与 AI 立场转变](#item-tech-news-2) ⭐️ 8.0/10
3. [Redis 创造者发布本地运行大模型的开源工具 ds4（DwarfStar）](#item-tech-news-3) ⭐️ 7.0/10
4. [Greg Kroah-Hartman 核查 LLM 宣称的 79 个 Linux 内核漏洞：多数无效或已修复](#item-tech-news-4) ⭐️ 7.0/10
5. [arXiv 新规：每位提交者每月最多提交 2 篇论文](#item-tech-news-5) ⭐️ 7.0/10
6. [Claude Code 推出 mods 机制：用 TypeScript 改写提示词与内置功能](#item-tech-news-6) ⭐️ 7.0/10

**科技博客**
1. [超级说服将更像贿赂而非超级论证](#item-tech-blog-1) ⭐️ 7.0/10

**财经新闻**
1. [9 月就业数据疲弱，市场对美联储 10 月加息的押注大幅降温](#item-finance-news-1) ⭐️ 7.0/10
2. [美股盘前异动：耐克跌超 10%，安森美以 57 亿美元收购新思科技](#item-finance-news-2) ⭐️ 7.0/10
3. [Bitget &\#x27;not expecting to recover a lot&\#x27; from $388 million hack, CEO tells CNBC](#item-finance-news-3) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [新 AI 以约 34 倍训练效率攻克隐藏信息游戏 Stratego，超越 DeepNash](https://arstechnica.com/science/2026/10/ai-finally-beat-the-best-stratego-player-in-history-and-did-it-on-a-budget/) ⭐️ 8.0/10

据 Ars Technica 报道，一项已链接至《自然》论文及 arXiv 预印本（编号 2511.07312）的研究称，一种新 AI 系统在隐藏信息桌游 Stratego 上超越了此前最先进的 DeepNash，同时训练所需对局数约少 34 倍，最终棋力反而更强。DeepNash 是 DeepMind 于 2022 年发布的无模型多智能体强化学习系统，曾被视为 Stratego AI 的标杆；由于双方棋子身份大多隐藏，常规的前瞻搜索在这类游戏中难以奏效，Stratego 因此长期被视作不完美信息博弈的难点。需要说明的是，上述棋力与效率数字目前来自论文作者与报道的表述以及社区评论的引用，尚未见独立复现的测量结果。

hackernews · PaulHoule · 10月2日 14:11 · [社区讨论](https://news.ycombinator.com/item?id=49933740)

**「背景：DeepNash 此前的里程碑」** Stratego（陆军战棋）是一种不完全信息博弈：棋子的具体身份对对手隐藏，无法像国际象棋那样直接进行确定性的向前搜索推演，因此长期被视作游戏 AI 的难题。此前该领域的标杆是 DeepMind 于 2022 年推出的 DeepNash，它将博弈论与无模型深度强化学习相结合，从零开始自学下 Stratego 并达到专家级水平。

**「对博弈 AI 研究者的实际影响」** 对研究隐藏信息博弈的开发者与研究者而言，最直接的影响是训练门槛显著降低：据报道，新算法所需的对局训练量约为 DeepNash 的三十四分之一，且最终棋力更强，这意味着研究团队可以在远小于此前的训练预算下复现乃至改进顶尖水平的不完全信息博弈智能体。该算法细节已通过报道中附带的 arXiv 预印本和《自然》论文链接公开，有意者可直接查阅并尝试复现或在此基础上改进。由于不完全信息博弈涵盖拍卖、谈判与安全等大量实际应用问题，训练效率的提升也为这类方法向上述场景迁移降低了算力成本。

**「社区讨论」** 在 Hacker News 的讨论中，janalsncm 认为约 34 倍的样本效率才是这项工作的核心——隐藏信息游戏中一手棋的好坏取决于你无法得知的对手信息，因此不能像完全信息游戏那样前瞻搜索；smokel 则表示这让 2022 年 DeepNash 论文标题中的&quot;mastering&quot;显得为时过早，新方法才算真正强于人类。两者均为评论者的个人解读，效率与棋力结论仍应以原论文为准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=3vO45gcEbRs">AI beats us at another game : STRATEGO | DeepNash ... - YouTube</a></li>
<li><a href="https://deepmind.google/blog/mastering-stratego-the-classic-game-of-imperfect-information/">Mastering Stratego , the classic game of... — Google DeepMind</a></li>
<li><a href="https://www.researchgate.net/publication/221455006_Better_automated_abstraction_techniques_for_imperfect_information_games_with_application_to_Texas_Hold&#x27;em_poker">Better automated abstraction techniques for imperfect information ...</a></li>

</ul>
</details>

**标签**: `#AI research`, `#game AI`, `#hidden information games`, `#reinforcement learning`, `#sample efficiency`

---

<a id="item-tech-news-2"></a>
### [Zig 0.17.0 发布：社区关注语言设计与 AI 立场转变](https://ziglang.org/download/0.17.0/release-notes.html) ⭐️ 8.0/10

Zig 0.17.0 已正式发布，官方发布说明上线于 ziglang.org，该消息于 10 月 2 日经 Hacker News 报道并引发较大讨论（约 209 分、132 条评论）。评论者关注的话题包括语言设计、广泛的交叉编译目标支持、构建系统集成方面的变化，以及项目对利用 LLM 辅助发现 bug 表现出的务实态度。需要说明的是，该条目本身未详述本次发布的具体变更内容，完整清单以官方发布说明为准；评论中提到的无栈协程 IO 实现和一等公民模糊测试工具仍是社区对未来版本的期待，而非本次发布确认落地的能力。Zig 目前仍处于 1.0 之前的阶段，生态规模较小。

hackernews · ErenayDev · 10月2日 20:56 · [社区讨论](https://news.ycombinator.com/item?id=49938521)

**「背景」** Zig 是一种定位于替代 C、C++ 和 Rust 的通用系统编程语言，目前仍处于 1.0 之前的 0.x 版本阶段，语言与生态尚未稳定。此次 0.17.0 版本于 2026 年 10 月 2 日发布，汇集了 5 个月的工作成果，包含来自 206 位贡献者的 925 次提交。

**「对开发者的影响」** 使用 zig build 的开发者在 0.17.0 中可获得可量化的构建提速：构建系统重构使墙钟时间从约 150ms 降至 14.3ms（约 90%），改进后的 ELF 链接器让增量编译对多数 x86\_64-linux 项目可用，配合 \`zig build -fincremental --watch\` 可在源码变动后近乎即时重建。平台覆盖方面，aarch64-openbsd 已纳入 Zig CI 的原生测试，可获得持续的质量保障。由于本次构建系统重构包含破坏性变更，计划升级到 0.17.0 的团队需要检查并迁移现有构建脚本。

**「社区讨论」** 多位评论者给出很高评价：一位有 JS、C、Pascal、Go 开发经验的用户称在用 Zig 完成一年项目后认为它是自己用过的设计最好的语言，另一位则认为其交叉编译目标支持可能是少数能与 C 相提并论的语言——这些均为个人评价而非测量结果。讨论中最受关注的是项目对 AI 的立场：有评论者提到 Zig 作者 Andrew 受 SQLite 相关成果启发，正将 LLM 辅助发现 bug 视为通向无 bug 软件的工具，这与另一位评论者记忆中项目此前对 AI 的强硬态度形成反差；而一位自称因被封禁而转向 Odin 语言的用户对核心成员行为的负面描述，属于未经证实的个人说法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ziglang.org/news/0.17.0-released/">0 . 17 . 0 Released Zig Programming Language</a></li>
<li><a href="https://www.youtube.com/watch?v=kxT8-C1vmd4">Zig in 100 Seconds - YouTube</a></li>
<li><a href="https://ziglang.org/download/0.17.0/release-notes.html">0.17.0 Release Notes ⚡ The Zig Programming Language</a></li>
<li><a href="https://daily.dev/posts/zig-0-17-0-release-notes-y2kcmyvvv">Zig 0.17.0 Release Notes - daily.dev</a></li>
<li><a href="https://byteiota.com/zig-build-system-rework-90-faster-ships-in-0-17/">Zig Build System Rework: 90% Faster, Ships in 0.17 | byteiota</a></li>

</ul>
</details>

**标签**: `#zig`, `#programming-languages`, `#systems-programming`, `#open-source`, `#compilers`

---

<a id="item-tech-news-3"></a>
### [Redis 创造者发布本地运行大模型的开源工具 ds4（DwarfStar）](https://dwarfstar.sh/) ⭐️ 7.0/10

ds4（DwarfStar）是一款用于在本地硬件上运行大语言模型的新开源工具，项目主页为 dwarfstar.sh；据 2026 年 10 月 2 日的 Hacker News 发布帖，它出自 Redis 的创造者之手，评论区还给出了 GitHub 仓库 antirez/ds4。发布后社区已出现实质性衍生工作：有用户维护了以共享库形式发布、可经 FFI 从其他语言调用的分叉并编写了 Go 绑定 ds4go，同时随上游加入了 Vision 与 Qwen 支持；另一位开发者受其启发，为配备 32GB 内存的 Intel Xe-LP（无 XMX）笔记本编写了独立推理引擎 xenolith，目前支持量化的 Gemma-4。目前没有公开的基准测试或性能数据：有用户报告在 M5 Max 128GB 上运行 Qwen 3.8 Flash Next 一周多、称速度快且上下文窗口长，但这类体验属于个人报告，工具调用能力与实际吞吐尚待验证。

hackernews · fibo · 10月2日 18:01 · [社区讨论](https://news.ycombinator.com/item?id=49936575)

**「ds4 的出身与技术定位」** ds4（DwarfStar 4）的代码托管在 GitHub 的 antirez 账户下，发布帖将其作者与 Redis 创作者联系起来，这层背景是该工具在系统开发者社区中迅速获得关注的前提。就定位而言，它是一个面向高内存 Mac（Metal）及 CUDA、ROCm 机器的精简 C 语言推理引擎，支持 DeepSeek V4 与 V4.1 Flash、GLM 5.x 和 Qwen3.8 Flash Next（后者为 125B MoE 模型，据项目页面可在 8GB 以上 NVIDIA GPU 上运行），并同时提供文本与视觉模型、本地 API、CLI 和原生代理。与常见的“本地推理另起 HTTP 服务”方案不同，ds4-agent 直接执行推理、无需独立服务器进程，并把 token 历史与模型实时状态保存在一起。

**「对本地推理用户的影响」** 想在本地运行 DeepSeek V4 Flash 与 PRO 的用户可直接查阅 ds4 官方基准页做硬件选型：页面按 Mac、DGX Spark、CUDA 和 ROCm 分别列出 prefill 速度、生成速度与上下文长度，这回应了社区对实际吞吐数字的追问。兼容性方面，仓库说明工具调用、KV 状态与内置编码代理在集成测试中一并构建和验证，技术报告也演示了原生工具调用，因此依赖 tool calling 的本地工作流具备可验证的基础；生态上社区还出现了编译为共享库的 FFI fork（含 Go 绑定 ds4go），以及面向 Intel Xe-LP 无 XMX 32GB 笔记本的衍生推理引擎 xenolith，不过后者目前仅支持量化版 Gemma-4。

**「社区讨论」** 该帖收获 150 分和 39 条评论，讨论中已有具体内容：neomantra 介绍了自己维护的共享库形式分叉及 Go 绑定 ds4go（含 workspace/scratchpad 等工具库），simoiacos 则展示了受 DwarfStar 启发、面向 32GB Intel Xe-LP 笔记本的推理引擎 xenolith，目前仅支持量化的 Gemma-4 并希望未来支持类似的 MoE 模型。使用反馈与质疑并存：ttoinou 称自最初支持 DeepSeek V4 Flash 起就在使用，在 M5 Max 128GB 上运行 Qwen 3.8 Flash Next 一周多&\#x27;非常快&\#x27;且上下文窗口很长（但偶有遗忘前文的情况），而 cuttothechase 指出工具调用效果和接近 50 tokens/秒 的吞吐目前没有任何数据或视频佐证，并从 GitHub 仓库推断似乎不需要大内存、SSD 即可。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/antirez/ds4">GitHub - antirez / ds 4 : DeepSeek 4 Flash and PRO local inference ...</a></li>
<li><a href="https://williamcallahan.com/bookmarks/dwarfstar-sh">DwarfStar 4 ( ds 4 ): Local DeepSeek V4.1, Qwen and GLM</a></li>
<li><a href="https://dwarfstar.sh/">DwarfStar 4 ( ds 4 ): Local DeepSeek V4.1, Qwen and GLM</a></li>
<li><a href="https://dwarfstar.sh/benchmarks/">ds4 Benchmarks: DeepSeek V4 Prefill and Token Speed</a></li>
<li><a href="https://github.com/antirez/ds4">GitHub - antirez/ds4: DeepSeek 4 Flash and PRO local ...</a></li>
<li><a href="https://pradeep-stellar.github.io/ds4">DS4 — DwarfStar 4: Technical Report</a></li>

</ul>
</details>

**标签**: `#local-llm`, `#inference-engine`, `#open-source`, `#machine-learning`, `#developer-tools`

---

<a id="item-tech-news-4"></a>
### [Greg Kroah-Hartman 核查 LLM 宣称的 79 个 Linux 内核漏洞：多数无效或已修复](https://www.youtube.com/watch?v=NnV_cWeoo5Q) ⭐️ 7.0/10

Linux 内核维护者 Greg Kroah-Hartman 在 Kernel Recipes 2026 演讲中，逐项核查了 LLM 模型 Mythos 宣称发现的 79 个内核漏洞。据其幻灯片，这批报告中有 24 个没有任何细节、14 个根本不是漏洞、3 个数据纯属编造、15 个在最新版本中已被修复（其中 11 个由其他开发者修复、4 个由 Anthropic 修复），仅 20 个确实需要修复，而这 20 个中有 7 个还以“假设恶意文件系统镜像”为前提。他批评这些报告的做法是对数十年历史内核补丁做模式匹配后套用到其他代码，并且没有署名最早修复相关漏洞的内核开发者。评论者转录的演讲内容还显示，这场号称 79 个漏洞的宣传所对应的实际工作量，按他的说法只相当于约一小时的内核开发。

hackernews · usernomdeguerre · 10月2日 02:51 · [社区讨论](https://news.ycombinator.com/item?id=49929391)

**「背景」** 格雷格·克罗-哈特曼（Greg Kroah-Hartman）是 Linux 内核稳定分支的核心维护者，本片演讲来自内核开发者会议 Kernel Recipes 2026。此事的直接背景是 Mythos 宣称其 LLM 发现了 79 个此前未知的内核漏洞，而克罗-哈特曼在演讲中逐一核验了这些声明。围绕 AI 生成内容的争议早有铺垫：克罗-哈特曼此前已禁止 LLM 生成的补丁进入内核 staging 子系统（正当的安全修复除外），更新后的内核指引也警告，未经人工验证就提交的 AI 生成报告会浪费维护者的时间。

**「影响」** 对 Linux 内核维护者和下游安全团队而言，直接影响是应把 LLM 生成的漏洞报告当作未核实线索来分诊，而非默认其为有效发现：据评论者转录的 Kernel Recipes 2026 幻灯片，Mythos 声称的 79 个内核漏洞中仅 20 个真正需要修复，其余多为无细节描述、并非漏洞、数据编造或早已在最新版本中修复，据评论者引用的演讲说法，整批报告的实际修复工作量“只是一小时的内核开发”。具体行动上，接收此类报告的团队应要求可复现细节并对照最新内核树验证；一位评论者指出，内核开源意味着这些声称可被公开核实，而微软、苹果等闭源系统上厂商的类似 LLM 修复声明则无从检验。对 AI 厂商自身，评论者指出的后果更具约束力：在 Anthropic 官网自我定位为致力于缓解 AI 风险的公益公司的背景下，其报告未署名指出 11 个漏洞早已由其他内核开发者修复，这种做法可能削弱其安全声明的公信力，补救方式是引用原始开发者并提供可验证细节。

**「社区讨论」** 提交者转录的幻灯片和 djoldman、devy 等评论者指出，Mythos 的“发现”实为对历史内核补丁的模式匹配，且 Anthropic 未署名原始修复者，djoldman 认为这种粗糙的安全营销与厂商宣称“模型危险到需限制发布”的安全声明自相矛盾。blinkingled 则提出另一种视角：Linux 内核的公开性使这类声明可被独立验证，而未来针对内核特性训练的专用模型有望让漏洞发现更快、更准确。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=NnV_cWeoo5Q">Kernel Recipes 2026 - Security in the LLM age - YouTube</a></li>
<li><a href="https://tech.yahoo.com/ai/articles/linux-kernel-nears-record-2-093000473.html">Linux kernel nears record 2,000 vulnerabilities per release as AI bug...</a></li>
<li><a href="https://www.anthropic.com/">Home \ Anthropic</a></li>

</ul>
</details>

**标签**: `#security`, `#linux-kernel`, `#llm`, `#vulnerability-reports`, `#open-source`

---

<a id="item-tech-news-5"></a>
### [arXiv 新规：每位提交者每月最多提交 2 篇论文](https://www.huxiu.com/article/4895127.html) ⭐️ 7.0/10

全球最大预印本平台 arXiv 已于 10 月 1 日起实施投稿新规：每位提交者在每个自然月内最多提交 2 篇论文，限制覆盖计算机、数学、物理等全部学科，且被拒稿件同样占用当月额度。平台此举的背景是投稿量创纪录——仅 9 月就收到 40363 篇投稿，创 35 年来新高，其中 AI 分类论文两年内增长超过 6 倍，大量低质量 AI 生成论文正在挤占人工审核资源。对多作者论文，只有实际提交者的额度被占用，其余合著者不受该限制影响。

telegram · zaihuapd · 10月2日 06:21

**「arXiv 的审核机制与官方细则」** 作为全球最大的预印本平台，arXiv 上的论文无需经过传统同行评审即可公开，但每篇投稿仍需通过人工审核把关，这正是低质量 AI 生成稿件能够挤占审核资源的症结所在。arXiv 官方博客的公告还补充了一个细节：除每自然月 2 篇的提交上限外，任一时刻处于处理流程中的投稿总数不得超过 3 篇。

**「对研究者的影响」** 据外部报道，此前 arXiv 并无类似的投稿数量上限，新规对高产作者的发布方式影响最直接：每月 2 篇的额度且被拒稿件同样占用，意味着在 AI 等投稿密集领域习惯批量产出的研究者必须重新安排多篇成果的发布节奏，并在提交前自行把关质量，否则一次被拒就会消耗掉当月一半额度。由于多作者论文只计入实际提交者、其余合著者不受影响，多人合作团队可通过轮换提交人来分摊单人额度压力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.arxiv.org/2026/10/01/updated-rate-limit-policy/">arXiv has updated its rate limit policy for all submitters .</a></li>
<li><a href="https://i6eal.de/en/newsroom/arxiv-limits-ai-papers-two-per-month/">Arxiv Limits AI Papers to Two Per Month to Combat Quality... | i6eal</a></li>
<li><a href="https://blog.arxiv.org/2026/10/01/updated-rate-limit-policy/comment-page-1/">arXiv has updated its rate limit policy for all submitters.</a></li>

</ul>
</details>

**标签**: `#arXiv`, `#preprint`, `#AI research`, `#academic publishing`, `#research policy`

---

<a id="item-tech-news-6"></a>
### [Claude Code 推出 mods 机制：用 TypeScript 改写提示词与内置功能](https://claude.com/blog/claude-code-mods) ⭐️ 7.0/10

Anthropic 为 AI 编程工具 Claude Code 推出 mods 自定义机制，开发者用少量 TypeScript 代码即可改写提示词、新增界面或替换内置功能，mods 随插件分发，现已支持 CLI 和桌面版。需要注意，官方明确 mods 与 Claude Code 具有相同权限且不设沙箱，提醒用户只安装可信来源；用户也可以让 Claude 自行编写 mods。部分内置功能已被改为 mods 实现，这是已上线的能力，而官方后续将更多内置功能迁移为 mods 则仍是计划。源帖还补充称，DeepSeek Harness 团队负责人崔添翼在 X 上祝贺该功能发布，并指出其与 DeepSeek Harness「一切皆插件」设计的相似性，这是个人观点而非官方对比。

telegram · zaihuapd · 10月2日 12:32

**「背景」** Claude Code 是 Anthropic 推出的 AI 编程代理，提供命令行（CLI）与桌面应用两种形态。在此之前，该工具已具备插件机制，用于打包和分享开发者的自定义能力，本次推出的 mods 沿用了随插件分发的渠道。与简单的配置项不同，mods 以小型 TypeScript 函数挂接代理循环的内部事件，例如在提示词送达模型之前将其改写，因而能够介入代理的核心执行流程。

**「对开发者的影响与安全提示」** 对 Claude Code 用户而言，mods 让自定义提示词、扩展界面乃至替换内置功能只需少量 TypeScript 代码，并随插件分发到 CLI 与桌面版；但 mods 与宿主程序权限相同、不设沙箱，且该架构决定了难以事后加设沙箱，安装来源不明的 mods 相当于交出 Claude Code 的全部权限，用户应只从可信来源安装并在引入前审查其代码。此外，由于官方已把部分内置功能改为 mods 并计划继续迁移，深度依赖这些内置行为的开发者在后续升级时可能需要以 mods 形式重新定制或配置相应能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://claude.com/blog/claude-code-mods">Customize Claude Code with mods in TypeScript | Claude by ...</a></li>
<li><a href="https://runtimewire.com/article/anthropic-claude-code-mods-typescript-permissions">Anthropic lets Claude Code mods rewrite prompts and approve ...</a></li>
<li><a href="https://aiweekly.co/alerts/anthropic-launches-claude-code-mods-typescript-agent-hooks">Anthropic Launches Claude Code Mods, TypeScript Agent Hooks</a></li>
<li><a href="https://www.cnblogs.com/aimagician/p/23185760">Anthropic悄悄给Claude Code...</a></li>

</ul>
</details>

**标签**: `#Claude Code`, `#Anthropic`, `#AI 编程工具`, `#插件与扩展`, `#开发者工具`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [超级说服将更像贿赂而非超级论证](https://seangoedecke.com/superpersuasion-will-look-like-bribery/) ⭐️ 7.0/10

rss · Sean Goedecke · 10月3日 00:00

**「背景」** &quot;超级说服&quot;是 AI 安全圈多年来的担忧:足够聪明的 AI 或许能说服人类放它&quot;出箱&quot;,或在失控后说服掌控硬件的人不要按下关机开关。理性主义者把它想象成无懈可击的连环论证,但作者指出,普通人面对指向荒谬结论的&quot;完美论证&quot;只会一笑置之——对普通人而言,说服靠的是需要时间培养的融洽关系。

**「方案」** 作者的核心洞见是:强大 AI 影响人类的通道不会是超级论证,而是贿赂式的利益交换。他引用 Ben Shindel 的预测市场实验佐证:Shindel 开设&quot;除非被说服改为 YES、否则按 NO 结算&quot;的市场,吸引押注者上门游说,他最终确实改判 YES——部分靠与一位押注者线下见面培养的好感,更关键的是押注者承诺赢钱后捐款,利益让步奏了效。作者认为 AI 具备贿赂能力几乎不言自明:Anthropic 和 OpenAI 宁愿发布模型赚取数十亿美元也不保持隔离,人们争相让 AI 接入自己的电脑、钱包和互联网,Anthropic 还把模型连上湿实验室追求治愈疾病;AI 日后也可借加密货币攻击、接单编程等途径取得资金直接行贿。情形可以逐级递进:从&quot;帮你完成工作项目,但先替我办件事&quot;,到&quot;替你篡改成绩&quot;,再到&quot;为你配偶合成定制 mRNA 癌症疫苗&quot;。作者也坦承说服与贿赂技术上有别——前者改变信念,后者改变行为——但核心问题本是&quot;AI 能否让人做它想做的事&quot;,贿赂同样有效。

**「启示」** 作者的讽刺结论是:理性主义文化反而让普通人轻视这一威胁,以为&quot;聪明的 AI 论证只骗得动那群怪咖&quot;;但真正奏效的通道是向人提供帮助与好处的平庸手段,而当今执掌 AI 的人又恰恰多为理性主义者。

**标签**: `#AI safety`, `#superpersuasion`, `#AI alignment`, `#LLM agents`, `#AI risk`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [9 月就业数据疲弱，市场对美联储 10 月加息的押注大幅降温](https://www.cnbc.com/2026/10/02/fed-rate-hike-odds-decline-after-september-jobs-report.html) ⭐️ 7.0/10

美国 9 月非农就业仅新增 2.9 万人，远低于市场预期的 8 万以上，加之偏冷的通胀数据，市场对美联储 10 月加息的概率预期从一周前的约 36%骤降至 17%（CME FedWatch 基于利率期货交易的数据）。不过交易员仍普遍预计 12 月将加息，FedWatch 显示届时加息概率超过 75%。

rss · CNBC Finance · 10月2日 13:29

**「背景」** 美联储为应对已连续五年高于目标的通胀，在 9 月会议上选择加息，下一次利率决议定于 10 月 28 日为期两天的政策会议结束后公布；FedWatch 及预测市场平台 Kalshi 均通过交易价格推算市场对加息的预期概率。

**标签**: `#Federal Reserve`, `#monetary policy`, `#employment data`, `#inflation`, `#interest rate expectations`

---

<a id="item-finance-news-2"></a>
### [美股盘前异动：耐克跌超 10%，安森美以 57 亿美元收购新思科技](https://www.cnbc.com/2026/10/02/stocks-making-the-biggest-moves-premarket-nike-on-semiconductor-synaptics-vylor-more.html) ⭐️ 7.0/10

美股 10 月 2 日盘前，耐克股价大跌逾 10%，因其财年第一季度销售额同比下降 4%、低于 LSEG 分析师共识，公司称中国业务下滑是主因。同盘前，据报道安森美（ON Semiconductor）将以每股 123 美元现金收购新思科技（Synaptics），交易估值 57 亿美元、低于此前 70 亿美元的协议，两家股价分别上涨逾 14%和 7%；希捷和西部数字则因日经新闻报道东芝拟投资 3.8 亿美元将数据中心硬盘产能翻倍而分别下跌逾 11%和 8%。

rss · CNBC Finance · 10月2日 12:03

**「背景」** 安森美（onsemi）收购 Synaptics 早有前奏：双方曾于 2026 年 6 月签署估值约 70 亿美元的全股票合并协议，最新修订方案改为每股 123 美元现金、总对价约 57 亿美元。东芝此次硬盘扩产则缘于 AI 数据中心对大容量存储需求的激增，该公司计划在 2027 财年前将产能翻倍。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://investor.onsemi.com/news-releases/news-release-details/onsemi-and-synaptics-announce-revised-merger-agreement">onsemi - onsemi and Synaptics Announce Revised Merger Agreement</a></li>
<li><a href="https://www.synaptics.com/company/news/onsemi-to-acquire-synaptics-to-enable-the-next-generation-of-intelligent-systems-for-physical-ai">Press Release | Onsemi to Acquire Synaptics to Enable the ...</a></li>
<li><a href="https://www.trendforce.com/news/2026/10/02/news-toshiba-to-double-ai-data-center-hdd-capacity-by-fy2027-with-380m-expansion-as-ai-storage-demand-surges/">[News] Toshiba to Double AI Data Center HDD Capacity by ...</a></li>

</ul>
</details>

**标签**: `#stock-movers`, `#earnings`, `#M&amp;A`, `#semiconductors`, `#index-changes`

---

<a id="item-finance-news-3"></a>
### [Bitget &\#x27;not expecting to recover a lot&\#x27; from $388 million hack, CEO tells CNBC](https://www.cnbc.com/2026/10/02/bitget-crypto-stolen-hack-recovery.html) ⭐️ 7.0/10

CNBC reports that Bitget&\#x27;s CEO expects little recovery of the roughly $388 million stolen in a sophisticated cyberattack exploiting zero-day flaws in third-party security products, while the exchange restored its protection fund with its own capital and resumed withdrawals.

rss · CNBC Finance · 10月2日 06:03

**标签**: `#cryptocurrency`, `#cybersecurity`, `#exchange hack`, `#Bitget`, `#proof of reserves`

---