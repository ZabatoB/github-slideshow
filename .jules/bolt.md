## 2024-12-26 - Client-side Markdown in Static Sites
**Learning:** Even in static sites (Jekyll), legacy templates often include client-side parsers (`marked.js`) which are redundant when build-time rendering (`kramdown`) is used.
**Action:** Always check `_config.yml` for markdown settings and remove client-side parsers if server-side rendering is active.
