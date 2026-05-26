---
tags: [strategy, ai, prompt-engineering, chatgpt, founders, operators, productivity, dan-martell]
source_videos: [dan-martell-ai-cheat-codes-2026]
applies_to: universal
last_updated: 2026-05-25
---

# Strategy: Master Prompt Architecture

## Summary

The Master Prompt Architecture is Dan Martell's 4-tier system for turning any AI from a generic chatbot into a five-year-colleague-level operator. Each tier multiplies the previous one. The architecture is the reason two people using the same tool get structurally different outputs — one has the system, one has a blank prompt.

---

## The 4-Tier System

### Tier 1 — Personal Leverage (Master Prompt + Custom Instructions)

**What it is:** A reusable context profile that tells the AI who you are, what you're building, and how you think.

**What to include in your Master Prompt:**
- Business model and revenue range
- Target customer and key problems solved
- Products, services, pricing, offer structure
- Current priorities, projects, constraints
- Brand voice and decision-making style
- Tools used and team operations

**How to build it:** Ask ChatGPT to interview you for the master prompt. Answer using voice mode. When it generates the final master prompt, move it into Canvas to edit and tighten. Upload once. Use everywhere.

**Custom Instructions layer:** Set default rules that apply to every chat automatically.
- Tone and writing style (short, direct, no fluff)
- Preferred format (bullets, tables, step-by-step)
- Your constraints (time, team size, tools)
- How to handle uncertainty (flag assumptions, offer options)

**Purpose:** Reduces editing time because the AI follows your rules automatically from the first output.

---

### Tier 2 — Team Leverage (System Prompts)

**What it is:** Tested, reusable prompts built for specific outputs across departments.

**System Prompt Creation Loop:**
1. Describe exact desired output (deliverable, tone, format, constraints)
2. Generate the output
3. Refine in Canvas until publication-ready
4. Ask ChatGPT to write the system prompt that reliably generates that output
5. Test in a fresh chat; tighten until consistent
6. Save as internal asset

**High-payoff applications:**
- Sales: outbound scripts, follow-up sequences, objection handling
- Marketing: content briefs, landing page frameworks, ad angles
- Operations: SOPs, checklists, QA rubrics, onboarding
- Finance: analysis summaries, variance explanations, scenario planning
- Hiring: role scorecards, interview questions, candidate evaluation

**The asset:** A system prompt library becomes department-level intellectual property. Each prompt eliminates a repeated decision. Each decision eliminated is leverage compounded.

---

### Tier 3 — Compounding Leverage (AI Projects)

**What it is:** Dedicated workspaces where context accumulates over time. The AI remembers your brand, your customers, your history.

**What to store in a Project:**
- Brand voice and style guides
- ICP notes, market research, positioning
- Customer calls, meeting notes, email threads (as PDFs)
- Performance reports, dashboards, scorecards
- Existing assets: SOPs, scripts, landing pages, offers

**How to prompt inside Projects (simplified because context is loaded):**
- "Act as head of marketing. Draft the 5-email sequence for this campaign."
- "Act as investor. What questions should I ask based on these updates?"
- "Act as ops lead. Turn this process into an SOP with QA checklist."

**The compound effect:** "Outputs improve because the context improves."

---

### Tier 4 — Scalable Leverage (Custom GPTs)

**What it is:** Packaged system prompts deployed as organizational tools — consistent, repeatable, usable by anyone on the team.

**What to include:**
- The system prompt (the instruction asset)
- Optional knowledge files (master prompt, SOPs, examples)
- Clear output rules (format, constraints, guardrails)
- Short "how to use this" starter prompt

**High-value Custom GPTs to build first:**
- **Content Brief Builder** — SEO brief, outline, FAQs, schema in one run
- **Sales Follow-Up Writer** — brand voice replies with next steps
- **SOP Generator** — turns meeting notes into process docs and checklists
- **Candidate Scorer** — scores resumes against a role scorecard
- **Meeting Summary → Action Plan** — converts notes to priorities and tasks

**The moat:** "A good system prompt is reusable. A great system prompt is teachable. A library of them becomes an operating system your competitors cannot copy quickly."

---

## The 7 Prompt Keywords (Control Framework)

Use these keywords inside any prompt to get dramatically different outputs:

| Keyword | What It Does |
|---|---|
| **Act as [role]** | Sets expertise and voice — "Act as a growth marketer with 10 years SaaS experience" |
| **Deep research** | Forces research workflow with verification and synthesis |
| **First principles** | Rebuilds answer from fundamentals instead of clichés |
| **Devil's advocate** | Stress-tests assumptions, surfaces risks and blind spots |
| **Constraints first** | Forces specificity — timeline, tools, budget, team size |
| **Format as** | Makes output instantly usable — tables, YAML, JSON, checklists |
| **Verify and cite** | Pushes for sourcing and inline references |

**Combining keywords:** "Act as a senior ops lead. First principles: rebuild this onboarding process. Constraints first: 2-person team, 30-day window, no new software. Format as a checklist."

---

## The Reverse Prompt Framework

**The problem:** Most people write prompts forward (describe what you want → get output → iterate).
**The fix:** Build backward from a great output.

Process:
1. Get a great output (however you got there)
2. Ask: "Write the system prompt that would reliably generate an output like this every time"
3. Test the generated system prompt in a fresh chat
4. Refine until consistent
5. Save and reuse

**Result:** Perfect outputs with less back and forth — copy-paste repeatability.

---

## Sequencing Principle

"Sequencing equals success."

Tier 1 before Tier 2. Tier 2 before Tier 3. Tier 3 before Tier 4. Founders who jump to Custom GPTs before building their master prompt get generic tools. Founders who build in sequence get compounding leverage.

---

## Source

- Source video: Dan Martell — "The AI Cheat Codes Every Founder Needs in 2026"
- Source article: danmartell.com — "Master Prompts, System Prompts, and Custom GPTs"

## Related Pages

- [[three-levels-of-ai]] — the framework this strategy implements
- [[ai-operating-system-for-founders]] — why this architecture matters
- [[ai-tool-stack-for-founders]] — which tools to apply this architecture to
- [[zero-inbox-system]] — one applied example of this system in action
