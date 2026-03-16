---
name: feature-design-doc
description: Create comprehensive Feature Design Documents (FDDs) with technical feasibility research, executive summaries, problem analysis, implementation approaches, and resource requirements. Use when documenting features for cross-functional teams, assessing technical feasibility, bridging product and engineering, or when the user asks for feature design docs, technical feasibility analysis, or feature specification deliverables.
allowed-tools: Read, Grep, Glob, Write, WebSearch
---

# Feature Design Document (FDD) Generator

## Voice
Read and embody: `reference/voice/scout-persona.md`

## Purpose
Provides structured templates for comprehensive Feature Design Documents that bridge product and engineering. Outputs multi-audience documentation with executive summaries, problem analysis, technical approaches, feasibility assessments, and resource requirements.

## Pairs Well With
- `research-lead` - For research methodology and technical feasibility validation
- `product-manager` - For product strategy and business case decisions
- `engineering-lead` - For technical approach and architecture decisions
- `tech-lead` - For implementation details and code-level design

## When This Skill Activates

- User requests "feature design doc" or "FDD"
- Documenting technical feasibility for product proposals
- Creating cross-functional feature specifications
- Bridging product requirements and engineering implementation
- Preparing comprehensive feature documentation for stakeholders
- Assessing feasibility before committing to development

## Capabilities

### Feature Design Document Structure

Generates comprehensive FDDs with these sections:

1. **Executive Summary** - For stakeholders and leadership
2. **Problem & Opportunity** - For product managers
3. **Proposed Solution** - For all audiences
4. **Technical Approach** - For engineering teams
5. **Feasibility Assessment** - For decision makers
6. **Resource Requirements** - For planning
7. **Success Metrics** - For measurement
8. **Risks & Mitigations** - For risk management
9. **Open Questions** - For resolution tracking
10. **Appendices** - For detailed reference

### Multi-Audience Design

**Stakeholders/Executives** → Executive Summary, Business Value, Resource Requirements
**Product Managers** → Problem/Opportunity, Success Metrics, User Impact
**Engineering Leads** → Technical Approach, Feasibility, Dependencies
**Individual Contributors** → Implementation Details, API Specs, Data Models

### Feasibility Assessment Framework

Evaluates features across dimensions:
- **Technical Complexity:** Low / Medium / High
- **Risk Level:** Low / Medium / High
- **Dependencies:** Internal / External / None
- **Timeline Estimate:** Days / Weeks / Months
- **Resource Requirements:** Team size and composition

## Output Template

