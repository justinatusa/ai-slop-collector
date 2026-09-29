---
title: hannsxpeter/humanizer — tell-patterns de-slop skill
source_url: https://github.com/hannsxpeter/humanizer
source_date: 2026-05-15
source_title: humanizer — Pure-prompt skill that de-slops AI-sounding prose
captured: 2026-09-30
lang: en
models: [claude, gpt, gemini, unattributed]
tags: [humanizer, tell-patterns, skill, Copilot, Gemini]
---

# 来源摘录（verbatim）

仓库：https://github.com/hannsxpeter/humanizer （created 2026-05-15）

## README

> Pure-prompt skill that de-slops AI-sounding prose and rewrites it in a writer's voice, with faithfulness and restraint guards. Works with Claude Code, Cursor, Codex, Antigravity, Gemini, Pi Coder, OpenCode, and Copilot.

## tell-patterns.md（节选）

```markdown
# Tell-Pattern Catalog

Read this during Pass 2 (tell removal). This is a diagnostic lens, not a
find-and-replace table. For every flag, fix the underlying thought, then check
the **Restraint** note before touching anything. A single instance is rarely a
tell; recurrence and co-occurrence are what give a machine away. The one
exception is pattern 31 (chat-UI contamination): a single instance is
near-certain confirmation.

Each entry has four parts:

- **Detect** what it looks like in the wild.
- **Why it reads as AI** the underlying tendency, so you fix the cause.
- **Before / After** one concrete pair.
- **Restraint** when this is genuinely fine and should be left alone.

## Table of contents

**Family A: Inflated significance**
1. Undue emphasis on significance, legacy, and broader trends
2. Notability and media-coverage name-dropping
3. Superficial "-ing" analyses
4. Persuasive-authority tropes

**Family B: Promotional and evasive language**
5. Promotional and advertisement-like language
6. Vague attribution and weasel words
7. Sycophantic and servile tone
8. Filler phrases
9. Excessive hedging

**Family C: Formulaic structure**
10. Formulaic "challenges and future prospects"
11. Negative parallelism and tailing negation
12. Rule-of-three overuse
13. Generic positive conclusion
14. Signposting and announcements
15. Diff-anchored writing

**Family D: Lexical tics**
16. Overused AI vocabulary
17. Elegant variation (synonym cycling)
18. False ranges
19. Hyphenated-pair overuse

**Family E: Syntactic tics**
20. Copula avoidance
21. Passive voice and subjectless fragments

**Family F: Formatting and artifacts**
22. Em dash overuse
23. Boldface overuse
24. Inline-header vertical lists
25. Title case in headings
26. Decorative emojis
27. Curly quotation marks
28. Collaborative chatbot artifacts
29. Knowledge-cutoff disclaimers
30. Fragmented headers
31. Chat-UI contamination artifacts
32. Debunking-pose headings

---

## Family A: Inflated significance

The model reaches for importance it has not earned. The fix is almost always
to delete the inflation and let the concrete fact carry its own weight.

### 1. Undue emphasis on significance, legacy, and broader trends

- **Detect:** "marks a pivotal moment," "stands as a testament," "underscores
  the importance of," "reflects a broader shift," "a turning point in."
- **Why it reads as AI:** the model editorializes about importance instead of
  reporting the thing, because grand framing is high-probability filler.
- **Before:** "The acquisition stands as a pivotal moment, reflecting broader
  shifts in the tooling landscape."
- **After:** "The acquisition was Notion's biggest yet, and it finally gave
  them the calendar product they had failed to build twice."
- **Restraint:** real historical significance, stated plainly with evidence, is
  not this pattern. "It was the first FDA approval for the class" is a fact.

### 2. Notability and media-coverage name-dropping

- **Detect:** listing outlets or famous names purely to borrow credibility:
  "covered by major outlets," "praised by leading experts."
- **Why it reads as AI:** the model gestures at authority it cannot cite
  specifically, so it name-drops categories.
- **Before:** "The study was widely covered by major media and praised by
  leading researchers."
- **After:** "Nature ran it as a cover story; two replication attempts have
  since failed."
- **Restraint:** a specific, sourced attribution ("per the FT's March audit")
  is the opposite of this pattern. Keep it.

### 3. Superficial "-ing" analyses

- **Detect:** participle phrases tacked on to simulate depth: "...sparking
  debate," "...highlighting the need for," "...paving the way for."
- **Why it reads as AI:** the trailing gerund implies analysis without doing
  any. It is a rhythmic reflex, not a thought.
- **Before:** "The feature shipped late, highlighting the need for better
  planning and underscoring broader process gaps."
- **After:** "The feature shipped six weeks late because the spec changed
  twice in QA."
- **Restraint:** a participle that carries real information ("...shipping with
  a known data-loss bug") is fine. The test is whether it says anything.

### 4. Persuasive-authority tropes

- **Detect:** "at its core," "what really matters here," "the key takeaway is,"
  "make no mistake," "the truth is."
- **Why it reads as AI:** the model performs insight with a frame instead of
  delivering the insight.
- **Before:** "At its core, what really matters here is that users want speed."
- **After:** "Users abandoned the flow at the 4-second mark. They want speed."
- **Restraint:** an occasional emphatic frame in genuinely argumentative or
  spoken-register prose is human. One per piece is not a tell.

---

## Family B: Promotional and evasive language

The model sells, softens, or pads. Fixes here usually shorten the text.

### 5. Promotional and advertisement-like language

- **Detect:** "vibrant," "stunning," "seamless," "breathtaking," "nestled,"
  "rich tapestry," "must-have," "game-changing."
- **Why it reads as AI:** marketing register is dense in training data and
  gets applied where neutral description belongs.
- **Before:** "This stunning, seamless platform offers a rich tapestry of
  game-changing features."
- **After:** "The platform does three things: import, dedupe, and export.
  The dedupe is the only part competitors do not have."
- **Restraint:** actual marketing copy the user asked for can be vivid. Match
  the brief. This pattern is about unbidden ad-speak in neutral prose.

### 6. Vague attribution and weasel words

- **Detect:** "experts say," "studies show," "many believe," "it is widely
  regarded," "some argue."
- **Why it reads as AI:** the model invokes consensus it cannot source.
- **Before:** "Experts say the approach is generally effective."
- **After:** "In the 2024 Cochrane review of 12 trials, it beat placebo in 9."
  (If no source exists, drop the claim or own it: "I think it works.")
- **Restraint:** honest uncertainty stated as the writer's own ("I am not
  sure, but my read is...") is human and should stay.

### 7. Sycophantic and servile tone

- **Detect:** "Great question!" "I hope this helps," "happy to dive deeper,"
  reflexive praise of the topic or reader.
- **Why it reads as AI:** assistant-training rewards agreeableness; it leaks
  into the prose.
- **Before:** "That's a fantastic point, and it's absolutely worth exploring
  this important topic further."
- **After:** (delete entirely; start with the substance.)
- **Restraint:** genuine warmth in a personal letter or note is not servility.
  Context decides.

### 8. Filler phrases

- **Detect:** "due to the fact that," "in order to," "it is worth noting
  that," "in the realm of," "when it comes to."
- **Why it reads as AI:** padding raises token count without raising content.
- **Before:** "In order to improve performance, it is worth noting that
  caching, when it comes to read paths, helps."
- **After:** "Caching the read path cut p95 latency in half."
- **Restraint:** "in order to" once, for rhythm, is not a crime. Flag the
  cluster, not the lone instance.

### 9. Excessive hedging

- **Detect:** stacked qualifiers: "may potentially sometimes," "it could
  arguably be considered," "in some cases this might possibly."
- **Why it reads as AI:** safety training rewards non-commitment.
- **Before:** "This could potentially, in some cases, arguably be considered a
  minor improvement."
- **After:** "This is a small improvement. It saves about 200ms."
- **Restraint:** one honest hedge on a genuinely uncertain claim is good
  writing. Mixed feelings are a human marker (see do-not-flag.md). Keep them.

---

## Family C: Formulaic structure

The model defaults to template shapes. Fixes here change the architecture of
the passage, not its words.

### 10. Formulaic "challenges and future prospects"

- **Detect:** a section that lists generic difficulties followed by generic
  optimism: "Despite challenges, the future looks bright."
- **Why it reads as AI:** it is a learned essay scaffold filled with
  placeholders.
- **Before:** "Despite challenges around adoption and cost, the future of the
  technology remains promising."
- **After:** "The blocker is cost: it is 4x the incumbent and the price has
  not moved in two years. Nobody has a credible plan to change that."
```
