## 2026-02-04 - [Jekyll + Reveal.js Redundancy]
**Learning:** Static site generators like Jekyll render Markdown server-side, making client-side parsers like marked.js redundant unless using data-markdown dynamic loading.
**Action:** Audit static site configs for unused client-side libraries that duplicate server-side functionality.