```markdown
# Feature Design Document: [Feature Name]

**Document ID:** FDD-[ID]
**Status:** [Draft / Review / Approved / Implemented]
**Created:** [Date]
**Author:** [Name, Role]
**Last Updated:** [Date]

---

## Document Summary

| Field | Value |
|-------|-------|
| **Feature Name** | [Descriptive name] |
| **Target Release** | [Version or date] |
| **Priority** | [P0 / P1 / P2 / P3] |
| **Complexity** | [Low / Medium / High] |
| **Estimated Effort** | [e.g., "2-3 weeks, 2 engineers"] |
| **Status** | [Draft / Review / Approved / In Progress / Shipped] |

**Quick Links:**
- Related User Stories: [US-XXX]
- Design Mockups: [Link]
- Technical Spike: [Link]
- Project Tracker: [Link]

---

## Executive Summary

[2-3 paragraph overview targeting executives and stakeholders who may only read this section]

**Problem:**
[One sentence: What problem are we solving?]

**Solution:**
[One sentence: What are we building?]

**Why Now:**
[One sentence: Why is this important now?]

**Impact:**
- **Users:** [e.g., "Reduces task completion time by 40%"]
- **Business:** [e.g., "Expected to increase conversion by 15%"]
- **Technical:** [e.g., "Reduces infrastructure costs by $X/month"]

**Resource Ask:**
- [X] engineers for [Y] weeks
- [Budget if applicable]
- [Other resources needed]

**Recommendation:**
[Go / No-Go / Needs More Research] - [One sentence justification]

---

## Problem & Opportunity

### Current State

**What exists today:**
[Describe current situation, workarounds, or limitations]

**Pain Points:**
1. **[Pain Point 1]**
   - **Who:** [Affected users/stakeholders]
   - **Frequency:** [How often this occurs]
   - **Impact:** [Business or user impact]
   - **Evidence:** [Data, research findings, or quotes]

2. **[Pain Point 2]**
   - **Who:** [Affected users/stakeholders]
   - **Frequency:** [How often this occurs]
   - **Impact:** [Business or user impact]
   - **Evidence:** [Data, research findings, or quotes]

### Market Context

**Competitive Landscape:**
- [How competitors handle this]
- [Market expectations or standards]
- [Gaps or opportunities]

**User Research:**
- [Summary of relevant user research]
- [Number of users affected or requesting]
- [Quotes or testimonials]

### Opportunity

**Business Value:**
- **Revenue:** [Impact on revenue - direct or indirect]
- **Retention:** [Impact on churn or engagement]
- **Acquisition:** [Impact on new user growth]
- **Efficiency:** [Cost savings or productivity gains]

**Strategic Alignment:**
- [How this aligns with company/product strategy]
- [What this enables for future roadmap]

**Cost of Inaction:**
- [What happens if we don't build this]
- [Competitive risk, user churn, missed opportunity]

---

## Proposed Solution

### Overview

[2-3 paragraph description of the proposed feature]

### User Experience

**User Flow:**

```
[User Journey]
1. Entry Point → [Where user starts]
2. Action 1 → [What user does and sees]
3. Action 2 → [What user does and sees]
4. Completion → [End state and outcome]
```

**Key Interactions:**
- [Interaction 1 and behavior]
- [Interaction 2 and behavior]

**UI/UX Highlights:**
- [Notable design decision 1]
- [Notable design decision 2]

### Functional Requirements

**Must Have (P0):**
- [Requirement 1]
- [Requirement 2]

**Should Have (P1):**
- [Requirement 1]
- [Requirement 2]

**Nice to Have (P2):**
- [Requirement 1]
- [Requirement 2]

**Out of Scope:**
- [Explicitly not included - may be future iteration]

### Non-Functional Requirements

**Performance:**
- [e.g., "API response time < 200ms at p95"]
- [e.g., "Page load time < 2s"]

**Scalability:**
- [e.g., "Support 10K concurrent users"]
- [e.g., "Handle 1M records"]

**Availability:**
- [e.g., "99.9% uptime"]

**Security:**
- [e.g., "PII encryption at rest and in transit"]
- [e.g., "Role-based access control"]

**Accessibility:**
- [e.g., "WCAG 2.1 AA compliance"]

**Compatibility:**
- [e.g., "Support Chrome, Firefox, Safari (last 2 versions)"]

---

## Technical Approach

### Architecture Overview

**High-Level Design:**

```
[Architectural diagram in text form or link to diagram]

┌─────────────┐
│   Client    │
│  (React)    │
└──────┬──────┘
       │ HTTPS
       ▼
┌─────────────┐
│   API GW    │
│  (Node.js)  │
└──────┬──────┘
       │
       ▼
┌─────────────┐     ┌─────────────┐
│  Service A  │────▶│  Database   │
│  (Go)       │     │  (Postgres) │
└─────────────┘     └─────────────┘
```

**Key Components:**

1. **[Component Name]**
   - **Purpose:** [What it does]
   - **Technology:** [Stack/framework]
   - **Responsibilities:** [Key functions]
   - **Interfaces:** [APIs, events, data flows]

2. **[Component Name]**
   - **Purpose:** [What it does]
   - **Technology:** [Stack/framework]
   - **Responsibilities:** [Key functions]
   - **Interfaces:** [APIs, events, data flows]

### Data Model

**New Entities:**

```typescript
// Example data model
interface FeatureEntity {
  id: string;
  userId: string;
  attribute1: string;
  attribute2: number;
  createdAt: Date;
  updatedAt: Date;
}
```

**Database Schema Changes:**

```sql
-- New tables
CREATE TABLE feature_table (
  id UUID PRIMARY KEY,
  user_id UUID REFERENCES users(id),
  attribute1 VARCHAR(255),
  created_at TIMESTAMP DEFAULT NOW()
);

