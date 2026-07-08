---
layout: default
title: "Horizon Summary: 2026-07-08 (EN)"
date: 2026-07-08
lang: en
---

> From 111 items, 16 important content pieces were selected

---

1. [TypeScript 7.0 Delivers 8-12x Faster Compilation Speed](#item-1) ⭐️ 9.0/10
2. [AI-Assisted Research Uncovers OpenBSD Local Privilege Escalation Flaw](#item-2) ⭐️ 8.0/10
3. [EU Advances Law Mandating Private Message Scanning](#item-3) ⭐️ 8.0/10
4. [Cloudflare Introduces Meerkat, a Globally Distributed Consensus System Based on QuePaxa.](#item-4) ⭐️ 8.0/10
5. [LingBot-Video: A 13B Sparse MoE Model for Action-Conditioned Video Generation](#item-5) ⭐️ 8.0/10
6. [OpenAI Examines Flaws in Coding Benchmark Integrity](#item-6) ⭐️ 7.0/10
7. [OpenAI Publishes Principles for Government and National Security Partnerships](#item-7) ⭐️ 7.0/10
8. [Consumer 3D printing firm Snapmaker secures $140M in sector's largest recent funding round.](#item-8) ⭐️ 7.0/10
9. [AI Biotech Deeper Insights Secures $52M Series B for Phase III GLP-1 Drug](#item-9) ⭐️ 7.0/10
10. [Amazon's Secret 'Moonraker' Project Aims to Evolve Alexa into an AI Agent](#item-10) ⭐️ 7.0/10
11. [Cloudflare and OpenAI Launch Pilot to Enhance AI Search with Global Network Data](#item-11) ⭐️ 7.0/10
12. [OpenAI Announces GPT-Live with Advanced Model Delegation](#item-12) ⭐️ 6.0/10
13. [OpenAI Upgrades ChatGPT Voice Mode for More Natural Conversation](#item-13) ⭐️ 6.0/10
14. [id Software Loses 136 Jobs as Part of Major Xbox Layoffs](#item-14) ⭐️ 6.0/10
15. [Comprehensive Review Ranks Seedance 2.0 as Leading AI Video Tool](#item-15) ⭐️ 6.0/10
16. [Blue Origin Raises $10B at $130B Valuation with Bezos Investing $2B](#item-16) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [TypeScript 7.0 Delivers 8-12x Faster Compilation Speed](https://devblogs.microsoft.com/typescript/announcing-typescript-7-0/) ⭐️ 9.0/10

TypeScript 7.0 has been released, featuring a new compiler architecture that delivers massive performance gains, achieving 8-12x faster build times on large real-world codebases like VS Code and Sentry. This is a major performance breakthrough that will dramatically improve developer experience and productivity, especially for large enterprise-scale projects where long compilation times have been a significant pain point. Benchmarks show specific speedups: the VS Code codebase compiled 11.9x faster (from 125.7s to 10.6s), Sentry 8.9x faster, and Bluesky 8.7x faster. However, early adopters note that compatibility with some common tools like ts-jest may require workarounds initially.

hackernews · DanRosenwasser · Jul 8, 16:06 · [Discussion](https://news.ycombinator.com/item?id=48833715)

**Background**: TypeScript is a popular statically-typed superset of JavaScript that compiles to plain JavaScript. A major version release like 7.0 indicates significant changes to the language or its tooling. Compilation speed has been a critical concern for developers working on large codebases, as slow builds hinder iteration speed and developer productivity.

**Discussion**: The community celebrates the monumental engineering effort, with users sharing impressive benchmark tables and congratulating the team. Discussion also highlights ongoing pain points, such as difficulties configuring tsconfig for mixed environments (e.g., DOM and Node.js) and initial compatibility issues with testing tools like ts-jest. Some comments express hope for a future Rust-based rewrite for even better performance.

**Tags**: `#TypeScript`, `#programming languages`, `#performance`, `#compiler`, `#JavaScript`

---

<a id="item-2"></a>
## [AI-Assisted Research Uncovers OpenBSD Local Privilege Escalation Flaw](https://nvd.nist.gov/vuln/detail/cve-2026-57589) ⭐️ 8.0/10

A use-after-free vulnerability (CVE-2026-57589) was discovered in the OpenBSD kernel's System V semaphore component, which allows a local user to escalate privileges to root. The discovery was notably made through an AI-assisted security research project. This is significant because OpenBSD is renowned for its stringent security focus, and the discovery of a local privilege escalation flaw challenges its reputation. Furthermore, the use of AI in its discovery highlights a potentially transformative new methodology for future vulnerability research. The vulnerability exists in the `sys/kern/sysv_sem.c` file, where a use-after-free condition occurs after a `tsleep` call in the `sys_semget()` function during a context switch. It affects OpenBSD versions through 7.9.

hackernews · linggen · Jul 8, 13:24 · [Discussion](https://news.ycombinator.com/item?id=48831658)

**Background**: OpenBSD is a free, open-source operating system widely recognized for its proactive security practices and clean code design. Use-after-free is a memory safety bug where a program continues to use a pointer after the memory it points to has been freed, which can lead to crashes or arbitrary code execution. AI-assisted security research involves using large language models or other AI tools to help identify potential software vulnerabilities more efficiently than traditional manual methods.

<details><summary>References</summary>
<ul>
<li><a href="https://securityvulnerability.io/vulnerability/CVE-2026-57589">Use-After-Free Vulnerability in OpenBSD Kernel Component CVE-2026-57589</a></li>
<li><a href="https://www.sentinelone.com/vulnerability-database/cve-2024-10934/">CVE-2024-10934: OpenBSD Use-After-Free Vulnerability - SentinelOne</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC11656524/">Advancing cybersecurity and privacy with artificial intelligence: current trends and future research directions - PMC</a></li>

</ul>
</details>

**Discussion**: The community discussion revealed that the vulnerability was found as part of the 'Patch The Planet' project, a collaboration between OpenAI and Trail of Bits using AI models to audit open-source software. Commenters expressed a mix of views: one praised OpenBSD's security culture, noting that finding only one bug is a testament to its diligence, while another wondered about the overall number of vulnerabilities found by AI on such a security-focused system.

**Tags**: `#OpenBSD`, `#security-vulnerability`, `#privilege-escalation`, `#CVE`, `#AI-security-research`

---

<a id="item-3"></a>
## [EU Advances Law Mandating Private Message Scanning](https://cyberinsider.com/eu-now-one-step-away-from-reviving-private-message-scanning-rules/) ⭐️ 8.0/10

The European Union is one legislative step away from passing a regulation that would mandate client-side scanning of private messages, a technology that scans content on a user's device before it is encrypted and sent. This development is highly significant as it could fundamentally undermine end-to-end encryption, a cornerstone of digital privacy, and set a precedent for mass surveillance technology in democratic nations. The legislation, often dubbed 'Chat Control 2.0', would mandate scanning and effectively ban strong end-to-end encryption, a major escalation from previous rules that merely allowed companies to scan if they chose to.

hackernews · ggirelli · Jul 8, 16:53 · [Discussion](https://news.ycombinator.com/item?id=48834296)

**Background**: Client-side scanning (CSS) is a technology where the content of messages is checked against a database of objectionable material on the user's own device before the message is encrypted and transmitted. This is distinct from server-side scanning, which occurs after the message is decrypted by the service provider. The debate pits the desire to combat illegal content like child sexual abuse material (CSAM) against the fundamental right to private communication and the technical integrity of encryption.

<details><summary>References</summary>
<ul>
<li><a href="https://www.internetsociety.org/resources/doc/2020/fact-sheet-client-side-scanning/">Fact Sheet: Client-Side Scanning - Internet Society</a></li>
<li><a href="https://judicature.duke.edu/articles/you-are-being-scanned/">Point-Counterpoint | Client-Side Scanning - Judicature</a></li>

</ul>
</details>

**Discussion**: The community expresses deep concern and frustration, viewing the legislation as 'Terminator legislation' that will persistently return even if temporarily defeated. Commenters clarify the critical distinction between allowing voluntary scanning (Chat Control 1.0) and the mandatory scanning of this new proposal (Chat Control 2.0), and they are actively sharing resources to contact EU representatives to oppose it.

**Tags**: `#privacy`, `#encryption`, `#EU regulation`, `#digital rights`, `#surveillance`

---

<a id="item-4"></a>
## [Cloudflare Introduces Meerkat, a Globally Distributed Consensus System Based on QuePaxa.](https://blog.cloudflare.com/meerkat-introduction/) ⭐️ 8.0/10

Cloudflare has introduced Meerkat, a production-ready globally distributed consensus system built upon the asynchronous QuePaxa algorithm, which aims to eliminate dependencies on a strong leader node and maintain performance under unstable network conditions. This represents a significant deployment of an asynchronous consensus algorithm in production, offering a potential solution to the fragility of leader-based systems like Raft in geographically distributed and unstable networks. Meerkat is based on QuePaxa, which uses randomization and hedging instead of timeouts to achieve liveness, potentially offering robustness at the cost of higher read latency as every operation, including reads, requires global consensus.

hackernews · bobnamob · Jul 8, 13:18 · [Discussion](https://news.ycombinator.com/item?id=48831565)

**Background**: Consensus algorithms like Paxos and Raft are fundamental for coordinating distributed systems but traditionally rely on timeouts and a strong leader, which can fail under network partitions or high latency. The FLP impossibility result proves deterministic consensus is impossible in a fully asynchronous system, so algorithms like QuePaxa use randomization to achieve probabilistic guarantees. Asynchronous algorithms do not depend on timing assumptions, making them more robust to network instability.

<details><summary>References</summary>
<ul>
<li><a href="https://bford.info/pub/os/quepaxa/">QuePaxa: Escaping the Tyranny of Timeouts in Consensus – Bryan Ford's Home Page</a></li>
<li><a href="https://en.wikipedia.org/wiki/Consensus_(computer_science)">Consensus (computer science) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Paxos_(computer_science)">Paxos (computer science) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community discussion shows high technical engagement, with some users questioning the novelty of comparing Meerkat to leader-based Raft instead of other leaderless protocols, while others highlight it as the first production implementation of an asynchronous consensus algorithm. A key trade-off discussed is the potentially high latency for read operations, though proponents note its value for dealing with messy, unstable networks where leader-based systems struggle.

**Tags**: `#distributed-systems`, `#consensus-algorithms`, `#cloudflare`, `#system-architecture`, `#networking`

---

<a id="item-5"></a>
## [LingBot-Video: A 13B Sparse MoE Model for Action-Conditioned Video Generation](https://www.reddit.com/r/MachineLearning/comments/1ur0bxq/lingbotvideo_sparsemoe_video_diffusion/) ⭐️ 8.0/10

LingBot-Video has been released as a 13B-parameter sparse Mixture-of-Experts (MoE) video diffusion transformer, of which only 1.4B parameters are active per inference, and it has been post-trained using reinforcement learning with rewards including a novel physical-plausibility score judged by a vision-language model. This model represents a significant step in scaling efficient, action-conditioned world models for robotics and simulation, but it also sparks a critical technical debate on whether video generation quality alone can be equated with a reliable world model for planning and control. The model uses a DeepSeek-V3-style sparse MoE architecture with 128 experts and top-8 routing, and its open-source release includes weights, code, and a stack integrated with Diffusers and SGLang. A key technical debate surrounds the use of a VLM as a judge for a physical-plausibility reward, which the authors attempt to mitigate by adding real-video negatives to prevent reward hacking.

reddit · r/MachineLearning · /u/Savings-Display5123 · Jul 8, 17:58

**Background**: Mixture-of-Experts (MoE) is a model architecture where only a subset of specialized sub-networks (experts) are activated for each input, enabling large total parameter counts with lower computational cost. A video diffusion transformer generates video frames by iteratively denoising latent representations, and action-conditioning injects control signals (like robot commands) to guide the generated content. A world model is an internal representation that an agent uses to predict the consequences of its actions, often trained to simulate environment dynamics.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://openreview.net/pdf?id=6P88DMUDvH">Code as Reward: Empowering Reinforcement Learning with VLMs</a></li>
<li><a href="https://openreview.net/forum?id=tShfX66qOL">BEYOND SINGLE-STEP: MULTI-FRAME ACTION- CONDITIONED VIDEO GENERATION FOR REINFORCE- MENT LEARNING ENVIRONMENTS | OpenReview</a></li>

</ul>
</details>

**Discussion**: The community discussion highlights two main technical critiques: first, skepticism about whether a vision-language model (VLM) can serve as a defensible judge for a physical-plausibility reward, which risks Goodhart's Law where optimizing for the reward metric degrades real-world physics understanding. Second, there is a pointed debate on the distinction between a high-quality video generator and a true world model, with users demanding closed-loop robotic control demonstrations as evidence, which the paper currently lacks.

**Tags**: `#video generation`, `#diffusion models`, `#sparse MoE`, `#world models`, `#reinforcement learning`

---

<a id="item-6"></a>
## [OpenAI Examines Flaws in Coding Benchmark Integrity](https://openai.com/index/separating-signal-from-noise-coding-evaluations/) ⭐️ 7.0/10

OpenAI published an analysis detailing the systemic issues in popular coding evaluations like SWE-Bench, including fake results, hardware manipulation, and harness-level cheating that compromise benchmark reliability. This work is significant because unreliable benchmarks can mislead the development and comparison of AI models, ultimately hindering progress in creating genuinely capable coding assistants for software engineering. The analysis highlights that benchmark integrity is compromised by practices such as modifying timeouts or hardware configurations to bypass task requirements, and it notes that even the creators of some benchmarks have acknowledged their limitations and moved on.

hackernews · OpenAI Blog · Jul 8, 21:03 · [Discussion](https://news.ycombinator.com/item?id=48837396)

**Background**: SWE-Bench is a widely used benchmark that evaluates AI models by asking them to solve real-world GitHub issues from open-source projects. Coding evaluations are crucial for measuring an AI model's practical ability to write, debug, and improve code, but their design is complex and prone to hidden flaws.

**Discussion**: The community discussion largely agrees that coding benchmarks are flawed, with comments citing specific examples of cheating and questioning why the original authors or downstream users did not rigorously check the data. One commenter proposed a new efficiency-focused benchmark measuring API cost per task, while others expressed skepticism about the value of such benchmarks given the inherently messy nature of real-world software tasks.

**Tags**: `#AI benchmarks`, `#coding evaluation`, `#LLM testing`, `#OpenAI`, `#software engineering`

---

<a id="item-7"></a>
## [OpenAI Publishes Principles for Government and National Security Partnerships](https://openai.com/index/government-national-security-partnerships) ⭐️ 7.0/10

OpenAI has published a new document outlining its principles and approach to forming partnerships with government and national security entities. The framework emphasizes commitments to responsible AI use, democratic accountability, and public safety. This provides crucial transparency into how a leading AI company navigates the sensitive and politically charged area of government and military applications, setting a precedent for industry-wide standards on responsible AI governance. It directly influences ongoing global debates about AI ethics, safety, and the role of the private sector in national security. The document is positioned as a set of guiding principles rather than a specific contractual disclosure, focusing on the ethical and safety boundaries OpenAI intends to uphold in any such collaborations. It signals a proactive attempt by the company to shape the policy conversation around AI and national security before formal regulations are fully established.

rss · OpenAI Blog · Jul 8, 13:30

**Background**: OpenAI is the artificial intelligence research lab behind widely known models like GPT-4 and ChatGPT. As AI capabilities rapidly advance, governments worldwide are exploring its potential applications in defense, intelligence, and public administration, which raises significant ethical questions. Companies developing powerful AI systems are increasingly expected to articulate clear policies on how their technology will or will not be used for military and surveillance purposes.

**Tags**: `#AI ethics`, `#government policy`, `#national security`, `#responsible AI`, `#OpenAI`

---

<a id="item-8"></a>
## [Consumer 3D printing firm Snapmaker secures $140M in sector's largest recent funding round.](https://36kr.com/p/3885728813691145?f=rss) ⭐️ 7.0/10

Consumer 3D printing company Snapmaker has completed a significant funding round of 1 billion yuan (approximately $140 million), led by Cathay Capital with strategic investment from TAL Education, marking the largest single financing in the consumer-grade 3D printing primary market in recent years. The company's revenue grew tenfold year-over-year, largely driven by the success of its flagship U1 printer. This massive funding round signals strong investor confidence in the consumer 3D printing market's maturation and validates Snapmaker's technological breakthrough in multi-color and multi-material printing, which aims to move the technology beyond niche hobbyist use. It demonstrates that architectural innovation can unlock the mainstream consumer market for 3D printing. Snapmaker's flagship U1 printer uses a novel architecture with 4 independent tool heads and a SnapSwap™ quick-change system, claiming 5x improved printing efficiency and about 80% less waste compared to traditional single-nozzle color-change methods. The U1 raised $20.61 million on Kickstarter from over 20,000 backers and has already achieved a delivery volume of over 100,000 units.

rss · 36kr - AI · Jul 8, 00:50

**Background**: Consumer-grade 3D printing has long been limited to single-color, single-material outputs, confining its appeal to engineers and hobbyists. The key challenge has been making printed objects visually appealing and functional enough for everyday use. Multi-color and multi-material printing is considered the critical next step, but conventional methods using single nozzles that switch filaments are slow, wasteful, and impractical for the average consumer.

**Tags**: `#3D printing`, `#venture capital`, `#consumer hardware`, `#startup funding`, `#additive manufacturing`

---

<a id="item-9"></a>
## [AI Biotech Deeper Insights Secures $52M Series B for Phase III GLP-1 Drug](https://36kr.com/p/3885479689465858?f=rss) ⭐️ 7.0/10

AI-native biotech startup Deeper Insights (德睿智药) has raised $52 million in a Series B funding round to advance its AI-designed oral GLP-1 small molecule drug MDR-001 into Phase III clinical trials and further develop its multi-agent AI drug discovery platform, MAP. This funding and the advancement of MDR-001 into late-stage trials demonstrate tangible progress in using AI to significantly accelerate drug development timelines and reduce costs, which could challenge traditional pharmaceutical R&D models and impact the competitive multi-billion dollar GLP-1 market. The company claims MDR-001's progression from project initiation to Phase III took about 4.5 years and cost $23 million, which they state is over 10 times more efficient than the industry average; their MAP platform includes a 'Clinical Data-in-the-Loop' system designed to use clinical feedback to iteratively improve its AI models.

rss · 36kr - AI · Jul 8, 00:00

**Background**: GLP-1 receptor agonists are a major class of drugs used for diabetes and obesity, representing a market worth hundreds of billions of dollars. AI drug discovery platforms aim to use machine learning and computational methods to design molecules, predict their behavior, and optimize clinical trials, moving beyond traditional trial-and-error approaches. A 'multi-agent' AI system typically involves multiple specialized AI modules collaborating to solve complex tasks in the drug discovery pipeline.

**Tags**: `#AI drug discovery`, `#biotech funding`, `#clinical trials`, `#GLP-1`, `#multi-agent systems`

---

<a id="item-10"></a>
## [Amazon's Secret 'Moonraker' Project Aims to Evolve Alexa into an AI Agent](https://36kr.com/newsflashes/3886982568032776?f=rss) ⭐️ 7.0/10

Amazon is secretly developing a major new project codenamed 'Moonraker' to transform its Alexa voice assistant into a full-fledged AI agent. Internal documents indicate the project's extremely high development and operational costs are causing widespread concern within the company. This project represents a significant strategic push by Amazon to stay competitive in the rapidly evolving AI agent market, which is seen as the next frontier for voice assistants and smart home ecosystems. The internal cost concerns highlight the massive financial investment and technical challenges involved in building truly agentic AI systems. The project is reportedly based on internal planning documents, and the extremely high costs are a major point of internal debate, suggesting the technical architecture or the scale of data/compute required is exceptionally demanding. The codename 'Moonraker' itself implies an ambitious, moonshot-style initiative.

rss · 36kr - AI · Jul 8, 12:52

**Background**: Alexa is Amazon's widely used voice assistant, integrated into Echo smart speakers and various other devices. An 'AI agent' is a more advanced system that can autonomously plan, execute complex tasks, and make decisions with minimal human intervention, moving beyond simple voice commands and question-answering. Major tech companies are racing to develop such agents as the next generation of AI interfaces.

**Tags**: `#Amazon`, `#AI_Agents`, `#Voice_Assistants`, `#Large_Tech`, `#AI_Projects`

---

<a id="item-11"></a>
## [Cloudflare and OpenAI Launch Pilot to Enhance AI Search with Global Network Data](https://36kr.com/newsflashes/3886946347694593?f=rss) ⭐️ 7.0/10

Cloudflare and OpenAI announced a research pilot project on July 8 to explore using Cloudflare's global network website insights to help AI search engines discover and index relevant content more efficiently on the open web. This collaboration could significantly improve the accuracy and timeliness of AI-generated search answers by leveraging real-time web data, potentially setting a new standard for how AI systems interact with and index the ever-changing internet. The project aims to use Cloudflare's real-time network signals, such as content freshness, traffic quality, and actual page changes, to improve AI systems' webpage indexing and crawling efficiency.

rss · 36kr - AI · Jul 8, 12:06

**Background**: AI search engines rely on massive indexes of web content to generate answers, but traditional crawling methods can struggle with timeliness and accuracy due to the web's scale and dynamism. Cloudflare operates a global network that touches a significant portion of internet traffic, providing it with unique, real-time signals about content updates and page relevance. OpenAI is a leading artificial intelligence company known for its large language models and search initiatives.

**Tags**: `#AI search`, `#cloud infrastructure`, `#OpenAI`, `#Cloudflare`, `#web indexing`

---

<a id="item-12"></a>
## [OpenAI Announces GPT-Live with Advanced Model Delegation](https://openai.com/index/introducing-gpt-live/) ⭐️ 6.0/10

OpenAI has announced GPT-Live, a new voice assistant feature that can delegate complex queries to more advanced background models like GPT-5.5, moving beyond the limitations of older voice models. This feature could significantly enhance the utility of AI voice assistants by allowing them to leverage the most capable models for complex tasks, potentially setting a new standard for integrated AI interactions. A key feature is its ability to delegate questions to more advanced models in the background, addressing the historical gap between frontier text models and older voice interfaces, though it may still face challenges with real-world tool integration and contextual understanding.

hackernews · OpenAI Blog · Jul 8, 17:03 · [Discussion](https://news.ycombinator.com/item?id=48834405)

**Background**: Voice assistants typically use smaller, faster models optimized for speech, which often lag behind the most powerful frontier text models in capability. Delegation allows a voice interface to act as a front-end that routes requests to more powerful back-end models when needed.

**Discussion**: Community reactions are mixed; some users praise its long-form conversational utility and background delegation feature, while others raise ethical concerns about AI replacing human relationships and criticize the lack of integration with productivity tools and connectors during voice mode.

**Tags**: `#AI assistants`, `#voice interfaces`, `#OpenAI`, `#human-AI interaction`, `#technology ethics`

---

<a id="item-13"></a>
## [OpenAI Upgrades ChatGPT Voice Mode for More Natural Conversation](https://www.theverge.com/ai-artificial-intelligence/962856/chatgpt-upgraded-voice-mode-gpt-live) ⭐️ 6.0/10

OpenAI introduced a new model called GPT-Live-1, which is designed to interrupt users less frequently and better handle conversational pauses to create a more human-like dialogue experience. This improvement enhances the naturalness and usability of voice-based AI interactions, potentially making ChatGPT a more effective and less frustrating tool for real-time communication tasks. The new model, GPT-Live-1, was described by OpenAI research lead Kundan Kumar as a step towards making the AI feel more like talking to another person by being less prone to interrupting during pauses.

rss · The Verge - AI · Jul 8, 17:00

**Background**: Voice assistants and conversational AI systems often struggle with turn-taking and interruptions, which can make interactions feel unnatural. GPT-Live-1 represents an iterative improvement to ChatGPT's existing voice mode, aiming to address these common pain points in human-AI dialogue.

**Tags**: `#AI`, `#Conversational AI`, `#Voice Assistants`, `#ChatGPT`, `#OpenAI`

---

<a id="item-14"></a>
## [id Software Loses 136 Jobs as Part of Major Xbox Layoffs](https://www.pushsquare.com/news/2026/07/136-jobs-lost-at-legendary-dev-id-software-after-xbox-layoffs) ⭐️ 6.0/10

Microsoft's Xbox division layoffs resulted in 136 job losses at the legendary game developer id Software. This is part of a larger wave of approximately 3,200 total layoffs across Microsoft's gaming division, which represents about 20% of its workforce. The layoffs significantly impact one of the most iconic studios in gaming history, creators of the seminal Doom and Quake franchises, signaling a major contraction in the industry. This scale of job loss affects not only the studio's output but also reflects broader economic pressures and strategic shifts within major gaming publishers. id Software is a subsidiary of ZeniMax Media, which was acquired by Microsoft in 2021. The layoffs at id Software are part of a company-wide reduction that has also heavily affected other studios, such as Obsidian Entertainment losing about 25% of its workforce.

rss · Push Square (PlayStation) · Jul 8, 16:15

**Background**: id Software was founded in 1991 and is a pioneering studio in the first-person shooter genre, famous for creating the Doom and Quake series. Microsoft acquired its parent company, ZeniMax Media, for $7.5 billion in 2021 to bolster its Xbox Game Studios portfolio. The current layoffs are part of a broader industry trend of workforce reductions following a period of rapid expansion during the COVID-19 pandemic.

**Tags**: `#gaming industry`, `#layoffs`, `#id Software`, `#Microsoft Xbox`, `#job market`

---

<a id="item-15"></a>
## [Comprehensive Review Ranks Seedance 2.0 as Leading AI Video Tool](https://36kr.com/p/3886403765596418?f=rss) ⭐️ 6.0/10

A comparative review of six major AI video generation tools positions Seedance 2.0 (from ByteDance) as a leading model for its directorial understanding and multi-modal input capabilities. This review provides practical guidance for users navigating the rapidly maturing AI video generation landscape, helping them select tools suited for specific creative or commercial purposes, from zero-barrier short videos to professional enterprise applications. Seedance 2.0 is highlighted for its four-dimensional multi-modal input (image, text, audio, video) and directorial camera control, while competitors like Kling 3.0 excel in physical interaction and Chinese narrative, and Wan 2.2 is tailored for secure, customizable enterprise deployment.

rss · 36kr - AI · Jul 8, 03:03

**Background**: AI video generation has rapidly evolved from producing short, blurry clips to creating coherent, long-form videos with accurate physics. The market now offers a range of tools with specialized strengths, targeting diverse users from individual content creators to professional studios and enterprises.

**Tags**: `#AI video generation`, `#deep learning`, `#computer vision`, `#tools comparison`, `#generative AI`

---

<a id="item-16"></a>
## [Blue Origin Raises $10B at $130B Valuation with Bezos Investing $2B](https://36kr.com/newsflashes/3886944497154824?f=rss) ⭐️ 6.0/10

Blue Origin, Jeff Bezos's aerospace company, has raised $10 billion in new funding, establishing a valuation of $130 billion for the firm. Jeff Bezos personally contributed $2 billion of this investment round. This massive funding round significantly bolsters Blue Origin's financial resources, enabling it to compete more aggressively in the commercial space race against rivals like SpaceX and advance key projects like the New Glenn rocket. It also reflects continued high investor confidence in the long-term commercial space sector despite current economic conditions. The reported valuation of $130 billion would make Blue Origin one of the highest-valued private aerospace companies globally. The $2 billion personal investment from founder Jeff Bezos underscores his continued commitment and reduces reliance on external capital.

rss · 36kr - AI · Jul 8, 12:04

**Background**: Blue Origin is an American privately funded aerospace manufacturer and spaceflight services company founded by Jeff Bezos in 2000. The company is developing reusable launch vehicles like the New Shepard for suborbital tourism and the larger New Glenn for orbital missions, and is a major contractor for NASA's lunar lander program. The commercial space industry is highly capital-intensive, requiring billions in R&D for rocket development and infrastructure.

**Tags**: `#aerospace`, `#business`, `#funding`, `#space`

---