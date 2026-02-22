# The Commons — Web Design & Monetization Principles
**Date**: February 22, 2026

---

## Platform Recommendation: Ghost (Self-Hosted)

| Option | Fees | Newsletter | Membership | SEO | Ads | Verdict |
|--------|------|-----------|------------|-----|-----|---------|
| **Ghost** | 0% | ✅ Built-in | ✅ Stripe integration | ✅ Excellent | ⚠️ Manual | **Winner** |
| WordPress | 0% | Plugin needed | Plugin needed | ✅ Good | ✅ Best | Too much maintenance |
| Substack | 10% cut | ✅ Built-in | ✅ Built-in | ❌ Poor | ❌ None | Discovery is good but 10% fee kills margins at scale |
| Custom | 0% | Build it | Build it | ✅ Full control | ✅ Full control | Overkill for launch |

**Why Ghost**: Zero platform fees, built-in memberships + newsletters + Stripe payments, blazing fast (great for SEO), beautiful default themes, I can self-host on a $5/mo VPS. It's what The Browser, 404 Media, and dozens of successful indie publishers use.

**Self-hosted cost**: ~$5-12/month (DigitalOcean/Hetzner). Ghost Pro is $25-35/mo if we don't want to manage hosting.

---

## Design Principles (What Actually Converts)

### 1. Newsletter-First, Not Article-First

The #1 conversion metric for a news site isn't page views, it's **email subscribers**. Every design decision should serve this.

**What this means:**
- Homepage hero = newsletter signup, not latest article
- "Get the daily briefing free" above the fold on every page
- Email capture in: header, mid-article, end-of-article, exit-intent popup
- Sticky bottom bar on mobile: "Subscribe free"

**The numbers:**
- Newsletter signup forms in headers convert 2-3x better than sidebar
- Pop-ups after 1-2 article views convert 3-5%
- Mid-article CTAs outperform end-of-article by 40%

### 2. Axios-Style Brevity as the Default

The sites that grow fastest (Axios, Morning Brew, 1440) share one trait: **scannable format**. Not walls of text.

**Article format:**
- **Headline** (sharp, clear, opinionated)
- **One-line summary** (the tweet version)
- **Why it matters** (2-3 sentences)
- **The details** (3-5 bullet points)
- **The bottom line** (one sentence, the take)
- **Go deeper** (link to source)

This format is:
- Perfect for SEO (structured, keyword-rich)
- Perfect for social sharing (headline + summary = tweet)
- Perfect for newsletters (scan in 30 seconds)
- Perfect for AI production (structured = templateable)

### 3. Speed Is Money

Every 100ms of load time costs ~7% in conversions. Political news audiences are especially impatient. Google ranks fast sites higher.

**Targets:**
- LCP (Largest Contentful Paint): < 2.5 seconds
- INP (Interaction to Next Paint): < 200ms
- CLS (Cumulative Layout Shift): < 0.1
- Page weight: < 500KB
- Time to Interactive: < 3 seconds