-- Indexes
CREATE INDEX idx_feature_user ON feature_table(user_id);

-- Migrations needed
ALTER TABLE existing_table ADD COLUMN new_field VARCHAR(100);
```

**Data Volume Estimates:**
- Initial: [X records/day, Y GB storage]
- 1 Year: [X records/day, Y GB storage]
- Growth rate: [X% monthly]

### API Specifications

**New Endpoints:**

```
POST /api/v1/feature
GET /api/v1/feature/:id
PUT /api/v1/feature/:id
DELETE /api/v1/feature/:id
```

**Example Request/Response:**

```json
// POST /api/v1/feature
Request:
{
  "attribute1": "value",
  "attribute2": 123
}

Response (201 Created):
{
  "id": "uuid",
  "attribute1": "value",
  "attribute2": 123,
  "createdAt": "2026-03-15T10:00:00Z"
}
```

**Error Handling:**
- [Error scenario 1 and response]
- [Error scenario 2 and response]

### Technology Stack

**Frontend:**
- [Framework/library - e.g., "React 18"]
- [Key dependencies - e.g., "TanStack Query for data fetching"]
- [Build tools - e.g., "Vite"]

**Backend:**
- [Language/framework - e.g., "Node.js with Express"]
- [Key libraries - e.g., "Prisma ORM"]

**Infrastructure:**
- [Hosting - e.g., "Vercel for frontend, Cloud Run for backend"]
- [Database - e.g., "Cloud SQL (PostgreSQL 15)"]
- [Other services - e.g., "Cloud Storage for file uploads"]

**New Dependencies:**
- [Library 1 - e.g., "pdf-lib for PDF generation (MIT license)"]
- [Library 2 - justification if new]

### Implementation Approach

**Phase 1: [Phase Name] (Week 1-2)**
- [Task 1]
- [Task 2]
- **Deliverable:** [What's done]
- **Risk:** [Any risks in this phase]

**Phase 2: [Phase Name] (Week 3-4)**
- [Task 1]
- [Task 2]
- **Deliverable:** [What's done]
- **Risk:** [Any risks in this phase]

**Phase 3: [Phase Name] (Week 5-6)**
- [Task 1]
- [Task 2]
- **Deliverable:** [What's done]
- **Risk:** [Any risks in this phase]

### Testing Strategy

**Unit Tests:**
- [Coverage target - e.g., ">80% for new code"]
- [Key areas to test]

**Integration Tests:**
- [API contract tests]
- [Database integration tests]

**E2E Tests:**
- [Critical user flows to cover]
- [Tools - e.g., "Playwright"]

**Performance Tests:**
- [Load testing approach]
- [Benchmarks to validate]

**Security Tests:**
- [Authentication/authorization scenarios]
- [Input validation tests]

---

## Feasibility Assessment

### Technical Complexity

**Rating:** [Low / Medium / High]

**Complexity Factors:**

| Factor | Level | Notes |
|--------|-------|-------|
| **Architecture Changes** | Low/Med/High | [e.g., "Requires new microservice"] |
| **Data Migration** | Low/Med/High | [e.g., "Backfill 10M records"] |
| **Third-Party Integration** | Low/Med/High | [e.g., "New payment provider"] |
| **Performance Optimization** | Low/Med/High | [e.g., "Query optimization needed"] |
| **Security Requirements** | Low/Med/High | [e.g., "PII handling, compliance"] |

**Overall Complexity Justification:**
[Why this rating? What makes it complex or straightforward?]

### Dependencies

**Internal Dependencies:**

| Dependency | Owner | Status | Risk |
|------------|-------|--------|------|
| [System/Team A] | [Team name] | [Ready/In Progress/Blocked] | Low/Med/High |
| [System/Team B] | [Team name] | [Ready/In Progress/Blocked] | Low/Med/High |

**External Dependencies:**

| Dependency | Vendor/Service | Status | Risk |
|------------|----------------|--------|------|
| [Third-party API] | [Provider] | [Available/TBD] | Low/Med/High |
| [Tool/Library] | [Name] | [Stable/Beta] | Low/Med/High |

**Blocking Items:**
- [Critical dependency that must be resolved before starting]

### Risks

| Risk | Probability | Impact | Mitigation |
|------|-------------|--------|------------|
| [Risk 1] | High/Med/Low | High/Med/Low | [Strategy] |
| [Risk 2] | High/Med/Low | High/Med/Low | [Strategy] |
| [Risk 3] | High/Med/Low | High/Med/Low | [Strategy] |

**Example:**
| Risk | Probability | Impact | Mitigation |
|------|-------------|--------|------------|
| Third-party API rate limits | High | Medium | Implement caching layer, negotiate higher limits |
| Data migration fails | Low | High | Dry-run migration in staging, build rollback plan |
| Performance at scale | Medium | High | Load test early, plan for horizontal scaling |

### Unknowns & Research Needed

**Technical Spikes Required:**
- [ ] [Spike 1 - e.g., "Research PDF generation libraries"] - Owner: [Name] - Due: [Date]
- [ ] [Spike 2 - e.g., "Prototype async job queue"] - Owner: [Name] - Due: [Date]

**Unvalidated Assumptions:**
- [Assumption 1 - e.g., "Database can handle write load"] - How to validate: [Method]
- [Assumption 2] - How to validate: [Method]

---

## Resource Requirements

### Team Composition

**Engineering:**
- [X] Backend Engineers
- [X] Frontend Engineers
- [X] Full-Stack Engineers
- [X] DevOps/Infrastructure Engineers
- [X] QA/Test Engineers

**Non-Engineering:**
- [X] Product Manager (% time)
- [X] Designer (% time)
- [X] Technical Writer
- [Other roles as needed]

### Timeline Estimate

**Best Case:** [X weeks]
**Expected Case:** [Y weeks]
**Worst Case:** [Z weeks]

**Effort Breakdown:**

| Phase | Effort (engineer-weeks) | Calendar Time | Team Size |
|-------|-------------------------|---------------|-----------|
| Design & Planning | [X] weeks | [Y] weeks | [Z] engineers |
| Implementation | [X] weeks | [Y] weeks | [Z] engineers |
| Testing & QA | [X] weeks | [Y] weeks | [Z] engineers |
| Deployment & Rollout | [X] weeks | [Y] weeks | [Z] engineers |
| **Total** | **[X] weeks** | **[Y] weeks** | **[Z] engineers** |

**Critical Path:**
[What determines the minimum timeline? What can't be parallelized?]

### Budget Estimate

**Engineering Costs:**
- [X] engineer-weeks × $[rate] = $[total]

**Infrastructure Costs:**
- [e.g., "Cloud resources: $X/month ongoing"]
- [e.g., "Third-party services: $Y/month"]

**One-Time Costs:**
- [e.g., "Data migration: $X"]
- [e.g., "License fees: $Y"]

**Total Estimated Cost:** $[total]

### Opportunity Cost

**Trade-Offs:**
- Building this means NOT building: [Alternative feature]
- Team capacity impact: [How this affects other work]

---

## Success Metrics

### Key Performance Indicators (KPIs)

| Metric | Baseline | Target | Timeline | Measurement |
|--------|----------|--------|----------|-------------|
| [User Metric] | [Current] | [Goal] | [When] | [How tracked] |
| [Business Metric] | [Current] | [Goal] | [When] | [How tracked] |
| [Technical Metric] | [Current] | [Goal] | [When] | [How tracked] |

**Example:**
| Metric | Baseline | Target | Timeline | Measurement |
|--------|----------|--------|----------|-------------|
| Feature adoption | 0% | 30% of MAU | 3 months | Analytics event |
| Task completion time | 8 min | 2 min | 1 month | Session timing |
| Error rate | N/A | <0.1% | Ongoing | Error monitoring |

### Success Criteria

**Launch Criteria (Definition of Done):**
- [ ] All P0 requirements implemented and tested
- [ ] Performance benchmarks met
- [ ] Security review passed
- [ ] Documentation complete
- [ ] Rollout plan approved

**Post-Launch Success Indicators:**
- [Indicator 1 - e.g., "50% of target users try feature in first week"]
- [Indicator 2 - e.g., "< 5 P1 bugs reported in first month"]
- [Indicator 3 - e.g., "User satisfaction score > 4.0/5.0"]

### Monitoring & Validation

**How we'll track success:**
- [Analytics/telemetry setup]
- [User feedback collection]
- [Performance monitoring]

**Review Cadence:**
- 1 week post-launch: [Quick health check]
- 1 month post-launch: [KPI review]
- 3 months post-launch: [Full retrospective]

---

## Rollout Plan

### Deployment Strategy

**Approach:** [Big Bang / Phased Rollout / Canary / Feature Flag]

**Phases:**

**Phase 1: Internal Beta**
- **Audience:** [Internal team, X users]
- **Duration:** [Y days]
- **Success Criteria:** [What validates moving to next phase]

**Phase 2: Limited Beta**
- **Audience:** [% of users or specific segment]
- **Duration:** [Y days]
- **Success Criteria:** [What validates moving to next phase]

**Phase 3: General Availability**
- **Audience:** [All users]
- **Rollout:** [Gradual % or all at once]
- **Monitoring:** [What to watch]

### Rollback Plan

**Trigger Conditions:**
- [Condition that would trigger rollback - e.g., "Error rate > 1%"]

**Rollback Procedure:**
1. [Step 1]
2. [Step 2]
3. [Step 3]

**Data Considerations:**
- [How to handle data created during rollback period]

---

## Open Questions

### Product Questions

- [ ] **[Question 1]**
  - **Context:** [Why this matters]
  - **Owner:** [Who needs to answer]
  - **Deadline:** [When decision needed]
  - **Options:** [Possible answers]

- [ ] **[Question 2]**
  - **Context:** [Why this matters]
  - **Owner:** [Who needs to answer]
  - **Deadline:** [When decision needed]

### Technical Questions

- [ ] **[Question 1]**
  - **Context:** [Why this matters]
  - **Owner:** [Who needs to research/decide]
  - **Deadline:** [When decision needed]
  - **Spike Required:** [Yes/No]

### Design Questions

- [ ] **[Question 1]**
  - **Context:** [Why this matters]
  - **Owner:** [Designer name]
  - **Deadline:** [When decision needed]

---

## Alternatives Considered

### Alternative 1: [Approach Name]

**Description:**
[What this alternative entailed]

**Pros:**
- [Advantage 1]
- [Advantage 2]

**Cons:**
- [Disadvantage 1]
- [Disadvantage 2]

**Why Not Chosen:**
[Rationale for rejecting this approach]

### Alternative 2: [Approach Name]

**Description:**
[What this alternative entailed]

**Pros:**
- [Advantage 1]

**Cons:**
- [Disadvantage 1]

**Why Not Chosen:**
[Rationale for rejecting this approach]

---

## Appendices

### Appendix A: Related Documents

- [Link to User Research Report]
- [Link to Design Mockups]
- [Link to Technical Spike Results]
- [Link to Competitive Analysis]

### Appendix B: Technical Details

[Deep technical details that don't belong in main sections]

### Appendix C: Glossary

| Term | Definition |
|------|------------|
| [Term 1] | [Definition] |
| [Term 2] | [Definition] |

---

## Approvals

| Role | Name | Signature | Date |
|------|------|-----------|------|
| Product Manager | [Name] | | |
| Engineering Lead | [Name] | | |
| Tech Lead | [Name] | | |
| Designer | [Name] | | |
| [Other Stakeholder] | [Name] | | |

---

## Revision History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 0.1 | [Date] | [Name] | Initial draft |
| 0.2 | [Date] | [Name] | Added technical approach per engineering feedback |
| 1.0 | [Date] | [Name] | Approved for implementation |

---

**Status:** [Draft / Ready for Review / Approved / In Implementation / Shipped]
**Next Review:** [Date when this should be revisited]
```

