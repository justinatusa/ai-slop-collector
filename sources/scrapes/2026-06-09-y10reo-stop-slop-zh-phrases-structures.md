---
title: y10reo/stop-slop-zh — phrases.md + structures.md（全文）
source_url: https://github.com/y10reo/stop-slop-zh/blob/main/references/phrases.md
source_date: 2026-06-09
source_title: phrases.md / structures.md
captured: 2026-09-30
lang: zh
models: [zh-slop, unattributed]
tags: [github, phrases, structures, 中文]
---

# 来源摘录（verbatim）

## phrases.md

```markdown
# Phrases

Use this file for deeper phrase cleanup after the main rules. Do not replace mechanically. Delete a phrase only when it adds no factual, tonal, or genre value.

## Empty Intensifiers

Cut when the sentence keeps the same meaning:

- 非常、十分、极其、特别、格外、相当、尤其、真的、确实、的确、实在、极大地、充分地
- 很大程度上、在一定程度上、某种程度上、从某种意义上说
- 一种、某种、一定的、相应的、相关的、所谓的

Prefer a concrete measure:

| Avoid | Prefer |
|---|---|
| 显著提升 | 从 4.2 秒降到 0.8 秒 |
| 大幅减少 | 从 30 条降到 2 条 |
| 非常重要 | 影响审批能不能通过 |
| 很有帮助 | 每周少做 3 小时重复工作 |

## Nominalized Verb Shells

Replace with direct verbs or actions:

| Avoid | Prefer |
|---|---|
| 进行优化 | 优化 / 改了哪一处 |
| 实现增长 | 增长 / 涨了多少 |
| 做出选择 | 选择 / 选 |
| 采取措施 | 具体做法 |
| 提供保障 | 保障 / 谁负责什么 |
| 给予支持 | 支持 |
| 起到作用 | 起作用 / 做了什么 |
| 加以改进 | 改进 |
| 推动落地 | 谁把什么做完 |
| 赋能业务 | 帮哪个岗位省了什么 |

## Meta-Commentary

Delete unless the user asked for a teaching outline:

- 接下来我将、本文将、本文旨在、下面我们来看、让我们来探讨
- 以下是几点、主要包括以下几个方面、我们可以从以下维度来看
- 值得注意的是、值得一提的是、不得不说、毫无疑问、不容忽视
- 总的来说、综上所述、由此可见、概括而言、归根结底

## Vague Attribution

Name the source, method, or person. If none exists, remove the claim.

- 专家认为、业内人士指出、观察者表示、行业报告显示、数据显示、研究表明
- 多个来源显示、外界普遍认为、有观点认为、有人指出、相关机构称

Better:

| Weak | Strong |
|---|---|
| 专家认为这会影响行业 | 清华大学某团队在 2025 年报告中估计，客服外包岗位需求下降了 12% |
| 数据显示用户更满意 | 4 月 NPS 从 31 升到 45，主要增长来自企业版用户 |
| 业内人士表示前景广阔 | 删掉，除非能说清谁、在哪、基于什么判断 |

## Promotional Language

Cut or prove with evidence:

- 开创性、颠覆性、革命性、里程碑式、划时代
- 无缝、极致、强大、卓越、领先、先进、全新升级
- 充满活力、丰富多彩、令人叹为观止、迷人、必游之地
- 深刻、深远、重大、核心、关键、重要、宝贵
- 不断演变的格局、广阔前景、巨大潜力、无限可能

## Overclaim Verbs

Check the evidence before keeping these:

- 验证、证实、表明、证明、彰显、凸显、体现、标志着
- 必将、大概率、唯一、最佳、绝对、彻底、完美
- 成功验证、充分证明、强烈需求、真实需求、市场认可

Prefer narrower wording:

| Avoid | Prefer |
|---|---|
| 成功验证市场需求 | 说明早期用户愿意付费 |
| 充分证明产品有效 | 项目方/测试数据显示某项指标变化 |
| 必将迎来增长 | 可能受益于某个明确因素 |
| 风险被彻底封锁 | 付款前提和回购责任被写入协议 |

## Slogan Endings

Usually delete:

- 这，就是...的力量
- 唯有...，方能...
- 在这个...的时代，我们更需要...
- 让我们一起，向着...前进
- 未来可期，行则将至
- 这不仅是一种选择，更是一种态度
- 为...注入新的活力

## Chatbot Residue

Delete from final prose:

- 当然可以、好的、没问题
- 希望这对你有帮助
- 如果你还需要，我可以继续
- 下面是、以下是、我将为你
- 作为一个 AI、根据我的训练数据、截至我的知识更新

## Fake Intimacy And Platform Cliches

Use only when the original platform and audience require them:

- 家人们、宝子们、姐妹们、朋友们、亲爱的读者
- 真的绝了、谁懂啊、狠狠爱住、闭眼冲、直接封神
- 一整个、狠狠、拿捏、天花板、YYDS

For Xiaohongshu/Douyin, replace cliches with lived details instead of making the text stiff.
```

