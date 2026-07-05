---
layout: default
title: "Horizon Summary: 2026-07-05 (EN)"
date: 2026-07-05
lang: en
---

> From 66 items, 10 important content pieces were selected

---

1. [Huawei releases V2 of Tao's Law paper with engineering details and test data.](#item-1) ⭐️ 9.0/10
2. [Prompt Injection Bug in YouTube AI Could Leak Creators' Private Videos](#item-2) ⭐️ 8.0/10
3. [More Capable Language Models May Perform Worse at Tool Calling](#item-3) ⭐️ 8.0/10
4. [Potential Session Data Leakage Reported Between LLM User Accounts](#item-4) ⭐️ 8.0/10
5. [AI Model Claude Fable Drives sqlite-utils 4.0rc2 Release](#item-5) ⭐️ 8.0/10
6. [GPT-5.5 Codex regression traced to reasoning-token clustering at 516.](#item-6) ⭐️ 7.0/10
7. [USAF: Open-Source Sparse Fine-Tuning for MoE Models on Consumer GPUs](#item-7) ⭐️ 7.0/10
8. [Fanfiction community splits over AI detection methods and false accusations.](#item-8) ⭐️ 6.0/10
9. [Semiconductor and AI Trends Drive Growth for Chinese Fluorine New Materials](#item-9) ⭐️ 6.0/10
10. [Micron Invests $9.3 Billion to Expand Hiroshima Plant for AI Memory Chips](#item-10) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Huawei releases V2 of Tao's Law paper with engineering details and test data.](https://36kr.com/newsflashes/3880931591254019?f=rss) ⭐️ 9.0/10

Huawei's semiconductor head He Tingbo released Version 2 of the 'Tao's Law' paper, which adds extensive engineering implementation details, real-world quantitative data, and a production roadmap for the time constant (τ) scaling theory. The update introduces the 'LogicFolding' technique with its 'gear ratio' concept for 3D chip design and provides specific performance parameters for the Kirin 2026 chip. This update strengthens Huawei's proposed paradigm shift for post-Moore's Law semiconductor scaling by moving from theoretical framework to practical engineering validation with real chip data, potentially guiding a new architectural path for advanced chip design. It presents a concrete roadmap for next-generation chips, challenging the industry's traditional reliance on geometric scaling. A key technical detail is the 'LogicFolding' architecture, which uses a 'gear ratio' to optimize vertical logic partitioning, shifting 3D design from 'macro-block-level discrete optimization' to 'unit-level continuous optimization' when hybrid bonding pitch approaches top-metal routing dimensions. The paper includes a new data table for the Kirin 2026 chip, specifying voltage, frequency, normalized power consumption, area, and power density parameters against a Kirin 9030 Pro baseline.

rss · 36kr - AI · Jul 4, 06:35

**Background**: Moore's Law, the observation that the number of transistors on a chip doubles approximately every two years, has guided the semiconductor industry for decades but is approaching physical and economic limits. The 'Tao's Law' is Huawei's proposed alternative framework for post-Moore scaling, using the time constant (τ) as a new universal metric to optimize system performance across hierarchical levels, from devices to entire systems. LogicFolding is a 3D chip design technique that vertically stacks active logic layers using through-silicon vias and hybrid bonding to shorten signal paths, reducing delay and power consumption.

<details><summary>References</summary>
<ul>
<li><a href="https://www.huawei.com/en/news/2026/5/ieee-iscas-tau-scaling">HUAWEI Presents the Tau (τ) Scaling Law, Enabling ...</a></li>
<li><a href="https://d-sci.org/index.php/dsci/article/view/40">A Formal Investigation of Tau (τ) Scaling Theory for Multi ...</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/semiconductors/peking-university-builds-3d-chip-design-tool-tailored-to-huaweis-logicfolding-architecture">Chinese university builds 3 D chip design tool... | Tom's Hardware</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#chip-design`, `#3D-stacking`, `#Huawei`, `#post-Moore-Law`

---

<a id="item-2"></a>
## [Prompt Injection Bug in YouTube AI Could Leak Creators' Private Videos](https://javoriuski.com/post/youtube) ⭐️ 8.0/10

A security researcher disclosed a prompt injection vulnerability in YouTube's AI-powered comment suggestion feature, where an attacker's malicious comment can cause the AI to leak details about a creator's private, unlisted videos when the creator uses the feature in YouTube Studio. This vulnerability highlights a fundamental and practical security flaw in integrating LLMs into user-facing products, potentially compromising creator privacy and platform trust, and underscores the systemic challenge of defending against prompt injection attacks. The attack requires a multi-step social engineering chain: an attacker must post a crafted comment on a creator's video, and the creator must then voluntarily click YouTube's suggested AI prompt to summarize comments in YouTube Studio. The vulnerability exploits the lack of clear role boundaries between user-provided comments and system instructions in the AI's processing.

hackernews · javxfps · Jul 4, 16:45 · [Discussion](https://news.ycombinator.com/item?id=48786781)

**Background**: Prompt injection is a known class of security vulnerability in Large Language Model (LLM) applications where malicious instructions embedded in user input can hijack the model's behavior. YouTube's AI comment suggestion feature is designed to help creators efficiently manage and respond to large volumes of comments by generating draft replies or summaries. A critical security principle for such systems is to strictly separate untrusted user input from trusted system prompts, a principle this vulnerability appears to violate.

<details><summary>References</summary>
<ul>
<li><a href="https://genai.owasp.org/llmrisk/llm01-prompt-injection/">LLM01:2025 Prompt Injection - OWASP Gen AI Security Project</a></li>
<li><a href="https://www.hackerone.com/ai/prompt-injection-deep-dive">AI Prompt Injection : Vulnerability , Impact, and Remediation</a></li>

</ul>
</details>

**Discussion**: The community discussion shows significant engagement, with a former Google engineer suggesting YouTube's handling may be influenced by internal performance review structures rather than pure security triage. Many commenters express disbelief that YouTube does not classify prompt injection as a bug, while others praise the researcher's clear and factual disclosure style.

**Tags**: `#security-vulnerability`, `#prompt-injection`, `#youtube`, `#ai-security`, `#privacy`

---

<a id="item-3"></a>
## [More Capable Language Models May Perform Worse at Tool Calling](https://lucumr.pocoo.org/2026/7/4/better-models-worse-tools/) ⭐️ 8.0/10

The article identifies a paradox where increasingly capable large language models (LLMs) show degraded performance in tool-calling tasks, such as generating incorrect syntax or inventing fields, which challenges the assumption that general model improvement translates to better specialized tool integration. This issue is significant because reliable tool-calling is fundamental for building practical AI agents and developer tools, and its degradation directly impacts the cost, latency, and reliability of LLM-powered applications. The article highlights that models trained in 'forgiving' runtimes may learn to invent interface details, causing problems when integrated with strict external systems, and that alternative approaches like providing clear error guidance or using standardized interfaces like `curl` can mitigate the issue.

hackernews · leemoore · Jul 4, 20:16 · [Discussion](https://news.ycombinator.com/item?id=48788599)

**Background**: Tool calling (or function calling) refers to the ability of an LLM to generate structured commands, like API requests, to interact with external tools and services. This capability is essential for creating AI agents that can perform actions in the real world, such as querying databases or controlling software. As models are trained primarily on vast text corpora, their proficiency in following precise, often idiosyncratic, tool-specific schemas does not necessarily scale with their general reasoning power.

<details><summary>References</summary>
<ul>
<li><a href="https://dev.to/amartyajha/how-poor-tool-calling-behavior-increases-llm-cost-and-latency-3idf">How Poor Tool Calling Behavior Increases LLM Cost and Latency</a></li>
<li><a href="https://a16z.com/emerging-architectures-for-llm-applications/">Emerging Architectures for LLM Applications - Andreessen Horowitz</a></li>
<li><a href="https://www.ibm.com/think/topics/ai-agents">What Are AI Agents ? | IBM</a></li>

</ul>
</details>

**Discussion**: Developers shared practical solutions, emphasizing that clear, helpful error messages are a simple and effective fix that allows the model to self-correct within a session. Others advocated for using well-known, standardized interfaces like `curl` commands over complex, custom protocols like MCP for more reliable integration. A commenter also noted that this creates a potential economic moat, as fine-tuning models on specific closed-source harnesses can lock users into particular ecosystems.

**Tags**: `#LLM`, `#tool-calling`, `#software-engineering`, `#AI-agents`, `#developer-tools`

---

<a id="item-4"></a>
## [Potential Session Data Leakage Reported Between LLM User Accounts](https://github.com/anthropics/claude-code/issues/74066) ⭐️ 8.0/10

A GitHub issue and Hacker News discussion have surfaced community reports of potential session or cache data being swapped or leaked between different user accounts on major LLM platforms like Claude and GPT. The issue highlights specific anecdotes where API infrastructure allegedly caused response mix-ups. This is significant because it raises critical security and privacy concerns for the rapidly growing multi-tenant LLM industry, potentially eroding user trust if sensitive data can leak across organizational boundaries. Such incidents could impact enterprise adoption and demand stricter data isolation protocols from providers. While the reports are based on user anecdotes and have not been officially confirmed as widespread vulnerabilities, a Claude Code team member responded by stating they are confident the specific incident reported was a hallucination but that the team is investigating. The discussion references potential causes like API gateway errors handling HTTP status codes or cache collisions.

hackernews · chatmasta · Jul 4, 14:03 · [Discussion](https://news.ycombinator.com/item?id=48785485)

**Background**: Large Language Model (LLM) providers often deploy multi-tenant architectures where a single infrastructure serves many users or organizations, making proper data isolation a fundamental security requirement. Techniques like prompt caching are used to improve performance, but if not implemented with strict tenant boundaries, they can create risks for data leakage. Ensuring that one customer's data or context never bleeds into another's session is a critical, non-negotiable aspect of production LLM system design.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@michael.hannecke/llm-prompt-caching-what-you-should-know-2665d76d3d8d">LLM Prompt Caching: Performance and Security Guide | Medium</a></li>
<li><a href="https://www.thedataexperts.us/work/secure-multi-tenant-llm-platform-framework.html">Secure Multi-Tenant LLM Platform: A Build-and-Transfer…</a></li>
<li><a href="https://aws.amazon.com/blogs/machine-learning/multi-tenant-llm-analytics-with-row-level-security-how-we-built-a-secure-agent-on-aws/">Multi-tenant LLM analytics with row-level security: How we built a secure agent on AWS | Artificial Intelligence</a></li>

</ul>
</details>

**Discussion**: The community discussion is divided between skepticism and concern; some users believe the reports are likely hallucinations or context-related artifacts, while others share corroborating personal experiences of seeing anomalous, out-of-context responses that seemed meant for other users. A member of the Claude Code team officially responded to clarify they are investigating but lean towards the hallucination explanation for the specific report.

**Tags**: `#AI/ML security`, `#LLM infrastructure`, `#data privacy`, `#system reliability`

---

<a id="item-5"></a>
## [AI Model Claude Fable Drives sqlite-utils 4.0rc2 Release](https://simonwillison.net/2026/Jul/5/sqlite-utils-fable/#atom-everything) ⭐️ 8.0/10

Simon Willison used Claude Fable to perform a final code review of sqlite-utils 4.0rc1, identifying 5 'release-blocking' bugs over 37 prompts and 34 commits, leading to the 4.0rc2 release. This demonstrates a practical, cost-effective use of AI in a real-world open-source software release process, potentially validating AI as a tool for high-stakes code review and bug discovery. The process involved +1,321 -190 lines of code changes across 30 files, and one critical bug found was that `delete_where()` could cause data loss by poisoning the database connection.

rss · Simon Willison · Jul 5, 01:00

**Background**: sqlite-utils is a popular Python library and CLI for working with SQLite databases. Semantic Versioning (SemVer) is a versioning scheme where a major version increment signifies incompatible API changes, making major releases significant and rare for maintainers. Claude Fable is an advanced AI model from Anthropic.

<details><summary>References</summary>
<ul>
<li><a href="https://semver.org/">Semantic Versioning 2.0.0 | Semantic Versioning</a></li>
<li><a href="https://github.com/simonw/sqlite-utils">GitHub - simonw/sqlite-utils: Python CLI utility and library ...</a></li>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#AI-assisted development`, `#SQLite`, `#open-source`, `#software release`, `#Claude AI`

---

<a id="item-6"></a>
## [GPT-5.5 Codex regression traced to reasoning-token clustering at 516.](https://github.com/openai/codex/issues/30364) ⭐️ 7.0/10

Users have identified a reproducible performance regression in GPT-5.5 Codex where the model's reasoning process clusters around exactly 516 tokens, leading to incorrect outputs. When the model uses significantly more thinking tokens (6000-8000), it returns the correct result. This issue undermines the reliability of a major AI coding assistant, directly affecting developers' productivity and trust in automated coding tools. It highlights ongoing challenges with LLM consistency and the risks of silent, server-side changes in commercial AI services. The regression appears related to an 'adaptive thinking' mechanism, where short reasoning paths yield wrong answers while longer paths are correct. Some users report that this issue has persisted for months and have switched to alternative models like Claude as a workaround.

hackernews · maille · Jul 4, 21:51 · [Discussion](https://news.ycombinator.com/item?id=48789428)

**Background**: OpenAI Codex is an AI system designed to generate code, and its performance is often measured by the accuracy and efficiency of its outputs. Token clustering in this context likely refers to the model allocating a fixed, potentially suboptimal, number of computational 'thinking' tokens for a task. Performance regressions in such tools can be caused by internal model updates or changes in inference infrastructure.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48749961">Codex reasoning - token clustering at 516 may be... | Hacker News</a></li>
<li><a href="https://community.openai.com/t/severe-regression-in-gpt-5-codex-performance/1358412">Severe regression in GPT-5 Codex performance - Codex - OpenAI ...</a></li>
<li><a href="https://github.com/openai/codex/issues/6835">Significant Performance Regression in Codex from v0.4.39 ...</a></li>

</ul>
</details>

**Discussion**: The community confirms the regression is easily reproducible, with many reporting daily quality jumps and have already switched to alternatives like Claude due to OpenAI's lack of response. Some compare it to past regressions in competing products and debate using per-token pricing or local models to avoid such silent server-side issues.

**Tags**: `#GPT-5.5`, `#AI coding`, `#performance regression`, `#OpenAI Codex`, `#LLM reliability`

---

<a id="item-7"></a>
## [USAF: Open-Source Sparse Fine-Tuning for MoE Models on Consumer GPUs](https://www.reddit.com/r/MachineLearning/comments/1unl62q/if_your_gpu_can_run_inference_it_should_be_able/) ⭐️ 7.0/10

A new open-source method called USAF enables fine-tuning of large Mixture-of-Experts models by training only the expert weights and the router, demonstrated on a consumer AMD GPU with 12GB VRAM. This method significantly lowers the hardware barrier for fine-tuning large, state-of-the-art MoE models, potentially democratizing access to model customization for researchers and developers without enterprise-grade hardware. The project is released under the Apache 2.0 license and specifically targets sparse expert weights and the router, which is a different approach compared to common adapter-based methods like LoRA.

reddit · r/MachineLearning · /u/tsuyu122 · Jul 4, 21:56

**Background**: Mixture-of-Experts (MoE) models use a sparse architecture where a router network selects a subset of specialized expert subnetworks (the 'experts') for each input, allowing for a large total parameter count while keeping computation manageable. Fine-tuning such models is challenging because standard techniques often require updating all parameters or adding adapters to the entire dense structure. The USAF method focuses on updating only the expert weights and the router itself, leveraging the model's inherent sparsity to reduce memory and compute requirements.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>
<li><a href="https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-mixture-of-experts">A Visual Guide to Mixture of Experts (MoE)</a></li>
<li><a href="https://www.ibm.com/think/topics/mixture-of-experts">What is mixture of experts? | IBM</a></li>

</ul>
</details>

**Tags**: `#Mixture-of-Experts`, `#Fine-tuning`, `#Open-Source`, `#GPU-Inference`, `#Machine-Learning`

---

<a id="item-8"></a>
## [Fanfiction community splits over AI detection methods and false accusations.](https://www.theverge.com/tech/960854/ai-fanfiction-ao3-claude-detector) ⭐️ 6.0/10

A new movement within the fanfiction community is actively trying to identify and exclude authors using generative AI tools like Claude and ChatGPT, but the detection methods being implemented are questionable and risk causing false accusations against human writers. This conflict highlights the tension between preserving human creativity and adopting new technology, with flawed detection tools potentially silencing legitimate writers and damaging trust within creative communities. The community's response has created internal divisions, as the broad rejection of AI tools like Claude and ChatGPT is being enforced through detection methods that are prone to error, meaning any fanfic writer could be wrongly accused.

rss · The Verge - AI · Jul 4, 12:00

**Background**: Generative AI can create text, code, and images, and AI detection tools use methods like analyzing text patterns or statistical likelihood to guess if content was machine-written, though they often struggle with false positives—incorrectly flagging human work as AI. Fanfiction communities, centered on platforms like Archive of Our Own (AO3), value original human expression, making the introduction of AI a point of significant cultural and ethical conflict.

<details><summary>References</summary>
<ul>
<li><a href="https://www.grammarly.com/blog/ai/how-do-ai-detectors-work/">How Do AI Detectors Work? Key Methods and Limitations | Grammarly</a></li>
<li><a href="https://lawlibguides.sandiego.edu/c.php?g=1443311&p=10721367">The Problems with AI Detectors: False Positives and False Negatives - Generative AI Detection Tools - Guides at University of San Diego Legal Research Center</a></li>

</ul>
</details>

**Tags**: `#AI ethics`, `#creative writing`, `#content detection`, `#community conflict`, `#generative AI`

---

<a id="item-9"></a>
## [Semiconductor and AI Trends Drive Growth for Chinese Fluorine New Materials](https://36kr.com/newsflashes/3882063262068998?f=rss) ⭐️ 6.0/10

A research report from Everbright Securities identifies that leading Chinese fluorine chemical companies are accelerating their expansion into high-value fluorine new materials, creating a second growth curve driven by breakthroughs in semiconductor-grade hydrofluoric acid and liquid cooling fluids for AI infrastructure. This shift is significant as it enables domestic companies to break foreign monopolies in critical semiconductor supply chains and positions them to capitalize on the rapidly growing demand for advanced thermal management solutions in AI and high-performance computing data centers. Domestic producers have achieved G5-grade electronic hydrofluoric acid with PPT-level purity, passing certification from top foundries, while fluorine chemical firms are developing perfluoropolyether (PFPE) coolants essential for immersion liquid cooling systems due to their superior insulation and thermal properties.

rss · 36kr - AI · Jul 5, 01:18

**Background**: Electronic-grade hydrofluoric acid is a key wet chemical essential for semiconductor manufacturing, and G5 is the highest purity standard. Immersion liquid cooling is an advanced thermal management technique where components are submerged in a non-conductive fluid, becoming crucial for cooling high-power AI chips and data centers as traditional air cooling reaches its limits.

<details><summary>References</summary>
<ul>
<li><a href="https://www.toutiao.com/article/7644957391921873427/">半导体“工业味精”G5级氢氟酸：硬核技术壁垒与国产替代</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/1945118179559998489">全氟碳化合物（如全氟聚醚PFPE）作为浸没式液冷系统的核心冷却液</a></li>
<li><a href="https://www.eet-china.com/mp/a480686.html">2026最新湿电子化学品产业发展报告深度解读（建议收藏）</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#materials-science`, `#AI-infrastructure`, `#industry-analysis`, `#fluorochemistry`

---

<a id="item-10"></a>
## [Micron Invests $9.3 Billion to Expand Hiroshima Plant for AI Memory Chips](https://36kr.com/newsflashes/3882061184413701?f=rss) ⭐️ 6.0/10

Micron Technology has begun construction on a $9.3 billion (1.5 trillion yen) expansion of its Hiroshima, Japan plant to produce advanced memory chips, including High Bandwidth Memory (HBM) for AI applications, with initial shipments expected around the summer of 2028. This major investment directly supports the global AI hardware supply chain, as HBM is a critical component for high-performance AI processors like those from NVIDIA, and it reflects the intense competition among memory giants (Micron, Samsung, SK Hynix) to expand capacity for the AI boom. The expansion project carries a total investment of 1.5 trillion yen ($9.3 billion), and the Hiroshima facility is specifically designated to produce HBM, which is essential for AI accelerators; this announcement comes shortly after SK Hynix revealed its own plan to invest $51.46 billion in a new NAND plant in South Korea.

rss · 36kr - AI · Jul 5, 01:16

**Background**: High Bandwidth Memory (HBM) is a high-performance memory interface that uses 3D stacking of DRAM chips connected with through-silicon vias (TSVs) to achieve much higher bandwidth and power efficiency than traditional memory, making it vital for AI and high-performance computing. Major memory chip manufacturers are currently in an intense investment cycle to expand advanced production capacity to meet soaring demand driven by artificial intelligence applications.

<details><summary>References</summary>
<ul>
<li><a href="https://theoutpost.ai/news-story/micron-technology-breaks-ground-on-9-3-billion-hiroshima-plant-expansion-for-ai-memory-chips-28213/">Micron Technology $9.3B Hiroshima Plant Expansion</a></li>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#HBM`, `#AI hardware`, `#investment`, `#manufacturing`

---