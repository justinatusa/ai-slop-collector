# AI Slop Collector

专门收集「AI 味」样本与可复用反例，给以后去 AI 味、审稿、反向喂模型用。

现在只做积累，不急着做成完整工具。

## 怎么用

1. 看到一段典型 AI 套话 / 空洞结构 / 假专业词，丢进 `patterns/` 或 `examples/`。
2. 每条尽量写清：原文摘录、为什么算 slop、改成什么更好（可空）、出处（可空）。
3. 以后去 AI 味流程可以反向读这个仓，当负面样例库。

## 目录

| 路径 | 用途 |
|------|------|
| `patterns/` | 可复用模式（词、句式、结构） |
| `examples/` | 整段或整篇坏样本（可脱敏） |
| `sources/` | 外部参考链接与笔记 |

## 命名

- 模式文件：`kebab-case.md`，例如 `fake-certainty.md`
- 示例文件：`YYYY-MM-DD-short-note.md`

## 调研索引

- [sources/INDEX.md](sources/INDEX.md) — 带 URL 的 verbatim 摘录导航
- `sources/scrapes/` — 按来源一文一文件

## 种子条目

- [钉子域 / 假钉子隐喻](patterns/nail-domain-metaphor.md) — 你点名的一类
- [中文禁用空词（初稿）](patterns/zh-banned-empty-words.md) — 从既有去 AI 味清单摘出

## 原则

- 只记可验证的坏味道，不猜「是不是 AI 写的」。
- 保留作者真实声音；这里收集的是该删的模式，不是「把人写的也磨平」。
- 不确定就标 `status: draft`，以后再收紧。
