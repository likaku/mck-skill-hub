# McKinsey PPT Design

> *Consultant-grade PowerPoint presentations, generated in seconds.*

## Overview

| Attribute | Value |
|-----------|-------|
| **Quadrant** | 🐹 Hollow Victory |
| **Tier** | ✅ Production |
| **Author** | Kaku |
| **Tags** | `consulting` `ppt` `design` `automation` `mckinsey` |

## What Problem Does This Solve?

Consultants spend 40-60% of their working hours on slide formatting — adjusting fonts, aligning boxes, ensuring color consistency. This skill automates the entire design layer, producing McKinsey-grade decks from structured content. **You focus on the storyline; the skill handles the pixels.**

## Quick Start

```bash
# Copy to your Claude skills directory
cp -r . ~/.claude/skills/mck-ppt-design/
```

## Usage

```
"Create a 10-slide strategy presentation for [Client Name] covering
market analysis, competitive landscape, and recommended next steps.
McKinsey style, navy and white color scheme."
```

The skill will:
1. Parse your content structure
2. Select optimal layouts for each slide
3. Apply the full McKinsey design system
4. Generate a production-ready .pptx file

## How It Works

The skill encodes a complete design specification:
- **16+ slide layout patterns** (title, agenda, two-column, big number, process flow, table+insight, etc.)
- **Strict typography hierarchy** (Georgia headers + Arial body + KaiTi Chinese)
- **Color-coded design tokens** (#051C2C Navy, #333333 Dark Gray, etc.)
- **Python-pptx code generation** with post-save cleanup to prevent file corruption

## Related Skills

- [mck-chart-design](../mck-chart-design/) — Editorial-style data visualization prompts
- [professional-speech](../professional-speech/) — Presentation talking points and structure
- [workbuddy-ppt-engine](../workbuddy-ppt-engine/) — Lower-level Python-pptx automation engine

---

*Part of the [Mck-skills](../../../README.md) gallery — Skills for a better Way of Living & Working.*