---

## Workflows

### Creating a Feature Design Document

1. **Gather Context**
   - Review user research and problem statements
   - Understand business goals and constraints
   - Identify stakeholders and audiences

2. **Write Executive Summary**
   - Start with this even though it goes first
   - Distill to core problem, solution, impact, ask
   - Make it standalone for exec readers

3. **Document the Problem**
   - Current state and pain points
   - Evidence from research or data
   - Market context and opportunity
   - Business value and strategic alignment

4. **Describe the Solution**
   - User experience and flows
   - Functional requirements (prioritized)
   - Non-functional requirements

5. **Design Technical Approach**
   - High-level architecture
   - Data models and API specs
   - Technology choices and justifications
   - Implementation phases

6. **Assess Feasibility**
   - Rate complexity honestly
   - Identify dependencies and blockers
   - List risks with mitigations
   - Note unknowns requiring research

7. **Estimate Resources**
   - Team composition needed
   - Timeline (best/expected/worst)
   - Budget (engineering + infra + other)
   - Opportunity cost

8. **Define Success**
   - KPIs with baselines and targets
   - Launch criteria
   - Post-launch validation plan

9. **Plan Rollout**
   - Deployment strategy
   - Phasing approach
   - Rollback plan

10. **List Open Questions**
    - Product, technical, design unknowns
    - Owners and deadlines for resolution

