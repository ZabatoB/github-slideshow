## 2025-12-17 - [Static Site Asset Redundancy]
**Learning:** Jekyll sites using kramdown render Markdown server-side; client-side parsers like `marked.js` in Reveal.js are redundant payload.
**Action:** Verify if `markdown: kramdown` is set in `_config.yml` and remove client-side markdown dependencies from `Reveal.initialize`.
