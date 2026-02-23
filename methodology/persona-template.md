# {Product Name} Persona Template & Scorecard Standards

**Version**: 1.0
**Purpose**: Structural specification for all CIA-legend persona documents. Every persona across all 8 role files MUST conform to this template.
**{Product Name} Version Reference**: {Version}

---

## Document Structure

Each role file (`{project-directory}/persona-legends-{role}.md`) follows this structure:

```
# Persona Legends: {Role Title}
**Project**: {Product Name} User Testing
**Version**: 2.0 (Expanded — CIA-Legend Depth with Legacy Workflow Mapping)

---

## PERSONA {N}: {FULL NAME} — {Role} ({Title})

### PART A: THE LEGEND
### PART B-0: BEFORE {Product Name} — A Day in {Name}'s Life
### PART B: A DAY IN {NAME}'S LIFE ({Product Name})
### PART C: THE UNCOMFORTABLE QUESTIONS
### PART D: SCORECARD

---

[Repeat for each persona in this role]

---

## MIGRATION COMPLETENESS TABLE — {Role}

| Workflow Step | Legacy Tool | Time (Legacy) | {Product Name} Equivalent | Status | Time ({Product Name}) | Delta | Legacy Pain Score (1-5) | Innovation Opportunity |
|---------------|-------------|---------------|---------------------|--------|-------------------|-------|------------------------|----------------------|

---

## CROSS-PERSONA COMPARISON — {Role}

| Dimension | Persona 1 | Persona 2 | ... |
|-----------|-----------|-----------|-----|

---

## EXECUTIVE SUMMARY — {Role}

**Top 3 Critical Findings:**
1. ...
2. ...
3. ...

**Platform Score**: {weighted average across all personas in this role}
```

---

## PART A: THE LEGEND — Required Fields

Every persona's Part A MUST contain these subsections in this order:

### Identity & Background
- **Name**: Full name, age
- **Education**: Degrees, certifications, year obtained
- **Career Arc**: Chronological career history with companies, titles, and years. Minimum 3 career stops.
- **Defining Failure**: A specific, detailed professional failure with dollar amounts and consequences
- **Defining Triumph**: A specific, detailed professional success with measurable outcomes
- **Why {Product Name}** (internal) / **Why This Organization** (external): Motivation for current role

### Personal Life
- **Family**: Relationship status, dependents, key details
- **Routine**: Morning and evening bookends (6am / 11pm)
- **Technology**: Overall relationship with technology — devices, habits, preferences
- **Workspace**: Physical setup — monitors, device, physical items on desk
- **Non-Work Stress**: A specific personal stressor that humanizes the persona and occasionally affects work focus

### Behavioral Psychology
- **MBTI**: 4-letter type with archetype name. **NO DUPLICATES WITHIN A ROLE.**
- **Big Five**: All 5 traits rated (High/Moderate/Low) with brief context
- **Decision Style**: How they make decisions (data-driven, relationship-driven, process-driven, etc.)
- **Software Reaction**: What they do when software fails or doesn't meet expectations
- **Incomplete Feature Tolerance**: X/10 rating with explanation
- **Cognitive Biases**: 2-3 named cognitive biases with relevance to their software use

### Software History (optional for external roles — use "Technology Experience" instead)
- **Tools used**: Listed with years of experience and emotional relationship (per Legacy Tool Emotional Signatures)
- **Tabs open**: Typical browser/app arrangement
- **Keyboard shortcuts**: Power user indicators
- **Screen**: Display setup

---

## PART B-0: BEFORE {Product Name} — Required Fields

This section documents the persona's FULL daily workflow using ONLY their legacy tools. No {Product Name} references.

### Required Elements:
1. **Morning arrival routine** — what they check first, in what order
2. **Tool sequence** — each tool used, in the order encountered, with approximate time spent
3. **Specific task walkthroughs** — minimum 3 detailed task narratives showing click-by-click (or tab-by-tab) interaction with legacy tools
4. **Handoff friction points** — who do they wait on? For what? How long? What breaks?
5. **Data re-entry incidents** — same data entered in 2+ systems, with time cost
6. **Cost of workarounds** — time, money, or risk created by manual processes
7. **Emotional relationship with legacy tools** — use the Legacy Tool Emotional Signatures (see Creative Direction in persona-expansion.md)
8. **End-of-day state** — what remains undone, what carries over

### "Before {Product Name}" for External Roles (Investor, Lender)
External personas have two layers:
1. **Their own tool stack** (what they use daily regardless of the organization)
2. **Their interaction workflow** (how they receive/review data from the organization)

Both layers must be documented.

