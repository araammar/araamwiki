# Reference: Cold Email Tool Stack — Lee Gjenj's 2025 System
tags: [reference, tool, cold-email, B2B, outbound, automation, tech-stack]
tool_type: multi-tool cold email system
source: DDGcd1JoJV0 — Lee Gjenj, Cold Email Masterclass 2025

## Overview

The complete tool stack used in Lee Gjenj's cold email system as of 2025. Organized by function. Most tools have alternatives; the starred ones are Lee's explicit recommendations.

---

## Sending & Campaign Management

| Tool | Role | Notes |
|------|------|-------|
| **Instantly AI** ⭐ | Primary sending platform, campaign management, AB testing, UniBox, AI reply suggestions | ~$97+/month; native Clay integration; built-in AB testing; API for ReplyJI |
| **Smartly** | Alternative sending platform | Also cited as a top consolidator |

---

## Domain & Mailbox Setup

| Tool | Role | Notes |
|------|------|-------|
| **GoDaddy** | Domain registrar | Spread across multiple registrars |
| **Namecheap** | Domain registrar | Alternative to GoDaddy |
| **Porkbun** | Domain registrar | Budget-friendly option |
| **Namify** | Domain name generator | Finds variations on your target domain with different TLDs |
| **Microsoft 365** ⭐ | Mailbox provider | Preferred for most cold email operations; less strict than Google |
| **Google Workspace** | Mailbox provider | Better reputation signal but stricter enforcement |

---

## Email Warming

| Tool | Role | Notes |
|------|------|-------|
| **MailReach** ⭐ | Automated inbox warming | 4 weeks minimum before sending; builds domain/mailbox reputation |

---

## List Building — Lead Sources

| Tool | Role | Notes |
|------|------|-------|
| **Apollo.io** ⭐ | B2B lead database | Free tier + trustedleads.io hack for bulk export |
| **trustedleads.io** ⭐ | Apollo bypass | Paste Apollo filter URL → they scrape 10K leads for ~$50 |
| **ICPS** | LinkedIn scraper | 10K leads/day; auto-validates emails |
| **LinkedIn Sales Navigator** | B2B lead sourcing | Premium LinkedIn; pairs with ICPS or manual export |
| **Apify** | Custom scrapers | Google Maps, LinkedIn Jobs, social media, custom sources |

---

## Email Verification

| Tool | Role | Notes |
|------|------|-------|
| **Million Verifier** ⭐ | Standard email verification | Layer 1; removes hard bounces |
| **Findmail.com** ⭐ | Catch-all verification | Layer 2; ~50% of catch-alls are deliverable; most competitors skip this |

---

## Lead Enrichment & Personalization

| Tool | Role | Notes |
|------|------|-------|
| **Clay** ⭐ | Enrichment + AI personalization + workflow automation | $350+/month Explorer; use own API keys; Claggents for AI research |
| **Perplexity** | AI-powered research | Used inside Clay/N8N for lead research; also standalone |

---

## Signal Tools

| Tool | Role | Notes |
|------|------|-------|
| **Trigify** | LinkedIn social signals | Monitors LinkedIn engagement; ~$2,000+/month; high-volume only |
| **Crunchbase** | Funding data signals | Free + paid tiers; API available |
| **Apify** | Custom signal scrapers | Build any signal workflow (job listings, news, etc.) |
| **Clay native signals** | Built-in signals | Pre-built job change, news, hiring signals in Clay |

---

## Workflow Automation

| Tool | Role | Notes |
|------|------|-------|
| **Make.com** ⭐ | Mid-tier automation | Recommended for intermediates; 12 months free via Lee's Insiders |
| **N8N** | Advanced automation | Powers ReplyJI 2.0; open-source; self-hostable |
| **Zapier** | Automation alternative | Higher cost; mentioned but not recommended as primary |

---

## Reply Automation (ReplyJI Stack)

| Tool | Role | Notes |
|------|------|-------|
| **N8N** | Workflow orchestration | Core engine of ReplyJI 2.0 |
| **Superbase** | Knowledge base / database | Free; stores AI training data and reply history |
| **Claude (Anthropic)** ⭐ | Reply generation | Writes personalized cold email replies in ReplyJI |
| **Notion** | Human review interface | Review queue where team approves AI-generated replies |
| **Airtable** | Alternative review interface | Used instead of Notion by some operators |
| **Instantly AI API** | Reply sending | ReplyJI sends replies directly via Instantly API |

---

## Voicemail Drops

| Tool | Role | Notes |
|------|------|-------|
| **Drop Cowboy** ⭐ | Voicemail drop delivery | Affordable; strong APIs; preferred tool |
| **GoHighLevel** | All-in-one with voicemail | Built-in voicemail drop feature within automation workflows |
| **ElevenLabs** | AI voice cloning | Clone your voice; generate custom personalized voicemail audio |

---

## Direct Mail

| Tool | Role | Notes |
|------|------|-------|
| **Handwritten** ⭐ | Premium handwritten letters | 3D printer with real pen; ~$3/letter; gets opened; high-value leads only |
| **Clicksend** | Bulk cheap letters | Pennies per letter; scale; not handwritten; lower open rate |

---

## LinkedIn Automation

| Tool | Role | Notes |
|------|------|-------|
| **Hey Reach** ⭐ | LinkedIn outreach automation | 30 connections/day limit; automate connection requests + messages |

---

## Attribution & Analytics

| Tool | Role | Notes |
|------|------|-------|
| **Hyros** ⭐ | Multi-touch attribution | For paid ad campaigns alongside cold email; tracks what actually converts |

---

## AI Writing

| Tool | Role | Notes |
|------|------|-------|
| **Claude** ⭐ | Email copy, voicemail scripts, RLMs, reply generation | Used for Tap 2 body copy, voicemail scripts, and ReplyJI |
| **OpenAI / ChatGPT** | Alternative AI | Used in Instantly's built-in AI; OpenAI Assistants in Make.com workflows |

---

## Stack by Use Case

**Starter stack (100–500 emails/day, $200–400/month):**
- 5 domains (Namecheap/GoDaddy) + Microsoft 365 mailboxes
- MailReach (warming)
- Instantly AI (sending)
- Apollo free + trustedleads.io (list)
- Million Verifier (verification)
- Instantly built-in AI (reply management)

**Intermediate stack (1,000–5,000 emails/day, $800–1,500/month):**
- Everything above + more domains/mailboxes
- Clay Explorer ($350/month) for enrichment
- Make.com for reply automation
- Findmail.com (catch-all verification)
- Drop Cowboy + ElevenLabs (voicemail drops)
- Facebook + Google retargeting pixels

**Advanced stack (5,000–10,000+ emails/day, $3,000+/month):**
- Full infrastructure (100+ domains, 400+ mailboxes)
- Clay + Trigify ($2,000+/month)
- N8N + ReplyJI 2.0 + Superbase
- Handwritten (direct mail for interested replies)
- Hey Reach (LinkedIn automation)
- Crunchbase + Apify signal workflows
- Hyros for attribution

## Related Pages
- [[cold-email-masterclass-2025]]
- [[cold-email-deliverability]]
- [[cold-email-list-building]]
- [[signal-based-outreach]]
- [[clay-ai-workflow]]
- [[replyji-system]]
- [[omni-channel-outreach]]
- [[cold-email-scaling]]
