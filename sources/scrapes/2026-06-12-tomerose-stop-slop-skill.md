---
title: tomerose/stop-slop — 去AI味 Skill（中英）
source_url: https://github.com/tomerose/stop-slop
source_date: 2026-06-12
source_title: Stop Slop — 去 AI 味写作技能
captured: 2026-09-30
lang: zh
models: [claude, gpt, zh-slop, unattributed]
tags: [stop-slop, skill, Copilot, Claude]
---

# 来源摘录（verbatim）

仓库：https://github.com/tomerose/stop-slop （created 2026-06-12）

## README 定位

> 去AI味写作技能 — 5维评分体系，检测41种AI反模式。让 Claude/Cursor/Copilot 写出人话。

## SKILL.md（全文）

```markdown
---
name: stop-slop
description: Remove AI writing patterns from prose. Use when drafting, editing, or reviewing text to eliminate predictable AI tells. Triggers on: writing prose, editing drafts, reviewing content, 写作, 文案, 去AI味.
version: 1.0.0
author: MangoOS × 第三自习室
license: MIT
tags: [writing, editing, AI-detection, prose, quality, chinese, english]
marketplace:
  claude-skills: true
  cursor-skills: true
  copilot-skills: true
---

# Stop Slop — 去 AI 味写作

Eliminate predictable AI writing patterns from prose. 系统化检测并消除 AI 写作反模式。

## Core Rules

1. **Cut filler phrases.** Remove throat-clearing openers, emphasis crutches, and all adverbs. See [references/phrases.md](references/phrases.md).

2. **Break formulaic structures.** Avoid binary contrasts, negative listings, dramatic fragmentation, rhetorical setups, false agency. See [references/structures.md](references/structures.md).

3. **Use active voice.** Every sentence needs a human subject doing something. No passive constructions. No inanimate objects performing human actions.

4. **Be specific.** No vague declaratives. Name the specific thing. No lazy extremes ("every," "always," "never").

5. **Put the reader in the room.** No narrator-from-a-distance voice. "You" beats "People." Specifics beat abstractions.

6. **Vary rhythm.** Mix sentence lengths. Two items beat three. End paragraphs differently. No em dashes.

7. **Trust readers.** State facts directly. Skip softening, justification, hand-holding.

8. **Cut quotables.** If it sounds like a pull-quote, rewrite it.

## Quick Checks

Before delivering prose, scan for:

- [ ] Any adverbs? Kill them.
- [ ] Any passive voice? Find the actor, make them the subject.
- [ ] Inanimate thing doing a human verb? Name the person.
- [ ] Sentence starts with a Wh- word? Restructure.
- [ ] Any "here's what/this/that" throat-clearing? Cut to the point.
- [ ] Any "not X, it's Y" contrasts? State Y directly.
- [ ] Three consecutive sentences match length? Break one.
- [ ] Paragraph ends with punchy one-liner? Vary it.
- [ ] Em-dash anywhere? Remove.
- [ ] Vague declarative? Name the specific implication.
- [ ] Narrator-from-a-distance? Put the reader in the scene.
- [ ] Meta-joiners ("The rest of this essay...")? Delete.

## Scoring

Rate 1-10 on each dimension:

| Dimension | Question |
|-----------|----------|
| Directness | Statements or announcements? |
| Rhythm | Varied or metronomic? |
| Trust | Respects reader intelligence? |
| Authenticity | Sounds human? |
| Density | Anything cuttable? |

**Below 35/50: revise. Target ≥ 45/50 for publishable quality.**

## Examples

See [references/examples.md](references/examples.md) for before/after transformations.

## Chinese-Specific Notes

中文 AI 写作的额外反模式：

- **"在当今...的时代"** → 砍掉，直接说
- **"不仅仅是...更是..."** → 二元对立的中文变体
- **"值得我们深思"** → 让读者自己判断
- **"随着...的发展"** → 万能开头模板
- **"综上所述"** → 直接给结论
- **四字成语堆砌** → 每段最多1个
- **"毋庸置疑/显而易见/众所周知"** → 全砍

## License

MIT

```

## phrases.md（节选）

