# [AINews] SpaceXAI launches Grok 4.5, first Opus-class model post Cursor acquisition

- Type: podcast
- Profile: zh_standard
- Model: deepseek-v4-pro
- Generated: 2026-07-09T23:10:11.881695+00:00
- Channel: Latent Space
- Source: https://www.latent.space/p/ainews-spacexai-launches-grok-45

## Summary

SpaceXAI 发布了 Grok 4.5，这是其首个明确针对编程和智能体（agents）工作流的前沿模型。该模型由 xAI 与 Cursor 合作训练，定位并非绝对基准测试的冠军，而是以“能力/成本比”为核心卖点，提供接近 Opus 级别的性能，但速度更快、成本更低。发布时机恰好在 OpenAI 的 GPT-5.6 确认发布的前一天，使其成为 GPT-5.5 等效模型发布窗口期的最后一位重要参与者。

**核心要点**
- **定位与合作伙伴**：Grok 4.5 被描述为“Opus 级”模型，但更侧重经济性和速度。它是与 Cursor 合作训练的，Cursor 称其为“我们迄今为止最强大的模型”，并且是“首个为超越软件工程领域而构建的模型”。
- **定价与效率**：官方定价为每百万输入 tokens 2 美元，输出 tokens 6 美元，远低于同期竞品（如 GPT-5.6 的 5/30 美元，Opus 4.8 的 5/25 美元）。缓存命中可享 75% 折扣，但超过 20 万 tokens 的长输入成本翻倍。
- **模型规模**：据第三方报道，Grok 4.5 的参数量达到 1.5 万亿，是 Grok 4.3 的 3 倍，标志着 xAI 首次进入真正的旗舰编程智能体赛道。
- **基准测试表现**：在 Artificial Analysis 的智能指数中排名第四，得分 54，仅次于 Fable 5、GPT-5.5 和 Opus 4.8。在 τ³-Banking 任务上取得 33% 的最高分。其编程智能体指数得分 76，与 GPT-5.5 持平。关键优势在于效率：完成智能指数任务的平均输出 tokens 比 Opus 4.8 低 60% 以上，编程智能体任务的总 tokens 消耗（190 万）远低于 Fable 5（720 万）和 GPT-5.5（620 万）。

**值得展开的细节**
- **上下文窗口**：初始上下文窗口为 50 万 tokens（低于 Grok 4.3 的 100 万），但 Elon Musk 表示可能在下周恢复至 100 万。
- **生态支持**：发布当日即获得 Hermes Agent、OpenRouter 等平台的支持，并在 Grok Build、API 和 Cursor 产品中可用。Cursor 还宣布首周提供双倍使用额度。
- **产品线区分**：Cursor 明确表示 Grok 4.5 与 Composer 系列属于不同“重量级”，Composer 2.5 将继续保留，未来还会有该较小级别的模型。
- **基准测试饱和**：OpenAI 的评估团队指出，即使是强大的 SWE-Bench Pro 也已饱和或存在根本性缺陷，业界正在寻找如 FrontierCode 等后继基准。

**对 AI、投资、产品及研究的启示**
- **市场结构变化**：xAI 以“足够好且更便宜”的策略强势切入编程智能体市场，直接挑战 Anthropic 和 OpenAI 在该领域的主导地位。这可能会加速模型商品化，迫使其他前沿实验室在定价上做出回应。
- **投资关注点转移**：基准测试的绝对领先优势正在减弱，投资评估应更关注模型的效率指标（如每美元智能指数得分、任务 tokens 消耗）和垂直场景的深度优化能力。
- **产品构建策略**：对于构建 AI 产品的团队，Grok 4.5 提供了一个高性价比的新选择，尤其是在需要大量 tokens 消耗的复杂智能体工作流中，其成本优势可能极为显著。产品设计上需考虑模型切换的灵活性。
- **研究方向**：模型评估正面临基准测试饱和的挑战，需要开发更能反映真实世界复杂编程和智能体任务的新基准。同时，如何在不显著增加参数量的前提下提升效率，是重要的研究方向。

**来源链接**：[AINews: SpaceXAI launches Grok 4.5, first Opus-class model post Cursor acquisition](https://www.latent.space/p/ainews-spacexai-launches-grok-45)
