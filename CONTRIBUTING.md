# Contributing to Mck-skills

Thank you for wanting to contribute! Every skill in this gallery exists because someone turned a frustration into a solution.

## Two Ways to Contribute

### 1. Submit a Skill Idea (No Code)

Open an [Issue](../../issues/new) using the **Skill Idea** template. Describe:
- What problem it solves
- Which quadrant it serves
- Who benefits most

### 2. Build a Full Skill

#### Quick Start

```bash
# Fork and clone
git clone https://github.com/YOUR-USERNAME/mck-skills.git
cd mck-skills

# Create from template
cp -r template/skill-template/ skills/[quadrant]/[your-skill-name]/

# Edit your SKILL.md and README.md, then submit a PR
git checkout -b skill/your-skill-name
git add .
git commit -m "feat: add your-skill-name to [quadrant]"
git push origin skill/your-skill-name
```

#### Folder Structure

```
skills/[quadrant]/[skill-name]/
├── SKILL.md          # Required — machine-readable skill definition
├── README.md         # Required — human-readable documentation
├── scripts/          # Optional — helper scripts
└── examples/         # Optional — example inputs/outputs
```

#### SKILL.md Format

```yaml
---
name: your-skill-name
description: |
  One paragraph. What does it do? When should it trigger?
quadrant: hollow-victory  # hollow-victory | purposeful-impact | the-drift | quiet-contentment
tier: beta                # production | beta | planned
author: Your Name
tags: [tag1, tag2, tag3]
---

# Skill Name

## When to Use
[Trigger conditions]

## Workflow
[Step-by-step process]

## Examples
[2-3 usage examples]
```

## Pick Your Quadrant

| Question | Quadrant |
|----------|----------|
| Does this automate busywork so I can focus on higher-value thinking? | 🐹 **Hollow Victory** |
| Does this help me build something meaningful with my skills? | 🚀 **Purposeful Impact** |
| Does this give me structure when I feel directionless? | ⚓ **The Drift** |
| Does this enrich my life outside of work? | 🕯️ **Quiet Contentment** |

## Quality Standards

- **Clear problem statement** — What specific pain does this solve?
- **Structured approach** — MECE, hypothesis-driven, or framework-based
- **Professional outputs** — Would you put this in front of a partner?
- **Tested with real use cases** — Not just theoretical
- **Well-documented** — Another person should be able to use it in 5 minutes

## PR Review

We review all PRs within **48 hours**. Criteria:

1. **Quadrant fit** — Does the skill genuinely belong where it's placed?
2. **Quality** — Is the output consulting-grade?
3. **Uniqueness** — Does it solve a problem not already covered?
4. **Documentation** — Can someone else use it immediately?

## Code of Conduct

Be excellent to each other. We're all trying to work smarter and live better.
