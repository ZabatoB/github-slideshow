## 2024-10-24 - [Jekyll & Reveal.js Architecture]
**Learning:** This Jekyll site uses server-side Markdown rendering (via Kramdown), so Reveal.js client-side Markdown plugins (`marked.js`, `markdown.js`) are unnecessary overhead.
**Action:** Always check if the static site generator handles content rendering before including client-side parsers.
