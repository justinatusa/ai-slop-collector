---
title: 说人话 — 「钉死」归入暴力动作腔（operation-manual + v1.9.2）
source_url: https://github.com/MrGeDiao/shuorenhua/blob/main/evals/legacy-v2.4.1/references/operation-manual.md.txt
source_date: 2026-07-05
source_title: 微操作手册（legacy v2.4.1 归档）/ CHANGELOG v1.9.2
author: MrGeDiao
captured: 2026-09-30
lang: zh
models: [gpt, chatgpt, gpt-5, gpt-5.x-codex, claude, opus, zh-slop]
tags: [钉死, 暴力动作腔, 说人话, skill]
---

# 来源摘录（verbatim）

主链：https://github.com/MrGeDiao/shuorenhua/blob/main/evals/legacy-v2.4.1/references/operation-manual.md.txt  
对照：https://github.com/MrGeDiao/shuorenhua/releases/tag/v1.9.2 ；CHANGELOG `[1.9.2] - 2026-07-05` 写明「暴力动作腔补 `钉死`」。

> 注：现行 v2.5.0 运行包已收为 SKILL + editing-guide + examples；本文件是 legacy 归档，仍含「钉死」归类原文。

## 变体归并 · 暴力动作腔（legacy operation-manual）

### 默认动作

- 先判它属于哪一类，再决定怎么改，不要先急着往词表加新词
- 现阶段默认归到这 7 类：
  - `调试腔 / 工程师腔`：`收窄 / 坐实 / 对上了 / 锁住 / 收口 / 更硬`
  - `庸医问诊腔`：`抠出来 / 揪出来 / 扒开 / 拽出来 / 捞出来`
  - **`暴力动作腔`：`砍一刀 / 补一刀 / 钉死 / 狠狠干 / 拍脑门`**
  - `主动出击腔`：`要不要我 / 我立马开始 / 只要你回复我 / 顺手 / 趁热 / 我先……`
  - `总结提示腔`：`一句话总结 / 结论先说 / 简单的说 / 说人话就是`
  - `过度接住 / 心理判断腔`：`你只是太久没被稳稳接住了 / 不用向我解释 / 你不是敏感`
  - `郑重预告 / 身份认证式夸奖`：`我必须很认真地说一句 / 你问到了问题的核心 / 顶刊作者的素养`
- 同类变体默认按代表项同样处理：删姿态层，保留真正的动作、事实和结论，以及条件与情态

## CHANGELOG v1.9.2（对照摘录）

## [1.9.2] - 2026-07-05 — Claude 5 口癖巡检 / 标点腔 pattern pack

### Changed
- references/operation-manual.md 变体归并：郑重预告族补「诚实宣言」（我必须诚实地说 / 说句实话）与「装坦诚」（说个真实变化 / 缺点也说一句）两组识别信号，明确只删姿态层、自曝的真信息必须保留；**暴力动作腔补 `钉死`**；主动出击腔补 `趁热`；语域混搭补「强行游戏化 / 职业化比喻」识别信号（刺客 / 奶妈式产品比喻）和中英混排技术词的放行边界。
