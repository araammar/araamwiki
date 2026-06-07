# Concept: Cold Email Deliverability & Technical Infrastructure
tags: [cold-email, deliverability, DNS, domain, mailbox, warming, spam, B2B, technical]
source: DDGcd1JoJV0 — Lee Gjenj, Cold Email Masterclass 2025

## Summary / Definition

The technical foundation that determines whether your cold emails reach inboxes or spam folders. Deliverability is determined by domain reputation, mailbox reputation, DNS configuration, warming history, and sending patterns. Getting this wrong before you write a single email means your campaigns will fail regardless of copy quality.

## Why It Matters

Email service providers (Google, Microsoft) monitor every signal: domain age, IP reputation, copy patterns, sending velocity, open rates, reply rates, spam complaints. One compromised domain contaminates all associated mailboxes. Technical infrastructure is the unglamorous foundation that unlocks everything else.

## How It Works / The Mechanism

### Domain Strategy

**Buy from multiple registrars:**
- GoDaddy, Namecheap, Porkbun
- Spreading domains across registrars prevents mass account suspension from a single provider

**Domain naming with Namify:**
- Generate variations similar to your primary domain using different TLDs (.co, .io, .net, .email, .agency, etc.)
- Never send from your primary business domain — protect its reputation at all costs
- Example: primary = `agencyname.com` → cold email domains = `agencyname.co`, `agencyname.io`, `useagencyname.com`

**Domain volume for scale:**
- 100 domains × 4 mailboxes each = 400 mailboxes
- 400 mailboxes × 25 emails/day = 10,000 cold emails/day
- For starting out: even 10 domains × 4 mailboxes = 40 mailboxes = 1,000 emails/day

### DNS Configuration (Non-Negotiable)

All three records must be configured on every sending domain:

| Record | Purpose | Required |
|--------|---------|----------|
| **SPF** | Authorizes which servers can send email from your domain | Yes |
| **DKIM** | Cryptographic signature that verifies email authenticity | Yes |
| **DMARC** | Policy for handling email that fails SPF/DKIM checks | Yes |

**DMARC starting policy:** `p=none` (monitor mode — don't reject failing mail while you're learning your setup)

Missing any of these records causes immediate deliverability problems. Every major ESP checks for all three.

### Email Provider Selection

**Microsoft 365 (preferred for most):**
- Less strict enforcement than Google
- Better for higher-volume sending
- Preferred for most cold email operations

**Google Workspace:**
- Better sender reputation signal
- Stricter enforcement and policies
- Use for smaller volume or when Google brand association matters
- Google's policies are tighter — you can get accounts suspended more easily

### Warming

- Use MailReach for automated inbox warming
- Minimum 4 weeks of warming before sending any cold email from a new mailbox
- Warming = automated emails sent between mailboxes to simulate human usage, build reputation score
- Don't shortcut this. A warmed mailbox delivers; an unwarmed one doesn't.

### Sending Limits

| Limit | Value | Reason |
|-------|-------|--------|
| Max emails/mailbox/day | 25 (30 absolute max) | Exceeding triggers spam pattern detection |
| Max leads/domain | 1,000 | Keeps domain reputation manageable |
| Campaign throttle | 10% per day increase | Sudden volume spikes flag spam |

### Mailbox Infrastructure at Scale

- Aim for 4 mailboxes per domain (each domain has 4 addresses: `john@`, `sarah@`, `mike@`, `team@`)
- Each mailbox sends 25 emails/day
- Spread mailboxes across sending platforms (Instantly AI, Smartly) for additional redundancy
- Rotate sending so no single mailbox sends the same campaign

### Hyros for Attribution

- When spending on paid ads alongside cold email, Hyros provides attribution tracking
- Ensures you know which campaigns, channels, and touchpoints drove conversions
- Essential for accurate ROI measurement when running omni-channel outreach

### What Kills Deliverability

1. **Sending from unwarmed mailboxes**
2. **Identical copy across all mailboxes** — ESPs detect patterns; use spin tax
3. **Links and images in initial emails** — both trigger spam filters
4. **Too many emails too fast** — sending 200/day from a new mailbox immediately
5. **High spam complaint rate** — above 0.1% starts hurting deliverability
6. **Using your primary domain** — one problem contaminates your entire business email
7. **Missing DNS records** — SPF/DKIM/DMARC gaps cause immediate filtering

### Monitoring Deliverability

- Watch reply rates — sustained low reply rates often indicate spam folder placement
- Monitor spam complaint rates in Instantly dashboard
- Test new domain/mailbox setups by sending to seed accounts before campaign launch
- Reduce sending volume and re-warm if you see a deliverability drop

## What to Steal / Application

- Build the infrastructure first. Copy and lists don't matter if emails land in spam.
- Budget for domains, mailboxes, and warming before spending on lead data
- Treat domains as expendable — when one gets burned, you retire it and spin up a replacement
- The 100-domain model sounds like overkill until you realize one domain can be flagged and you lose zero volume because you have 99 more

## Related Pages
- [[cold-email-masterclass-2025]]
- [[cold-email-list-building]]
- [[cold-email-scaling]]
- [[triple-tap-copywriting]]
- [[cold-email-tool-stack]]
