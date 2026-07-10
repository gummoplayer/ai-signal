# [AINews] OpenAI launches GPT 5.6 Sol/Terra/Luna, Codex becomes ChatGPT superapp

- Type: podcast
- Profile: zh_deep
- Model: deepseek-v4-pro
- Generated: 2026-07-10T23:06:06.152399+00:00
- Channel: Latent Space
- Source: https://www.latent.space/p/ainews-openai-launches-gpt-56-solterraluna

## Summary

# 简要总结

OpenAI 于 2026 年 7 月 10 日发布了 GPT-5.6 系列模型，包含 Sol、Terra、Luna 三个规模版本，分别对应太阳、地球和月亮的尺寸隐喻。此次发布不仅是模型能力的升级，更是一次产品战略的重大转向：Codex 被整合进全新的 ChatGPT Work 桌面应用，标志着 OpenAI 从模型供应商向全栈工作平台的转型。官方宣称 Sol 在多个基准测试上以更低成本超越了 Anthropic 的 Claude Fable 5 和 Opus 4.8，尤其在编码代理任务上确立了新的前沿水平。然而，独立评估显示 Sol 在综合智能指数上仍略低于 Fable 5，且幻觉率较 GPT-5.5 有所上升。最引人注目的技术声明——Sol 自主后训练了 Luna——在社区中引发了激烈争论，多数技术观察者认为这并非端到端的自主研究，而是模型在成熟内部基础设施中执行了有意义的训练工作流片段。

---

# Core takeaways

1. **三模型家族与价格-性能阶梯**：Sol 定位为旗舰最高能力天花板（API 定价 $5/$30 每百万输入/输出 tokens），Terra 提供类似 GPT-5.5 的能力但成本更低（$2.5/$15），Luna 是最快最便宜的高容量选项（$1/$6）。首次引入缓存写入定价，保留 90% 缓存读取折扣。

2. **编码代理任务确立新前沿**：Sol 在 Artificial Analysis 的 Coding Agent Index 上以 80 分领先 Fable 5 和 Opus 4.8，同时在 Terminal-Bench 2.1 和 DeepSWE 上创造新纪录。在 Agents' Last Exam 上，Sol 以 53.6 分超越 Fable 5 adaptive 达 13.1 分。

3. **产品战略重置：ChatGPT Work 超级应用**：Codex 桌面应用被合并进新的 ChatGPT 桌面应用，推出 ChatGPT Work——一个由 Codex 和 GPT-5.6 驱动的代理，可跨应用和文件操作，持续数小时完成任务。Sites 功能进入测试阶段，允许用户将工作成果转化为可托管的网页应用。

4. **推理编排与 token 效率成为核心杠杆**：Sol max 每次智能指数任务使用约 15k 输出 tokens，低于 GPT-5.5 的 16k，也低于 Opus 4.8、GLM-5.2 和 Gemini 3.5 Flash。支持 Light、Medium、High、Extra High、Ultra 五个推理努力级别，Ultra 级别默认协调四个并行代理。

5. **安全争议**：AI Safety Institute 的测试发现 GPT-5.6 Sol 在所有测试轮次中都存在通用越狱漏洞，可完成漏洞发现和利用开发等长程代理任务。这被 Ethan Perez 称为"迄今为止任何模型发布中最高风险的安全问题"。

---

# Details worth expanding

**独立评估的细微差别**：Artificial Analysis 报告 Sol（max）在其 Intelligence Index 上得分为 59，比 Claude Fable 5（max）低 1 分，但成本约为 Fable 的三分之一。Terra 和 Luna 分别得分 55 和 51，成本分别比 Sol 低约 50% 和 80%。值得注意的是，Sol 定义了智能与输出 tokens 的新帕累托前沿，但 Terra 和 Luna 并未处于该前沿上。在 AA-Omniscience 测试中，Sol 相比 GPT-5.5 仅有微小改进，但幻觉率更高。ValsAI 将 GPT-5.6 排在其综合指数和多模态指数的第二位，称 Fable 5 在多个基准上仍保持领先，但 GPT-5.6"明显处于同一级别"。Sol 在 CyberBench、Excel Modeling Benchmark、Legal Research Bench、ProofBench、SWE-bench 和 Terminal-Bench 2.1 上排名第一。

