## 2024-05-23 - Reveal.js Client-Side Redundancy
**Learning:** In a server-side rendered Jekyll site, Reveal.js markdown plugins (`marked.js`, `markdown.js`) are unnecessary bloat because the content is already HTML.
**Action:** Always check `_config.yml` (e.g., `markdown: kramdown`) to confirm SSR before removing client-side parsers.
