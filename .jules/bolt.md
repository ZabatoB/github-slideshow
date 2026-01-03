## 2024-05-23 - Duplicate CSS Loading
**Learning:** Legacy projects often accumulate duplicate asset references in shared includes (like `head.html`), where they are harder to spot than in component-based architectures.
**Action:** Audit all `_includes` files for redundant `<link>` and `<script>` tags, especially when `node_modules` paths are manually referenced.

## 2024-05-23 - Redundant Client-Side Parsers
**Learning:** Static site generators (like Jekyll) that pre-render content (Markdown to HTML) eliminate the need for client-side parsers (like `marked.js`), but template boilerplate often retains them by default.
**Action:** Always verify if client-side dependencies overlap with server-side build steps and remove the client-side counterparts if they are unused.
