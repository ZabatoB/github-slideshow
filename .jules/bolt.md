## 2024-12-27 - [Duplicate Asset Loading]
**Learning:** Browser caching does not eliminate the parsing cost of duplicate CSS files. Loading `reveal.css` twice not only wastes a network request (if not cached) but forces the browser to re-parse the styles, potentially triggering unnecessary style recalculations. Additionally, ordering is critical: `reset.css` must strictly precede framework styles to function correctly.
**Action:** Always audit `head.html` or equivalent template partials for duplicate `<link>` tags and verify cascading order (`reset` -> `base` -> `theme`).

## 2024-12-27 - [Server-Side vs Client-Side Rendering]
**Learning:** In a Jekyll + Reveal.js setup, including `marked.js` and `markdown.js` is often a redundant default pattern. Since Jekyll (via kramdown) pre-renders Markdown into HTML at build time, these client-side parsers add significant bloat (~44KB) without adding value, unless `data-markdown` is explicitly used for dynamic slides.
**Action:** Remove client-side Markdown parsers in Static Site Generator environments unless there is a specific requirement for runtime Markdown rendering (e.g., fetching external `.md` files).
