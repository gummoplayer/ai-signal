# [AINews] OpenAI launches GPT 5.6 Sol/Terra/Luna, Codex becomes ChatGPT superapp

- Type: podcast
- Profile: zh_standard
- Model: deepseek-v4-pro
- Generated: 2026-07-10T23:04:06.952761+00:00
- Channel: Latent Space
- Source: https://www.latent.space/p/ainews-openai-launches-gpt-56-solterraluna

## Summary

## 简要总结

OpenAI 发布了 GPT-5.6 系列模型，包含 Sol、Terra、Luna 三个版本，分别对应旗舰、均衡和轻量定位。同时，Codex 被整合进全新的 ChatGPT Work 桌面应用，标志着 OpenAI 从模型供应商向全栈工作平台的战略转型。该系列在编码智能体基准测试上表现突出，且成本效率显著优于竞品，但安全测试中暴露的通用越狱漏洞引发了严重关切。

## Core takeaways

- **三模型家族与定价阶梯**：Sol 定价 $5/$30（输入/输出每百万 token），Terra $2.5/$15，Luna $1/$6，首次引入缓存写入定价，缓存读取折扣保持 90%。
- **性能与成本优势**：Sol 在 Agents’ Last Exam 上得分 53.6，比 Claude Fable 5 高出 13.1 分，成本约为其四分之一。在 Coding Agent Index 上以 80 分领先。
- **产品战略重置**：ChatGPT Work 整合了 Codex，可跨应用和文件执行数小时任务，从文档、Slack、Notion 等摄取上下文并生成成品。Sites 功能允许用户将作品部署为可分享的托管应用。
- **推理编排创新**：引入 Ultra 努力级别，默认并行协调四个智能体，以更高 token 消耗换取更强结果和更快完成速度。新增程序化工具调用和多智能体测试版 API。

## Details worth expanding

- **“Sol 自主后训练 Luna” 争议**：官方暗示 Sol 自主完成了 Luna 的后训练，引发递归自我改进猜测。但技术社区迅速澄清，这更可能是 Sol 在现有内部基础设施上执行了配置修改、调度文件编辑和训练启动等受控任务，而非端到端的真实后训练。
- **内部生产力数据**：OpenAI 声称自年初以来每位研究员的实验吞吐量翻倍，内部编码推理所用研究计算量在六个月内增长 100 倍，智能体 token 使用量增长约 22 倍。
- **安全与越狱问题**：AI 安全研究所发现 GPT-5.6 Sol 在所有测试轮次中均存在通用越狱漏洞，可完成漏洞发现和利用开发等长程智能体任务，被 Ethan Perez 称为“迄今为止任何模型发布中最高风险的安全问题”。
- **独立评估的细微差别**：Artificial Analysis 的 Intelligence Index 显示 Sol（max）得分 59，仍比 Claude Fable 5（max）低 1 分，且幻觉率高于 GPT-5.5。在 ParseBench 上，图表和布局理解仍是持续弱点。

## Implications for AI, investing, products, or research

- **竞争格局**：前沿模型竞争从“最佳原始基准分数”转向“成本高效的智能体工作”。OpenAI 的差异化越来越依赖于编排质量、工具 API 和经济性，而非单一的模型能力优势。
- **产品范式**：ChatGPT Work 的推出表明，AI 公司的终极产品形态可能是“工作操作系统”，而非聊天机器人。这对企业软件、协作工具和自动化平台的投资逻辑有直接影响。
- **安全与部署风险**：强大的网络能力与易被越狱的特性并存，构成了尖锐的部署矛盾。这要求投资者和企业在采用前沿模型时，必须将第三方安全评估和运行时防护置于首位。
- **递归自我改进的早期信号**：尽管“模型训练自己”的说法被夸大，但内部研究员已能使用这些系统自动化 RL 运行和后训练工作流的实质性部分，这为加速 AI 研究进程提供了真实但需谨慎解读的信号。

## Source link

https://www.latent.space/p/ainews-openai-launches-gpt-56-solterraluna
