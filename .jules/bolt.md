# Bolt's Journal

## 2024-05-22 - Jekyll & Reveal.js Optimization
**Learning:** In Jekyll-based reveal.js sites, content is often pre-rendered to HTML by Jekyll (using kramdown/rouge). This renders client-side Markdown parsers (marked.js) and potentially highlighters redundant, unless specifically using `data-markdown` attributes.
**Action:** Always check `_config.yml` and source templates before assuming client-side libraries are needed. Checking for `data-markdown` usage confirmed we can remove `marked.js` and `markdown.js`.
