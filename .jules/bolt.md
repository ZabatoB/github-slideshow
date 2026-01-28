## 2025-05-22 - [Redundant Markdown Processing]
**Learning:** This Jekyll-based Reveal.js setup renders Markdown server-side (via Kramdown). Including Reveal.js's client-side Markdown plugins (`marked.js`, `markdown.js`) is redundant and adds unnecessary weight (~38KB) and execution time.
**Action:** Always check if static site generators are already handling content processing before keeping client-side libraries that do the same thing.
