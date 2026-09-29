# AI Slop Collector

专门收集「AI 味」样本与可复用反例，给以后去 AI 味、审稿、反向喂模型用。

## 本仓怎么组织

- **平铺 verbatim**：外部来源一文一文件，正文照抄，不二次改写。
- **按来源时间新 → 旧**：见 [sources/INDEX.md](sources/INDEX.md)；抓取日另记在 frontmatter `captured`。
- **优先新模型材料**：大规模 Opus 系列、GPT-5.6 Sol / gpt-5.x / Codex、有 Grok 的条目优先保留与置顶；`source_date` 早于 **2026-05-01** 的老泛用词表移出主表（见 `sources/archive-pre-2026-05/`）。

现在只做积累，不急着做成完整工具。

## 怎么用

1. 看到一段典型 AI 套话 / 空洞结构 / 假专业词，丢进 `patterns/` 或 `examples/`。
2. 每条尽量写清：原文摘录、为什么算 slop、改成什么更好（可空）、出处（可空）。
3. 外部长文 / 词表：写入 `sources/scrapes/`，frontmatter 必含 `source_url`、`source_date`、`models`、`captured`，并更新 INDEX。

## 目录

| 路径 | 用途 |
|------|------|
| `patterns/` | 可复用模式（词、句式、结构）；跨 scrape 合并见 [`patterns/DEDUPED.md`](patterns/DEDUPED.md) |
| `examples/` | 整段或整篇坏样本（可脱敏） |
| `sources/scrapes/` | 外部原文 verbatim 平铺 |
| `sources/INDEX.md` | 来源日新→旧导航表 |
| `sources/archive-pre-2026-05/` | 已剔除的早期材料 |

## 命名

- 模式文件：`kebab-case.md`
- scrape 文件：优先 `YYYY-MM-DD-<slug>.md`（来源日；未知则用抓取日）

## 种子条目

- [钉子域 / 假钉子隐喻](patterns/nail-domain-metaphor.md)
- [中文禁用空词（初稿）](patterns/zh-banned-empty-words.md)
- [「不是…而是…」](patterns/not-x-but-y.md)

## 原则

- 只记可验证的坏味道，不猜「是不是 AI 写的」。
- 保留作者真实声音；这里收集的是该删的模式，不是「把人写的也磨平」。
- 不确定就标 `status: draft`，以后再收紧。
