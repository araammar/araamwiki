# Araamwiki — Marketing Knowledge Base

## Overview

This is a structured marketing knowledge base (wiki) powered by Claude Code. It ingests raw content (transcripts, notes, scripts, articles) and automatically organizes it into a searchable, interlinked wiki.

---

## Vault Structure

```
Araamwiki/
├── raw/                    ← Drop new files here before ingesting
├── wiki/
│   ├── brands/             ← One page per brand (voice, audience, strategy)
│   ├── scripts/            ← Every reel script, tagged by brand/hook/length/topic
│   ├── ideas/              ← Reel angles, content concepts, product ideas — scored and tagged
│   ├── campaigns/          ← Campaign docs, timelines, results, learnings
│   ├── strategies/         ← Frameworks, playbooks, research, best practices
│   ├── concepts/           ← Any concept worth capturing: marketing, psychology, culture, B2B, tech
│   ├── products/           ← One subfolder per product (overview, messaging, launch, research)
│   │   └── [product-name]/ ← e.g., caret-model/
│   ├── reference/          ← Tool documentation, system references, how-to guides
│   ├── INDEX.md            ← Master index of everything in the vault
│   └── LOG.md              ← Operation history (every ingest logged here)
├── CLAUDE.md               ← This file
```

**The vault is intentionally broad.** Ingest anything: transcripts, product docs, competitive research, audience research, launch plans, messaging frameworks, creator systems, B2B content, tools, ideas — it all belongs here if it's worth capturing.

---

## How to Ingest New Content

1. Drop your file into `/raw` (any format: .txt, .md, .pdf transcript, notes, etc.)
2. Say: `ingest [filename]`
3. Claude will:
   - Read the file from `/raw`
   - Identify all relevant entities: brands, scripts, ideas, campaigns, strategies, concepts
   - Create or update the appropriate wiki pages (never just one page — always decomposed)
   - Cross-link all related pages using `[[wiki links]]`
   - Update `INDEX.md` with all new/updated pages
   - Log the operation in `LOG.md` with timestamp, source file, and what was created/updated

### Ingest Rules Claude Follows

1. **Never create just one page** — every piece of content gets broken into the right wiki pages across the right folders
2. **Always link related pages** to each other using `[[wiki links]]`
3. **Always update INDEX.md** after every ingest
4. **Always log in LOG.md** — timestamp, file ingested, pages created/updated
5. **Tag every page** with relevant brands, topics, hook types, or campaign names
6. **Auto-create brand pages** — if a brand appears and has no page yet, create it immediately
7. **Auto-create product subfolders** — if a product is ingested, create `wiki/products/[product-name]/` and place all product pages there
8. **Use concepts/ broadly** — capture any named idea, framework, mental model, or insight worth keeping, regardless of domain (marketing, psychology, B2B, product, culture, creator systems, etc.)

---

## Page Formats by Folder

### `/wiki/brands/[BrandName].md`
```
# Brand: [Name]
tags: [brand, industry, niche]

## Voice & Tone
## Target Audience
## Brand Colors & Aesthetics
## Strategy & Positioning
## Do's
## Don'ts
## Related Scripts: [[script-links]]
## Related Campaigns: [[campaign-links]]
## Related Concepts: [[concept-links]]
```

### `/wiki/scripts/[slug].md`
```
# Script: [Title]
tags: [brand, hook-type, length, topic, format]
brand: [[BrandName]]
hook_type: [curiosity | pain-point | story | controversy | tutorial | transformation]
length: [short | medium | long] (seconds if known)
topic: [topic]

## Hook
## Body
## CTA
## Notes / Variations
## Related Ideas: [[idea-links]]
## Campaign: [[campaign-link]]
```

### `/wiki/ideas/[slug].md`
```
# Idea: [Title]
tags: [brand, topic, format, hook-type]
brand: [[BrandName]]
score: [1-10]
status: [raw | refined | scripted | produced]

## Concept
## Why It Works
## Hook Angle
## Target Audience
## Related Scripts: [[script-links]]
## Related Concepts: [[concept-links]]
```

### `/wiki/campaigns/[slug].md`
```
# Campaign: [Name]
tags: [brand, platform, goal, status]
brand: [[BrandName]]
status: [planning | active | complete]
timeline: [dates]

## Goal
## Strategy
## Content Plan
## Results & Metrics
## Learnings
## Related Scripts: [[script-links]]
## Related Strategies: [[strategy-links]]
```

### `/wiki/strategies/[slug].md`
```
# Strategy: [Title]
tags: [topic, framework, platform, brand]
applies_to: [brands or universal]

## Summary
## Framework / Steps
## When to Use
## Examples
## Related Concepts: [[concept-links]]
## Related Campaigns: [[campaign-links]]
```

### `/wiki/concepts/[slug].md`
```
# Concept: [Name]
tags: [topic, domain]

## Summary / Definition
## Why It Matters
## How It Works / The Mechanism
## What to Steal / Application
## Related Pages: [[links]]
```

*Concepts can cover any domain: marketing, psychology, culture, B2B, product, creator systems, platform mechanics, business strategy — anything worth keeping and cross-linking.*

### `/wiki/products/[product-name]/[slug].md`
```
# [Product Name] — [Doc Type]
tags: [product, topic]
product: [Product Name]
status: [planning | in-progress | live]

## [Relevant sections based on doc type]
## Related Pages: [[links]]
```

*Product docs: overview, competitive research, messaging angles, launch plans, ICP research, pricing, roadmap.*

### `/wiki/reference/[slug].md`
```
# Reference: [Tool or System Name]
tags: [reference, tool, topic]
tool_type: [type]

## Overview
## [Usage / Parameters / How It Works]
## Related Pages: [[links]]
```

---

## How to Search and Query the Vault

Tell Claude what you're looking for in plain language:

- `"Show me all scripts for [brand]"`
- `"Find all pain-point hooks we've written"`
- `"What concepts appear most in our campaigns?"`
- `"List all ideas scored 8 or above"`
- `"What do we know about [brand]'s audience?"`
- `"Show me everything related to [topic]"`
- `"Show me the Caret Model wiki"`
- `"What messaging angles do we have for [product]?"`
- `"Find all concepts about creator systems"`

Claude will search `INDEX.md`, read relevant pages, and synthesize an answer.

---

## How to Update Existing Pages

When new content is related to something already in the vault:

- Claude will detect the overlap during ingest
- It will **add** to existing pages (not overwrite them)
- It will add new links and update tags as needed
- The `LOG.md` entry will note which pages were updated vs. created

You can also manually say: `"Update [[PageName]] with this: [content]"`

---

## Tips

- The more raw content you drop in, the richer the wiki becomes
- Brand pages improve over time as more content is ingested
- Use `"review INDEX.md"` any time to get a full map of the vault
- Use `"show LOG.md"` to see the full operation history
