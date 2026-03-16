# Research Deliverable Skills

Supporting skills for the **research-lead** agent. These skills provide structured templates and workflows for common research deliverables.

## Philosophy

The **research-lead agent** owns the METHODOLOGY of how to do research well - when to use which research methods, how to validate findings, how to structure analysis.

These **skills** own the DELIVERABLE FORMATS - structured templates for outputs that various audiences need.

**Together:** The agent provides the methodology and judgment, the skills provide the execution templates.

---

## Available Skills

### 1. competitive-analysis

**Purpose:** Create structured competitive landscape analysis reports
**Output:** Competitive analysis with feature matrices and positioning
**Audience:** Product managers, stakeholders, executives

**Use when:**
- Analyzing competitor products and features
- Creating competitive positioning assessments
- Identifying market gaps and opportunities
- Preparing stakeholder reports on competitive landscape

**Triggers:**
- "competitive analysis"
- "competitor research"
- "feature comparison"
- "market landscape"

---

### 2. market-sizing

**Purpose:** Generate TAM/SAM/SOM market opportunity analysis
**Output:** Market sizing report with methodology and projections
**Audience:** Executives, investors, product strategy team

**Use when:**
- Estimating total addressable market (TAM)
- Calculating serviceable markets (SAM/SOM)
- Building business case financial projections
- Assessing market opportunity for features or products

**Triggers:**
- "market sizing"
- "TAM SAM SOM"
- "addressable market"
- "market opportunity"

---

### 3. user-story-brief

**Purpose:** Create user-centric feature documentation
**Output:** User stories with personas, acceptance criteria, and metrics
**Audience:** Development teams, product managers, QA

**Use when:**
- Writing development-ready requirements
- Translating user research into features
- Creating acceptance criteria for sprint planning
- Documenting features for engineering handoff

**Triggers:**
- "user story"
- "acceptance criteria"
- "feature requirements"
- "user-centric documentation"

---

### 4. feature-design-doc (FDD)

**Purpose:** Comprehensive technical feasibility research for features
**Output:** Multi-audience feature documentation bridging product and engineering
**Audience:** Product managers, engineering leads, stakeholders, developers

**Use when:**
- Documenting complex features requiring cross-functional alignment
- Assessing technical feasibility before commitment
- Bridging product requirements and technical implementation
- Creating specifications for features with significant resource investment

**Triggers:**
- "feature design doc"
- "FDD"
- "technical feasibility"
- "feature specification"

---

## When to Use Which Skill

```
Research Phase              Deliverable Needed          Use Skill
────────────────────────────────────────────────────────────────────
Market Research          →  Competitor Landscape    →  competitive-analysis
Market Research          →  Opportunity Sizing     →  market-sizing
User Research            →  Dev Requirements       →  user-story-brief
Feature Definition       →  Cross-Functional Doc   →  feature-design-doc
```

---

## How Skills Pair with Research-Lead

### Research-Lead Provides:
- Research methodology guidance
- Data source validation
- Analysis frameworks
- Quality standards for research
- When to use which research method

### Skills Provide:
- Structured output templates
- Formatting conventions
- Section organization
- Calculation frameworks
- Deliverable-specific workflows

### Example Workflow:

1. **User:** "I need to analyze our competitors"
2. **Research-Lead:** Determines methodology (what to research, how to gather data, what to analyze)
3. **competitive-analysis skill:** Structures the output into standardized report format
4. **Research-Lead:** Reviews findings for analytical rigor and insight quality

---

## Skill Characteristics

All research deliverable skills share these traits:

**Multi-Audience Design:**
- Executive summaries for leadership
- Technical details for implementation teams
- Business context for product managers

**Evidence-Based:**
- Require data sources and citations
- Document methodology and assumptions
- Note limitations and caveats

**Actionable:**
- Clear recommendations or next steps
- Success metrics defined
- Open questions tracked

**Versioned:**
- Include revision history
- Track approval status
- Note next review dates

---

## Output Conventions

### File Naming
```
[deliverable-type]/[name]-[date].md

Examples:
competitive-analysis/crm-market-2026-03.md
market-sizing/tam-sam-som-2026-q1.md
user-stories/US-123-pdf-export.md
features/FDD-005-report-builder.md
```

### Status Tracking
All deliverables include status field:
- **Draft** - Work in progress
- **Review** - Ready for stakeholder review
- **Approved** - Approved for implementation/use
- **Implemented** - (For specs) Built and shipped
- **Archived** - No longer current

---

## Integration with Other Agents

These skills work well alongside:

- **research-lead** - Methodology and analysis quality
- **product-manager** - Product strategy and prioritization
- **engineering-lead** - Technical approach and feasibility
- **tech-lead** - Implementation details and architecture
- **qa-lead** - Testing strategy and acceptance criteria

---

## Future Skill Candidates

Potential additional research deliverable skills:

- **technical-spike-report** - Document results of technical research/prototyping
- **user-research-summary** - Structure interview/survey findings
- **experiment-design** - A/B test design and hypothesis documentation
- **launch-retrospective** - Post-launch analysis and learnings

---

*These skills are implementation specialists. For research methodology and strategic decisions, consult the research-lead agent.*
