---
name: market-sizing
description: Generate TAM/SAM/SOM market opportunity analysis reports with sizing methodology, assumptions, and financial projections. Use when estimating market size, calculating TAM SAM SOM, assessing market opportunity, or when the user asks for market sizing analysis, addressable market calculations, or opportunity assessment deliverables.
allowed-tools: Read, Grep, Glob, Write, WebSearch
---

# Market Sizing Report Generator

## Voice
Read and embody: `reference/voice/scout-persona.md`

## Purpose
Provides structured templates and calculation frameworks for market sizing analysis. Outputs standardized TAM/SAM/SOM reports with methodology documentation, assumptions, and market opportunity assessments.

## Pairs Well With
- `research-lead` - For research methodology, data source validation, and analytical rigor
- `product-manager` - For market selection decisions and go-to-market strategy

## When This Skill Activates

- User requests "market sizing" or "TAM SAM SOM analysis"
- Calculating total addressable market (TAM)
- Estimating serviceable addressable market (SAM)
- Projecting serviceable obtainable market (SOM)
- Preparing market opportunity reports for executives or investors
- Building business case financial projections

## Capabilities

### Market Sizing Report Structure

Generates comprehensive market sizing reports with these sections:

1. **Executive Summary** - Market opportunity at a glance
2. **Market Definition** - Scope, boundaries, and segmentation
3. **TAM Analysis** - Total addressable market calculation
4. **SAM Analysis** - Serviceable addressable market refinement
5. **SOM Projection** - Serviceable obtainable market target
6. **Methodology & Assumptions** - How numbers were derived
7. **Growth Projections** - Market trends and future outlook
8. **Strategic Implications** - What the numbers mean for business

### TAM/SAM/SOM Framework

**TAM (Total Addressable Market)**
- The total revenue opportunity if you achieved 100% market share
- Answers: "How big is the universe?"

**SAM (Serviceable Addressable Market)**
- The portion of TAM you can realistically serve with your product/service
- Answers: "How much can we actually reach?"

**SOM (Serviceable Obtainable Market)**
- The realistic share you can capture in the near term (1-3 years)
- Answers: "What's our target?"

### Calculation Methods

**Top-Down Approach:**
- Start with total market size from industry reports
- Apply filters and constraints to narrow down

**Bottom-Up Approach:**
- Start with unit economics and customer counts
- Build up from fundamental drivers

**Value Theory Approach:**
- Calculate value delivered to customers
- Estimate pricing based on value capture

## Output Template

