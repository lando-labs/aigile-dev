---
name: competitive-analysis
description: Create structured competitive landscape analysis reports with positioning matrices, feature comparisons, and opportunity identification. Use when analyzing competitors, creating competitive positioning, comparing product features, or when the user asks for competitive analysis, market landscape assessment, or competitor research deliverables.
allowed-tools: Read, Grep, Glob, Write, WebSearch
---

# Competitive Analysis Report Generator

## Voice
Read and embody: `reference/voice/scout-persona.md`

## Purpose
Provides structured templates and workflows for creating competitive analysis reports. Outputs standardized reports with feature comparison matrices, competitive positioning, and strategic opportunity identification.

## Pairs Well With
- `research-lead` - For research methodology, analysis frameworks, and strategic guidance
- `product-manager` - For product positioning decisions and feature prioritization

## When This Skill Activates

- User requests "competitive analysis" or "competitor research"
- Creating competitive landscape assessments
- Building feature comparison matrices
- Analyzing market positioning
- Identifying competitive gaps and opportunities
- Preparing reports for product managers or stakeholders

## Capabilities

### Competitive Analysis Report Structure

Generates comprehensive competitive analysis reports with these sections:

1. **Executive Summary** - Key findings and strategic implications
2. **Competitive Landscape** - Players identified and categorized
3. **Feature Comparison Matrix** - Side-by-side capability assessment
4. **Positioning Analysis** - Strategic positioning of each competitor
5. **Gaps & Opportunities** - Market whitespace and differentiation opportunities
6. **Strategic Recommendations** - Actionable next steps

### Feature Comparison Matrix

Creates structured comparison tables:

| Feature/Capability | Our Product | Competitor A | Competitor B | Competitor C |
|-------------------|-------------|--------------|--------------|--------------|
| [Feature 1] | ✅ Advanced | ✅ Basic | ❌ None | ✅ Advanced |
| [Feature 2] | ✅ Basic | ✅ Advanced | ✅ Basic | ✅ Advanced |

Legend:
- ✅ Advanced: Full-featured implementation
- ✅ Basic: Limited implementation
- ⚠️ Partial: In development or incomplete
- ❌ None: Not available

### Positioning Matrix

Generates 2x2 positioning visualizations using text-based representations or recommendations for visual tools.

## Output Template

```markdown
# Competitive Analysis: [Product/Market Name]

**Date:** [Date]
**Analyst:** [Name]
**Audience:** Product managers, stakeholders, executives

---

## Executive Summary

[2-3 paragraphs summarizing key findings, competitive threats, and strategic opportunities]

**Key Findings:**
- [Finding 1]
- [Finding 2]
- [Finding 3]

---

## Competitive Landscape

### Market Overview
[Description of the competitive landscape, market maturity, and key dynamics]

### Competitors Identified

#### Tier 1: Direct Competitors
- **[Competitor Name]** - [Brief description, market position, key strengths]
- **[Competitor Name]** - [Brief description, market position, key strengths]

#### Tier 2: Indirect Competitors
- **[Competitor Name]** - [Brief description, overlap areas]

#### Tier 3: Potential Entrants
- **[Company/Category]** - [Why they might enter, threat level]

---

## Feature Comparison Matrix

### Core Capabilities

| Feature/Capability | Our Product | [Competitor A] | [Competitor B] | [Competitor C] |
|-------------------|-------------|----------------|----------------|----------------|
| [Category 1] | | | | |
| - [Feature 1.1] | ✅ Advanced | ✅ Basic | ❌ None | ✅ Advanced |
| - [Feature 1.2] | ✅ Basic | ✅ Advanced | ✅ Basic | ⚠️ Partial |
| [Category 2] | | | | |
| - [Feature 2.1] | ✅ Advanced | ❌ None | ✅ Basic | ✅ Basic |

### Differentiation Assessment

**Our Strengths:**
- [Unique capability or advantage]
- [Unique capability or advantage]

**Competitive Advantages (others):**
- **[Competitor]:** [Their unique strength]
- **[Competitor]:** [Their unique strength]

---

## Positioning Analysis

### Strategic Positioning

**Positioning Dimensions:**
- **Axis 1:** [e.g., Price - Low to High]
- **Axis 2:** [e.g., Feature Completeness - Basic to Advanced]

**Quadrant Placement:**

```
High Features
    |
    | [Competitor C]
    |           [Our Product]
    |
    | [Competitor B]
