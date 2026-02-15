# NorthStar Persona Template & Scorecard Standards

**Version**: 1.0
**Purpose**: Structural specification for all CIA-legend persona documents. Every persona across all 8 role files MUST conform to this template.
**NorthStar Version Reference**: v0.7.2

---

## Document Structure

Each role file (`.sisyphus/drafts/persona-legends-{role}.md`) follows this structure:

```
# Persona Legends: {Role Title}
**Project**: NorthStar Dealflow OS User Testing
**Version**: 2.0 (Expanded — CIA-Legend Depth with Legacy Workflow Mapping)

---

## PERSONA {N}: {FULL NAME} — {Role} ({Title})

### PART A: THE LEGEND
### PART B-0: BEFORE NORTHSTAR — A Day in {Name}'s Life
### PART B: A DAY IN {NAME}'S LIFE (NorthStar)
### PART C: THE UNCOMFORTABLE QUESTIONS
### PART D: SCORECARD

---

[Repeat for each persona in this role]

---

## MIGRATION COMPLETENESS TABLE — {Role}

| Workflow Step | Legacy Tool | Time (Legacy) | NorthStar Equivalent | Status | Time (NorthStar) | Delta | Legacy Pain Score (1-5) | Innovation Opportunity |
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
- **Why Tri-Star** (internal) / **Why This GP** (external): Motivation for current role

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

## PART B-0: BEFORE NORTHSTAR — Required Fields

This section documents the persona's FULL daily workflow using ONLY their legacy tools. No NorthStar references.

### Required Elements:
1. **Morning arrival routine** — what they check first, in what order
2. **Tool sequence** — each tool used, in the order encountered, with approximate time spent
3. **Specific task walkthroughs** — minimum 3 detailed task narratives showing click-by-click (or tab-by-tab) interaction with legacy tools
4. **Handoff friction points** — who do they wait on? For what? How long? What breaks?
5. **Data re-entry incidents** — same data entered in 2+ systems, with time cost
6. **Cost of workarounds** — time, money, or risk created by manual processes
7. **Emotional relationship with legacy tools** — use the Legacy Tool Emotional Signatures (see Creative Direction in persona-expansion.md)
8. **End-of-day state** — what remains undone, what carries over

### "Before NorthStar" for External Roles (Investor, Lender)
External personas have two layers:
1. **Their own tool stack** (what they use daily regardless of Tri-Star)
2. **Their GP-interaction workflow** (how they receive/review data from sponsors like Tri-Star)

Both layers must be documented.

### Constraints:
- NO NorthStar mentions in this section
- NO "NorthStar should..." or "ideally this would..." statements
- NO aspirational feature specs — this section is purely descriptive of existing reality
- Tools referenced MUST be consistent with the persona's Software History in Part A
- Time estimates MUST be plausible (not suspiciously round)

---

## PART B: A DAY IN {NAME}'S LIFE (NorthStar) — Required Fields

This section documents the persona's experience WITH NorthStar. Carries forward from existing persona format.

### Required Elements:
1. **Login/arrival context** — how they get to NorthStar, what else is open
2. **First-screen reaction** — what they notice first (per Screen-Loading Behavior assignment from Creative Direction)
3. **Primary task attempt** — the MAIN thing they try to do, step by step
4. **Dead-end discovery** — at least one moment where NorthStar fails them (missing feature, broken link, access wall)
5. **Workaround employed** — what they do instead (email someone, open Excel, call a colleague)
6. **Secondary task attempt** (if applicable) — another workflow they try
7. **Cross-role interaction** — at least one moment where they need data from or need to communicate with another role
8. **Session end** — when they close NorthStar, what was accomplished vs. what wasn't

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
| Daily Workflow Coverage | Can the admin manage users, review dashboards, prepare board reports, and oversee firm operations from NorthStar? |
| Data Completeness | Are dashboard metrics clickable and drill-downable? Can they trace data back to its source? |
| Audit & Controls | Does NorthStar provide audit trails, period locks, role-based access enforcement, and change logs? |
| Role Fit | Does the admin view surface the right data at the right level of detail? Are admin-specific tools functional? |
| Adoption Likelihood | Would this persona actually use NorthStar daily, or revert to legacy tools? |

### Analyst:
| Capability | Description |
|------------|-------------|
| Underwriting Workflow | Can the analyst move from napkin-level screening to full pro forma to scenario comparison without leaving NorthStar? |
| Data Input/Output | Is data entry efficient? Can models be exported, shared, or versioned? Is there document/data ingestion? |
| Scenario Modeling | Does NorthStar support sensitivity analysis, stress testing, and side-by-side scenario comparison? |
| Collaboration | Can the analyst share models with BD, present to IC, or hand off to Finance? |
| Adoption Likelihood | Would this persona use NorthStar as primary underwriting tool, or revert to Excel? |

### IR (Investor Relations):
| Capability | Description |
|------------|-------------|
| LP Relationship Management | Can IR manage the full LP lifecycle: prospecting, onboarding, communication, reporting, capital calls, distributions? |
| Campaign Execution | Does NorthStar support structured fundraising campaigns with target lists, outreach tracking, and pipeline visualization? |
| Data Sync Reliability | Does GHL integration work reliably? Are contact records consistent across CRM and NorthStar? |
| Portal Preview/Testing | Can IR preview what investors see in the portal? Can they verify data accuracy before LP access? |
| Adoption Likelihood | Would IR use NorthStar for daily LP management, or maintain a parallel GHL/Sheets workflow? |

### BD (Business Development):
| Capability | Description |
|------------|-------------|
| Deal Screening Speed | Can BD quickly evaluate a new opportunity — napkin math, comparable check, go/no-go recommendation — within NorthStar? |
| Data Completeness (Fund Visibility) | Does NorthStar give BD visibility into available capital, fund terms, and investment criteria to qualify deals? |
| Scenario Analysis | Can BD model multiple deal structures, run sensitivities, and compare scenarios to present to IC? |
| Collaboration/Sharing | Can BD share deal packages, invite team review, or export materials for external use? |
| Adoption Likelihood | Would BD use NorthStar for deal analysis, or default to personal Excel models? |

### PM (Project Manager / Operator):
| Capability | Description |
|------------|-------------|
| Construction Workflow Coverage | Does NorthStar support daily logs, RFIs, submittals, change orders, draw requests, or any construction management function? |
| Budget Visibility | Can the PM see project budgets, cost-to-date, committed costs, and budget-to-actual variance within NorthStar? |
| Schedule Integration | Does NorthStar provide scheduling, milestone tracking, or critical path visibility beyond entitlements? |
| Cross-Role Data Access | Can the PM see financial data (invoices, payments, draw status) relevant to their projects without emailing Finance? |
| Adoption Likelihood | Would the PM use NorthStar beyond entitlements tracking, or remain in Procore/Excel? |

### Finance (CFO / Controller):
| Capability | Description |
|------------|-------------|
| GL & Journal Accuracy | Does the General Ledger enforce double-entry, maintain proper chart of accounts, and handle multi-entity postings correctly? |
| Reconciliation Capability | Can Finance perform bank reconciliation (import, match, approve) within NorthStar? |
| Reporting Reliability | Are financial statements (Income Statement, Balance Sheet, Cash Flow) accurate enough for external presentation? |
| Compliance/Controls | Does NorthStar provide period locks, approval chains, audit trails, and segregation of duties? |
| Adoption Likelihood | Would Finance use NorthStar's accounting module, or maintain Yardi/QuickBooks as the system of record? |

### Investor:
| Capability | Description |
|------------|-------------|
| Portfolio Visibility | Can the investor see their total portfolio: investments, returns, capital calls, distributions, across all positions? |
| Data Accuracy | Are the financial figures shown (invested amount, NAV, IRR, distributions) correct and current? |
| Document Access | Can the investor access K-1s, quarterly reports, PPMs, subscription agreements, and other key documents? |
| Competitive Comparison | How does NorthStar's investor portal compare to Juniper Square, Addepar, or other GP portals the investor has seen? |
| Adoption Likelihood | Would the investor bookmark NorthStar's portal, or request PDF reports via email instead? |

### Lender:
| Capability | Description |
|------------|-------------|
| Covenant Monitoring | Can the lender view real-time or periodic covenant compliance data (DSCR, LTV, Debt Yield) for their loans? |
| Balance Accuracy | Does the portal show correct outstanding balance, payment history, and amortization schedule? |
| Payment History | Can the lender see all payments received, draw history (for construction loans), and remaining commitment? |
| Regulatory Compliance Signal | Does NorthStar provide data in a format useful for the lender's internal regulatory reporting (CECL, concentration)? |
| Adoption Likelihood | Would the lender check NorthStar's portal for compliance data, or continue requiring manual PDF reports? |

---

## Migration Completeness Table — Column Specification

Each role file MUST end with a per-role Migration Completeness Table using these columns:

| Column | Description |
|--------|-------------|
| **Workflow Step** | Specific task or action in the role's daily workflow (e.g., "Bank reconciliation — import statement") |
| **Legacy Tool** | Which tool handles this step today (e.g., "Yardi Voyager") |
| **Time (Legacy)** | Approximate time to complete this step in the legacy tool |
| **NorthStar Equivalent** | The NorthStar feature/page that addresses this step (or "None") |
| **Status** | One of: **Replaced** (NorthStar fully handles it) / **Partial** (NorthStar partially handles it) / **Missing** (NorthStar has no equivalent) / **Broken** (NorthStar has the feature but it doesn't work correctly) |
| **Time (NorthStar)** | Approximate time in NorthStar (or "N/A" if Missing) |
| **Delta** | Time saved or lost (positive = faster in NorthStar, negative = slower, "N/A" if Missing) |
| **Legacy Pain Score (1-5)** | How painful is this step in the legacy tool? 1 = trivial, 5 = excruciating. Provides comparison baseline. |
| **Innovation Opportunity** | For "Missing" or "Partial" items: should NorthStar **Replicate** (build same feature), **Reimagine** (solve the problem differently), or **Skip** (deliberately not address this)? |

### Migration Table Rules:
- Minimum 8 workflow steps per role
- At least one step MUST have Status = "Replaced" (even underserved roles have something)
- Tables are per-ROLE, not per-persona — individual personas contribute observations to the role table
- Legacy Pain Score creates the comparison baseline DA requested: high Legacy Pain + low NorthStar status = high priority gap

---

## Cross-Persona Comparison Matrix — Format

Each role file with 2+ personas MUST include a comparison matrix:

| Dimension | {Persona 1 Name} | {Persona 2 Name} | {Persona 3 Name} | ... |
|-----------|-------------------|-------------------|-------------------|-----|
| MBTI | ENTJ | ESFP | INTJ | ... |
| Seniority | COO (20+ yr) | Junior (3 yr) | Director (15 yr) | ... |
| Primary Device | Desktop dual-monitor | iPad Pro | Laptop | ... |
| Emotional Arc | The Overwhelmed Newcomer | The Genuine Enthusiast | The Vindicated Skeptic | ... |
| Screen-Loading Behavior | The Number Scanner | The Speed Scroller | The Skeptic Squinter | ... |
| Legacy Tool Dependency | High (Airtable) | Low (pen-and-paper) | Medium (Argus) | ... |
| NorthStar Score | 2.4 | 1.8 | 2.0 | ... |
| NEW GAP Identified | {gap description} | {gap description} | {gap description} | ... |

---

## MBTI Assignment Constraints

### Rule: No MBTI duplicates within a role file.

### Already Assigned (from existing personas — DO NOT REUSE within these roles):
| Role | Persona | MBTI |
|------|---------|------|
| Admin | Sarah Chen | ENTJ |
| IR | Marcus Williams | ENFJ |
| BD | James Okafor | INTJ |
| PM | Lisa Nguyen | ISTJ |
| Finance | David Park | ISTJ |
| Investor | Catherine Moore | INTJ |
| Lender | Robert Chen | ESTJ |

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
1. **{Finding}**: {1-2 sentence description with specific NorthStar reference}
2. **{Finding}**: {1-2 sentence description}
3. **{Finding}**: {1-2 sentence description}

### New Gaps Discovered (not in original 7-persona evaluation):
- {NEW GAP}: {description} — discovered by {persona name}
- {NEW GAP}: {description} — discovered by {persona name}

### Recommendation:
{1-2 sentences on what must change for this role to adopt NorthStar}
```

---

## Quality Checklist (for QA validation — Phase 5)

- [ ] 8 persona files exist in `.sisyphus/drafts/`
- [ ] Total persona count across all files is 22-24
- [ ] Every persona contains all 5 required sections (Part A, B-0, B, C, D)
- [ ] Every persona file ends with a Migration Completeness Table
- [ ] Every persona file ends with an Executive Summary
- [ ] No two personas within the same role share an MBTI type
- [ ] No "Uncomfortable Questions" are repeated within a role
- [ ] All NorthStar references are grounded in actual codebase (v0.7.2)
- [ ] All "Before NorthStar" (Part B-0) sections contain ZERO NorthStar mentions
- [ ] Every new persona identifies at least one "NEW GAP" not found by existing personas
- [ ] Every Migration Completeness Table has minimum 8 workflow steps
- [ ] Every Migration Completeness Table includes Legacy Pain Score and Innovation Opportunity columns
- [ ] Cross-Persona Comparison Matrix exists in every file with 2+ personas
- [ ] Question Gap Coverage table exists in every file with 2+ personas