### Constraints:
- NO {Product Name} mentions in this section
- NO "{Product Name} should..." or "ideally this would..." statements
- NO aspirational feature specs — this section is purely descriptive of existing reality
- Tools referenced MUST be consistent with the persona's Software History in Part A
- Time estimates MUST be plausible (not suspiciously round)

---

## PART B: A DAY IN {NAME}'S LIFE ({Product Name}) — Required Fields

This section documents the persona's experience WITH {Product Name}. Carries forward from existing persona format.

### Required Elements:
1. **Login/arrival context** — how they get to {Product Name}, what else is open
2. **First-screen reaction** — what they notice first (per Screen-Loading Behavior assignment from Creative Direction)
3. **Primary task attempt** — the MAIN thing they try to do, step by step
4. **Dead-end discovery** — at least one moment where {Product Name} fails them (missing feature, broken link, access wall)
5. **Workaround employed** — what they do instead (email someone, open Excel, call a colleague)
6. **Secondary task attempt** (if applicable) — another workflow they try
7. **Cross-role interaction** — at least one moment where they need data from or need to communicate with another role
8. **Session end** — when they close {Product Name}, what was accomplished vs. what wasn't

### Physical/Behavioral Details:
- Reference the persona's Physical Habits During Software Use (from Creative Direction)
- Include Internal Monologue Voice snippets in italics
- Show the Emotional Arc assigned to this persona (from Creative Direction)

---

## PART C: THE UNCOMFORTABLE QUESTIONS — Required Fields

- Minimum 5 questions, maximum 7
- Questions MUST be:
  - Written in the persona's voice (using their Internal Monologue Voice style)
  - Specific to features/gaps they encountered in Part B
  - Grounded in real codebase state (reference actual pages, actual access controls, actual data gaps)
  - Each targeting a DIFFERENT gap than other questions in the same list
- **NO recycled questions within a role** — each persona in a role must ask different questions
- **NEW personas MUST identify at least ONE "NEW GAP"** not found by existing personas in that role

---

## PART D: SCORECARD — Required Fields

Scorecard table format:

```markdown
| Capability | Score (0-5) | Notes |
|------------|-------------|-------|
| {Capability 1} | X | {specific observation} |
| {Capability 2} | X | {specific observation} |
| {Capability 3} | X | {specific observation} |
| {Capability 4} | X | {specific observation} |
| {Capability 5} | X | {specific observation} |
| **Average** | **X.X** | **{VERDICT}** |
```

### Verdict Scale:
- **4.0-5.0**: PASS — Role is well-served
- **2.5-3.9**: CONDITIONAL PASS — Usable with workarounds
- **1.0-2.4**: FAIL — Not viable for daily use
- **0.0-0.9**: CRITICAL FAIL — Actively harmful to role workflow

---

## Per-Role Scorecard Rubrics

### Admin:
| Capability | Description |
|------------|-------------|
| Daily Workflow Coverage | Can the admin manage users, review dashboards, prepare reports, and oversee operations from {Product Name}? |
| Data Completeness | Are dashboard metrics clickable and drill-downable? Can they trace data back to its source? |
| Audit & Controls | Does {Product Name} provide audit trails, period locks, role-based access enforcement, and change logs? |
| Role Fit | Does the admin view surface the right data at the right level of detail? Are admin-specific tools functional? |
| Adoption Likelihood | Would this persona actually use {Product Name} daily, or revert to legacy tools? |

### Analyst:
| Capability | Description |
|------------|-------------|
| Analysis Workflow | Can the analyst move from initial screening to detailed analysis to scenario comparison without leaving {Product Name}? |
| Data Input/Output | Is data entry efficient? Can models be exported, shared, or versioned? Is there document/data ingestion? |
| Scenario Modeling | Does {Product Name} support sensitivity analysis, stress testing, and side-by-side scenario comparison? |
| Collaboration | Can the analyst share models with peers, present to leadership, or hand off to other teams? |
| Adoption Likelihood | Would this persona use {Product Name} as primary analysis tool, or revert to spreadsheets? |

### IR (Investor Relations):
| Capability | Description |
|------------|-------------|
| Relationship Management | Can IR manage the full stakeholder lifecycle: prospecting, onboarding, communication, reporting, and tracking? |
| Campaign Execution | Does {Product Name} support structured campaigns with target lists, outreach tracking, and pipeline visualization? |
| Data Sync Reliability | Does external integration work reliably? Are contact records consistent across systems? |
| Portal Preview/Testing | Can IR preview what stakeholders see in the portal? Can they verify data accuracy before access? |
| Adoption Likelihood | Would IR use {Product Name} for daily relationship management, or maintain a parallel workflow? |

