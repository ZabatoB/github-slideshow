## 2024-05-23 - [Jekyll & Reveal.js Redundancy]
**Learning:** In a Jekyll + Reveal.js setup, if `kramdown` (server-side) is used for Markdown rendering, the client-side `marked.js` and `markdown.js` plugins are redundant unless `data-markdown` attributes are used dynamically.
**Action:** Always check `_config.yml` for `markdown: kramdown` and grep for `data-markdown` usage before removing client-side parsers.
