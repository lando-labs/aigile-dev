---
name: user-story-brief
description: Create user-centric feature documentation with personas, problem statements, acceptance criteria, and success metrics. Use when writing user stories, documenting feature requirements, creating acceptance criteria, or when the user asks for user story format, feature briefs, or development-ready requirements documentation.
allowed-tools: Read, Grep, Glob, Write
---

# User Story Brief Generator

## Voice
Read and embody: `reference/voice/scout-persona.md`

## Purpose
Provides structured templates for user-centric feature documentation. Outputs standardized user story briefs with clear personas, problem statements, proposed solutions, acceptance criteria, and success metrics ready for development teams.

## Pairs Well With
- `research-lead` - For user research methodology and insight validation
- `product-manager` - For prioritization decisions and product strategy alignment
- `engineering-lead` - For technical feasibility and implementation approach

## When This Skill Activates

- User requests "user story" or "write a user story"
- Creating development-ready feature documentation
- Documenting requirements for engineering teams
- Writing acceptance criteria for features
- Translating user research into actionable requirements
- Preparing feature briefs for sprint planning

## Capabilities

### User Story Brief Structure

Generates comprehensive user story documentation with these sections:

1. **Story Overview** - Title, ID, and priority
2. **User Persona** - Who this is for
3. **Problem Statement** - What problem we're solving
4. **Proposed Solution** - How we'll solve it
5. **Acceptance Criteria** - Definition of done
6. **Success Metrics** - How we'll measure success
7. **Context & Background** - Why this matters
8. **Dependencies** - What's needed
9. **Open Questions** - What's unresolved

### User Story Format

Follows standard format:
```
As a [persona]
I want [capability]
So that [benefit/outcome]
```

### Acceptance Criteria Format

Uses "Given/When/Then" (Gherkin) format for clarity:
```
Given [precondition]
When [action]
Then [expected result]
```

## Output Template

```markdown
# User Story: [Descriptive Title]

**Story ID:** [e.g., US-123]
**Date Created:** [Date]
**Created By:** [Name]
**Priority:** [High / Medium / Low]
**Status:** [Draft / Ready / In Progress / Done]

---

## Story Statement

**As a** [user persona/role]
**I want** [capability or feature]
**So that** [benefit or value achieved]

**Example:**
> As a project manager
> I want to export task reports to PDF
> So that I can share progress with stakeholders who don't have system access

---

## User Persona

**Primary User:** [Persona name or role]

**Profile:**
- **Role/Title:** [e.g., "Marketing Manager"]
- **Experience Level:** [e.g., "3-5 years in role"]
- **Technical Proficiency:** [e.g., "Moderate - comfortable with SaaS tools"]
- **Goals:** [What they're trying to achieve]
- **Pain Points:** [Current frustrations or challenges]
- **Usage Context:** [When/where/how they'll use this]

**User Quote:**
> "[Verbatim quote from user research capturing their need or frustration]"

---

## Problem Statement

### Current Situation

[Describe the current state and why it's problematic]

**Impact:**
- [Who is affected]
- [Frequency of occurrence]
- [Business impact or cost]

**Evidence:**
- [User research finding 1]
- [Metric or data point]
- [Customer feedback quote]

### Jobs to be Done

When users encounter [situation], they are trying to [achieve goal], but currently they must [workaround/manual process], which leads to [negative outcome].

**Success Criteria:**
Users will know this problem is solved when they can [desired capability] without [current friction].

---

## Proposed Solution

### Feature Overview

[1-2 paragraph description of the proposed solution]

### User Flow

**Step-by-step experience:**

1. **Entry Point:** [How user initiates this feature]
2. **Step 1:** [User action and system response]
3. **Step 2:** [User action and system response]
4. **Step 3:** [User action and system response]
5. **Completion:** [End state and confirmation]

### Key Interactions

**Primary Actions:**
- [Action 1 and what it does]
- [Action 2 and what it does]

**System Responses:**
- [How system responds to user actions]
- [Feedback mechanisms]

### Edge Cases Addressed

- **[Edge Case 1]:** [How solution handles it]
- **[Edge Case 2]:** [How solution handles it]

---

## Acceptance Criteria

### Functional Requirements

**Scenario 1: [Happy Path]**
```gherkin
Given [precondition - user state or system state]
When [user action or trigger]
Then [expected result or behavior]
  And [additional expected result]
