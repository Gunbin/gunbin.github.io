---
title: "Markmap Test"
date: 2026-04-26
description: "Validation page for Markmap rendering and readability."
keywords: ["markmap", "mindmap", "test"]
disableComments: true
---

# Markmap test

This block renders a mindmap directly from markdown headings.  
If rendering fails, you will only see raw code.

```markmap
# TrendRadar Improvement Plan v1.0
## P0 Immediate
### 1-1 Top-heavy internal links
- Link only in top 50%
- Allow partial keyword matching
- Limit one link per URL
### 1-2 Visual layer expansion
- Flexible Mermaid insertion
- Flexible Markmap insertion
- Hugo shortcode callouts
## P1 Near-term
### 3-1 Manual freshness button
- Pick one old post
- Pull latest headline
- Append one-line summary
## On hold
### 2-2 Topical silo writing
### 3-2 Drip-feeding scheduler
### 3-3 Telegram outreach bot
```

## Validation checklist

- Tree hierarchy renders correctly
- Longer labels stay readable
- Contrast remains clear in light/dark mode
