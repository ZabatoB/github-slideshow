## 2026-02-02 - [Jekyll Reveal.js Optimization]
**Learning:** Jekyll sites utilizing Reveal.js typically perform server-side Markdown rendering (e.g., via kramdown). In such architectures, loading client-side parsers like `marked.js` and `markdown.js` is redundant and negatively impacts performance.
**Action:** Verify `_config.yml` for markdown settings and inspect layout files. If content is pre-rendered, remove client-side markdown dependencies from the Reveal.js initialization configuration.
