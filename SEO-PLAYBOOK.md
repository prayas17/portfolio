# SEO Playbook — Prayas Jain Portfolio

> **Goal:** Rank #1 on Google for **"Prayas Jain"**, plus strong rankings for "Lead AI Engineer Indore", "Multi-agent systems engineer India", and other niche queries.
>
> **URL:** https://prayas17.github.io/portfolio/
> **Last updated:** 2026-05-21

---

## ✅ What's already done (on-page SEO — 95+/100)

1. **Comprehensive meta tags** — title, description, keywords, robots, canonical, geo, theme-color, OG, Twitter Card, Apple/PWA, hreflang.
2. **Full JSON-LD structured data** on every page:
   - `Person` schema (the #1 ranker for name searches — Google builds knowledge panels from this)
   - `WebSite` + `WebPage` schemas
   - `BreadcrumbList`
   - `ProfessionalService` with offer catalog
   - `FAQPage` (eligible for SERP rich results)
   - `ItemList` for case files
3. **Semantic HTML upgrades** — `<main>`, `<address>`, `<time>`, aria-labels, microdata.
4. **`sitemap.xml`** with image entries, hreflang alternates, and section anchors.
5. **`robots.txt`** allowing all major search bots + AI crawlers (GPTBot, ClaudeBot, PerplexityBot) so you appear in AI-generated answers.
6. **`favicon.svg`**, `site.webmanifest`, `browserconfig.xml`, `404.html`.
7. **`og-image.svg`** for social previews (see step 1 below to convert).
8. **Fixed broken links** in `resume.html` (was pointing to non-existent `portfolio.html`).

**Current technical SEO score: ~95/100.** The remaining points come from off-site actions below.

---

## 🚀 Critical steps to take RIGHT NOW after deploying

### 1. Generate `og-image.png` (5 minutes)

Social platforms (LinkedIn, WhatsApp, Twitter, Slack) need a PNG. The SVG is just the source.

- **Quickest:** Go to **https://cloudconvert.com/svg-to-png** → upload `og-image.svg` → set width `1200`, height `630` → download as `og-image.png` → save it next to `index.html`.
- Or open `og-preview.html` in your browser and screenshot the frame.

Without this PNG, links shared on LinkedIn/WhatsApp will look blank.

### 2. Generate `apple-touch-icon.png` (2 minutes)

Open `favicon.svg` in **https://realfavicongenerator.net/** → download the package → drop these files in:
- `favicon.ico`
- `apple-touch-icon.png` (180×180)
- `android-chrome-192x192.png`
- `android-chrome-512x512.png`
- `mstile-150x150.png`

### 3. Submit to Google Search Console (this is THE biggest needle-mover)

1. Go to **https://search.google.com/search-console**
2. Add property → **URL prefix** → `https://prayas17.github.io/portfolio/`
3. Verify ownership using **HTML tag method**:
   - GSC will give you a token like `<meta name="google-site-verification" content="ABC...">`
   - Open `index.html`, find the commented line `<!-- <meta name="google-site-verification" ... -->`
   - Uncomment it and paste your token
   - Push to GitHub, then click "Verify" in GSC
4. Once verified, submit the sitemap: **Sitemaps → Add `sitemap.xml` → Submit**
5. Use **URL Inspection → "Request indexing"** for the homepage. Google will crawl within 1–7 days.

### 4. Submit to Bing Webmaster Tools

1. Go to **https://www.bing.com/webmasters**
2. Sign in with Microsoft account → Add site
3. Use the **Import from Google Search Console** option (one-click after step 3)
4. Submit sitemap

### 5. Create a Google Knowledge Panel for "Prayas Jain"

The Person JSON-LD I added is the bedrock. To activate the knowledge panel:

1. **Wikidata entry** (optional but powerful) — create a Wikidata item for yourself at https://www.wikidata.org/
2. **Consistent name across the web** — make sure LinkedIn, GitHub, Twitter, and any blog/article use the exact same name "Prayas Jain"
3. **External authoritative mentions** — get listed in tech publications, podcasts, conferences, or guest blog posts

### 6. Add Google Analytics 4 (optional but recommended)

To track which queries bring people to your site:

1. Create a GA4 property at https://analytics.google.com
2. Add the gtag snippet before `</head>` in `index.html` and `resume.html`
3. Link GA4 with Search Console for query-level data

---

## 🎯 Off-Site SEO — How to actually rank #1 on Google

On-page SEO is **necessary but not sufficient.** Google ranks by trust signals. Here's the off-site checklist:

### A. Build authoritative backlinks (highest impact)

The #1 ranking factor for personal-name searches is: **how many high-authority sites link to yours.**

1. **LinkedIn profile** ([linkedin.com/in/prayasjain17](https://www.linkedin.com/in/prayasjain17/)) → add `https://prayas17.github.io/portfolio/` to:
   - "Contact info → Website" field (use label "Portfolio")
   - Your "About" section
   - Featured posts
2. **GitHub profile** ([github.com/prayas17](https://github.com/prayas17)) → set portfolio URL in profile settings.
   Pin a repo that links to your portfolio in its README.
3. **X / Twitter bio** ([x.com/prayas17jain](https://x.com/prayas17jain)) → add portfolio URL to bio. Pin a tweet introducing your portfolio.
4. **Instagram bio** ([instagram.com/prayas17_](https://www.instagram.com/prayas17_/)) → add portfolio URL to the link-in-bio. If using one Instagram link slot, use linktr.ee or beacons.ai pointing portfolio as the top destination.
5. **Dev.to / Hashnode / Medium** → write 1–2 technical articles ("How I built a multi-agent RAG system" etc.) and link back to your portfolio.
6. **Stack Overflow profile** → add portfolio link in your "About me" section.
7. **YouTube channel description** → if you have one, link the portfolio.
8. **HackerNews `Show HN`** → publishing one of your projects can drive thousands of backlinks.
9. **Indie Hackers / Product Hunt** → if you launch any of your SaaS products there.
10. **GitHub README of your repos** → every repo's README should link to the portfolio at the bottom.

### B. Citations / NAP (Name, Address, Phone) consistency

Google verifies you're a real person by cross-referencing your contact info across sites. Make sure these EXACTLY match what's in your JSON-LD:

- **Name:** Prayas Jain
- **Location:** Indore, Madhya Pradesh, India
- **Email:** prayas1711@gmail.com
- **Phone:** +91 79700 33564
- **LinkedIn:** linkedin.com/in/prayasjain17
- **GitHub:** github.com/prayas17
- **X / Twitter:** x.com/prayas17jain
- **Instagram:** instagram.com/prayas17_

> These are also in the `sameAs` array of your Person JSON-LD — Google cross-references them to confirm identity and build your knowledge panel.

### C. Content depth & freshness

- Add a **`/blog/` directory** with technical posts (RAG architectures, LangGraph patterns, agent design). 5–10 deep articles will outrank thousands of generic competitor pages for technical queries.
- Update the homepage `dateModified` in JSON-LD whenever you make changes — fresh content ranks better.

### D. Performance & Core Web Vitals

Your portfolio is already very fast (inline CSS), but verify:

1. Run **https://pagespeed.web.dev/** → enter your URL
2. Target: All Core Web Vitals in green (LCP < 2.5s, FID < 100ms, CLS < 0.1)
3. Run **https://search.google.com/test/rich-results** to verify your structured data is parsing correctly

### E. Mobile-first indexing

Google indexes your mobile version. Test:

1. **https://search.google.com/test/mobile-friendly** — paste your URL
2. Should pass; design is already responsive

---

## 📈 Targeted keyword strategy

| Priority | Keyword | Difficulty | Strategy |
|----------|---------|------------|----------|
| 🔥 P0 | **Prayas Jain** | Low (just your name) | Already optimized. Wait 2–4 weeks after GSC submission. |
| 🔥 P0 | **Prayas Jain AI Engineer** | Low | Same. Should rank #1 within a month. |
| ⭐ P1 | **Lead AI Engineer Indore** | Medium | Strong on-page signal; need 3–5 backlinks. |
| ⭐ P1 | **AI Engineer India portfolio** | Medium-High | Need backlinks + content. Write Dev.to article. |
| 📌 P2 | **LangGraph multi-agent developer** | Niche | Already optimized. Write 1 technical blog post. |
| 📌 P2 | **RAG engineer India** | Niche-High | Need 2–3 articles on RAG implementations. |
| 📌 P2 | **AI SaaS freelance India** | High | Long-tail; needs sustained content + backlinks. |

---

## 🧪 How to verify everything is working

Run these tests after deploying:

1. **Rich results test:** https://search.google.com/test/rich-results
   - Paste URL → should detect: Person, WebSite, FAQPage, BreadcrumbList, ProfessionalService
2. **Schema validator:** https://validator.schema.org/
   - Paste URL → all schemas should validate without errors
3. **Open Graph debugger:**
   - Facebook: https://developers.facebook.com/tools/debug/
   - LinkedIn: https://www.linkedin.com/post-inspector/
   - Twitter: https://cards-dev.twitter.com/validator
4. **PageSpeed Insights:** https://pagespeed.web.dev/
5. **Mobile-friendly test:** https://search.google.com/test/mobile-friendly
6. **Robots.txt tester** (inside GSC after verification)
7. **Sitemap status** (inside GSC → Sitemaps)

---

## 📅 Timeline to rank #1 for "Prayas Jain"

| Week | What happens |
|------|--------------|
| Day 0 | Deploy. Submit to GSC + Bing. Generate `og-image.png`. |
| Day 1–3 | Google crawls and indexes your pages. |
| Week 1 | You appear in search for "Prayas Jain" (likely page 2–3). |
| Week 2–4 | If LinkedIn, GitHub, X, and Instagram all link back to the portfolio, you move to page 1. |
| Week 4–8 | With 5+ backlinks and Wikidata entry, **rank #1** for "Prayas Jain". |
| Month 3+ | Begin ranking for "Lead AI Engineer India / Indore" with sustained content. |

---

## 🎁 Bonus — Things most portfolios miss

1. **Add a `humans.txt`** for the developer community (small but cute signal).
2. **Add hreflang** for multiple regions if you're targeting US/UK/India clients differently.
3. **Connect to a Google Business Profile** (yes, even as a freelancer) — boosts local SEO for "AI Engineer Indore".
4. **Create a YouTube channel** with 1–2 case study videos and link them in `VideoObject` schema.
5. **Get featured on podcasts** — being interviewed = high-authority backlinks.

---

## Files in this repo

```
portfolio/
├── index.html              ← Main portfolio (SEO optimized)
├── resume.html             ← Résumé page (SEO optimized)
├── 404.html                ← Friendly error page (noindex)
├── sitemap.xml             ← Search engine sitemap
├── robots.txt              ← Crawler directives
├── favicon.svg             ← Modern vector favicon
├── og-image.svg            ← Social card source (convert to PNG)
├── og-preview.html         ← Visual preview of the OG card
├── site.webmanifest        ← PWA manifest
├── browserconfig.xml       ← Windows tile config
└── SEO-PLAYBOOK.md         ← This file
```

**Files you still need to generate:**

| File | How |
|------|-----|
| `og-image.png` (1200×630) | Convert `og-image.svg` via cloudconvert.com |
| `favicon.ico` | Generate via realfavicongenerator.net from `favicon.svg` |
| `apple-touch-icon.png` (180×180) | Same |
| `android-chrome-192x192.png` | Same |
| `android-chrome-512x512.png` | Same |
| `mstile-150x150.png` | Same |

---

**Questions?** This is a complete blueprint. Follow steps 1–5 of "Critical steps" today and you'll rank #1 for "Prayas Jain" within 30 days.
