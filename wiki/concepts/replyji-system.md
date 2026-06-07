# Concept: ReplyJI — Autonomous Cold Email Reply System
tags: [cold-email, automation, AI, reply-management, N8N, Notion, Instantly, B2B]
source: DDGcd1JoJV0 — Lee Gjenj, Cold Email Masterclass 2025

## Summary / Definition

ReplyJI is Lee Gjenj's custom AI reply automation system for managing cold email responses at scale. It categorizes incoming replies, performs research on leads, generates personalized responses using Claude and a trained knowledge base, queues them for human review in Notion, and sends approved replies directly via the Instantly API. As it gets corrected, it trains itself not to make the same mistakes again.

**The core insight:** Replying within 30 minutes of a lead responding increases conversion by 60%. At scale, humans can't do this alone. ReplyJI solves speed and personalization simultaneously.

## Why It Matters

Getting replies is only half the battle. Converting replies to calls is where revenue is made. ReplyJI manages the conversion layer — the gap between "interested reply" and "booked call" — which most cold emailers handle manually and slowly.

## How It Works / The Mechanism

### The Three Levels of Reply Automation

**Level 1 — Beginner: Instantly Built-In**
- No setup required beyond connecting OpenAI API key
- Settings path: Instantly → Settings → Preferences → AI Automations
- Enable: AI reply suggestions, positive reply notifications, snippet saving
- Leave AI inbox manager OFF initially (too autonomous until you trust it)
- Works for anyone with fewer than 10 replies/day

**Level 2 — Intermediate: Make.com Automation**
- Custom automation that catches replies via webhook
- Workflow: incoming reply → Perplexity research on lead → OpenAI assistant generates reply draft → log to Google Sheets → email team with draft + research + UniBox link
- Team reviews draft in Google Sheets → manually sends via Instantly UniBox
- Templates available in Lee's resources
- Best for: 5–20 replies/day, teams that want research assistance but human control

**Level 3 — Advanced: ReplyJI 2.0 (Full System)**
- Fully autonomous with human check option
- Built on N8N (workflow automation) + Superbase (knowledge base) + Claude (copy) + Notion (review queue) + Instantly API (sending)
- Self-improving: team corrections train the AI over time

---

### ReplyJI 2.0 — Architecture

```
Incoming reply (Instantly webhook)
  ↓
Get thread via Instantly API
  ↓
AI categorization agent:
  - Interested → research + draft → Notion review queue
  - Custom path (RLM trigger) → automatic, no human check
  - Soft no → simple template reply, nearly always correct, send direct
  - Hard no → delete lead, add to block list, no reply
  ↓
For "Interested" replies:
  - Perplexity agent researches lead
  - Memory module recalls conversation history (ongoing threads)
  - Claude writes personalized reply
  - Superbase knowledge base consulted for historical training
  - Convert to HTML (Instantly format)
  - Create Notion page with: category, last message, AI reply, good column
  ↓
Team reviews in Notion:
  - Read AI reply
  - If correct: click "Good" → triggers webhook → sends via Instantly API
  - If wrong: write corrected reply + reasoning → triggers training
  ↓
Training module:
  - AI agent reviews corrected copy and reasoning
  - Identifies what to update in Superbase knowledge base
  - Updates knowledge base so same mistake doesn't recur
```

### Reply Categories

ReplyJI categorizes every reply into one of four buckets:

| Category | What It Means | Action |
|---------|-------------|--------|
| **Interested** | Prospect wants to have a conversation | Research → draft → Notion queue |
| **Custom path** | Prospect triggered an RLM workflow (reverse lead magnet) | Automatic — no human check |
| **Soft no** | Mild objection, "maybe later," not flat refusal | Simple template reply, nearly always auto-correct |
| **Hard no** | Unsubscribe, anger, firm refusal | Delete lead + add to block list |

### The Soft No — Underrated Category

Most systems handle "interested" and "not interested." ReplyJI breaks down the "not interested" category into soft no vs. hard no, which is operationally important:

- **Soft no replies still deserve a response** — timing objections often convert later
- Template for soft nos is nearly 100% accurate → Lee sends these directly without human review
- Hard nos waste time and resources; route them out immediately

### Notion Review Interface

The Notion page created for each "interested" reply contains:
- **Category label** assigned by AI
- **Last message** from the lead
- **AI-generated reply**
- **"Good" column** — the trigger column (team selects: Good / Send AI Sequence / other)
- **Delivery status** — confirmed sent or failed
- **Additional research** on the lead

Team workflow is minimal: open Notion, read the AI reply, if it's right click "Good." That's it.

### The Training Loop

ReplyJI gets better over time through structured team feedback:

1. Team sees AI reply that got something wrong
2. Team writes the correct reply
3. Team enters the reasoning for why the AI was wrong
4. "Train AI" button triggers the training module
5. N8N agent processes the corrected copy, the original reply, and the reasoning
6. Superbase knowledge base is updated to prevent the same mistake
7. All future similar replies benefit from this correction

**First week:** High training volume; expect to correct frequently
**After 1 week of training:** System handles most replies correctly autonomously
**Ongoing:** Occasional corrections as new edge cases emerge

### When to Launch ReplyJI

- **Under 10 replies/day:** Use Instantly's built-in AI. Don't build ReplyJI yet.
- **10+ replies/day:** Volume justifies the setup cost. Launch ReplyJI.
- **Key principle:** Don't solve problems you don't have. First, get the replies. Then automate them.

### Technical Requirements

- N8N (workflow automation — can self-host or cloud)
- Superbase (free, open-source database for knowledge base)
- Claude API (for reply generation)
- Notion or Airtable (review interface)
- Instantly API access (for reading threads and sending replies)
- Perplexity API (for lead research)
- Make.com or custom webhooks for Notion trigger automations

## What to Steal / Application

- The soft no / hard no distinction is immediately applicable — build two different response paths
- "30 minutes = 60% higher conversion" is the benchmark that justifies any reply automation investment
- Start with Level 1 (Instantly built-in) → prove it can handle your replies → move to Level 2 → move to Level 3 only when you have 10+ interested replies/day
- The training feedback loop is the compounding advantage — the system improves with every correction
- Pair with [[reverse-lead-magnets]] for the custom path (auto-triggered, no human needed)

## Related Pages
- [[cold-email-masterclass-2025]]
- [[reverse-lead-magnets]]
- [[triple-tap-copywriting]]
- [[omni-channel-outreach]]
- [[cold-email-scaling]]
- [[cold-email-tool-stack]]
