---
tags: [reference, tool, reel, ideas, scoring, creative-strategy]
tool_type: idea-generator-and-scorer
model: claude-opus-4-5
last_updated: 2026-05-25
---

# Reference: Reel Idea Tool

## Overview

A tool that generates reel ideas from a brief and scores them against 8 criteria. Can also take an existing idea and score it, generate angle variations, or produce a full brief. Uses claude-opus-4-5 for generation.

---

## Scoring Criteria (100 points total)

| Criterion | Points | What It Measures |
|---|---|---|
| **Tension** | 20 | Does the hook create immediate friction or unresolved curiosity? |
| **Counter-intuitive** | 20 | Does it contradict what the audience already believes? |
| **Visual proof** | 15 | Can this be demonstrated visually (screen rec, side-by-side, data)? |
| **Bigger idea** | 15 | Does it point toward something larger than the specific example? |
| **Cost/time stake** | 10 | Does the viewer stand to lose something if they don't act on this? |
| **Specific audience** | 10 | Does it signal clearly who it's for (not everyone)? |
| **Timeliness** | 5 | Is this happening now, or is it evergreen? |
| **Blame reframe** | 5 | Does it shift blame from the person to a system or bad information? |

**Total:** 100 points. Anything 75+ is a strong idea. 85+ is publish-immediately territory.

---

## 4 Modes

### `full` mode
Takes a brief or topic and generates 5-8 fully scored ideas with angle variations.

Input: topic + audience + context
Output: ideas with hook options, visual proof suggestions, and score breakdown

### `angles` mode
Takes a single idea and generates 3-5 hook angle variations. Each variation targets a different hook type (see [[reel-script-tool]] hook taxonomy).

### `score` mode
Takes an existing idea (written by the user) and scores it against the 8 criteria with notes on where it's strong and where to improve.

### `brief` mode
Takes a scored idea and generates a production brief: hook, body structure, visual proof plan, CTA, estimated engagement profile.

---

## Usage

```
# Generate ideas
reel-idea [topic] [audience] [context]

# Score an existing idea
reel-idea score "[idea text]"

# Generate hook angles for an idea
reel-idea angles "[idea text]"

# Generate full production brief
reel-idea brief "[idea text]"
```

---

## Idea Quality Filters (Applied During Generation)

Ideas are filtered against these disqualifiers before scoring:

- Generic enough to apply to any creator (fails Specific Audience)
- No visual proof possible (fails Visual Proof)
- Requires 60+ seconds to set up the premise (fails Tension — hook window too slow)
- Pure information delivery with no tension or reframe (fails Counter-intuitive)

---

## High-Scoring Idea Patterns (from dataset)

- "I tested X vs Y on the same [specific thing]" — typically scores 80-90
- "[Person/role] with zero [credential signal] is outperforming [established player]" — typically scores 85+
- "You're not [stated problem]. You're [real problem]." — typically scores 80-88
- Screen recording reveals with measurable outcomes — typically scores 82-90 depending on relevance

---

## Related Pages

- [[reel-script-tool]] — downstream tool that takes scored idea to script
- [[reel-storyboard-tool]] — final stage of the production pipeline
- [[linkedin-post-dna]] — hook taxonomy that informs scoring criteria