11. **Document Alternatives**
    - Other approaches considered
    - Why the proposed solution was chosen

12. **Review & Iterate**
    - Product manager: business case and requirements
    - Engineering lead: technical approach and feasibility
    - Design: user experience and flows
    - Research-lead: methodology and evidence quality

### When to Create an FDD vs Other Docs

**Use FDD when:**
- Feature requires cross-functional coordination
- Technical feasibility is uncertain
- Resource investment is significant (>2 weeks)
- Multiple stakeholders need to align
- You need to bridge product and engineering

**Use User Story when:**
- Feature is well-understood and straightforward
- Primarily for development team consumption
- Clear acceptance criteria is the main need

**Use Technical Design Doc when:**
- Implementation details need deep technical specification
- Architecture decisions need documentation
- Primarily for engineering team consumption

**FDD is the bridge** - less detailed than pure technical specs, more technical than product requirements.

---

## Patterns

### FDD Sizing Guide

**Small FDD (1-2 weeks effort):**
- Light on technical details
- Fewer open questions
- Faster review cycle
- May skip some appendices

**Medium FDD (2-6 weeks effort):**
- Full template coverage
- Moderate technical depth
- Multiple review cycles
- Standard approval process

**Large FDD (>6 weeks effort):**
- Extensive technical appendices
- May split into multiple docs
- Requires technical spikes first
- Longer review and approval cycle

### Common FDD Anti-Patterns

**Too Implementation-Focused:**
- FDD should cover "what" and "why," not every "how" detail
- Save detailed code architecture for separate tech specs

**Missing Business Context:**
- Engineers need to understand WHY to make good tradeoffs
- Always include problem statement and business value

**Premature Precision:**
- Don't over-specify before validation
- It's okay to have open questions
- Mark unknowns clearly rather than guessing

**Missing Feasibility Assessment:**
- "We should build X" without "Can we build X?"
- Always include complexity, risks, and dependencies

---

## Limitations

- Does NOT make product prioritization decisions (consult product-manager)
- Does NOT determine technical architecture (consult engineering-lead or tech-lead)
- Does NOT conduct research or validate findings (consult research-lead)
- Does NOT make design decisions (consult designers)
- Provides documentation structure and feasibility frameworks, not decision-making authority

---

## Output Locations

Save feature design documents to:
- `docs/features/FDD-[ID]-[feature-name].md`
- `design-docs/[feature-name]-fdd.md`
- Shared documentation platform (Notion, Confluence, etc.)
- Or location specified by user

Use consistent FDD-ID format for traceability (e.g., FDD-001, FDD-002).

Include version number and date in filename for tracking iterations.