```markdown
# Market Sizing Analysis: [Product/Market Name]

**Date:** [Date]
**Analyst:** [Name]
**Audience:** Executives, investors, product strategy team

---

## Executive Summary

**Market Opportunity:**
- **TAM:** $[X]B - [Brief description]
- **SAM:** $[X]M - [Brief description]
- **SOM (Year 1):** $[X]M - [Brief description]
- **SOM (Year 3):** $[X]M - [Brief description]

**Key Insights:**
- [Insight 1 - e.g., "Market growing at 25% CAGR"]
- [Insight 2 - e.g., "Underserved segment represents 40% of SAM"]
- [Insight 3 - e.g., "Early mover advantage window: 18-24 months"]

**Strategic Recommendation:**
[One paragraph on what this market sizing means for go/no-go decision]

---

## Market Definition

### Scope & Boundaries

**Market Category:** [e.g., "SaaS project management tools"]

**Geographic Scope:** [e.g., "North America initially, global expansion planned"]

**Customer Segments Included:**
- [Segment 1 - e.g., "Software development teams (5-50 people)"]
- [Segment 2]
- [Segment 3]

**Exclusions:**
- [What's explicitly not included and why]

### Market Segmentation

| Segment | Description | Size Estimate | Priority |
|---------|-------------|---------------|----------|
| [Segment A] | [Description] | [% of market] | High/Med/Low |
| [Segment B] | [Description] | [% of market] | High/Med/Low |
| [Segment C] | [Description] | [% of market] | High/Med/Low |

---

## TAM Analysis - Total Addressable Market

### Calculation Method: [Top-Down / Bottom-Up / Value Theory]

**Top-Down Calculation:**

```
Total Market Size (Industry)          = $[X]B
× Relevant Segment %                  = [X]%
× Geographic Coverage                 = [X]%
= TAM                                 = $[X]B
```

**Bottom-Up Validation:**

```
Total Potential Customers             = [X] companies/users
× Average Annual Contract Value (ACV) = $[X]
= TAM                                 = $[X]B
```

### TAM Breakdown

| Market Component | Value | % of TAM | Notes |
|-----------------|-------|----------|-------|
| [Component 1] | $[X]B | [X]% | [Context] |
| [Component 2] | $[X]M | [X]% | [Context] |
| [Component 3] | $[X]M | [X]% | [Context] |
| **Total TAM** | **$[X]B** | **100%** | |

### Data Sources

- [Source 1 - e.g., "Gartner Market Analysis 2026"]
- [Source 2 - e.g., "CB Insights Funding Data"]
- [Source 3 - e.g., "Primary research survey (n=500)"]

---

## SAM Analysis - Serviceable Addressable Market

### Refinement Factors

**What reduces TAM to SAM:**

1. **Geographic Constraints**
   - TAM includes: [e.g., "Global market"]
   - We can serve: [e.g., "North America only in Year 1"]
   - Reduction: [X]%

2. **Product-Market Fit Constraints**
   - TAM includes: [e.g., "All company sizes"]
   - We target: [e.g., "Mid-market (50-500 employees)"]
   - Reduction: [X]%

3. **Distribution Constraints**
   - TAM includes: [e.g., "All channels"]
   - We can reach: [e.g., "Online/self-serve only"]
   - Reduction: [X]%

4. **Pricing/Budget Constraints**
   - TAM includes: [e.g., "All budget levels"]
   - We fit: [e.g., "$10K+ annual budgets"]
   - Reduction: [X]%

### SAM Calculation

```
TAM                                   = $[X]B
× Geographic Filter                   = [X]%
× Target Segment Filter               = [X]%
× Distribution Channel Filter         = [X]%
× Budget/Pricing Filter               = [X]%
= SAM                                 = $[X]M
```

### SAM Breakdown by Segment

| Segment | TAM Portion | Filters Applied | SAM | Priority |
|---------|-------------|-----------------|-----|----------|
| [Segment A] | $[X]M | [X]% reachable | $[X]M | High |
| [Segment B] | $[X]M | [X]% reachable | $[X]M | Medium |
| **Total** | **$[X]M** | | **$[X]M** | |

---

## SOM Projection - Serviceable Obtainable Market

### Realistic Market Capture

**What we can actually win in the near term:**

### Year 1 Projection

**Target Market Share:** [X]% of SAM

**Calculation:**
```
SAM                                   = $[X]M
× Year 1 Market Share Target          = [X]%
= Year 1 SOM                          = $[X]M
```

**Underlying Assumptions:**
- Customer acquisition: [X] customers in Year 1
- Average ACV: $[X]
- Sales efficiency: [X] months avg sales cycle

**Bottlenecks/Constraints:**
- [e.g., "Sales team capacity: 2 AEs can close ~50 deals/year"]
- [e.g., "Product readiness: MVP suitable for early adopters only"]

### Year 3 Projection

**Target Market Share:** [X]% of SAM

**Calculation:**
```
SAM (projected growth)                = $[X]M
× Year 3 Market Share Target          = [X]%
= Year 3 SOM                          = $[X]M
```

**Growth Assumptions:**
- Customer base: [X] customers by Year 3
- Average ACV growth: $[X] → $[X]
- Market share progression: [Y1: X%] → [Y2: X%] → [Y3: X%]

### SOM Sensitivity Analysis

| Scenario | Market Share | SOM (Year 3) | Probability |
|----------|--------------|--------------|-------------|
| Conservative | [X]% | $[X]M | [X]% |
| Base Case | [X]% | $[X]M | [X]% |
| Optimistic | [X]% | $[X]M | [X]% |

---

## Methodology & Assumptions

### Data Collection Methods

**Primary Research:**
- [Method 1 - e.g., "Customer interviews (n=50)"]
- [Method 2 - e.g., "Survey of target segment (n=500)"]

**Secondary Research:**
- [Source 1 - e.g., "Industry analyst reports (Gartner, Forrester)"]
- [Source 2 - e.g., "Competitor financial disclosures"]
- [Source 3 - e.g., "Government/trade association data"]

### Key Assumptions

**Market Assumptions:**
- Market growth rate: [X]% CAGR (source: [source])
- Customer budget allocation: [assumption]
- Competitive dynamics: [assumption]

**Product Assumptions:**
- Product-market fit: [assumption]
- Pricing strategy: [assumption]
- Distribution efficiency: [assumption]

**Business Assumptions:**
- Sales team ramp: [assumption]
- Customer acquisition cost (CAC): $[X]
- Customer lifetime value (LTV): $[X]
- LTV:CAC ratio: [X:1]

### Limitations & Caveats

- **Data gaps:** [What data was unavailable or estimated]
- **Market volatility:** [Factors that could change quickly]
- **Competitive response:** [How competitors might react]
- **Technology shifts:** [Potential disruptions]

---

## Growth Projections

### Market Trends

**Historical Growth:**
- [Time period]: Market grew from $[X] to $[X] ([X]% CAGR)

**Projected Growth:**
- Next 3 years: $[X] → $[X] ([X]% CAGR)
- Drivers: [Key growth drivers]

### Market Maturity

**Current Stage:** [Emerging / Growth / Mature / Declining]

**Indicators:**
- [Indicator 1 - e.g., "Funding activity increasing 40% YoY"]
- [Indicator 2 - e.g., "New entrants joining market quarterly"]
- [Indicator 3]

### Expansion Opportunities

**Adjacent Markets:**
- [Market 1]: Additional TAM of $[X]
- [Market 2]: Additional TAM of $[X]

**Geographic Expansion:**
- [Region 1]: Adds $[X] to SAM
- [Region 2]: Adds $[X] to SAM

---

## Strategic Implications

### Market Attractiveness

**Positives:**
- [e.g., "Large TAM ($XB) with high growth (X% CAGR)"]
- [e.g., "Underserved segment represents significant opportunity"]
- [e.g., "Early market stage allows for category definition"]

**Challenges:**
- [e.g., "Competitive landscape is crowded"]
- [e.g., "Customer acquisition costs are high"]
- [e.g., "Market education required"]

### Go-to-Market Implications

**Recommended Strategy:**
- **Initial Focus:** [Which segment of SAM to target first]
- **Expansion Path:** [How to grow from SOM to larger SAM capture]
- **Resource Requirements:** [What's needed to achieve SOM targets]

**Investment Requirements:**
- Sales/marketing: $[X] to achieve Year 1 SOM
- Product development: $[X] to serve SAM effectively
- Total capital: $[X] over [X] years

### Risk Assessment

| Risk | Impact | Mitigation |
|------|--------|------------|
| [Risk 1] | High/Med/Low | [Strategy] |
| [Risk 2] | High/Med/Low | [Strategy] |

---

## Appendix

### Calculation Details

**Detailed TAM Calculation:**
```
[Step-by-step breakdown of all calculations]
```

**Detailed SAM Calculation:**
```
[Step-by-step breakdown of all calculations]
```

**Detailed SOM Calculation:**
```
[Step-by-step breakdown of all calculations]
```

### Data Sources Bibliography

1. [Full citation]
2. [Full citation]
3. [Full citation]

### Competitive Benchmarks

| Competitor | Reported Revenue | Estimated Market Share | Customer Count |
|------------|------------------|------------------------|----------------|
| [Company A] | $[X]M | [X]% | [X] |
| [Company B] | $[X]M | [X]% | [X] |

---

**Last Updated:** [Date]
**Next Review:** [Recommended review date - typically quarterly]
**Version:** [Version number]
```

