## 2025-01-27 - Unnecessary Client-Side Markdown
**Learning:** This Jekyll-based Reveal.js setup renders Markdown server-side (Kramdown). The default Reveal.js client-side Markdown plugins (`marked.js`, `markdown.js`) are included in `script.html` but are completely redundant, wasting bandwidth and main thread time.
**Action:** Always verify if a static site generator's server-side rendering makes client-side libraries redundant.