```

**Example:**
```gherkin
Given I am viewing a project with completed tasks
When I click "Export Report" and select "PDF format"
Then a PDF report is generated within 5 seconds
  And the PDF includes all tasks with status, assignee, and completion date
  And the PDF is automatically downloaded to my device
```

**Scenario 2: [Alternative Path]**
```gherkin
Given [different precondition]
When [user action]
Then [expected result]
```

**Scenario 3: [Error Handling]**
```gherkin
Given [error condition]
When [user action]
Then [graceful error handling]
  And [user-friendly error message]
```

### Non-Functional Requirements

**Performance:**
- [e.g., "Report generation completes in < 5 seconds for projects with < 1000 tasks"]

**Usability:**
- [e.g., "Export feature is discoverable within 3 clicks from any project view"]

**Accessibility:**
- [e.g., "Export functionality is keyboard accessible (WCAG 2.1 AA)"]

**Security:**
- [e.g., "Only users with 'Viewer' role or higher can export reports"]

**Compatibility:**
- [e.g., "PDFs render correctly in Adobe Reader, Preview, and Chrome"]

### Out of Scope

**Explicitly NOT included in this story:**
- [Feature or capability that won't be addressed]
- [Feature or capability that won't be addressed]

*(Note: These may become future stories)*

---

## Success Metrics

### Primary Metrics

**How we'll measure if this solves the problem:**

| Metric | Current Baseline | Target | Measurement Method |
|--------|------------------|--------|--------------------|
| [Metric 1] | [Current value] | [Target value] | [How measured] |
| [Metric 2] | [Current value] | [Target value] | [How measured] |

**Example:**
| Metric | Current Baseline | Target | Measurement Method |
|--------|------------------|--------|--------------------|
| Report sharing rate | 15% of users | 40% of users | Analytics event tracking |
| Time to share report | 8 min (manual) | < 1 min (export) | User session timing |
| User satisfaction | 3.2/5 | 4.5/5 | Post-feature survey (n=100) |

### Secondary Metrics

**Additional indicators of success:**
- [Metric - e.g., "Reduced support tickets related to reporting"]
- [Metric - e.g., "Increased feature adoption among paid users"]

### Validation Approach

**How we'll know if we succeeded:**
- [Method 1 - e.g., "User interviews 2 weeks post-launch (n=10)"]
- [Method 2 - e.g., "Analytics tracking for 30 days post-launch"]
- [Method 3 - e.g., "A/B test results compared to control group"]

---

## Context & Background

### Why This Matters

**Business Value:**
- [Impact on revenue, retention, acquisition, etc.]
- [Strategic alignment with company goals]

**User Value:**
- [How this improves user experience]
- [What pain point this removes]

### Related Research

**User Research:**
- [Link to research findings or summary]
- [Number of users reporting this need]
- [Severity/frequency of the problem]

**Competitive Analysis:**
- [How competitors handle this]
- [Market expectations]

### Historical Context

**Previous Attempts:**
- [Any prior solutions tried and why they failed/were removed]

**Evolution:**
- [How this request has evolved or been requested over time]

---

## Dependencies

### Technical Dependencies

**Systems/Services Required:**
- [Dependency 1 - e.g., "PDF generation library"]
- [Dependency 2 - e.g., "Background job queue for async processing"]

**Data Requirements:**
- [What data needs to be available]
- [Data quality or completeness requirements]

### Design Dependencies

**Required Before Development:**
- [ ] UI/UX mockups for export dialog
- [ ] PDF template design approved
- [ ] Error message copy written

### Other User Stories

**Blockers:**
- [Story that must be completed first]

**Related Stories:**
- [Story that pairs with this one]

---

## Open Questions

### Unresolved Items

**Product Questions:**
- [Question 1 - e.g., "Should exports be limited by user role/plan tier?"]
- [Question 2 - e.g., "What happens if report generation fails?"]

**Technical Questions:**
- [Question 1 - e.g., "Max file size for generated PDFs?"]
- [Question 2 - e.g., "Should we support scheduled/automated exports?"]

**Design Questions:**
- [Question 1 - e.g., "Should export be a modal or inline action?"]

### Decisions Needed

- [ ] **[Decision Point 1]** - Owner: [Name] - By: [Date]
- [ ] **[Decision Point 2]** - Owner: [Name] - By: [Date]

---

## Attachments

### Mockups & Designs
- [Link to Figma/design file]

### Research Assets
- [Link to user research report]
- [Link to survey results]

### Technical Specs
- [Link to technical design doc if separate]

---

## Revision History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | [Date] | [Name] | Initial draft |
| 1.1 | [Date] | [Name] | Added acceptance criteria per feedback |

---

**Approved By:** [Product Manager Name]
**Approved Date:** [Date]
**Ready for Development:** [Yes/No]
```

