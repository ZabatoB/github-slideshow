## 2026-02-06 - Redundant Client-Side Parsers in SSG
**Learning:** In Jekyll sites using Reveal.js, client-side Markdown parsers (`marked.js`) are often redundant because Jekyll renders Markdown to HTML server-side.
**Action:** Always check if SSG renders content before loading client-side parsers. Verify by grepping for `data-markdown`.
