## 2024-05-23 - [Remove Redundant Client-Side Markdown Parsing]
**Learning:** The architecture uses Jekyll's server-side rendering (Kramdown) for slide content, injected via '{{ post.content }}'. Client-side Markdown parsers ('marked.js', 'markdown.js') in Reveal.js dependencies are redundant unless 'data-markdown' is used, which it isn't in this project.
**Action:** Always verify if a static site generator is already handling content processing before keeping default client-side libraries.
