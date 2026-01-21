## 2026-01-21 - [Jekyll + Reveal.js Architecture]
**Learning:** This Jekyll site uses server-side Markdown rendering (Kramdown) but was redundantly loading client-side parsers (`marked.js`, `markdown.js`) in `_includes/script.html`.
**Action:** When working with Jekyll-based Reveal.js sites, always verify if `data-markdown` is actually used. If not, client-side parsers are dead weight and should be removed.

## 2026-01-21 - [Verification Constraints]
**Learning:** Verification via Playwright is impossible in this environment due to the lack of Jekyll/Ruby build tools. `file://` access fails because Liquid templates aren't rendered.
**Action:** Rely on static analysis and rigorous logic verification for Liquid/Jekyll templates when build tools are absent.
