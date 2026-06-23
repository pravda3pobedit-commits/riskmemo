# Message Risk Audit MVP

Static landing page for a manual suspicious-message review service.

## What This Is

- One static Russian landing page plus an English version under `/en/`.
- Designed for Vercel static hosting.
- No backend, no accounts, no payments yet.
- Intake is manual at first: Tally is the primary form. Do not show a public email on the page.

## Files

- `index.html` - landing page.
- `en/index.html` - English landing page.
- `styles.css` - page styling.
- `assets/hero-analysis.svg` and `assets/hero-analysis-en.svg` - visual previews of a risk memo.
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

Current RU public form URL: `https://tally.so/r/eqobyx`.
Current EN public form URL: `https://tally.so/r/lbg18v`.

## English Page

The English page lives at `/en/`. The root and English pages link to each other
with visible RU/EN links, canonical URLs, and `hreflang` alternates. `sitemap.xml`
also includes both URLs.

## Vercel

Deploy as a static project from this folder. No build command is needed.
