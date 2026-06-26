# SEO Implementation Plan - Message Risk Audit

Date: 2026-06-26

## Core Line

The site should not sound like an abstract AI detector. The red line is:

> Check the message through human filters before replying, sending documents, paying money, opening links, or sharing access.

The five recurring filters:

1. Who is writing?
2. What exactly is promised?
3. What are they asking for before trust is established?
4. Where is the pressure, urgency, secrecy, or emotional push?
5. What safe next question or reply slows the situation down?

## Sprint 1 - Implemented Locally

Pages:

1. `/ru/proverit-vakansiyu-na-moshennichestvo/`
   - Intent: `проверить вакансию на мошенничество`, `как понять что вакансия развод`, `фейковая вакансия`.
   - Angle: remote job or employer message before money, documents, links, or contract.

2. `/ru/rabota-v-telegram-moshenniki/`
   - Intent: `работа в телеграм мошенники`, `мошенники в телеграм работа`, `удаленная работа мошенники`.
   - Angle: Telegram job messages, tasks, likes, crypto deposits, bots/channels, quick payouts.

3. `/job-offer-scam-check/`
   - Intent: `job offer scam`, `are recruiter texts a scam`, `remote job scam text message`, `fake recruiter text`.
   - Angle: recruiter text or remote job offer before replying, sending ID, paying fees, or opening links.

Homepage changes:

- Added "Popular checks" / "Популярные проверки" blocks.
- Linked the first three intent pages from both RU and EN homepages.
- Kept `Message Risk Audit` as the brand, while the visible SEO language uses user anxiety.

Technical changes:

- Added canonical URLs.
- Added language alternates for the RU vacancy and EN job offer pair.
- Added BreadcrumbList and FAQPage JSON-LD on intent pages.
- Updated `sitemap.xml` with all new pages and `lastmod` `2026-06-26`.
- Updated README and the local zip artifact.

## Deployment Step

After approval:

1. Deploy the static folder to Vercel production.
2. Verify live HTTP 200 for:
   - `/`
   - `/en/`
   - `/ru/proverit-vakansiyu-na-moshennichestvo/`
   - `/ru/rabota-v-telegram-moshenniki/`
   - `/job-offer-scam-check/`
   - `/sitemap.xml`
3. Check live HTML for:
   - canonical tags
   - sitemap inclusion
   - JSON-LD validity
   - links to Tally forms
4. Submit the three new URLs in Google Search Console URL Inspection.

## First 7-14 Days After Deployment

Daily:

- Request indexing once for each new page if Google has not crawled it.
- Check URL Inspection status, not only the general Pages report.

Weekly:

- In GSC Performance, filter by each new page.
- Categorize queries into:
  - vacancy/job scam
  - Telegram work scam
  - recruiter text/job offer
  - documents/passport
  - generic message checker
  - irrelevant/noise

Decisions:

- Impressions = 0: strengthen internal links and add YouTube links to the exact matching page.
- Impressions with average position 30-90: expand examples and FAQ.
- Average position under 20 but CTR weak: rewrite title and meta description.
- Repeated new query cluster: create the next page around that intent.

## Sprint 2 Candidates

Build only after the first pages receive crawl/query signals:

1. `/ru/rabotodatel-prosit-pasport-ili-dokumenty/`
2. `/scam-text-checker/`
3. `/telegram-scam-message-check/`

These should reuse the same human-filter structure, not become thin SEO articles.

## YouTube Linking

Future video descriptions should link to the matching page, not always the homepage:

- Vacancy/job scam video -> `/ru/proverit-vakansiyu-na-moshennichestvo/`
- Telegram job scam video -> `/ru/rabota-v-telegram-moshenniki/`
- English job offer text video -> `/job-offer-scam-check/`

Use UTM links:

`?utm_source=youtube&utm_medium=video&utm_campaign=message_risk&utm_content=job_offer_scam`
