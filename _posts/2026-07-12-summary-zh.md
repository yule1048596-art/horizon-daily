---
layout: default
title: "Horizon Summary: 2026-07-12 (ZH)"
date: 2026-07-12
lang: zh
---

> 从 63 条内容中筛选出 12 条重要资讯。

---

1. [研究揭示 Claude Code 的 Token 使用量是 OpenCode 的四倍以上。](#item-1) ⭐️ 8.0/10
2. [陶哲轩使用现代编码智能体构建应用程序](#item-2) ⭐️ 8.0/10
3. [Ghostel：一款基于 libghostty 的全新 Emacs 终端模拟器。](#item-3) ⭐️ 8.0/10
4. [Zer0Fit 将谷歌的 TabFM 和 TimesFM 打包成本地 MCP 服务器，用于零样本机器学习任务。](#item-4) ⭐️ 8.0/10
5. [Chromium 的 Math.tanh()函数成为可暴露用户操作系统的指纹识别向量](#item-5) ⭐️ 7.0/10
6. [对 AI 数据中心扩张的地方性抵抗标志着一场新的社会冲突。](#item-6) ⭐️ 7.0/10
7. [中国 97 家具身数据公司一年融资 44.7 亿元](#item-7) ⭐️ 7.0/10
8. [英国公布 20 亿英镑人工智能作战实验室建设计划](#item-8) ⭐️ 7.0/10
9. [苹果失败的造车项目意外推动了其强大的 AI 芯片发展](#item-9) ⭐️ 6.0/10
10. [Anthropic 澄清 Claude Code 中模型选择与努力程度的混淆](#item-10) ⭐️ 6.0/10
11. [人工智能热潮导致燃气轮机价格三年内上涨三倍](#item-11) ⭐️ 6.0/10
12. [长鑫科技 IPO 将成为今年 A 股最大上市项目](#item-12) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [研究揭示 Claude Code 的 Token 使用量是 OpenCode 的四倍以上。](https://systima.ai/blog/claude-code-vs-opencode-token-overhead) ⭐️ 8.0/10

一项实证研究发现，Anthropic 的 Claude Code 在读取用户输入之前发送了大约 33,000 个 Token 的初始系统提示，而 OpenCode 仅使用约 7,000 个 Token，其开销相差超过四倍。 这种差异凸显了开发者在使用 AI 编码工具时面临的重大成本和效率问题，因为过高的 Token 使用量会直接转化为更高的 API 成本，并可能影响整个行业的工具采用和货币化策略。 这种低效归因于 Claude Code 的缓存策略和“脚手架”开销，社区轶事表明其激进的子代理使用会进一步消耗 Token 预算；然而，一些人认为，不比较任务质量或成功率，仅凭原始 Token 数量作为指标是不够的。

hackernews · systima · 7月12日 18:25 · [社区讨论](https://news.ycombinator.com/item?id=48883275)

**背景**: 像 Claude Code 和 OpenCode 这样的 AI 编码助手，是作为通过 API 与大语言模型（LLM）交互的代理运行的。“脚手架”指的是工具自身的代码，它负责构建提示、管理上下文和编排工具，这些操作本身会在处理用户实际查询之前消耗 Token。对于采用按使用量付费 API 模型的开发者工具来说，Token 消耗是一个关键的成本因素。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/opencode-ai/opencode">GitHub - opencode-ai/opencode: A powerful AI coding agent. Built for the terminal. · GitHub</a></li>
<li><a href="https://docs.anthropic.com/en/docs/claude-code/overview">Claude Code overview - Anthropic</a></li>
<li><a href="https://github.com/ai-boost/awesome-harness-engineering">GitHub - ai-boost/awesome-harness-engineering: Awesome list for AI agent harness engineering: tools, patterns, evals, memory, MCP, permissions, observability, and orchestration. · GitHub</a></li>

</ul>
</details>

**社区讨论**: 社区讨论存在分歧：一些用户反映 Claude Code 的子代理极其耗费 Token，而另一些人则怀疑高 Token 用量是 Anthropic 故意为之的货币化策略。多位评论者指出，仅凭 Token 数量是一个有缺陷的比较指标，并呼吁应整体评估任务完成质量、成本和开发者体验。

**标签**: `#AI-coding-tools`, `#token-efficiency`, `#developer-tools`, `#cost-optimization`, `#benchmarking`

---

<a id="item-2"></a>
## [陶哲轩使用现代编码智能体构建应用程序](https://terrytao.wordpress.com/2026/07/11/old-and-new-apps-via-modern-coding-agents/) ⭐️ 8.0/10

菲尔兹奖得主陶哲轩公开分享了他使用像 Claude 这样的大型语言模型编码智能体，快速构建交互式应用程序和用于其工作的教育可视化的积极经验。 来自世界著名数学家的认可表明，人工智能编码工具已经强大到足以让高级的非软件专业用户创建有价值的技术内容，这预示着软件创建的重大民主化。 陶哲轩强调，对于像可视化这样辅助性的、非关键任务的交互内容，使用大语言模型生成的代码的下行风险是可接受的，他将这些工具定位为有用的辅助手段，而非核心智力工作的替代品。

hackernews · subset · 7月12日 11:09 · [社区讨论](https://news.ycombinator.com/item?id=48880170)

**背景**: 现代人工智能编码智能体，如 Cursor 和 Claude Code，是利用大型语言模型通过交互式提示协助开发者生成、重构和调试代码的软件工具。它们代表了从简单的代码补全到更自主的执行循环的转变，使没有深厚软件工程专业知识的用户也能构建功能性的应用程序。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@dave-patten/the-state-of-ai-coding-agents-2026-from-pair-programming-to-autonomous-ai-teams-b11f2b39232a">The State of AI Coding Agents (2026): From Pair Programming to Autonomous AI Teams | by Dave Patten | Medium</a></li>
<li><a href="https://www.augmentcode.com/tools/8-top-ai-coding-assistants-and-their-best-use-cases">8 Best AI Coding Assistants [Updated May 2026] | Augment Code</a></li>

</ul>
</details>

**社区讨论**: 讨论显示出极大的热情，用户们分享了大语言模型如何彻底改变了教育材料和可视化的创建。也有幽默的评论将陶哲轩使用这些工具比作米其林星级厨师使用微波炉，同时也有平衡的观点指出，这些工具最适合用于非关键的辅助任务，而非核心工作。

**标签**: `#AI coding agents`, `#LLM applications`, `#software development`, `#education technology`, `#Terence Tao`

---

<a id="item-3"></a>
## [Ghostel：一款基于 libghostty 的全新 Emacs 终端模拟器。](https://dakra.github.io/ghostel/) ⭐️ 8.0/10

Ghostel 是一款使用 libghostty 库的新型 Emacs 终端模拟器软件包，旨在提供比 vterm 等现有选项更出色的性能和功能。 它为 Emacs 用户提供了可能更快、更可靠的终端模拟体验，这对于依赖编辑器内终端工作流的开发者至关重要。 该项目在 GitHub 上维护，并包含了与 vterm 及另一个名为“eat”的模拟器的功能对比。用户报告称其在 TUI 应用程序上性能明显更快，但也注意到一些早期问题，例如偶尔的清屏显示错误和卡死现象。

hackernews · signa11 · 7月12日 08:52 · [社区讨论](https://news.ycombinator.com/item?id=48879504)

**背景**: Ghostty 是一款现代终端模拟器，而 libghostty 是其可嵌入库，旨在让其他应用程序集成一个功能完整的终端。在 Emacs 中，像 vterm 这样的终端模拟器允许用户在不离开编辑器的情况下运行 Shell 命令，但它们可能存在性能或兼容性限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mitchellh.com/writing/libghostty-is-coming">Libghostty Is Coming – Mitchell Hashimoto</a></li>
<li><a href="https://github.com/emacsmirror/vterm">GitHub - emacsmirror/ vterm : Fully-featured terminal emulator · GitHub</a></li>

</ul>
</details>

**社区讨论**: 项目维护者提供了背景信息和对比链接，而早期采用者则充满热情，一位用户称其“非常棒”并可能成为日常主力工具。然而，用户也提出了关于输入模式处理的实际问题，并指出了一些粗糙之处，例如偶尔的卡死。

**标签**: `#emacs`, `#terminal-emulator`, `#tools`, `#open-source`, `#performance`

---

<a id="item-4"></a>
## [Zer0Fit 将谷歌的 TabFM 和 TimesFM 打包成本地 MCP 服务器，用于零样本机器学习任务。](https://www.reddit.com/r/MachineLearning/comments/1uue8cc/zer0fit_i_took_googles_new_tabfm_timesfm_ml/) ⭐️ 8.0/10

一位开发者创建了 Zer0Fit，这是一个基于 Docker 的 MCP 服务器，它封装了谷歌新发布的 TabFM 和 TimesFM 基础模型，使得从 Open WebUI 等聊天界面进行零样本的预测、分类和回归任务成为可能。 这个项目简化了将强大的零样本机器学习基础模型集成到开发者工作流程中的过程，有望在无需深厚模型训练或超参数调优专业知识的情况下，使高性能机器学习的使用变得更加普及。 该服务器需要至少 16GB 显存的 NVIDIA GPU，并且仅支持 CUDA，它具有动态模型加载功能以及 5 分钟的 TTL 以管理内存；在零样本测试中表现出色，在 Iris 数据集上达到了 94.7% 的准确率，回归测试的 R2 为 0.91。

reddit · r/MachineLearning · /u/Porespellar · 7月12日 12:32

**背景**: TabFM 是谷歌研究院最近发布的一个基础模型，专为表格数据的零样本分类和回归设计，其功能类似于大型语言模型但针对表格数据。TimesFM 则是一个时间序列预测基础模型，在超过 1000 亿个真实世界时间点的庞大数据集上进行了预训练。MCP（模型上下文协议）是一个开放标准，允许像 LLM 这样的 AI 应用程序连接到外部工具、数据源和工作流程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://research.google/blog/introducing-tabfm-a-zero-shot-foundation-model-for-tabular-data/">Introducing TabFM : A zero-shot foundation model for tabular data</a></li>
<li><a href="https://research.google/blog/a-decoder-only-foundation-model-for-time-series-forecasting/">A decoder-only foundation model for time-series forecasting</a></li>
<li><a href="https://modelcontextprotocol.io/">What is the Model Context Protocol ( MCP )? - Model Context Protocol</a></li>

</ul>
</details>

**标签**: `#foundation-models`, `#machine-learning`, `#MCP-server`, `#zero-shot-learning`, `#Docker`

---

<a id="item-5"></a>
## [Chromium 的 Math.tanh()函数成为可暴露用户操作系统的指纹识别向量](https://scrapfly.dev/posts/browser-math-os-fingerprint/) ⭐️ 7.0/10

自 Chromium 148 版本起，V8 JavaScript 引擎开始使用宿主操作系统的本地数学库（libm）来计算 Math.tanh()函数，而不是之前内置的例程，这导致其输出因操作系统不同而产生差异，从而形成一个独特的指纹。 这产生了一种新的、微妙的浏览器指纹识别技术，可帮助反机器人系统识别用户或发现不一致之处，例如声称使用不同操作系统的伪装 User-Agent 头与实际运行的系统之间的矛盾。 Math.tanh 目前是 Chromium 中唯一一个通过计算结果泄漏操作系统信息的 Math.*函数，而这种不对称性本身就可以作为一个可检查的信号。该行为已在较新的 glibc 版本上得到确认，这些版本使用了 CORE-MATH 项目中正确舍入的 tanh 实现，使得指纹信息更加针对特定的操作系统版本。

hackernews · joahnn_s · 7月12日 21:12 · [社区讨论](https://news.ycombinator.com/item?id=48884853)

**背景**: 浏览器指纹识别是一种基于用户浏览器和设备特征的独特组合（如屏幕分辨率、已安装字体和画布渲染）来跟踪或识别用户的技术。IEEE 754 标准定义了浮点运算的执行方式，但不同的操作系统和数学库（如 libm）在实现 tanh()等超越函数时可能存在细微差异，从而导致计算结果有微小不同。Chromium 的 V8 引擎是驱动 Google Chrome 和许多其他浏览器的 JavaScript 运行时。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://scrapfly.dev/posts/browser-math-os-fingerprint/">Your Browser Does Math Differently on Every OS, and Anti-Bot...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Floating-point_arithmetic">Floating-point arithmetic - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区讨论中包含了对文章来源的质疑，一位评论者暗示这是由 AI 生成的，目的是推广该安全公司的服务。其他人则强调，这个问题凸显了推动实现正确舍入超越函数的必要性，并指出现代 glibc 已经为 tanh 实现了这一点。也有少数评论者指出，大多数指纹识别解决方案关注的是唯一性信号而非操作系统检测，因此这项技术的实际影响值得商榷。

**标签**: `#browser-fingerprinting`, `#security`, `#javascript`, `#floating-point`, `#chromium`

---

<a id="item-6"></a>
## [对 AI 数据中心扩张的地方性抵抗标志着一场新的社会冲突。](https://www.theverge.com/column/963346/ai-data-centers-fight) ⭐️ 7.0/10

The Verge 的一篇通讯文章将日益增长的地方性和环保性反对 AI 数据中心快速建设的现象，描述为一场重大社会斗争的开端。 这场新兴的冲突凸显了 AI 产业庞大的基础设施需求给当地带来的切实影响，例如对电网和社区资源的压力，预示着未来可能发生的政策与监管斗争。 文章指出，这种抵抗早在当前 AI 热潮威胁到当地电网之前数年就已开始，表明对数据中心占地和资源消耗的担忧并非新事，但目前正在加剧。

rss · The Verge - AI · 7月12日 12:00

**背景**: AI 数据中心需要消耗巨量电力用于计算和冷却，通常从当地电网取电并消耗大量水资源。全球建设 AI 能力的竞赛导致了大规模建设此类设施的热潮，选址往往着眼于廉价的土地和电力，有时在初期缺乏充分的社区协商。

**标签**: `#AI infrastructure`, `#data centers`, `#environmental impact`, `#local policy`, `#tech backlash`

---

<a id="item-7"></a>
## [中国 97 家具身数据公司一年融资 44.7 亿元](https://36kr.com/p/3892027841362694?f=rss) ⭐️ 7.0/10

一项行业调查识别出中国 97 家具身数据公司，其中 15 家纯数据服务商在过去一年（2025 年 7 月至 2026 年 7 月）融资约 44.7 亿元。 该分析表明，具身数据已发展成为一条独立的产业赛道，对机器人和具身 AI 模型的训练至关重要，但其融资规模相较于“大脑派”模型公司仍属适度。 数据采集方法主要分为四大类：真机遥操、无本体采集、仿真合成和互联网视频蒸馏，其中大多数公司采取多路线策略以满足多样化的训练需求。

rss · 36kr - AI · 7月12日 02:16

**背景**: 具身智能是指通过物理身体进行感知和行动的智能系统，其训练需要大量的真实世界交互数据。“数据金字塔”概念说明不同阶段需要不同类型的数据（真实数据、模拟数据、网络数据），而“仿真到现实的鸿沟”——即模拟数据无法完美复制真实世界物理特性——仍然是推动对多样化数据源需求的关键挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tech.ifeng.com/c/8uh5s4oHQ2h">tech.ifeng.com/c/8uh5s4oHQ2h</a></li>

</ul>
</details>

**标签**: `#embodied AI`, `#data collection`, `#robotics`, `#industry analysis`, `#funding trends`

---

<a id="item-8"></a>
## [英国公布 20 亿英镑人工智能作战实验室建设计划](https://36kr.com/newsflashes/3892413575559941?f=rss) ⭐️ 7.0/10

英国国防部宣布投入 20 亿英镑建立人工智能作战实验室，旨在利用智能技术全面升级军事训练体系并重塑演习模式。 这项巨额政府投资凸显了人工智能在现代战争中的战略重要性，旨在加强英国本土国防工业并创造技术岗位。 该项目将由多家本土防务企业组成的联合体执行，联动众多本地供应商，并包含青年技术学徒项目以及为退役军人开辟的技术就业途径。

rss · 36kr - AI · 7月12日 09:32

**背景**: 全球范围内，各国军队正越来越多地将人工智能整合到训练中，以提高训练真实性、加速决策并分析大量作战数据以获得战略优势。由人工智能驱动的模拟可以实时调整场景，并提供可扩展的个性化训练，代表着国防现代化的重大转变。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://breakingdefense.com/2025/10/ai-in-the-loop-transforming-military-training-and-system-design-through-smarter-simulation/">AI in the loop: Transforming military training and system design through smarter simulation - Breaking Defense</a></li>
<li><a href="https://www.fmj.co.uk/vivo-defence-launches-data-and-ai-apprenticeships-with-multiverse/">VIVO Defence launches data and AI apprenticeships with Multiverse</a></li>

</ul>
</details>

**标签**: `#AI`, `#Defense`, `#Government Investment`, `#Military AI`, `#UK`

---

<a id="item-9"></a>
## [苹果失败的造车项目意外推动了其强大的 AI 芯片发展](https://www.theverge.com/tech/964519/apple-silicon-self-driving-car-ai-m7-ultra) ⭐️ 6.0/10

尽管苹果的自动驾驶汽车项目“泰坦计划”最终被放弃，但该项目的需求直接推动了公司强大端侧 AI 处理器的研发。 这揭示了失败的雄心勃勃的研发项目如何能产生重大的、成功的衍生技术，从而增强公司的核心产品及其在广阔市场中的竞争力。 该自动驾驶平台需要强大的端侧 AI 处理能力以实现实时决策，这一需求推动了相关技术创新，这些创新后来惠泽了 M 系列等 Apple Silicon 芯片，但具体的车载处理器从未完成。

rss · The Verge - AI · 7月12日 16:27

**背景**: 苹果秘密的自动驾驶汽车项目内部代号为“泰坦计划”，始于 2014 年左右，经过十年的工作和多次领导层变动后于 2024 年正式取消。端侧 AI 处理对于自动驾驶车辆至关重要，使其能够分析传感器数据并做出实时驾驶决策，而无需依赖云连接。苹果的神经网络引擎是集成在 Apple Silicon 芯片中的专用神经网络处理单元，用于加速机器学习任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Apple_car_project">Apple car project - Wikipedia</a></li>
<li><a href="https://apple.fandom.com/wiki/Neural_Engine">Neural Engine | Apple Wiki | Fandom</a></li>
<li><a href="https://objectways.com/blog/boosting-the-situational-awareness-of-self-driving-cars-using-ai/">AI for Smarter Situational Awareness in Self-Driving Cars</a></li>

</ul>
</details>

**标签**: `#apple-silicon`, `#ai-chips`, `#self-driving-cars`, `#technology-history`, `#corporate-rd`

---

<a id="item-10"></a>
## [Anthropic 澄清 Claude Code 中模型选择与努力程度的混淆](https://36kr.com/p/3892222176574211?f=rss) ⭐️ 6.0/10

Anthropic 官方发布指南，解释许多 Claude Code 用户错误地将“模型”选择与“努力程度”混为一谈，导致在调整努力设置可能更有效的情况下，不必要地升级到 Fable 等更大的模型。 这一澄清有助于用户通过了解如何为特定任务正确配置 Claude Code 来优化成本和性能，可能提高整个开发者生态系统的效率。 “模型”设置更改底层 AI 的冻结权重和能力，而“努力程度”控制 Claude 承担的工作量，例如读取文件或运行测试；高努力的小模型可以胜过低努力的大模型。

rss · 36kr - AI · 7月12日 05:47

**背景**: Claude Code 是 Anthropic 的 AI 编码助手，允许开发者通过命令行界面与 Claude 模型交互，它包含模型选择（例如 Fable）和努力程度（从低到 xhigh）的设置。2026 年 3 月，Anthropic 为了降低延迟，暂时将默认努力程度从高改为中，导致用户抱怨性能下降，随后在 4 月恢复。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.bswen.com/blog/2026-03-13-claude-code-effort-settings/">How to Set Claude Code Effort Level : CLI Flags... | BSWEN</a></li>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://www.sitepoint.com/claude-code-21-the-complete-xhigh-and-autoverification-guide-2026/">Claude Code 2.1: The Complete xHigh and Auto-Verification Guide...</a></li>

</ul>
</details>

**社区讨论**: 文章提到了 GitHub 上的抱怨以及 AMD AI 负责人 Stella Laurenzo 等人的批评，她测量到 Claude 的思考努力程度下降了 67%，表明用户对悄然更改感到极度沮丧。这凸显了社区对 AI 工具更新透明度的更广泛关注。

**标签**: `#AI_models`, `#optimization`, `#user_experience`, `#Anthropic`, `#Claude_Code`

---

<a id="item-11"></a>
## [人工智能热潮导致燃气轮机价格三年内上涨三倍](https://36kr.com/newsflashes/3892556678543880?f=rss) ⭐️ 6.0/10

受人工智能数据中心需求激增的推动，燃气轮机的价格在过去三年内累计上涨了约 300%，微软等大型科技公司正在向 GE Vernova 等供应商采购大量设备。 这一价格飙升凸显了人工智能热潮如何在能源基础设施供应链中造成严重瓶颈，极大地影响了建设用于人工智能训练和推理的大型数据中心的成本和可行性。 微软最近向 GE Vernova 采购了 7 台大型燃气轮机为其得州数据中心供电，每台售价超过 2.5 亿美元，这表明尽管价格高昂，市场需求仍然远超供应。

rss · 36kr - AI · 7月12日 11:37

**背景**: 燃气轮机是为大型数据中心提供可靠、按需电力的关键设备，尤其是在美国等电网容量可能跟不上需求的地区。人工智能热潮加速了这些高耗电设施的建设，给 GE Vernova、西门子和卡特彼勒等涡轮机制造商的供应链带来了压力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wap.stockstar.com/detail/IG2026020900020061">北美“ 电 荒”， 燃 气 轮 机 成AI基建，联德股份迎市场红利-证券之星</a></li>
<li><a href="https://news.fx168news.com/cooperate/2507/7346700.shtml">GE Vernova ：AI热潮下 的 能 源 新王-FX168财经网</a></li>

</ul>
</details>

**标签**: `#AI`, `#energy`, `#infrastructure`, `#supply-chain`, `#data-centers`

---

<a id="item-12"></a>
## [长鑫科技 IPO 将成为今年 A 股最大上市项目](https://36kr.com/newsflashes/3892554879515140?f=rss) ⭐️ 6.0/10

长鑫科技计划于 7 月 16 日启动科创板 IPO 网上申购，拟募资 295 亿元，这将是今年 A 股规模最大的首次公开募股。 此次 IPO 为中国本土半导体产业，特别是 DRAM 存储芯片生产领域，带来了重大的资本注入，这对于减少对外依赖、推进国家在人工智能和计算领域的发展至关重要。 本次 IPO 的网上发行申购上限为 167.2 万股，顶格申购需配沪市市值 1672 万元，由于发行股票数量庞大，预计中签率相对较高。

rss · 36kr - AI · 7月12日 11:18

**背景**: 长鑫科技是中国推动半导体自给自足战略中的关键企业，专注于用于电脑和智能手机等设备的 DRAM 存储芯片。科创板是上海证券交易所推出的类似纳斯达克的科技板块，采用注册制上市机制，旨在为创新型企业提供融资便利。存储芯片是一种战略性商品，其供应安全日益被视为人工智能和其他先进技术发展的关键。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tuoluo.cn/article/detail-10128903.html">从百亿巨亏到千亿净利，爆红的 长 鑫 科 技 是如何炼成的？_ 陀螺 科 技</a></li>
<li><a href="https://en.wikipedia.org/wiki/Shanghai_Stock_Exchange_STAR_Market">Shanghai Stock Exchange STAR Market - Wikipedia</a></li>
<li><a href="https://laoyaoba.com/n/984247">算力争霸战打响！ 2026全球博弈， 存 储 芯 片 成必争战略高地</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#IPO`, `#A-share market`, `#memory chips`, `#China tech`

---