### BD (Business Development):
| Capability | Description |
|------------|-------------|
| Opportunity Screening Speed | Can BD quickly evaluate a new opportunity — initial assessment, comparison, go/no-go recommendation — within {Product Name}? |
| Data Completeness | Does {Product Name} give BD visibility into available resources, terms, and criteria to qualify opportunities? |
| Scenario Analysis | Can BD model multiple scenarios, run sensitivities, and compare options to present to leadership? |
| Collaboration/Sharing | Can BD share packages, invite team review, or export materials for external use? |
| Adoption Likelihood | Would BD use {Product Name} for analysis, or default to personal spreadsheet models? |

### PM (Project Manager / Operator):
| Capability | Description |
|------------|-------------|
| Project Workflow Coverage | Does {Product Name} support daily logs, task tracking, submissions, change management, or other project functions? |
| Budget Visibility | Can the PM see project budgets, cost-to-date, committed costs, and budget-to-actual variance within {Product Name}? |
| Schedule Integration | Does {Product Name} provide scheduling, milestone tracking, or critical path visibility? |
| Cross-Role Data Access | Can the PM see financial data (invoices, payments, status) relevant to their projects without emailing Finance? |
| Adoption Likelihood | Would the PM use {Product Name} for project management, or remain in legacy tools? |

### Finance (CFO / Controller):
| Capability | Description |
|------------|-------------|
| GL & Journal Accuracy | Does the General Ledger enforce double-entry, maintain proper chart of accounts, and handle multi-entity postings correctly? |
| Reconciliation Capability | Can Finance perform reconciliation (import, match, approve) within {Product Name}? |
| Reporting Reliability | Are financial statements accurate enough for external presentation? |
| Compliance/Controls | Does {Product Name} provide period locks, approval chains, audit trails, and segregation of duties? |
| Adoption Likelihood | Would Finance use {Product Name}'s accounting module, or maintain legacy systems as the system of record? |

### Investor:
| Capability | Description |
|------------|-------------|
| Portfolio Visibility | Can the investor see their total portfolio: investments, returns, capital activity, distributions, across all positions? |
| Data Accuracy | Are the financial figures shown (invested amount, valuation, returns, distributions) correct and current? |
| Document Access | Can the investor access key documents and reports? |
| Competitive Comparison | How does {Product Name}'s investor portal compare to other industry portals the investor has seen? |
| Adoption Likelihood | Would the investor bookmark {Product Name}'s portal, or request reports via email instead? |

### Lender:
| Capability | Description |
|------------|-------------|
| Compliance Monitoring | Can the lender view real-time or periodic compliance data for their loans? |
| Balance Accuracy | Does the portal show correct outstanding balance, payment history, and schedule details? |
| Payment History | Can the lender see all payments received, transaction history, and remaining commitment? |
| Regulatory Compliance Signal | Does {Product Name} provide data in a format useful for the lender's internal regulatory reporting? |
| Adoption Likelihood | Would the lender check {Product Name}'s portal for compliance data, or continue requiring manual reports? |

---

## Migration Completeness Table — Column Specification

Each role file MUST end with a per-role Migration Completeness Table using these columns:

