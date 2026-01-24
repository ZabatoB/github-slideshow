## 2026-01-24 - Unnecessary Client-Side Markdown Parsing
**Learning:** The project uses Jekyll to render Markdown to HTML server-side, but also included `marked.js` and `markdown.js` (Reveal.js plugins) for client-side parsing. This resulted in unused JavaScript being downloaded and parsed.
**Action:** When working with Static Site Generators (SSG) + Reveal.js, verify if content is pre-rendered. If so, remove client-side Markdown parsers to save bandwidth and processing time.