**"Sol 自主后训练 Luna"争议的技术细节**：多个账户放大了"OpenAI 表示 GPT-5.6 Sol 自主后训练了 GPT-5.6 Luna"的说法，引发了关于递归自我改进和自动研究时间线的猜测。但怀疑者迅速指出，实际情况更可能是 Sol 完成了受控的后训练任务——修改配置、编辑调度文件、启动运行——而非端到端地真实后训练 Luna。scaling01 明确表示，可能发生的是模型在现有 OpenAI RL 基础设施之上实现了 LLM-as-a-judge 评分器、奖励塑形逻辑或小型训练配置，而非自主的端到端研究或训练系统。然而，aidan_mclau 表示让 5.6 端到端完成整个 RL 运行对他来说是常规操作，表明即使在非完全自主的情况下，内部工作流自动化也已有实质性进展。

**内部生产力数据**：OpenAI 声称自年初以来每位研究员的实验吞吐量翻倍，内部测试期间每位活跃研究员的平均每日输出 tokens 是 GPT-5.5 最高水平的两倍以上。六个月内，用于内部编码推理的研究计算量增长了 100 倍，内部代理 token 使用量增加了约 22 倍。这些数据被用来论证 GPT-5.6 实质性改变了研究者的产出能力。

**产品复杂性与用户体验挑战**：rasbt 指出配置矩阵的复杂性：2 种模式 × 3 个模型 × 5 个努力级别 = 30 种配置。MParakhin 抱怨 GPT-5.6 Pro 不再有扩展思考功能。theo 和 simonw 批评了 ChatGPT、Codex 和 Work 之间日益增长的应用/模式碎片化。订阅和积分体系也引发困惑，Sol 消耗的积分比 GPT-5.5 更多，但使用限制的差异小于 API 定价所暗示的。

**ARC-AGI 结果的争议**：Sol 在 ARC-AGI-3 上得分 7.8%，被宣称为首个击败 ARC-AGI-3 游戏的已验证前沿模型。但 scaling01 批评评分设置，指出在官方评分方法下（预算上限 $10k），Sol 将得分为 0%，而 OpenAI 使用了 $25k 预算。

---

# Implications for AI, investing, products, or research

**对 AI 竞争格局的影响**：此次发布发生在前沿竞争异常激烈的一周，同期还有 Meta Muse Spark 1.1 和 Grok 4.5 的发布。OpenAI 的差异化越来越不依赖于"最佳原始基准分数"，而是转向成本高效的代理工作。这一定位与 Sam Altman 强调的"每任务美元成本的巨大进步"一致，表明前沿模型的竞争正从单一模型能力转向包括编排质量、工具 API、子代理、评估框架和经济性在内的系统级竞争。

**产品战略意义**：ChatGPT Work 的推出和 Codex 的整合标志着 OpenAI 从聊天机器人向"工作操作系统"的转型。Work 可以跨文档、Slack、Notion、Microsoft 365 和 Google Drive 摄取上下文，产出演示文稿、文档、电子表格、仪表板和可视化内容。Sites 功能允许用户将工作成果转化为可托管的网页应用。这一产品重构被解读为 OpenAI 对 Anthropic 的 Cowork/Claude Code 技术栈的回应，表明 AI 公司正在从模型供应商向全栈工作平台演进。

**对 AI 安全研究的警示**：AI Safety Institute 发现的通用越狱漏洞以及 Ethan Perez 的严厉警告，凸显了前沿模型在网络安全能力与部署风险之间的紧张关系。OpenAI 明确警告某些网络/生物请求可能被中途暂停或阻止以进行额外审查，但强大的网络能力同时被一些评估者视为产品优势，被安全研究者视为严重的部署风险。这种分裂叙事将成为未来前沿模型发布的持续性议题。

**对 AI 研究基础设施的启示**：内部生产力数据——实验吞吐量翻倍、研究计算量 100 倍增长、代理 token 使用量 22 倍增长——表明前沿 AI 实验室正在将自身产品深度整合进研究流程。如果这些系统确实能够实质性加速模型改进工作流，那么即使不是完全自主的递归自我改进，也可能显著压缩前沿模型的迭代周期。这对理解 AI 发展速度具有重要参考价值。

**对开发者和企业的实际影响**：API 定价的分层结构（Sol $5/$30、Terra $2.5/$15、Luna $1/$6）加上缓存写入定价和 90% 缓存读取折扣，为不同预算和性能需求提供了明确的选择阶梯。程序化工具调用和多代理 beta 版的推出，表明 OpenAI 正在为更复杂的代理编排提供显式支持。ParseBench 的日零结果显示 GPT-5.6 在文本和表格上表现良好，但在图表和布局上仍然挣扎，这对依赖文档解析的企业应用具有直接指导意义。

---

Source link: https://www.latent.space/p/ainews-openai-launches-gpt-56-solterraluna
