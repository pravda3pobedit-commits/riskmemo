# Message Risk Audit MVP

Static landing page for a manual suspicious-message review service.

## What This Is

- One static Russian landing page plus an English version under `/en/`.
- Three first SEO intent pages:
  - `/ru/proverit-vakansiyu-na-moshennichestvo/`
  - `/ru/rabota-v-telegram-moshenniki/`
  - `/job-offer-scam-check/`
- The Russian landing page embeds the YouTube explainer video `https://www.youtube.com/watch?v=Sr0RIx4Is40`.
- The English landing page embeds the YouTube explainer video `https://www.youtube.com/watch?v=zgaB2GT45Ho`.
- Designed for Vercel static hosting.
- No backend, no accounts, no payments yet.
- Intake is manual at first: Tally is the primary form. Do not show a public email on the page.

## Files

- `index.html` - landing page.
- `en/index.html` - English landing page.
- `ru/proverit-vakansiyu-na-moshennichestvo/index.html` - Russian vacancy scam check page.
- `ru/rabota-v-telegram-moshenniki/index.html` - Russian Telegram job scam check page.
- `job-offer-scam-check/index.html` - English job offer scam check page.
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

## SEO Sprint 1

The first intent pages are built around human-filter review, not automatic AI verdicts.
Each page should keep the same core line: check who is writing, what they promise,
what they ask for, where they apply pressure, and what safe reply can slow the situation down.

## Vercel

Deploy as a static project from this folder. No build command is needed.
