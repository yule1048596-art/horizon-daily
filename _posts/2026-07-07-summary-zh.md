---
layout: default
title: "Horizon Summary: 2026-07-07 (ZH)"
date: 2026-07-07
lang: zh
---

> 从 109 条内容中筛选出 15 条重要资讯。

---

1. [PgDog：基于 Rust 的新型 Postgres 连接池解决状态泄漏和 NOTIFY 问题](#item-1) ⭐️ 8.0/10
2. [腾讯发布 Hy3，一款采用 Apache 2.0 许可的 2950 亿参数 MoE 开源模型。](#item-2) ⭐️ 8.0/10
3. [OpenClaw 超越 React 成为 GitHub 最高星项目，标志 AI Agent 热潮](#item-3) ⭐️ 8.0/10
4. [MIRA：一个用于《火箭联盟》实时四人对战的 50 亿参数世界模型。](#item-4) ⭐️ 8.0/10
5. [Mozilla CTO 将举办 AMA 讨论首份开源 AI 现状报告](#item-5) ⭐️ 8.0/10
6. [新防御方法将模型适应限制在可信 LoRA 子空间中以抵御中毒攻击](#item-6) ⭐️ 8.0/10
7. [Kokoro：一款高质量、对 CPU 友好的本地文本转语音模型](#item-7) ⭐️ 7.0/10
8. [sqlite-utils 4.0 发布，新增重大数据库架构迁移功能](#item-8) ⭐️ 7.0/10
9. [谷歌扩展 Gemini API 托管代理功能，新增后台任务和远程 MCP 支持](#item-9) ⭐️ 7.0/10
10. [Meta 推出 Muse Image 人工智能图像生成模型，并整合到 Instagram 和 WhatsApp 中](#item-10) ⭐️ 7.0/10
11. [字节跳动 Seedance 2.0 AI 模型扭转公司声誉](#item-11) ⭐️ 7.0/10
12. [诉讼威胁关停 SpaceX 的 Colossus 数据中心供电，450 亿美元合同面临风险。](#item-12) ⭐️ 7.0/10
13. [Anthropic 面向订阅用户将 Claude Cowork AI 扩展至移动端和网页端。](#item-13) ⭐️ 6.0/10
14. [中国矿区无人驾驶公司易控智驾将以 130 亿港元估值在港上市](#item-14) ⭐️ 6.0/10
15. [前大疆员工创业做消费级纺织机，获红杉顺为米哈游数亿融资。](#item-15) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [PgDog：基于 Rust 的新型 Postgres 连接池解决状态泄漏和 NOTIFY 问题](https://pgdog.dev/blog/why-yet-another-connection-pooler) ⭐️ 8.0/10

一款名为 PgDog 的新型 PostgreSQL 连接池已面世，它使用 Rust 编写。该工具通过一种新颖的按客户端会话状态跟踪方法，解决了连接状态泄漏和 NOTIFY 性能下降等关键问题。 此解决方案意义重大，因为连接状态泄漏是使用连接池的典型 Postgres 环境中一个严重且未被充分重视的问题，可能导致数据损坏。同时，提升 NOTIFY 性能也有助于构建更具扩展性的、基于 PostgreSQL 原生发布/订阅机制的实时应用。 PgDog 的核心创新在于跟踪每个客户端的会话状态，以防止连接在客户端间复用时发生泄漏。对于 NOTIFY，它在连接池层终止 LISTEN/NOTIFY，并通过 Tokio 广播通道分发消息，仅将 Postgres 用作消息代理。

hackernews · levkk · 7月7日 15:36 · [社区讨论](https://news.ycombinator.com/item?id=48819308)

**背景**: 连接池通过管理可复用的数据库连接池来提升数据库的可扩展性。然而，一个关键问题是，当连接被复用时，来自一个客户端的会话级状态（如搜索路径或事务状态）可能会“泄漏”给另一个客户端。PostgreSQL 内置的 LISTEN/NOTIFY 提供了一种简单的进程间通信机制，但存在已知的性能瓶颈，尤其是在大规模场景下。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.enterprisedb.com/blog/listening-postgres-how-listen-and-notify-syntax-promote-high-availability-application-layer">How LISTEN and NOTIFY Keep Postgres Highly Available at ... - EDB PostgreSQL: docs: LISTEN/NOTIFY performance considerations A Deep Dive into Postgres NOTIFY for Real-Time Database ... Scaling Postgres LISTEN/NOTIFY - PgDog Real‑Time Communication with PostgreSQL LISTEN/NOTIFY and ... GitHub - joelonsql/pg-bench-listen-notify: A Rust ...</a></li>
<li><a href="https://www.postgresql.org/docs/current/sql-notify.html">PostgreSQL: Documentation: 18: NOTIFY</a></li>

</ul>
</details>

**社区讨论**: 社区讨论对项目采用 AGPL 许可证表示积极认可。用户对连接状态泄漏问题的严重性表示惊讶，并询问了查询缓存和多租户模式切换支持等潜在功能。一位用户提出了一个合理的担忧，即 NOTIFY 的性能修复是否会影响事务完整性。

**标签**: `#PostgreSQL`, `#Database`, `#Connection Pooling`, `#Open Source`, `#Rust`

---

<a id="item-2"></a>
## [腾讯发布 Hy3，一款采用 Apache 2.0 许可的 2950 亿参数 MoE 开源模型。](https://simonwillison.net/2026/Jul/6/hy3/#atom-everything) ⭐️ 8.0/10

腾讯发布了 Hy3，这是一款采用 Apache 2.0 许可证的 2950 亿参数混合专家模型。该模型拥有 210 亿活跃参数和 38 亿 MTP 层参数，声称其性能优于同等规模的模型，并可与参数量多 2-5 倍的旗舰开源模型相媲美。 此次发布意义重大，因为它提供了来自中国主要科技公司的一款强大的、采用宽松许可证的大语言模型，可能会加速研究和商业应用。据报道该模型已在超过 50 款产品中集成，表明其具有很强的实用性和性能，这对现有开源生态中主导模型的地位构成了挑战。 完整模型权重为 598GB，但 FP8 量化版本仅为 300GB，上下文长度为 256K tokens。该模型在 OpenRouter 上可免费使用至 7 月 21 日，便于用户立即进行测试和应用。

rss · Simon Willison · 7月6日 23:57

**背景**: 混合专家是一种模型架构，它使用专门的子模型或“专家”来高效地处理任务的不同部分，从而在不成比例增加计算成本的情况下实现高容量。FP8 量化是一种通过将权重表示为 8 位浮点格式来减小模型体积的技术，可在兼容硬件上实现更快的推理。多词预测是一种辅助训练方法，模型同时预测多个未来的词元以提高性能和效率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained - Hugging Face</a></li>
<li><a href="https://www.emergentmind.com/topics/fp8-quantization">FP8 Quantization in Deep Neural Networks</a></li>
<li><a href="https://deepwiki.com/deepseek-ai/DeepSeek-V3/4.4-multi-token-prediction-(mtp)">Multi-Token Prediction (MTP) | deepseek-ai/DeepSeek-V3 | DeepWiki</a></li>

</ul>
</details>

**标签**: `#large language models`, `#open source`, `#Mixture-of-Experts`, `#AI models`, `#Tencent`

---

<a id="item-3"></a>
## [OpenClaw 超越 React 成为 GitHub 最高星项目，标志 AI Agent 热潮](https://36kr.com/p/3885061350617350?f=rss) ⭐️ 8.0/10

开源 AI Agent 项目 OpenClaw 已超越 Facebook 的 React 框架，以超过 25.2 万星标成为 GitHub 历史上星标最多的代码库。其在 3 月 1 日的最新更新合并了 90 余个拉取请求，其中包括针对中国用户的深度本土化适配和与飞书的原生集成。 这一里程碑是开发者社区对 AI Agent 范式热情与投入的强大文化信号，表明可能正在从传统聊天机器人向能够自主执行任务的 AI 进行转变。它凸显了围绕自主智能体不断增长的生态系统，尽管同时也暴露了专业炒作与普通用户实际可用性之间的巨大差距。 OpenClaw 被定义为一个自主 AI 代理平台，而不仅仅是聊天机器人，能够通过自然语言执行管理日历和自动化工作流等现实世界任务。尽管它是开源的，但部署需要 Node.js 环境和命令行配置等技术设置，这催生了收费 500-1000 元的暴利“上门安装”产业，而云服务商现在则提供一键部署的替代方案。

rss · 36kr - AI · 7月7日 06:23

**背景**: React 是由 Meta（原 Facebook）开发的用于构建用户界面的基础 JavaScript 库，主导了网络开发十多年。AI Agent 不同于更简单的聊天机器人；它们是设计用来感知环境、做出决策并采取自主行动以实现目标的系统，通常与工具和软件进行交互。GitHub 星标是衡量开源开发者生态系统中项目受欢迎程度和社区兴趣的指标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenClaw">OpenClaw - Wikipedia</a></li>
<li><a href="https://redis.io/blog/ai-agent-vs-chatbot/">AI Agent vs Chatbot: Key Differences Explained - Redis</a></li>
<li><a href="https://www.star-history.com/">GitHub Star History — Track & Compare Open Source Star Growth</a></li>

</ul>
</details>

**社区讨论**: 文章本身呈现了社区内的争论，一方面将 OpenClaw 视为一种文化现象和开创性 AI Agent 并对其充满开发者式的追捧，另一方面则批评其对普通用户而言存在较高的使用门槛。文中强调的一个关键观点是新兴的付费安装服务行业，这凸显了该项目“开放且易用”的理念与其实际技术复杂性之间的脱节。

**标签**: `#AI Agents`, `#GitHub Trends`, `#Open Source Hype`, `#Developer Tools`, `#AI Assistants`

---

<a id="item-4"></a>
## [MIRA：一个用于《火箭联盟》实时四人对战的 50 亿参数世界模型。](https://www.reddit.com/r/MachineLearning/comments/1upofuw/mira_multiplayer_interactive_world_models_trained/) ⭐️ 8.0/10

由 General Intuition、Kyutai 和 Epic Games 合作开发的 MIRA 已公开发布，这是一个拥有 50 亿参数的世界模型，基于 10,000 小时的《火箭联盟》合成数据进行训练。它能够在单块 NVIDIA B200 GPU 上以每秒 20 帧的速度实现四名玩家的实时游戏对战。 这展示了交互式世界模型在可扩展性方面的重大里程碑，证明了它们能够处理以前被认为极具挑战性的复杂、多智能体、实时环境。模型、代码和大量数据集的公开发布，极大地降低了游戏 AI 和具身智能体进一步研究的门槛。 该模型提供了一个可在线试玩的演示，技术报告已在 ICML 会议上发表，现场还提供了使用 PlayStation 手柄的互动演示。用于训练的 1,000 小时四人游戏数据集子集也已同步发布。

reddit · r/MachineLearning · /u/MasterScrat · 7月7日 07:59

**背景**: 世界模型是强化学习中的一个关键概念，指 AI 智能体学习环境的内部模拟，从而能够在不进行昂贵的真实世界交互的情况下预测结果和规划行动。通过模拟或其他 AI 方法生成的合成数据，对于大规模训练此类模型至关重要，它克服了收集真实世界数据的限制和成本。NVIDIA B200 是一款尖端的数据中心 GPU，以其巨大的内存和针对大型 AI 工作负载的高性能而闻名。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/1803.10122">[1803.10122] World Models - arXiv.org</a></li>
<li><a href="https://jarvislabs.ai/ai-faqs/nvidia-b200-specs">NVIDIA B200 Specs and Price: 192GB Blackwell GPU for ...</a></li>
<li><a href="https://arxiv.org/html/2403.04190v1">Generative AI for Synthetic Data Generation: Methods ...</a></li>

</ul>
</details>

**社区讨论**: Reddit 上的讨论凸显了用户对该模型技术成就的浓厚兴趣，尤其是在单块高端 GPU 上实现实时多人对战的能力。用户们正在询问合成数据的生成过程，并将 MIRA 的方法与其他世界模型和像 GameNGen 这样的游戏模拟器进行比较。

**标签**: `#world models`, `#reinforcement learning`, `#interactive AI`, `#game AI`, `#scalable AI`

---

<a id="item-5"></a>
## [Mozilla CTO 将举办 AMA 讨论首份开源 AI 现状报告](https://www.reddit.com/r/MachineLearning/comments/1upxdvc/raffi_krikorian_cto_mozilla_ama_on_the_state_of/) ⭐️ 8.0/10

Mozilla 首席技术官 Raffi Krikorian 宣布，将于东部时间 7 月 14 日下午 1 点举行一场直播 AMA，讨论他们新发布的《开源 AI 现状》报告中的发现，该报告审视了开源 AI 在生产环境中的实际现状。 此次活动探讨了“免费”模型的真实成本、企业 AI 营销与现实之间的差距以及中国开源模型日益增长的影响力等关键且及时的争论，为在 AI 生态系统中摸索的开发者和企业提供了直接相关的见解。 该报告基于 950 多名开发者的见解，将具体分析使用闭源工具的“隐性成本”、位于模型之上的“智能体操作层”带来的运营开销，以及有能力的中国免费模型引发的竞争格局转变。

reddit · r/MachineLearning · /u/raffikrikorian · 7月7日 14:51

**背景**: “智能体操作层”指的是围绕 AI 模型、管理其生命周期、工具访问和生产安全性的运营基础设施层，它正日益被视为 AI 领域新的竞争战场。“中国效应”则凸显了阿里巴巴的 Qwen 等中国公司提供的强大、免费的开源模型在全球范围内的快速采用，这正在重塑市场动态和开发者的信任。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://opendatascience.com/what-is-an-agent-harness-the-architecture-behind-reliable-agentic-ai/">What is an Agent Harness? The Architecture Behind Agentic AI</a></li>
<li><a href="https://aibusiness.com/nlp/open-source-vs-closed-models-the-true-cost-of-running-ai">Open Source vs. Closed Models: The True Cost of Running AI</a></li>
<li><a href="https://fortune.com/2025/11/25/outside-the-u-s-and-europe-the-momentum-of-chinas-open-source-ai-models-is-plain-to-see/">Why China's open source AI models are eating the world | Fortune</a></li>

</ul>
</details>

**标签**: `#open-source-ai`, `#enterprise-adoption`, `#ai-ecosystem`, `#developer-tools`, `#mozilla`

---

<a id="item-6"></a>
## [新防御方法将模型适应限制在可信 LoRA 子空间中以抵御中毒攻击](https://www.reddit.com/r/MachineLearning/comments/1uq68li/what_if_a_model_could_only_learn_what_trusted/) ⭐️ 8.0/10

一篇新论文提出了一种防御方法，该方法将微调更新限制在一个由可信 LoRA 适配器池定义的子空间内，从而使恶意中毒更新在几何上无法达到。该方法已在 196 个公开的 LoRA 适配器（包括专门设计的自适应攻击）上进行了测试，结果显示攻击成功率大幅下降，同时有用适应性基本得以保留。 这种方法将防御范式从检测中毒数据转变为从根本上限制模型可以学习的内容，为抵御可能嵌入隐藏后门的微调中毒攻击提供了一种强大的几何保障。这对于设备端助手或在大型、可能不受信任的数据集上微调的模型等场景尤为重要。 该防御的工作原理是将微调梯度投影到由可信 LoRA 适配器构成的子空间上，从而在数学上约束更新方向。作者已将论文、代码和实验公开发布，并邀请社区尝试破解该防御。

reddit · r/MachineLearning · /u/Bright_Warning_8406 · 7月7日 20:00

**背景**: LoRA（低秩适应）是一种流行的高效微调大型模型的技术，它通过添加小型、可训练的适配器层而非修改所有参数来实现。微调中毒是一种攻击手段，其中少量恶意数据被插入到微调数据集中，导致模型表现出隐藏行为，例如由特定短语触发的后门。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LoRA_(machine_learning)">LoRA (machine learning) - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2409.18169">[2409.18169] Harmful Fine-tuning Attacks and Defenses for ...</a></li>
<li><a href="https://arxiv.org/html/2505.22358v1">Budget-Adaptive Adapter Tuning in Orthogonal Subspaces for ...</a></li>

</ul>
</details>

**社区讨论**: Reddit 上的社区讨论显示出很高的参与度，用户对这种几何启发的方法表示了兴趣，并就其局限性、实际适用性以及针对该防御本身发起对抗性攻击的可能性提出了深刻的问题。

**标签**: `#AI Safety`, `#Fine-tuning`, `#LoRA`, `#Backdoor Defenses`, `#Machine Learning`

---

<a id="item-7"></a>
## [Kokoro：一款高质量、对 CPU 友好的本地文本转语音模型](https://ariya.io/2026/03/local-cpu-friendly-high-quality-tts-text-to-speech-with-kokoro/) ⭐️ 7.0/10

拥有 8200 万参数的 Kokoro 文本转语音模型作为开源权重系统发布，它在提供高质量、自然语音的同时，针对消费级 CPU 进行了优化，无需强大的 GPU 即可高效运行。 这使得高质量的文本转语音技术能够在标准计算机上用于文章阅读、辅助功能工具和个人生产力等实际日常应用，无需昂贵硬件，显著降低了使用门槛。 一个关键的技术细节是，Kokoro 允许用户手动添加国际音标（IPA）发音指南来纠正同形异义词的发音错误，但在尝试朗读仅仅一两个单词时，效果可能稍逊一筹。

hackernews · speckx · 7月7日 18:24 · [社区讨论](https://news.ycombinator.com/item?id=48821576)

**背景**: 传统的高质量文本转语音模型通常需要强大的 NVIDIA GPU 和大量计算资源进行推理，这使得它们难以用于日常或本地使用。近年来的趋势是开发可以在 CPU 或移动设备上运行的轻量级开源模型。此类模型的架构，如 Kokoro 的双平台设计，采用了量化等技术来减少模型大小和计算负载，同时保持音频质量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/hexgrad/kokoro">GitHub - hexgrad/kokoro: https://hf.co/hexgrad/Kokoro-82M</a></li>
<li><a href="https://localclaw.io/blog/local-tts-guide-2026">Local TTS Guide 2026 — Best Open-Source Text-to-Speech Models</a></li>
<li><a href="https://github.com/kyutai-labs/pocket-tts">GitHub - kyutai-labs/pocket-tts: A TTS that fits in your CPU ...</a></li>

</ul>
</details>

**社区讨论**: 用户对 Kokoro 表现出极大的热情，特别赞扬了它能够在 GTX 1650 GPU 或纯 CPU 等低端硬件上运行的能力，这催生了诸如基于 RSS 的文章播客等创意项目。一个普遍指出的痛点是希望有更好的集成桌面工具，例如用于即时文本转语音的 Mac 小部件，一些用户也指出它在发音单个单词或处理特定同形异义词方面存在局限性，需要手动进行国际音标干预。

**标签**: `#text-to-speech`, `#local-ai`, `#accessibility`, `#python`, `#audio-processing`

---

<a id="item-8"></a>
## [sqlite-utils 4.0 发布，新增重大数据库架构迁移功能](https://simonwillison.net/2026/Jul/7/sqlite-utils-4/#atom-everything) ⭐️ 7.0/10

sqlite-utils 4.0 引入了原生的数据库架构迁移功能、通过新的 `db.atomic()` 方法实现嵌套事务，以及对复合外键的支持，这是自 2020 年 3.0 版本以来该工具包的首次重大版本升级。 此次发布通过提供内置、可靠的工具来管理数据库架构变更和复杂事务，显著改善了开发工作流程，减少了对外部迁移库的依赖，并使 SQLite 在应用程序开发中更加稳健。 迁移使用 sqlite-utils 库定义为 Python 函数，并可利用强大的 `table.transform()` 方法实现超出 SQLite 原生 ALTER TABLE 限制的表结构变更；升级指南指出了一些虽小但重要的破坏性变更。

rss · Simon Willison · 7月7日 19:32

**背景**: sqlite-utils 是一个流行的 Python 命令行工具和库，用于创建、检查和操作 SQLite 数据库。数据库架构迁移是一种系统性地应用、跟踪和版本化数据库结构随时间增量变更的方法。复合外键是涉及多个列的约束，用于在表之间建立关系。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jul/7/sqlite-utils-4/">sqlite-utils 4.0, now with database schema migrations</a></li>
<li><a href="https://sqlite-utils.datasette.io/en/latest/migrations.html">Database migrations - sqlite-utils</a></li>
<li><a href="https://github.com/simonw/sqlite-utils">GitHub - simonw/sqlite-utils: Python CLI utility and library ... Managing Database Versions and Migrations in SQLite GitHub - simonw/sqlite-migrate: A simple database migration ... sqlite-utils 4.0, now with database schema migrations #Shorts SQLite Versioning & Migration Strategies for Evolving Apps</a></li>

</ul>
</details>

**标签**: `#sqlite`, `#database-migrations`, `#python`, `#developer-tools`, `#open-source`

---

<a id="item-9"></a>
## [谷歌扩展 Gemini API 托管代理功能，新增后台任务和远程 MCP 支持](https://blog.google/innovation-and-ai/technology/developers-tools/expanding-managed-agents-gemini-api/) ⭐️ 7.0/10

谷歌已扩展其 Gemini API 中的托管代理功能，新增了对后台任务和远程模型上下文协议（MCP）能力的支持。 此次扩展为开发者提供了更强大灵活的工具，用于构建能够处理长时间运行进程并与外部数据源集成的复杂 AI 代理，从而简化复杂应用的开发流程。 托管代理功能允许开发者通过文件定义代理，并通过单个 API 调用在安全的云沙盒中运行它们，提供一个用于推理和代码执行的远程 Linux 环境。

rss · Google AI Blog · 7月7日 08:54

**背景**: Gemini API 中的托管代理提供了一个无服务器平台，开发者可以在不管理底层基础设施的情况下部署 AI 代理。模型上下文协议（MCP）是一种标准，它使得 AI 代理能够以结构化的方式与外部服务和数据源（如 Azure 或 Power BI）进行交互。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aistudio.google.com/managed-agents">Managed Agents in Gemini API | Google AI Studio</a></li>
<li><a href="https://blog.google/innovation-and-ai/technology/developers-tools/managed-agents-gemini-api/">Build managed agents with the Gemini API - The Keyword</a></li>
<li><a href="https://learn.microsoft.com/en-us/azure/developer/ai/intro-agents-mcp">Build Agents using Model Context Protocol on Azure</a></li>

</ul>
</details>

**标签**: `#AI-agents`, `#Google-Gemini`, `#API-development`, `#developer-tools`

---

<a id="item-10"></a>
## [Meta 推出 Muse Image 人工智能图像生成模型，并整合到 Instagram 和 WhatsApp 中](https://www.theverge.com/tech/962485/meta-muse-image-ai-model-instagram) ⭐️ 7.0/10

Meta 推出了 Muse Image，这是其超级智能实验室部门开发的首款 AI 图像生成模型，现已为 Meta AI、Instagram 和 WhatsApp 的图像创建工具提供支持，并计划很快扩展到 Facebook 和 Messenger。 此次发布标志着 Meta 在为核心功能开发自有的专有 AI 模型方面迈出了重要一步，摆脱了对第三方工具的依赖，并将生成式 AI 深度嵌入其庞大的社交媒体生态系统，这将直接影响数十亿用户。 Muse Image 模型是 Meta 超级智能实验室开发的更广泛的 Muse AI 模型家族的一部分，它取代了 Meta 各平台上用于图像生成功能的先前第三方集成。

rss · The Verge - AI · 7月7日 20:31

**背景**: Meta 超级智能实验室（MSL）是 Meta 于 2025 年 6 月成立的专门 AI 研究部门，旨在开发超级智能系统和个人超级智能。Muse 模型家族（包括早期的 Muse Spark）代表了该实验室的成果，而 Muse Image 则是首个专注于图像生成的模型。社交媒体平台正日益整合生成式 AI 以增强用户内容创作，这一趋势既带来了创造性的可能性，也引发了伦理问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/07/07/meta-ai-muse-image.html">Meta debuts Muse Image, Superintelligence Labs' first AI ...</a></li>
<li><a href="https://ai.meta.com/blog/introducing-muse-spark-msl/">Introducing Muse Spark: Scaling Towards Personal Superintelligence</a></li>
<li><a href="https://grokipedia.com/page/meta_superintelligence_labs">Meta Superintelligence Labs</a></li>

</ul>
</details>

**标签**: `#AI image generation`, `#Meta AI`, `#Generative AI`, `#Social media integration`, `#Product launch`

---

<a id="item-11"></a>
## [字节跳动 Seedance 2.0 AI 模型扭转公司声誉](https://36kr.com/p/3885177884078083?f=rss) ⭐️ 7.0/10

字节跳动的 Seedance 2.0 视频生成模型，在内部做出大胆决定后扩展至 2000 亿参数，成为公司首个在商业上取得成功且领先的 AI 产品，显著提升了其在 AI 行业的声誉。 这一成功表明大型 AI 模型可以实现高利润，据报告 Seedance 贡献了字节跳动 MaaS 收入的一半以上，并证明了战略性的模型扩展和数据投入可以在视频生成领域解锁新的商业机会。 该模型的开发涉及整合团队、从基于 UNet 的架构切换到 DiT（扩散变换器）架构以实现更好的扩展，并在训练数据质量和结构上重点投入，尽管其使用的 GPU 资源相对全球竞争对手较少。

rss · 36kr - AI · 7月7日 07:30

**背景**: 视频生成模型（如 Seedance）是一种经过训练的 AI 系统，能够从文本、图像或其他输入创建逼真的视频。缩放定律（Scaling Law）的概念表明，增加模型参数量（例如 2000 亿）和训练数据量可以带来显著的性能提升，Seedance 2.0 在开发中成功应用了这一原则，而此前较小版本的表现落后于竞争对手（如快手的可灵）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://seed.bytedance.com/en/seedance2_0">Seedance 2.0 - seed.bytedance.com</a></li>
<li><a href="https://arxiv.org/pdf/2604.14148v1">Seedance 2.0: Advancing Video Generation for World Complexity</a></li>

</ul>
</details>

**标签**: `#ByteDance`, `#AI Model`, `#Video Generation`, `#Company Strategy`, `#Deep Learning`

---

<a id="item-12"></a>
## [诉讼威胁关停 SpaceX 的 Colossus 数据中心供电，450 亿美元合同面临风险。](https://36kr.com/newsflashes/3885567094583304?f=rss) ⭐️ 7.0/10

一起诉讼已提起，请求法院下令关停为 SpaceX 的 Colossus 2 数据中心供电的燃气轮机，理由是其在未取得所需许可的情况下运营。此法律行动直接危及 SpaceX 与人工智能公司 Anthropic 签订的 450 亿美元合同的一部分。 此案凸显了大规模人工智能基础设施项目面临的重大法律和运营风险，尤其是在能源许可和合规方面。关停可能会扰乱主要的 AI 计算供应链，并给对推进 AI 能力至关重要的高价值企业合作关系带来压力。 诉讼认为燃气轮机在未获得必要许可的情况下运营，下级法院很可能会在获得许可期间下令关停，但 SpaceX 可能被给予一段合规时间。Colossus 2 数据中心是一座千兆瓦级设施，对向 Anthropic 等合作伙伴提供算力至关重要。

rss · 36kr - AI · 7月7日 12:49

**背景**: Colossus 是由埃隆·马斯克旗下公司开发的数据中心综合体，其中 Colossus 2 是其扩建部分，旨在成为全球首批千兆瓦级 AI 训练设施之一。大型数据中心通常需要为能源基础设施（包括燃气轮机等现场发电设备）申请复杂的许可。像 Anthropic 这样的 AI 公司严重依赖从 xAI 等提供商处获得海量专用算力来训练其先进模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Colossus_(data_center)">Colossus (data center) - Wikipedia</a></li>
<li><a href="https://techcrunch.com/2026/05/20/anthropic-will-pay-xai-1-25-billion-per-month-for-compute/">Anthropic will pay xAI $1.25B per month for compute - TechCrunch</a></li>
<li><a href="https://www.clarkhill.com/news-events/news/epa-turbine-rules-air-permitting-data-centers/">EPA’s New Turbine Rules Ease Air Permits for Data Centers</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#data center`, `#legal risk`, `#SpaceX`, `#Anthropic`

---

<a id="item-13"></a>
## [Anthropic 面向订阅用户将 Claude Cowork AI 扩展至移动端和网页端。](https://www.theverge.com/ai-artificial-intelligence/961978/anthropic-claude-cowork-mobile-web) ⭐️ 6.0/10

从周二开始，Anthropic 首次将其 Claude Cowork AI 平台向移动端和网页端开放。此次发布首先面向 Max 计划订阅用户，其他计划的用户将在未来几周内获得访问权限。 此次扩展显著降低了 Claude Cowork（一款强大的知识工作智能体 AI）的使用门槛，使其脱离桌面应用的限制，在用户随身携带的设备上可用。这标志着 Anthropic 正推动将先进的 AI 能力融入日常的移动和网页工作流程。 Claude Cowork 基于与 Claude Code 相同的智能体架构构建，能够自主完成复杂的多步骤任务，如研究综合和文档准备，而不仅仅是响应提示。访问权限最初仅限于高用量的 Max 订阅层级，该层级提供每月 100 美元和 200 美元两种计划。

rss · The Verge - AI · 7月7日 17:46

**背景**: Claude Cowork 是 Anthropic 的平台，它将智能体 AI 能力——即系统可以自主执行多步骤知识工作任务——带给了 Claude。此前，此功能仅通过 Claude 桌面应用程序提供。Max 计划是 Anthropic 面向高级用户推出的高端订阅层级，与标准 Pro 计划相比，它提供了大幅提高的使用限额。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://claude.com/product/cowork">Claude Cowork: Claude Code power for knowledge work | Claude ...</a></li>
<li><a href="https://claude.com/pricing">Plans & Pricing | Claude by Anthropic</a></li>
<li><a href="https://intuitionlabs.ai/articles/claude-max-plan-pricing-usage-limits">Claude Max Plan Explained: Pricing, Limits & Features</a></li>

</ul>
</details>

**标签**: `#AI`, `#product-launch`, `#Anthropic`, `#Claude`

---

<a id="item-14"></a>
## [中国矿区无人驾驶公司易控智驾将以 130 亿港元估值在港上市](https://36kr.com/p/3885318981366023?f=rss) ⭐️ 6.0/10

易控智驾，这家拥有全球最大活跃无人驾驶矿卡车队的公司，将于 2025 年 7 月 8 日以 18C 特专科技公司的身份在香港联交所上市，估值约 130 亿港元。 此次上市标志着无人驾驶技术在工业和物流领域的商业化迈出了重要一步，显示了投资者对高增长（尽管仍在亏损）的专业细分领域科技公司的兴趣。 公司正从自建并运营车队的重资产模式，向为客户的车辆提供自动驾驶系统的轻资产模式转型，这使得毛利率从亏损改善至 2025 年的 10.1%，但净亏损仍在扩大，经营性现金流持续为负。

rss · 36kr - AI · 7月7日 08:32

**背景**: 香港联交所《上市规则》第 18C 章于 2023 年推出，为可能未达到传统盈利或收入门槛的特专科技公司提供了上市途径。面向商用车（尤其是矿区等封闭环境）的自动驾驶技术面临着独特的挑战，需要能处理重载、复杂地形和保障安全的稳健系统，这与乘用车自动驾驶有所不同。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.hkex.com.hk/Listing/Rules-and-Resources/Guidance/IPO/Listing-of-Specialist-Technology-Companies?sc_lang=zh-HK">特專科技公司上市 - HKEX</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/675578805">主流自动驾驶方案的庖丁解牛，商用车和乘用车的本质需求到底有什么异...</a></li>
<li><a href="https://www.cnblogs.com/star-elink/p/19252921">矿卡无人驾驶从理论到落地的全过程记录（转载） - 星创易联 - 博客园</a></li>

</ul>
</details>

**标签**: `#autonomous vehicles`, `#mining tech`, `#IPO`, `#AI applications`, `#Chinese tech`

---

<a id="item-15"></a>
## [前大疆员工创业做消费级纺织机，获红杉顺为米哈游数亿融资。](https://36kr.com/p/3876837605585160?f=rss) ⭐️ 6.0/10

前大疆工程师胡文鑫创立浪爪智能（CLAWLAB），开发消费级纺织工作站，并连续完成多轮数亿元融资，投资方包括红杉、顺为资本和米哈游等顶级机构。 此轮融资验证了 DIY 纺织和智能家用手工工具存在巨大且服务不足的市场，通过用软硬件一体化技术现代化传统工艺，有望开创个性化制造的新平台。 公司首款产品为用于市场验证的自动簇绒枪，但其核心创新是规划中的纺织“工作站”平台，该平台利用自研 AI 智能体将照片或简单绘图等输入转化为机器可执行的编织图案，大幅降低了设计门槛。

rss · 36kr - AI · 7月7日 02:29

**背景**: 全球 DIY 纺织与编织爱好者社区规模庞大，核心活跃爱好者达数千万级别，潜在覆盖人群可破亿。90 年代的传统家用编织机纯属机械装置，且需要高超技巧。将现代机器人技术、运动规划和计算机图形学集成到消费产品中，标志着该品类的重大技术飞跃，正朝着“放入原料、得到成品”的桌面制造模式发展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.alibaba.com/showroom/home-weaving-machine.html">Home Weaving Machine - High Quality DIY Loom for Kids Images Domestic Weaving Machine - Automatic High-Speed Textile Loom Amazon.com: Weaving Machine Weaving Machine For Home Textile - SMIT Weaving machine home-AliExpress Home Weaving Machine Smart Air Jet Loom Making Fiberglass ... Zcvtbye Knitting Machine, 48 Needles, Smart Weaving Loom Kit ...</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/21245173537">软硬件一体化产品的优势及应用 - 知乎</a></li>
<li><a href="https://www.taobao.com/list/item/cTlzc0RqVnBUeXh4OHhXZ2llZUt5UT09.htm">tufting gun簇绒枪 地毯织枪 电动工具DIY戳戳绣 专用圈绒-淘宝Taobao ...</a></li>

</ul>
</details>

**标签**: `#hardware`, `#startup`, `#consumer-electronics`, `#venture-capital`, `#textile-tech`

---