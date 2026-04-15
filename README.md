# re1gn Jekyll site explained

A simple Jekyll blog starter for GitHub Pages.

## Run locally

```bash
bundle init
bundle add jekyll webrick
bundle exec jekyll serve
```

Then open the local URL Jekyll gives you.

## Create a new post

Add a file in `_posts/` with this format:

```text
YYYY-MM-DD-title.md
```

Example front matter:

```markdown
---
layout: post
title: "My New Post"
date: 2026-04-15 18:00:00 -0500
---

Write here in Markdown.
```

## Deploy to GitHub Pages

If you're using GitHub Pages with Jekyll support, push the files to your repo root or just make a file in the "Pages" folder.
