## 2026-01-26 - Static Site Generator vs Client-Side Rendering
**Learning:** In a Jekyll-based Reveal.js site, `marked.js` and `markdown.js` were included for client-side rendering, but Jekyll processes Markdown at build time. This resulted in ~40KB of dead code.
**Action:** When working with SSGs (Jekyll, Hugo, etc.) + JS frameworks, always verify if client-side parsers are redundant.
