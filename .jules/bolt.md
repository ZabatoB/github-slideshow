## 2024-05-23 - Reveal.js Optimization
**Learning:** Jekyll sites using Reveal.js often include unnecessary client-side Markdown parsers (`marked.js`, `markdown.js`) even when using server-side rendering (kramdown). Removing them saves significant bandwidth and parsing time.
**Action:** Always check `dependencies` in `Reveal.initialize` for unused plugins when optimizing Reveal.js sites. Verify `data-markdown` usage before removing.
