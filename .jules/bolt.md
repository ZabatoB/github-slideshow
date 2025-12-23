## 2024-05-23 - [Static Site Asset Redundancy]
**Learning:** Jekyll sites often include client-side parsers (like `marked.js`) in templates copied from dynamic examples, even when content is fully rendered server-side.
**Action:** Always check `_config.yml` for server-side renderers (like `kramdown`) and remove corresponding client-side JS libraries to reduce payload.
