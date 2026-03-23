# Post Template

Use this when creating a new post in `_posts/`.

---

## Front Matter (required)

```yaml
---
title: "Your Title Here"
date: YYYY-MM-DD
categories: [笔记]   # 笔记 | 随想
tags: []             # optional, e.g. [CSE, 算法]
---
```

---

## How to Add a New Post

1. **Filename**: `YYYY-MM-DD-slug.md` inside `_posts/`
2. **Decide category**:
   - `笔记` — course notes, tech posts; source from Obsidian
   - `随想` — personal thoughts, opinions; write directly
3. **Fill front matter** (title, date, categories required)
4. **Write body** in Markdown below the `---`
5. **Add images**: save to `assets/`, reference as `/assets/filename.png`
6. **Done** — push to `main` and it's live

---

## Quick Reference

| Item | Where |
|------|-------|
| Post file | `_posts/YYYY-MM-DD-title.md` |
| Images | `assets/` |
| PDFs | `_posts/` (not gitignored here) |
| Categories | `笔记` (notes) or `随想` (thoughts) |
