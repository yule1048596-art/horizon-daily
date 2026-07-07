---
layout: default
title: "Horizon Summary: 2026-07-07 (EN)"
date: 2026-07-07
lang: en
---

> From 109 items, 15 important content pieces were selected

---

1. [PgDog: New Rust-based Postgres Pooler Fixes State Leakage & NOTIFY](#item-1) ⭐️ 8.0/10
2. [Tencent releases Hy3, a 295B-parameter open-source MoE model under Apache 2.0.](#item-2) ⭐️ 8.0/10
3. [OpenClaw Surpasses React as Most-Starred GitHub Project, Signaling AI Agent Hype](#item-3) ⭐️ 8.0/10
4. [MIRA: A 5B-parameter world model for real-time 4-player Rocket League gameplay.](#item-4) ⭐️ 8.0/10
5. [Mozilla CTO to Host AMA on Inaugural State of Open Source AI Report](#item-5) ⭐️ 8.0/10
6. [Novel Defense Constrains Model Adaptation to Trusted LoRA Subspace Against Poisoning](#item-6) ⭐️ 8.0/10
7. [Kokoro: A High-Quality, CPU-Friendly Local Text-to-Speech Model](#item-7) ⭐️ 7.0/10
8. [sqlite-utils 4.0 Released with Major Schema Migration Support](#item-8) ⭐️ 7.0/10
9. [Google Expands Gemini API Managed Agents with Background Tasks and Remote MCP](#item-9) ⭐️ 7.0/10
10. [Meta Launches Muse Image AI Model Integrated into Instagram and WhatsApp](#item-10) ⭐️ 7.0/10
11. [ByteDance's Seedance 2.0 AI Model Reverses Company's Reputation](#item-11) ⭐️ 7.0/10
12. [Lawsuit threatens to shut down SpaceX's Colossus data center power, risking $45B contract.](#item-12) ⭐️ 7.0/10
13. [Anthropic expands Claude Cowork AI to mobile and web for subscribers.](#item-13) ⭐️ 6.0/10
14. [Chinese Autonomous Mining Truck Firm Yikong Zhijie to IPO in Hong Kong at $1.3B Valuation](#item-14) ⭐️ 6.0/10
15. [Ex-DJI engineer's startup gets major funding for consumer-grade textile machines.](#item-15) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [PgDog: New Rust-based Postgres Pooler Fixes State Leakage & NOTIFY](https://pgdog.dev/blog/why-yet-another-connection-pooler) ⭐️ 8.0/10

PgDog, a new PostgreSQL connection pooler written in Rust, has been introduced. It addresses critical issues like connection state leakage and NOTIFY performance degradation through a novel per-client session state tracking approach. This solution is significant because connection state leakage is a serious and underappreciated problem in typical Postgres setups using connection poolers, potentially causing data corruption. Improving NOTIFY performance also enables more scalable real-time applications built on PostgreSQL's native pub/sub mechanism. PgDog's core innovation is tracking per-client session state to prevent leakage when connections are reused between clients. For NOTIFY, it terminates LISTEN/NOTIFY at the pooler and fans out messages over Tokio broadcast channels, using Postgres only as the broker.

hackernews · levkk · Jul 7, 15:36 · [Discussion](https://news.ycombinator.com/item?id=48819308)

**Background**: Connection poolers improve database scalability by managing a pool of reusable database connections. However, a key problem is that session-level state (like search paths or transaction status) from one client can 'leak' to another when a connection is reused. PostgreSQL's built-in LISTEN/NOTIFY provides a simple inter-process communication mechanism but has known performance bottlenecks, especially at scale.

<details><summary>References</summary>
<ul>
<li><a href="https://www.enterprisedb.com/blog/listening-postgres-how-listen-and-notify-syntax-promote-high-availability-application-layer">How LISTEN and NOTIFY Keep Postgres Highly Available at ... - EDB PostgreSQL: docs: LISTEN/NOTIFY performance considerations A Deep Dive into Postgres NOTIFY for Real-Time Database ... Scaling Postgres LISTEN/NOTIFY - PgDog Real‑Time Communication with PostgreSQL LISTEN/NOTIFY and ... GitHub - joelonsql/pg-bench-listen-notify: A Rust ...</a></li>
<li><a href="https://www.postgresql.org/docs/current/sql-notify.html">PostgreSQL: Documentation: 18: NOTIFY</a></li>

</ul>
</details>

**Discussion**: The community discussion highlights positive sentiment towards the project's use of the AGPL license. Users expressed surprise at the severity of the connection state leakage problem and inquired about potential features like query caching and multi-tenant schema switching support. One user raised a valid concern about whether the NOTIFY performance fix compromises transactional integrity.

**Tags**: `#PostgreSQL`, `#Database`, `#Connection Pooling`, `#Open Source`, `#Rust`

---

<a id="item-2"></a>
## [Tencent releases Hy3, a 295B-parameter open-source MoE model under Apache 2.0.](https://simonwillison.net/2026/Jul/6/hy3/#atom-everything) ⭐️ 8.0/10

Tencent has released Hy3, a 295B-parameter Mixture-of-Experts (MoE) model with an Apache 2.0 license. The model, which has 21B active parameters and 3.8B MTP layer parameters, claims to outperform similar-sized models and rival flagship open-source models with 2-5 times more parameters. This release is significant as it provides a powerful, permissively licensed large language model from a major Chinese tech company, potentially accelerating research and commercial adoption. Its reported integration across over 50 products suggests strong practical utility and performance, challenging the dominance of existing models in the open-source ecosystem. The full model weights are 598GB, but an FP8 quantized version is available at 300GB, with a context length of 256K tokens. The model is offered for free on OpenRouter until July 21st, making it accessible for immediate testing and application.

rss · Simon Willison · Jul 6, 23:57

**Background**: Mixture-of-Experts (MoE) is a model architecture that uses specialized sub-models or 'experts' to handle different parts of a task efficiently, allowing for high capacity without proportionally increasing computational cost. FP8 quantization is a technique that reduces model size by representing weights in 8-bit floating-point format, enabling faster inference on compatible hardware. Multi-Token Prediction (MTP) is an auxiliary training method where a model predicts multiple future tokens at once to improve performance and efficiency.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained - Hugging Face</a></li>
<li><a href="https://www.emergentmind.com/topics/fp8-quantization">FP8 Quantization in Deep Neural Networks</a></li>
<li><a href="https://deepwiki.com/deepseek-ai/DeepSeek-V3/4.4-multi-token-prediction-(mtp)">Multi-Token Prediction (MTP) | deepseek-ai/DeepSeek-V3 | DeepWiki</a></li>

</ul>
</details>

**Tags**: `#large language models`, `#open source`, `#Mixture-of-Experts`, `#AI models`, `#Tencent`

---

<a id="item-3"></a>
## [OpenClaw Surpasses React as Most-Starred GitHub Project, Signaling AI Agent Hype](https://36kr.com/p/3885061350617350?f=rss) ⭐️ 8.0/10

The open-source AI Agent project OpenClaw has surpassed Facebook's React framework to become the most-starred repository in GitHub history, accumulating over 252,000 stars. Its latest update on March 1 integrated over 90 pull requests, including deep localization for Chinese users and native integration with Feishu (Lark). This milestone is a powerful cultural signal of the developer community's excitement and investment in the AI Agent paradigm, suggesting a potential shift beyond traditional chatbots towards autonomous, task-executing AI. It highlights the growing ecosystem around autonomous agents, though it also exposes the significant gap between professional hype and practical usability for average users. OpenClaw is defined as an autonomous AI agent platform, not just a chatbot, capable of executing real-world tasks like managing calendars and automating workflows via natural language. Despite its open-source nature, deployment requires technical setup with Node.js and command-line configuration, which has spawned a lucrative 'installation service' industry charging 500-1000 yuan, while cloud providers now offer one-click deployment alternatives.

rss · 36kr - AI · Jul 7, 06:23

**Background**: React is a foundational JavaScript library for building user interfaces, developed by Meta (formerly Facebook), and has dominated web development for over a decade. AI Agents are distinct from simpler chatbots; they are systems designed to perceive their environment, make decisions, and take autonomous actions to achieve goals, often interacting with tools and software. GitHub stars are a measure of a project's popularity and community interest within the open-source developer ecosystem.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenClaw">OpenClaw - Wikipedia</a></li>
<li><a href="https://redis.io/blog/ai-agent-vs-chatbot/">AI Agent vs Chatbot: Key Differences Explained - Redis</a></li>
<li><a href="https://www.star-history.com/">GitHub Star History — Track & Compare Open Source Star Growth</a></li>

</ul>
</details>

**Discussion**: The article itself presents a debate within the community, contrasting the 'cultural phenomenon' and developer worship of OpenClaw as a pioneering AI Agent with the practical challenges and criticism regarding its high barrier to entry for ordinary users. A key viewpoint highlighted is the emerging industry of paid installation services, which underscores the disconnect between the project's 'open and accessible' ethos and its actual technical complexity.

**Tags**: `#AI Agents`, `#GitHub Trends`, `#Open Source Hype`, `#Developer Tools`, `#AI Assistants`

---

<a id="item-4"></a>
## [MIRA: A 5B-parameter world model for real-time 4-player Rocket League gameplay.](https://www.reddit.com/r/MachineLearning/comments/1upofuw/mira_multiplayer_interactive_world_models_trained/) ⭐️ 8.0/10

MIRA, a collaborative project from General Intuition, Kyutai, and Epic Games, has been publicly released as a 5-billion parameter world model trained on 10,000 hours of synthetic Rocket League data. It enables real-time gameplay for four players at 20 frames per second on a single NVIDIA B200 GPU. This demonstrates a major scalability milestone for interactive world models, showing they can handle complex, multi-agent, real-time environments previously thought too challenging. The public release of the model, code, and a substantial dataset significantly lowers the barrier for further research in game AI and embodied agents. The model is hosted for a playable online demo, and the technical report was presented at the ICML conference, where an interactive demo with PlayStation controllers was also available. The training dataset is a subset of 1,000 hours of 4-player gameplay that has also been released.

reddit · r/MachineLearning · /u/MasterScrat · Jul 7, 07:59

**Background**: World models are a key concept in reinforcement learning where an AI agent learns an internal simulation of its environment, allowing it to predict outcomes and plan actions without costly real-world interaction. Synthetic data, generated through simulation or other AI methods, is crucial for training such models on a massive scale, overcoming the limitations and cost of collecting real-world data. The NVIDIA B200 is a state-of-the-art datacenter GPU known for its massive memory and high performance for large AI workloads.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/1803.10122">[1803.10122] World Models - arXiv.org</a></li>
<li><a href="https://jarvislabs.ai/ai-faqs/nvidia-b200-specs">NVIDIA B200 Specs and Price: 192GB Blackwell GPU for ...</a></li>
<li><a href="https://arxiv.org/html/2403.04190v1">Generative AI for Synthetic Data Generation: Methods ...</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion highlights strong interest in the model's technical achievements, particularly its real-time multiplayer capability on a single high-end GPU. Users are inquiring about the synthetic data generation process and comparing MIRA's approach to other world models and game simulators like GameNGen.

**Tags**: `#world models`, `#reinforcement learning`, `#interactive AI`, `#game AI`, `#scalable AI`

---

<a id="item-5"></a>
## [Mozilla CTO to Host AMA on Inaugural State of Open Source AI Report](https://www.reddit.com/r/MachineLearning/comments/1upxdvc/raffi_krikorian_cto_mozilla_ama_on_the_state_of/) ⭐️ 8.0/10

Mozilla's CTO, Raffi Krikorian, has announced a live AMA session on July 14 at 1pm ET to discuss the findings of their new 'State of Open Source AI' report, which examines the practical realities of open-source AI in production. This event addresses critical, timely debates about the true costs of 'free' models, the gap between enterprise AI marketing and reality, and the growing influence of Chinese open-source models, offering insights directly relevant to developers and businesses navigating the AI ecosystem. The report draws on insights from over 950 developers and will specifically analyze the 'hidden tax' of using closed-source tools, the operational overhead of the 'agentic harness' layer that sits on top of models, and the competitive shift caused by capable, free Chinese models.

reddit · r/MachineLearning · /u/raffikrikorian · Jul 7, 14:51

**Background**: The 'agentic harness' refers to the operational infrastructure layer around an AI model that manages its lifecycle, tool access, and safety in production, which is increasingly seen as the new competitive battleground in AI. The 'China effect' highlights the rapid global adoption of powerful, free open-source models from Chinese companies like Alibaba's Qwen, which is reshaping market dynamics and developer trust.

<details><summary>References</summary>
<ul>
<li><a href="https://opendatascience.com/what-is-an-agent-harness-the-architecture-behind-reliable-agentic-ai/">What is an Agent Harness? The Architecture Behind Agentic AI</a></li>
<li><a href="https://aibusiness.com/nlp/open-source-vs-closed-models-the-true-cost-of-running-ai">Open Source vs. Closed Models: The True Cost of Running AI</a></li>
<li><a href="https://fortune.com/2025/11/25/outside-the-u-s-and-europe-the-momentum-of-chinas-open-source-ai-models-is-plain-to-see/">Why China's open source AI models are eating the world | Fortune</a></li>

</ul>
</details>

**Tags**: `#open-source-ai`, `#enterprise-adoption`, `#ai-ecosystem`, `#developer-tools`, `#mozilla`

---

<a id="item-6"></a>
## [Novel Defense Constrains Model Adaptation to Trusted LoRA Subspace Against Poisoning](https://www.reddit.com/r/MachineLearning/comments/1uq68li/what_if_a_model_could_only_learn_what_trusted/) ⭐️ 8.0/10

A new paper proposes a defense that restricts fine-tuning updates to a subspace defined by a pool of trusted LoRA adapters, making malicious poisoning updates geometrically unreachable. The approach was tested on 196 public LoRA adapters, including adaptive attacks, showing sharply reduced attack success while preserving useful adaptation. This method shifts the defense paradigm from detecting poisoned data to fundamentally restricting what a model can learn, offering a robust geometric safeguard against fine-tuning poisoning attacks that could embed hidden backdoors. It is particularly relevant for scenarios like on-device assistants or models fine-tuned on large, potentially untrusted datasets. The defense works by projecting fine-tuning gradients onto a subspace formed by trusted LoRA adapters, mathematically constraining the update directions. The authors have made the paper, code, and experiments publicly available and have invited the community to attempt to break the defense.

reddit · r/MachineLearning · /u/Bright_Warning_8406 · Jul 7, 20:00

**Background**: LoRA (Low-Rank Adaptation) is a popular technique for efficiently fine-tuning large models by adding small, trainable adapter layers instead of modifying all parameters. Fine-tuning poisoning is an attack where a small amount of malicious data is inserted into the fine-tuning dataset to cause the model to exhibit hidden behaviors, such as backdoors triggered by specific phrases.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LoRA_(machine_learning)">LoRA (machine learning) - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2409.18169">[2409.18169] Harmful Fine-tuning Attacks and Defenses for ...</a></li>
<li><a href="https://arxiv.org/html/2505.22358v1">Budget-Adaptive Adapter Tuning in Orthogonal Subspaces for ...</a></li>

</ul>
</details>

**Discussion**: The community discussion on Reddit shows strong engagement, with users expressing interest in the geometrically-inspired approach and asking insightful questions about its limitations, real-world applicability, and potential for adversarial attacks against the defense itself.

**Tags**: `#AI Safety`, `#Fine-tuning`, `#LoRA`, `#Backdoor Defenses`, `#Machine Learning`

---

<a id="item-7"></a>
## [Kokoro: A High-Quality, CPU-Friendly Local Text-to-Speech Model](https://ariya.io/2026/03/local-cpu-friendly-high-quality-tts-text-to-speech-with-kokoro/) ⭐️ 7.0/10

The Kokoro TTS model, with 82 million parameters, has been released as an open-weight system that delivers high-quality, natural-sounding speech while being optimized to run efficiently on consumer CPUs, eliminating the need for powerful GPUs. This makes high-quality text-to-speech technology accessible for practical, everyday applications like article reading, accessibility tools, and personal productivity on standard computers without expensive hardware, significantly lowering the barrier to entry. A key technical detail is that Kokoro allows users to manually add International Phonetic Alphabet (IPA) pronunciation guides to correct mispronunciations of homographs, though it may fall short when trying to say just a single word or two.

hackernews · speckx · Jul 7, 18:24 · [Discussion](https://news.ycombinator.com/item?id=48821576)

**Background**: Traditional high-quality text-to-speech models often require powerful NVIDIA GPUs and significant computational resources for inference, making them inaccessible for casual or local use. Recent trends focus on developing lightweight, open-source models that can run on CPUs or mobile devices. The architecture of such models, like Kokoro's dual-platform design, involves techniques such as quantization to reduce the model size and computational load while preserving audio quality.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/hexgrad/kokoro">GitHub - hexgrad/kokoro: https://hf.co/hexgrad/Kokoro-82M</a></li>
<li><a href="https://localclaw.io/blog/local-tts-guide-2026">Local TTS Guide 2026 — Best Open-Source Text-to-Speech Models</a></li>
<li><a href="https://github.com/kyutai-labs/pocket-tts">GitHub - kyutai-labs/pocket-tts: A TTS that fits in your CPU ...</a></li>

</ul>
</details>

**Discussion**: Users express strong enthusiasm for Kokoro, particularly praising its ability to run on lower-end hardware like a GTX 1650 GPU or pure CPU, which has enabled creative projects like RSS-based article podcasters. A common pain point highlighted is the desire for better integrated desktop tools, such as a Mac widget for instant text-to-speech, and some users note its limitations in pronouncing single words or handling specific homographs without manual IPA intervention.

**Tags**: `#text-to-speech`, `#local-ai`, `#accessibility`, `#python`, `#audio-processing`

---

<a id="item-8"></a>
## [sqlite-utils 4.0 Released with Major Schema Migration Support](https://simonwillison.net/2026/Jul/7/sqlite-utils-4/#atom-everything) ⭐️ 7.0/10

sqlite-utils 4.0 introduces native database schema migrations, nested transactions via a new `db.atomic()` method, and support for compound foreign keys, marking the toolkit's first major version bump since 3.0 in 2020. This release significantly enhances developer workflow by providing built-in, reliable tools for managing database schema changes and complex transactions, reducing the need for external migration libraries and making SQLite more robust for application development. Migrations are defined as Python functions using the sqlite-utils library and can leverage the powerful `table.transform()` method to alter tables beyond SQLite's native ALTER TABLE limitations; the upgrade guide notes some small but significant breaking changes.

rss · Simon Willison · Jul 7, 19:32

**Background**: sqlite-utils is a popular Python CLI utility and library for creating, inspecting, and manipulating SQLite databases. Database schema migrations are a systematic way to apply, track, and version incremental changes to a database's structure over time. Compound foreign keys are constraints involving multiple columns that establish relationships between tables.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jul/7/sqlite-utils-4/">sqlite-utils 4.0, now with database schema migrations</a></li>
<li><a href="https://sqlite-utils.datasette.io/en/latest/migrations.html">Database migrations - sqlite-utils</a></li>
<li><a href="https://github.com/simonw/sqlite-utils">GitHub - simonw/sqlite-utils: Python CLI utility and library ... Managing Database Versions and Migrations in SQLite GitHub - simonw/sqlite-migrate: A simple database migration ... sqlite-utils 4.0, now with database schema migrations #Shorts SQLite Versioning & Migration Strategies for Evolving Apps</a></li>

</ul>
</details>

**Tags**: `#sqlite`, `#database-migrations`, `#python`, `#developer-tools`, `#open-source`

---

<a id="item-9"></a>
## [Google Expands Gemini API Managed Agents with Background Tasks and Remote MCP](https://blog.google/innovation-and-ai/technology/developers-tools/expanding-managed-agents-gemini-api/) ⭐️ 7.0/10

Google has expanded the Managed Agents feature in its Gemini API to include support for background tasks and remote Model Context Protocol (MCP) capabilities. This expansion provides developers with more powerful and flexible tools for building sophisticated AI agents that can handle long-running processes and integrate with external data sources, streamlining complex application development. The Managed Agents feature allows developers to define agents via files and run them in secure cloud sandboxes with a single API call, providing a remote Linux environment for reasoning and code execution.

rss · Google AI Blog · Jul 7, 08:54

**Background**: Managed Agents in the Gemini API provide a serverless platform where developers can deploy AI agents without managing underlying infrastructure. The Model Context Protocol (MCP) is a standard that enables AI agents to interact with external services and data sources, such as Azure or Power BI, in a structured way.

<details><summary>References</summary>
<ul>
<li><a href="https://aistudio.google.com/managed-agents">Managed Agents in Gemini API | Google AI Studio</a></li>
<li><a href="https://blog.google/innovation-and-ai/technology/developers-tools/managed-agents-gemini-api/">Build managed agents with the Gemini API - The Keyword</a></li>
<li><a href="https://learn.microsoft.com/en-us/azure/developer/ai/intro-agents-mcp">Build Agents using Model Context Protocol on Azure</a></li>

</ul>
</details>

**Tags**: `#AI-agents`, `#Google-Gemini`, `#API-development`, `#developer-tools`

---

<a id="item-10"></a>
## [Meta Launches Muse Image AI Model Integrated into Instagram and WhatsApp](https://www.theverge.com/tech/962485/meta-muse-image-ai-model-instagram) ⭐️ 7.0/10

Meta has launched Muse Image, the first AI image generation model from its Superintelligence Labs division, which now powers image-creation tools within Meta AI, Instagram, and WhatsApp, with plans to expand to Facebook and Messenger soon. This launch marks a significant step for Meta in developing its own proprietary AI models for core features, moving away from third-party tools, and deeply embedding generative AI into its massive social media ecosystem, which will directly affect billions of users. The Muse Image model is part of the broader Muse AI model family developed by Meta Superintelligence Labs, and it replaces previous third-party integrations for image generation features across Meta's platforms.

rss · The Verge - AI · Jul 7, 20:31

**Background**: Meta Superintelligence Labs (MSL) is Meta's dedicated AI research division established in June 2025 to develop superintelligent systems and 'personal superintelligence'. The Muse family of models, including the earlier Muse Spark, represents MSL's output, with Muse Image being the first focused on image generation. Social media platforms are increasingly integrating generative AI to enhance user content creation, a trend that raises both creative possibilities and ethical questions.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/07/07/meta-ai-muse-image.html">Meta debuts Muse Image, Superintelligence Labs' first AI ...</a></li>
<li><a href="https://ai.meta.com/blog/introducing-muse-spark-msl/">Introducing Muse Spark: Scaling Towards Personal Superintelligence</a></li>
<li><a href="https://grokipedia.com/page/meta_superintelligence_labs">Meta Superintelligence Labs</a></li>

</ul>
</details>

**Tags**: `#AI image generation`, `#Meta AI`, `#Generative AI`, `#Social media integration`, `#Product launch`

---

<a id="item-11"></a>
## [ByteDance's Seedance 2.0 AI Model Reverses Company's Reputation](https://36kr.com/p/3885177884078083?f=rss) ⭐️ 7.0/10

ByteDance's Seedance 2.0 video generation model, scaled to 200 billion parameters after a bold internal decision, became the company's first commercially successful and leading AI product, significantly improving its reputation in the AI industry. This success demonstrates that large AI models can be highly profitable, with Seedance reportedly generating over half of ByteDance's MaaS revenue and proving that strategic scaling and data investment can unlock new commercial opportunities in video generation. The model's development involved consolidating teams, switching from a UNet-based to a DiT (Diffusion Transformer) architecture for better scaling, and focusing heavily on training data quality and structure, despite using comparatively fewer GPU resources than global competitors.

rss · 36kr - AI · Jul 7, 07:30

**Background**: Video generation models like Seedance are AI systems trained to create realistic videos from text, images, or other inputs. The scaling law concept suggests that increasing a model's parameter count (e.g., to 200B) and training data volume can lead to significant performance improvements, a principle successfully applied in Seedance 2.0's development after earlier, smaller versions underperformed competitors like Kuaishou's Kling.

<details><summary>References</summary>
<ul>
<li><a href="https://seed.bytedance.com/en/seedance2_0">Seedance 2.0 - seed.bytedance.com</a></li>
<li><a href="https://arxiv.org/pdf/2604.14148v1">Seedance 2.0: Advancing Video Generation for World Complexity</a></li>

</ul>
</details>

**Tags**: `#ByteDance`, `#AI Model`, `#Video Generation`, `#Company Strategy`, `#Deep Learning`

---

<a id="item-12"></a>
## [Lawsuit threatens to shut down SpaceX's Colossus data center power, risking $45B contract.](https://36kr.com/newsflashes/3885567094583304?f=rss) ⭐️ 7.0/10

A lawsuit has been filed requesting a court order to shut down the gas turbines powering SpaceX's Colossus 2 data center, claiming operation without required permits. This legal action directly jeopardizes a part of SpaceX's $45 billion contract with AI company Anthropic. This case highlights the significant legal and operational risks facing large-scale AI infrastructure projects, particularly concerning energy permitting and compliance. A shutdown could disrupt major AI compute supply chains and strain high-value corporate partnerships crucial for advancing AI capabilities. The lawsuit argues the gas turbines are operating without the necessary permits, and a lower court is likely to order a shutdown while permits are obtained, though SpaceX might be granted a compliance period. The Colossus 2 data center is a gigawatt-scale facility critical for providing compute to partners like Anthropic.

rss · 36kr - AI · Jul 7, 12:49

**Background**: Colossus is a data center complex developed by Elon Musk's companies, with Colossus 2 being an expansion designed to be one of the world's first gigawatt-scale AI training facilities. Large data centers often require complex permits for energy infrastructure, including on-site power generation like gas turbines. AI companies like Anthropic heavily depend on securing massive amounts of specialized compute from providers like xAI to train their advanced models.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Colossus_(data_center)">Colossus (data center) - Wikipedia</a></li>
<li><a href="https://techcrunch.com/2026/05/20/anthropic-will-pay-xai-1-25-billion-per-month-for-compute/">Anthropic will pay xAI $1.25B per month for compute - TechCrunch</a></li>
<li><a href="https://www.clarkhill.com/news-events/news/epa-turbine-rules-air-permitting-data-centers/">EPA’s New Turbine Rules Ease Air Permits for Data Centers</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#data center`, `#legal risk`, `#SpaceX`, `#Anthropic`

---

<a id="item-13"></a>
## [Anthropic expands Claude Cowork AI to mobile and web for subscribers.](https://www.theverge.com/ai-artificial-intelligence/961978/anthropic-claude-cowork-mobile-web) ⭐️ 6.0/10

Starting Tuesday, Anthropic is making its Claude Cowork AI platform accessible on mobile and web for the first time. The initial rollout is exclusive to Max plan subscribers, with availability expanding to users on other plans in the coming weeks. This expansion significantly lowers the barrier to access for Claude Cowork, a powerful agentic AI for knowledge work, by freeing it from the desktop app and making it available on the devices users carry everywhere. It signals Anthropic's push to integrate advanced AI capabilities into daily mobile and web workflows. Claude Cowork is built on the same agentic architecture as Claude Code and can autonomously complete complex, multi-step tasks like research synthesis and document preparation, rather than simply responding to prompts. Access is initially restricted to the high-usage Max subscription tier, which offers plans at $100 and $200 per month.

rss · The Verge - AI · Jul 7, 17:46

**Background**: Claude Cowork is Anthropic's platform that brings agentic AI capabilities—where the system can act autonomously to complete multi-step knowledge work tasks—to Claude. Previously, this functionality was only available through the Claude desktop application. The Max plan is Anthropic's premium subscription tier aimed at power users, offering substantially higher usage limits compared to the standard Pro plan.

<details><summary>References</summary>
<ul>
<li><a href="https://claude.com/product/cowork">Claude Cowork: Claude Code power for knowledge work | Claude ...</a></li>
<li><a href="https://claude.com/pricing">Plans & Pricing | Claude by Anthropic</a></li>
<li><a href="https://intuitionlabs.ai/articles/claude-max-plan-pricing-usage-limits">Claude Max Plan Explained: Pricing, Limits & Features</a></li>

</ul>
</details>

**Tags**: `#AI`, `#product-launch`, `#Anthropic`, `#Claude`

---

<a id="item-14"></a>
## [Chinese Autonomous Mining Truck Firm Yikong Zhijie to IPO in Hong Kong at $1.3B Valuation](https://36kr.com/p/3885318981366023?f=rss) ⭐️ 6.0/10

Yikong Zhijie, the operator of the world's largest active autonomous mining truck fleet, is set to list on the Hong Kong Stock Exchange on July 8, 2025, under the Chapter 18C specialist technology company regime, with a valuation of approximately HK$13 billion. This IPO represents a significant milestone for the commercialization of autonomous driving technology in the industrial and logistics sectors, demonstrating investor appetite for high-growth, albeit loss-making, technology companies in a specialized niche. The company is transitioning from a capital-heavy model of owning and operating its own fleet to an asset-light model of providing its autonomous driving system to customers' own trucks, which has improved gross margins from negative to 10.1% in 2025, though it still reports growing net losses and negative operating cash flow.

rss · 36kr - AI · Jul 7, 08:32

**Background**: Chapter 18C of the Hong Kong Listing Rules, introduced in 2023, provides a pathway for specialist technology companies that may not meet traditional profit or revenue thresholds to list on the HKEX. Autonomous driving technology for commercial vehicles, particularly in enclosed environments like mines, faces distinct challenges and requires robust systems for handling heavy loads, complex terrain, and safety, differentiating it from passenger vehicle autonomous driving.

<details><summary>References</summary>
<ul>
<li><a href="https://www.hkex.com.hk/Listing/Rules-and-Resources/Guidance/IPO/Listing-of-Specialist-Technology-Companies?sc_lang=zh-HK">特專科技公司上市 - HKEX</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/675578805">主流自动驾驶方案的庖丁解牛，商用车和乘用车的本质需求到底有什么异...</a></li>
<li><a href="https://www.cnblogs.com/star-elink/p/19252921">矿卡无人驾驶从理论到落地的全过程记录（转载） - 星创易联 - 博客园</a></li>

</ul>
</details>

**Tags**: `#autonomous vehicles`, `#mining tech`, `#IPO`, `#AI applications`, `#Chinese tech`

---

<a id="item-15"></a>
## [Ex-DJI engineer's startup gets major funding for consumer-grade textile machines.](https://36kr.com/p/3876837605585160?f=rss) ⭐️ 6.0/10

Former DJI engineer Hu Wenxin founded CLAWLAB to develop a consumer-grade textile station, raising hundreds of millions in funding from top investors like Sequoia, Shunwei, and miHoYo across multiple rounds. This funding validates a massive, underserved market for DIY textiles and smart home crafting tools, potentially creating a new platform for personalized manufacturing by modernizing a traditional craft with integrated hardware and software. The company's first product was an automatic tufting gun for market validation, but its core innovation is a planned textile 'Station' platform using a proprietary AI agent to translate simple inputs like photos or drawings into machine-executable knitting patterns, significantly lowering the design barrier.

rss · 36kr - AI · Jul 7, 02:29

**Background**: The global DIY textile and knitting community is enormous, with dedicated hobbyists numbering in the tens of millions and a much broader potential audience of over a hundred million people. Traditional home knitting machines from the 1990s were purely mechanical and required significant skill. Integrating modern robotics, motion planning, and computer graphics into a consumer product represents a significant technical leap for this category, moving towards a 'put in material, get out product' desktop fabrication model.

<details><summary>References</summary>
<ul>
<li><a href="https://www.alibaba.com/showroom/home-weaving-machine.html">Home Weaving Machine - High Quality DIY Loom for Kids Images Domestic Weaving Machine - Automatic High-Speed Textile Loom Amazon.com: Weaving Machine Weaving Machine For Home Textile - SMIT Weaving machine home-AliExpress Home Weaving Machine Smart Air Jet Loom Making Fiberglass ... Zcvtbye Knitting Machine, 48 Needles, Smart Weaving Loom Kit ...</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/21245173537">软硬件一体化产品的优势及应用 - 知乎</a></li>
<li><a href="https://www.taobao.com/list/item/cTlzc0RqVnBUeXh4OHhXZ2llZUt5UT09.htm">tufting gun簇绒枪 地毯织枪 电动工具DIY戳戳绣 专用圈绒-淘宝Taobao ...</a></li>

</ul>
</details>

**Tags**: `#hardware`, `#startup`, `#consumer-electronics`, `#venture-capital`, `#textile-tech`

---