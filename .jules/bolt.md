## 2025-01-22 - Unnecessary Client-Side Markdown Parsing
**Learning:** Jekyll sites using Reveal.js often include `marked.js` and `markdown.js` by default for client-side rendering. However, since Jekyll pre-renders content to HTML, these libraries are often redundant payload, adding ~40KB of unnecessary JS.
**Action:** Always check `script.html` or Reveal.js initialization in Jekyll/Reveal.js projects for unused `markdown` dependencies and remove them to save bandwidth and parse time.
