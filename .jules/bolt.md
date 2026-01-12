## 2024-05-23 - Unnecessary Client-Side Parsing in Static Sites
**Learning:** In a Jekyll + Reveal.js setup, Markdown is often pre-rendered by Jekyll. Including client-side parsers like `marked.js` is redundant and bloats the bundle.
**Action:** Verify if `data-markdown` is actually used. If not, remove `marked.js` and `markdown.js` dependencies.
