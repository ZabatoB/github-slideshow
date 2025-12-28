# Bolt's Journal

## 2024-05-22 - Initial Setup
**Learning:** This journal tracks critical performance learnings to avoid repeating mistakes.
**Action:** Always check this file before starting optimization tasks.

## 2025-12-28 - Unnecessary Client-Side Parsing
**Learning:** Jekyll sites using Reveal.js often render markdown server-side (kramdown), making the default client-side `marked.js` and `markdown.js` plugins redundant and wasteful.
**Action:** Always verify if `data-markdown` is used before assuming client-side parsers are needed; otherwise remove them to save bandwidth.
