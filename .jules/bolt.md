## 2024-01-20 - Unnecessary Client-Side Parsing in Server-Side Apps
**Learning:** In a Jekyll-based Reveal.js setup, the content is rendered to HTML on the server. Including client-side Markdown parsers (`marked.js`, `markdown.js`) is redundant and adds 40KB+ of unnecessary payload.
**Action:** Always check the rendering pipeline. If the server delivers HTML, ensure client-side parsers are removed from the initialization.
