## 2024-05-23 - [Static Site Client-Side Parsers]
**Learning:** Even in static sites (Jekyll), boilerplate configurations often include unused client-side parsers (like marked.js for Reveal.js). Removing these can significantly reduce bundle size (44KB in this case) without affecting functionality when content is pre-rendered.
**Action:** Always verify if 'convenience' plugins in UI libraries are actually used by the application logic or if the work is already done at build time.
