---
name: mck-ppt-design
description: |
  McKinsey-style PowerPoint presentation design framework with Python-pptx automation.
  Creates consultant-grade decks from scratch using a comprehensive design system
  including typography hierarchy, color palettes, layout patterns, and line treatments.
  Trigger when users need professional presentations, slide decks, or pitch materials.
quadrant: hollow-victory
tier: production
author: Kaku
tags: [consulting, ppt, design, automation, mckinsey, python-pptx]
---

# McKinsey PPT Design Skill

> *Create consultant-grade PowerPoint presentations with one prompt.*

## When to Use

Activate this skill when:

- User asks to create a McKinsey-style, BCG-style, or consultant-grade PPT
- User mentions "deck", "presentation", "slides" in a professional context
- User provides structured content (strategy, analysis, recommendations) and needs visual output
- User references "workbuddy-ppt" or "mck-ppt" design patterns

## Design System

### Color Palette

| Color | Hex | Usage |
|-------|-----|-------|
| **NAVY** | #051C2C | Primary — titles, circles, headers |
| **WHITE** | #FFFFFF | Backgrounds, text on navy |
| **BLACK** | #000000 | Lines, text separators |
| **DARK_GRAY** | #333333 | Body text |
| **MED_GRAY** | #666666 | Secondary text, labels |
| **LINE_GRAY** | #CCCCCC | Table row separators |
| **BG_GRAY** | #F2F2F2 | Background panels |

### Typography Hierarchy

| Level | Font | Size | Weight | Color |
|-------|------|------|--------|-------|
| Slide Title | Georgia | 22pt | Bold | NAVY |
| Subtitle | Arial | 18pt | Bold | DARK_GRAY |
| Body Text | Arial | 14pt | Regular | DARK_GRAY |
| Labels | Arial | 11pt | Regular | MED_GRAY |
| Source | Arial | 9pt | Italic | MED_GRAY |
| Chinese Text | KaiTi | varies | Regular | — |

### Core Principles

1. **Extreme Minimalism** — Remove all non-essential visual elements
2. **Consistency** — Repeat visual language across all slides
3. **Hierarchy** — Title 22pt → Sub 18pt → Body 14pt → Source 9pt
4. **Flat Design** — No 3D, no shadows, no gradients
5. **Rectangle-based lines** — Use `add_hline()`, NEVER `add_connector()`

## Layout Catalog (16+ patterns)

| # | Layout | Best For |
|---|--------|----------|
| 1 | Title Slide | Opening / section dividers |
| 2 | Agenda | Meeting flow overview |
| 7 | Two-Column | Side-by-side comparison |
| 8 | Big Number | Single impactful statistic |
| 10 | Process Flow | Step-by-step workflows |
| 25 | Key Takeaway | Left detail + right summary |
| 71 | Table + Insight | Structured arguments + insight panel ⭐ |

### Opening Slide Priority (Slides 2-5)

1. **Table + Insight (#71)** — structured arguments + insight panel
2. **Big Number (#8)** — single impactful statistic
3. **Key Takeaway (#25)** — left detail + right summary

## Workflow

### Step 1: Content Analysis
Parse user input for: key message, data points, structure, audience

### Step 2: Layout Selection
Match content type to optimal layout pattern

### Step 3: Design Application
Apply design system (colors, typography, spacing)

### Step 4: Python-pptx Generation
Generate production-ready .pptx file

### Step 5: Cleanup
Run `full_cleanup()` to remove theme artifacts

## Version History

| Version | Date | Changes |
|---------|------|---------|
| 2.0.4 | 2026-03-19 | #14 Three-Pillar retired → replaced by #71 Table+Insight |
| 1.1.0 | 2026-03-03 | Rectangle-based lines, three-layer corruption defense |
| 1.0.0 | 2026-03-02 | Initial specification |
