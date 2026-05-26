---
tags: [reference, tool, linkedin, copywriting, posts, hooks, engagement]
tool_type: post-generator
last_updated: 2026-05-25
---

# Reference: LinkedIn Post Tool

## Overview

A CLI tool for generating LinkedIn posts using the DNA from 100 analyzed posts across 12 top creators. Takes a topic, goal, and optional register preference and outputs a complete post with hook, body, and close — optimized for the specified engagement engine.

---

## Input Parameters

```
linkedin-post [topic] [goal] [register?] [hook_type?]
```

- **topic:** What the post is about
- **goal:** `comments` | `reposts` | `reactions`
- **register (optional):** `welsh` | `codie` | `jasmin` | `sahil` | `leila`
- **hook_type (optional):** Override the auto-selected hook type

---

## The 13 Hook Types

| # | Type | Pattern | Best For |
|---|---|---|---|
| 1 | Problem Reframe | "Most X don't have a Y problem. They have a Z problem." | Comments |
| 2 | Permission Declaration | "I'll say it so you don't have to." | Comments + Reactions |
| 3 | False Belief Reframe | "You're not afraid of X. You're afraid of Y." | Comments |
| 4 | Stakes Escalation | Small → life-defining consequence | Reactions |
| 5 | Named Framework | Proper noun label first, explanation second | Reposts |
| 6 | Anaphora List | Repeat opening phrase across 4-6 lines | Comments + Reposts |
| 7 | Business Identity Reframe | "You're not in X business. You're in Y business." | Reactions |
| 8 | Age-Bracket Targeting | "If you're in your [Xs], read this." | Comments |
| 9 | Journey Arc | Two hyper-specific data points + time gap | Reactions |
| 10 | Anti-Shortcut Declaration | State the hack doesn't exist | Comments |
| 11 | Platform Insider | "[Platform] is doing X." | Reactions |
| 12 | Single Open Question | One to three words. No setup. | Comments |
| 13 | Third-Person Proxy | "I have a friend who..." | Comments |

---

## The 7 Closing Move Types

| # | Type | Effect |
|---|---|---|
| 1 | Definitional Reframe | Most shareable — redefines a word |
| 2 | Paradox Close | Highest repost rate — two truths that seem to contradict |
| 3 | Contrast Pair | Chase vs works. No connectives. |
| 4 | Character Sketch | Invite reader to self-identify |
| 5 | Superlative Declaration | "X is the only sustainable form of Y." |
| 6 | Philosophical Elevation | Zoom from specific to universal |
| 7 | Open Question Close | A question so specific it demands a real answer |

---

## 3 Engagement Engines

### Comment-Driver
Hooks: permission_declaration, single_open_question, anaphora_list, third_person_proxy
Close: open_question_close or definitional_reframe
Rule: Never ask for comments explicitly.

### Repost-Driver
Use: paradox_close, named_framework, tricolon_escalation, anti_shortcut_declaration
Rule: Closer must work as standalone quotable sentence.

### Reactions-Driver
Use: first-person tool observation, journey_arc, stakes_escalation
Rule: Casual, specific, authoritative.

---

## 5 Creator Registers

| Register | Voice Signature |
|---|---|
| **Welsh** | Calm authority. Philosophy + business fused. Numbered lists. Stakes at life-level. Never hype. |
| **Codie** | Permission-giving. Suppressed beliefs stated unapologetically. Paradox closes. |
| **Jasmin** | Comment machine. Conversation over broadcasting. Tricolon escalation. Vulnerability as positioning. |
| **Sahil** | Named frameworks. False belief reframes. Third-person proxy. Character sketches. |
| **Leila** | Declaration mode. Superlative closers. Competence as identity. |

---

## What the Tool Will Never Write

- Explicit engagement asks ("Comment below", "Drop a like") — penalized by March 2026 Authenticity Update
- External links in post body — tool always places links in first comment
- Generic advice without specific detail
- Rounded numbers (outputs "192,138" not "190K")

---

## Source Data

DNA derived from 100 real posts across 12 creators. Full analysis: [[linkedin-post-dna]]

---

## Related Pages

- [[linkedin-post-dna]] — the full analysis this tool is built on
- [[linkedin-content-strategy-2026]] — the algorithm and platform strategy context
- [[reel-script-tool]] — parallel tool for video content
