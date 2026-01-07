## 2024-05-23 - [Static Site Client-Side Parsers]
**Learning:** Even in static sites (Jekyll), client-side parsers like `marked.js` might be included by default in templates/libraries (Reveal.js), adding unnecessary weight (44KB in this case) when content is already pre-rendered server-side.
**Action:** Always verify if client-side libraries in static site templates are actually needed or if the build step already handles the functionality.
