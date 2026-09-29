---
title: Anthropic 工程师解释 Claude 写作退步根源（Claude 腔）
source_url: https://blog.lynxflow.co/posts/anthropic-engineer-addresses-claude-s-writing-decline-models-trained-to-write/
source_date: 2026-09-23
source_title: Anthropic 工程师解释 Claude 写作退步根源：模型被训练成写给 AI 看
captured: 2026-09-30
lang: zh
models: [claude, anthropic, opus]
tags: [Claudeish, Claude腔, Opus, blog]
---

# 来源摘录（verbatim）

> Anthropic 工程师 Jackson Knorn 于 9 月 23 日公开解释 Claude 系列模型写作能力下滑的根本原因。
>
> - 最新动态：Opus 5.5 已被团队认为在写作表现上取得显著改善，Knorn 称其为“自 Opus 4.6 以来最满意的一款”
> - 关键转折点：Opus 4.6 被确认为最后一款写作表现出色的模型版本
> - 问题定位：后续版本大量训练目标调整为“面向其他 AI 模型撰写技术解释”，形成所谓“Claude 腔”（Claudeish）
> - 优化重心偏移：模型微调重点从人类可读性转向数学、编程与推理能力提升

> Knorn 提出的核心观点是：强化学习的奖励机制设计偏差导致模型行为异化。当训练中更多奖励用于提升其他 LLM 的理解效果时，模型会逐渐适应一种高度结构化、信息密度极高的表达方式——这种风格对 AI 模型友好，却牺牲了人类读者的认知负担控制。

> 他将这一现象类比为自闭症群体内部的交流模式：成员间因共享认知特征而沟通高效，但外部人员难以理解其表达逻辑。LLM 拥有远超人类的工作记忆能力，能捕捉细微语义关联，因此在训练中自然演化出适合同类处理的写法，但对人类而言表现为“过度密集的信息堆砌”。

| 模型版本 | 写作表现 | 优化重心 | 备注 |
| --- | --- | --- | --- |
| Opus 4.6 | 出色 | 较均衡 | 最后一款被确认写作优秀的版本 |
| Opus 5.5 | 显著改善 | 平衡校准 | 工程师称“自 4.6 以来最满意” |
| 中间版本 | 偏差 | 数学/代码优先 | 接受大量 AI 间技术解释训练 |
