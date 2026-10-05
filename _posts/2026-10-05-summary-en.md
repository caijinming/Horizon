---
layout: default
title: "Horizon Summary: 2026-10-05 (EN)"
date: 2026-10-05
lang: en
---

> From 23 items, 3 important content pieces were selected

---

**Technology News**
1. [Nolan Lawson asks why developers don&\#x27;t &quot;use the platform&quot;](#item-tech-news-1) ⭐️ 7.0/10
2. [Reddit claims top Kaggle ARC-AGI-3 scores jumped from 7% to 56%](#item-tech-news-2) ⭐️ 7.0/10
3. [White House Forms &\#x27;Super Intelligence Force&\#x27; AI Task Force With 120-Day Risk Report](#item-tech-news-3) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Nolan Lawson asks why developers don&\#x27;t &quot;use the platform&quot;](https://nolanlawson.com/2026/10/03/why-dont-more-developers-use-the-platform/) ⭐️ 7.0/10

Nolan Lawson published an essay on his blog on October 3, 2026, asking why most web developers build with frameworks like React instead of &quot;using the platform&quot; of native browser APIs, and the piece drew heavy engagement on Hacker News \(277 points, 288 comments\). The essay includes criticism of web components&\#x27; design as part of explaining why direct platform development has not caught on more widely. It is an opinion essay rather than a new tool, standard, or benchmark, so its claims are arguments to evaluate rather than shipped capabilities or independently measured results.

hackernews · vinhnx · Oct 4, 04:10 · [Discussion](https://news.ycombinator.com/item?id=49950554)

**「The &quot;use the platform&quot; debate」** &quot;Use the platform&quot; is a long-standing argument in web development: rather than rebuilding functionality in JavaScript, developers should rely on what the browser provides natively, such as semantic HTML, CSS, and built-in behaviors. As the author&\#x27;s own site states, advocates of web standards, performance, and accessibility have implored developers for years to follow this advice — asking why build something yourself in JavaScript when the browser can do it for you — and Nolan Lawson counts himself among those advocates. That positioning makes the essay an examination from inside the movement of why developers nonetheless keep defaulting to frameworks like React.

**「Practical takeaway」** For developers weighing &quot;use the platform&quot; advice, the discussion points to a case-by-case check rather than a blanket rule: commenters document concrete platform gaps, reporting that native &lt;datalist&gt; form suggestions are unusable in most browsers and that Web Components are rarely adopted without wrapper libraries such as Lit. The practical action is to verify the specific platform APIs a project depends on across target browsers before removing a framework like React — a gap the essay itself attributes to browsers historically playing catch-up with the ecosystem built on top of them.

**「Community discussion」** Several commenters pushed back on the idea that platform APIs are ready for direct use: one argued React simply made feasible what was &quot;extremely difficult and cumbersome&quot; with native APIs alone and called web components &quot;an incredible idea poorly implemented,&quot; while another said web components are a badly designed API that few developers use without wrappers like Lit. A third cited the native &lt;datalist&gt; element as a concrete case, claiming its implementations are so poor in most browsers that rolling your own autocomplete remains justified.

<details><summary>References</summary>
<ul>
<li><a href="https://nolanlawson.com/2026/10/03/why-dont-more-developers-use-the-platform/">Why don’t more developers “use the platform”? | Read the Tea ...</a></li>
<li><a href="https://nolanlawson.com/">Read the Tea Leaves | Software and other dark arts, by Nolan ...</a></li>
<li><a href="https://nolanlawson.com/2026/10/03/why-dont-more-developers-use-the-platform/">Why don’t more developers “ use the platform ”? | Read the Tea Leaves</a></li>

</ul>
</details>

**Tags**: `#web-development`, `#frontend-frameworks`, `#web-components`, `#browser-apis`, `#javascript`

---

<a id="item-tech-news-2"></a>
### [Reddit claims top Kaggle ARC-AGI-3 scores jumped from 7% to 56%](https://www.reddit.com/r/MachineLearning/comments/1wxcd4k/top_arc%CE%B1gi3_scores_on_kaggle_just_went_from_7_to/) ⭐️ 7.0/10

A post in r/MachineLearning claims that the top score on the Kaggle ARC-AGI-3 leaderboard rose from 7% to 56% within roughly 30 days, attributing the jump to small locally-run models operating inside agent harnesses. The poster, /u/we\_are\_mammals, says these small models now exceed average human performance on a benchmark he describes as intentionally designed to favor humans, with Kaggle competition rules restricting entrants to small local models. The only supplied evidence is a leaderboard screenshot that the author himself calls out-of-date, and the post includes no methodology details, primary results, or independent verification, so the reported jump remains unconfirmed.

reddit · r/MachineLearning · /u/we\_are\_mammals · Oct 4, 10:24 · [Discussion](https://www.reddit.com/r/MachineLearning/comments/1wxcd4k/top_arc%CE%B1gi3_scores_on_kaggle_just_went_from_7_to/)

**「How ARC-AGI-3 differs from earlier versions」** ARC-AGI-3 is the newest version of the ARC-AGI benchmark family: ARC-AGI-1 and ARC-AGI-2 presented static input-output grid pairs from which systems had to infer and apply transformation rules, while ARC-AGI-3 instead places agents in turn-based game environments with no stated rules, instructions, or win conditions. Reports on the benchmark described frontier models such as GPT-5, Claude, and Gemini scoring below 1% on this format. On the official leaderboard, ARC Prize&\#x27;s Kaggle track runs competition submissions under strict, competition-specific compute constraints, showcasing purpose-built efficient methods.

**「Impact」** For entrants in the ARC Prize 2026 Kaggle track, the reported jump—if confirmed by official scores—would make agent-harness engineering rather than model scale the decisive competitive factor, since Kaggle rules restrict participants to small local models, which the post credits for the gain. It would also pressure the benchmark&\#x27;s premise: ARC-AGI-3 is scored so that 100% means matching human efficiency across its games, and the ARC Prize Foundation separately measures human performance as a baseline, so scores above average-human level within a month would call those baselines into question. The figures remain unverified, however; a third-party leaderboard snapshot lists GPT-6 Astra leading overall at 62.7%, but it does not corroborate the specific 7%-to-56% Kaggle claim, so competitors should await confirmed official numbers before drawing conclusions.

<details><summary>References</summary>
<ul>
<li><a href="https://arcprize.org/leaderboard">ARC Prize - Leaderboard</a></li>
<li><a href="https://dev.to/codepawl/gpt-5-claude-gemini-all-score-below-1-arc-agi-3-just-broke-every-frontier-model-5dbj">GPT-5, Claude, Gemini All Score Below 1% - ARC AGI 3 Just Broke...</a></li>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>
<li><a href="https://arcprize.org/blog/arc-agi-3-human-dataset">Measuring Human Performance on ARC-AGI-3 | ARC Prize</a></li>
<li><a href="https://benchlm.ai/benchmarks/arcagi3">ARC-AGI-3 Leaderboard &amp; Scores — October 2026 | BenchLM.ai</a></li>

</ul>
</details>

**Tags**: `#ARC-AGI`, `#benchmarks`, `#machine-learning`, `#reasoning`, `#kaggle`

---

<a id="item-tech-news-3"></a>
### [White House Forms &\#x27;Super Intelligence Force&\#x27; AI Task Force With 120-Day Risk Report](https://www.wsj.com/tech/ai/new-ai-task-force-to-report-on-risks-of-technology-after-public-and-industry-concerns-b6308bef) ⭐️ 7.0/10

According to the Wall Street Journal, the White House has created an AI task force named the &\#x27;Super Intelligence Force,&\#x27; led by Director of National Intelligence Jay Clayton, who confirmed the role to the paper; a senior White House official said it makes Clayton effectively the administration&\#x27;s &\#x27;AI czar.&\#x27; The group is charged with assessing the risks of artificial intelligence and what responsibility the federal government should take for the technology, and per the report is due to deliver a risk assessment within 120 days. Despite mounting safety concerns, President Trump has ruled out new AI regulation, instead backing a voluntary framework built on external safety audits and stronger internal controls, with staying ahead of China cited as the priority. Clayton said the president asked for a team to ensure the US &\#x27;continues to lead in superintelligence&\#x27; while putting the interests of the American people first, and told industry executives the country is &\#x27;leading by a lot&\#x27; and will keep that lead.

telegram · zaihuapd · Oct 4, 02:37

**「The &\#x27;AI czar&\#x27; model and its voluntary-first mandate」** An &\#x27;AI czar&\#x27; is an informal Washington label for an official who coordinates policy across the government without heading a dedicated regulator; CNBC reports that Jay Clayton, the sitting Director of National Intelligence, was tapped for that role atop the new White House task force. The group&\#x27;s working method follows the administration&\#x27;s voluntary-first posture: corroborating reports say it plans to work with AI companies rather than replace industry-led safeguards, review existing laws and potential congressional action, and build government systems for handling warnings involving breaches, hacks, and AI model jailbreaks.

**「Impact」** AI companies operating in the US should not expect new binding requirements from this initiative in the near term, since the administration&\#x27;s stated preference is a voluntary framework of external safety audits and stronger internal controls. The 120-day risk report will be the first concrete indication of what federal role the task force proposes over AI, making it the key document for firms tracking US policy.

<details><summary>References</summary>
<ul>
<li><a href="https://www.yahoo.com/news/politics/articles/trump-ai-czar-outlines-u-035456290.html">Trump’s new AI czar outlines U.S. strategy for AI risks and leadership...</a></li>
<li><a href="https://www.cnbc.com/2026/10/03/trump-jay-clayton-ai-czar.html">Trump taps Director of National Intelligence Jay Clayton as AI czar</a></li>
<li><a href="https://www.aa.com.tr/en/americas/white-house-forms-task-force-to-assess-ai-risks-opportunities-wsj/4077340">White House forms task force to assess AI risks , opportunities: WSJ</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#AI governance`, `#US government`, `#AI safety`, `#tech industry`

---