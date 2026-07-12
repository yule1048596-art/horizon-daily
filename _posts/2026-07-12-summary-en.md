---
layout: default
title: "Horizon Summary: 2026-07-12 (EN)"
date: 2026-07-12
lang: en
---

> From 63 items, 12 important content pieces were selected

---

1. [Claude Code uses 4x more tokens than OpenCode, study reveals.](#item-1) ⭐️ 8.0/10
2. [Terence Tao uses modern coding agents to build applications](#item-2) ⭐️ 8.0/10
3. [Ghostel: A new terminal emulator for Emacs powered by libghostty.](#item-3) ⭐️ 8.0/10
4. [Zer0Fit packages Google's TabFM and TimesFM as a local MCP server for zero-shot ML.](#item-4) ⭐️ 8.0/10
5. [Chromium's Math.tanh() Becomes a Fingerprinting Vector Exposing the User's OS](#item-5) ⭐️ 7.0/10
6. [Local resistance to AI data center expansion marks a new societal conflict.](#item-6) ⭐️ 7.0/10
7. [97 Chinese Embodied AI Data Firms Raised 4.47B Yuan in One Year](#item-7) ⭐️ 7.0/10
8. [UK Unveils £2 Billion Plan for AI Combat Laboratory](#item-8) ⭐️ 7.0/10
9. [Apple's Failed Car Project Boosted Its Powerful AI Chip Development](#item-9) ⭐️ 6.0/10
10. [Anthropic Clarifies Claude Code's Model vs. Effort Level Confusion](#item-10) ⭐️ 6.0/10
11. [AI Boom Triples Gas Turbine Prices Over Three Years](#item-11) ⭐️ 6.0/10
12. [Changxin Memory Tech's IPO Set to Be Largest A-Share Listing This Year](#item-12) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Claude Code uses 4x more tokens than OpenCode, study reveals.](https://systima.ai/blog/claude-code-vs-opencode-token-overhead) ⭐️ 8.0/10

An empirical study found that Anthropic's Claude Code sends approximately 33,000 tokens in its initial system prompt before reading user input, while OpenCode uses only about 7,000 tokens, representing a more than fourfold difference in overhead. This disparity highlights significant cost and efficiency concerns for developers using AI coding tools, as excessive token usage directly translates to higher API costs and could influence tool adoption and monetization strategies across the industry. The inefficiency is attributed to Claude Code's cache strategy and harness overhead, with community anecdotes suggesting its aggressive use of sub-agents can further burn through token budgets; however, some argue that raw token count alone is an insufficient metric without comparing task quality or success rates.

hackernews · systima · Jul 12, 18:25 · [Discussion](https://news.ycombinator.com/item?id=48883275)

**Background**: AI coding assistants like Claude Code and OpenCode function as agents that interact with large language models (LLMs) via APIs. The 'harness' refers to the tool's own code that constructs prompts, manages context, and orchestrates tools, which itself consumes tokens before the user's actual query is processed. Token consumption is a critical cost factor in developer tools that use pay-per-use API models.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/opencode-ai/opencode">GitHub - opencode-ai/opencode: A powerful AI coding agent. Built for the terminal. · GitHub</a></li>
<li><a href="https://docs.anthropic.com/en/docs/claude-code/overview">Claude Code overview - Anthropic</a></li>
<li><a href="https://github.com/ai-boost/awesome-harness-engineering">GitHub - ai-boost/awesome-harness-engineering: Awesome list for AI agent harness engineering: tools, patterns, evals, memory, MCP, permissions, observability, and orchestration. · GitHub</a></li>

</ul>
</details>

**Discussion**: The community debate is divided: some users report Claude Code's sub-agents are extremely token-intensive, while others suspect the high token usage is a deliberate monetization strategy by Anthropic. Several commenters note that token count alone is a flawed comparison metric and call for evaluating task completion quality, cost, and developer experience holistically.

**Tags**: `#AI-coding-tools`, `#token-efficiency`, `#developer-tools`, `#cost-optimization`, `#benchmarking`

---

<a id="item-2"></a>
## [Terence Tao uses modern coding agents to build applications](https://terrytao.wordpress.com/2026/07/11/old-and-new-apps-via-modern-coding-agents/) ⭐️ 8.0/10

Fields Medalist Terence Tao publicly shares his positive experience using large language model (LLM) coding agents, like Claude, to quickly build interactive applications and educational visualizations for his work. This endorsement from a world-renowned mathematician demonstrates that AI coding tools are powerful enough for sophisticated, non-software-specialist users to create valuable technical content, suggesting a significant democratization of software creation. Tao emphasizes that for supplementary, non-mission-critical interactive content like visualizations, the downside risk of using LLM-generated code is acceptable, positioning these tools as useful aids rather than replacements for core intellectual work.

hackernews · subset · Jul 12, 11:09 · [Discussion](https://news.ycombinator.com/item?id=48880170)

**Background**: Modern AI coding agents, such as Cursor and Claude Code, are software tools that leverage large language models to assist developers by generating, refactoring, and debugging code through interactive prompts. They represent a shift from simple code completion to more autonomous execution loops, enabling users without deep software engineering expertise to build functional applications.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@dave-patten/the-state-of-ai-coding-agents-2026-from-pair-programming-to-autonomous-ai-teams-b11f2b39232a">The State of AI Coding Agents (2026): From Pair Programming to Autonomous AI Teams | by Dave Patten | Medium</a></li>
<li><a href="https://www.augmentcode.com/tools/8-top-ai-coding-assistants-and-their-best-use-cases">8 Best AI Coding Assistants [Updated May 2026] | Augment Code</a></li>

</ul>
</details>

**Discussion**: The discussion shows strong enthusiasm, with users sharing how LLMs have revolutionized creating educational materials and visualizations. There is also humorous commentary comparing Tao's use of these tools to a Michelin-starred chef using a microwave, and a balanced perspective noting these tools are best for non-critical, supplementary tasks rather than core work.

**Tags**: `#AI coding agents`, `#LLM applications`, `#software development`, `#education technology`, `#Terence Tao`

---

<a id="item-3"></a>
## [Ghostel: A new terminal emulator for Emacs powered by libghostty.](https://dakra.github.io/ghostel/) ⭐️ 8.0/10

Ghostel is a new terminal emulator package for Emacs that uses the libghostty library, aiming to offer improved performance and features compared to existing options like vterm. It provides Emacs users with a potentially faster and more reliable terminal emulation experience, which is critical for developers who rely on terminal workflows within their editor. The project is maintained on GitHub and includes a feature comparison with vterm and another emulator called 'eat'. Users report noticeably faster performance with TUI apps, but note some early-stage issues like occasional clearing glitches and freezes.

hackernews · signa11 · Jul 12, 08:52 · [Discussion](https://news.ycombinator.com/item?id=48879504)

**Background**: Ghostty is a modern terminal emulator, and libghostty is its embeddable library designed to let other applications integrate a full-featured terminal. Within Emacs, terminal emulators like vterm allow users to run shell commands without leaving the editor, but they can have performance or compatibility limitations.

<details><summary>References</summary>
<ul>
<li><a href="https://mitchellh.com/writing/libghostty-is-coming">Libghostty Is Coming – Mitchell Hashimoto</a></li>
<li><a href="https://github.com/emacsmirror/vterm">GitHub - emacsmirror/ vterm : Fully-featured terminal emulator · GitHub</a></li>

</ul>
</details>

**Discussion**: The maintainer provided context and comparison links, while early adopters are enthusiastic, with one user calling it 'amazing' and a potential daily driver. However, users also pointed out practical questions about input mode handling and noted some rough edges like occasional freezes.

**Tags**: `#emacs`, `#terminal-emulator`, `#tools`, `#open-source`, `#performance`

---

<a id="item-4"></a>
## [Zer0Fit packages Google's TabFM and TimesFM as a local MCP server for zero-shot ML.](https://www.reddit.com/r/MachineLearning/comments/1uue8cc/zer0fit_i_took_googles_new_tabfm_timesfm_ml/) ⭐️ 8.0/10

A developer created Zer0Fit, a Docker-based MCP server that wraps Google's new TabFM and TimesFM foundation models, enabling zero-shot forecasting, classification, and regression tasks from chat interfaces like Open WebUI. This project simplifies the integration of powerful, zero-shot ML foundation models into developer workflows, potentially democratizing access to high-performance machine learning without the need for extensive model training or hyperparameter tuning expertise. The server requires an NVIDIA GPU with at least 16GB of VRAM and is CUDA-only, with dynamic model loading and a 5-minute TTL to manage memory; it showed strong zero-shot performance, achieving 94.7% accuracy on the Iris dataset and an R2 of 0.91 on regression tests.

reddit · r/MachineLearning · /u/Porespellar · Jul 12, 12:32

**Background**: TabFM is a recently released foundation model from Google Research designed for zero-shot classification and regression on tabular data, functioning similarly to a large language model but for tables. TimesFM is a time-series forecasting foundation model pretrained on a massive dataset of over 100 billion real-world time-points. MCP (Model Context Protocol) is an open standard that allows AI applications like LLMs to connect to external tools, data sources, and workflows.

<details><summary>References</summary>
<ul>
<li><a href="https://research.google/blog/introducing-tabfm-a-zero-shot-foundation-model-for-tabular-data/">Introducing TabFM : A zero-shot foundation model for tabular data</a></li>
<li><a href="https://research.google/blog/a-decoder-only-foundation-model-for-time-series-forecasting/">A decoder-only foundation model for time-series forecasting</a></li>
<li><a href="https://modelcontextprotocol.io/">What is the Model Context Protocol ( MCP )? - Model Context Protocol</a></li>

</ul>
</details>

**Tags**: `#foundation-models`, `#machine-learning`, `#MCP-server`, `#zero-shot-learning`, `#Docker`

---

<a id="item-5"></a>
## [Chromium's Math.tanh() Becomes a Fingerprinting Vector Exposing the User's OS](https://scrapfly.dev/posts/browser-math-os-fingerprint/) ⭐️ 7.0/10

Since Chromium version 148, the V8 JavaScript engine computes the Math.tanh() function using the host operating system's native libm library instead of a bundled routine, causing its output to vary by OS and create a unique fingerprint. This creates a new, subtle browser fingerprinting technique that can help anti-bot systems identify users or detect inconsistencies, such as a spoofed User-Agent header claiming a different OS than the one actually running. Math.tanh is currently the only Math.* function in Chromium that leaks the OS through its calculation result, and this asymmetry itself can be used as a checkable signal. The behavior has been confirmed on recent glibc versions, which use the correctly rounded tanh implementation from the CORE-MATH project, making the fingerprints even more OS-version specific.

hackernews · joahnn_s · Jul 12, 21:12 · [Discussion](https://news.ycombinator.com/item?id=48884853)

**Background**: Browser fingerprinting is a technique used to track or identify users based on unique combinations of their browser and device characteristics, such as screen resolution, installed fonts, and canvas rendering. The IEEE 754 standard defines how floating-point arithmetic should be performed, but different operating systems and mathematical libraries (like libm) can have slight variations in the implementation of transcendental functions like tanh(), leading to minute differences in results. Chromium's V8 engine is the JavaScript runtime that powers Google Chrome and many other browsers.

<details><summary>References</summary>
<ul>
<li><a href="https://scrapfly.dev/posts/browser-math-os-fingerprint/">Your Browser Does Math Differently on Every OS, and Anti-Bot...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Floating-point_arithmetic">Floating-point arithmetic - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community discussion includes skepticism about the article's origin, with one commenter suggesting it was AI-generated to promote the security company's services. Others highlight that this issue underscores the push for correctly rounded transcendental functions, noting that modern glibc already implements this for tanh. A few commenters also point out that most fingerprinting solutions focus on unique signals rather than OS detection, making this technique's practical impact debatable.

**Tags**: `#browser-fingerprinting`, `#security`, `#javascript`, `#floating-point`, `#chromium`

---

<a id="item-6"></a>
## [Local resistance to AI data center expansion marks a new societal conflict.](https://www.theverge.com/column/963346/ai-data-centers-fight) ⭐️ 7.0/10

A newsletter article from The Verge frames the growing local and environmental opposition to the rapid construction of AI data centers as the beginning of a significant societal struggle. This emerging conflict highlights the tangible local impacts, such as strain on power grids and community resources, driven by the massive infrastructure demands of the AI industry, signaling potential policy and regulatory battles ahead. The piece notes that resistance began years before the current AI boom threatened local power grids, indicating that concerns over data center footprints are not new but are now intensifying.

rss · The Verge - AI · Jul 12, 12:00

**Background**: AI data centers require enormous amounts of electricity for computation and cooling, often drawing power from local grids and consuming significant water resources. The global rush to build AI capabilities has led to a boom in constructing these large-scale facilities, frequently in locations chosen for cheap land and power, sometimes with limited initial community consultation.

**Tags**: `#AI infrastructure`, `#data centers`, `#environmental impact`, `#local policy`, `#tech backlash`

---

<a id="item-7"></a>
## [97 Chinese Embodied AI Data Firms Raised 4.47B Yuan in One Year](https://36kr.com/p/3892027841362694?f=rss) ⭐️ 7.0/10

An industry survey identified 97 Chinese companies in the embodied data sector, with 15 pure data service providers raising approximately 4.47 billion yuan over the past year (July 2025 to July 2026). This analysis reveals that embodied data has matured into an independent industry track, crucial for training robots and embodied AI models, though its funding scale is still modest compared to investments in 'brain' model companies. Data collection methods are categorized into four main routes: real-machine teleoperation, body-less collection, simulation synthesis, and internet video distillation, with the majority of companies pursuing a multi-route strategy to meet diverse training needs.

rss · 36kr - AI · Jul 12, 02:16

**Background**: Embodied AI refers to intelligent systems that perceive and act through a physical body, requiring massive amounts of real-world interaction data for training. The 'data pyramid' concept illustrates that different data types (real, simulated, web-derived) are needed at various stages, and the 'sim-to-real' gap—where simulated data fails to perfectly replicate real-world physics—remains a key challenge driving demand for diverse data sources.

<details><summary>References</summary>
<ul>
<li><a href="https://tech.ifeng.com/c/8uh5s4oHQ2h">tech.ifeng.com/c/8uh5s4oHQ2h</a></li>

</ul>
</details>

**Tags**: `#embodied AI`, `#data collection`, `#robotics`, `#industry analysis`, `#funding trends`

---

<a id="item-8"></a>
## [UK Unveils £2 Billion Plan for AI Combat Laboratory](https://36kr.com/newsflashes/3892413575559941?f=rss) ⭐️ 7.0/10

The UK Ministry of Defence announced a £2 billion investment to establish an AI combat laboratory, aiming to modernize military training and reshape exercises using intelligent technology. This substantial government investment underscores the strategic importance of AI in modern warfare and aims to bolster the UK's domestic defense industry and create technical jobs. The project will be executed by a consortium of domestic defense companies, involve numerous local suppliers, and include a youth technical apprenticeship program and pathways for veterans into technical employment.

rss · 36kr - AI · Jul 12, 09:32

**Background**: Globally, militaries are increasingly integrating AI to enhance training realism, accelerate decision-making, and analyze vast operational data for a strategic advantage. AI-driven simulations can adapt scenarios in real-time and provide scalable, personalized training, representing a significant shift in defense modernization.

<details><summary>References</summary>
<ul>
<li><a href="https://breakingdefense.com/2025/10/ai-in-the-loop-transforming-military-training-and-system-design-through-smarter-simulation/">AI in the loop: Transforming military training and system design through smarter simulation - Breaking Defense</a></li>
<li><a href="https://www.fmj.co.uk/vivo-defence-launches-data-and-ai-apprenticeships-with-multiverse/">VIVO Defence launches data and AI apprenticeships with Multiverse</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Defense`, `#Government Investment`, `#Military AI`, `#UK`

---

<a id="item-9"></a>
## [Apple's Failed Car Project Boosted Its Powerful AI Chip Development](https://www.theverge.com/tech/964519/apple-silicon-self-driving-car-ai-m7-ultra) ⭐️ 6.0/10

Apple's abandoned self-driving car program, Project Titan, directly accelerated the development of the company's powerful on-device AI processors, even though the vehicle itself was never completed. This highlights how failed ambitious R&D initiatives can yield significant, successful technological spin-offs that strengthen a company's core products and competitive position in the broader market. The self-driving platform required powerful on-device AI processing for real-time decision-making, which drove innovations that later benefited Apple Silicon chips like the M-series, though the specific car processor was never finalized.

rss · The Verge - AI · Jul 12, 16:27

**Background**: Apple's secret self-driving car project, known internally as Project Titan, began around 2014 and was officially canceled in 2024 after a decade of work and multiple leadership changes. On-device AI processing is critical for autonomous vehicles to analyze sensor data and make real-time driving decisions without relying on cloud connectivity. Apple's Neural Engine is a dedicated Neural Processing Unit (NPU) integrated into its Apple Silicon chips to accelerate machine learning tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Apple_car_project">Apple car project - Wikipedia</a></li>
<li><a href="https://apple.fandom.com/wiki/Neural_Engine">Neural Engine | Apple Wiki | Fandom</a></li>
<li><a href="https://objectways.com/blog/boosting-the-situational-awareness-of-self-driving-cars-using-ai/">AI for Smarter Situational Awareness in Self-Driving Cars</a></li>

</ul>
</details>

**Tags**: `#apple-silicon`, `#ai-chips`, `#self-driving-cars`, `#technology-history`, `#corporate-rd`

---

<a id="item-10"></a>
## [Anthropic Clarifies Claude Code's Model vs. Effort Level Confusion](https://36kr.com/p/3892222176574211?f=rss) ⭐️ 6.0/10

Anthropic officially published guidance explaining that many Claude Code users incorrectly conflate 'Model' selection with 'Effort' level, leading to unnecessary upgrades to larger models like Fable when adjusting effort settings would be more effective. This clarification helps users optimize costs and performance in AI-assisted coding by understanding how to properly configure Claude Code for their specific tasks, potentially improving efficiency across the developer ecosystem. The 'Model' setting changes the underlying AI's frozen weights and capabilities, while the 'Effort' level controls how much work Claude undertakes, such as reading files or running tests; a high-effort smaller model can outperform a low-effort larger one.

rss · 36kr - AI · Jul 12, 05:47

**Background**: Claude Code is Anthropic's AI coding assistant that lets developers interact with Claude models via a command-line interface, and it includes settings for model selection (e.g., Fable) and effort levels (from low to xhigh). In March 2026, Anthropic temporarily changed the default effort level from high to medium to reduce latency, causing user complaints about degraded performance before reverting it in April.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.bswen.com/blog/2026-03-13-claude-code-effort-settings/">How to Set Claude Code Effort Level : CLI Flags... | BSWEN</a></li>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://www.sitepoint.com/claude-code-21-the-complete-xhigh-and-autoverification-guide-2026/">Claude Code 2.1: The Complete xHigh and Auto-Verification Guide...</a></li>

</ul>
</details>

**Discussion**: The article references GitHub complaints and criticism from figures like AMD's AI lead Stella Laurenzo, who measured a 67% drop in Claude's thinking effort, indicating significant user frustration with the stealth change. This highlights a broader community concern about transparency in AI tool updates.

**Tags**: `#AI_models`, `#optimization`, `#user_experience`, `#Anthropic`, `#Claude_Code`

---

<a id="item-11"></a>
## [AI Boom Triples Gas Turbine Prices Over Three Years](https://36kr.com/newsflashes/3892556678543880?f=rss) ⭐️ 6.0/10

The price of gas turbines has increased by approximately 300% over the past three years, driven by surging demand from AI data centers, with major companies like Microsoft securing large orders from suppliers like GE Vernova. This price surge highlights how the AI boom is creating severe bottlenecks in energy infrastructure supply chains, significantly impacting the cost and feasibility of building the massive data centers required for AI training and inference. Microsoft recently ordered seven large gas turbines from GE Vernova for its Texas data centers, with each unit costing over $250 million, indicating that demand continues to far outstrip supply despite the high cost.

rss · 36kr - AI · Jul 12, 11:37

**Background**: Gas turbines are critical components for generating reliable, on-demand power for large data centers, especially in regions like the US where grid capacity may lag behind demand. The AI boom has accelerated the construction of these power-hungry facilities, straining the supply chain for turbine manufacturers like GE Vernova, Siemens, and Caterpillar.

<details><summary>References</summary>
<ul>
<li><a href="https://wap.stockstar.com/detail/IG2026020900020061">北美“ 电 荒”， 燃 气 轮 机 成AI基建，联德股份迎市场红利-证券之星</a></li>
<li><a href="https://news.fx168news.com/cooperate/2507/7346700.shtml">GE Vernova ：AI热潮下 的 能 源 新王-FX168财经网</a></li>

</ul>
</details>

**Tags**: `#AI`, `#energy`, `#infrastructure`, `#supply-chain`, `#data-centers`

---

<a id="item-12"></a>
## [Changxin Memory Tech's IPO Set to Be Largest A-Share Listing This Year](https://36kr.com/newsflashes/3892554879515140?f=rss) ⭐️ 6.0/10

Changxin Memory Technologies is scheduled to launch its online subscription for its STAR Market IPO on July 16, aiming to raise 29.5 billion yuan, which would be the largest A-share IPO of the year. This IPO represents a major capital infusion for China's domestic semiconductor industry, specifically targeting DRAM memory chip production, which is crucial for reducing foreign dependency and advancing the nation's AI and computing sectors. The IPO involves 167.2 million shares available for online subscription, requiring a Shanghai market value of 16.72 million yuan for the maximum application, and is projected to have a relatively high lottery win rate due to its large share issuance volume.

rss · 36kr - AI · Jul 12, 11:18

**Background**: Changxin Memory Technologies is a key player in China's push for semiconductor self-sufficiency, focusing on DRAM memory chips used in devices like computers and smartphones. The STAR Market is Shanghai's Nasdaq-style tech board that uses a registration-based listing system, designed to facilitate fundraising for innovative companies. Memory chips are a strategic commodity, as their supply security is increasingly seen as critical for the development of AI and other advanced technologies.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tuoluo.cn/article/detail-10128903.html">从百亿巨亏到千亿净利，爆红的 长 鑫 科 技 是如何炼成的？_ 陀螺 科 技</a></li>
<li><a href="https://en.wikipedia.org/wiki/Shanghai_Stock_Exchange_STAR_Market">Shanghai Stock Exchange STAR Market - Wikipedia</a></li>
<li><a href="https://laoyaoba.com/n/984247">算力争霸战打响！ 2026全球博弈， 存 储 芯 片 成必争战略高地</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#IPO`, `#A-share market`, `#memory chips`, `#China tech`

---