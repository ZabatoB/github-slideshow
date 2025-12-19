## 2024-05-23 - [Redundant Client-Side Parsing]
**Learning:** Static site generators (like Jekyll) render Markdown server-side. Including client-side parsers like `marked.js` in the final bundle is redundant and harmful to performance.
**Action:** Always check if content rendering is handled at build time before including client-side parsing libraries. Remove them if unnecessary.
