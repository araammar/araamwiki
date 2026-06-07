# Strategy: Cold Email Masterclass 2025 — Lee Gjenj's Complete System
tags: [cold-email, B2B, outbound, lead-generation, automation, AI, strategy]
applies_to: [B2B agencies, freelancers, SaaS, high-ticket services, universal outbound]
source: DDGcd1JoJV0 — Lee Gjenj, Cold Email Masterclass 2025 (436 minutes)

## Summary

The most complete cold email system documented in the wiki. Lee Gjenj's full masterclass covers every layer of outbound from technical infrastructure through list building, offer/copy creation, campaign management, AB testing, reply automation, and omni-channel follow-up. The three-pillar architecture runs everything.

## The Three Pillars

```
Pillar 1: Technical Infrastructure
  → Domains, mailboxes, DNS, warming, deliverability

Pillar 2: List Building & Targeting
  → Lead sources, verification, qualification, signals

Pillar 3: Offer & Copy
  → Triple Tap Framework, Reverse Lead Magnets, AB testing
```

## Framework / Steps

### 1. Technical Infrastructure
- Buy domains from different registrars (GoDaddy, Namecheap, Porkbun) to spread risk
- Use Namify to generate domain variations similar to primary domain, different TLDs
- Set up DNS: SPF, DKIM, DMARC on every domain (DMARC: `p=none` initially)
- Use MailReach for warming — minimum 4 weeks before sending cold email
- Prefer Microsoft 365 for most mailboxes; Google Workspace for smaller volume
- Send max 25 emails/mailbox/day (30 absolute max)
- Keep 1,000 leads per domain maximum
- Never send cold email from your primary domain
- See: [[cold-email-deliverability]]

### 2. Lead Source Selection (Decision Tree)
- **B2B companies** → LinkedIn (Sales Navigator) + Apollo
- **Local/B2C businesses** → Google Maps scraping
- **Influencers/creators** → Social media scraping (custom)
- Apollo hack: free account → set filters → copy URL → trustedleads.io ($50 for 10K leads)
- ICPS tool: LinkedIn scraper, 10K leads/day, auto-validates emails
- See: [[cold-email-list-building]]

### 3. Multi-Layer Email Verification
1. Million Verifier → standard verification
2. Findmail.com → catch-all email verification (~50% of catch-alls are deliverable)
- Never skip verification — unverified lists destroy sender reputation

### 4. AI Lead Qualification
- Before enrichment/personalization, run qualification prompt
- Qualification reduces list by 30–50%, increases reply rates 2–3x
- Prompt asks: does this lead match your ICP criteria?
- See: [[cold-email-list-building]]

### 5. Signal-Based Targeting
- True Signals: real-time buying intent data points (job changes, hiring, funding, news, LinkedIn engagement)
- Tools: Trigify (LinkedIn social signals), Crunchbase (funding), Apify + N8N (custom signals), Clay native signals
- Signal-based campaigns outperform standard: >5% reply rate vs. 1–2%
- See: [[signal-based-outreach]]

### 6. Clay AI Workflow
- Full enrichment pipeline: Apollo → qualify → verify → personalize → push to Instantly
- Claggents: AI agents that research leads automatically
- $350/month Explorer plan (use own API key to save cost)
- AI personalization: only 2–8 words from non-obvious internet research — test against control first
- See: [[clay-ai-workflow]]

### 7. Offer & Copy — Triple Tap Framework
- **Tap 1 (Open):** Subject line + preview text. Never signal the sale. Only curiosity or relevance.
- **Tap 2 (Read):** Email body. Problem + credibility in 2–3 sentences max. No links. No images. Spin tax on every phrase.
- **Tap 3 (Act):** CTA. One word reply. Never ask to book a call in first email. Use soft opt-out not "unsubscribe."
- Once they reply → warm email → can now send links, images, video, sales language
- See: [[triple-tap-copywriting]]

### 8. Reverse Lead Magnets
- AI-generated custom assets that appear hand-crafted per prospect
- Perceived value = perceived time investment; automation can deliver this at scale
- Trigger on reply interest → no human check needed if system is set up
- See: [[reverse-lead-magnets]]

### 9. Campaign Structure & AB Testing
- 3 emails max per sequence: Initial → Nudge (2–5 days later) → Dump (breakup)
- Test one element at a time
- Campaigns test audiences; AB variations test copy/offer
- Track opportunities (interested replies), not just reply rate
- J Number: emails needed to book one call — find this before scaling
- Benchmarks: >5% reply (signal campaigns), 1–2% (good), <1% (low)
- See: [[cold-email-ab-testing]]

### 10. Scaling
- Scaling equation: target emails/day ÷ 25 = mailboxes needed
- 100 domains × 4 mailboxes = 400 mailboxes → 10K emails/day
- Only scale after J Number is proven and consistent
- See: [[cold-email-scaling]]

### 11. Reply Automation — Three Levels
1. **Beginner:** Instantly built-in AI (AI inbox manager + snippets)
2. **Intermediate:** Make.com automation → catch replies → Perplexity research → OpenAI draft → Google Sheets + team email
3. **Advanced:** ReplyJI 2.0 — N8N + Superbase knowledge base + Claude + Notion + Instantly API
- Launch ReplyJI when you have 10+ interested replies per day
- See: [[replyji-system]]

### 12. Omni-Channel Follow-Up
- Cold email is top of funnel → cheapest clicks available
- Once prospect clicks any link, pixel them for retargeting
- Channels: paid retargeting, voicemail drops, direct mail, LinkedIn automation
- See: [[omni-channel-outreach]]

## When to Use

Any B2B business, agency, freelancer, or SaaS company doing outbound. The system scales from solo operator to enterprise. Start with Pillar 1 → 2 → 3 in sequence; don't jump to automation before fundamentals are solid.

## Key Mental Models

- **J Number:** The emails needed per booked call — the north star metric before any scaling decision
- **Top-of-funnel is the most expensive part of marketing** — cold email makes it cheap; retargeting keeps it cheap
- **Don't automate what you don't have yet** — build volume of replies before automating replies
- **Reply = warm email** — the rules change completely once they've replied; use it
- **Spin tax is mandatory** — ESPs detect identical copy patterns across mailboxes; randomize every phrase

## Related Concepts
- [[cold-email-deliverability]]
- [[cold-email-list-building]]
- [[triple-tap-copywriting]]
- [[reverse-lead-magnets]]
- [[signal-based-outreach]]
- [[clay-ai-workflow]]
- [[cold-email-ab-testing]]
- [[cold-email-scaling]]
- [[replyji-system]]
- [[omni-channel-outreach]]
- [[implicit-objection-marketing]]
- [[future-of-cold-email]]
- [[cold-email-tool-stack]]
- [[offer-architecture]]
- [[b2b-outbound-audience-2026]]
