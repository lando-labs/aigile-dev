# AIgile Dev

**AI-Native Agile Development Plugin**

AIgile Dev brings AI-assisted agile workflows to your development process. Plan sprints, execute focused work, validate with market research, and ship with confidence.

## What's Included

### Skills

| Skill | Purpose |
|-------|---------|
| **vibecoding-sprint** | Sprint planning, execution, and close-out with semantic versioning |
| **market-research** | Focused product/market research with agile output templates |

### Agents

| Agent | Purpose |
|-------|---------|
| **product-skeptic** | BS detection and validation for research findings |
| **frontend-lead** | UI architecture, component design, UX guidance |
| **api-architect** | API design, backend services, error handling |
| **data-modeler** | Database schemas, relationships, migrations |
| **devops-guide** | Deployment, CI/CD, environment configuration |
| **qa-lead** | Test strategy, coverage decisions, quality assurance |

## Core Workflow

```
Research → Document → Plan → Execute → Ship
```

1. **Research**: Validate ideas with focused market research
2. **Document**: Capture findings as issues/features
3. **Plan**: Group into focused sprints with version targeting
4. **Execute**: Work through sprint with AI assistance
5. **Ship**: Close out with verification, tagging, and release

## Getting Started

### First Time?

Say: "Help me plan my first sprint"

AIgile will:
1. Set up the sprint directory structure
2. Walk you through key concepts
3. Create your first sprint plan

### Already Know Agile?

Quick commands:
- "Plan my next sprint"
- "Start the sprint"
- "Run the checks"
- "Close out the sprint"

## Philosophy

AIgile is:
- **SCM agnostic** - Works with GitHub, GitLab, or local-only
- **Tech stack agnostic** - Node, Python, Go, Rust, whatever
- **Methodology focused** - The process matters, tools are injectable

Configure your tooling in `.claude/sprint.config.json`:

```json
{
  "scm": {
    "provider": "github"
  },
  "closeout": {
    "test": "pytest",
    "build": "poetry build"
  }
}
```

## Skills Reference

### vibecoding-sprint

Sprint planning and execution with:
- Issue analysis and grouping
- 3-sprint planning with semver targeting
- Manifest hydration with full issue context
- Pre-close verification (tests, lint, build)
- Release tagging and archival

See `skills/vibecoding-sprint/SKILL.md`

### market-research

Focused product/market research with:
- Competitive analysis
- Market sizing
- User story validation
- Sprint goal research briefs

Outputs to agile-ready templates.

See `skills/market-research/SKILL.md`

## Agents Reference

### product-skeptic

Validates research findings with:
- Source verification
- Numbers validation
- AI slop detection
- BS detection (opinion as fact, cherry-picked data)

Use when you need a critical eye on research before acting on it.
