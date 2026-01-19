## 2024-05-23 - [Static Site Performance]
**Learning:** In static sites (Jekyll), client-side markdown parsers like `marked.js` are redundant if content is pre-rendered. Removing them saves significant bandwidth and parsing time without functional loss.
**Action:** Always check if client-side libraries duplicate server-side/build-time functionality.
