# AIgile Dev Glossary

Quick reference for terms used in this plugin.

## Sprint Planning

| Term | Definition |
|------|------------|
| **Sprint** | A focused work period targeting a specific version bump. Contains related issues grouped by feature or discipline. |
| **Manifest** | A markdown file documenting a sprint's scope, issues, acceptance criteria, and status. Lives in `.claude/sprints/manifests/`. |
| **Hydrate** | To fetch full issue details from GitHub and embed them in a sprint manifest. Happens when you "start the sprint". |
| **Close-out** | The workflow for completing a sprint: verify, tag, release, archive. |

## Versioning

| Term | Definition |
|------|------------|
| **Semver** | Semantic Versioning (MAJOR.MINOR.PATCH). Each sprint targets a specific version bump. |
| **MAJOR** | Breaking changes (v1.0.0 → v2.0.0). API changes, migrations, redesigns. |
| **MINOR** | New features (v1.0.0 → v1.1.0). Backwards-compatible additions. |
| **PATCH** | Bug fixes (v1.0.0 → v1.0.1). Backwards-compatible fixes. |

## Agents

| Term | Definition |
|------|------------|
| **Agent** | A Claude Code specialist with expertise in a specific domain. Owns methodology, not implementation. |
| **Roster** | The team of agents available for a project. AIgile Dev includes 7 methodology agents. |
| **Methodology** | The three-phase approach agents follow: Research → Build → Follow-up. |
| **Strategic Planner** | Agent class for cross-cutting decisions (qa-lead, devops-guide, research-lead, product-skeptic). Uses Opus model. |
| **Technology Implementer** | Agent class for domain-specific guidance (frontend-lead, api-architect, data-modeler). Uses Sonnet model. |

## Skills

| Term | Definition |
|------|------------|
| **Skill** | A workflow automation with specific triggers and outputs. Complements agents. |
| **Trigger** | A phrase that activates a skill (e.g., "plan my sprint", "competitive analysis"). |
| **Deliverable** | The structured output a skill produces (manifest, report, brief). |

## Research

| Term | Definition |
|------|------------|
| **Competitive Analysis** | Research skill for analyzing competitors and market positioning. |
| **Market Sizing** | Research skill for TAM/SAM/SOM analysis. |
| **User Story Brief** | Research skill for user-centric feature documentation. |
| **Feature Design Doc (FDD)** | Research skill for technical feasibility research bridging product and engineering. |
| **TAM** | Total Addressable Market - the full market demand for a product. |
| **SAM** | Serviceable Addressable Market - the segment you can reach. |
| **SOM** | Serviceable Obtainable Market - the realistic portion you can capture. |

## Git Workflow

| Term | Definition |
|------|------------|
| **Sprint Branch** | Branch created for sprint work: `sprint/v1.2.0-feature-name`. |
| **Branch Protection** | GitHub setting requiring PRs for main. Sprints respect this. |
| **Atomic Commit** | One commit per issue for clean rollbacks. |

## Configuration

| Term | Definition |
|------|------------|
| **sprint.config.json** | Optional config file at `.claude/sprint.config.json` for customizing closeout commands and behavior. |
| **Closeout Commands** | Commands run before closing a sprint: typecheck, lint, test, e2e, build. |
| **blockOnMissing** | Config option to require confirmation when tests aren't configured. |
