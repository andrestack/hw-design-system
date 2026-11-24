# Funnel pages: build brief

What to build on hinterlandweb.com, in launch order, with a reference page for each. Study the references for structure only. Don't copy their copy or design: every page follows `design-system/README.md` (voice in first person "I", Australian spelling, dark navy theme, one teal action per view, one gold-marked phrase per headline).

Stack: Astro on Cloudflare, Polar checkout (digital), Stripe Payment Links (done-for-you deposits), Turnstile on every form.

## 1. Free site audit (`/audit`)

**Job:** capture a URL and an email. Show the cost of staying put. Send SMBs to done-for-you and DIYers to the guide.

**Reference:** [BrowserCat migrate](https://www.browsercat.com/migrate). What to take from it:
- a "paste your URL" hero
- free analysis, pay only to migrate
- a 5-year cost chart against Wix and Squarespace
- prices tiered by page count

**Sections:**
1. Hero: "Is your website costing you more than it should?" URL field + button.
2. Result panel: platform detected, PageSpeed mobile score, page count from the sitemap, plugin/CMS exposure, estimated yearly running cost vs Astro on Cloudflare.
3. Two doors: "Do it yourself (US$9 guide)" and "I'll move it for you (from A$1,490)".
4. Email gate for the full PDF report.

**Build notes:** a Cloudflare Worker does the fetch and the PageSpeed API call. Rate-limit by IP, and put Turnstile on the submit button. Never store anything about a site except the URL and the email the visitor gives us.

## 2. The Exit Guide, US$9 (`/exit`)

**Job:** tripwire. One offer, one button. At checkout, offer the Kit as a +US$20 upgrade.

**Reference:** [systeme.io: the tripwire funnel](https://systeme.io/learn/tripwire-funnel/), for the structure: lead magnet, then low-price offer, then bump, then upsell.

**Sections:**
1. Headline naming the pain (renewals, plugin updates, the hack).
2. What's inside: 5 bullets.
3. "Will this work for my site?" check: green (brochure, blog), amber (bookings, forms), red (members, LMS).
4. Price + button.
5. Short FAQ: do I need to code, do I need Claude, refunds (14 days).

## 3. Thank-you + one-time offer (`/exit/thanks`)

**Job:** offer Exit Kit Pro at a launch price straight after purchase. Polar's checkout success URL points here.

## 4. Kit / Pro sales page (`/exit-kit`)

**Reference:** [Gradually.ai migration skill](https://www.gradually.ai/en/wordpress-migration-skill/). What to take from it:
- step-by-step "how the migration works"
- a green/yellow/red compatibility check
- author bio with a P.S.
- three pricing cards
- a 12-question FAQ
- Polar checkout

**Sections:**
1. Hero.
2. Before/after numbers from a real migration.
3. How it works.
4. Compatibility check.
5. What's in the repo.
6. About André.
7. Pricing cards (Guide / Kit / Pro).
8. FAQ.
9. Closing button.

## 5. Done-for-you (`/move-my-site`), AUD

**References:**
- [Sitewright](https://sitewright.pages.dev/services/migrate/): "from" price, page range and timeline up front; SEO fears answered first.
- [Hapy](https://hapy.co/migrate-to-astro/): four steps, "send your link → know the price → we rebuild → launch".

**Sections:**
1. Hero with a "from A$1,490" price.
2. Three packages.
3. What you keep: domain, Cloudflare, GitHub.
4. Care plans.
5. Local proof: Sunshine Coast and pool businesses.
6. Enquiry form with the URL pre-filled from the audit.

**Must say:** rankings kept through 301 redirects, email keeps working, you own everything. That's what separates us from US$49 automated migrations.

## 6. "WordPress site hacked?" (`/wordpress-hacked`)

**Job:** landing page for Google Search ads.

**Sections:**
1. One urgent promise.
2. The rescue price.
3. Phone number.
4. Audit button.
5. Three steps.

Keep it short; fast load is itself the proof.

## 7. Masterclass (`/masterclass`)

**Job:** US$197 + membership.

**Proof:** real screens from Swimart / PoolTrackr / Duty Manager workflows (names in examples made up).

## Tracking

- Cloudflare Web Analytics on every page.
- Meta Pixel + Conversions API on the guide, the thank-you page and the Kit page (needed for Meta's purchase optimisation).
- A GA4 conversion on the done-for-you enquiry and on the audit submit.