---

## Workflows

### Creating a User Story Brief

1. **Identify the User Need**
   - Review user research findings
   - Identify specific persona and their goal
   - Understand the current pain point

2. **Write the Story Statement**
   - Use "As a / I want / So that" format
   - Focus on outcome, not implementation
   - Keep it concise (1-2 sentences)

3. **Document the Persona**
   - Reference existing persona profiles or create lightweight profile
   - Include relevant context (role, experience, goals)
   - Add user quotes from research if available

4. **Define the Problem**
   - Current state and why it's inadequate
   - Evidence from research or data
   - Impact on users and business

5. **Describe the Solution**
   - High-level approach (not detailed implementation)
   - User flow from start to finish
   - Key interactions and edge cases

6. **Write Acceptance Criteria**
   - Use Given/When/Then format
   - Cover happy path, alternative paths, and error cases
   - Include non-functional requirements
   - Be specific and testable

7. **Define Success Metrics**
   - How you'll measure if the problem is solved
   - Current baseline and target values
   - Validation approach (when and how to measure)

8. **Add Context & Dependencies**
   - Why this matters (business and user value)
   - What's needed to build this
   - Related stories or blockers

9. **List Open Questions**
   - What's unresolved
   - Who needs to decide
   - By when decisions are needed

10. **Review & Refine**
    - Validate with research-lead for user insight accuracy
    - Review with product-manager for strategic alignment
    - Review with engineering-lead for feasibility

### Converting Research to User Stories

**From user research findings:**
1. Identify patterns and common needs across users
2. Group similar needs into story candidates
3. Prioritize based on frequency and impact
4. Write story statement capturing the core need
5. Pull evidence and quotes to support problem statement
6. Define what "success" looks like from user perspective

**From feature requests:**
1. Identify the underlying user need (not just the requested solution)
2. Research whether other users have the same need
3. Write story from user perspective (not requestor's suggested implementation)
4. Propose solution that addresses the root need
5. Include the original request as context

---

## Patterns

### Good User Story Characteristics (INVEST)

- **Independent:** Can be developed separately from other stories
- **Negotiable:** Details can be discussed and refined
- **Valuable:** Delivers clear value to users or business
- **Estimable:** Team can estimate effort required
- **Small:** Can be completed in one sprint
- **Testable:** Clear acceptance criteria enable verification

### Story Sizing Guidance

**Too Big (Epic - needs splitting):**
- Takes > 1 sprint to complete
- Has multiple distinct acceptance criteria groups
- Involves multiple user personas or use cases

**Right Size:**
- Can be completed in 1 sprint
- Has clear, focused acceptance criteria
- Delivers one complete user capability

**Too Small (Task - might be too granular):**
- Doesn't deliver standalone user value
- Is an implementation detail
- Should be part of a larger story

### Common Story Patterns

**CRUD Operation:**
```
As a [user]
I want to [create/read/update/delete] [entity]
So that I can [manage/track/organize] [outcome]
```

**Report/Export:**
```
As a [user]
I want to [generate/export/share] [information]
So that I can [communicate/analyze/backup] [purpose]
```

**Integration:**
```
As a [user]
I want [system A] to [interact with] [system B]
So that I can [avoid manual work/get unified view] [benefit]
```

**Notification/Alert:**
```
As a [user]
I want to be notified when [event occurs]
So that I can [take action/stay informed] [outcome]
```

---

## Limitations

- Does NOT make prioritization decisions (consult product-manager)
- Does NOT determine research methodology or validate user insights (consult research-lead)
- Does NOT make technical implementation decisions (consult engineering-lead)
- Provides documentation structure and templates, not product strategy or technical design

---

## Output Locations

Save user story briefs to:
- `docs/user-stories/US-[ID]-[title-slug].md`
- `features/[feature-name]/user-story.md`
- Project management tool (e.g., Jira, Linear, GitHub Issues)
- Or location specified by user

Use consistent ID format for traceability (e.g., US-001, US-002).
