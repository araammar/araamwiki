# Concept: Cold Email AB Testing & Campaign Optimization
tags: [cold-email, AB-testing, campaign, optimization, metrics, B2B, outbound]
source: DDGcd1JoJV0 — Lee Gjenj, Cold Email Masterclass 2025

## Summary / Definition

The systematic process of testing one variable at a time to identify what drives cold email performance. Campaigns test audiences; AB variations test copy and offers. The goal is finding the "J Number" — the number of emails needed to book one call — and then scaling once that number is proven.

## Why It Matters

Without structured testing, you don't know if poor results come from the wrong audience, wrong offer, wrong copy, or wrong timing. Changing multiple things at once makes it impossible to know what worked. Single-variable testing is the only way to build real knowledge.

## How It Works / The Mechanism

### The Testing Hierarchy

```
Level 1: Campaign test → different audiences / ICPs
Level 2: AB variation test → different copy / offer within same audience
```

**Never change both audience and copy at the same time.** You'll get data you can't learn from.

### What Campaigns Test

A "campaign" in Instantly is the container. Campaigns test:
- Different ICP segments (e.g., CMOs at SaaS companies vs. CMOs at e-commerce brands)
- Different lead sources (Apollo vs. LinkedIn scrape)
- Different signals (hiring signal vs. funding signal)
- Different geographic markets
- Different company sizes

### What AB Variations Test

AB variations within a campaign are copy/offer tests:
- Subject line A vs. subject line B
- Body angle A (pain-focused) vs. angle B (curiosity-focused)
- CTA A ("Worth a chat?") vs. CTA B ("Relevant to you?")
- Offer A (audit) vs. Offer B (demo)
- Spin tax variation A vs. spin tax variation B

**Isolate the variable.** Change only the element you're testing. Keep everything else identical.

### What to Track — Opportunities, Not Reply Rate

The standard cold email metric is reply rate. Lee argues this is incomplete and misleading.

**The better metric: Opportunities**

An opportunity = an interested reply that could become a booked call.

Why opportunities matter more than reply rates:
- A 10% reply rate full of "not interested" and "unsubscribes" is worthless
- A 2% reply rate that's all interested replies is valuable
- Reply rate tells you people responded; opportunity rate tells you the quality of those responses

**Secondary metric: J Number**

J Number = total emails sent ÷ booked calls generated

If you sent 500 emails and booked 5 calls, your J Number is 100.

J Number is the north star because it directly translates to revenue math:
- J Number × cost per email sent = cost per call booked
- Cost per call booked × close rate = customer acquisition cost
- If CAC is acceptable, scale the infrastructure

### Campaign Benchmarks

| Performance Level | Reply Rate | Context |
|-----------------|-----------|---------|
| Signal-based (strong signals) | >5% | Trigify/hiring/funding signals; narrowly targeted |
| High performing | >3% | Strong copy + good list quality |
| Good | 1–2% | Healthy standard campaign |
| Low performing | <1% | List quality, copy, or ICP issue |

A "good" campaign at 1–2% reply rate is not a failure — it's a baseline to optimize from. A signal-based campaign at 5% is exceptional.

### Testing Cadence

- Run variations for minimum 200–500 emails each before drawing conclusions
- Small sample sizes produce unreliable data — resist the urge to call winners early
- Once you have a winner, roll it to 100% of sends before starting the next test
- Test one thing at a time: subject → body → CTA → offer → audience (in that order of impact, roughly)

### The Sequence Structure

**3 emails maximum per sequence:**
1. **Initial:** Main pitch (Triple Tap framework)
2. **Nudge:** 2–5 days later. Short. "Did this land with you?" type message. No new pitch.
3. **Dump (breakup email):** "I'll stop emailing. Was this the wrong time, or wrong fit?" — sometimes generates replies from people who ignored emails 1 and 2

### When to Stop a Campaign

- Below 0.5% reply rate after 200+ sends: diagnose before scaling
- High spam complaints (>0.1%): pause immediately, check copy and list quality
- Reply rate was good but no opportunities: ICP is wrong or offer doesn't match the pain

### The J Number Decision Framework

```
Find J Number (test at small scale)
  ↓
Is J Number economically viable?
  If yes → scale infrastructure (more mailboxes/domains)
  If no → improve copy or offer before scaling
  ↓
Prove J Number is consistent across 2–3 campaigns
  ↓
Scale to target email volume
```

Don't scale before finding a consistent J Number. Scaling a broken campaign burns infrastructure and budget.

## What to Steal / Application

- Define your "opportunity" before launching — what counts as a qualified interested reply for your offer?
- Calculate your J Number in the first 200 emails; don't wait for the campaign to "finish"
- Test subject lines first — they have the highest leverage (controls Tap 1 open rate)
- Use AB variations in Instantly (built-in feature) to test two subject lines simultaneously
- Signal campaigns are a separate test from copy tests — run them as separate campaigns, not AB variations

## Related Pages
- [[cold-email-masterclass-2025]]
- [[triple-tap-copywriting]]
- [[cold-email-scaling]]
- [[cold-email-list-building]]
- [[signal-based-outreach]]
- [[replyji-system]]
