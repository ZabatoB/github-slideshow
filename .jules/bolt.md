## 2025-12-31 - [Jekyll/Reveal.js Duplicate Assets]
**Learning:** Checking for duplicate asset loading in template partials (like head.html) and removing unused client-side parsers (like marked.js) when server-side rendering is used are high-impact, low-risk optimizations.
**Action:** Always inspect included partials for redundant resource loading and verify if client-side libraries are actually needed given the build process.
