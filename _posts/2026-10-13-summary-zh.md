---
layout: default
title: "Horizon Summary: 2026-10-13 (ZH)"
date: 2026-10-13
lang: zh
---

> 从 42 条内容中筛选出 12 条重要资讯。

---

**科技新闻**
1. [黑客利用联网制冷控制器远程触发欧洲超市冷柜除霜](#item-tech-news-1) ⭐️ 8.0/10
2. [开源项目把 WiFi 7 路由器改造成 320 Msps 软件无线电接收器](#item-tech-news-2) ⭐️ 8.0/10
3. [Python 3.15 发布：PEP 810 显式惰性导入与 Tachyon 采样分析器](#item-tech-news-3) ⭐️ 8.0/10
4. [用 C 语言构建现代 Web 应用：安全加固与部署实录](#item-tech-news-4) ⭐️ 7.0/10
5. [Codex CLI 默认安装自更新后台守护进程，社区找出隐藏开关](#item-tech-news-5) ⭐️ 7.0/10
6. [Meta 发布新模型 Muse Wonder，实测表现与隐私问题遭质疑](#item-tech-news-6) ⭐️ 7.0/10
7. [Looped Diffusion Transformer 开源：去噪步骤内循环复用模块，深度采样时可调](#item-tech-news-7) ⭐️ 7.0/10
8. [learnc 开源工具自动拟合 C 代码常量：JPEG 体积缩小 9.1%、VAD F1 提升](#item-tech-news-8) ⭐️ 7.0/10

**财经新闻**
1. [美联储哈马克：或需进一步加息，防止通胀心态固化](#item-finance-news-1) ⭐️ 7.0/10
2. [中欧就混动与电动汽车贸易达成共识，中方配额不低于其他来源](#item-finance-news-2) ⭐️ 7.0/10
3. [新能源汽车出口退税率下调至 9%，2027 年 4 月起实施](#item-finance-news-3) ⭐️ 7.0/10
4. [税务行政处罚新裁量基准 11 月起施行，社保欠缴最高罚 3 倍](#item-finance-news-4) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [黑客利用联网制冷控制器远程触发欧洲超市冷柜除霜](https://www.tomshardware.com/tech-industry/cyber-security/unprecedented-cyberattack-cripples-supermarket-fridges-across-europe-as-hackers-activate-automatic-defrosting-delivery-and-store-prices-also-impacted-by-incident) ⭐️ 8.0/10

据 Tom&\#x27;s Hardware 援引路透社、BBC 与《世界报》的报道，黑客利用联网的商业制冷控制器在欧洲多家超市远程强制启动自动除霜程序，造成食品腐损，法国连锁超市 Intermarché称约 150 家门店成为攻击目标，配送和门店价格也受到影响。报道关联的 Claroty Team82 研究此前曾披露 Danfoss 制冷控制器中的漏洞，社区评论进一步指出涉案设备疑似包括已停止安全支持的 Danfoss SM800（2021 年终止支持）和 SC355（2016 年终止支持）等老旧型号。目前公开信息仍以受影响超市和媒体的通报为主，攻击者的具体入侵路径与身份尚无独立证实。

hackernews · Zeekaas · 10月12日 12:16 · [社区讨论](https://news.ycombinator.com/item?id=50055304)

**「背景」** 这类联网制冷控制器的安全隐患此前已有公开记录：安全研究团队 Claroty Team82 曾在 Danfoss AK-SM800A 平台上发现三个漏洞，其中一个隐藏的“当日口令”（code-of-the-day）认证机制可被滥用以绕过标准登录控制，进而实现远程代码执行。Danfoss 随后为 AK-SM8xxA 系列冷藏控制器发布了新固件，修复了 Team82 披露的这一认证绕过漏洞。据报道，本次欧洲超市攻击针对的正是此类存在已知漏洞的老旧 Danfoss 制冷控制器。

**「影响：客户数据泄露与遗留控制器联网风险」** 对消费者而言，最直接的后续影响是数据安全：同一轮针对 Intermarché的网络攻击还窃取了近 30 万名客户的个人信息，相关方面呼吁这些客户在未来数周内对网络钓鱼等在线风险保持警惕。对仍联网运行老旧制冷控制器的商超与设施运营方而言，事件暴露出一个具体的兼容性隐患：社区讨论将疑似被利用的设备指向 Danfoss SM800（2021 年停止支持）、SC355（2016 年停止支持）等旧型号控制器，而本次事件证明此类可远程访问的设备确实能被攻击者用来直接操纵制冷硬件，运营方需要尽快审查这类系统的互联网暴露面并评估补丁或更换安排。

**「社区讨论」** 评论中讨论最多的是商用冷柜为何会接入互联网：有人引用 Danfoss 官方材料指出远程诊断和控制可为多门店运营节省上门维护成本，也有人举例称部分新式商用设备甚至依赖付费订阅才能运行，即联网是厂商强加的商业模式而非用户选择；另有评论者认为，运营 15-20 年老旧控制器的基层维护方既没有预算做安全审查，也没有余裕定期更换设备。还有评论者猜测本次事件可能与 2026 年 8 月美国军事基地食品超市冷柜遭类似攻击的事件相关，但这一关联目前仅为推测。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/claroty_team82-activity-7330549882962735105-h-MB">Danfoss fixes AK-SM8xxA Series cooler controllers vulnerability</a></li>
<li><a href="https://safetynews.au/story/refrigeration-controller-flaws-threaten-cold-chains">Refrigeration controller flaws threaten cold chains</a></li>
<li><a href="https://www.connexionfrance.com/news/intermarche-cyberattack-affects-nearly-300000-customers/806317">Intermarché cyberattack 2026 : Nearly 300,000 customers&#x27; data stolen...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#OT security`, `#IoT`, `#critical infrastructure`, `#legacy systems`

---

<a id="item-tech-news-2"></a>
### [开源项目把 WiFi 7 路由器改造成 320 Msps 软件无线电接收器](https://github.com/h0m3us3r/w1700k-sdr) ⭐️ 8.0/10

开源项目 w1700k-sdr（作者 h0m3us3r）演示了如何将 WiFi 7 路由器的芯片组改造成采样率高达 320 Msps 的软件定义无线电（SDR）接收器，用于 5 GHz 频段的宽带射频接收。这种带宽的接收能力此前通常需要价格高昂的专用 SDR 硬件，该项目提供了一个极为廉价的路径，但它是需要用户自己动手改装的开源方案，而非开箱即用的产品。该项目于 10 月 12 日经 Hacker News 传播（282 分、74 条评论），有射频领域评论者表示，想不出更便宜的办法在 5 GHz 频段获得 320 Msps 的接收能力。

hackernews · djfergus · 10月12日 12:41 · [社区讨论](https://news.ycombinator.com/item?id=50055593)

**「背景：Wi-Fi 7 芯片为何能充当宽带 SDR」** 软件定义无线电（SDR）以高速采样加软件处理取代专用射频电路，而能覆盖 5 GHz 频段、采样率达数百 Msps 的宽带接收机此前通常依赖昂贵的专业仪器。现代 Wi-Fi 路由器的射频芯片本身就是宽带收发器——此次被改造的 Gemtek W1700K 即内置联发科 MT7996 芯片，能以最高 320 Msps 采集 14 位原始 IQ 数据，再由 Airoha AN7581 SoC 经 10 GbE 输出——这正是它能被改造成 SDR 接收机的硬件基础。据 Hacker News 上的评论者介绍，同一作者此前还曾把 ESP32 Wi-Fi 微控制器改造成 SDR（eSpDR 项目），本项工作可视为同一思路向更强硬件的延伸。

**「对预算型 SDR 用户的实际影响」** 对预算有限的软件无线电（SDR）爱好者和射频实验者而言，这切实降低了 5 GHz 频段宽带接收的门槛：以往实现 320 Msps 级别的宽带数字化接收通常依赖昂贵的专用 SDR 硬件，而该项目证明一台量产 WiFi 7 路由器即可胜任，且整套方案在 GitHub 上开源，愿意动手的用户可以按仓库指引复现。需要注意的是它只提供接收功能，且要求设备使用项目所支持的那款 WiFi 7 芯片组——有社区用户猜测搭载同款芯片并内置 PCIe（可装 NVMe）的 Banana Pi R4 应该也能运行，但这一说法尚未经项目作者验证。

**「社区讨论」** 评论者 aftbit 表示自己不知道还有更便宜的途径在 5 GHz 获得 320 Msps 接收能力；一位有服务监测仪维修经验的用户 mikewarot 称赞该方案令人惊叹，并建议在此基础上加装衰减器、5 GHz 低通滤波器和上/下变频器来搭建类似射频监测仪的设备。另有评论者 yonatan8070 指出同一开发者此前还用 ESP32 微控制器做过 SDR（eSpDR 项目），希望这类方法能扩展到普通笔记本的 WiFi 网卡；thebeardisred 则推测由于芯片组相同，带 NVMe PCIe 接口的 Banana Pi R4 路由器应该也能运行该项目——这些均为个人观点与推测，尚未经过独立验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/h0m3us3r/w1700k-sdr">GitHub - h0m3us3r/w1700k-sdr</a></li>
<li><a href="https://hackaday.com/2026/10/12/wifi-router-does-software-defined-radio/">WiFi Router Does Software-Defined Radio | Hackaday</a></li>

</ul>
</details>

**标签**: `#software-defined-radio`, `#hardware-hacking`, `#wifi-7`, `#rf`, `#open-source`

---

<a id="item-tech-news-3"></a>
### [Python 3.15 发布：PEP 810 显式惰性导入与 Tachyon 采样分析器](https://simonwillison.net/2026/Oct/12/python-3-15/) ⭐️ 8.0/10

Python 3.15 正式发布，官方下载页面与由 3.14 和 3.15 发布经理 Hugo van Kemenade 整理的《What&\#x27;s new in Python 3.15》指南均已上线。最受关注的新特性是 PEP 810 引入的显式惰性导入：通过 lazy import  或 lazy from pathlib import Path 这样的语法，模块会在后续代码首次使用其符号时才真正加载；Simon Willison 指出这直接解决了他的 LLM CLI 工具的痛点——此前插件文档只能建议手动惰性导入，因为安装使用 sentence\_transformers 等重依赖的插件会给每次 llm 命令调用增加数秒启动时间。其他亮点包括 PEP 798 的推导式解包语法（例如 \[\*sublist for sublist in lists\]），以及标准库新增的 Tachyon 采样分析器（profiling.sampling），它可以通过 PID 附加到运行中的进程收集栈样本并生成火焰图，原有 cProfile 则更名为 profiling.tracing。性能方面，Miguel Grinberg 基于 3.15.0rc3 的测试显示 3.15 与 3.14 基本持平，仅实验性 JIT 在斐波那契测试中比标准解释器快 1.2 倍，这是他首次观察到 JIT 带来明显提升；对需要兼容所有受支持版本的开源维护者而言，这次发布意味着可以放弃 Python 3.10 支持，并开始采用 3.11 的特性。

rss · Simon Willison · 10月12日 18:15

**「背景」** Python 每年推出一个大版本，而 Willison 维护着需要兼容所有受支持 Python 版本的开源项目，因此每次新版本发布都意味着放弃最旧的版本——这次是 Python 3.10——并把代码下限抬到能用上 3.11 特性的水平。惰性导入改变的是 Python 默认在 import 语句执行时立即加载模块的行为；此前 Willison 只能在 LLM CLI 的插件文档中建议作者手动惰性加载昂贵依赖，因为安装使用 sentence\_transformers 这类重型依赖的插件曾让每次 llm 命令调用多耗时数秒。在新分析器出现之前，标准库只自带 cProfile 这类基于追踪的工具，低开销的采样式性能分析一直要依赖 py-spy 等第三方方案。

**「对维护者的实际影响」** 按照五年的支持周期，Python 3.10 已于 2026 年 10 月 1 日停止接收包括安全修复在内的所有更新，因此维护覆盖所有受支持版本开源库的开发者现在可以从支持矩阵中移除 3.10，并开始采用 Python 3.11 的语言特性；仍在生产环境中运行 3.10 的团队则应尽快升级，以免错失后续安全补丁。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://endoflife.ai/article-python-310-eol">Python 3.10 End of Life: October 2026, When Security Fixes Stop</a></li>
<li><a href="https://end-of-life.org/python/3.10/">Python 3.10 End of Life – end-of-life.org</a></li>

</ul>
</details>

**标签**: `#python`, `#language-features`, `#lazy-imports`, `#pep-810`, `#open-source`

---

<a id="item-tech-news-4"></a>
### [用 C 语言构建现代 Web 应用：安全加固与部署实录](https://prophitt.me/writing/a-modern-web-app-in-c) ⭐️ 7.0/10

开发者 prophittcorey 在个人博客发布长文，完整记录了用 C 语言构建一个现代 Web 应用的过程，重点覆盖部署与安全加固实践，包括借助 pledge、chroot 等机制进行权限降级。文章在 Hacker News 上引发较大反响，获得 426 分和 175 条评论。这不是新框架或工具的发布，而是一篇面向对系统级 Web 开封感兴趣工程师的技术深度分享，展示了相对于主流 Web 技术栈的一种非主流但论证充分的替代思路。

hackernews · prophittcorey · 10月12日 16:13 · [社区讨论](https://news.ycombinator.com/item?id=50058528)

**「背景」** 这类项目依托的 CGI 是 Web 开发的早期模式：Web 服务器（如 nginx）在每次请求到达时启动一个独立的可执行程序来生成响应，而非让后端进程常驻；评论区多位开发者回忆，二十多年前用 Perl 或 C 编写 CGI 十分常见，后来的 FastCGI 则让程序以常驻方式运行，以减少每请求反复启动的开销。另一个前提是 pledge 与 chroot 等沙箱机制（pledge 源自 OpenBSD）：通过限制进程可调用的系统调用和可见的文件系统范围来收缩权限，为缺乏内存安全保障的 C 程序划定更小的受攻击面。

**「影响」** 对维护小型自托管服务或内部工具的工程师而言，这篇文章提供了一个用 C 语言实现、并依赖操作系统级隔离（pledge、chroot）来弥补内存安全短板的可参考案例。有意效仿的团队需要注意 pledge 是 OpenBSD 的系统调用，需确认目标平台对相应沙箱机制的支持情况，并自行承担 C 代码安全加固的责任。

**「社区讨论」** 评论者对这一做法看法分化：ramses0 认可文中论证并补充称 busybox 内置了 cgi-bin 支持，assimpleaspossi 分享了自己 22 年前用 C 和 FastCGI 为餐厅构建在线订餐系统并长期稳定运行的亲身经历；而 brainless 则表示不认同 nginx 每个请求都调用一次二进制的模型，他的产品后端选择 Rust 与 SQLite 配合框架并保持常驻状态。这些均为个人经验与偏好，并非对文中方案的客观评测。

**标签**: `#C`, `#web-development`, `#systems-programming`, `#security`, `#technical-deep-dive`

---

<a id="item-tech-news-5"></a>
### [Codex CLI 默认安装自更新后台守护进程，社区找出隐藏开关](https://github.com/openai/codex/issues/48195) ⭐️ 7.0/10

OpenAI 的 Codex CLI 默认会安装一个常驻且自动更新的后台守护进程，官方文档没有提供关闭选项，这一行为在 Hacker News 上引发了 488 分、248 条评论的讨论。社区成员发现，可在 ~/.codex/config.toml 的 \[features\] 段中设置 daemon\_auto\_start = false 来禁用它；另一个变通方法是删除守护进程启动时写入 ~/.codex 的 pid 和锁文件，将其替换为指向 /dev/null 的符号链接并用 chattr +i 锁定。用户还报告了实际影响：有人发现累积的旧版本占用约 12GB 磁盘空间，另有用户称自动更新会随机破坏仓库权限、使 .git 变为只读并阻塞任务执行。以上均来自用户报告，来源中未见 OpenAI 的官方回应。

hackernews · whimblepop · 10月12日 18:29 · [社区讨论](https://news.ycombinator.com/item?id=50060694)

**「背景」** 守护进程自动启动并非此次才出现：据 2026 年 9 月 25 日的发布说明，自 Codex CLI v0.157.0 起，仅打开一个交互式 codex 会话就会启动持久后台守护进程（codex app-server --managed-daemon），并被设为稳定版默认行为，企业等有严格进程隔离策略的部署需自行显式关闭。同日有用户在 GitHub 上提交 issue（\#48195），要求将 daemon\_auto\_start 改为默认关闭、需主动开启的功能，或至少在启用前询问一次。后续报道补充称，该守护进程每小时自我更新一次，且可能中断正在运行的 agent 任务，这些行为正是当前社区不满的直接前因。

**「对开发者的实际影响」** 通过 npm 全局安装 Codex CLI（受影响版本如 0.157.0）的开发者会在不知情的情况下运行一个持续自更新的后台守护进程。有用户报告旧版本累积占用约 12GB 磁盘空间，另有用户称自动更新会随机破坏仓库权限（.git 目录变为只读），导致任务数小时被阻塞。受影响用户目前可在 ~/.codex/config.toml 中设置 \[features\] daemon\_auto\_start = false 来关闭该行为，但这一配置项未被官方文档记录，后续版本可能变更或失效；也有用户采用删除 ~/.codex 下 pid 与锁文件、替换为指向 /dev/null 的符号链接并用 chattr +i 锁定的临时规避手段。已有用户在 GitHub 提交请求，要求将 daemon\_auto\_start 改为默认关闭或安装时征询用户同意。

**「社区讨论」** 有评论者认为，一个通过 NPM 安装的 CLI 默认运行自更新守护进程尤其令人警惕，而 whimblepop 分享的配置开关与文件系统级变通方案是帖子中最实用的内容。对工具质量的评价分歧明显：icantevenhold 称约 12GB 的磁盘占用“似乎很疯狂”并认为 Codex 在各项指标上都比 Claude Code 更糟；dllu 报告守护进程 bug 使任务每几小时被阻塞一次，令其无法信任 Codex 执行目标；reacharavindh 则改用仅依赖 bash 的极简 harness 来避开这类复杂工具链。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://codex.danielvaughan.com/2026/09/25/codex-cli-daemon-auto-start-stable-default-v0157/">Daemon Auto-Start Is Now the Stable Default in Codex CLI v0 ...</a></li>
<li><a href="https://github.com/openai/codex/issues/48195">CLI: make `daemon_auto_start` opt-in — a persistent, self ...</a></li>
<li><a href="https://elsolitario.org/en/2026/10/12/codex-cli-daemon-auto-start-opt-in-en/">Codex CLI Daemon: Why Users Want It Opt-In - elsolitario.org</a></li>
<li><a href="https://github.com/openai/codex/issues/48195">CLI : make ` daemon _auto_start` opt-in — a persistent, self-updating...</a></li>

</ul>
</details>

**标签**: `#openai`, `#codex-cli`, `#developer-tools`, `#ai-coding-assistants`, `#software-supply-chain`

---

<a id="item-tech-news-6"></a>
### [Meta 发布新模型 Muse Wonder，实测表现与隐私问题遭质疑](https://research.meta.ai/blog/muse-wonder) ⭐️ 7.0/10

Meta 研究部门于 2026 年 10 月 12 日宣布了新的 AI 模型 Muse Wonder，并通过 dev.meta.ai 上的配套 Muse Code 开发者页面向公众开放试用。该发布在 Hacker News 上引发高热度讨论（551 分、304 条评论），但现有材料未包含公告本身的技术细节，模型规格、基准方法与可用范围均无法核实。评论区的上手测试显示，实际表现与其强劲的基准分数存在落差：一项图像转 HTML 对比测试中，Muse Wonder（high）明显逊于 Opus 5.5，更接近中端 Claude 模型的水平，测试者推测其视觉模型可能是短板。另有用户报告，在 Muse Code 页面用 Meta 账号登录时，登录认证环节出现了陌生他人的个人资料，疑似邮箱与账号资料被暴露给其他用户，且账号设置无法访问、不断收到登录通知——该问题目前仅为用户报告，尚未得到证实。

hackernews · meetpateltech · 10月12日 16:48 · [社区讨论](https://news.ycombinator.com/item?id=50059115)

**「背景」** Meta 过去一段时间在前沿模型上被认为落后于 Anthropic 与 OpenAI 的顶级产品，第三方评测方指出这是 Meta 近来首款据称真正具备与两家头部模型竞争实力的模型。此次发布的 Muse Wonder 系列包含 Muse Wonder 与 Muse Wonder Full 两款，是 Meta 迄今能力最强的模型，官方宣称其面向个人与专业智能体任务，并在智能体、记忆和编程等关键基准上达到业界最优（state-of-the-art）水平。

**「对开发者的影响」** 考虑试用或接入 Muse Wonder 的开发者应先在自己的真实任务上验证模型表现，而非直接采信基准分数：社区用户 jjcm 的图像转 HTML 实测发现其输出质量更接近中端档位的 Claude（Sonnet/Haiku），明显逊于 Opus 5.5，与其亮眼的基准成绩存在落差。此外，用户 pmuse 报告在通过 Muse Code 站点登录 Meta 账号时，认证流程中出现了陌生他人的账户资料，且账号设置无法访问；由于该问题尚未获 Meta 官方确认，在澄清之前开发者应谨慎在该平台登录或绑定账号。Muse Code 与 Muse Spark 目前通过 Meta Model API 开发者门户（dev.meta.ai）提供。

**「社区讨论」** 观点方面，一位评论者认为越多的公司接近前沿越好，可以避免单家公司在递归自我改进时代垄断权力并将其价值观强加于全行业，尽管他本人对 Meta 颇有不满。另一位以模型对比著称的用户则沿用其标志性的“鹈鹕”绘图测试，将 Muse Wonder 与 8 月的 Muse Spark 1.2、9 月的 Muse 1.3 放在一起比较，并指出 1.3 似乎喜欢给鹈鹕加动画。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://research.meta.ai/blog/muse-wonder">Muse Wonder | Meta AI Research</a></li>
<li><a href="https://about.fb.com/news/2026/10/introducing-muse-wonder-models/">Introducing Muse Wonder and Muse Wonder Full: Frontier Models ...</a></li>
<li><a href="https://www.agent-one.dev/blog/muse-wonder">Meta Muse Wonder: Benchmarks, Pricing, API, and How to Use It</a></li>
<li><a href="https://dev.meta.ai/">Meta Model API Developer Portal</a></li>

</ul>
</details>

**标签**: `#artificial-intelligence`, `#meta`, `#large-language-models`, `#benchmarking`, `#model-release`

---

<a id="item-tech-news-7"></a>
### [Looped Diffusion Transformer 开源：去噪步骤内循环复用模块，深度采样时可调](https://www.reddit.com/r/MachineLearning/comments/1x49d61/looped_diffusion_transformer_the_same_blocks_run/) ⭐️ 7.0/10

Looped Diffusion Transformer（论文 arXiv 2609.40305，9 月 30 日）不再把文生图 DiT 做大，而是让同一组共享的 transformer 模块在每个去噪步骤内运行多次；论文指出朴素的循环并不可靠，需配合每次循环上的深监督（deep supervision）与自调制注意力（self-modulating attention）才能生效。其头条结论称，260M 参数的循环模型在多个基准上以约 4.9 倍更少的推理计算击败了 6.5 倍大的模型，且在固定推理预算下增加循环深度比增加去噪步数更有帮助——这些数字仍属作者自报，未经独立验证。B/16 的代码与权重以 MIT 许可发布，权重托管在 Hugging Face 的 sensenova 组织下；模型按深度 4 训练，README 称其他深度无需重新训练即可使用。发帖者在 M5 Pro 上（PyTorch MPS、fp32、100 步 Euler、CFG 6.0、每个提示复用同一随机种子）对深度 1 至 4 做了实测：绝大多数画质变化发生在深度 3 之前，深度 3 与 4 在各提示下输出非常接近；单张图耗时从约 23 至 24 秒（深度 1）升至 43 至 47 秒（深度 4）。

reddit · r/MachineLearning · /u/Fit-Ant2238 · 10月12日 18:13

**「背景」** 在典型的文本到图像扩散变压器（DiT）中，每个去噪步骤对应网络的一次完整前向传播，想提升质量通常要把模型本身做得更大。这项工作沿用的概念先例是&quot;循环深度&quot;（looped / recurrent-depth）语言模型：让同一组权重块反复迭代，且迭代次数到采样阶段才选定，从而在单张图像上按需用算力换取精修程度。据 Hugging Face 论文页与 arXiv 摘要页，该论文以编号 2609.40305 于 9 月 30 日发布，归属计算机视觉与机器学习类目。

**「影响」** 从事文生图或高效推理的开发者现在可以直接下载 MIT 许可的 B/16 代码与权重，在不重新训练的情况下于采样阶段调整循环深度，按需交换计算量与单图精细度；但发帖者的初步实测提示画质收益在深度 3 左右趋于饱和，且深度 4 的耗时约为深度 1 的两倍，因此实际使用时从较低深度试起可能更划算。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/papers/2609.40305">Paper page - Looped Diffusion Transformer</a></li>
<li><a href="https://arxiv.org/abs/2609.40305">[ 2609 . 40305 ] Looped Diffusion Transformer</a></li>

</ul>
</details>

**标签**: `#diffusion-models`, `#transformers`, `#efficient-inference`, `#text-to-image`, `#open-source`

---

<a id="item-tech-news-8"></a>
### [learnc 开源工具自动拟合 C 代码常量：JPEG 体积缩小 9.1%、VAD F1 提升](https://www.reddit.com/r/MachineLearning/comments/1x4dlbm/learnc_fit_the_constants_in_existing_c_code_to/) ⭐️ 7.0/10

开源工具 learnc 能在不改动 C 代码结构的前提下，按用户用 C 编写的评分函数自动调整代码中的具名常量，并把新值直接写回原文件。作者在留出数据上报告了两项结果：为 stb\_image\_write.h 调优 128 个 JPEG 量化表条目（在 12 张 Kodak 图上调参、另 12 张测试）后，等 SSIM 下 BD-rate 改善 9.1%，帖子称该结果已在 libjpeg 中用 scikit-image 独立复现，比 mozjpeg 的量化表再优 2.7%；对 Google WebRTC VAD 的 vad\_core.c 中全部常量调优后，F1 在 LibriParty eval 上从 0.810 升至 0.859。作者同时说明局限：JPEG 在低于 1 bpp 时没有收益，该方法适合数十到数百个常量的规模，不适合大型权重集合。代码以 MIT 许可发布在 GitHub（devanmolsharma/learnc），其中 VAD 结果仍属自报，有待社区复现。

reddit · r/MachineLearning · /u/keep\_up\_sharma · 10月12日 20:51

**「背景：JPEG 量化表与 mozjpeg 基线」** JPEG 编码通过 8×8 量化表控制码率与失真的权衡：标准实现沿用统一、预定义的量化表，而率失真优化等做法会针对图像内容定制量化矩阵的各个系数，这些系数正是以魔数常量形式写死在代码中的。Mozilla 的 mozjpeg 是 libjpeg-turbo 的补丁项目，通过 trellis 量化和重新调校的量化表预设来同时提升画质与压缩率，并与 JPEG 标准及绝大多数已部署解码器保持兼容，因此常被用作量化表优化的强基线。learnc 的另一个测试对象 Google WebRTC VAD 则是在 vad\_core.c 中以一组手工常量判断语音与静音的模块。

**「实际影响」** 维护内嵌调优常量的 C 项目（如图像编码器、语音检测等信号处理代码）的开发者，可以在不重写代码的情况下用自定义指标搜索更优常量值；前提是能写出可编译的评分函数，并应在留出数据上自行复核结果，且按作者说明低于 1 bpp 的 JPEG 场景不会获益。代码已以 MIT 许可在 GitHub 公开，可直接下载验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://salivity.github.io/jpeg/article/rate-distortion-optimization-in-jpeg-quantization">Rate-Distortion Optimization in JPEG Quantization - jpeg</a></li>
<li><a href="https://github.com/mozilla/mozjpeg">GitHub - mozilla/mozjpeg: Improved JPEG encoder. DCT and Quantization | mozilla/mozjpeg | DeepWiki JPEG Quantization Tables Explained: Why Quality 80 Isn&#x27;t ... Quantization Tables in JPEG Digital Forensics - jpeg Rate–distortion optimal evolutionary algorithm for JPEG ... Quantization Table Redesign for the JPEG Compression ...</a></li>

</ul>
</details>

**标签**: `#autotuning`, `#C programming`, `#image compression`, `#voice activity detection`, `#open source tools`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [美联储哈马克：或需进一步加息，防止通胀心态固化](https://www.cnbc.com/2026/10/12/beth-hammack-fed-inflation-policy.html) ⭐️ 7.0/10

美联储上月刚进行三年来首次加息，克利夫兰联储主席、FOMC 投票委员哈马克（Beth Hammack）周一表示，为使通胀及时回归 2%目标，适宜维持限制性货币政策立场，并倾向“较快进行小幅调整”，暗示可能进一步加息。最新数据显示，美国 8 月 PCE 物价指数同比上涨 3.4%，剔除食品和能源的核心 PCE 同比上涨 3%，均高于 2%的目标。

rss · CNBC Finance · 10月13日 02:58

**「背景」** 美联储已于 2026 年 9 月将政策利率上调至 3.75%至 4.00%区间，为三年来首次加息，而美国通胀已连续逾五年高于央行 2%的目标。哈马克是 2026 年轮换后新增的 FOMC 投票成员之一，政策立场偏向收紧（即倾向于通过更高利率抑制通胀）。

**「影响」** 交易员目前对美联储 12 月加息的定价接近 88%（CME FedWatch 数据）；若进一步加息，背负房贷和贷款的家庭与企业将面临更高的借贷成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.plus500.com/en-sz/newsandmarketinsights/understanding-fed-dissents-what-could-a-divided-fed-mean">Fed Dissents Explained: Navigating a Divided FOMC | Plus500</a></li>
<li><a href="https://www.usbank.com/investing/financial-perspectives/market-news/federal-reserve-interest-rate.html">Fed raises rates to 3.75%-4.00%, first hike since 2023 | U.S ...</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#monetary policy`, `#interest rates`, `#inflation`, `#Beth Hammack`

---

<a id="item-finance-news-2"></a>
### [中欧就混动与电动汽车贸易达成共识，中方配额不低于其他来源](https://www.mofcom.gov.cn/xwfb/sjfzrfb/art/2026/art_4d502e1d49fd4480b39a6cfd0d752038.html) ⭐️ 7.0/10

中国商务部宣布，中欧在贸易投资磋商机制下就混合动力汽车和电动汽车贸易达成多项共识，其中中方企业获得的配额待遇将不低于欧盟其他进口来源地。混动汽车安排以 2025 年为基准向上调整，以兼顾中方企业出口空间，欧方并将继续推进中国企业价格承诺及其他复审程序；中方保留在世贸组织框架下的争端解决权利。

telegram · zaihuapd · 10月12日 06:19

**「背景」** 此前欧盟对中国产电动汽车征收反补贴税且相关关税并未取消，双方长期以&quot;价格承诺&quot;（企业承诺出口价不低于约定下限，以换取豁免）作为解决途径（tool-1-2；tool-1-3）。就在数日前，欧盟贸易专员曾表示中方同意将混动车对欧出口减半，双方并商定于明年 1 月举行部长级视频会议（tool-1-1）。

**「对欧出口中国车企直接受益」** 对欧出口混动和电动汽车的中国车企将直接受益：混动车出口安排以 2025 年为基点向上、配额享受不低于欧方其他进口来源的非歧视待遇，且欧方继续推进价格承诺复审，为企业出口规模和成本提供更可预期的条件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.zaobao.com.sg/news/china/story20261009-9813146">欧 盟 贸 易 专员： 中 国同意将 混 动 汽 车 对 欧 出口减半 | 联合早报</a></li>
<li><a href="https://www.21jingji.com/article/20241107/herald/91f8e13f10d2180221ee70c3d8dd61bd.html">21jingji.com/article/20241107/herald/91f8e13f10d2180221ee70c3d8dd...</a></li>
<li><a href="https://post.smzdm.com/p/anv9okk0/">post.smzdm.com/p/anv9okk0</a></li>
<li><a href="https://www.chinaautosupplier.com/show_article-87647.html">chinaautosupplier.com/show_article-87647.html</a></li>
<li><a href="http://www.evobserver.com/archives/23691">evobserver.com/archives/23691</a></li>

</ul>
</details>

**标签**: `#China-EU trade`, `#electric vehicles`, `#trade policy`, `#automotive industry`, `#Ministry of Commerce`

---

<a id="item-finance-news-3"></a>
### [新能源汽车出口退税率下调至 9%，2027 年 4 月起实施](https://www.news.cn/20261012/9709731f470b42f9a84825c2e4eb914b/c.html) ⭐️ 7.0/10

财政部、税务总局 10 月 12 日发布公告，自 2027 年 4 月 1 日起，将新能源汽车增值税出口退税率由 13%下调至 9%，同时取消电子烟设备装置等产品的增值税出口退税。

telegram · zaihuapd · 10月12日 11:00

**「背景」** 出口退税是指国家把出口商品在国内环节已缴纳的增值税退还给出口企业，退税率下调意味着企业出口时自行承担的税负增加。此前中国长期以财税优惠扶持新能源汽车，例如 2020 年的稳定和扩大汽车消费措施曾将免征车辆购置税政策延续至 2022 年底。

**「影响」** 向海外出口新能源汽车的车企可获得的退税将减少，若无法通过提高售价转嫁，出口成本上升会压缩其利润空间。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.gov.cn/zhengce/zhengceku/2020-05/03/content_5508575.htm">关于稳定和扩大 汽 车 消费若干措施的通知_ 国 务 院 部 门文件_ 中 国 政 府网</a></li>

</ul>
</details>

**标签**: `#fiscal policy`, `#export tax rebate`, `#new energy vehicles`, `#China`, `#trade`

---

<a id="item-finance-news-4"></a>
### [税务行政处罚新裁量基准 11 月起施行，社保欠缴最高罚 3 倍](https://fgk.chinatax.gov.cn/zcfgk/c100012/c5252754/content.html) ⭐️ 7.0/10

国家税务总局发布 2026 年第 20 号公告，推出《全国税务行政处罚裁量基准（2026 年版）》，自 2026 年 11 月 1 日起施行，首次将用人单位逾期不缴或少缴社保费纳入处罚事项，按欠缴金额和占比分档，经责令限期缴纳后仍不缴的最高可处欠缴金额 3 倍罚款，同时须补缴欠费并按日加收万分之五滞纳金；基准施行前的违法行为原则上适用当时规定，且该基准本身不能单独作为处罚依据。

telegram · zaihuapd · 10月13日 02:45

**「背景」** 行政处罚裁量基准是行政机关依据《行政处罚法》制定并向社会公布的执法尺度，用来统一同类违法行为在处罚轻重上的选择空间。此前部分地区已先后统一了各自区域内的执行标准，国家税务总局也于 2026 年 7 月就这一全国版基准公开征求意见。

**「谁受影响」** 2026 年 11 月 1 日起，全国各类用人单位若经责令限期缴纳后仍不缴或少缴社保费，除须补缴欠费并按日加收万分之五滞纳金外，还可能被处最高欠缴金额 3 倍的罚款，按时足额缴费的企业则不受该处罚条款约束。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://paper.people.com.cn/rmrb/pc/attachement/202607/18/0378ed27-fe07-41dc-95b0-b5fb063d3b93.pdf">paper.people.com.cn/rmrb/pc/attachement/202607/18/0378ed27-fe07...</a></li>
<li><a href="https://npcobserver.com/wp-content/uploads/2023/09/2021-Administrative-Punishments-Law-Revision_Gazette.pdf">npcobserver.com/wp-content/uploads/2023/09/2021-Administrative...</a></li>

</ul>
</details>

**标签**: `#税务处罚`, `#社保欠缴`, `#政策监管`, `#企业合规`, `#中国税务`

---