# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

---

## Project

A Jekyll blog hosting SJTU-SE course notes & thoughts on **GitHub Pages** (popc0rn.github.io). Theme is `minima`. No local build needed — push to `main` and it's live.

---

## Workflow

**Write → Commit → Push → Done.**

No CI/CD, no staging. `main` is the production branch. GitHub Pages rebuilds automatically on every push.

---

## Structure

| Path | Purpose |
|------|---------|
| `_config.yml` | Jekyll config (title, author, theme) |
| `_posts/` | Blog posts in Markdown |
| `_posts/assets/` | Images and PDFs embedded in posts |
| `obsidian/` | Obsidian vault — independent note-taking workspace, NOT part of the Jekyll build |

---

## Post Conventions

- **Filename**: `YYYY-MM-DD-title.md` (Jekyll requirement)
- **Front matter**: required `title`, `date` at minimum
- **Images**: place in `_posts/assets/`, reference with `/assets/filename.png`
- **PDFs**: committed directly to `_posts/` (`.pdf` is gitignored individually, not from that dir)
- Write in Markdown; embed Obsidian notes here after organizing them

## Content Types

This is a **personal blog**, not just a course notes archive. Two main types:

### 笔记 (Notes)
- Course notes, technical posts, problem solutions
- Source: Obsidian vault → refined → `_posts/`
- Style: structured, clear, educational; can include math/code

### 随想 (Thoughts)
- Personal opinions, reflections, random musings, reviews, opinions
- Source: direct write into `_posts/`
- Style: casual, personal voice, can be short and opinionated

For any new post, decide: **笔记** (from Obsidian, polished) or **随想** (direct, personal). Both belong here equally.

---

## Obsidian → Jekyll Pipeline

This is a two-tool workflow:

1. **Obsidian** — raw note-taking and organizing
2. **Jekyll `_posts/`** — polished notes formatted as blog posts

When a note is ready, extract it from Obsidian, format with Jekyll front matter, and place in `_posts/`.

---

## Key Commands

```bash
# Preview locally (optional, for when you want to check before pushing)
bundle exec jekyll serve

# Just push — that's it
git add . && git commit -m "feat: your change" && git push
```
