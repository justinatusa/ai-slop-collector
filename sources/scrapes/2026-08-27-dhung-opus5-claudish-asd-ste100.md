---
title: Opus 5 Claudish — how to shut it up (ASD-STE100)
source_url: https://dhung.dev/blog/opus-5-claudish-here-is-how-to-shut-it-up
source_date: 2026-08-27
source_title: Opus 5 Claudish. Here is how to shut it up.
captured: 2026-09-30
lang: en
models: [claude, anthropic, opus]
tags: [Claudish, Opus5, ASD-STE100, coined-terms]
---

# 来源摘录（verbatim）

来源：dhung.dev，2026-08-27。

> I keep seeing people complain because Opus 5 is Claudish (a new term if you ask me, this was never a problem back on Opus 4.6).

## Core diagnosis

> Opus 5 makes up names for things, and puts the answer I asked for somewhere in the middle.

## ASD-STE100 style rules (excerpt)

> 1. **One word, one meaning.** Pick one term per concept. Never vary it, never reuse it for something else.
> 2. **One sentence, one action.** Split anything doing double duty.
> 3. **Command or state, never hedge.** … Active voice, simple tense …
> 6. **Break clusters apart.** No noun stacks over three words, no essential info in parentheses, no em dashes, no semicolons, use lists for sequences.
>
> **Never coin a term, and never write a sentence that needs one.** … Eight forms follow. … metaphors as names … slogans …

## AVOID / PREFER

> AVOID   The cache isn't the bottleneck, the serializer is. This is the load-bearing insight.
> PREFER  The serializer is the bottleneck. The cache performs fine.
>
> AVOID   Fixed. The retry path now short-circuits on the tombstone marker, which keeps the dead-letter lane honest.
> PREFER  Fixed. Deleted records are now skipped during retry, so failed jobs no longer reprocess them.

> The style on its own works for the first twenty or thirty turns, then the Claudish creeps back …
