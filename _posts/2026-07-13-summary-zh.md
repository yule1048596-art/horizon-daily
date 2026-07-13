---
layout: default
title: "Horizon Summary: 2026-07-13 (ZH)"
date: 2026-07-13
lang: zh
---

> 从 96 条内容中筛选出 15 条重要资讯。

---

1. [三星健康应用威胁：若用户拒绝 AI 训练，将删除其健康数据](#item-1) ⭐️ 8.0/10
2. [苹果 SpeechAnalyzer API 基准测试显示其在实时转录速度上超越 Whisper](#item-2) ⭐️ 7.0/10
3. [Climate.gov 网站数据被销毁后，通过开放数据存档努力得以保存。](#item-3) ⭐️ 7.0/10
4. [对 15 款旧 GPU 进行基准测试，评估其运行现代 AI 工作负载的性价比](#item-4) ⭐️ 7.0/10
5. [维基百科暂时避免英国《在线安全法》的严格监管分类](#item-5) ⭐️ 7.0/10
6. [iOS 27 公开测试版预览：Siri AI 如何改变 iPhone 使用方式](#item-6) ⭐️ 7.0/10
7. [字节跳动利用 Seed AI 的世界模型团队探索自动驾驶](#item-7) ⭐️ 7.0/10
8. [苹果加速 AI 芯片研发，跳过 M6 变体直接开发 M7](#item-8) ⭐️ 7.0/10
9. [英特尔追加 50 亿欧元投资以扩大爱尔兰 AI 芯片工厂产能](#item-9) ⭐️ 7.0/10
10. [DOOMQL：一款完全使用 SQLite SQL 查询构建的类《毁灭战士》游戏引擎。](#item-10) ⭐️ 6.0/10
11. [西蒙·威尔森分享 Datasette 项目的 GitHub 代码频率图，展示 AI 编码代理的影响。](#item-11) ⭐️ 6.0/10
12. [直接责任人（DRI）](#item-12) ⭐️ 6.0/10
13. [前大疆工程师创业公司获近 5000 万元融资，研发消费级四足机器人。](#item-13) ⭐️ 6.0/10
14. [Om AI 推出 VLX：全球首个面向物理 AI 的端侧流式多模态模型](#item-14) ⭐️ 6.0/10
15. [零差云控完成数亿元 C++轮融资，用于人形机器人关节产能扩张](#item-15) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [三星健康应用威胁：若用户拒绝 AI 训练，将删除其健康数据](https://neow.in/cWsyMTV3) ⭐️ 8.0/10

三星健康应用实施了一项政策，如果用户选择退出其数据用于 AI 训练，该应用将删除用户的个人健康数据，包括睡眠、用药、医疗记录和月经周期跟踪详情。 这种做法引发了重大的隐私和用户同意问题，因为它本质上是在胁迫用户交出敏感健康数据用于 AI 开发，以换取设备功能的全部访问权限，为消费技术领域树立了一个令人不安的先例。 用户报告称，退出 AI 训练会导致其 Galaxy Watch 的许多功能无法使用，这引发了用户的沮丧，并质疑三星是否应退还部分设备费用。该政策涵盖了一系列广泛的敏感个人健康类别。

hackernews · bundie · 7月13日 20:01 · [社区讨论](https://news.ycombinator.com/item?id=48897991)

**背景**: 三星健康是一款主要的健康与健身追踪应用，可与 Galaxy Watch 等设备配对使用。将用户数据用于训练人工智能模型已成为大型科技公司中常见但颇具争议的做法，通常通过更新服务条款来使其合法化。这种方法与允许用户在不丧失核心功能的情况下选择退出的模式形成了对比。

**社区讨论**: 社区反应普遍负面，用户对政策的胁迫性质及其对设备可用性的影响表示愤怒。评论者将此与谷歌等公司的其他敌视用户的做法相提并论，同时有人指出三星会删除敏感数据而不是使用它，算是一个“唯一的亮点”。

**标签**: `#privacy`, `#data-ethics`, `#consumer-tech`, `#health-data`, `#user-consent`

---

<a id="item-2"></a>
## [苹果 SpeechAnalyzer API 基准测试显示其在实时转录速度上超越 Whisper](https://get-inscribe.com/blog/apple-speech-api-benchmark.html) ⭐️ 7.0/10

一项基准测试比较显示，苹果为 iOS 26 推出的新 SpeechAnalyzer API 在实时转录任务上比 OpenAI 的 Whisper 模型更快，同时保持了相当的准确性。 这一进展标志着苹果正致力于推动高性能的设备端 AI 语音处理，这可能减少对云端 API 的依赖，并对那些作为 Whisper 等模型包装器的第三方应用市场构成威胁。 SpeechAnalyzer API 随 iOS 26 推出，使用 Swift 构建，完全在设备端运行以保护隐私，并支持长音频和远距离录音等功能。该基准测试专门针对 Whisper-Large-V2 模型进行了比较。

hackernews · get-inscribe · 7月13日 16:06 · [社区讨论](https://news.ycombinator.com/item?id=48894752)

**背景**: Whisper 是由 OpenAI 开发的流行开源自动语音识别（ASR）模型，以其在多语言环境下的准确性而闻名。苹果此前的语音 API 是 SFSpeechRecognizer，新的 SpeechAnalyzer 代表了苹果生态系统内为开发者提供的速度和灵活性方面的重大升级。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.apple.com/documentation/speech/speechanalyzer">SpeechAnalyzer | Apple Developer Documentation</a></li>
<li><a href="https://developer.apple.com/videos/play/wwdc2025/277/">Bring advanced speech-to-text to your app with SpeechAnalyzer</a></li>
<li><a href="https://en.wikipedia.org/wiki/Whisper_(speech_recognition_system)">Whisper (speech recognition system) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区讨论观点不一：一些用户指出，虽然速度提升对实时转录很有价值，但由于 Whisper 的准确性，他们可能会继续在非实时任务中使用它。其他人则认为基准测试应包含更现代的替代模型，如英伟达的 Nemotron 或 Mistral 的 Voxtral，并预测苹果的原生 API 很可能会使许多第三方‘包装器’应用变得多余。一位开发者分享了将其集成到自己应用中的尝试，还有用户推荐了 Willow 等替代工具以获得更好的转录质量。

**标签**: `#speech-recognition`, `#apple`, `#api-benchmark`, `#ai-inference`, `#developer-tools`

---

<a id="item-3"></a>
## [Climate.gov 网站数据被销毁后，通过开放数据存档努力得以保存。](https://werd.io/climate-gov-was-destroyed-open-data-saved-it/) ⭐️ 7.0/10

在美国政府 Climate.gov 网站被摧毁后，其数据通过开放数据倡议成功保存，避免了关键气候信息的永久丢失。 这一事件凸显了去中心化存档和公共领域原则在保护政府数据免受政治或制度变更影响方面的关键作用，确保了公众能长期获取宝贵的科学资源。 此次保存依赖于社区驱动的努力和现有的开放数据存档，因为该网站自身的基础设施已停止运行；未来的可持续性，特别是持续数据收集方面，仍然是一个挑战，经常在资助模式的讨论中被提及。

hackernews · benwerd · 7月13日 19:57 · [社区讨论](https://news.ycombinator.com/item?id=48897945)

**背景**: Climate.gov 是一个提供权威气候科学数据、工具和资源的美国联邦网站。开放数据是指可自由供任何人使用、再利用和再分发的数据，其保存是数字遗产领域的一个关键关切。去中心化存档方法，例如使用 IPFS 或 Filecoin 等协议的方法，将数据分布在网络中，以防止单点故障和审查。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://libguides.gwu.edu/data-preservation/data-preservation-tools">Data Preservation and Data Sources: Data Preservation Tools</a></li>
<li><a href="https://medium.com/@dandy_latte_pig_253/project-description-kyve-is-a-decentralized-data-archiving-protocol-bfb24199496f">PROJECT DESCRIPTION KYVE is a decentralized data archiving ...</a></li>
<li><a href="https://www.filecoin.io/">World's Largest Decentralized Storage Network for Humanity's Data</a></li>

</ul>
</details>

**社区讨论**: 社区讨论集中于政府数据作为公共领域的合法性、维持持续数据收集与归档历史数据之间的后勤挑战，以及默认使用 IPFS 等去中心化存储托管政府内容的技术可行性。一些评论者质疑依赖捐赠来维持他们认为应由税收资金支持的功能。

**标签**: `#open-data`, `#digital-preservation`, `#government-transparency`, `#data-archiving`, `#climate-data`

---

<a id="item-4"></a>
## [对 15 款旧 GPU 进行基准测试，评估其运行现代 AI 工作负载的性价比](https://esologic.com/benchmarking-tesla-gpus/) ⭐️ 7.0/10

一项全面的基准测试对 15 款较旧、低成本的“电子垃圾”GPU 进行了评估，测试它们在运行现代大语言模型（LLMs）及其他 AI 推理任务时的性能表现。 这项研究对注重成本的开发者和研究人员意义重大，它证明了廉价、老旧的硬件在运行现代 AI 工作负载时仍然可行，这有助于降低入门门槛并促进可持续计算实践。 基准测试侧重于大语言模型的实际推理性能指标，社区讨论则揭示了具体的真实配置案例，例如使用多块 Tesla P4 GPU 构建虚拟 48GB 显存配置，以运行 200 亿至 300 亿参数的模型。

hackernews · eso_logic · 7月13日 13:48 · [社区讨论](https://news.ycombinator.com/item?id=48892638)

**背景**: 现代 AI 工作负载，尤其是大语言模型推理，传统上需要昂贵的高端 GPU 和充足的显存。像 NVIDIA Tesla 系列这样的“电子垃圾”或旧数据中心 GPU 虽已退役，但能以极低成本提供可观的计算能力和显存。诸如 llama.cpp 之类的工具通过使用量化技术（例如 Q4KM）来降低内存和计算需求，从而使这些模型能够在此类硬件上高效运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lambda.ai/gpu-benchmarks">GPU Benchmarks for Deep Learning | Lambda</a></li>
<li><a href="https://inferensys.com/guides/green-ai-and-computational-efficiency/how-to-design-for-hardware-longevity-and-reduce-e-waste">How to Design for Hardware Longevity and Reduce E-Waste</a></li>
<li><a href="https://arxiv.org/html/2604.09048">Watt Counts: Energy-Aware Benchmark for Sustainable LLM ...</a></li>

</ul>
</details>

**社区讨论**: 社区成员积极分享替代配置和性能细节；例如，一位用户描述了一个包含六块 Tesla P4 GPU 的系统，能在 200 亿至 300 亿参数的模型上实现每秒 7 至 12 个 token 的输出速度，另一位用户则推荐了更新的 Radeon Pro V620 显卡，因其有更好的支持和速度。部分评论还对功耗数据表示兴趣，并指出文章图片加载量过大。

**标签**: `#GPU benchmarking`, `#AI hardware`, `#cost-effective computing`, `#LLM inference`, `#e-waste`

---

<a id="item-5"></a>
## [维基百科暂时避免英国《在线安全法》的严格监管分类](https://en.wikipedia.org/wiki/Wikipedia:Wikipedia_Signpost/2026-07-13/Special_report) ⭐️ 7.0/10

英国通信监管机构 Ofcom 同意维基百科目前不符合《在线安全法》中一类服务的资格，从而暂时避免了最严格的监管要求。 这一决定意义重大，因为一类服务的分类将迫使维基百科实施代价高昂且可能侵蚀匿名性的措施（如年龄验证），从而威胁其由志愿者驱动的开放知识模式。 维基百科的暂时豁免是基于对法律的一种新颖解释，但维基媒体基金会警告称，未来的一类服务分类对该平台及其全球志愿者社区而言仍然是一个生存威胁。

hackernews · hn_acker · 7月13日 15:59 · [社区讨论](https://news.ycombinator.com/item?id=48894671)

**背景**: 英国《2023 年在线安全法》为在线服务创建了一个分层责任体系，其中一类服务承担最广泛的义务，可能包括关于用户身份验证和内容审核透明度的额外责任。Ofcom 是负责实施和执行这些规则的英国监管机构。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wikimediafoundation.org/news/2026/07/10/wikimedia-foundation-challenges-uk-online-safety-act-regulations/">Wikimedia Foundation Challenges UK Online Safety Act ...</a></li>
<li><a href="https://www.ofcom.org.uk/online-safety/illegal-and-harmful-content/additional-duties-for-categorised-online-services">Implementing the Online Safety Act: Additional duties for ...</a></li>
<li><a href="https://www.legislation.gov.uk/uksi/2025/226/made">The Online Safety Act 2023 (Category 1, Category 2A and ...</a></li>

</ul>
</details>

**社区讨论**: 社区讨论对政府越权和身份验证的必要性表达了强烈质疑，评论者认为此类要求应成为例外而非常态。一些用户质疑英国法律传统中“做出例外”的做法与美国严格解释法律的做法之间的差异，另一些用户则警告称，现在若不挑战监管越权行为，可能导致数字自由受到永久性限制。

**标签**: `#internet-regulation`, `#online-safety`, `#free-speech`, `#policy`, `#wikipedia`

---

<a id="item-6"></a>
## [iOS 27 公开测试版预览：Siri AI 如何改变 iPhone 使用方式](https://www.theverge.com/tech/964714/siri-ai-public-beta-preview-ios-27-hands-on) ⭐️ 7.0/10

苹果发布了 iOS 27 的首个公开测试版，其中包含由人工智能驱动的 Siri 重大更新。《The Verge》的实地测试预览表明，这些变化已经在影响 iPhone 的实际使用习惯。 此次公开测试版的发布表明，苹果为其核心语音助手打造的最新 AI 增强功能正从开发者测试阶段进入主流用户评估阶段，这可能会重塑数百万 iPhone 用户日常与设备交互的方式。 作者自 6 月初以来一直在测试该操作系统，以评估其是否达到苹果主题演讲中的承诺，这表明评测是基于长期使用而非简短体验。文章指出，今年的 iOS 升级被形容为'Snow Leopard'类型的更新，暗示其重点在于优化和底层改进。

rss · The Verge - AI · 7月13日 20:43

**背景**: Siri 是苹果集成在其操作系统中的 AI 驱动虚拟助手。iOS 是运行在 iPhone 上的移动操作系统。'公开测试版'是指在最终稳定版发布前向公众开放的软件预发布版本。'Snow Leopard 更新'这一说法源自 macOS 10.6 Snow Leopard，这是苹果的一个操作系统版本，以其专注于性能、稳定性和优化而非重大新功能而闻名。

**标签**: `#iOS`, `#Siri`, `#AI`, `#Apple`, `#mobile OS`

---

<a id="item-7"></a>
## [字节跳动利用 Seed AI 的世界模型团队探索自动驾驶](https://36kr.com/p/3893815451417347?f=rss) ⭐️ 7.0/10

字节跳动正探索进入自动驾驶领域，该项目由旗下 Seed AI 部门周畅的世界模型团队负责，目标应用场景包括无人物流。 字节跳动这样的科技巨头凭借强大的 AI 资源和人才进入自动驾驶领域，可能会颠覆行业竞争格局，尤其是在世界模型已成为技术共识的当下。 公司官方回应否认有做智能驾驶业务的计划，但报道称该项目处于早期筹备状态，并已吸引来自头部自动驾驶公司的人才；其团队的世界模型专长被认为可直接应用。

rss · 36kr - AI · 7月13日 08:34

**背景**: 世界模型是一种旨在学习理解和预测物理世界动态的 AI 系统，这对于自动驾驶汽车模拟和规划驾驶行为至关重要。字节跳动的 Seed 团队成立于 2023 年，是负责大语言模型、多模态模型和世界模型等研究的核心 AI 部门。物理 AI 是指在真实物理世界中运行并与之互动的人工智能，自动驾驶和机器人（具身智能）是其两大主要应用领域。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://seed.bytedance.com/">ByteDance Seed</a></li>
<li><a href="https://arxiv.org/abs/2501.11260">[2501.11260] A Survey of World Models for Autonomous Driving</a></li>

</ul>
</details>

**标签**: `#autonomous-driving`, `#world-models`, `#bytedance`, `#physical-AI`, `#industry-competition`

---

<a id="item-8"></a>
## [苹果加速 AI 芯片研发，跳过 M6 变体直接开发 M7](https://36kr.com/newsflashes/3894068327759108?f=rss) ⭐️ 7.0/10

据报道，苹果正调整其 Mac 芯片路线图，计划跳过原定的 M6 Pro、M6 Max 和 M6 Ultra 等高端版本，以加速推进 M7 系列芯片的研发，其中 M7 Ultra 预计于 2028 年推出，其目标是在 AI 性能上接近英伟达 Blackwell 等专用 AI 加速器。 这一战略转变标志着苹果将其芯片研发重心大幅转向 AI 能力，直接挑战英伟达在 AI 加速器市场的主导地位，并可能重塑消费设备和数据中心 AI 硬件的竞争格局。 M7 Ultra 芯片预计采用台积电的 1.4 纳米制程节点，并将作为苹果下一代 AI 服务器芯片的基础，而能力更强的 M8 及后续芯片也已在研发之中。

rss · 36kr - AI · 7月13日 12:51

**背景**: 自 M1 芯片以来，苹果的 M 系列芯片一直遵循着一致的发布模式，即在基础款芯片之后，通常会在同一代内推出 Pro、Max 和 Ultra 等变体，以满足不同性能层级的需求。英伟达的 Blackwell 架构是其面向数据中心和高性能计算的最新一代 AI 专用 GPU。台积电的 1.4 纳米（A14）制程节点是一项未来的先进制造技术，有望在性能、功耗效率和晶体管密度方面带来显著提升。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.techspot.com/news/113085-apple-next-big-mac-leap-could-skip-m6.html">Apple is reportedly skipping M6 Pro, Max, and Ultra chips to ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Blackwell_(microarchitecture)">Blackwell (microarchitecture) - Wikipedia</a></li>
<li><a href="https://www.tweaktown.com/news/107877/tsmcs-next-gen-a14-1-4nm-process-node-is-progressing-smoothly-and-is-ahead-of-schedule/index.html">TSMC's next-gen A14 ( 1 . 4 nm ) process node is 'progressing smoothly...</a></li>

</ul>
</details>

**标签**: `#Apple Silicon`, `#AI Hardware`, `#Chip Architecture`, `#Mac`, `#NVIDIA`

---

<a id="item-9"></a>
## [英特尔追加 50 亿欧元投资以扩大爱尔兰 AI 芯片工厂产能](https://36kr.com/newsflashes/3894027379899655?f=rss) ⭐️ 7.0/10

英特尔宣布将向其位于爱尔兰莱克斯利普的园区追加投资 50 亿欧元（约 57 亿美元），用于扩大先进芯片制造能力，以满足人工智能和高性能计算需求。 这项重大资本投资反映了英特尔重夺制造业领导地位并在蓬勃发展的 AI 芯片市场竞争的战略推动，将直接影响数据中心基础设施和全球半导体供应链。 资金将用于升级现有设施、安装先进制造设备并扩建自动化系统，以提升 Intel 3 制程节点芯片的产能，包括 Intel Xeon 6 及下一代服务器处理器，同时扩大研发活动。

rss · 36kr - AI · 7月13日 12:09

**背景**: 英特尔的'Intel 3'是其 3 纳米级别的制程技术，是高性能数据中心和网络芯片的关键节点。Xeon 6 处理器是英特尔最新服务器 CPU 系列的一部分，旨在整合服务器机架并提升每瓦性能。这项投资符合行业趋势，即主要芯片制造商正在积极扩大 AI 加速器和高性能计算处理器的产能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://semiwiki.com/wikis/industry-wikis/intel-3nm-process-node-intel-3-wiki/">Intel 3 Process Technology Wiki - Semiwiki</a></li>
<li><a href="https://www.allaboutcircuits.com/news/intel-launches-new-xeon-6-data-center-processor-family-computex-2024/">Intel Launches New Data Center Processor Family at Computex 2024...</a></li>
<li><a href="https://en.wikipedia.org/wiki/3_nm_process">3 nm process - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI hardware`, `#semiconductor manufacturing`, `#Intel`, `#investment`, `#high-performance computing`

---

<a id="item-10"></a>
## [DOOMQL：一款完全使用 SQLite SQL 查询构建的类《毁灭战士》游戏引擎。](https://simonwillison.net/2026/Jul/13/doomql/#atom-everything) ⭐️ 6.0/10

一个名为 DOOMQL 的创意演示项目使用了 GPT-5.6 Sol AI 模型构建，它将 SQLite 用作完整的游戏引擎来运行一款类《毁灭战士》游戏，其中移动、碰撞、敌人和渲染均由 SQL 查询处理。 这个项目以一种有趣且非常规的方式展示了 SQL 的计算能力以及 GPT-5.6 等现代 AI 模型的能力，启发了关于如何将数据库语言用于其传统角色之外领域的创造性思维。 该游戏被实现为一个 Python 终端脚本，使用了一个巨大的 SQL 查询和递归通用表表达式（CTE）来实现光线追踪器，并且它在执行时会创建一个 SQLite 数据库文件，可以用 Datasette 等工具进行探索。

rss · Simon Willison · 7月13日 22:34

**背景**: SQLite 是一个流行的、自包含的、无服务器的 SQL 数据库引擎，用于许多应用程序中的本地数据存储。“光线追踪”是一种模拟光线物理行为来生成图像的渲染技术，常用于 3D 图形。文中提到的 uv 包管理器是一个用 Rust 编写的现代高性能 Python 开发工具，可作为 pip 的快速替代品。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/previewing-gpt-5-6-sol/">Previewing GPT‑5.6 Sol: a next-generation model - OpenAI</a></li>
<li><a href="https://github.com/astral-sh/uv">GitHub - astral-sh/uv: An extremely fast Python package and ... Installation | uv - Astral uv · PyPI Python UV: The Ultimate Guide to the Fastest Python Package ... uv: A Complete Guide to Python's Fastest Package Manager Managing Python Projects With uv: An All-in-One Solution</a></li>

</ul>
</details>

**标签**: `#SQL`, `#game-development`, `#creative-coding`, `#SQLite`, `#demo`

---

<a id="item-11"></a>
## [西蒙·威尔森分享 Datasette 项目的 GitHub 代码频率图，展示 AI 编码代理的影响。](https://simonwillison.net/2026/Jul/13/datasette-code-frequency/#atom-everything) ⭐️ 6.0/10

西蒙·威尔森发布了他 Datasette 开源项目的 GitHub 代码频率图，显示在 2026 年代码活动出现巨大峰值，他将此归因于使用了 Opus 4.8 和 GPT-5.5 等先进的 AI 编码代理和模型。 这为 AI 编码助手如何能显著放大个人开发者的产出量提供了一个具体、数据驱动的可视化证据，为关于 AI 对软件开发生产力影响的持续讨论提供了一个切实的衡量指标。 图表显示，2026 年某一周出现了创纪录的 37,022 行代码添加峰值，作者将其直接与 Opus 4.8、GPT-5.5 和 Fable 5 等 AI 模型的使用联系起来，表明从间歇性的人工驱动活动转变为更频繁的、由 AI 放大的活动。

rss · Simon Willison · 7月13日 21:45

**背景**: Datasette 是一个流行的开源 Python 工具，用于探索和发布数据，可以将数据集转化为交互式网站和 API。GitHub 的代码频率图是一个标准的仓库指标，它可视化展示了项目历史上每周的代码增删量，常被用来发现开发趋势或重大重构事件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.github.com/en/repositories/viewing-activity-and-data-for-your-repository/analyzing-changes-to-a-repositorys-content">Analyzing changes to a repository's content - GitHub Docs</a></li>
<li><a href="https://opensources.dev/resource/datasette">datasette — opensources .dev</a></li>
<li><a href="https://agentic.ai/">Agentic AI Tools Directory — Find AI That Actually Does Things</a></li>

</ul>
</details>

**标签**: `#AI-assisted development`, `#open source`, `#GitHub metrics`, `#developer productivity`

---

<a id="item-12"></a>
## [直接责任人（DRI）](https://simonwillison.net/2026/Jul/12/directly-responsible-individuals/#atom-everything) ⭐️ 6.0/10

西蒙·威利森探讨了直接责任人（DRI）的概念，他认为人工智能不应被指定为 DRI，因为责任追究始终是人类独有的特质。

rss · Simon Willison · 7月12日 23:57

**标签**: `#AI ethics`, `#organizational management`, `#LLM agents`, `#accountability`, `#software engineering`

---

<a id="item-13"></a>
## [前大疆工程师创业公司获近 5000 万元融资，研发消费级四足机器人。](https://36kr.com/p/3893473722514181?f=rss) ⭐️ 6.0/10

由前大疆工程师和香港中文大学校友创立的光之跃迁科技已完成近五千万元天使轮融资，由正轩领投，用于产品研发、算法迭代及量产准备。公司计划在 2027 年 CES 展会上正式发布产品。 这标志着消费级机器人市场正从娱乐陪伴向实用工具转型，专注于解决搬运、辅助行动等真实户外场景的体力劳动需求。聚焦于非结构化环境有助于将四足机器人从新奇玩具发展为具备实际生产力的消费装备，开辟新的市场品类。 公司正在构建一个用于全地形辅助的四层智能架构，并计划推出适应不同地形（城市、轻城市、户外）的产品线。技术创新包括可从原始视频学习运动策略的 LMV 框架，以及通过优化设计将关节模组零部件从约 18 个精简至 11 个的系统性硬件降本策略。

rss · 36kr - AI · 7月13日 02:47

**背景**: 四足机器人是一种足式机器人，相比轮式平台在崎岖不平的地形上具有更好的机动性，适合户外环境。强化学习（RL）是训练其运动控制策略的关键人工智能技术，通过模拟或真实环境中的试错学习实现稳定行走。'消费级'通常意味着相比工业或研究型号，更注重低成本、易用性和面向家庭的应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hub.baai.ac.cn/view/7863">《智源周刊：强化学习》第5期：强化学习应用之机器人 - 智源社区</a></li>
<li><a href="https://www.leikeji.com/article/70715">消 费 级 最强：魔 法 原子发布MagicDog-W轮式 四 足 机 器 人 - 雷科技</a></li>
<li><a href="https://www.agilex.ai/chassis/3">120KG负载履带式全地形移动机器人底盘 | BUNKER PRO 2.0 | 松灵机器人</a></li>

</ul>
</details>

**标签**: `#robotics`, `#startups`, `#consumer electronics`, `#venture capital`, `#AI`

---

<a id="item-14"></a>
## [Om AI 推出 VLX：全球首个面向物理 AI 的端侧流式多模态模型](https://36kr.com/p/3893445208717826?f=rss) ⭐️ 6.0/10

Om AI 推出了 VLX 系列模型，该公司将其描述为全球首个为物理 AI 设计的端侧原生流式多模态模型，声称能为机器人、无人机等设备实现完整的感知-定位-决策闭环。 这一进展可能代表了物理 AI 架构的转变，它通过在设备端而非云端处理连续的视频流，从而可能为机器人和其他边缘设备在延迟和连接性至关重要的应用中实现实时、自主操作。 VLX 系列包含三个模型（VLX-Flow、VLX-Seek、VLX-Go），旨在完全在边缘设备上运行，无需依赖云端，并且该公司声称已取得商业成功，营收达到亿元人民币级别。

rss · 36kr - AI · 7月13日 02:39

**背景**: 物理 AI 是指在物理世界中进行感知、推理和行动的人工智能系统，常见于机器人、自动驾驶汽车和无人机等领域。该领域正在探索多种技术路线，如视觉-语言-动作（VLA）模型和世界模型。边缘计算是指在设备本身本地处理数据，而不是将其发送到远程数据中心，这对于需要低延迟或间歇性连接的应用至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ai-market-watch.com/news/om-ai-releases-first-end-side-streaming-multimodal-model-for-physical-world-at-c-1q5dow">**Om AI launches VLX, world’s first end-side streaming ...</a></li>
<li><a href="https://www.cnet.com/tech/services-and-software/physical-ai/">Physical AI Is Already Here. How It Works and What's Coming ...</a></li>
<li><a href="https://github.com/om-ai-lab/VLX-Flow">om-ai-lab/VLX-Flow - GitHub</a></li>

</ul>
</details>

**标签**: `#multimodal AI`, `#edge computing`, `#physical AI`, `#robotics`, `#model architecture`

---

<a id="item-15"></a>
## [零差云控完成数亿元 C++轮融资，用于人形机器人关节产能扩张](https://36kr.com/p/3885232033378308?f=rss) ⭐️ 6.0/10

零差云控近日完成由同创伟业领投的数亿元 C++轮融资，用于扩充机器人精密关节产能和布局全球市场。 此次大额融资表明投资者对人形机器人核心供应链的信心强劲，也标志着在需求激增的背景下，提升可靠零部件的规模化产能已成为行业的关键瓶颈。 公司 2025 年营收同比增长超过 100%，其中人形机器人订单贡献约 65%的增速；其通过模块化集成应对人形机器人设计的“不可能三角”，将关节轴向长度较行业通用方案缩减 44%，整机重量下降超两成。

rss · 36kr - AI · 7月13日 02:37

**背景**: 人形机器人开发面临一个根本性的设计挑战，即“不可能三角”——在物理上难以同时实现类人的灵活性、强大的负载能力和紧凑的人体尺寸。零差云控成立于 2016 年，专注于一体化机器人关节模组，旨在将这些核心部件标准化，从而简化组装并降低机器人制造商的成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.honpine.com/Robot-Joint-Motor.html">Harmonic Drive Planetary Reducer Robot Joint Motor Factory...</a></li>
<li><a href="https://eu.36kr.com/en/p/3864146944414980">Humanoid Robots : Still Learning to Work, but Dexterous Hands Turn...</a></li>

</ul>
</details>

**标签**: `#humanoid robotics`, `#venture capital`, `#supply chain`, `#robot components`, `#Chinese tech`

---