```markdown
# Phrases to Remove

## Throat-Clearing Openers

Remove these announcement phrases. State the content directly.

- "Here's the thing:"
- "Here's what [X]"
- "Here's this [X]"
- "Here's that [X]"
- "Here's why [X]"
- "The uncomfortable truth is"
- "It turns out"
- "The real [X] is"
- "Let me be clear"
- "The truth is,"
- "I'll say it again:"
- "I'm going to be honest"
- "Can we talk about"
- "Here's what I find interesting"
- "Here's the problem though"

Any "here's what/this/that" construction is throat-clearing before the point. Cut it and state the point.

## Emphasis Crutches

These add no meaning. Delete them.

- "Full stop." / "Period."
- "Let that sink in."
- "This matters because"
- "Make no mistake"
- "Here's why that matters"

## Business Jargon

Replace with plain language.

| Avoid | Use instead |
|-------|-------------|
| Navigate (challenges) | Handle, address |
| Unpack (analysis) | Explain, examine |
| Lean into | Accept, embrace |
| Landscape (context) | Situation, field |
| Game-changer | Significant, important |
| Double down | Commit, increase |
| Deep dive | Analysis, examination |
| Take a step back | Reconsider |
| Moving forward | Next, from now |
| Circle back | Return to, revisit |
| On the same page | Aligned, agreed |

## Adverbs

Kill all adverbs. No -ly words. No softeners, no intensifiers, no hedges.

Specific offenders:

- "really"
- "just"
- "literally"
- "genuinely"
- "honestly"
- "simply"
- "actually"
- "deeply"
- "truly"
- "fundamentally"
- "inherently"
- "inevitably"
- "interestingly"
- "importantly"
- "crucially"

Also cut these filler phrases:

- "At its core"
- "In today's [X]"
- "It's worth noting"
- "At the end of the day"
```

## structures.md（节选）

```markdown
# Structures to Avoid

## Binary Contrasts

These create false drama. State the point directly.

| Pattern | Problem |
|---------|---------|
| "Not because X. Because Y." / "Not because X, but because Y." | Telegraphed reversal |
| "[X] isn't the problem. [Y] is." | Formulaic reframe |
| "The answer isn't X. It's Y." | Predictable pivot |
| "It feels like X. It's actually Y." | Setup/reveal cliche |
| "The question isn't X. It's Y." | Rhetorical misdirection |
| "Not X. But Y." / "not X, it's Y" / "isn't X, it's Y" | Mechanical contrast |
| "It's not this. It's that." | Same formula, different words |
| "stops being X and starts being Y" | False transformation arc |
| "doesn't mean X, but actually Y" | Negation-then-assertion crutch |
| "is about X but not Y" | False distinction |
| "not just X but also Y" | Additive hedge |

**Instead:** State Y directly. "The problem is Y." "Y matters here." Drop the negation entirely.

## Negative Listing

Listing what something is *not* before revealing what it *is*. A rhetorical striptease.

| Pattern | Problem |
|---------|---------|
| "Not a X... Not a Y... A Z." | Dramatic buildup through negation |
| "It wasn't X. It wasn't Y. It was Z." | Same structure, past tense |

**Instead:** State Z. The reader doesn't need the runway.

## Dramatic Fragmentation

Sentence fragments for emphasis read as manufactured profundity.

| Pattern | Problem |
|---------|---------|
| "[Noun]. That's it. That's the [thing]." | Performative simplicity |
| "X. And Y. And Z." | Staccato drama |
| "This unlocks something. [Word]." | Artificial revelation |

**Instead:** Complete sentences. Trust content over presentation.

## Rhetorical Setups

These announce insight rather than deliver it.

| Pattern | Problem |
|---------|---------|
| "What if [reframe]?" | Socratic posturing |
| "Here's what I mean:" | Redundant preview |
| "Think about it:" | Condescending prompt |
| "And that's okay." | Unnecessary permission |

**Instead:** Make the point. Let readers draw conclusions.

## Formulaic Constructions

| Pattern | Problem |
|---------|---------|
| "By the time X, I was Y." | Narrative template |
| "X that isn't Y" | Indirect. Say "X is broken" |

## False Agency

Giving inanimate things human verbs. Complaints don't "become" fixes. Bets don't "live or die." Decisions don't "emerge." A person does something to make those things happen. AI loves this because it avoids naming the actor.

| Pattern | Problem |
|---------|---------|
| "a complaint becomes a fix" | The complaint did nothing. Someone fixed it. |
| "a bet lives or dies in days" | Bets don't have lifespans. Someone kills the project or ships it. |
| "the decision emerges" | Decisions don't emerge. Someone decides. |
| "the culture shifts" | Cultures don't shift on their own. People change behavior. |
| "the conversation moves toward" | Conversations don't move. Someone steers. |
| "the data tells us" | Data sits there. Someone reads it and draws a conclusion. |
| "the market rewards" | Markets don't reward. Buyers pay for things. |

**Instead:** Name the human. "The team fixed it that week" beats "the complaint becomes a fix." If no specific person fits, use "you" to put the reader in the seat.
```
