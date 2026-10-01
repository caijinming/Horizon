---
layout: default
title: "Horizon Summary: 2026-10-01 (ZH)"
date: 2026-10-01
lang: zh
---

> 从 41 条内容中筛选出 12 条重要资讯。

---

**科技新闻**
1. [谷歌公布新一代前沿模型 Gemini 4 Argon，全面开放尚需等待](#item-tech-news-1) ⭐️ 9.0/10
2. [EDG C++ 编译器前端在 GitHub 公开](#item-tech-news-2) ⭐️ 8.0/10
3. [32 名研究者历时八个月发布现代 NLP 分词技术综述](#item-tech-news-3) ⭐️ 7.0/10
4. [CO2Jump：免训练自校正采样器改善文图一致性](#item-tech-news-4) ⭐️ 7.0/10
5. [DeepSeek 开源华为升腾版核心 AI 基础组件](#item-tech-news-5) ⭐️ 7.0/10
6. [Cloudflare 宣布计划成为公共证书颁发机构](#item-tech-news-6) ⭐️ 7.0/10
7. [Baseten 将 Kimi K3 接入 OpenAI Codex 企业付费结算通道](#item-tech-news-7) ⭐️ 7.0/10
8. [Reddit 将于 11 月停用 RSS，2027 年 3 月关闭公开 API](#item-tech-news-8) ⭐️ 7.0/10
9. [OpenAI 称瓦解模型蒸馏攻击，归因月之暗面相关人员](#item-tech-news-9) ⭐️ 7.0/10

**财经新闻**
1. [Kalshi, Polymarket trading volumes on some products raise questions amid massive growth](#item-finance-news-1) ⭐️ 7.0/10
2. [中国商务部警告：若欧盟限制中国企业将&quot;坚决回应&quot;](#item-finance-news-2) ⭐️ 7.0/10
3. [中国证监会据报道为人形机器人 IPO 设三项新标准，多数申请企业恐难达标](#item-finance-news-3) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [谷歌公布新一代前沿模型 Gemini 4 Argon，全面开放尚需等待](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-argon/) ⭐️ 9.0/10

谷歌通过官方博客公布了新一代前沿大模型 Gemini 4 Argon，该消息在 Hacker News 上获得 985 分和 666 条评论的高热度讨论。此次属于公告而非全面发布：讨论中引用的公告原文称，谷歌将继续收集早期测试者反馈并完善防护机制，之后再“尽快”向开发者、企业和消费者开放，普通用户目前尚无法直接使用。被引用的公告内容还提到 Argon 智能体正在谷歌内部执行 C/C++ 代码库向 Rust 的迁移，但由于本次提供的公告正文并不完整，相关能力与性能宣称暂无法独立核实。

hackernews · bradleyg223 · 9月30日 20:04 · [社区讨论](https://news.ycombinator.com/item?id=49913571)

**「背景」** Gemini 4 Argon 是 Google DeepMind 旗下 Gemini 前沿模型系列的最新一代，由 Google DeepMind 高级副总裁 Koray Kavukcuoglu 于 2026 年 9 月 30 日公布，官方将其定位为面向长周期任务的前沿模型，应用方向包括真实世界软件工程、法律与金融类企业知识工作以及网络防御。此次属于发布公告而非全面上线：官方称模型&quot;即将推出&quot;（rolling out soon），第三方报道显示其将先向网络安全团队提供，之后才面向开发者、企业和消费者开放，全面可用的时间表尚未确定。

**「Argon 尚未开放使用，基准领先缺乏独立验证」** Argon 目前仅向一小批网络安全合作伙伴和早期测试者开放，开发者、企业和普通消费者仍无法直接使用，短期内的实际可用性影响有限。有意评估或采用该模型的团队需要等待 Google 根据早期反馈完善护栏后再扩大开放。此外，其宣称在多数类别中领先 Anthropic Claude Opus 5.5、Claude Fable 5.1 和 OpenAI GPT-6 Astra 的基准成绩均来自 Google 自行发布的数据，尚无独立测试支持，技术选型决策应将这一不确定性纳入考量。

**「社区讨论」** 评论区的核心争论围绕行业格局：nickysielicki 认为前沿实验室今年轮番领先的“蛙跳”态势证伪了 Dario Amodei 此前“赢家通吃”（concentrating）的判断，AI 能力正变得更分散而非集中；juanre 由此建议开发者在工作流中保持模型与供应商可替换。体验分享方面，taylorfinley 描述了 Gemini 3.8 Flash 在其 Strix Halo 设备上自动附加 GDB、逆向内核 ioctl 接口并编写 LD\_PRELOAD C shim 以修复 ROCm/llama.cpp 兼容问题的亲身经历，babelfish 则借公告中“尽快开放”的措辞调侃谷歌“又一次没能发布模型”。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-argon/">Introducing Gemini 4 Argon - The Keyword</a></li>
<li><a href="https://www.datacamp.com/blog/gemini-4-argon">Gemini 4 Argon: Benchmarks, Pricing, and Access | DataCamp</a></li>
<li><a href="https://venturebeat.com/technology/google-unveils-gemini-4-argon-retaking-benchmark-lead-over-openai-and-anthropic-but-in-limited-release">Google unveils Gemini 4 Argon, retaking benchmark lead over ...</a></li>
<li><a href="https://www.trendingtopics.eu/gemini-4-argon-google-anthropic-openai/">Google Finally Brings Gemini 4 Into the Fight Against ...</a></li>
<li><a href="https://www.axios.com/2026/09/30/google-gemini-4">Google unveils Gemini 4, long-awaited answer to OpenAI and ...</a></li>

</ul>
</details>

**标签**: `#artificial-intelligence`, `#google`, `#large-language-models`, `#gemini`, `#ai-industry`

---

<a id="item-tech-news-2"></a>
### [EDG C++ 编译器前端在 GitHub 公开](https://edgcpp.org/#transition) ⭐️ 8.0/10

Edison Design Group（EDG）已将其长期专有的 C++ 编译器前端公开在 GitHub 的 edgcpp/compiler 仓库中，采用 Apache-2.0（含 LLVM 例外条款）许可证，并在 edgcpp.org 发布了过渡公告和文档。该代码库保留了可追溯到 1990 年的提交历史，这套前端数十年来被广泛嵌入商业 C++ 工具，最著名的用途是为 Visual C++ 的 IntelliSense 提供代码补全支持。社区评论指出，公告中未提及 EDG 公司据称正在收缩关闭，这次公开很可能是其收尾动作，因此项目的长期维护前景尚不确定。

hackernews · iandinwoodie · 9月30日 19:26 · [社区讨论](https://news.ycombinator.com/item?id=49913192)

**「背景」** Edison Design Group（EDG）的 C++ 前端是一款以高度符合 C++ 标准著称的编译器前端，过去约三十年间始终以专有授权形式提供给编译器和开发工具厂商嵌入使用，被视为业界使用最广泛的前端之一；据社区开发者介绍，Visual C++ 的 IntelliSense 便采用该前端而非微软自研的编译前端。评论者还指出，此次公开的代码库保留了最早可追溯至 1990 年的完整提交历史，这在同类开源转移案例中相当罕见。

**「实际影响」** 对长期依赖 EDG 前端的编译器、IDE 与静态分析工具厂商而言，最直接的后果是：这套此前专有的前端现以 Apache 2.0 许可证公开源码，且官方表示将接受社区对代码库的贡献，团队可以自行审计、修改并提交补丁，而不必再依赖闭源授权。非营利组织 The C++ Alliance——拥有在职编译器工程师并深度参与 C++ 标准与 Boost 社区——已成为 EDG 的非营利托管方，承担其后续的社区维护角色。将 EDG 嵌入商业产品的团队应关注新公开仓库的更新节奏，并评估在社区贡献模式下，跟进上游变更与维护内部定制之间的同步成本。

**「社区讨论」** 评论者 jabl 指出公告未提及 EDG 公司正在收缩，并引用维基百科条目所引的 Herb Sutter 2025 年 11 月 C++ 标准会议报告作为依据，认为这正是开源前端的动因。badsectoracula 则探讨能否借助其源到源编译能力把 C++ 库转译为其他语言（例如将 FLTK 编译为 Free Pascal 供 Lazarus 使用），以缓解在非 C++ 环境中集成 C++ 库的长期痛点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://edgcpp.org/">Open Source Transition · EDGCPP</a></li>
<li><a href="https://techplanet.today/post/edg-c-front-end-goes-open-source-a-historic-moment-for-the-c-community">EDG C++ Front-End Goes Open Source: A Historic Moment for the ...</a></li>
<li><a href="https://edgcpp.org/">Open Source Transition · EDGCPP</a></li>
<li><a href="https://www.phoronix.com/news/EDG-CPP-Open-Sourced">EDG C/ C++ Front - End Open -Sourced - Phoronix</a></li>

</ul>
</details>

**标签**: `#C++`, `#compilers`, `#open-source`, `#developer-tools`, `#programming-languages`

---

<a id="item-tech-news-3"></a>
### [32 名研究者历时八个月发布现代 NLP 分词技术综述](https://www.reddit.com/r/MachineLearning/comments/1wuccjf/tokenization_a_survey_for_modern_nlp_r/) ⭐️ 7.0/10

在 r/MachineLearning 社区，用户 /u/mcmcmcmcmcmcmcmcmc\_ 发布了一份现代 NLP 分词（tokenization）综述，称由 32 名分词研究者历时约 8 个月完成，并附有 alphaXiv 链接（2609.tokenization-survey-modern-nlp）。据帖子介绍，综述覆盖分词算法、评估方法、多语言处理、编码方式与理论，并讨论了潜在分词、视觉分词等替代方案，以及约束生成、token 修复（token healing）和分词器安全等相邻议题。需要指出的是，这是一则作者自行发布的介绍帖，带有一定宣传色彩，其覆盖范围与结论尚未经独立验证；该工作定位为领域参考资料，而非新方法或基准突破。

reddit · r/MachineLearning · /u/mcmcmcmcmcmcmcmcmc\_ · 9月30日 18:13

**「分词的基础概念与前期综述」** 分词（tokenization）是现代 NLP 的基础环节：语言模型并非直接读取字符或单词，而是读取分词器切分出的子词单元，因此切分方式会影响多语言覆盖、数字与代码处理乃至生成质量。尽管作用面广，该领域长期被认为研究不足——2025 年 2 月一篇关于离散分词器的综述就指出，当时文献中仍缺少对该方向的全面系统性梳理，而本次发布的分词综述正是对这一基础环节的补充。

**「影响」** 对从事大语言模型研究与工程的开发者而言，这份综述可作为分词器设计、评估、多语言表现及安全风险（如分词器安全）等决策的集中参考入口；但由于内容来自作者自述，使用前应核对原始论文以确认各章节的实际覆盖范围与结论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2502.12448v1">From Principles to Applications: A Comprehensive Survey of ...</a></li>

</ul>
</details>

**标签**: `#tokenization`, `#NLP`, `#large language models`, `#survey`, `#machine learning`

---

<a id="item-tech-news-4"></a>
### [CO2Jump：免训练自校正采样器改善文图一致性](https://www.reddit.com/r/MachineLearning/comments/1wtyl5m/concurrent_image_understanding_and_generation/) ⭐️ 7.0/10

来自 Google、Google DeepMind 与石溪大学的研究人员（作者自述论文已被 NeurIPS 2026 接收，该说法尚属自报）发布 CO2Jump，一种面向耦合马尔可夫跳跃过程的免训练自校正采样器，针对联合模型并行生成文本与图像时&quot;文本说对、图像画错&quot;的不一致问题。该采样器每步去噪只需一次模型前向传播，利用文本置信度与跨模态注意力引导图像更新，并允许低置信度 token 被重新掩码后再生成，从而在生成过程中修正早期决定；采样器本身无需额外训练，实验在同一个任务微调模型上对比不同采样方法。作者在图像编辑、迷宫求解与 nonogram（数图）三类任务上评估，并引入 JEdit-1M、JMaze-200K、JNono-200K 三个新数据集，其中拼图类基准要求文本答案与生成图像同时正确才计为联合正确。作者报告，在 8–512 个采样步范围内，CO2Jump 是其对比的采样器中唯一在编辑质量与文本接地（grounding）两方面均单调提升的方法。

reddit · r/MachineLearning · /u/Upstairs\_Theme2785 · 9月30日 07:28

**「技术背景」** CO2Jump 建立在掩码离散扩散（常以马尔可夫跳跃过程形式化）生成模型之上：这类模型从全部被掩码的离散 token 出发，在多步去噪中逐步填充内容，而&quot;重掩码&quot;（remasking）机制允许模型在生成过程中撤回并重做低置信度的决定，该论文的技术背景部分正是以掩码扩散模型与重掩码为出发点。另一个必要前提是统一多模态模型的发展：单一模型同时承担图像理解（文本输出）与图像生成，但两类输出并行产生、彼此缺少校验环节，因此文字答案与所绘图像可能出现不一致。

**「影响」** 对研究联合多模态模型及离散扩散、马尔可夫跳跃过程采样方法的研究者而言，CO2Jump 可作为免训练的采样替换方案直接作用于现有任务微调模型，三个新数据集也为文本-图像一致性提供了可验证的联合正确性判据，作者还公开征集其他能同时评估一致性与正确性的任务。不过需要注意，所报告的收益目前仅在任务微调模型以及编辑、迷宫、数图等较窄的基准上得到验证，方法在更通用场景下的有效性尚未证实。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/papers/2607.13188.md">huggingface.co/ papers /2607.13188.md</a></li>
<li><a href="https://www.alphaxiv.org/abs/2607.13188">Concurrent Image Understanding and Generation ... | alphaXiv</a></li>

</ul>
</details>

**标签**: `#machine-learning`, `#generative-models`, `#multimodal`, `#discrete-diffusion`, `#sampling-methods`

---

<a id="item-tech-news-5"></a>
### [DeepSeek 开源华为升腾版核心 AI 基础组件](https://mp.weixin.qq.com/s/X41mKH4Ds-VXUAnK6M8Eww) ⭐️ 7.0/10

据报道，DeepSeek 于 2026 年 9 月 30 日开源了面向华为升腾平台的基础组件，涵盖 TileLang 高级语言编译工具、计算库 DeepGEMM Ascend 与 TileKernels、分布式通信库 DeepEP Ascend，以及 FlashMLA 和 DeepSelect，与其英伟达平台的组件形成对应。DeepSeek 称相关组件在多项测试中性能接近硬件上限，但这一说法属于厂商自述，报道本身未附仓库链接或第三方验证数据，实际可用性有待仓库公开后确认。此外，DeepSeek 正与华为共同推进升腾 950 的 128 卡超节点方案，这属于进行中的合作计划，而非已交付的成品。

telegram · zaihuapd · 9月30日 03:09

**「背景」** DeepSeek 此前已围绕其模型运行开源了一整套自研基础设施，但原本面向英伟达 GPU 构建：DeepGEMM 负责矩阵运算，DeepEP 负责芯片间大规模通信，TileKernels 负责标准向量计算，FlashMLA 是面向长上下文的注意力内核库，DeepSelect 负责数据过滤。其中 FlashMLA 的仓库说明显示其已为 DeepSeek-V4.1 模型在 NVIDIA GPU 和华为升腾 NPU 上的推理提供支持，而此次的 DeepGEMM-Ascend 则与原版 DeepGEMM 完全 API 兼容，支持 BF16、FP8、FP4 精度的 GEMM 计算。

**「对升腾部署团队的影响」** 若此次开源发布属实，在华为升腾平台部署 DeepSeek 模型的团队可直接复用其官方计算与通信组件（DeepGEMM、DeepEP、FlashMLA 等），减少自行将 CUDA 生态代码移植到 CANN 的工作量——CUDA 与 CANN 之间的移植成本正是团队评估升腾方案时的已知考量之一（tool-3-1）。但该发布目前仅有单一转载来源、无仓库链接，“性能接近硬件上限”出自 DeepSeek 自述且未经独立验证，因此在迁移生产负载前，团队应先等待官方仓库地址和第三方基准测试结果，并确认组件与所用升腾芯片型号及 CANN 版本的兼容性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/deepseek-ai/DeepGEMM-Ascend">GitHub - deepseek-ai/DeepGEMM-Ascend: DeepGEMM-Ascend: clean ...</a></li>
<li><a href="https://github.com/deepseek-ai/FlashMLA">GitHub - deepseek-ai/FlashMLA: FlashMLA: Efficient Multi-head ...</a></li>
<li><a href="https://startupfortune.com/deepseek-open-sources-chip-tools-that-could-let-huawei-replace-nvidia-in-china/">DeepSeek open sources chip tools that could let Huawei ...</a></li>
<li><a href="https://www.spheron.network/blog/huawei-ascend-950-vs-nvidia-b300-b200-llm-inference-2026/">Huawei Ascend 950 vs NVIDIA B300 and B200 for LLM Inference ...</a></li>

</ul>
</details>

**标签**: `#deepseek`, `#huawei-ascend`, `#ai-infrastructure`, `#open-source`, `#ai-hardware`

---

<a id="item-tech-news-6"></a>
### [Cloudflare 宣布计划成为公共证书颁发机构](https://blog.cloudflare.com/cloudflare-certificate-authority/) ⭐️ 7.0/10

Cloudflare 宣布计划成为公共证书颁发机构（CA），已申请加入 Chrome、Apple、Microsoft 和 Mozilla 四大根证书计划，并与 GlobalSign 签署协议收购一个受广泛信任的根证书。目前该 CA 尚未开始签发任何证书，此次属于计划公告而非已上线的签发能力，能否入根仍取决于各浏览器和操作系统厂商的审核。新 CA 将优先支持 ACME 协议实现证书的自动签发与续期，并计划在 2027 年第一季度签发生产级默克尔树证书（MTC），以面向后量子时代的互联网安全需求。

telegram · zaihuapd · 9月30日 06:26

**「背景」** 要让证书在浏览器和操作系统中获得默认信任，公共 CA 需被 Chrome、Apple、Microsoft、Mozilla 各自运营的根证书计划接纳，或链接到某个已受信任的根；据外部报道，Cloudflare 从 GlobalSign 收购的根证书签发于 2012 年，正是这样的存量可信根。另据报道，Cloudflare 上使用免费 ACME 证书的站点目前由第三方 CA 签发，若新 CA 通过各根计划审核，这些站点可能迎来新的签发者。

**「对网站运营者与开发者的影响」** 对网站运营者和开发者而言，若 Cloudflare 的根证书未来被 Chrome、Apple、Microsoft 和 Mozilla 的根证书计划接纳，市场上将新增一个优先支持 ACME 自动签发与续期的公共 CA 选项，可简化证书的获取和续期流程；但目前它尚未签发任何证书，现有部署无需立即变更。需要留意的是其计划在 2027 年第一季度签发生产级默克尔树证书（MTC）以面向后量子互联网，依赖 TLS 的系统可据此时间点提前评估抗量子证书迁移的准备工作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ppc.land/cloudflare-targets-q1-2027-for-its-first-quantum-safe-web-certificates/">Cloudflare targets Q1 2027 for its first quantum-safe web certificates</a></li>
<li><a href="https://blog.cloudflare.com/cloudflare-certificate-authority/">Building a certificate authority for the whole Internet | Cloudflare Blog</a></li>
<li><a href="https://www.voicendata.com/security/cloudflare-public-certificate-authority-expands-web-pki-12596095">Cloudflare Public Certificate Authority Expands Web PKI</a></li>

</ul>
</details>

**标签**: `#Cloudflare`, `#certificate-authority`, `#PKI`, `#TLS`, `#post-quantum`

---

<a id="item-tech-news-7"></a>
### [Baseten 将 Kimi K3 接入 OpenAI Codex 企业付费结算通道](https://36kr.com/newsflashes/4005691489112198) ⭐️ 7.0/10

据 36 氪快讯，美国 AI 基础设施公司 Baseten 宣布，企业用户可在 OpenAI 编程工具 Codex 中调用中国开源大模型 Kimi K3，相关调用费用直接计入企业既有的 OpenAI 采购承诺额度，无需走新的供应商采购流程。报道称这使 Kimi K3 成为中国开源模型中首个进入 OpenAI 企业付费结算体系的产品。该消息目前仅有一条简短快讯支撑，属于 Baseten 单方宣布，缺少模型接入方式、可用范围等技术细节和独立信源验证，实际落地情况有待进一步确认。

telegram · zaihuapd · 9月30日 11:23

**「OpenAI Codex 的企业采购承诺机制」** Kimi K3 是中国公司月之暗面（Moonshot AI）推出的开源大模型，此前中国开源模型一直未能进入 OpenAI 面向企业客户的计费结算体系。OpenAI 的编程工具 Codex 面向企业客户采用采购承诺模式结算，企业预先锁定一定消费额度并按实际用量扣减，过去若要使用其他厂商的模型，企业通常需要另签供应商合同、走独立的采购流程。Baseten 是一家提供模型托管推理服务的美国 AI 基础设施公司，此次充当了 Kimi K3 与 OpenAI 企业结算通道之间的承载方。

**「企业侧影响：无需新增供应商流程，启用前需核实结算条款」** 对已与 OpenAI 存在采购承诺的企业而言，最直接的影响是可以在 Codex（OpenAI 的编程智能体工具，提供可本地运行的 CLI 等形态）中直接调用 Kimi K3，费用计入既有 OpenAI 额度，无需再走新增供应商的采购与合规流程，这为企业评估和引入这款中国开源模型降低了门槛。需留意的是，该消息目前仅来自 36 氪的一条快讯，Baseten 侧的具体定价、可用范围以及企业合同是否默认覆盖此类第三方模型调用均无细节，相关团队在启用前应与 OpenAI 和 Baseten 核实结算条款与适用范围。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://technode.com/2026/09/30/kimi-k3-enters-openais-enterprise-codex-channel-and-billing-system/">Kimi K3 enters OpenAI’s enterprise Codex channel and billing ...</a></li>
<li><a href="https://www.techflowpost.com/en-US/newsletter/138394">Kimi K3 Integrates with OpenAI Codex Enterprise Channel ...</a></li>
<li><a href="https://github.com/openai/codex">GitHub - openai / codex : Lightweight coding agent that runs in your...</a></li>

</ul>
</details>

**标签**: `#大模型生态`, `#开源模型`, `#企业 AI 采购`, `#OpenAI Codex`, `#模型互操作性`

---

<a id="item-tech-news-8"></a>
### [Reddit 将于 11 月停用 RSS，2027 年 3 月关闭公开 API](https://techcrunch.com/2026/09/30/reddit-is-killing-rss-feeds-ending-public-api-access-because-of-ai-bots/) ⭐️ 7.0/10

Reddit 宣布将于 2026 年 11 月 13 日起停止 RSS 订阅支持，并计划在 2027 年 3 月关闭公开 API，理由是这些渠道已被用于大规模抓取和自动化滥用，尤其是 AI 机器人。这一变化将影响依赖 RSS 的订阅用户、第三方应用和机器人开发者，以及使用自动化工具的版主。作为过渡安排，Reddit 建议版主改用 Discord Relay，并要求第三方应用和机器人开发者在 2027 年 1 月 12 日前完成注册，否则将失去 API 访问权限。目前该消息来自对 TechCrunch 报道的转载，属于 Reddit 公布的计划时间表而非已生效的变更。

telegram · zaihuapd · 10月1日 00:27

**「RSS 与公开 API 的既有用途」** RSS（Really Simple Syndication，简易信息聚合）是一种开放的网络订阅格式，允许用户和应用程序以标准化方式获取网站的更新内容，Reddit 此前长期为站点提供此类订阅源。Reddit 的公开 API 则支持以编程方式访问站内对话，被社交媒体监测产品、研究人员使用的工具以及 AI 助手等产品广泛采用，这些现存的依赖关系正是此次关闭政策波及的范围。

**「开发者与版主需在截止日期前完成迁移」** 依赖 Reddit 公开 API 的第三方应用和机器人开发者必须在 2027 年 1 月 12 日前完成注册，才能在 API 关闭后保留访问权限。使用 RSS 频道接收社区提醒的版主被建议在 11 月 13 日前将相关流程迁移到 Discord Relay Devvit 应用。需要留意的兼容性限制是，Reddit 承认部分 RSS 用途没有直接替代方案，习惯用 RSS 阅读器订阅 Reddit 的读者在停用后只能改用其他方式获取内容。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/09/30/reddit-is-killing-rss-feeds-ending-public-api-access-because-of-ai-bots/">Reddit is killing RSS feeds and ending public API ... | TechCrunch</a></li>
<li><a href="https://tech.slashdot.org/story/26/09/30/1841213/reddit-is-killing-rss-feeds-ending-public-api-access">Reddit Is Killing RSS Feeds , Ending Public API Access - Slashdot</a></li>
<li><a href="https://techbeat.co/story/reddit-ends-rss-feeds-and-public-api-as-ai-data-revenue-grows">Reddit Ends RSS Feeds and Public API as AI Data Revenue Grows</a></li>
<li><a href="https://mashable.com/tech/reddit-rss-feeds-public-api-shutdown-ai-scraping">Reddit is shutting down RSS and public API access. Blame AI.</a></li>
<li><a href="https://tech.yahoo.com/social-media/articles/reddit-killing-rss-feeds-ending-174500068.html">Reddit is killing RSS feeds and ending public API access ...</a></li>

</ul>
</details>

**标签**: `#reddit`, `#api`, `#rss`, `#developer-ecosystem`, `#ai-bots`

---

<a id="item-tech-news-9"></a>
### [OpenAI 称瓦解模型蒸馏攻击，归因月之暗面相关人员](https://openai.com/index/disrupting-a-coordinated-model-distillation-campaign/) ⭐️ 7.0/10

OpenAI 宣称已瓦解一起协调进行的模型蒸馏攻击活动，攻击者通过操纵与模型的交互来提取其受保护的推理内容。OpenAI 称该活动最早于 2026 年 7 月初出现，7 月 24 日至 25 日达到高峰，涉及 4000 多名用户的 1.6 万次请求，并称到 7 月 28 日已有 1.5 万余名用户的相关活动被瓦解（来源未说明这两组数字之间的具体关系）。OpenAI 将该活动的核心部分归因于与月之暗面（Kimi 开发商）有关的人员，但这一归因目前仅为 OpenAI 的单方面说法，尚无独立核实，且两家公司存在直接竞争关系。OpenAI 表示已通过 Frontier Model Forum 等渠道与业界和政府共享相关发现。

telegram · zaihuapd · 10月1日 01:18

**「背景：模型蒸馏与受保护的推理内容」** 模型蒸馏泛指借助一个模型的输出来训练或改进另一个模型，OpenAI 在公告中将“对抗性蒸馏”定义为系统性、未经授权地利用一个模型的输出或推理内容来训练、复现或改进另一个模型。推理模型的原始思维链被厂商视为需要保护的核心资产，据 CyberScoop 报道，OpenAI 称攻击者此次使用了“新型”手段绕过用于保护推理内容的加密机制。被 OpenAI 指认的月之暗面是一家中国 AI 公司，以 Kimi 系列模型（包括 K3）著称；该归因目前主要来自 OpenAI 的单方面披露，尚无独立核实。

**「行业与合规影响」** OpenAI 已通过 Frontier Model Forum 渠道向业界和政府共享此次事件信息，其他模型供应商可能据此收紧针对批量提取行为的使用限制与监测，依赖自动化流水线调用其 API 的开发者和组织需关注服务条款执行趋严带来的合规风险。此外，由于 Kimi 等中国开源模型正以低价或免费提供相当性能，且美国 AI 公司和政府此前已指控中国企业进行“系统性”蒸馏攻击，OpenAI 此次归因（目前仍为其单方面说法，尚无独立核实）可能使中国开源模型在海外市场面临更严格的审查。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/disrupting-a-coordinated-model-distillation-campaign/">Disrupting a coordinated model-distillation campaign | OpenAI</a></li>
<li><a href="https://cyberscoop.com/openai-moonshot-ai-model-distillation-attack/">OpenAI reveals ‘novel’ encryption bypass used in distillation ...</a></li>
<li><a href="https://wccftech.com/moonshot-ai-of-kimi-k3-fame-tried-to-crack-openais-encrypted-reasoning-through-16000-requests-bolstering-trump-administrations-distillation-claims/">Moonshot AI Of Kimi K3 Fame Tried To Crack OpenAI ... - Wccftech</a></li>
<li><a href="https://cyberscoop.com/openai-moonshot-ai-model-distillation-attack/">OpenAI reveals ‘novel’ encryption bypass used in distillation ...</a></li>
<li><a href="https://www.cnbc.com/2026/10/01/openai-chinas-moonshot-ai-kimi.html">OpenAI links China’s Moonshot AI to extraction attempt - CNBC</a></li>

</ul>
</details>

**标签**: `#AI security`, `#model distillation`, `#OpenAI`, `#Moonshot AI \(Kimi\)`, `#industry competition`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [Kalshi, Polymarket trading volumes on some products raise questions amid massive growth](https://www.cnbc.com/2026/09/30/kalshi-polymarket-trading-volume-scrutiny.html) ⭐️ 7.0/10

CNBC reports that unusual trading volume patterns on Kalshi and Polymarket are fueling concerns about potentially inflated or wash-traded volumes at a time when both platforms command multibillion-dollar valuations, face reported CFTC scrutiny, and are reportedly exploring public listings.

rss · CNBC Finance · 9月30日 21:09

**标签**: `#prediction-markets`, `#trading-volumes`, `#wash-trading-concerns`, `#CFTC-scrutiny`, `#IPO-valuations`

---

<a id="item-finance-news-2"></a>
### [中国商务部警告：若欧盟限制中国企业将&quot;坚决回应&quot;](https://www.cnbc.com/2026/09/30/china-warns-europe-increases-trade-pressure.html) ⭐️ 7.0/10

中国商务部周二晚间表示，若欧盟对中国企业或产品实施限制，中国将&quot;坚决回应&quot;，并称此类举动会&quot;严重损害互信&quot;并扰乱正在进行的贸易谈判。此前欧盟贸易专员谢夫乔维奇要求北京在 10 月前交出&quot;具体成果&quot;，否则面临&quot;更严厉措施&quot;；据媒体报道，德法正推动欧盟委员会加快打造一种可效仿美国&quot;301 条款&quot;、据称能在 24 小时内将中国隔绝于欧盟市场的工具。去年欧盟与中国的货物加服务贸易总额达 8800 亿欧元（约合 1 万亿美元），欧盟对华货物贸易逆差为全球最大。

rss · CNBC Finance · 9月30日 03:39

**「背景」** 欧盟与中国今夏一直在进行贸易谈判，布鲁塞尔要求中方在 10 月前拿出“具体成果”，以缩小其对华创纪录的贸易逆差。所谓“301 式工具”，指仿照美国《301 条款》的机制，可为欧盟在贸易争端中对华采取加征关税等更强硬措施提供新手段；据外部报道，法国和德国正推动欧盟委员会加快开发这一工具。

**「潜在影响」** 若欧盟最终推出&quot;301 式&quot;限制而中国兑现报复承诺，双方贸易中规模最大的电气设备和机械设备等品类的进出口企业，将直接面临关税上调或市场准入受阻的成本风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://informedclearly.com/en/trade-war/61779/eu-china-trade-war-european-section-301-2026">EU-China Trade War: Brussels&#x27; European Section 301 Explained</a></li>
<li><a href="https://www.firstpost.com/business/china-eu-trade-tensions-section-301-trade-tool-beijing-eu-trade-policy-14049259.html">China warns of ‘resolute response’ as EU weighs US-style ...</a></li>
<li><a href="https://ec.europa.eu/eurostat/statistics-explained/SEPDF/cache/55157.pdf">EU trade with China - latest developments Statistics Explained</a></li>

</ul>
</details>

**标签**: `#China-EU trade`, `#trade tensions`, `#retaliation threat`, `#trade policy`, `#tariffs`

---

<a id="item-finance-news-3"></a>
### [中国证监会据报道为人形机器人 IPO 设三项新标准，多数申请企业恐难达标](https://www.cnbc.com/2026/09/29/china-criteria-humanoid-robot-ipos.html) ⭐️ 7.0/10

据三位知情人士透露，中国证监会通过“窗口指导”（即监管层非正式的口头指引）要求人形机器人企业上市须满足三项标准：拥有可持续收入和商业订单、亏损持续收窄（一位人士称需提供三年预测）、掌握机器人“大脑”或灵巧手等核心技术。即使只需满足其中两项，已向港交所递交上市申请的至少二十余家企业中，恐怕也鲜有甚至无一达标。

rss · CNBC Finance · 9月30日 02:50

**「背景」** 中国目前有逾 100 家人形机器人企业，“具身智能”虽连续两年获政府工作报告支持，但官方也曾警示行业泡沫；作为行业风向标的宇树科技 8 月 19 日上市首日股价暴涨逾 460%至 845 元，至周一已近乎腰斩至 459.65 元。

**「潜在影响」** 若上述指导属实并执行，逾百家人形机器人初创企业及其背后的政府与民间资本将面临上市退出渠道收窄——该行业二季度投资额达 470.9 亿元（约 69.5 亿美元），是一季度的两倍多。

**标签**: `#China regulation`, `#humanoid robots`, `#IPO`, `#CSRC`, `#AI sector`

---