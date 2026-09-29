# 贡献指南

感谢你愿意补一条「AI 味」样本。本仓只做 verbatim 积累，不猜「是不是 AI 写的」。

## 加一条 scrape

1. 在 `sources/scrapes/` 新建 `YYYY-MM-DD-<slug>.md`（日期用**来源日**，不是抓取日）。
2. frontmatter 至少包含：

```yaml
---
title: 简短标题
source_url: https://...
source_date: YYYY-MM-DD
captured: YYYY-MM-DD
lang: zh   # 或 en / mixed / zh-Hant
models: [claude, opus]   # 或 gpt / grok / zh-slop / unattributed 等
---
```

3. 正文**平铺照抄**原文关键段落（可节选，标明节选）；不要二次改写、不要「润色」。
4. 同一 `source_url` **不要**再建第二个文件。
5. 更新 [`sources/INDEX.md`](sources/INDEX.md)：按 `source_date` **新 → 旧**插入一行。
6. 若词句表有新增，可顺手更新根目录 [`SLOP.md`](SLOP.md)。

## 加一条 pattern / example

- `patterns/`：可复用的词、句式、结构（kebab-case 文件名）。
- `examples/`：整段坏样本（可脱敏），写清为什么算 slop、更好的写法（可空）。

## PR 建议

- 一次 PR 聚焦一类来源或一个模型家族更好 review。
- 说明原链、来源日、为什么值得收。
- 不要提交假数据、编造引用或未授权私聊全文。

## 许可

贡献内容默认按本仓 [MIT License](LICENSE) 授权。外部原文的版权仍属原作者；本仓仅作研究/对照摘录。
