## 2024-05-23 - [Jekyll vs Client-side Markdown]
**Learning:** In Jekyll + Reveal.js projects, Reveal's client-side Markdown plugins (`marked.js`, `markdown.js`) are often redundant because Jekyll compiles Markdown to HTML at build time.
**Action:** Always check if `data-markdown` attributes are used before assuming Reveal.js Markdown plugins are needed. Removing them saves significant payload.