**How:**
- Ghost is already fast out of the box
- No heavy JavaScript frameworks
- Lazy-load images
- Serve via Cloudflare CDN (free tier)
- Minimal ads initially (they're the #1 speed killer)

### 4. Clean, Professional, Not Flashy

Looking at the competitors:

- **Rebel News**: Cluttered, red/aggressive, video-heavy, banner ads everywhere. Looks like a tabloid. This repels the audience we want.
- **The Hub**: Clean, navy/white, serious. But a bit boring and old-fashioned. Newspaper layout.
- **Daily Wire**: Dark mode, media-heavy, subscription-focused. Professional but very American.
- **Axios**: The gold standard for modern news design. Clean, white, lots of space, scannable.

**The Commons should look like**: Axios meets The Hub. Clean white/navy palette. Lots of whitespace. Strong typography. No clutter. Feels trustworthy and modern, not angry or cluttered.

### 5. Mobile-First (60%+ of Traffic)

- Single-column layout on mobile
- Large tap targets for newsletter signups
- Sticky bottom bar with subscribe CTA
- Fast: no huge images above fold
- Dark mode support (conservative audiences skew older, dark mode is easier on eyes)

---

## Monetization Architecture

### Phase 1: Audience Building (Months 1-6)
**Revenue: $0-500/month**

Revenue isn't the goal. Email list growth is.

- All content free
- No paywall
- Newsletter signup everywhere
- Programmatic ads (Google AdSense): minimal, non-intrusive
  - Expected CPM: $1-5 for political content
  - At 50K pageviews/month: ~$50-250/month
- Goal: 5,000 newsletter subscribers

### Phase 2: Freemium (Months 6-12)
**Revenue: $2,000-8,000/month**

- Launch paid tier: $9/month or $89/year ("Commons Member")
- Free tier: daily news articles + free newsletter
- Paid tier: deep analysis, premium newsletter, early access, no ads
- Free-to-paid ratio: **70% free / 30% paid**
- Metered paywall: 5 free premium articles/month, then paywall
- Conversion target: 2-5% of newsletter subs → paid
  - 5,000 subs × 3% = 150 paid × $9/mo = $1,350/month
  - 10,000 subs × 4% = 400 paid × $9/mo = $3,600/month
  - 20,000 subs × 5% = 1,000 paid × $9/mo = $9,000/month

### Phase 3: Diversified (Year 2+)
**Revenue: $10,000-30,000/month**

- Sponsored content (native ads): $500-2,000 per sponsored post
  - Political CPMs: $4-12 programmatic, $8-20 direct/native
- Newsletter sponsorships: $25-100 CPM
  - At 20,000 subs: $500-2,000 per send
- Premium podcast (ads + subscriber-only)
- Event partnerships (election coverage specials)

### Revenue Model Summary

| Phase | Timeline | Monthly Revenue | Key Metric |
|-------|----------|----------------|------------|
| Build | Mo 1-6 | $0-500 | Email subscribers |
| Monetize | Mo 6-12 | $2-8K | Paid conversion rate |
| Scale | Year 2 | $10-30K | Revenue per subscriber |

---

## Specific Design Decisions

### Color Palette
- **Primary**: Deep navy (#1a2744) — authority, trust, conservative without being aggressive
- **Accent**: Warm gold (#c8a84e) — premium feel, Canadian (wheat, maple)
- **Background**: Clean white (#ffffff) or warm off-white (#fafaf8)
- **Text**: Near-black (#1a1a1a) for readability
- **Avoid**: Red (too aggressive/Rebel), bright blue (too Liberal), green (too NDP)

### Typography
- **Headlines**: Strong serif (like Georgia, Charter, or Playfair Display) — gravitas, newspaper heritage
- **Body**: Clean sans-serif (Inter, system fonts) — modern, readable
- **This combination says**: serious journalism meets modern digital

### Logo Concept
- Simple wordmark: "THE COMMONS" in strong serif
- Optional: small maple leaf or Parliament building silhouette as icon
- Must work at favicon size and on social media avatars

### Homepage Layout

```
┌──────────────────────────────────────────┐
│  THE COMMONS          [Subscribe] [Login] │
│  News · Analysis · Opinion · Podcast      │
├──────────────────────────────────────────┤
│                                           │
│  📧 Get the daily briefing. Free.        │
│  [your@email.com] [Subscribe]             │
│                                           │
├──────────────────────────────────────────┤
│                                           │
│  TOP STORY                                │
│  ┌─────────────────────────────────────┐  │
│  │ [Hero Image]                        │  │
│  │ Headline: Bold, Opinionated         │  │
│  │ One-line summary                    │  │
│  │ 3 min read · Author                 │  │
│  └─────────────────────────────────────┘  │
│                                           │
│  TODAY'S BRIEFING                         │
│  • Story 1 headline — one line take       │
│  • Story 2 headline — one line take       │
│  • Story 3 headline — one line take       │
│  • Story 4 headline — one line take       │
│  [Read full briefing →]                   │
│                                           │
│  ┌─────────────── AD ──────────────────┐  │
│  │  Tasteful native ad                  │  │
│  └──────────────────────────────────────┘  │
│                                           │
│  ANALYSIS          │  OPINION             │
│  Card 1            │  Card 1              │
│  Card 2            │  Card 2              │
│                                           │
│  📧 Join 10,000+ Canadians who start     │
│     their day with The Commons            │
│  [Subscribe Free]                         │
│                                           │
├──────────────────────────────────────────┤
│  About · Contact · Advertise · Privacy    │
│  Independent. Not government-funded.      │
│  © 2026 The Commons News                 │
└──────────────────────────────────────────┘
```

### Article Page Layout

```
┌──────────────────────────────────────────┐
│  THE COMMONS          [Subscribe] [Login] │
├──────────────────────────────────────────┤
│                                           │
│  CATEGORY · 3 min read                    │
│                                           │
│  Headline: Strong and Clear               │
│  Subhead: The one-line take               │
│                                           │
│  By Author · Feb 22, 2026                 │
│  [Share] [Tweet] [Copy link]              │
│                                           │
│  [Hero Image — optional]                  │
│                                           │
│  WHY IT MATTERS                           │
│  Two sentences of context.                │
│                                           │
│  THE DETAILS                              │
│  • Bullet point one                       │
│  • Bullet point two                       │
│  • Bullet point three                     │
│                                           │
│  📧 Like this? Get it daily, free.       │
│  [Subscribe]                              │
│                                           │
│  THE BOTTOM LINE                          │
│  One opinionated sentence.                │
│                                           │
│  SOURCES: [link] [link]                   │
│                                           │
│  ── RELATED ──                            │
│  Card 1 · Card 2 · Card 3                │
│                                           │
│  📧 The Commons Daily Briefing           │
│  [your@email.com] [Subscribe Free]        │
└──────────────────────────────────────────┘
```

### Newsletter Email Design

```
┌──────────────────────────────────────────┐
│  THE COMMONS · Daily Briefing             │
│  February 22, 2026                        │
├──────────────────────────────────────────┤
│                                           │
│  Good morning.                            │
│                                           │
│  THE BIG STORY                            │
│  Headline — 2 sentence summary.           │
│  Why it matters. One sentence take.       │
│                                           │
│  ──────────                               │
│                                           │
│  📊 BY THE NUMBERS                       │
│  • Stat 1                                 │
│  • Stat 2                                 │
│  • Stat 3                                 │
│                                           │
│  ──────────                               │
│                                           │
│  WHAT ELSE                                │
│  🇨🇦 Canada: Headline (link)            │
│  💰 Economy: Headline (link)             │
│  🌍 World: Headline (link)               │
│  🤖 Tech/AI: Headline (link)             │
│                                           │
│  ──────────                               │
│                                           │
│  THE TAKE                                 │
│  One paragraph of analysis/opinion.       │
│  This is where the voice lives.           │
│                                           │
│  ──────────                               │
│                                           │
│  Was this forwarded to you?               │
│  [Subscribe free →]                       │
│                                           │
│  THE COMMONS · Independent Canadian News  │
│  Not government-funded. Never will be.    │
└──────────────────────────────────────────┘
```

---

## Key Conversion Tactics (Ranked by Impact)

1. **Exit-intent popup** with newsletter signup — 3-5% conversion rate
2. **Mid-article email capture** — 40% better than end-of-article
3. **Sticky mobile bottom bar** — always visible CTA
4. **Metered paywall** (5 free articles/month) — 10-20% conversion lift over hard paywall
5. **Free 7-day trial** for paid tier — 20-40% boost
6. **"Forward to a friend"** link in every newsletter — organic growth engine
7. **Social proof** ("Join 10,000+ Canadians") — builds trust
8. **One CTA per page, repeated** — don't confuse, just ask clearly

---

## Technical Stack

| Component | Choice | Cost |
|-----------|--------|------|
| CMS | Ghost (self-hosted) | $5-12/mo (VPS) |
| Hosting | DigitalOcean or Hetzner | Included above |
| CDN | Cloudflare (free tier) | $0 |
| Email sending | Ghost built-in (Mailgun) | ~$0.80/1000 emails |
| Payments | Stripe | 2.9% + $0.30/transaction |
| Analytics | Plausible (privacy-first) | $9/mo |
| Domain | thecommons.news | ~$20/yr |
| **Total** | | **~$30-50/month** |

---

## What NOT To Do (Lessons from Competitors)

1. **Don't be Rebel News**: No red/aggressive palette, no video autoplay, no banner ad spam, no donation popups every scroll
2. **Don't be legacy Postmedia**: No paywalled homepage, no cluttered ads, no 15-second load times
3. **Don't be a Substack clone**: Need a real website for SEO and brand, not just a newsletter page
4. **Don't add ads too early**: Ads slow the site and train users to expect free content. Build the email list first, monetize second
5. **Don't ignore mobile**: 60%+ of political news consumption is on phones
