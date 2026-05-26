---
tags: [reference, tool, reel, storyboard, visual, layout, production]
tool_type: storyboard-generator
last_updated: 2026-05-25
---

# Reference: Reel Storyboard Tool

## Overview

A tool that generates visual storyboard layouts for reels. Takes a script or concept and outputs a structured frame-by-frame layout with visual specifications, text overlays, and production notes. Uses 12 base layout types.

---

## The 12 Layout Types

| Layout ID | Description |
|---|---|
| `split` | Vertical split — two panels side by side |
| `purple_card` | Dark purple card with centered text overlay |
| `black_split` | Black background with split content zones |
| `collage_editorial` | Editorial grid, multiple images + text |
| `full_bleed` | Full-screen image or video, minimal text |
| `dark_card_red` | Dark card with red accent — high-contrast text |
| `h_split` | Horizontal split — top/bottom panels |
| `split_rec` | Split with screen recording panel |
| `screen_rec` | Full-screen recording with overlay text |
| `vert_split_wipe` | Vertical split with animated wipe transition |
| `dark_card_black` | Black card with white text — authority mode |
| `collage_grid` | Grid collage — 4+ image tiles |

---

## The "Ace It" Process

The storyboard tool uses a playwright overlay comparison to verify visual fidelity:

1. Generate storyboard spec for each frame
2. Render the layout using the specified template
3. Compare rendered output to the reference layout via playwright overlay
4. Flag any deviation in text placement, color, or proportions
5. Iterate until overlay comparison passes

---

## Caption Emphasis Rules

Caption styling signals tone and authority:

- **Light font + bold keyword + period** = authority register
  - Example: "Deliverability *isn't* a tool problem. It's an infrastructure problem."
- **All caps word** = high-stakes emphasis; use sparingly (once per frame max)
- **Italic** = whisper/aside register; used for subtext or parenthetical
- No emoji in authority-register layouts

---

## Layout Selection Guide

| Goal | Recommended Layout |
|---|---|
| Proof/receipts (screen recording) | `screen_rec` or `split_rec` |
| Contrarian claim | `dark_card_black` or `dark_card_red` |
| Before/after comparison | `split` or `h_split` |
| Multi-point list | `collage_editorial` or `collage_grid` |
| Story-driven | `full_bleed` |
| Product reveal | `vert_split_wipe` |

---

## Integration

The storyboard tool is used downstream of the reel idea and script tools:

1. [[reel-idea-tool]] — generates and scores ideas
2. [[reel-script-tool]] — writes the script
3. **reel-storyboard-tool** — translates script into visual frames

---

## Related Pages

- [[reel-script-tool]] — generates the script this tool storyboards
- [[reel-idea-tool]] — upstream idea generation
- [[linkedin-post-tool]] — companion tool for text-only content
