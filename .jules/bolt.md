## 2024-05-23 - Missing package.json and Redundant Assets
**Learning:** The repo contains `package-lock.json` and `node_modules` but lacks `package.json`, which prevents running npm scripts directly. Additionally, the project uses Jekyll for server-side Markdown rendering but still loads `marked.js` and `markdown.js` (client-side parsers) in the Reveal.js initialization, which is redundant.
**Action:** Always check for `package.json` even if `package-lock.json` exists. Remove redundant client-side parsers when server-side rendering is used.