| Column | Description |
|--------|-------------|
| **Workflow Step** | Specific task or action in the role's daily workflow (e.g., "Reconciliation — import statement") |
| **Legacy Tool** | Which tool handles this step today (e.g., "System X") |
| **Time (Legacy)** | Approximate time to complete this step in the legacy tool |
| **{Product Name} Equivalent** | The {Product Name} feature/page that addresses this step (or "None") |
| **Status** | One of: **Replaced** ({Product Name} fully handles it) / **Partial** ({Product Name} partially handles it) / **Missing** ({Product Name} has no equivalent) / **Broken** ({Product Name} has the feature but it doesn't work correctly) |
| **Time ({Product Name})** | Approximate time in {Product Name} (or "N/A" if Missing) |
| **Delta** | Time saved or lost (positive = faster in {Product Name}, negative = slower, "N/A" if Missing) |
| **Legacy Pain Score (1-5)** | How painful is this step in the legacy tool? 1 = trivial, 5 = excruciating. Provides comparison baseline. |
| **Innovation Opportunity** | For "Missing" or "Partial" items: should {Product Name} **Replicate** (build same feature), **Reimagine** (solve the problem differently), or **Skip** (deliberately not address this)? |

### Migration Table Rules:
- Minimum 8 workflow steps per role
- At least one step MUST have Status = "Replaced" (even underserved roles have something)
- Tables are per-ROLE, not per-persona — individual personas contribute observations to the role table
- Legacy Pain Score creates the comparison baseline: high Legacy Pain + low {Product Name} status = high priority gap

---

## Cross-Persona Comparison Matrix — Format

Each role file with 2+ personas MUST include a comparison matrix:

| Dimension | {Persona 1 Name} | {Persona 2 Name} | {Persona 3 Name} | ... |
|-----------|-------------------|-------------------|-------------------|-----|
| MBTI | ENTJ | ESFP | INTJ | ... |
| Seniority | Senior (20+ yr) | Junior (3 yr) | Mid-level (15 yr) | ... |
| Primary Device | Desktop dual-monitor | Tablet | Laptop | ... |
| Emotional Arc | {Emotional archetype} | {Emotional archetype} | {Emotional archetype} | ... |
| Screen-Loading Behavior | {Behavior type} | {Behavior type} | {Behavior type} | ... |
| Legacy Tool Dependency | High ({tool}) | Low ({tool}) | Medium ({tool}) | ... |
| {Product Name} Score | 2.4 | 1.8 | 2.0 | ... |
| NEW GAP Identified | {gap description} | {gap description} | {gap description} | ... |

---

## MBTI Assignment Constraints

### Rule: No MBTI duplicates within a role file.

### Already Assigned (from existing personas — DO NOT REUSE within these roles):
| Role | Persona | MBTI |
|------|---------|------|
| Admin | {Persona Name} | ENTJ |
| IR | {Persona Name} | ENFJ |
| BD | {Persona Name} | INTJ |
| PM | {Persona Name} | ISTJ |
| Finance | {Persona Name} | ISTJ |
| Investor | {Persona Name} | INTJ |
| Lender | {Persona Name} | ESTJ |

### Available Pool (16 types minus assigned):
INFJ, INFP, ENFP, ENTP, ISFJ, ISFP, ESFJ, ESFP, ISTP, ESTP, INTP, ENTJ*, ENFJ*, INTJ*, ISTJ*, ESTJ*

*Starred types are already assigned to one role — they CAN be used for a DIFFERENT role's persona, but CANNOT be duplicated within the same role.*

---

## Uncomfortable Questions — Uniqueness Tracking

Each role file must track which gaps its personas' questions target. Format:

```markdown
### Question Gap Coverage — {Role}
| Gap Targeted | Persona 1 Q# | Persona 2 Q# | Persona 3 Q# |
|--------------|---------------|---------------|---------------|
| No audit trail | Q1 | - | - |
| Dead-end navigation | - | Q2 | - |
| Missing budget visibility | - | - | Q1 |
```

This ensures no two personas in the same role ask about the same gap.

---

## Executive Summary — Format

Each role file MUST end with a 1-page executive summary:

```markdown
## EXECUTIVE SUMMARY — {Role}

**Personas Evaluated**: {count}
**Platform Score Range**: {min} - {max} (Average: {avg})
**Verdict**: {PASS / CONDITIONAL PASS / FAIL / CRITICAL FAIL}

### Top 3 Critical Findings:
1. **{Finding}**: {1-2 sentence description with specific {Product Name} reference}
2. **{Finding}**: {1-2 sentence description}
3. **{Finding}**: {1-2 sentence description}

### New Gaps Discovered (not in original 7-persona evaluation):
- {NEW GAP}: {description} — discovered by {persona name}
- {NEW GAP}: {description} — discovered by {persona name}

### Recommendation:
{1-2 sentences on what must change for this role to adopt {Product Name}}
```

---

## Quality Checklist (for QA validation — Phase 5)

- [ ] 8 persona files exist in `{project-directory}/`
- [ ] Total persona count across all files is 22-24
- [ ] Every persona contains all 5 required sections (Part A, B-0, B, C, D)
- [ ] Every persona file ends with a Migration Completeness Table
- [ ] Every persona file ends with an Executive Summary
- [ ] No two personas within the same role share an MBTI type
- [ ] No "Uncomfortable Questions" are repeated within a role
- [ ] All {Product Name} references are grounded in actual codebase ({Version})
- [ ] All "Before {Product Name}" (Part B-0) sections contain ZERO {Product Name} mentions
- [ ] Every new persona identifies at least one "NEW GAP" not found by existing personas
- [ ] Every Migration Completeness Table has minimum 8 workflow steps
- [ ] Every Migration Completeness Table includes Legacy Pain Score and Innovation Opportunity columns
- [ ] Cross-Persona Comparison Matrix exists in every file with 2+ personas
- [ ] Question Gap Coverage table exists in every file with 2+ personas
