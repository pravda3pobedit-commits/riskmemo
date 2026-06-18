# Message Risk Audit MVP

Static landing page for a manual suspicious-message review service.

## What This Is

- One static Russian landing page.
- English page can be added later under `/en/`.
- Designed for Vercel static hosting.
- No backend, no accounts, no payments yet.
- Intake is manual at first: Tally is the primary form. Do not show a public email on the page.

## Files

- `index.html` - landing page.
- `styles.css` - page styling.
- `assets/hero-analysis.svg` - visual preview of a risk memo.
- `robots.txt` and `sitemap.xml` - starter SEO files.
- `TRAFFIC_PLAN.md` - first traffic strategy.
- `KEYWORD_RESEARCH.md` - initial keyword clusters.
- `TALLY_FORM_SPEC.md` - exact fields for the first Tally intake form.
- `FUTURE_SCOPE.md` - serious future directions intentionally excluded from the MVP page.
- `vercel.json` - static hosting config.

## Before Publishing

1. Replace `https://message-risk-audit.vercel.app` in `sitemap.xml` and `index.html` if the deployed URL differs.
2. Add the deployed URL to Google Search Console and Yandex Webmaster.
3. Optional later: add Telegram CTA.

## Tally

Current public form URL: `https://tally.so/r/eqobyx`.

## Future English Page

When ready, add `en/index.html` and update:

- root page with an English language link.
- `sitemap.xml` with `/en/`.
- `hreflang` tags on both pages.
- `KEYWORD_RESEARCH.md` with live GSC/English-query findings.

## Vercel

Deploy as a static project from this folder. No build command is needed.
Deploy trigger: 2026-06-18
