## 2026-01-29 - Redundant Client-Side Parsers in Server-Side Rendering
**Learning:** When using Jekyll to generate Reveal.js slides, Markdown is rendered server-side by Jekyll (Kramdown). Including client-side parsers like `marked.js` and `markdown.js` is redundant payload (approx 30KB+ gzipped).
**Action:** Always check if the static site generator handles content rendering before including client-side libraries. Remove `marked.js` and `markdown.js` from `dependencies` in Reveal.js config if server-side rendering is used.
