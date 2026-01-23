## 2024-05-22 - Frontend Verification in CI-only Environments
**Learning:** In environments lacking build tools (e.g., missing `jekyll`), standard frontend verification (Playwright, visual inspection) is impossible for static site generators that rely on build-time templating (Liquid).
**Action:** When working in such environments, rely on code analysis, static verification of file contents, and unit tests if available. Document the limitation clearly.
