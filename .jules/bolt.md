## 2024-05-22 - Jekyll & Reveal.js Architecture
**Learning:** Jekyll sites using Reveal.js often include client-side Markdown parsers (`marked.js`, `markdown.js`) by default in their templates, even when Jekyll handles all Markdown rendering server-side (via Kramdown). This results in unnecessary payload and parsing overhead.
**Action:** Always check `_config.yml` for markdown settings and inspect `_includes` for redundant client-side parsers in Jekyll/Reveal.js projects.
