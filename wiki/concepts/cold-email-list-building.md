# Concept: Cold Email List Building & Lead Qualification
tags: [cold-email, list-building, leads, ICP, Apollo, LinkedIn, verification, qualification, AI]
source: DDGcd1JoJV0 — Lee Gjenj, Cold Email Masterclass 2025

## Summary / Definition

The process of building targeted, verified, and qualified lead lists for cold email campaigns. Quality beats quantity at every stage — a 1,000-person list of qualified ICPs outperforms a 10,000-person unqualified list. Three layers: sourcing → verification → AI qualification.

## Why It Matters

Your list is your targeting. The wrong ICP wastes budget, burns domains, generates spam complaints, and produces no revenue. The right ICP with a tight qualification filter can 2–3x reply rates before you write a single line of copy.

## How It Works / The Mechanism

### Lead Source Decision Tree

```
Who are you targeting?

B2B companies → LinkedIn + Apollo
Local/physical businesses → Google Maps scraping
Influencers/creators → Social media scraping (custom Apify)
```

### Apollo — The Primary B2B Lead Source

**Apollo.io** is the standard B2B lead database. Most cold emailers use it wrong.

**The trustedleads.io hack (free Apollo account):**
1. Create a free Apollo account
2. Set your filters (job title, industry, location, company size, email status)
3. Copy the URL from Apollo's search results page
4. Paste URL into trustedleads.io
5. They scrape the full filtered list → 10,000 leads for ~$50
- This bypasses Apollo's per-lead pricing for high-volume users

**Apollo filter best practices:**

| Filter | Use? | Notes |
|--------|------|-------|
| Job title | ✅ Always | Most important filter |
| Industry / keywords | ✅ Always | Defines your ICP |
| Location | ✅ Always | Especially for local-market offers |
| Company size | ✅ Always | Match to your offer's TAM |
| Email status (verified) | ✅ Always | Only export verified emails |
| Signal filters | ❌ Avoid | Unreliable data, burns credits |
| Revenue filter | ❌ Avoid | Private companies don't disclose; data is fictional |
| Buying intent | ❌ Avoid | Not reliable enough to filter on |

### ICPS Tool — LinkedIn Scraper

- Scrapes LinkedIn at scale: 10,000 leads/day
- Auto-validates emails during scraping
- Useful for LinkedIn-specific targeting where Apollo data is thin

### Google Maps Scraping

- Best for local businesses: dentists, restaurants, contractors, agencies, retail
- Use Apify's Google Maps Actor or similar
- Extract: business name, phone, email (if listed), address, category, rating
- Pair with custom email finding tools if email isn't in listing

### Multi-Layer Email Verification

Never send to an unverified list. Two-layer verification is the standard:

**Layer 1 — Million Verifier:**
- Standard verification: confirms email format, domain exists, mailbox exists
- Removes hard bounces before they happen
- All "Valid" results → send
- All "Invalid" results → discard

**Layer 2 — Findmail.com (catch-all verification):**
- Catch-all emails: domains configured to "accept" any email address (can't verify individual mailboxes)
- Standard verifiers mark these as "risky" — most senders skip them
- Findmail actually tests the specific mailbox → identifies which catch-alls are real
- ~50% of risky/catch-all emails are actually deliverable
- Unlocks a large segment of B2B leads your competitors are ignoring

**Verification workflow:**
```
Raw list → Million Verifier → 
  Valid → Include
  Invalid → Discard
  Catch-all/Risky → Findmail → 
    Deliverable → Include
    Not deliverable → Discard
```

### ICP Definition First

Before sourcing any leads, define your ICP completely:
- Job title(s) that control budget for your offer
- Industry(ies) you serve best
- Company size range (employees or revenue)
- Geographic location constraints
- Technology stack signals (if relevant)
- Pain indicators (if detectable from public data)

ICP is the foundation. Weak ICP = weak list = weak results no matter how good your copy.

### AI Lead Qualification

After verification, run every lead through an AI qualification prompt before enrichment or personalization.

**What it does:**
- Reviews lead data against your defined ICP criteria
- Scores or removes leads that don't match
- Can check for disqualifying factors (competitor employees, wrong company type, etc.)

**Results:**
- Reduces list by 30–50%
- Increases reply rates 2–3x
- Dramatically improves the quality of interested replies
- Worth the API cost every single time

**Prompt structure:**
- Input: lead name, title, company, company description
- Task: does this lead match [ICP criteria]? Score 1–10 or Yes/No
- Threshold: only include leads above [score threshold]

### Volume Guidelines

| Stage | Daily Volume | Approach |
|-------|------------|---------|
| Starting out | 100–500 emails/day | Focus on quality over quantity |
| Scaling | 1,000–5,000 emails/day | Need 40+ mailboxes |
| Full scale | 5,000–10,000+ emails/day | Need 200–400+ mailboxes |

Don't scale volume before finding your J Number (emails needed per booked call). Scaling a broken campaign just burns more infrastructure.

## What to Steal / Application

- Run the three-filter combo on Apollo (title + industry + company size) before any other filter
- Always verify before sending — skipping verification is false economy
- Run Findmail on catch-alls — you're leaving 50% of verified leads on the table if you don't
- Qualification prompt before enrichment/personalization: saves compute cost and improves results
- If your reply rates are low, check list quality before touching copy

## Related Pages
- [[cold-email-masterclass-2025]]
- [[signal-based-outreach]]
- [[clay-ai-workflow]]
- [[cold-email-deliverability]]
- [[cold-email-ab-testing]]
- [[cold-email-tool-stack]]
- [[b2b-outbound-audience-2026]]
