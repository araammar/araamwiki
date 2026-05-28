---
tags: [strategy, framework, AI, marketing, workflows, tools, automation, creative-strategy]
source_videos: [tSopiLVEreM]
last_updated: 2026-05-24
---

# Strategy: AI Workflows for Marketers

## Summary
AI has crossed the threshold from experimental tool to active displacer of mid-level creative and analytical jobs. This strategy guide covers the full practical landscape: where AI is actually replacing people (agency jobs, CGI, research), what level of AI engagement makes sense (superpowered vs. AI-enabled vs. resistant), and then a detailed walkthrough of specific workflows across three categories — strategy/research, visual production, and deep analytics. The goal is to become "AI-enabled" — someone who can do more, faster, and bat above their weight class using these tools — not someone obsessing over the latest model.

## When to Use This
- You're a marketer, creative director, or solo creator trying to understand where to invest your AI learning time
- You're doing brand strategy work and spending too much time on research
- You want to improve your visual content quality without hiring a full design team
- You're managing paid and organic content at scale and drowning in manual analysis
- You work at an agency or brand team and want to understand what's happening to your industry

## The Framework / Steps

### Understanding the Landscape

**The Agency Reality**
Major agency holding companies (the "Comms") are merging and eliminating thousands of creative jobs. The reason: mid-tier specialist roles (project manager + copywriter + strategist + art director + designer as separate people) can now be performed by 2–3 people enabled by AI. The agencies that survive will do more with less. Creatives who can jump the "exploitation gap" — operating independently with AI tools at agency quality for lower cost — will thrive.