---

## Workflows

### Creating a Market Sizing Report

1. **Define Market Scope**
   - Identify product/service category
   - Set geographic boundaries
   - Define customer segments

2. **Calculate TAM**
   - Gather industry data (top-down)
   - Calculate from first principles (bottom-up)
   - Validate with multiple methods

3. **Refine to SAM**
   - Identify realistic constraints
   - Apply filters sequentially
   - Document each reduction

4. **Project SOM**
   - Estimate realistic market share
   - Account for sales/distribution capacity
   - Create sensitivity scenarios

5. **Document Methodology**
   - Record all data sources
   - List key assumptions
   - Note limitations and caveats

6. **Generate Report**
   - Use template above
   - Include executive summary
   - Add visual representations if helpful

7. **Review & Validate**
   - Sanity check: Does SOM seem achievable?
   - Compare to competitor performance
   - Validate with research-lead for methodology

### Common Calculation Patterns

**SaaS Business:**
```
TAM = Total target companies × Average ACV
SAM = Companies matching ICP × Average ACV
SOM = Realistic customer acquisitions × Average ACV
```

**Consumer Product:**
```
TAM = Total addressable users × Average annual spend
SAM = Users in target demographics × Average annual spend
SOM = Realistic user acquisition × Average annual spend × Conversion rate
```

**Usage-Based Pricing:**
```
TAM = Total usage volume × Price per unit
SAM = Addressable usage volume × Price per unit
SOM = Realistic captured volume × Price per unit
```

---

## Limitations

- Does NOT make strategic decisions about market entry (consult product-manager)
- Does NOT determine research methodology or data source validity (consult research-lead)
- Does NOT create financial models beyond market sizing (consult financial planning team)
- Provides calculation frameworks and templates, not market analysis expertise

---

## Output Locations

Save market sizing reports to:
- `research/market-sizing/[market-name]-[date].md`
- `docs/business-case/market-analysis.md`
- Or location specified by user

Include date in filename for version tracking.