## structures.md

```markdown
# Structures

Chinese AI traces often live in structure rather than individual words. Fix structure before polishing words.

## Essay Skeleton

Avoid defaulting to:

```text
开篇定义/背景 -> 首先 -> 其次 -> 再次 -> 最后 -> 总结升华
```

Use one of these instead:

- Start with the actual claim.
- Start with a scene where the problem appears.
- Start with the surprising constraint.
- Start with the user's choice or tradeoff.
- Tell one story in time order.
- Explain one point deeply instead of listing three shallow points.

## Three-Part Balance

Patterns:

- 是...，是...，更是...
- 不仅是...，更是...
- 既要...，又要...，还要...
- 从...到...，从...到...
- 让...更...，让...更...，让...更...
- A、B、C 三个 nouns stacked to sound complete

Fix:

- Keep the one point that carries meaning.
- Split genuinely different claims into separate sentences.
- Use two items when both matter.
- Replace a list with one example.

Example:

> AI 不仅是工具，更是伙伴，更是未来生产力的入口。

Rewrite:

> 团队把 AI 当工具用：写测试、查日志、整理客服问题。

## Negative Contrast

Patterns:

- 不是 X，而是 Y
- 不只是 X，更是 Y
- 问题不在于 X，而在于 Y
- 真正重要的不是 X，而是 Y

Fix by stating Y directly unless the contrast carries real information.

## Abstract Subject Agency

Patterns:

- 时代呼唤...
- 科技改变...
- AI 赋能...
- 市场奖励...
- 行业推动...
- 数据告诉我们...
- 现实要求...

Fix:

- Name who acts.
- If the actor is unknowable, name the process.
- If the process is also vague, cut the sentence.

Example:

> 市场正在奖励更高效的团队。

Rewrite:

> 买家把预算给了能在两周内上线试点的团队。

## Nominalized Action Chains

Patterns:

- 对...进行...
- 为...提供...
- 通过...实现...
- 围绕...开展...
- 持续推进...建设
- 进一步加强...能力

Fix by finding the verb and object.

Example:

> 我们将围绕用户反馈开展产品体验优化工作。

Rewrite:

> 本周先改两个问题：登录慢，导出表格容易失败。

## Generic Meaning Inflation

Patterns:

- 标志着...
- 象征着...
- 体现了...
- 彰显了...
- 凸显了...
- 为...奠定基础
- 对...具有重要意义

Fix:

- If the sentence does not add factual information, delete it.
- If it has a real implication, name the implication.

## Evidence Leap

Patterns:

- Crowdfunding backers -> "market demand proven"
- Market-size report -> "this startup will grow"
- Product page promise -> "feature works"
- Theoretical model -> "final proof"
- Legal clause -> "risk eliminated"
- Media coverage -> "industry recognition"

Fix:

- State the evidence first.
- Name the narrow inference.
- Add the missing uncertainty if the original claim crosses the evidence boundary.

Example:

> 众筹 48.2 万美元成功验证了市场真实需求。

Rewrite:

> 众筹 48.2 万美元说明，早期支持者愿意提前付费。大众渠道转化、交付能力和留存还要单独验证。

## Vague Range

Patterns:

- 从个人到社会
- 从线上到线下
- 从认知到行动
- 覆盖工作、生活、学习的方方面面

Fix:

- Name the actual range.
- Use examples only when they are specific and relevant.

## Over-Formatted AI Output

Watch for:

- Every bullet starts with bold title + colon.
- Every section has "概念解释 -> 重要性 -> 做法 -> 小结".
- Emojis decorate headings.
- Tables are used to make thin ideas look structured.

Fix:

- Merge bullets into paragraphs when the items are not truly scan-worthy.
- Keep lists only for steps, options, requirements, or comparisons.
- Remove decorative emojis and mechanical bolding unless the user requested platform formatting.

## Repetition By Synonym

Chinese AI text often rotates synonyms to avoid repetition:

- 用户 / 消费者 / 受众 / 人群 / 客群
- 企业 / 组织 / 公司 / 平台 / 机构
- 问题 / 挑战 / 痛点 / 难题

Fix:

- Use one stable term when it refers to the same thing.
- Use different terms only when the distinction matters.

## Ending Patterns

Avoid ending every paragraph with a punchline, slogan, or value elevation. Let some paragraphs end on facts, examples, or a plain consequence.

Weak:

> 这就是长期主义的价值。

Better:

> 三个月后，续费率从 62% 回到 74%。
```
