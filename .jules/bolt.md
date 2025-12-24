## 2024-05-23 - Static Site Markdown Parsing
**Learning:** In static site generators like Jekyll, content is rendered to HTML at build time. Including client-side markdown parsers (like marked.js) in the output is often a redundant performance cost.
**Action:** Always check if client-side libraries are actually doing work that the build step has already completed. Remove them if redundant.
