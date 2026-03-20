---
name: workbuddy-ppt-engine
description: |
  Low-level Python-pptx automation engine implementing the McKinsey design system.
  Provides ready-to-use Python code patterns for programmatic PowerPoint generation
  including layout methods, typography helpers, line drawing utilities, and corruption defense.
  Trigger when users need to generate PPT files programmatically or customize the PPT engine.
quadrant: hollow-victory
tier: production
author: Kaku
tags: [python, pptx, automation, engine, developer, mckinsey]
---

# WorkBuddy PPT Engine

> *The Python-pptx backbone powering McKinsey-grade slide generation.*

## When to Use

Activate this skill when:

- User needs to generate PPT files programmatically using Python
- User wants to customize or extend the PPT design engine
- User needs specific python-pptx code patterns (layouts, typography, lines)
- User encounters PPT corruption issues and needs the cleanup pipeline

## Architecture

```
PPT Engine
├── Design Tokens (colors, fonts, sizes)
├── Layout Methods
│   ├── eng.title_slide()
│   ├── eng.agenda()
│   ├── eng.two_column()
│   ├── eng.big_number()
│   ├── eng.process_flow()
│   ├── eng.key_takeaway()
│   └── eng.table_insight()  ⭐ (recommended)
├── Helper Utilities
│   ├── add_hline()  — rectangle-based horizontal lines
│   ├── add_text()   — typography with proper hierarchy
│   └── add_shape()  — shapes with flat design
└── Cleanup Pipeline
    └── full_cleanup()  — removes <p:style> and theme shadows
```

## Key Technical Decisions

### Lines: Rectangles, Not Connectors
```python
# ✅ CORRECT — thin rectangle
def add_hline(slide, left, top, width, color=BLACK, height=Pt(0.75)):
    shape = slide.shapes.add_shape(MSO_SHAPE.RECTANGLE, left, top, width, height)
    shape.fill.solid()
    shape.fill.fore_color.rgb = color
    shape.line.fill.background()  # No border
    return shape

# ❌ WRONG — never use connectors
# slide.shapes.add_connector(...)  # Causes rendering issues
```

### Post-Save Cleanup (Three-Layer Defense)
1. Remove `<p:style>` elements that trigger theme overrides
2. Strip shadow effects from all shapes
3. Validate XML structure for PowerPoint compatibility

## Limitations

- Requires Python 3.8+ and python-pptx library
- Complex animations not supported (static slides only)
- Chart generation uses Midjourney prompts, not embedded Excel charts
