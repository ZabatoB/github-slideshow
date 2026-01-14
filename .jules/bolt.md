## 2024-05-22 - [Removing Unused Client-Side Libraries in Static Sites]
**Learning:** In Jekyll-based Reveal.js sites, markdown is often rendered server-side (kramdown). Including client-side markdown parsers (`marked.js`, `markdown.js`) is redundant and adds unnecessary network overhead.
**Action:** Always verify if markdown is rendered server-side or client-side before including parsing libraries.
