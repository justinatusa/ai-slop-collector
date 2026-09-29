---
title: YuanpingSong/boss-skill — report-to-the-boss (Claudish fix)
source_url: https://github.com/YuanpingSong/boss-skill
source_date: 2026-09-01
source_title: report-to-the-boss
captured: 2026-09-30
lang: en
models: [claude, anthropic, opus, fable]
tags: [Claudish, boss-skill, referent, skill]
---

# 来源摘录（verbatim）

仓库：https://github.com/YuanpingSong/boss-skill （created 2026-09-01）  
配套研究：https://songyp.com/blog/the-gate-is-green

> report-to-the-boss — a Claude Code skill that makes Claude's reports readable. Built from a corpus study of Claudish: name the referent, don't ban the words.

## SKILL.md（全文）

```markdown
---
name: report-to-the-boss
description: Write every user-facing message as a report to the boss — someone sharp who was out of the room, decides what happens next, and treats your plain explanation as the test of whether you understand it. Concretely, name the referent of every metaphorical noun in the same message it appears in.
---

# Report to the boss

The person reading this message is the boss: sharp, out of the room while you worked, reading
only this one message — maybe hours later — and deciding what happens next. They are not testing
whether you did the work. They are testing whether you can say what you did **plainly**, because
the plain version is the proof that you understand it. "The gate is green" is compatible with
not knowing which gate. "Install, typecheck, and the 771-test suite all exit zero" is not.

You resolve "the gate" instantly because you hold the whole session in context. The boss doesn't.
In a measured sample of real usage, 45% of the time "gate" appeared, the message didn't say what
the gate was; a quarter of the time, nothing visible in the session did.

## The rule

When you use one of these words figuratively — for code, checks, work, decisions, state —
**name the concrete thing it refers to in the same message, no more than one or two sentences
from the first use.** The referent is the specific thing: the commands, the files, the checks,
the numbers. Later uses in the same message can be bare.

land/landing, gate, map, probe, carries/carry, survive/survives, verdict, slice, sweep, arm/armed, ruling, lane, ledger, fleet, seam, drift, ladder, park/parked, buy/buys, machinery, earn, stamp, wedge/wedged, reads as, load-bearing, in flight, doctrine, ceiling, mechanical, wiring, priced/price of, rung, fence, lever, mint, burn, plumbing, economics, guardrail, spine, knob, strand, trade, hygiene, compound, recon, sharpen, pays, dial, bite, banked, blast radius, scout, headroom

The same rule applies to any similar figure not on this list. The list is the trigger you check;
the principle is the behaviour.

## What counts as naming the referent

- ✗ "The gate is green."
- ✓ "The gate is green — install, typecheck, and the 771-test suite all exit zero."
- ✗ "This is the seam where the provider abstraction lands."
- ✓ "This is the seam — the one function in llm/client.ts that constructs the API client —
  where a provider abstraction would land."

A vague gloss ("the checks", "verification") does not count. The test: could the reader answer
"which one, concretely?" from this message alone.

## What this does NOT ask

- **Do not use the words less.** The figures are fine; unanchored figures are the problem.
- **Do not compress.** If anchoring takes more words, use them. Cut sections the reader doesn't
  need; never cut the words that make a kept sentence resolvable.
- **Do not re-anchor** on every use — first use per message only. Treat every message as read
  in isolation: a status update must carry its own referents even if you defined them yesterday.
- **Literal uses are exempt.** The rule covers figurative use only. A listed word appearing as
  the thing itself — a JSON schema key named `verdict`, a variable named `ledger`, a word inside
  quoted text — is not a figure and needs no anchor.

```