**Four Levels of AI Engagement**
1. **Superpowered** — elite workflows, rare, probably not you (and that's fine)
2. **AI-Enabled** — using tools to do more faster, bat above your weight class. This is the goal.
3. **AI-Resistant (soft)** — reluctant but not opposed; this video is for you
4. **AI-Resistant (angry)** — actively anti-AI, commenting hostility online. This is a grief response to career uncertainty; recognize it and move on from the people stuck here.

The strategic imperative: if you work in any field where AI is being applied around you, being resistant means you get left behind. The goal is "enabled," not "replaced."

**What Brands Are Actually Doing**
- Valentino: AI-generated surreal art campaign, largely ignored the backlash
- Revolve: Full AI content series for a product launch
- Major e-commerce retailers: 20–30% of product imagery is now AI-generated; consumers can't tell
- Luxury CGI work: Firms are replacing high-paid 3D CGI artists with AI-generated equivalents. "No one even knows. Looks the same on feed."

---

### Workflow Category 1: Strategy & Research

**Tool: Perplexity / Comet (Agent Mode)**
Use for social media comment and video analysis at scale. The "Comet" feature within Perplexity's agent mode is specifically built for this. The workflow:
1. Open a TikTok search for your product category or competitor
2. Prompt: "Watch 100–300 of these videos, list the most mentioned brands with their pros and cons, and what content strategies are performing best in these reviews"
3. Let agent mode run in the background — can take 20+ minutes for 300 videos; work on other tasks while it runs
4. Output: comprehensive brand sentiment analysis, common complaints, content hook performance ranking, audience demographics, suggested hooks with engagement estimates

You can also prompt for demographic analysis (age/race breakdown visible in comments), screenshot-based sentiment work, and deep dives on specific competitors: "Give me all the top complaints about [competitor brand]." The TikTok comment section is the best brand strategy research environment available — real people giving unfiltered product reactions in real time.

This replaces hours of manual research that used to be done by junior analysts. Use the output to brief content, identify competitor weaknesses to address in your own content, and generate hook angles from real consumer language.

**Tool: Manis (Influencer Research)**
Use for building influencer seed lists at scale:
1. Set parameters: follower range (e.g., 5K–200K), keywords/brands mentioned, posting frequency (active in last 30 days)
2. Let Manis search TikTok via API, verify and filter, and return a list of 100–200 qualified creators
3. **Vibe-code a front end within Manis** — you can ask Manis to build a simple functional website/interface where team members enter keywords and parameters and receive the generated list, without needing you to run each search. One platform, minimal dev work, done in a single session.

This replaces manual influencer research and outreach list building — previously a multi-hour or multi-day task. The vibe-coded front end also removes the workflow bottleneck of routing everything through one person.

**Tool: Claude or ChatGPT (Brand Second Brain)**
Build a project in Claude/ChatGPT that functions as an in-house brand strategist:
- Upload the brand's value proposition, tone of voice, target audience profile, and past campaign examples
- Add any research outputs from Perplexity
- Set custom instructions: "You are the in-house brand strategist for [Brand]. Your tasks include: [list]. Your tone is [describe]. Do not [restrictions]."

Every new team member or collaborator can query this project for brand-consistent answers, campaign ideas, and copy direction. Eliminates the "I don't know the brand well enough" ramp-up time.

**Master Prompt Structure for a Brand Second Brain:**
```
You are the in-house brand strategist for [Brand Name].
Brand value proposition: [describe]
Target audience: [describe]
Tone of voice: [describe — e.g., direct, irreverent, expert but accessible]
What you help with: campaign ideation, copy review, content briefs, competitor analysis
What you avoid: [brand-specific no-gos]
```

Upload YouTube transcripts, newsletters, brand guidelines, and past reports as context files.

---

### Workflow Category 2: Visual Production

**Platform: Leonardo AI**
A single platform housing multiple AI models for images and video. Key workflows:

**Logo Animation**
1. Generate a metallic/stylized version of a logo using NanoBanana (ultra-accurate image model)
2. Import reference image into Kling 01 or Veo 3
3. Prompt: "Rotate around the logo slowly with cinematic lighting glinting off the surface"
4. Result: logo animation that used to require a 3D artist and hours/days of render time

**AI Transitions for Video**
Use the Frame Flow blueprint in Leonardo:
1. Upload start frame and end frame (two stills from different settings/times)
2. It generates a seamless video transition between them
3. Speed-ramp the output inside your edit for social media content

Replaces expensive bridge footage or awkward jump cuts.

**Product Spin Videos**
Use the Product Spin blueprint:
1. Upload a static product shot
2. Generate a 360-degree spin animation
3. Use as a cut shot in product videos or ads

**Animating Static Ads**
Take a static Meta ad image and animate the background:
1. Animate just the background layer
2. Place it behind your static text/product
3. Ad becomes a video with no new filming required

**AI Hooks for Ads**
Generate surreal, energetic, visually-arresting scenarios in NanoBanana and bring them to life with Veo or Kling. These "energy-based advertisements" tell stories impossible to tell with real footage. Most useful at the top of a Meta ad creative test battery.

**Likeness and Character Creation**
NanoBanana (Flux model) can combine reference images of real people with scenario images for social content hooks. Useful for: humorous hook images, "me at [pop culture scenario]" content, product placement with human likeness. Use responsibly and in alignment with platform guidelines.

---

### Workflow Category 3: Deep Analytics

**Excel Agent Mode**
Connect your content performance data to Excel and use agent mode for analysis:
- Upload your content pillar spreadsheet (views, saves, shares, hook rate, follows generated by post)
- Run prompts: "Find the top 5 correlated metrics to view count" → reveals that shares and saves are more predictive than hook rate
- "Plan a content mix to reach X new followers given my current average per-post performance, by pillar"
- Generate full competitive scorecards: "Build a ranking system for every [product category] product in the market using criteria [list], research each one, score them, and output a ranked table I can adjust weighting on"

**Competitive Scorecard Deep Dive:**
Ask Excel agent mode to build a weighted criteria scorecard for your product category. Example workflow for a setting spray:
1. Prompt: "Create a ranking parameter system and bring in every setting spray product in the market"
2. Agent builds criteria (hold, waterproof, finish, value) with weighted scores and researches each competitor
3. Output: fully ranked table with pros/cons per product — you can then adjust the weighting live ("make value more important than hold") and the rankings update
4. Also outputs top value props and common complaints for each competitor

No manual research required. The resulting ranked table in Excel becomes a living competitive intelligence document.

This replaces analyst work that would previously require hiring a specialist or outsourcing to an agency research team.

**HubSpot Loop Prompt Library**
A structured set of AI prompts covering the full marketing loop (Express → Tailor → Amplify → Evolve):
- Behavioral segmentation builder
- Customer journey mapper
- Predictive lead scoring model prompts
- Intent signal identification (requires feeding in your own page visit, email, and sales interaction data)
- Competitor gap analysis

These prompts require you to gather real data and feed it in — they're not magic wands. But with your data input, they produce analysis that would previously cost thousands to commission from an agency.

## Real Examples
- **Beauty brand campaign research**: Used Perplexity/Comet agent mode to watch 300 TikTok creatine review videos → identified top competing brands by mention frequency, common pros/cons, and best-performing content angles → fed results directly into organic content brief and ad hook library
- **Internal brand AI clone**: Uploaded all YouTube transcripts + newsletters + reports into a ChatGPT project → team can now query for brand strategy answers and get responses eerily accurate to the creator's actual perspective. This is the "creator clone" approach — not just a brand second brain, but a personal POV replication tool for scaling your thinking across a team
- **Manis influencer research with self-serve front end**: Defined parameters (5K–200K followers, mentioned competitor brands, posted in last 30 days) → Manis returned 100–200 qualified creators → then vibe-coded a simple front-end interface inside Manis so any team member can run the search without routing through the strategist
- **Competitive setting spray scorecard**: Excel agent mode researched every setting spray brand on the market, built a weighted scoring system (hold, waterproof, finish, value), and output a ranked table with adjustable criteria weighting and per-product pros/cons
- **Hospitality consultant**: Used Excel agent mode to analyze content pillar performance monthly → discovered that shares (not views or hook rate) most correlated with new follower growth → shifted strategy accordingly
- **Leebe fourth-wall AI campaign**: Brand ran a creator-hosted series ("is this real or is it AI?") on their main feed — used AI ambiguity as the content hook itself rather than concealing or justifying AI use. Strong positive response. See [[ai-content-postures-for-brands]] for the full posture taxonomy.

## Pitfalls to Avoid
- **Trying to use AI to generate viral organic scripts** — doesn't work, produces generic content that gets ignored
- **Running fully AI-generated faceless accounts** — no affinity, no monetization
- **Obsessing over AI image perfection** — the goal is useful output fast, not technically flawless generation
- **Using AI without human editorial judgment** — AI provides raw material; a human strategist decides what to use and why
- **Not feeding real data into the analytics prompts** — these tools only work as well as the data you give them; vague inputs produce vague outputs
- **Thinking AI resistance is a strategy** — it's a trajectory toward obsolescence in any creative/marketing field

## Related Concepts: [[AI in Marketing]], [[Creator Economy in 2026]], [[exploitation-gap]], [[ai-content-postures-for-brands]], [[quiz-funnel-strategy]]
## Related Strategies: [[Short-Form Video That Makes Money]], [[Personal Branding Full Playbook]]
