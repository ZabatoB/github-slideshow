## 2025-05-23 - Unused Client-Side Markdown Parsing
**Learning:** This Jekyll/Reveal.js setup renders everything server-side. Including `marked.js` and `markdown.js` in the client bundle is dead code (~44KB) because there are no `data-markdown` attributes used.
**Action:** When working with static site generators, check for unused client-side libraries that might be leftovers from default templates or examples.
