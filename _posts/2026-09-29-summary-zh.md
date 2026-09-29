---
layout: default
title: "Horizon Summary: 2026-09-29 (ZH)"
date: 2026-09-29
lang: zh
---

> 从 43 条内容中筛选出 12 条重要资讯。

---

**科技新闻**
1. [Anthropic 发布 Claude Sonnet 5.5：与 Sonnet 5 同价，更快更省并接管 claude.ai 免费档](#item-tech-news-1) ⭐️ 8.0/10
2. [德里配电改革：电网损耗从约 50%降至 5%](#item-tech-news-2) ⭐️ 7.0/10
3. [研究：AI 聊天服务向广告商披露对话数据并暴露会话链接](#item-tech-news-3) ⭐️ 7.0/10
4. [伦敦车站人脸识别试验扫描约 50 万张面孔：零逮捕、1 例误报](#item-tech-news-4) ⭐️ 7.0/10
5. [荷兰因美国制裁风险试点 NixOS，替代微软软件，首版拟于 2027 年底推出](#item-tech-news-5) ⭐️ 7.0/10
6. [SemiAnalysis 解析 GLM-5.3 稀疏注意力对 HBM 内存占用的影响](#item-tech-news-6) ⭐️ 7.0/10
7. [免费开源书籍《How to Make Your Model Fast》讲解全栈 ML 性能工程](#item-tech-news-7) ⭐️ 7.0/10
8. [快手可灵 Kling 4.0 宣布 10 月上线，Flash 版已小范围体验](#item-tech-news-8) ⭐️ 7.0/10

**财经新闻**
1. [AMD 宣布以 82 亿美元收购李飞飞创办的 World Labs](#item-finance-news-1) ⭐️ 8.0/10
2. [CNBC 分析：特朗普市政债券持仓超千笔，规模最高约 10 亿美元](#item-finance-news-2) ⭐️ 7.0/10
3. [中国证监会据报为人形机器人 IPO 设三道门槛，几乎无企业达标](#item-finance-news-3) ⭐️ 7.0/10
4. [电力审批延期，甲骨文就星际之门新墨西哥数据中心发不可抗力通知](#item-finance-news-4) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Anthropic 发布 Claude Sonnet 5.5：与 Sonnet 5 同价，更快更省并接管 claude.ai 免费档](https://simonwillison.net/2026/Sep/28/claude-sonnet-5-5/) ⭐️ 8.0/10

Anthropic 于 9 月 28 日发布 Claude Sonnet 5.5，官方宣称其运行速度比 Sonnet 5 快 30% 以上、多数任务成本最多降低 30%，定价与 Sonnet 5 持平，并称其在智能体编程基准 Terminal-Bench 4.0 上得分 70.6%（Sonnet 5 为 10.3%）。该模型也是首款搭载网络安全防护机制的 Sonnet：网络安全与前沿大模型开发类高风险请求会自动回退到 Sonnet 5 或被直接拦截，生物危害与蒸馏类请求则直接拦截。Simon Willison 的实测复现了一个与 Opus 5.5 相同的 bug——&quot;max&quot; 思考档位消耗 128,000 个 token（约 1.28 美元）后耗尽额度、未能生成 SVG，而 &quot;xhigh&quot; 档位则以 5.74 美分、耗时 41 秒产出质量不错的图形。Sonnet 5.5 现已全平台上线并成为 claude.ai 免费档的驱动模型，Willison 认为这使 Anthropic 目前的免费服务强于使用 Luna 5.6 的 ChatGPT 免费档；官方同时确认 Haiku 5.5 将在数周内发布。

rss · Simon Willison · 9月28日 22:07

**「背景」** Claude Sonnet 是 Anthropic 产品线中介于旗舰 Opus 与轻量 Haiku 之间的中端模型系列，Sonnet 5.5 是 Claude 5.5 家族继 Opus 5.5 之后发布的第二款模型，也是 Sonnet 5 在相同价格点上的直接换代。文中用于实测的&quot;骑自行车的鹈鹕&quot;SVG 生成是 Willison 常用的模型能力测试，其中的&quot;max&quot;&quot;xhigh&quot;指 Claude 可调节的思考档位（thinking effort）。Willison 在 2026 年 9 月 22 日的博文中曾记录 Opus 5.5 在&quot;max&quot;档位下过度思考、耗尽 token 预算后无法产出结果的问题，本次 Sonnet 5.5 复现的正是同一缺陷。

**「对开发者的实际影响」** 对现有 API 用户而言，Sonnet 5.5 是一次零成本切换：定价维持每百万 token 2/10 美元不变，官方称多数工作可提速 30% 以上、成本最多降低 30%，直接替换 Sonnet 5 即可获得收益。但需注意一个已复现的兼容性问题：&quot;max&quot; 思考档位会在消耗 128,000 token（约 1.28 美元）后无法产出结果，与 Opus 5.5 的已知 bug 相同，修复前应避免在该档位运行长思考任务，或设置用量上限加以防护。此外，该模型首次引入网络安全防护回退机制，网络安全相关的高风险请求会被自动降级至 Sonnet 5 或直接拦截，依赖响应一致性的应用需为此类行为变化做好准备。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.marktechpost.com/2026/09/28/anthropic-releases-claude-sonnet-5-5-70-6-on-terminal-bench-4-0-at-the-same-2-10-price/">Anthropic Releases Claude Sonnet 5.5: 70.6% on Terminal-Bench ...</a></li>
<li><a href="https://thenextweb.com/news/sonnet-5-5-cyber-distillation">Anthropic releases Claude Sonnet 5.5 with the cyber ... - TNW</a></li>

</ul>
</details>

**标签**: `#AI`, `#LLM`, `#Anthropic`, `#Claude`, `#model-release`

---

<a id="item-tech-news-2"></a>
### [德里配电改革：电网损耗从约 50%降至 5%](https://spectrum.ieee.org/delhi-electricity-loss) ⭐️ 7.0/10

IEEE Spectrum 发表长篇回顾报道，梳理德里如何通过对配电环节的私有化和现代化改造，把配电网损耗从约 50%降至 5%，并基本消除了长期存在的计划外停电。对德里居民而言，比降损更根本的变化是&quot;甩负荷&quot;式断电的终结——据评论者回忆，过去一天停电数次、复电时的电压浪涌常迫使用户抢拔昂贵家电。需要说明的是，这是一篇针对已完成基础设施转型的系统工程案例回顾，而非新技术的发布或厂商声明。

hackernews · rbanffy · 9月29日 12:43 · [社区讨论](https://news.ycombinator.com/item?id=49892245)

**「2002 年的配电私有化」** 德里这场改革的起点是 2002 年的配电私有化：BSES 与塔塔电力（Tata Power）接手各区的配电运营，并被赋予降低损耗的任务，当时德里全城的综合技术与商业（AT&amp;C）损耗率超过 52%。AT&amp;C 损耗由两部分构成：输配电过程中的技术性损耗，以及窃电、电表失灵等已供电却收不回电费的商业性损耗，这正是“损耗”一度能占供电量一半的原因。

**「对其他高损耗配电区的可复制性」** 德里模式对印度其他高损耗配电区具有直接参照价值：据塔塔电力自称，其主导的奥里萨邦配电改革同样实现了 AT&amp;C 损耗持续下降和大规模基础设施升级，并被称为全国标杆（该说法来自企业自身宣传，尚非独立评估）。对仍在高损耗和频繁计划外停电环境中运营的监管机构与配电公司，德里二十年尺度的量化结果——电网可靠性从 2002 年约 70% 升至 99.9% 以上、塔塔电力辖区损耗从 53.1% 降至 6.3%——表明私有化运营配合全面计量与防窃电改造可作为改革模板，但此类成效依赖长期持续投入，而非一次性设备升级。

**「社区讨论」** 评论者 motionlessveloc 回忆二十年前德里一天数次停电、复电浪涌迫使大家抢着拔掉电视和笔记本电脑的情形，认为终结&quot;甩负荷&quot;比降低线损更具革命性。其他讨论延伸至国际比较与后续路线：有人指出希腊电费单将线损单独列项、因此缺乏降损激励，有人认为文中数据里新加坡电网的表现才是更值得研究的故事，还有评论建议印度利用充足日照推广屋顶和垂直太阳能并搭配电池储能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://timesofindia.indiatimes.com/city/delhi/from-50-losses-to-6-how-delhi-fixed-its-power-loses/articleshow/130121379.cms">From 50 % losses to 6%: How Delhi fixed its power loses | Delhi News</a></li>
<li><a href="https://grokipedia.com/page/Tata_Power_Delhi_Distribution_Limited">Tata Power Delhi Distribution Limited — Grokipedia</a></li>
<li><a href="https://spectrum.ieee.org/delhi-electricity-loss">How Delhi Cut Electricity Loss from 50 to 5 Percent - IEEE Spectrum</a></li>
<li><a href="https://www.linkedin.com/posts/tata-power_revolutionizing-electricity-distribution-activity-7363840902613602304-GKUb">Tata Power -led Odisha discoms improve electricity access... | LinkedIn</a></li>

</ul>
</details>

**标签**: `#power-grid`, `#infrastructure`, `#energy`, `#india`, `#electrical-engineering`

---

<a id="item-tech-news-3"></a>
### [研究：AI 聊天服务向广告商披露对话数据并暴露会话链接](https://jorgegarciaherrero.com/wp-content/interactivos/20260916-Prompt-like-a-butterfly-sting-like-a-tracker-%28clean%29.pdf) ⭐️ 7.0/10

一项题为《Prompt like a Butterfly, Sting like a Tracker》的测量研究论文于 2026 年 9 月 29 日经 Hacker News 发布并引发广泛讨论（312 分、102 条评论），论文发现多家 AI 聊天服务提供商向第三方（包括广告商和追踪器）披露敏感的对话衍生数据，如会话标题、用户提示词和截图，且这些数据往往伴随可用于用户归因的持久标识符。研究还发现，部分提供商公开暴露未设访问控制的对话永久链接，追踪者借此能够读取整段对话内容。该论文属于对行业现行数据做法的测量记录，而非某家公司新近发生的意外泄露事件。

hackernews · damaru2 · 9月29日 09:03 · [社区讨论](https://news.ycombinator.com/item?id=49890226)

**「背景」** 这篇题为《Prompt like a Butterfly, Sting like a Tracker》的论文由 IMDEA Networks 研究员 Narseo Vallina-Rodríguez 领导的团队完成，并已被隐私技术领域经同行评审的学术论坛 PoPETs 2027 接收，说明其结论经过了学术审查。研究基于 2026 年 5 月在西班牙开展的测量，覆盖 9 个网页版 AI 聊天服务，其中 6 个被发现向第三方传输对话数据。不过该行为并非普遍存在：报告同时指出 Copilot、DeepSeek 和 Meta AI 在网页端未向第三方服务传输对话数据，因此隐私风险因具体服务商而异。

**「对用户的实际影响」** 对于主流 AI 聊天机器人的用户，这意味着在托管聊天界面中输入的提示词应被视为可能流向第三方：测量研究发现 20 款聊天机器人中有 17 款向至少一个第三方共享信息，其中 3 款通过 Microsoft Clarity 的会话回放功能以明文发送提示词和回答片段，15 款向广告、分析或社交端点传输会话 URL 或聊天标识符。可行的应对是避免在网页版聊天中粘贴医疗、法律或未发表工作等敏感内容，并留意是否意外生成了无访问控制的会话永久链接。需要注意的是，相关报道指出 ChatGPT 和 Claude 虽然比 Grok 有更强的访问控制，但仍在向广告和分析服务商传输部分标识符与元数据，因此换用&\#x27;隐私口碑更好&\#x27;的产品并不能完全消除暴露。

**「社区讨论」** 在 Hacker News 讨论中，用户 drywater2 反对“泄露”的说法，认为这类数据外流是有意的商业出售而非失误，而用户 pbasista 补充报告称 ChatGPT 网页版会在用户实际发送之前，周期性地将未完成的提示词发送到 conversation/prepare 端点，此类部分输入可能暴露写作节奏、纠错习惯和草稿思路的演变。另有用户 kdaniel\_03 将这一发现与本月早些时候一起涉及私密 Codex 会话中未发表草稿的署名争议相提并论，认为无论数据流向模型训练还是广告追踪，本应私密的提示词都难以保全，并因此主张开源模型是用户唯一可控的路径。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://jorgegarciaherrero.com/en/prompt-like-a-butterfly-sting-like-a-tracker/">Infographic of the paper &quot; Prompt like a Butterfly , sting like a tracker &amp;quo...</a></li>
<li><a href="https://www.drweb.de/ki-chatbots-chatdaten-tracker-werbenetzwerke/">Geben KI- Chatbots Ihre Chatdaten an Werbenetzwerke weiter?</a></li>
<li><a href="https://dzen.ru/b/aruhZhvMVjoeuHxk">6 из 9 веб-чатов передавали данные бесед сторонним... | Дзен</a></li>
<li><a href="https://arxiv.org/abs/2604.27438v1">Tracking Conversations: Measuring Content and Identity Exposure on AI ...</a></li>
<li><a href="https://grafa.com/en/news/crypto/ai-chatbot-data-leak-study">AI chatbots accused of leaking user data to ad trackers</a></li>

</ul>
</details>

**标签**: `#privacy`, `#ai-industry`, `#tracking`, `#chatbots`, `#security-research`

---

<a id="item-tech-news-4"></a>
### [伦敦车站人脸识别试验扫描约 50 万张面孔：零逮捕、1 例误报](https://www.theguardian.com/technology/2026/sep/29/trial-live-facial-recognition-cameras-london-stations-false-positive) ⭐️ 7.0/10

据《卫报》报道，英国一项在伦敦铁路车站试运行的实时人脸识别摄像头项目在数个月内扫描了约 50 万张面孔，最终未促成任何逮捕，仅记录了 1 例误报。这些是试验实际部署运行后得出的测量结果，而非厂商宣称或计划中的能力。报道称，这一结果正在引发关于公共 AI 监控价值与风险的争论。

hackernews · ilamont · 9月29日 11:35 · [社区讨论](https://news.ycombinator.com/item?id=49891480)

**「背景」** 实时人脸识别（LFR）指摄像头在车站等公共场所对过往人群进行实时面部扫描、并与警方监视名单自动比对的监控技术，英国此前多轮类似试点长期伴随隐私与公民自由方面的争议。与常规的官方评估发布不同，这项为期六个月、耗资超过 32 万英镑并占用警方近 100 小时工时的试验结果，是通过信息自由（FOI）申请披露的文件才公开的。

**「零战果数据成为扩张计划的直接反证」** 约 50 万次扫描零逮捕、仅一次误报的结果，为伦敦警察厅拟在圣诞节前将实时人脸识别扩展至伦敦市中心的计划提供了具体反证，而英国多家商店已在 7 月上线可即时向警方报警的类似系统。在都柏林—霍利黑德航线的同类试验同样扫描数千名乘客却无任何匹配之后，连续的零产出数据可能促使警方与车站运营方在继续部署前重新核算投入产出比，公民团体也由此获得了质疑公共 AI 监控成本与效用的量化依据。

**「社区讨论」** 评论者 blitzar 对数据规模提出算术上的质疑：按其估算，16 套设备在车站运行 6 个月却只扫描约 50 万张面孔，意味着摄像头约 99%的时间并未工作，且 50 万张大约只相当于利物浦街车站两天的日均客流。另有用户从不同角度提出质疑——jwally 追问此类监控（包括美国的 flock 摄像头）的实际投入产出比是否成立，Frieren 则批评街头摄像头正在助长“监控国家”式的氛围——这些均为个人观点，尚无独立数据加以验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theguardian.com/technology/2026/sep/29/trial-live-facial-recognition-cameras-london-stations-false-positive">Trial of live facial recognition cameras in London stations ...</a></li>
<li><a href="https://www.techmeme.com/260929/p16">Techmeme: FOI docs: UK police&#x27;s six-month live facial ...</a></li>
<li><a href="https://www.theguardian.com/technology/2026/sep/29/trial-live-facial-recognition-cameras-london-stations-false-positive">Trial of live facial recognition in London stations ... | The Guardian</a></li>
<li><a href="https://www.irishtimes.com/crime-law/2026/04/13/facial-recognition-trial-on-dublin-holyhead-route-scans-thousands-but-finds-no-matches/">Facial recognition trial on Dublin-Holyhead route scans thousands...</a></li>

</ul>
</details>

**标签**: `#facial-recognition`, `#surveillance`, `#privacy`, `#civil-liberties`, `#AI-ethics`

---

<a id="item-tech-news-5"></a>
### [荷兰因美国制裁风险试点 NixOS，替代微软软件，首版拟于 2027 年底推出](https://www.tomshardware.com/software/the-netherlands-is-rolling-alternative-nixos-based-software-ecosystem-after-u-s-sanctions-on-icc-took-microsoft-off-the-table-trial-programs-running-now-first-release-expected-at-end-of-2027) ⭐️ 7.0/10

在美国对国际刑事法院（ICC）法官实施制裁、暴露出对美国技术供应商的依赖风险之后，荷兰政府正在试点基于 NixOS 的软件生态，以替代微软产品。目前试用计划已经运行，但首个正式版本预计要到 2027 年底才会推出，因此这一替代生态仍处于早期验证阶段，属于已宣布的计划而非已落地的能力。推动该项目的直接原因是制裁带来的供应风险：当美国制裁波及 ICC 法官时，荷兰重新评估了政府软件体系完全依赖美国厂商的隐患。

hackernews · mywacaday · 9月29日 11:44 · [社区讨论](https://news.ycombinator.com/item?id=49891550)

**「背景：ICC 遭美国制裁的经过」** NixOS 是一个基于 Nix 包管理器、以声明式配置和可复现系统状态著称的开源 Linux 发行版。促成荷兰政府转向的直接前因是：2025 年，国际刑事法院（ICC）前首席检察官遭美国制裁后，不仅被禁止入境美国，还失去了微软企业邮箱的访问权限，个人和机构银行账户也被冻结。这家总部位于海牙的法院随后面临金融与 IT 服务被切断、甚至无法向美国雇员支付工资的风险，荷兰政府在旁观这一过程中意识到，关键服务的可用性可能取决于美国政府单方面做出的决定。

**「影响」** 在 2027 年底首个版本发布之前，荷兰各政府机构仍将继续运行微软产品，当前可实际参与的是正在进行的试点计划，这意味着整个转变是一条多年期路线图，而非立即可用的替代方案。如果试点按计划推进，公共部门的 IT 团队需要逐步积累 NixOS 相关的部署与维护能力，并解决与现有微软体系的迁移和兼容问题。

**「社区讨论」** 评论者 guidoiaquinti 报告称，受美国制裁引发的金融封锁影响，多名 ICC 法官一度无法访问银行账户、领取薪水或进行日常转账，这为荷兰的转向提供了具体背景，但该说法来自论坛评论，未经独立核实。其他评论意见分歧：silverFork 认为这更接近欧洲对美国产品的“自我制裁”，并主张开源替代方案的使用与支持成本远低于微软产品；SillyUsername 则认为离开 Windows 10/11 反而可能促使机构发现可行的新选择——两者均为个人观点而非已证实的事实。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://apnews.com/article/icc-trump-sanctions-eu-israel-netherlands-2c1cc314732f920c2de59396d3b556f6">The Dutch prepare for US sanctions against the International ...</a></li>
<li><a href="https://www.europesays.com/3271995/">The Netherlands Built a Nix-Basd Linux Desktop Because ...</a></li>

</ul>
</details>

**标签**: `#digital-sovereignty`, `#nixos`, `#open-source`, `#government-it`, `#linux`

---

<a id="item-tech-news-6"></a>
### [SemiAnalysis 解析 GLM-5.3 稀疏注意力对 HBM 内存占用的影响](https://newsletter.semianalysis.com/p/sparse-savings-persistent-demand-inside-glm53) ⭐️ 7.0/10

SemiAnalysis 于 2026 年 9 月 28 日发布由 Kimbo Chen 撰写的分析文章，主题是 GLM-5.3 所采用的稀疏注意力设计如何影响 HBM 显存占用，对评估推理显存成本与部署容量的团队具有参考价值。文章覆盖 KV cache 卸载、HiSparse、DeepSeek 稀疏注意力、IndexShare 以及单次 rollout 异步优化等相关技术，来源关键词还标示其涉及网络安全内容。需要注意的是，本次供给的材料仅包含文章标题与关键词，未附正文，因此文中关于内存节省幅度、性能或成本的具体论断均无法核实，应视为该媒体的待验证分析，而非已获独立测量的结果。

rss · Semianalysis · 9月28日 19:26

**「稀疏注意力与 KV 缓存」** 在大模型推理中，注意力层需要为历史 token 保存 KV 缓存，这部分数据通常驻留在 HBM 显存中，并随上下文变长成为带宽与容量开销的主要来源。据检索到的外部资料，Z.ai 的 GLM-5.3 采用 DeepSeek Sparse Attention（DSA）类稀疏注意力，在注意力计算时只动态选取少量 top-k token 参与运算，从而降低该环节的内存带宽占用。不过，由于 token 筛选步骤本身仍需访问完整上下文历史，KV 缓存依旧要整体保留在内存中，因此稀疏注意力削减的主要是注意力运算期间的访问量，并不必然等比减少总体内存容量需求——这是理解该文分析 HBM 用量的关键前提。

**「对推理部署方的实际影响」** 对运行 GLM-5.3 这类稀疏注意力模型的推理服务商而言，HBM 显存压力的缓解取决于 KV 缓存分层卸载基础设施是否到位：冷 KV 缓存若继续驻留在昂贵的 HBM 中会牺牲并发能力，而卸载层级过深又会推高延迟、损害用户体验。可采取的具体做法包括部署类似 SGLang 团队 HiSparse 的分层内存系统（主动将 KV 缓存从设备 HBM 卸载到主机 DRAM），或采用 Nvidia Dynamo 支持的从 GPU HBM 到 CPU DRAM、本地 SSD 再到网络存储的多级 KV 缓存卸载方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.partgenie.ai/insights/how-glm5-3-sparse-attention-affects-hbm-memory-usage-2">How GLM-5.3 Sparse Attention and Hierarchical Memory Shape Accelerator ...</a></li>
<li><a href="https://www.polaris7.io/signals/glm-53-sparse-attention-impact-on-dram-memory-tam">GLM-5.3 Sparse Attention Impact on DRAM Memory TAM</a></li>
<li><a href="https://newsletter.semianalysis.com/p/sparse-savings-persistent-demand-inside-glm53">Inside GLM-5.3: How Sparse Attention Affects DRAM Memory TAM</a></li>
<li><a href="https://404kresearch.substack.com/p/the-ai-memory-demand-landscape-the">The AI Memory Demand Landscape: The HBM Bandwidth Wall, KV Cache Expansion, and SSD Tiering</a></li>
<li><a href="https://www.blocksandfiles.com/ai-ml/2026/03/30/nvidia-and-its-partners-kv-cache-extenders/5209284">Nvidia and its partners&#x27; KV Cache extenders</a></li>

</ul>
</details>

**标签**: `#sparse-attention`, `#AI-inference`, `#HBM-memory`, `#KV-cache`, `#GLM-5.3`

---

<a id="item-tech-news-7"></a>
### [免费开源书籍《How to Make Your Model Fast》讲解全栈 ML 性能工程](https://www.reddit.com/r/MachineLearning/comments/1wt6ns4/i_wrote_a_free_opensource_book_on_making_ml/) ⭐️ 7.0/10

Reddit 用户 /u/SoloTiger\_ 发布了免费开源书籍《How to Make Your Model Fast: A Systems View of Efficient Machine Learning, from Silicon to Agents》，托管在 GitHub 仓库 usamahz/make-your-model-fast，并邀请 ML 系统、推理、编译器与边缘 AI 方向的从业者提供反馈和贡献。这本书的核心论点是：减少 FLOPs 不一定能让模型更快，优化前必须先判断系统究竟受计算、带宽、内存还是系统层面的约束，书中从 roofline 分析和硬件讲起建立这套判断直觉。全书路线依次覆盖内核（kernels）、编译器、量化、剪枝、视觉、端侧 LLM、机器人、性能分析（profiling）、推理服务（serving），最后讨论 agent 工作负载下的同类分析。以上内容均出自作者的自述发布，书籍的实际深度和质量尚无法仅凭该帖子独立验证。

reddit · r/MachineLearning · /u/SoloTiger\_ · 9月29日 10:35

**「背景」** 本书的前提是机器学习推理优化中的一个基础概念：模型在特定硬件上的实际速度取决于它受计算、显存带宽、内存还是系统开销约束，而不是 FLOPs 总量本身，因此量化、剪枝这类减少计算量的手段并不必然带来加速，优化前通常需要借助 roofline 分析等方法先定位瓶颈。从仓库状态看，该书 usamahz/make-your-model-fast 已发布第一版（v1.0）的 Release，可在 ai.usamah.me 免费在线阅读或下载。

**「影响」** 从事推理优化、编译器、边缘 AI 或 ML 系统工作的开发者现在可以免费获取这本覆盖 roofline 分析、内核、量化、服务到 agent 全栈的资料，并直接通过 GitHub 仓库 usamahz/make-your-model-fast 阅读或提交贡献，作者明确征集上述领域从业者的反馈与协作。对于需要判断量化、剪枝或内核优化是否值得投入的团队，书中&quot;先确定系统受算力、带宽、内存还是系统限制，再选择优化手段&quot;的分析路径提供了一个现成的参考框架；但由于该书为作者自行发布，内容质量尚未经独立验证，读者在采用前应自行评估其深度与准确性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/usamahz/make-your-model-fast/releases/tag/v1.0">Release How to Make Your Model Fast, first edition · usamahz/make-your-model-fast</a></li>

</ul>
</details>

**标签**: `#ml-systems`, `#performance-engineering`, `#inference-optimization`, `#quantization`, `#gpu-kernels`

---

<a id="item-tech-news-8"></a>
### [快手可灵 Kling 4.0 宣布 10 月上线，Flash 版已小范围体验](https://finance.sina.com.cn/stock/t/2026-09-28/doc-initmeau2827369.shtml) ⭐️ 7.0/10

快手可灵 AI 宣布，其 AI 视频生成模型 Kling 4.0 将于 10 月正式上线，目前这仍是官方预告，尚未正式发布。据公告，新版本计划支持 4K 及 1080p 10-bit HDR 视频输出，单次可输入最多 10 张图片、5 段视频和 7 个主体作为参考，并能生成最长 30 秒的视频。其中较轻量的 Kling 4.0 Flash 已于 9 月 28 日率先向小范围用户开放体验，完整版 4.0 的实际生成效果与可用性仍需等 10 月上线后验证。

telegram · zaihuapd · 9月29日 00:52

**「10-bit HDR 与先行版本」** 此次率先开放体验的 Kling 4.0 Flash 是完整版正式上线前的先行版本，一位获得早期访问的创作者称，完整版明显强于 Flash，尤其是在对话驱动的表演生成方面。公告中 10-bit HDR 规格的实际意义在于：AI 视频通常采用 8-bit（每通道约 256 级色阶），而 10-bit 可提供约 1024 级色阶，更多色阶能减少天空和色彩渐变在进入调色流程后出现的色带伪影。

**「影响」** 对依赖人物与服装一致性的带货、短剧和口播类创作者而言，可灵 4.0 的多参考输入（单次最多 10 张图、5 段视频、7 个主体）与 4K、1080p 10-bit HDR 输出，正好补强了这类工作流最需要的参考控制与成片规格——第三方测评显示可灵 2.6 在 IP 人设、口播与剧情场景本就以人像和音画同步见长，而可灵 3.0 在 2026 年初已位列四大主流 AI 视频模型之一。想提前上手的用户可关注 9 月 28 日已开放的小范围 Kling 4.0 Flash 体验渠道，正式版预计 10 月上线。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=b2jR0rOGEKQ">SPARE, a short film generated with the full version of Kling ... - YouTube</a></li>
<li><a href="https://www.drweb.de/kling-4-0-ki-video-30-sekunden-kuaishou/">Kling 4 . 0 : Was kann Kuaishous neues KI-Videomodell? | Dr. Web</a></li>
<li><a href="https://opencreator.io/zh/blog/ai-video-models-comparison-2026">主流AI 视频模型横向测评2026：Seedance、Veo、Sora、万相</a></li>
<li><a href="https://www.atlascloud.ai/blog/tips/seedance-vs-kling-vs-sora-vs-veo">Best Sora Alternatives in 2026: Seedance vs Kling vs Veo-Ultimate Head-to-Head Comparison - Atlas Cloud Blog</a></li>

</ul>
</details>

**标签**: `#AI 视频生成`, `#可灵 Kling`, `#快手`, `#生成式 AI`, `#模型发布`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [AMD 宣布以 82 亿美元收购李飞飞创办的 World Labs](https://ir.amd.com/news-events/press-releases/detail/1299/amd-to-acquire-world-labs-to-advance-the-future-of-ai-compute) ⭐️ 8.0/10

AMD 宣布以 82 亿美元收购李飞飞创办的“世界模型”AI 公司 World Labs，交易预计在年底前完成，仍需监管批准，李飞飞将加入 AMD 担任执行副总裁兼首席科学家。World Labs 的技术旨在让 AI 理解和模拟物理世界，并可用于生成机器人训练所需的模拟环境，此次收购将把其模型研发与 AMD 的芯片和计算平台结合。

telegram · zaihuapd · 9月29日 03:59

**「背景」** World Labs 于 2024 年由李飞飞创办并担任 CEO，她因在现代生成式 AI 多项基础研究中的贡献被称为&quot;AI 教母&quot;，曾执掌谷歌云 AI 业务。此次收购前，这家初创公司累计融资约 10 亿美元，其专注的&quot;世界模型&quot;技术旨在让 AI 更好地理解和模拟物理世界。

**「对行业的影响」** 在 AI 芯片市场与英伟达竞争的 AMD 借此加强机器人、模拟和物理 AI 能力，可能改变依赖模拟环境训练机器人的企业可选的技术供应商格局。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aifunding.me/insights/world-labs-deep-dive">World Labs : How a High-Growth AI Pioneer Is... | AI Funding</a></li>
<li><a href="https://cointelegraph.com/news/godmother-ai-world-labs-230-million-funding?trk=article-ssr-frontend-pulse_little-text-block">‘Godmother of AI ’ launches World Labs with $230M funding at...</a></li>
<li><a href="https://www.linkedin.com/news/story/amd-targets-physical-ai-with-82b-world-labs-acquisition-7608652/">AMD targets physical AI with $8.2B World Labs acquisition | LinkedIn</a></li>
<li><a href="https://www.androguider.com/2026/09/amd-to-acquire-fei-fei-lis-world-labs.html">AMD to Acquire Fei-Fei Li’s World Labs for $8.2 Billion in Bold AI Bet</a></li>

</ul>
</details>

**标签**: `#mergers-and-acquisitions`, `#AMD`, `#AI-compute`, `#world-models`, `#robotics`

---

<a id="item-finance-news-2"></a>
### [CNBC 分析：特朗普市政债券持仓超千笔，规模最高约 10 亿美元](https://www.cnbc.com/2026/09/29/trump-municipal-bond-portfolio.html) ⭐️ 7.0/10

CNBC 对财务披露文件的分析显示，美国总统特朗普的市政债券持仓已超过 1000 笔，总价值约 3 亿至 10 亿美元，其中许多发行人（包括城市、医院、学校和电力公司）直接受其政府的监管与拨款决定影响。CNBC 表示未发现特朗普利用政策信息交易或指示交易的证据，白宫与特朗普集团称其投资由独立机构管理的全权委托账户持有。

rss · CNBC Finance · 9月29日 14:37

**「背景」** 与普通联邦雇员不同，美国总统不在禁止官员参与涉及其个人财务利益事务的联邦利益冲突法（美国法典第 18 编第 208 条）的适用范围内，这一豁免源自老布什政府时期的立法安排。因此，特朗普持有市政债券（即城市、医院、公用事业等公共机构为融资而发行的债务）本身并不违法，但由于总统不受该法约束，其利益冲突疑虑难以通过现行法律追究。

**「影响」** 由于其账户持有获豁免更严格环保限制的燃煤电厂以及依赖 Medicaid 资金的医院等发行人的债券，伦理专家认为当联邦行动直接涉及具体发行人时，总统决策与个人财务的利益冲突问题最为突出。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://factually.co/fact-checks/politics/federal-ethics-rules-president-family-commercial-crypto-products-c0156c">What federal ethics or conflict - of - interest rules appl...</a></li>
<li><a href="https://www.law.cornell.edu/uscode/text/18/208">18 U . S . Code § 208 - Acts affecting a personal financial interest</a></li>
<li><a href="https://www.politico.com/story/2016/11/trump-bush-ethics-exemption-231773">Trump owes ethics exemption to George H.W. Bush - POLITICO</a></li>

</ul>
</details>

**标签**: `#municipal bonds`, `#conflict of interest`, `#financial disclosures`, `#Trump administration`, `#public finance`

---

<a id="item-finance-news-3"></a>
### [中国证监会据报为人形机器人 IPO 设三道门槛，几乎无企业达标](https://www.cnbc.com/2026/09/29/china-criteria-humanoid-robot-ipos.html) ⭐️ 7.0/10

据三位知情人士称，中国证监会已通过&quot;窗口指导&quot;要求拟上市的人形机器人企业满足三项标准：拥有可持续营收和商业订单、亏损收窄（一位消息人士称需提供三年预测）、并掌握&quot;机器人大脑&quot;或灵巧手等核心技术。在中国 100 多家具身智能初创公司中，预计只有极少数甚至没有一家能达到这些门槛，显示这一热门赛道正在降温。

rss · CNBC Finance · 9月29日 07:19

**「背景」** 中国证监会此前曾以促进投融资“动态平衡”为由分阶段限制 IPO，上一轮限制在监管负责人暗示放松前持续了约 18 个月。此次收紧发生在人形机器人板块明显过热之后：行业代表宇树科技 8 月 19 日在上海上市首日暴涨逾 460%后股价近乎腰斩，当局也多次警示该行业存在泡沫。

**「影响」** 若该指引属实，仅在港股一地已递交上市申请的至少二十余家人形机器人相关企业及其投资方，通过 IPO 融资或退出的路径可能受阻；行业数据机构 Xiniu 数据显示，该赛道二季度投资额达 470.9 亿元（约 69.5 亿美元），同比增逾六倍。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.szftbz.com/blog/china-companies-fundraising-options-narrow-after-ipo-restrictions">China companies&#x27; fundraising options narrow after IPO restrictions</a></li>
<li><a href="https://www.scmp.com/business/china-business/article/3300050/china-may-ease-ipo-curbs-csrc-head-signals-policy-loosening-morgan-stanley-says">China may ease IPO curbs as CSRC head signals policy loosening...</a></li>

</ul>
</details>

**标签**: `#China regulation`, `#humanoid robotics`, `#IPOs`, `#embodied AI`, `#CSRC`

---

<a id="item-finance-news-4"></a>
### [电力审批延期，甲骨文就星际之门新墨西哥数据中心发不可抗力通知](https://www.bloomberg.com/news/articles/2026-09-24/oracle-cites-force-majeure-to-shield-itself-on-controversial-data-center) ⭐️ 7.0/10

星际之门位于新墨西哥州的 Project Jupiter 数据中心因 2.45GW 配套微电网的环境与供电审批迟迟未获批，面临无法按 2028 年目标投运的风险，甲骨文已向项目开发方发出不可抗力通知，拟在外部因素导致延期时推迟部分付款。据 Bloomberg 与 TechCrunch 报道，该项目相关 180 亿美元银团贷款已出现折价交易，反映市场对超大型 AI 数据中心建设进度的担忧。

telegram · zaihuapd · 9月29日 05:46

**「背景」** 星际之门是 OpenAI 参与的超大规模 AI 算力基建计划，新墨西哥州 Project Jupiter 的开发方为 Blue Owl，据外部报道，此次卡住审批的供电配套具体涉及一条天然气管道。由于租约安排要求甲骨文即使无法使用设施也须继续付款，公司才援引不可抗力条款，为设施若无法在 2028 年投运时推迟部分付款留出空间。

**「影响」** 为该项目提供约 180 亿美元银团贷款的银行及债务投资者直接承压：贷款分销陷入停滞，市场报价跌至面值的 89%至 91%（约合 160 亿至 164 亿美元），反映投资者对项目进度和甲骨文信用状况的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=mNozPwLvJIY">Oracle Is Paying for a Data Center It Can&#x27;t Use - YouTube</a></li>
<li><a href="https://best-ai.org/ai-news/oracle-triggers-force-majeure-on-245-gw-stargate-data-center-in-new-mexico-over-energy-supply-delays-gm2tsb">Oracle Triggers Force Majeure on 2 . 45 - GW Stargate Data Center in...</a></li>
<li><a href="https://digg.com/tech/oxyjjcs1">Oracle reportedly sends notice to delay Project Jupiter payments if it...</a></li>
<li><a href="https://finance.biggo.com/news/aa2b00f9-d885-40e0-92db-6fd9f55ffe63">Oracle&#x27;s $18 Billion AI Loan Sells at a Discount, Banks Forced to Swallow a Hot Potato — BigGo Finance</a></li>
<li><a href="https://www.tradingkey.com/analysis/stocks/us-stocks/262176714-oracle-stock-forecast-18b-data-center-loan-trades-tradingkey">Oracle Stock Price Forecast: $18 Billion Data Center Loan Deeply Discounted, Will ORCL Continue to Fall?</a></li>
<li><a href="https://allweatherfinance.com/oracles-18-billion-ai-loan-is-being-sold-at-a-discount-highlighting-the-pressure-on-its-ai-financing-chain/">Oracle&#x27;s $18 billion AI loan is being sold at a discount, highlighting the pressure on its AI financing chain.</a></li>

</ul>
</details>

**标签**: `#AI数据中心`, `#甲骨文`, `#星际之门`, `#不可抗力`, `#银团贷款`

---