# Concept: Signal-Based Outreach
tags: [cold-email, signals, B2B, outbound, intent-data, Clay, Trigify, Apify, automation]
source: DDGcd1JoJV0 — Lee Gjenj, Cold Email Masterclass 2025

## Summary / Definition

Triggering cold email outreach based on real-time behavioral and business signals that indicate a prospect is actively experiencing a problem your offer solves. Instead of reaching out blind, you reach out when evidence suggests the timing is right. Signal-based campaigns routinely produce 5%+ reply rates vs. 1–2% for standard campaigns.

## Why It Matters

The right message at the right time beats a great message at a wrong time. Signals collapse the "spray and pray" model — they make outreach feel relevant because it is relevant. The prospect is genuinely experiencing what you're addressing right now.

## How It Works / The Mechanism

### What Counts as a True Signal

A True Signal is a real-time, externally verifiable data point that indicates buying intent or a changed situation. Not static database data. Not predicted intent. Actual observable events:

| Signal Type | What It Indicates | Where to Find It |
|-------------|-----------------|-----------------|
| Job change (new hire in role) | New decision-maker who wants to prove themselves | LinkedIn, Trigify |
| Company hiring for specific roles | Growth, expansion, new budget area | LinkedIn Jobs, job boards |
| Company news / press | New funding, product launch, expansion | Google News, Crunchbase |
| LinkedIn engagement | Prospect engaged with content in your niche | Trigify |
| Funding round | New money, new initiatives, new budget | Crunchbase |
| Company growth indicators | Headcount increase, new office | Apify custom scrapers |

### What NOT to Count as a Signal

- **"Buying intent" scores** from Apollo or similar: not reliable, based on page visit models that don't actually predict purchase behavior
- **Revenue data** on private companies: fictional; companies don't disclose this
- **Signal filters in Apollo:** Lee explicitly avoids these — they're unreliable

### Signal Tools

**Trigify** — LinkedIn Social Signals
- Monitors LinkedIn for engagement activity from your target accounts
- Identifies when prospects interact with content in your space
- Best for: SaaS, agencies, anything where LinkedIn engagement is a meaningful signal
- Cost: ~$2,000+/month — worth it at high volume; not for beginners

**Crunchbase** — Funding Data
- Real-time funding announcements (Series A, B, C, seed rounds)
- New funding = new budget, new initiatives, new urgency to solve problems fast
- Free and paid tiers; API available

**Apify + N8N** — Custom Signal Scrapers
- Build your own signal scrapers for any publicly available data
- Example: scrape LinkedIn Jobs daily for "Head of Marketing" hires → enrich → personalize → push to Instantly
- N8N orchestrates the workflow; Apify runs the scrapers
- Most flexible and customizable option

**Clay Native Signals**
- Built into Clay's enrichment platform
- Pre-built signal integrations (job changes, news, hiring)
- Easier to set up than custom Apify; less flexible

### Signal Workflows in Practice

**Workflow 1: Job Listing Signal (Hiring)**
```
Daily scrape LinkedIn Jobs → filter by target role (e.g., "Head of Sales") →
match to company in your ICP → enrich contact at that company →
write personalized email referencing the hiring signal → push to Instantly
```
Hook angle: "I saw you're hiring a [Role] — that usually means [problem you solve]. We help with that."

**Workflow 2: Social Signal (LinkedIn Engagement)**
```
Trigify monitors LinkedIn for engagement on content in your category →
prospect engages with relevant content → alert fires →
Clay enriches the contact → personalized email sent within 24–48 hours
```
Hook angle: Lead doesn't know you saw them engage; email feels coincidentally relevant.

**Workflow 3: Company Signal (Funding)**
```
Crunchbase API → daily scrape for new funding rounds in your ICP sector →
match companies → find decision-maker email →
personalize email referencing the round → push to Instantly via N8N
```
Hook angle: "Congrats on the [X] round. Companies that just raised typically face [problem]. We solve that."

### Benchmark Expectations

| Campaign Type | Expected Reply Rate |
|--------------|-------------------|
| Signal-based (strong signals) | >5% |
| Standard cold email (good list) | 1–2% |
| Standard cold email (average) | <1% |

Signal campaigns outperform by 3–5x. The cost of signal tooling ($2K+/month for Trigify) is justified once you're at volume.

### Cost Reality Check

- Signal workflows are expensive to set up and maintain
- Trigify: ~$2,000+/month
- Clay: $350+/month
- Apify: variable based on volume
- N8N: open-source but requires technical setup
- **Recommendation:** Start standard cold email → prove your offer converts → add signal infrastructure as you scale

## What to Steal / Application

- The hiring signal is the easiest to start with — LinkedIn Jobs is free and public
- Funding rounds via Crunchbase are second easiest — straightforward API
- Build Trigify into your stack only after you're sending 5,000+ emails/day
- Test: Run same ICP with signal-vs-no-signal split to prove lift before committing to tooling cost
- The headline stat (>5% reply rate) should be your benchmark for any signal campaign you launch

## Related Pages
- [[cold-email-masterclass-2025]]
- [[clay-ai-workflow]]
- [[cold-email-list-building]]
- [[cold-email-ab-testing]]
- [[cold-email-scaling]]
- [[cold-email-tool-stack]]
