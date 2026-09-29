# AI Slop Collector

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/justinatusa/ai-slop-collector?style=social)](https://github.com/justinatusa/ai-slop-collector/stargazers)
[![Last commit](https://img.shields.io/github/last-commit/justinatusa/ai-slop-collector)](https://github.com/justinatusa/ai-slop-collector/commits/main)

收集「AI 味」写作痕迹的原文样本与可复用模式——给审稿、去味、对照用。  
*A verbatim collector of AI-writing tells (Chinese-first).*

## 这是什么

大模型写出来的中文和英文，常有一套听得见的套话、口癖和假专业结构（不是…而是…、load-bearing、落盘/兜底、破折号表演……）。本仓把**网上已经公开写过的观察、词表、技能说明**平铺存下来，方便人翻、也方便以后做规则或评测。

不是检测器，也不声称「这段一定是 AI 写的」。只记可核对的坏味道与出处。

## 里面有什么

| 路径 | 内容 |
|------|------|
| [`patterns/`](patterns/) | 可复用模式（词、句式）；跨来源合并见 [`patterns/DEDUPED.md`](patterns/DEDUPED.md) |
| [`sources/scrapes/`](sources/scrapes/) | 外部原文 verbatim 平铺（一文一文件） |
| [`sources/INDEX.md`](sources/INDEX.md) | **导航**：按来源日新→旧 |
| [`sources/archive-pre-2026-05/`](sources/archive-pre-2026-05/) | 早于过滤线的材料 |
| [`examples/`](examples/) | 整段坏样本 |

覆盖重点包括：Claudeish / Claudish / Opus tells、ChatGPT / GPT-5.x·Codex 中文口癖、中文去 AI 味 skill、社区帖（X、LINUX DO 等）。

## 怎么贡献一条 scrape

1. 新建 `sources/scrapes/YYYY-MM-DD-<slug>.md`（日期用**来源日**）。
2. frontmatter 写清 `source_url`、`source_date`、`captured`、`models`。
3. 正文**照抄**（可节选），不改写。
4. 同一 URL 不重复建文件。
5. 主表只收 `source_date` **≥ 2026-05-01**（已知例外：linux.do 2026-03-16 gpt-5.x 口癖帖）。
6. 更新 [`sources/INDEX.md`](sources/INDEX.md)。

更细的约定见 [`CONTRIBUTING.md`](CONTRIBUTING.md)。

## 从哪看起

→ **[`sources/INDEX.md`](sources/INDEX.md)**（全部 scrape 导航）  
→ **[`patterns/DEDUPED.md`](patterns/DEDUPED.md)**（跨 scrape 高频词/句式）

## 许可

[MIT](LICENSE)。外部原文版权归原作者；此处仅作研究摘录。
