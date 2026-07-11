---
layout: default
title: "Horizon Summary: 2026-07-11 (EN)"
date: 2026-07-11
lang: en
---

> From 58 items, 10 important content pieces were selected

---

1. [Zhipu founder outlines post-Coding AI strategy in internal letter](#item-1) ⭐️ 8.0/10
2. [Stablecoin Issuer Circle Receives OCC Trust Bank Charter](#item-2) ⭐️ 8.0/10
3. [VultronRetriever model family released, topping MTEB leaderboard](#item-3) ⭐️ 8.0/10
4. [Ant: A New End-to-End JavaScript Ecosystem with Runtime, Tools, and Platform.](#item-4) ⭐️ 7.0/10
5. [Nvidia's GPU Financing Circular Structure Questioned as AI Boom Risk](#item-5) ⭐️ 7.0/10
6. [Geohot warns of AI enabling authoritarian control and information censorship by 2040.](#item-6) ⭐️ 7.0/10
7. [Meta disables Instagram AI deepfake feature after backlash](#item-7) ⭐️ 7.0/10
8. [ClickHouse Scales PgBouncer to 4x Throughput with SO_REUSEPORT and Peering](#item-8) ⭐️ 6.0/10
9. [CXMT IPO, SK Hynix US Debut, and OpenAI's ChatGPT Agent Launch](#item-9) ⭐️ 6.0/10
10. [ECB Official Warns AI Could Increase Inflation Volatility](#item-10) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Zhipu founder outlines post-Coding AI strategy in internal letter](https://36kr.com/p/3891132709206784?f=rss) ⭐️ 8.0/10

Zhipu's founder Tang Jie issued an internal letter titled 'The Great Wave Has Arrived,' announcing the company's 'Touch High' strategic plan. This plan shifts focus from AI coding successes to three new core capabilities: Long Horizon Tasks, Autonomous Agent Systems, and Self-Evolving AI. This signals a major strategic pivot for one of China's leading AI companies, moving beyond the current commercialization wave in AI coding to pioneer the next frontier of artificial general intelligence (AGI). It reflects an industry-wide shift from building chatbots to developing autonomous, reasoning agents capable of complex, long-term tasks. The strategic pivot follows Zhipu's massive market success, with its valuation increasing tenfold in six months to over one trillion HKD, surpassing Xiaomi, largely fueled by its bet on AI coding models like GLM-5.2. The new 'Touch High' plan prioritizes long-term R&D over short-term commercialization, focusing on AGI capabilities that the company believes will redefine industry boundaries.

rss · 36kr - AI · Jul 11, 11:28

**Background**: The letter references the 'DeepSeek R1' model as marking the end of the 'Chat paradigm,' suggesting that the exploration of conversational AI has matured. Zhipu, like Anthropic with its Claude models, bet early on enhancing AI's coding and reasoning abilities, viewing this as the next step toward more capable agents. MaaS (Model-as-a-Service) platforms, like Zhipu's, are a primary commercial model where companies pay to access powerful AI models via API.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.z.ai/guides/llm/glm-5.2">GLM - 5 . 2 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>
<li><a href="https://builtin.com/artificial-intelligence/deepseek-r1">What Is DeepSeek-R1? | Built In</a></li>
<li><a href="https://eu.36kr.com/en/p/3824235570631041">When Will AI Commercialization Drive Alibaba's Growth?</a></li>

</ul>
</details>

**Tags**: `#AI industry strategy`, `#large language models`, `#AI coding`, `#company analysis`, `#AI commercialization`

---

<a id="item-2"></a>
## [Stablecoin Issuer Circle Receives OCC Trust Bank Charter](https://36kr.com/newsflashes/3890740672838404?f=rss) ⭐️ 8.0/10

The U.S. Office of the Comptroller of the Currency (OCC) has approved Circle's application to establish a national trust bank, named Circle National Trust Bank, allowing the company to directly manage the reserves for its USDC stablecoin. This regulatory milestone allows a major stablecoin issuer to bring reserve management in-house, potentially increasing operational efficiency and setting a precedent for how digital asset companies integrate into the regulated financial system. The new charter is a national trust bank license, which permits reserve management but does not authorize Circle to conduct traditional commercial banking activities like accepting deposits or making loans.

rss · 36kr - AI · Jul 11, 05:10

**Background**: A national trust bank charter from the OCC has a more limited scope than a full commercial banking license, often sought by fintech and crypto companies for specific activities like asset custody. Stablecoins like USDC are digital tokens designed to maintain a stable value (typically pegged 1:1 to a fiat currency) by holding reserve assets such as cash and short-term government securities. Circle previously relied on third-party banks and custodians to hold these reserves supporting its over $73 billion USDC in circulation.

<details><summary>References</summary>
<ul>
<li><a href="https://phemex.com/blogs/trump-regulators-crypto-us-banking-system">Trump's OCC Is Pushing Crypto Into US Banking | Charters , Fed...</a></li>
<li><a href="https://www.bankingdive.com/news/paxos-seeks-occ-national-trust-charter-crypto-stablecoin/757621/">Paxos seeks OCC trust charter | Banking Dive</a></li>
<li><a href="https://www.circle.com/transparency">Transparency & Stability | Circle</a></li>

</ul>
</details>

**Tags**: `#stablecoin`, `#cryptocurrency`, `#banking-regulation`, `#Circle`, `#USDC`

---

<a id="item-3"></a>
## [VultronRetriever model family released, topping MTEB leaderboard](https://www.reddit.com/r/MachineLearning/comments/1utmxq8/vultronretriever_family_of_models_released_on/) ⭐️ 8.0/10

VultronRetriever, a new family of retrieval models, has been released on Hugging Face. The flagship model, VultronRetrieverPrime-8B, achieved the number one global ranking on the MTEB Leaderboard while offering a significantly smaller index footprint and higher throughput compared to previous leaders. This release is significant because it combines state-of-the-art retrieval performance with substantial efficiency gains, enabling powerful, fully offline applications on resource-constrained edge devices like smartphones. It represents a major step forward for deploying sophisticated AI retrieval capabilities outside of traditional cloud environments. The model family includes three variants: Prime (8B parameters), Core (4.5B), and Flash (0.8B), each ranking first in its respective class on MTEB. The models utilize the Hydra Architecture to provide both late-interaction retrieval and generation capabilities within a single model, and were trained with rigorously decontaminated datasets to ensure evaluation integrity.

reddit · r/MachineLearning · /u/madkimchi · Jul 11, 15:22

**Background**: The MTEB (Massive Text Embedding Benchmark) Leaderboard is a widely used benchmark for comparing the performance of text embedding and retrieval models across various tasks. Late interaction retrieval is a technique where queries and documents are processed separately and compared at a fine-grained, token-level, enabling precise semantic matching. The Hydra Architecture, referenced in the release, is a novel approach that unifies retrieval and generation in a single vision-language model by using dual attention heads.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2603.28554">[2603.28554] Hydra: Unifying Document Retrieval and Generation in a Single Vision-Language Model</a></li>
<li><a href="https://weaviate.io/blog/late-interaction-overview">An Overview of Late Interaction Retrieval Models... | Weaviate</a></li>
<li><a href="https://huggingface.co/blog/lyon-nlp-group/mteb-leaderboard-best-practices">MTEB Leaderboard : User guide and best practices</a></li>

</ul>
</details>

**Discussion**: As the Reddit discussion comments were not provided, a summary of community sentiment cannot be generated.

**Tags**: `#machine-learning`, `#retrieval-models`, `#MTEB`, `#edge-ai`, `#model-release`

---

<a id="item-4"></a>
## [Ant: A New End-to-End JavaScript Ecosystem with Runtime, Tools, and Platform.](https://antjs.org/) ⭐️ 7.0/10

The Ant project has evolved from a standalone JavaScript runtime into a comprehensive ecosystem that includes its own package manager (ants.land), a deployment platform, and a desktop application builder similar to Electron. It aims to provide a cohesive, all-in-one alternative to the fragmented JavaScript stack, which could simplify the developer experience and offer new choices beyond established players like Node.js, Deno, and Bun. The project is still in an early stage, and the author has acknowledged that it was initially built using a codebase derived from an existing AGPL-licensed engine, though it has since been rewritten.

hackernews · theMackabu · Jul 11, 20:07 · [Discussion](https://news.ycombinator.com/item?id=48875377)

**Background**: The JavaScript ecosystem is dominated by established runtimes like Node.js, with newer alternatives such as Deno and Bun gaining traction. Developers typically assemble tools like package managers (e.g., npm, yarn), bundlers, and deployment services separately. An end-to-end ecosystem like Ant attempts to integrate these components into a unified platform.

<details><summary>References</summary>
<ul>
<li><a href="https://betterstack.com/community/guides/scaling-nodejs/nodejs-vs-deno-vs-bun/">Node.js vs Deno vs Bun: Comparing JavaScript Runtimes | Better Stack Community</a></li>
<li><a href="https://ant.apache.org/">Apache Ant - Welcome</a></li>

</ul>
</details>

**Discussion**: The community discussion shows mixed sentiment: some users expressed skepticism about the project's trustworthiness and the author's claimed 'from-scratch' origin, citing past reliance on an AGPL codebase and a seemingly incomplete company structure. Others were intrigued by the rapid development pace and sought technical details on its performance claims compared to mature runtimes.

**Tags**: `#javascript-runtime`, `#ecosystem`, `#open-source`, `#developer-tools`, `#web-development`

---

<a id="item-5"></a>
## [Nvidia's GPU Financing Circular Structure Questioned as AI Boom Risk](https://io-fund.com/ai-stocks/nvidia-coreweave-nebius-circular-financing-gpu-boom) ⭐️ 7.0/10

An investigation reveals a financial loop where Nvidia invests equity in GPU cloud providers like CoreWeave, which in turn use that capital to purchase massive volumes of Nvidia's own GPUs, a pattern described as circular financing. This financing structure raises concerns that Nvidia could be artificially inflating demand for its GPUs and inflating a potential bubble in the AI infrastructure market, which would affect investors, data center operators, and the broader economy. Nvidia's $2 billion investment for a 9% stake in CoreWeave is relatively small compared to CoreWeave's projected $35 billion capital expenditure for 2026, suggesting the circular flow is a minor part of a much larger funding ecosystem.

hackernews · adletbalzhanov · Jul 11, 17:21 · [Discussion](https://news.ycombinator.com/item?id=48873836)

**Background**: GPU-as-a-Service (GPUaaS) is a cloud computing model where companies rent out access to powerful Graphics Processing Units (GPUs) for tasks like training AI models. CoreWeave and Nebius are leading 'neocloud' providers specializing in this service. Nvidia, the dominant designer of GPUs used for AI, has made equity investments in several such cloud startups, creating a complex supplier-customer relationship.

<details><summary>References</summary>
<ul>
<li><a href="https://io-fund.com/ai-stocks/nvidia-coreweave-nebius-circular-financing-gpu-boom">Nvidia, CoreWeave, and Nebius: Inside the Circular Financing of the GPU Boom</a></li>
<li><a href="https://www.spheron.network/blog/nvidia-neocloud-backstop-financing-circular-gpu-2026/">NVIDIA's Neocloud Backstop Financing Explained: What Circular GPU Financing Means for AI Teams in 2026 | Spheron Blog</a></li>
<li><a href="https://deploybase.ai/articles/coreweave-vs-nebius-gpuaas-ai-stocks-comparison">CoreWeave vs Nebius : GPUaaS AI Stocks Comparison | DeployBase</a></li>

</ul>
</details>

**Discussion**: Many commenters pushed back on the 'circular' label, arguing Nvidia's investment is a small hedge against hyperscaler power and that the real issue is the economic profitability of the massive GPU infrastructure build-out. Others raised serious concerns that the entire web of AI investment and debt could pose a systemic risk to the US economy, comparing it to the pre-2008 financial crisis.

**Tags**: `#AI infrastructure`, `#GPU financing`, `#Cloud computing`, `#Stock market`, `#Financial analysis`

---

<a id="item-6"></a>
## [Geohot warns of AI enabling authoritarian control and information censorship by 2040.](https://geohot.github.io//blog/jekyll/update/2026/07/11/ai-2040.html) ⭐️ 7.0/10

In a blog post, hardware hacker George Hotz (geohot) speculates that advanced AI systems could evolve from simple informational chatbots into tools for authoritarian regimes, capable of not just restricting information but also monitoring users for 'thoughtcrime' and subtly injecting ideological bias. The argument highlights a critical, speculative tension in AI ethics: while AI promises great utility, its potential integration into state surveillance and censorship could fundamentally threaten personal freedoms and privacy, drawing uncomfortable parallels to internet control debates. The post's core concern is about AI agents moving beyond passive information provision to active, real-world intervention and ideological enforcement, a scenario that commenters debated regarding its technical feasibility and the binary nature of 'freedom'.

hackernews · rvz · Jul 11, 18:04 · [Discussion](https://news.ycombinator.com/item?id=48874200)

**Background**: George Hotz is a well-known programmer and entrepreneur, founder of Comma.ai (self-driving tech) and TinyCorp. His blog post engages in philosophical speculation about the long-term societal impact of superintelligent AI, a common topic in AI safety and ethics circles.

**Discussion**: The community discussion was highly engaged and polarized. Some commenters shared the author's fear of AI being weaponized for mass surveillance and ideological control, while others criticized the argument as simplistic, pointing out that 'freedom' is not binary and that the real danger lies in AI agents performing harmful real-world actions, not just manipulating information.

**Tags**: `#AI ethics`, `#future of AI`, `#censorship`, `#privacy`, `#philosophy`

---

<a id="item-7"></a>
## [Meta disables Instagram AI deepfake feature after backlash](https://www.theverge.com/tech/964416/meta-instagram-ai-muse-image-deepfakes) ⭐️ 7.0/10

Meta has disabled an Instagram feature that allowed users to generate AI images based on public accounts' content simply by tagging them, following significant public backlash over privacy and consent concerns. This rapid reversal highlights the growing tension between the development of generative AI tools and the protection of user privacy and consent, setting a precedent for how platforms might handle similar features in the future. The original feature allowed AI-generated images to be created from the content of any public Instagram account without requiring the account owner's permission, which sparked widespread criticism.

rss · The Verge - AI · Jul 10, 23:49

**Background**: Generative AI tools can create realistic images, text, or other media, often by learning patterns from large datasets. Deepfakes specifically refer to AI-generated synthetic media, typically images or videos, that convincingly replace one person's likeness with another. The debate around such features centers on balancing technological innovation with ethical considerations like consent and data privacy.

**Discussion**: The public backlash and Meta's quick response suggest widespread community concern over the potential misuse of personal content and the violation of consent principles in AI applications, with many likely viewing this as a necessary step to protect user rights.

**Tags**: `#AI ethics`, `#content moderation`, `#privacy`, `#generative AI`, `#platform policy`

---

<a id="item-8"></a>
## [ClickHouse Scales PgBouncer to 4x Throughput with SO_REUSEPORT and Peering](https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres) ⭐️ 6.0/10

ClickHouse detailed how they achieved a 4x throughput increase in their managed PostgreSQL's PgBouncer connection pooler by implementing the SO_REUSEPORT socket option and enabling peering for better load distribution and query cancellation. This optimization allows a single PgBouncer instance to handle significantly more concurrent database connections, which is crucial for high-performance applications and managed database services seeking to improve efficiency and scalability. The key techniques are using the SO_REUSEPORT socket option to allow multiple worker processes to accept connections directly from the kernel and enabling PgBouncer's peering feature so that processes can forward query cancellation requests to the correct session owner.

hackernews · saisrirampur · Jul 11, 15:28 · [Discussion](https://news.ycombinator.com/item?id=48872874)

**Background**: PgBouncer is a popular, lightweight connection pooler for PostgreSQL that manages and reuses database connections to reduce overhead. The SO_REUSEPORT socket option is a Linux kernel feature that allows multiple sockets to bind to the same IP address and port, enabling the kernel to distribute incoming connections among them for better load balancing. Peering in PgBouncer is a feature where multiple PgBouncer processes can communicate with each other to maintain a consistent view of client sessions, which is essential for correctly handling session-specific operations like query cancellation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.f5.com/company/blog/nginx/socket-sharding-nginx-release-1-9-1">Socket Sharding in NGINX Release 1.9.1 | F5</a></li>
<li><a href="https://www.pgbouncer.org/config.html">PgBouncer config</a></li>
<li><a href="https://pgstef.github.io/talks/en/20250912_PGDayLowlands_PgBouncer-at-scale.pdf">PgBouncer at scale</a></li>

</ul>
</details>

**Discussion**: Community discussion included suggestions for alternative tools like Yandex's Odyssey and pgdog, questions about the simplicity of setting up peering in PostgreSQL, and shared experiences of running PgBouncer on Kubernetes for similar scalability.

**Tags**: `#postgresql`, `#connection-pooling`, `#performance`, `#infrastructure`

---

<a id="item-9"></a>
## [CXMT IPO, SK Hynix US Debut, and OpenAI's ChatGPT Agent Launch](https://36kr.com/p/3890553690192384?f=rss) ⭐️ 6.0/10

Chinese memory chip maker CXMT announced a major underwriter syndicate for its upcoming IPO, while South Korea's SK Hynix saw its US-listed shares surge nearly 13% on their Nasdaq debut. Separately, OpenAI launched ChatGPT Work, an AI agent powered by GPT-5.6 designed to automate complex tasks across applications. SK Hynix's successful US listing provides global investors with a direct channel to invest in the booming AI infrastructure sector, while CXMT's IPO marks a significant milestone for China's semiconductor self-sufficiency ambitions. OpenAI's agent launch signals a shift towards AI that can autonomously execute complex, long-duration work tasks, potentially transforming productivity software. SK Hynix raised approximately $26.5 billion through its ADR offering on Nasdaq, with shares closing up 12.8% on the first day. CXMT's IPO is scheduled for July 16 with a syndicate of six major Chinese brokerages. ChatGPT Work can operate for hours on end, integrating with the ChatGPT desktop app to produce deliverables like tables, slides, and web applications.

rss · 36kr - AI · Jul 11, 01:24

**Background**: SK Hynix is the world's second-largest memory chip manufacturer and a key supplier for AI hardware, particularly high-bandwidth memory for GPUs. CXMT, officially known as ChangXin Memory Technologies, is China's leading DRAM chipmaker and is often called the nation's first domestically-backed memory chip company to attempt a major IPO. American Depositary Receipts (ADRs) are certificates issued by US banks that represent shares in foreign companies, allowing those companies to be traded on US stock exchanges.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/features/2026-07-09/china-s-cxmt-chipmaker-eyes-ipo-to-challenge-samsung-sk-hynix-micron">China’s CXMT Chipmaker Eyes IPO to Challenge... - Bloomberg</a></li>
<li><a href="https://openai-dotcom-git-main-openai.vercel.app/index/chatgpt-for-your-most-ambitious-work/">ChatGPT is now a partner for your most ambitious work | OpenAI</a></li>
<li><a href="https://www.investopedia.com/terms/a/adr.asp">investopedia.com/terms/a/ adr .asp</a></li>

</ul>
</details>

**Tags**: `#technology-news`, `#semiconductor`, `#AI`, `#IPO`, `#ChineseTech`

---

<a id="item-10"></a>
## [ECB Official Warns AI Could Increase Inflation Volatility](https://36kr.com/newsflashes/3890739624540680?f=rss) ⭐️ 6.0/10

European Central Bank Governing Council member Emmanuel Moulin stated that artificial intelligence could increase inflation volatility due to its simultaneous effects on both supply and demand. This perspective from a senior central banker highlights a complex macroeconomic challenge, suggesting that AI's disruptive effects could complicate monetary policy aimed at stabilizing prices. Moulin specifically noted that AI might have an inflationary short-term effect due to increased capital expenditure, but could later suppress inflation as productivity gains materialize.

rss · 36kr - AI · Jul 11, 04:52

**Background**: Inflation volatility refers to the degree of fluctuation in the rate of price increases over time. Central banks like the ECB monitor this carefully, as stable inflation is typically a primary monetary policy goal. The macroeconomic impact of AI is a growing area of study, as its dual effects on productivity (supply-side) and new demand for goods/services and energy can create complex, non-linear dynamics.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ecb.europa.eu/press/key/date/2026/html/ecb.sp260706~b81aa4e329.en.html">AI and monetary policy | European Central Bank</a></li>
<li><a href="https://www.imf.org/en/Blogs/Articles/2023/10/04/how-managing-inflation-expectations-can-help-economies-achieve-a-softer-landing">How Managing Inflation Expectations Can Help Economies Achieve...</a></li>

</ul>
</details>

**Tags**: `#AI economics`, `#macroeconomics`, `#inflation`, `#central banking`, `#societal impact`

---