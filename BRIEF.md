# The Commons — Static Website Build Brief

## What to Build
A fully designed, static HTML/CSS website for "The Commons" — an independent, right-of-center Canadian digital news outlet. This is a one-time static build with real content. No CMS, no backend, just beautiful HTML/CSS/JS that could be deployed to any static host.

## Brand
- **Name**: The Commons
- **Tagline**: "Independent Canadian News"
- **Secondary tagline**: "Not government-funded. Never will be."
- **Position**: Center-right. Smart, credible, opinionated but not angry. Poilievre's energy meets The Hub's rigor.
- **Tone**: Sharp, direct, trustworthy. Like a smart friend who reads everything.

## Design Direction
- **Color palette**: Deep navy (#1a2744) primary, warm gold (#c8a84e) accent, clean white (#fafaf8) background, near-black (#1a1a1a) text
- **Typography**: Strong serif for headlines (Georgia or similar), clean sans-serif for body (Inter or system fonts)
- **Layout**: Axios-style clean, lots of whitespace, scannable
- **Feel**: Modern, authoritative, premium. NOT cluttered, NOT angry, NOT tabloid
- **Inspiration**: Axios (layout), The Athletic (premium feel), Morning Brew (newsletter-forward)

## Pages to Build

### 1. Homepage (index.html)
- Sticky header: "THE COMMONS" wordmark + nav (News, Analysis, Opinion, Podcast) + Subscribe button + Login
- Hero section: Newsletter signup prominently ("Get the daily briefing. Free." + email input + subscribe button)
- Top Story: Large hero card with image, headline, summary, author, read time
- Today's Briefing: 5-6 bullet-point story summaries (Axios style: headline + one-line take)
- Analysis section: 2-3 article cards in a grid
- Opinion section: 2-3 article cards
- Mid-page newsletter CTA: "Join 10,000+ Canadians who start their day with The Commons"
- Audio player section: "Listen to the latest update" with embedded HTML5 audio player (link to audio-6am.mp3)
- Footer: About, Contact, Advertise, Privacy, "Independent. Not government-funded."

### 2. Article page (article.html)
- Same header
- Article layout:
  - Category tag + read time
  - Headline (large serif)
  - Subhead / one-line take
  - Author + date + share buttons
  - "WHY IT MATTERS" section
  - "THE DETAILS" section (bullet points)
  - Mid-article newsletter CTA
  - "THE BOTTOM LINE" section (one opinionated sentence, styled differently)
  - Sources with links
  - Related articles (3 cards)
  - End-of-article newsletter CTA

### 3. Newsletter / Subscribe page (subscribe.html)
- Clean page explaining the free newsletter
- Email signup form (non-functional, just styled)
- "What you'll get" section with sample content
- Social proof: "Join thousands of Canadians..."
- FAQ section about paid tier (coming soon)

## Content (Use Real News from Feb 22, 2026)

### Top Story
**Headline**: "Armed Man Shot Dead at Mar-a-Lago as Secret Service Tightens Perimeter"
**Summary**: An armed man in his twenties was killed by Secret Service agents after breaching the secure perimeter at Trump's Florida resort overnight. Trump was not present. The FBI is investigating.
**Category**: World

### Today's Briefing Stories
1. 🏒 "Canada Falls Short Again: U.S. Takes Olympic Hockey Gold in Milano-Cortina" — Hellebuyck was unbeatable. Crosby: "We did everything but score." Third consecutive final loss.
2. 💰 "Trump's New 10% Tariff Spares CUSMA-Compliant Canadian Goods — But There's a Catch" — The exemption exists on paper. Small businesses lack the resources to prove compliance.
3. ⚖️ "Supreme Court Strikes Down Trump's Emergency Tariff Powers" — Ruling calls use of emergency powers "unlawful." Trump doubles down, calls tariffs "vital."
4. 🏠 "60% of Canadian Parents Will Offer Free Room and Board During Post-Secondary" — Cost of living is reshaping how families approach education funding.
5. 🏥 "Canada's New Chief Public Health Officer: Restoring Trust Is Priority One" — Dr. Joss Reimer wants a "proactive approach" to countering misinformation.
6. ✈️ "Porter Flight Slides Off Taxiway at Hamilton Airport" — Edmonton-to-Hamilton flight lost traction on landing. No injuries. Transport Canada reviewing.

### Analysis Article (for article.html)
**Headline**: "The CUSMA Carveout Is Meaningless If Small Businesses Can't Navigate It"
**Subhead**: Ottawa needs to move fast — not with diplomacy, but with practical help for Canadian exporters.
**Category**: Analysis · Economy
**Author**: The Commons
**Date**: February 22, 2026
**Read time**: 4 min

**Why it matters**: Trump's new 10% global tariff technically exempts CUSMA-compliant Canadian goods. But compliance requires documentation that many small and mid-size exporters aren't equipped to produce. The Canadian Chamber of Commerce is calling for urgent federal guidance.

**The details**:
- The White House fact sheet confirms CUSMA-compliant goods are exempt from the new 10% global tariff
- But exporters must prove compliance at the border with detailed origin documentation
- Large manufacturers with trade lawyers will manage. Small businesses with 10-50 employees will struggle
- The Canadian Chamber of Commerce is calling on Ottawa to fast-track compliance guidance
- Meanwhile, the Supreme Court's ruling against Trump's emergency tariff powers creates additional uncertainty
- Markets reopen Monday. The Canadian dollar closed at 71.2 cents U.S. Friday. Expect volatility

**The bottom line**: A tariff exemption you can't access isn't an exemption at all. The Carney government needs to deliver practical help — compliance hotlines, simplified documentation, expedited guidance — not just diplomatic statements.

**Sources**: White House fact sheet, Canadian Chamber of Commerce statement, Globe and Mail, Global News

### Opinion pieces (cards only, no full pages needed)
1. "The Landlord-Tenant Board Is Broken. Everyone Knows It. Nobody Fixes It." — The Brampton case is a symptom, not an anomaly.
2. "Three Olympic Finals, Three Losses: Time to Rethink How Canada Builds Hockey Teams" — Talent isn't the problem. The process is.

## Technical Requirements
- Pure HTML/CSS/JS — no frameworks, no build tools
- Responsive (mobile-first)
- Fast: minimal assets, system fonts where possible, lazy-load images
- Dark mode support via prefers-color-scheme media query
- Use placeholder images (solid color blocks with text overlays, or use picsum.photos)
- Audio player should reference audio-6am.mp3
- Newsletter forms should be styled but non-functional
- Sticky header on scroll
- Smooth, polished feel — this needs to look like a real, funded news outlet

## File Structure
```
index.html
article.html
subscribe.html
styles.css
script.js
audio-6am.mp3
```

## Important
- Make it look REAL. Not a template. Not a student project. This should look like it has a design team behind it.
- The quality bar is: someone visiting this site should think "this is a real news outlet" not "this is a prototype."
- Navy/gold/white color scheme throughout. Consistent. Premium.

When completely finished, run this command to notify me:
openclaw system event --text "Done: Built The Commons static website with homepage, article page, and subscribe page" --mode now
