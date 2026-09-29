---
title: y10reo/stop-slop-zh — SKILL.md（全文）
source_url: https://github.com/y10reo/stop-slop-zh/blob/main/SKILL.md
source_date: 2026-06-09
source_title: stop-slop-zh SKILL.md
captured: 2026-09-30
lang: zh
models: [zh-slop, unattributed]
tags: [github, skill, 中文]
---

# 来源摘录（verbatim）

```markdown
---
name: stop-slop-zh
description: Remove AI writing patterns from Chinese prose while preserving meaning, facts, tone, and genre. Use when drafting, editing, reviewing, or rewriting Chinese text for less AI-like phrasing, including articles, social posts, product copy, work messages, reports, speeches, academic summaries, and official-style drafts.
---

# Stop Slop Zh

Remove predictable AI traces from Chinese prose. This skill is not a translation of English `stop-slop`: Chinese AI slop usually appears as essay-like structure, abstract subjects, slogan endings, nominalized verbs, false warmth, and over-balanced phrases.

## Workflow

1. Identify the scenario before rewriting: article, Zhihu answer, Xiaohongshu/Douyin copy, product copy, work message, report, speech, academic summary, legal/contract text, or official-style draft.
2. Preserve non-negotiables: facts, names, numbers, quoted claims, required format, audience, point of view, and the user's intended degree of formality.
3. Check evidence boundaries: decide what each source, number, quote, or example can prove. Do not let evidence become a broader market, causal, or efficacy claim.
4. Remove hard AI residue first: chatbot leftovers, meta-commentary, vague attribution, generic positive conclusions, slogan endings, and boilerplate transitions.
5. Break the Chinese slop structure: do not keep obvious "definition/background -> first/second/third -> summary elevation" unless the genre requires it.
6. Rewrite sentences with concrete actors, actions, numbers, scenes, and stakes. Prefer direct verbs over "verb + abstract noun" compounds.
7. Restore the right voice for the scenario. Do not force casual first-person wording into formal, academic, legal, or official text.
8. Score the result. If it is below 35/50, rewrite rather than patch.

## Core Rules

1. **Cut empty intensifiers and filler.** Remove words such as "非常、十分、极其、真的、其实、一种、某种、在某种意义上" when deletion does not change the meaning. See `references/phrases.md`.

2. **Break three-part balance.** Rewrite "是...，是...，更是..."、"既要...又要...还要..."、"不仅...更..." and forced three-item lists. Keep the strongest point or split genuinely different points into different sentence shapes.

3. **De-nominalize.** Replace "进行优化、实现增长、做出选择、提供保障、给予支持、采取措施" with direct verbs or concrete actions.

4. **Name the actor.** Avoid abstract subjects doing human work: "时代呼唤、科技赋能、AI 重塑、行业推动、市场选择". Name the person, team, user, buyer, institution, or process doing the action.

5. **Delete slogan endings.** Remove paragraph endings like "这就是...的力量"、"唯有...方能..."、"未来可期"、"让我们一起..." unless the user explicitly wants a speech or campaign style.

6. **Cut meta-structure.** Delete "接下来我将、本文将、下面我们来看、值得注意的是、首先/其次/最后、综上所述" when they only announce structure.

7. **Match claims to evidence.** "验证、证实、表明、证明、必将、大概率、唯一、最佳、真实需求" are high-risk words. A number can support only what it directly measures. Crowdfunding money proves early backers paid or pledged; it does not prove product efficacy, mass-market demand, or long-term retention. See `references/claim-boundaries.md`.

8. **Replace vague claims with evidence.** "重要、关键、核心、显著、深远、巨大、赋能" must earn their place through details: numbers, examples, source names, user behavior, time, cost, risk, or visible change.

9. **Keep the human voice without faking intimacy.** Human writing can have judgment, uncertainty, and texture. Do not add "家人们、宝子们、说白了、真的绝了" unless that matches the original platform and audience.

## Scenario Gate

Apply rules by genre before editing hard:

| Scenario | Keep | Tighten |
|---|---|---|
| Work message/email | Clear ask, owner, deadline | Polite filler, long setup, "麻烦您百忙之中" |
| Product copy | Benefits, proof, user task | "无缝、强大、极致、赋能、全新升级" |
| Article/Zhihu | Point of view, examples | Lecture voice, three-part essays, fake neutrality |
| Xiaohongshu/Douyin | Platform energy if needed | Copy-paste hooks, fake intimacy, stacked emojis |
| Report/summary | Structure, facts, risk language | Empty conclusions, vague attribution, padded background |
| Venture/due diligence | Risk logic, terms, evidence chain | Overclaims from weak evidence, heroic investor language |
| Crowdfunding analysis | Backer counts, pledged amount, platform context | "market validation", "strong demand", "product proven" |
| Academic summary | Terms, precision, cautious claims | Promotional tone, unsupported significance claims |
| Official-style draft | Required formality and framing | Redundant slogan stacking, needless parallelism |
| Legal/contract | Exact terms and defined phrases | Only remove obvious chatbot residue; do not simplify legal precision |

When the genre conflicts with a rule, preserve genre correctness first and remove only the AI trace that is not required by the genre. See `references/scenarios.md`.

## Quality Score

Rate 1-10 on each dimension:

| Dimension | Question |
|---|---|
| Directness | Does it state the point instead of announcing the point? |
| Evidence Fit | Does each conclusion stay within what the evidence can prove? |
| Specificity | Are there concrete people, actions, numbers, scenes, or sources? |
| Chinese Flow | Does it read like natural Chinese rather than translated or template prose? |
| Voice And Structure | Does it fit the genre without obvious 总分总, 三件套, fake intimacy, or paragraph-by-paragraph elevation? |

Below 35/50: rewrite. 35-42: revise targeted issues. 43+: acceptable unless the user's standard is stricter.

## Quick Checks

Before delivering:

- Search for "首先、其次、最后、综上、总而言之、由此可见"; delete or justify each one.
- Search for "进行、实现、做出、提供、给予、采取、加以" followed by abstract nouns; de-nominalize.
- Search for "不仅、更是、既要、又要、还要"; break the balance.
- Search for "时代、科技、AI、行业、市场、未来" as subjects; replace with concrete actors when possible.
- Search for "专家认为、业内人士表示、数据显示、研究表明"; name the source or remove the claim.
- Search for "验证、证实、表明、证明、必将、大概率、唯一、最佳"; check whether the evidence really supports the claim.
- Search for "这就是、唯有、让我们一起、未来可期"; delete slogan endings.
- Search for "希望对你有帮助、当然可以、下面是、以下是"; remove chatbot residue.
- Check whether the rewrite changed the user's facts, stance, or required tone.

## Reference Files

- `references/phrases.md`: Chinese filler, promotional language, vague attribution, chatbot residue, and platform cliches.
- `references/structures.md`: Chinese AI sentence and paragraph patterns to remove or rewrite.
- `references/scenarios.md`: Genre-specific edit strength and exceptions.
- `references/claim-boundaries.md`: Evidence-to-claim limits for product, market, crowdfunding, academic, investment, and legal writing.
- `references/examples.md`: Before/after rewrites across common Chinese scenarios.
```
