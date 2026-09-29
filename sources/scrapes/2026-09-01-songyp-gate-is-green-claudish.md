---
title: The Gate Is Green — Claudish 50-word dictionary (measured)
source_url: https://songyp.com/blog/the-gate-is-green
source_date: 2026-09-01
source_title: The Gate Is Green
author: Max Song
captured: 2026-09-30
lang: en
models: [claude, anthropic, opus, fable, gpt, gpt-5]
tags: [Claudish, Claudeish, load-bearing, dictionary, corpus-study]
---

# 来源摘录（verbatim）

来源：Max Song, *The Gate Is Green*（2026-09-01）。原文：https://songyp.com/blog/the-gate-is-green  
方法：82 天 Claude Fable/Opus 输出 1.25M 词 vs 人类工程 prose 927k vs 同机 GPT-5 886k。

## TL;DR

> Why Claude's messages are hard to read — measured. With a 50-word dictionary of Claudish and the one instruction that targets the actual problem.

## Finding 1 — figurative nouns

> Claude's vocabulary is more concrete than mine, not less. Its signature move is using a concrete, physical noun for an abstract thing — the gate, the seam, the ledger, the lane. Nothing in your repo is any of those things.
>
> Against a 927,000-word corpus of pre-AI engineering prose … Claude runs about 7× the overall density of figurative language … Figurative nouns: 10.5×.
>
> Claude every 71 words one figurative noun; human engineers every 750 words one figurative noun.

## Finding 3 — mostly LLM, not only Claude

> | writer | figures per 1,000 words |
> | Claude 5 | 32.5 |
> | GPT-5, same machine | 23.3 |
> | human engineers | 4.3 |
>
> GPT-5 runs at 72% of Claude's rate — and five times the human rate. … load-bearing really is Claude (18× GPT-5's rate) … seam and handoff … more GPT-5 than Claude.

## Why ban-lists fail

> We banned the 17 most Claudish words. Compliance was perfect — all 17 vanished. And unlisted figures rose by 128% of the removed volume: fence appeared where guardrail was banned, land where gate was banned, carries where load-bearing was banned.

## Dictionary highlights (50 Claudish words; rates vs humans)

摘录部分词条（全文见原链）：

- **load-bearing** — Claude 133/M, humans absent. "so important that everything else depends on it"
- **gate** — Claude 2259/M, humans 18/M — verification run with authority to refuse
- **land / landing** — Claude 2362/M — work arrived complete at destination
- **seam** — join between two sides of a system
- **ledger / lane / fleet / spine / doctrine / blast radius / guardrail / wedge / plumbing / machinery**

## The fix

> The rule: use all fifty words freely — but on first use in a message, name the concrete referent within a sentence or two.
>
> Skill: https://github.com/YuanpingSong/boss-skill — `/report-to-the-boss`
