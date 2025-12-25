## 2024-05-23 - Reveal.js Client-Side Markdown Redundancy
**Learning:** In Jekyll-based Reveal.js presentations, server-side Markdown rendering (via Kramdown) renders client-side libraries (`marked.js`, `markdown.js`) completely redundant unless `data-markdown` is explicitly used.
**Action:** Always verify if client-side markdown parsing is actually utilized before loading heavy parsing libraries; prefer server-side rendering for static sites.