Low Price ----+---- High Price
    |
    | [Competitor A]
    |
    |
Low Features
```

### Market Segmentation

| Segment | Primary Players | Our Position | Opportunity |
|---------|----------------|--------------|-------------|
| Enterprise | [Competitors] | [Current position] | [Gap/Opportunity] |
| Mid-Market | [Competitors] | [Current position] | [Gap/Opportunity] |
| SMB | [Competitors] | [Current position] | [Gap/Opportunity] |

---

## Gaps & Opportunities

### Market Whitespace

**Underserved Segments:**
- [Segment description and why it's underserved]

**Missing Capabilities:**
- [Capability gap in the market]

### Competitive Advantages to Exploit

1. **[Advantage Area]**
   - What we have: [Our capability]
   - What they lack: [Competitor gap]
   - Opportunity: [How to leverage]

2. **[Advantage Area]**
   - What we have: [Our capability]
   - What they lack: [Competitor gap]
   - Opportunity: [How to leverage]

### Threats to Address

1. **[Threat Area]**
   - Competitor: [Who poses threat]
   - Their advantage: [What they have]
   - Our gap: [What we lack]
   - Mitigation: [How to address]

---

## Strategic Recommendations

### Immediate Actions (0-3 months)
1. [Recommendation with rationale]
2. [Recommendation with rationale]

### Near-term Initiatives (3-6 months)
1. [Recommendation with rationale]
2. [Recommendation with rationale]

### Long-term Strategy (6-12 months)
1. [Recommendation with rationale]
2. [Recommendation with rationale]

---

## Appendix

### Research Methodology
[How data was gathered, sources used, limitations]

### Data Sources
- [Source 1]
- [Source 2]

### Assumptions & Caveats
- [Assumption/limitation]

---

**Last Updated:** [Date]
**Next Review:** [Recommended review date]
```

---

## Workflows

### Creating a Competitive Analysis Report

1. **Gather Requirements**
   - Identify target market/product category
   - Define comparison dimensions (features, pricing, positioning)
   - Determine audience and report purpose

2. **Research Competitors**
   - Identify direct and indirect competitors
   - Gather feature lists, pricing, positioning materials
   - Document sources and evidence

3. **Build Feature Matrix**
   - Categorize features into logical groups
   - Assess each competitor's capability level
   - Note unique differentiators

4. **Analyze Positioning**
   - Map competitors on relevant dimensions
   - Identify strategic clusters
   - Note market gaps

5. **Generate Report**
   - Use the output template above
   - Fill in all sections with research findings
   - Include executive summary with key insights

6. **Review & Refine**
   - Validate findings with research-lead for methodology
   - Check for gaps in analysis
   - Ensure recommendations are actionable

### Updating an Existing Analysis

1. **Review previous analysis** - Understand baseline
2. **Identify changes** - New competitors, feature updates, positioning shifts
3. **Update affected sections** - Matrix, positioning, recommendations
4. **Document changes** - What changed and why it matters
5. **Update metadata** - Date, next review date

---

## Limitations

- Does NOT make strategic decisions about which competitors to prioritize (consult research-lead or product-manager)
- Does NOT determine research methodology (consult research-lead)
- Does NOT make product roadmap decisions based on competitive gaps (consult product-manager)
- Provides structure and templates, not research execution or analysis frameworks

---

## Output Locations

Save competitive analysis reports to:
- `research/competitive-analysis/[product-name]-[date].md`
- `docs/competitive/[product-name]-analysis.md`
- Or location specified by user

Include version date in filename for tracking updates over time.
