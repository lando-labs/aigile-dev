# Market Research Skill

Focused product/market research that outputs agile-ready artifacts.

## When to Use

Use this skill when you need to:
- Validate a product idea before building
- Research competitors before planning features
- Size a market opportunity
- Back user stories with research
- Inform sprint goals with data

## Workflow

### Phase 1: Scope

Understand the question before researching:
- What decision does this inform?
- What would change your approach?
- What's the minimum viable answer?

### Phase 2: Research

Gather sources (typically 3-10):
- Web search for market data
- Competitor websites/products
- Industry reports (if provided)
- User context (if provided)

### Phase 3: Synthesize

Identify:
- **Key findings** - What sources agree on
- **Conflicts** - Where sources disagree
- **Gaps** - What we still don't know

### Phase 4: Output

Deliver to appropriate template:
- Product Brief
- Competitive Analysis
- Market Sizing
- User Story Brief
- Sprint Goal Research

## Commands

**Quick research**:
> "Research [topic] for a product brief"

**Competitive analysis**:
> "Analyze competitors for [feature/market]"

**Validate user story**:
> "Research to validate: As a [user], I want [goal]"

**Sprint goal research**:
> "Research context for sprint goal: [goal]"

## Output Templates

All outputs use templates in `templates/` directory:

| Template | Use When |
|----------|----------|
| `product-brief.md` | Informing product decisions |
| `competitive-analysis.md` | Understanding market landscape |
| `market-sizing.md` | Sizing opportunity (TAM/SAM/SOM) |
| `user-story-brief.md` | Validating user stories |
| `sprint-goal-brief.md` | Informing sprint planning |

## Integration with Sprints

Market research integrates with vibecoding-sprint:

1. Research informs issue creation
2. Findings embedded in sprint manifests
3. Gaps become research spikes
4. Conflicts flagged for decision

## Quality Standards

Every research output must include:
- [ ] Clear question being answered
- [ ] Sources cited (with links)
- [ ] Confidence level (High/Medium/Low)
- [ ] Conflicts/uncertainties noted
- [ ] Gaps identified
- [ ] Actionable recommendation

## Using with product-skeptic

After research, invoke product-skeptic to validate:
> "Validate this research with the skeptic"

The skeptic will check:
- Do sources actually say what we claim?
- Are numbers plausible?
- Is this substantive or impressive-sounding fluff?
