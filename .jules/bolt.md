## 2024-10-24 - [Unnecessary Client-Side Parsing]
**Learning:** This Jekyll-based Reveal.js architecture renders slides server-side, making client-side Markdown parsers (`marked.js`, `markdown.js`) redundant and performance-draining.
**Action:** Always verify if static site generators are already handling content rendering before keeping client-side transformation libraries.
