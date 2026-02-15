# Persona-Driven Development: A Practitioner's Playbook

## What Is This?

Persona-Driven Development (PDD) is a product-agnostic methodology for building software that fits the user's reality with surgical precision. In traditional development, the software is often a rigid "mold" and the user is the "clay"—forced to deform their workflows, habits, and mental models to fit the constraints of the interface. If the button is on the left, the user moves their mouse to the left. If the data requires a specific format, the user spends hours in Excel preparing it. The user is expected to be plastic, while the software remains cast in iron.

PDD inverts this relationship. In PDD, the **Persona is the Mold**, and the **Software is the Clay**. We begin by casting a high-fidelity, "CIA-legend" depth mold of the user's existing reality—their legacy tools, emotional triggers, physical habits, and professional traumas. We then press the software into this mold. If the software doesn't fill every crevice of the persona's workflow, it is the software that must be reshaped, not the user.

This methodology treats personas not as marketing sketches, but as **executable specifications**. By documenting the "Before" state with the same rigor as the "After" state, we create a migration completeness roadmap that ensures the software solves for the user's actual life, rather than an idealized version of it.

You should use this methodology if:
- You are building complex, workflow-heavy software (B2B SaaS, internal tools, specialized professional platforms).
- You are migrating users from deeply entrenched legacy systems (Excel, legacy ERPs, manual processes).
- You are using AI agents for development and need high-fidelity "executable specifications" to guide them.
- You want to move beyond "happy path" testing and expose deep, structural gaps in your product.
- You are tired of building features that users "should" want but never actually use.
- You want to reduce the "adoption gap" between product launch and actual user utility.

## Where This Fits in the AI Development Landscape

The AI development landscape is rapidly evolving from simple code generation to complex agentic workflows. While early AI coding assistants focused on autocomplete, the current generation is moving toward autonomous agents that can plan and execute multi-step tasks.

However, a critical gap remains: **Requirement Fidelity**.

While frameworks like **CRAFTER** and **StrongDM** focus on technical infrastructure and access, and multi-agent systems like **ChatDev**, **MetaGPT**, and **AutoGen** focus on the software production process, PDD addresses the *human-centric requirement* problem.

PDD bridges the gap between **SyntheticUsers** (which uses AI for market research) and the actual implementation. It provides the "soul" and the "friction" that generic agentic development often lacks. By simulating the professional and psychological reality of the user, PDD ensures that AI agents are building toward a target that actually matters. It transforms the development process from "building what was asked" to "building what is needed to survive the user's daily life."

### Literature Positioning Summary

| Framework | Focus Area | PDD Integration |
| :--- | :--- | :--- |
| **CRAFTER** | Technical Infrastructure | PDD provides the requirements for the infrastructure. |
| **StrongDM** | Access & Security | PDD defines the role-based access requirements. |
| **ChatDev / MetaGPT** | Software Production | PDD provides the "executable specs" for the agents. |
| **SyntheticUsers** | Market Research | PDD takes research and turns it into implementation specs. |
| **AutoGen** | Multi-Agent Workflows | PDD uses AutoGen-style loops for persona generation. |

## The Process Overview

The PDD methodology follows an 8-step pipeline that transforms role-based evaluations into verified software implementations.

1.  **Evaluate**: Establish a baseline of the software's current utility for target roles.
2.  **Template**: Design a high-fidelity "CIA-legend" structure for personas.
3.  **Creative Direction**: Define the "texture" (habits, biases, emotional arcs) for the personas.
4.  **Generate**: Produce personas using a Generative-Critical agent loop.
5.  **Bridge**: Convert persona insights into a prioritized, actionable backlog.
6.  **Factory**: Set up validation infrastructure (Software Factory) to protect core logic.
7.  **Plan**: Design multi-wave execution plans based on the backlog.
8.  **Execute**: Implement changes and verify them against the persona "mold."

### Pipeline Inputs and Outputs

| Step | Primary Input | Primary Output |
| :--- | :--- | :--- |
| **1. Evaluate** | Current Codebase + Role Definitions | Role-Based Evaluation Docs + Scorecard |
| **2. Template** | Evaluation Results + Domain Research | Master Persona Template |
| **3. Creative Direction** | Persona Template | Creative Direction Toolkit |
| **4. Generate** | Template + Creative Direction | CIA-Legend Persona Files |
| **5. Bridge** | Persona Files + Evaluation Results | Prioritized Backlog (P0-P3) |
| **6. Factory** | Backlog + Core Logic | Validation Harness + Property Tests |
| **7. Plan** | Backlog + Factory Infrastructure | Multi-Wave Execution Plans |
| **8. Execute** | Execution Plan + Software Factory | Updated Codebase + Verification Evidence |

## Getting Started (Quick-Start Guide)

### Prerequisites
- **Functional Codebase**: A working prototype or v0.x product that can be evaluated. [adapt for your domain]
- **Role Access Matrix**: A clear definition of the organizational roles the software intends to serve. [insert your roles]
- **AI Infrastructure**: Access to LLMs (e.g., Claude 3.5 Sonnet, GPT-4o) for agentic loops.
- **Domain Knowledge**: Access to (or research on) the legacy tools and workflows of your target users. [replace with your domain]

### Minimum Viable Version (The "PDD Lite")
If you are short on time or resources, you can abbreviate the process:
- **Abbreviated Evaluation**: Focus only on the "Golden User Story" for each role.
- **Simplified Template**: Use a 2-page persona structure instead of the full CIA-legend.
- **Single-Agent Generation**: Skip the Critical Reviewer loop (though this increases the risk of homogeneity).
- **Unit Test Factory**: Use standard unit tests instead of a full Three-Zone architecture.

### Time Estimates
- **Step 1 (Evaluate)**: 4-8 hours per role.
- **Step 2 (Template)**: 4 hours (one-time setup).
- **Step 3 (Creative Direction)**: 4 hours (one-time setup).
- **Step 4 (Generate)**: 2-4 hours per batch of 5 personas.
- **Step 5 (Bridge)**: 8-16 hours (depending on persona count).
- **Step 6 (Factory)**: 2-5 days (depending on logic complexity).
- **Step 7 (Plan)**: 4-8 hours per execution wave.
- **Step 8 (Execute)**: Variable (task-dependent).

### Team Size Recommendations
- **Solo Developer**: Highly effective when using AI agents for generation and verification.
- **Small Team (2-5)**: One "Methodology Lead" (Product/Design) and 2-4 "Executors" (Engineering).
- **Enterprise**: Dedicated "Persona Architects" who maintain the mold across multiple product lines.

### Tool Recommendations
- **Persona Generation**: Claude 3.5 Sonnet (for creative depth) or GPT-4o.
- **Backlog Management**: Linear, GitHub Issues, or Trello.
- **Validation**: Playwright (UI), Vitest/Jest (Logic), Python/Bash (Data).
- **Documentation**: Obsidian, Notion, or a dedicated Git repository.

---

## Step-by-Step Methodology

### Step 1: Role-Based Evaluation
**Purpose**: To establish a baseline of the software's current utility for each target role and identify obvious "low-hanging" gaps. This step prevents the "blank slate" problem by forcing the development team to confront the existing reality of the product before imagining its future.

**Process**:
1.  **Role-Scoped Exploration**: An agent or developer assumes a generic role and attempts to perform the core "Golden User Story" for that role. [your story here]
2.  **Gap Identification**: Document every moment where the software fails to meet a role's needs.
    - **Technical Gaps**: Broken links, 404s, console errors.
    - **Functional Gaps**: Missing buttons, data silos, lack of permissions.
    - **UX Gaps**: Confusing navigation, lack of feedback, "Coming Soon" placeholders.
3.  **Baseline Scoring**: Rate the role's experience on a 0-5 scale across 5 key capabilities. [adapt for your domain]
4.  **Theme Extraction**: Identify cross-role patterns that indicate systemic architectural issues.

**Outputs**:
- Role-Based Evaluation Documents. [replace with your file names]
- Aggregate Scorecard showing the "Platform Average."

**Quality Gate**: Every identified gap must be traceable to a specific file or line of code in the current repository. No "vague" complaints allowed.

**WHY**: Without a baseline, development is aimless. Evaluating the "clay" before designing the "mold" ensures we know exactly where the software is currently too rigid or too thin to support a real user.

> **Case Study: NorthStar** — The initial evaluation revealed that while the underwriting math was solid, the "Admin Console" was a shell, forcing the COO to use developer tools for user management. This transformed a "UX improvement" into a "P1 Adoption Blocker."

---

### Step 2: Persona Template Design
**Purpose**: To create a standardized, high-fidelity structure for personas that forces depth and prevents "flat" character sketches. A "CIA-legend" persona is a complete professional and psychological biography that can withstand the scrutiny of a critical reviewer.

**Process**:
1.  **Structural Specification**: Define the required sections for every persona (Identity, Career Arc, Defining Failure, Psychology, Legacy Workflow, Current Experience). [placeholder for your sections]
2.  **Rubric Standardization**: Define the 5 scorecard capabilities for each role to ensure consistent evaluation. [insert your capabilities]
3.  **Constraint Definition**: Establish rules to prevent duplication (e.g., MBTI uniqueness, question uniqueness).
4.  **Migration Table Format**: Design a table that maps the transition from legacy to new (Workflow Step | Legacy Tool | Time | New Equivalent | Status | Delta).

**Outputs**:
- Master Persona Template (See Template A in Appendix).
- Per-role scorecard rubrics.

**Quality Gate**: The template must include a "Before" section that is strictly decoupled from the "After" section. This prevents the persona from "knowing" about the new software while they are describing their legacy life.

**WHY**: Standardizing the "mold" ensures that every persona provides a consistent level of pressure against the software. If the mold is shallow, the software will be shallow.

---

### Step 3: Creative Direction System
**Purpose**: To provide a "soul" to the personas, ensuring they act as distinct human beings with unique biases and habits rather than generic "user types." This system provides the "texture" for the mold.

**Process**:
1.  **Character Differentiation Toolkit**: Define a set of "Screen-Loading Behaviors" and "Physical Habits" that can be assigned to personas.
2.  **Emotional Arc Assignment**: Assign specific emotional journeys (e.g., Vindicated Skeptic, Betrayed Champion) to prevent a monoculture of "happy users."
3.  **Legacy Tool Emotional Signatures**: Characterize common legacy tools as personalities (e.g., Excel as the "Security Blanket").
4.  **Backstory Authenticity Rules**: Define untapped human experience categories (e.g., Career Pivot Regret, Imposter Syndrome).

**Outputs**:
- Creative Direction Toolkit (See Toolkit below).

**WHY**: Software is used by people, not roles. By embedding "Physical Habits" and "Emotional Arcs," we force the agent to simulate the *friction* of real-world use, which exposes UX flaws that a "perfect" user would never find.

#### Creative Direction Toolkit (Generalized)

**1. Screen-Loading Behavior** (What they notice FIRST when a page renders):
- **The Number Scanner**: Eyes go straight to figures and deltas. If a number looks "off," they stop everything.
- **The Layout Reader**: Scans structure and navigation first. They need to know "where am I?" before "what is this?"
- **The Status Checker**: Looks for alerts, notifications, and badges. They are driven by urgency.
- **The Skeptic Squinter**: Leans forward, looking for what's wrong in the fine print.
- **The Speed Scroller**: Scrolls to the bottom to gauge page length, then scrolls back up.
- **The Hesitant Hoverer**: Moves mouse slowly, hovers before clicking, reads tooltips.

**2. Physical Habits During Software Use**:
- **Dual-Monitor Orchestrator**: Drags windows between screens constantly.
- **Single-Screen Tab Switcher**: High-frequency Alt-Tab rhythm.
- **Notebook Annotator**: Writes physical notes while reading the screen.
- **Screenshot Collector**: Captures screens compulsively for "proof."
- **Phone-in-Hand Validator**: Checks a mobile device to cross-reference data.
- **iPad Touch-First**: Tries to swipe/tap, forgets they're on desktop.

**3. Relationship to Technology** (Emotional posture):
- **The Builder**: "Software is a tool I shape to my needs."
- **The Skeptic**: "Software lies until proven honest."
- **The Dependent**: "I can't function without my tools."
- **The Reluctant Adopter**: "I'll use it when I have to."
- **The Optimizer**: "I'll use it if it's faster."

**4. Internal Monologue Voice** (How their thoughts read):
- **Terse, decisive**: *"Wrong number. Who touched this?"*
- **Anxious, relationship-aware**: *"If they see this, I'm done."*
- **Engineer-analytical**: *"11.2% IRR. Let me stress the exit cap."*
- **Process-checklist**: *"Step 4 of 12. Update the milestone. Next."*
- **Precision-obsessed**: *"$31,800 ≠ $47,200. Unacceptable."*

**5. Emotional Arcs**:
- **The Vindicated Skeptic**: Doubted the new tool, was right.
- **The Betrayed Champion**: Advocated for the tool internally, now feels exposed by its failures.
- **The Pragmatic Adapter**: Shrugs, finds workarounds, doesn't complain.
- **The Silent Abandoner**: Uses it once, finds errors, never returns.
- **The Newcomer Explorer**: No legacy bias, discovers the product fresh.

**6. Legacy Tool Emotional Signatures**:
- **Excel**: The security blanket. "I know every cell. It never surprises me."
- **Legacy ERP**: The reliable workhorse. "Heavy, opinionated, sometimes slow—but it WORKS."
- **Modern SaaS**: The flexible friend. "It does whatever I want, but it'll snap under pressure."
- **Institutional Software**: The devil you know. "Ugly, complex, expensive—but it does the core math RIGHT."

---

### Step 4: Persona Generation with Quality Loop
**Purpose**: To produce the high-fidelity personas using a "Creative-Critical" loop that ensures both depth and authenticity. This step is where the "mold" is actually cast.

**Process**:
1.  **Creative Draft (The Creative Agent)**: A "Creative Agent" generates the persona's backstory, psychology, and "Before" workflow based on the template and creative direction. [your prompt here]
2.  **Critical Review (The Critical Reviewer)**: A "Critical Reviewer" challenges the draft. Is the legacy workflow too generic? Are the "Uncomfortable Questions" too soft?
3.  **Revision**: The Creative Agent sharpens the persona based on the critique, adding granularity and sharpening the critical edge.
4.  **Finalization**: The persona is written to the role-specific file, and the Migration Completeness Table is updated.

**Outputs**:
- Role-Specific Persona Files. [replace with your file paths]
- One complete task specification example.

**Quality Gate**: Every persona must identify at least one "NEW GAP" not found by previous evaluations. If a persona only echoes existing gaps, it is considered redundant and must be revised or replaced.

**WHY**: A single agent generating multiple personas will inevitably produce "voice homogeneity." The Generative-Critical loop introduces the necessary friction to keep the personas distinct and genuinely critical.

> **Case Study: NorthStar** — A Creative Agent drafted an Office Manager persona who was "frustrated." The Critical Reviewer demanded she be "scared" of breaking the database because she didn't understand the underlying tech. This led to the discovery of a missing "Undo" button for critical actions.

---

### Step 5: Persona-to-Backlog Bridge
**Purpose**: To convert the narrative insights and "Uncomfortable Questions" from the personas into a prioritized, actionable product backlog. This step is the "translation layer" between the human-centric mold and the technical-centric implementation.

**Process**:
1.  **Gap Extraction**: Extract every "Missing," "Broken," or "Partial" item from the Migration Completeness Tables.
2.  **Prioritization (P0-P3)**:
    - **P0 (Existential)**: Data shown to external parties is wrong; regulatory/legal risk.
    - **P1 (Adoption Blocker)**: Prevents a role from using the software as their primary tool.
    - **P2 (Friction)**: Forces workarounds but doesn't fully block adoption.
    - **P3 (Enhancement)**: Quality of life improvements.
3.  **Traceability Mapping**: Link every backlog item back to the specific persona(s) who exposed it.
4.  **The Counter-Intuitive Score Narrative**: Document the "Score Decline." (A decline in score often means you've successfully mapped the "unknown unknowns").

**Outputs**:
- Persona-to-Backlog Bridge Document. [replace with your document name]
- Prioritized Backlog.

**Quality Gate**: Every P0 item must be traceable to at least two distinct personas. This prevents "outlier" opinions from driving critical product decisions.

**WHY**: Documentation that isn't operationalized is waste. The Bridge ensures that the "pain" of the personas is converted directly into the "work" of the developers.

> **Case Study: NorthStar** — The platform score declined from 2.1 to 1.1 after high-fidelity personas were applied. This wasn't a failure; it was a success. It proved the methodology had successfully mapped the "unknown unknowns" of the user's reality, such as the fact that "Committed" capital was being displayed as "Invested," causing investor panic.

---

### Step 6: Validation Infrastructure (Software Factory)
**Purpose**: To create a "Three-Zone" architecture where human-reviewed core logic is protected from agent-generated UI and service code. This step provides the "safety net" for rapid, agent-driven development.

**Process**:
1.  **Zone 1: Golden Module (Human-Reviewed)**: Identify the "fiduciary" or core logic files that must never be agent-generated without human oversight. [insert your files]
2.  **Zone 2: Factory-Grown Code**: Define the areas where agents can work without human code review (UI components, pages, hooks, services). [placeholder for your scope]
3.  **Zone 3: Human-Authored Specs**: Create a library of scenarios and property tests that validate the Factory's output. [adapt for your domain]
4.  **Property Testing**: Implement invariant tests that run across 1000+ random valid inputs to ensure the "math" is always correct.

**Outputs**:
- Software Factory Infrastructure. [replace with your directory]
- Factory Principles (e.g., Golden Module Boundary, Scenarios as Holdout Sets).

**Quality Gate**: The Golden Module must pass 100% of property tests before any Zone 2 code is accepted.

**WHY**: In complex domains, "it looks right" isn't enough. The Software Factory provides the mathematical "floor" that allows agents to move fast in the UI layer without risking the integrity of the core data.

> **Case Study: NorthStar** — NorthStar identified 9 "Golden Module" files (e.g., `waterfall.ts`, `irr.ts`) that agents were forbidden from editing. This ensured that even if an agent built a beautiful new UI, the underlying financial math remained audited and correct.

---

### Step 7: Execution Planning
**Purpose**: To design a multi-wave execution plan that addresses the P0 and P1 gaps identified in the Bridge. This step is the "blueprint" for implementation.

**Process**:
1.  **Wave Definition**: Group backlog items into logical waves (Foundation, Infrastructure, Page Builds, Integration). [placeholder for your waves]
2.  **Dependency Mapping**: Identify the critical path (e.g., DB Migration → Types → Shared Hooks → Pages).
3.  **Agent Dispatch Summary**: Define the recommended agent profile and skills for each task. [insert your agent profiles]
4.  **Verification Strategy**: Define how each task will be verified without human intervention (Playwright, Vitest, Bash, LSP).

**Outputs**:
- Execution Plans. [replace with your plan paths]

**Quality Gate**: Every plan must include a "Must NOT Do" section to prevent scope creep.

**WHY**: Rushing into implementation without a plan leads to "spaghetti features." Execution planning ensures that the most critical gaps are solved first.

---

### Step 8: Implementation and Verification
**Purpose**: To execute the plan and verify that the "clay" (software) now fits the "mold" (persona). This is the final step in the development lifecycle.

**Process**:
1.  **Atomic Implementation**: Execute tasks one by one, following the "Must Do" and "Must NOT Do" guardrails.
2.  **Automated Verification**: Run the verification strategy for each task (Playwright screenshots, Vitest logic checks, Bash structural checks).
3.  **LSP Diagnostics**: Ensure all changed files are clean of errors and warnings.
4.  **Persona Re-Evaluation**: Re-run the persona against the new code to verify that the "Uncomfortable Questions" can now be answered positively.

**Outputs**:
- Updated Codebase.
- Verification Evidence. [replace with your evidence directory]

**Quality Gate**: 100% pass rate on all verification scenarios. No task is "completed" until the evidence is captured and the build passes.

**WHY**: Implementation is only complete when it is verified. By using automated tools to "see" what the persona sees, we close the loop between the requirements and the final product.

---

## Role Case Studies: Methodology in Action

To illustrate the impact of Persona-Driven Development, we examine how the methodology transforms requirements for various organizational roles.

### 1. The Administrator (COO / Managing Partner)
**The Mold**: A COO with 15 years of experience who scans for numbers first and uses dual monitors to orchestrate firm operations.
**The Legacy Reality**: Lives in Airtable and PowerPoint. Spends 3 days every quarter manually assembling board decks.
**The Discovery**: The methodology exposed that the "Admin Console" was a shell. The "Uncomfortable Question" was: "If a junior associate changes a critical assumption, how do I know?"
**The Software Deformation**: Added a robust Audit Log and an in-app User Management suite, moving from a "spectator" tool to a "command center."

### 2. The Analyst (Junior Underwriter)
**The Mold**: A precision-obsessed senior analyst who squints at the screen looking for errors.
**The Legacy Reality**: Spends 4 hours per deal manually transcribing data from PDFs into Excel.
**The Discovery**: The "Napkin Calculator" was excellent for math but failed at "Data Ingestion." The "Uncomfortable Question" was: "Why am I still typing 200 line items from a civil engineer's budget?"
**The Software Deformation**: Implementation of a CSV/PDF ingestion pipeline for budgets and pro formas.

### 3. Investor Relations (VP of IR)
**The Mold**: A relationship-aware VP who is anxious about stakeholder trust.
**The Legacy Reality**: Uses a standalone CRM and Google Sheets. Spends the day in a "read-only" trap in the new software.
**The Discovery**: The methodology revealed that `canEditData: false` made IR a spectator. The "Uncomfortable Question" was: "If a client commits on the phone, why do I have to log into a second system to record it?"
**The Software Deformation**: Permissions were updated to allow IR to edit CRM and commitment data directly.

### 4. Business Development (SVP of Acquisitions)
**The Mold**: An engineer-analytical SVP who builds his own tools.
**The Legacy Reality**: Uses a 23-tab Excel master model and a physical whiteboard for pipeline visualization.
**The Discovery**: The SVP was "capital blind." He was sourcing deals without knowing if the firm had the "dry powder" to close them.
**The Software Deformation**: Added a "Fund Availability" widget to the BD dashboard, aligning sourcing with capital appetite.

### 5. Project Manager (Director of Development)
**The Mold**: A process-checklist Director who treats specialized construction software as oxygen.
**The Legacy Reality**: Manages $100M+ in construction but was locked out of the "Finance" side of her own projects.
**The Discovery**: The "Three-Page Prison." PMs only saw 3 sidebar items. The "Uncomfortable Question" was: "Did we pay the architect yet? I have to email the CFO to find out."
**The Software Deformation**: PMs were granted access to project-specific accounting and budget-vs-actual reports.

### 6. Finance (CFO / Controller)
**The Mold**: A CPA who believes "software lies until proven honest."
**The Legacy Reality**: Manages 15+ entities in a legacy ERP. Reduced the monthly close from 22 steps to 8 days.
**The Discovery**: The "Ghost" Bank Reconciliation. The page existed but had no matching engine. The "Uncomfortable Question" was: "How do I lock a period so an analyst doesn't change last year's entries?"
**The Software Deformation**: Implementation of a hard "Period Lock" and a functional bank reconciliation engine.

### 7. External Investor (Family Office MD)
**The Mold**: A family office MD who expects "Goldman-level" reporting.
**The Legacy Reality**: Uses high-end portfolio aggregation tools. Is a "Silent Abandoner" if she sees errors.
**The Discovery**: The "Static Data Trap." The portal showed "Committed" as "Invested," causing genuine investor panic.
**The Software Deformation**: The data layer was refactored to distinguish between commitment, funded capital, and distributions.

### 8. External Lender (Bank VP)
**The Mold**: A Bank VP who cares only about risk and covenants.
**The Legacy Reality**: Uses core banking systems and red pens. Prints everything.
**The Discovery**: The "Null Covenant Crisis." The portal showed `[null]` for DSCR and LTV, which the VP interpreted as a "Technical Default" signal.
**The Software Deformation**: A bridge was built between the Accounting module (NOI) and the Lender Portal to auto-calculate covenants.

---

## Reusable Templates (Appendix)

### Template A: Persona Template
```markdown
# Persona Legend: [Name] — [Role] ([Title])

## PART A: THE LEGEND

### Identity & Background
- **Name**: [Full Name], [Age]
- **Education**: [Degrees, Certifications]
- **Career Arc**: [Minimum 3 stops with companies, titles, and years]
- **Defining Failure**: [Specific professional failure with $ amounts and consequences]
- **Defining Triumph**: [Specific professional success with measurable outcomes]
- **Motivation**: [Why they are in their current role]

### Behavioral Psychology
- **MBTI**: [4-letter type with archetype name]
- **Big Five**: [Openness, Conscientiousness, Extraversion, Agreeableness, Neuroticism]
- **Decision Style**: [e.g., Data-driven, Relationship-driven]
- **Software Reaction**: [What they do when software fails]
- **Physical Habit**: [From Toolkit]
- **Screen-Loading Behavior**: [From Toolkit]

## PART B-0: BEFORE [PRODUCT NAME] (Legacy Workflow)
*This section documents the persona's FULL daily workflow using ONLY their legacy tools. No mentions of the new software.*

### Morning Routine
[What they check first, in what order]

### Tool Sequence
1. **[Tool 1]**: [Action taken, time spent]
2. **[Tool 2]**: [Action taken, time spent]
3. **[Tool 3]**: [Action taken, time spent]

### Handoff Friction
[Who do they wait on? For what? How long? What breaks?]

### Legacy Pain Score
[1-5 rating of the current process]

## PART B: A DAY IN [NAME]'S LIFE ([PRODUCT NAME])
*This section documents the persona's experience WITH the new software.*

### First-Screen Reaction
[What they notice first, per their Screen-Loading Behavior]

### Primary Task Attempt
[Step-by-step narrative of their main goal]

### Dead-End Discovery
[At least one moment where the software fails them]

### Internal Monologue
*[Italicized thoughts reflecting their voice and emotional arc]*

## PART C: THE UNCOMFORTABLE QUESTIONS
*Minimum 5 questions, maximum 7. Written in the persona's voice.*

1. "[Question 1 targeting Gap A]"
2. "[Question 2 targeting Gap B]"
3. "[Question 3 targeting Gap C]"
4. "[Question 4 targeting Gap D]"
5. "[Question 5 targeting Gap E]"

## PART D: SCORECARD
| Capability | Score (0-5) | Notes |
|------------|-------------|-------|
| [Capability 1] | X | [Specific observation] |
| [Capability 2] | X | [Specific observation] |
| [Capability 3] | X | [Specific observation] |
| [Capability 4] | X | [Specific observation] |
| [Capability 5] | X | [Specific observation] |
| **Average** | **X.X** | **[VERDICT]** |

**Verdict Scale**:
- 4.0-5.0: PASS
- 2.5-3.9: CONDITIONAL PASS
- 1.0-2.4: FAIL
- 0.0-0.9: CRITICAL FAIL
```

### Template B: Scorecard Rubric
| Capability | Description | [placeholder] Role |
|------------|-------------|-------------------|
| **Workflow Coverage** | Can the user complete their core "Golden User Story" without workarounds? | [e.g. Admin] |
| **Data Integrity** | Is the data shown accurate, drill-downable, and trustworthy? | [e.g. Finance] |
| **Audit & Controls** | Does the system provide audit trails, locks, and permission enforcement? | [e.g. Compliance] |
| **Role Fit** | Does the view surface the right data at the right level of detail? | [e.g. Executive] |
| **Adoption Likelihood** | Would this persona actually use the tool daily, or revert to legacy tools? | [All Roles] |

### Template C: Migration Completeness Table
| Workflow Step | Legacy Tool | Time (Legacy) | [Product] Equivalent | Status | Time ([Product]) | Delta | Innovation Opportunity |
|---------------|-------------|---------------|----------------------|--------|------------------|-------|------------------------|
| [Step Name] | [e.g. Excel] | [e.g. 2 hrs] | [Feature Name] | [Missing/Partial/Replaced/Broken] | [e.g. 1.5 hrs] | [e.g. +30m] | [Replicate/Reimagine/Skip] |

### Template D: Task Specification
```markdown
## Task: [Task Name]
- **Persona Owner**: [Name of Persona who exposed this gap]
- **Problem**: [Description of the gap/friction as experienced by the persona]
- **Must Do**:
  - [Requirement 1: Technical fix]
  - [Requirement 2: UX improvement]
  - [Requirement 3: Data validation]
- **Must NOT Do**:
  - [Guardrail 1: Avoid specific anti-pattern]
  - [Guardrail 2: Do not break existing functionality]
- **Verification**:
  - [ ] [Playwright Scenario: Verify X can now do Y]
  - [ ] [Vitest: Logic check for Z]
  - [ ] [LSP Diagnostics Clean]
```

### Template E: Creative Direction Brief
```markdown
# Creative Direction Brief: [Batch Name]
- **Target Roles**: [List of roles to be generated]
- **Core Theme**: [e.g., "The Trust Crisis," "The Efficiency Bottleneck"]
- **Required Arcs**: [e.g., 2x Vindicated Skeptic, 1x Betrayed Champion]
- **Tool Signatures**: [Define how legacy tools should be characterized for this batch]
- **Constraint**: No two personas may share more than 2 toolkit elements.
- **Goal**: Identify at least [N] new gaps in the [Module Name].
```

---

## Case Study Boxes (NorthStar Examples)

> **Case Study: NorthStar** — **Step 1 (Evaluate)**: The initial evaluation of the "Investor Portal" revealed that while the UI was sleek, the "Distributions" tab was hardcoded to "No distributions yet," even for active investors. This turned a "Visual Polish" task into a "P0 Data Integration" task.

> **Case Study: NorthStar** — **Step 4 (Generate)**: By assigning the "Skeptic Squinter" behavior to a Lender persona, the methodology exposed that the portal showed `[null]` for DSCR and LTV. To a banker, a null covenant is a "Technical Default" signal, which would have been missed by a "Happy Path" user.

> **Case Study: NorthStar** — **Step 5 (Bridge)**: The methodology revealed that the platform score declined from 2.1 to 1.1 after high-fidelity personas were applied. This was a success: it proved the "mold" was deep enough to expose "unknown unknowns" like the fact that "Committed" capital was being displayed as "Invested," causing investor panic.

> **Case Study: NorthStar** — **Step 6 (Factory)**: To protect "fiduciary math," NorthStar identified 9 "Golden Module" files (e.g., `waterfall.ts`, `irr.ts`) that agents were forbidden from editing, ensuring financial integrity while allowing rapid UI iteration.

> **Case Study: NorthStar** — **Step 8 (Verification)**: A Playwright test was used to verify that a Project Manager could finally see the "Underwriting" tab, which had previously been hidden by a binary permission check, solving a "Critical Fail" for that role.

---

## Adapting the Methodology

### B2B SaaS (Enterprise)
In enterprise SaaS, the "Legacy Tool" is often a complex ERP or a "Frankenstein" of spreadsheets. Focus heavily on **Step 5 (Bridge)** to ensure the product roadmap is driven by user pain rather than feature parity with competitors. Use **Step 3 (Creative Direction)** to simulate the "inter-office tension" between different departments. [adapt for your team]

### Consumer Applications
For consumer apps, the "Legacy Tool" might be a physical habit or a competing app. Focus on **Step 3 (Creative Direction)** to map the emotional triggers and "Screen-Loading Behaviors" that drive retention. Use **Step 4 (Generate)** to create personas with varying levels of tech-savviness. [your users here]

### Internal Tools
Internal tools often suffer from "Good Enough" syndrome. Use **Step 1 (Evaluate)** and **Step 8 (Verification)** to prove that the new tool actually saves time compared to the manual process it replaces. Use the **Migration Completeness Table** to ensure no critical edge cases are lost in the transition. [replace with your metrics]

### Greenfield vs. Brownfield
- **Greenfield**: Use Step 4 (Generation) to "hallucinate" the user's legacy reality (e.g., "how they do this in their head or on paper") to define the initial requirements.
- **Brownfield**: Use Step 2 (Template) to map the existing software as the "Before" state for a major refactor. This ensures the refactor doesn't break the workflows users already rely on. [insert your legacy system]

---

## The Psychology of Software Adoption

PDD recognizes that software adoption is as much a psychological challenge as a technical one. By mapping the "Emotional Arc" and "Relationship to Technology," we can predict where users will resist the new software.

### Common Psychological Profiles

| Profile | Software Reaction | Adoption Strategy |
| :--- | :--- | :--- |
| **The Builder** | "I'll build my own Excel model." | Provide powerful export/API capabilities. |
| **The Skeptic** | "The software is lying to me." | Focus on audit trails and data transparency. |
| **The Dependent** | "I can't work without my legacy tool." | Ensure 100% feature parity for core tasks. |
| **The Reluctant Adopter** | "This is just more work for me." | Focus on automation and time-saving features. |

---

## Measuring Success with PDD

Success in PDD is not measured by "features shipped," but by "mold satisfaction."

### Key Performance Indicators (KPIs)

1.  **Persona Score Delta**: The difference between the "Before" and "After" scores for a persona.
2.  **Migration Completeness %**: The percentage of legacy workflow steps successfully replaced or reimagined.
3.  **Uncomfortable Question Resolution Rate**: The percentage of persona questions that can now be answered positively.
4.  **Adoption Velocity**: The time it takes for a real user matching a persona to move from the legacy tool to the new software.

---

## Common Pitfalls and How to Avoid Them

1.  **The "Happy Path" Bias**: Creating personas that are too easy to please.
    - *Fix*: Use the Critical Reviewer loop to sharpen the persona's edge.
2.  **The "Feature Factory" Trap**: Building every legacy feature without reimagining the workflow.
    - *Fix*: Use the "Innovation Opportunity" column in the Migration Table.
3.  **Documentation Rot**: Letting personas become outdated as the product evolves.
    - *Fix*: Re-run Step 8 (Verification) after every major release.
4.  **Homogeneity**: All personas sounding the same.
    - *Fix*: Enforce MBTI and Emotional Arc constraints in Step 3.

---

## Integrating PDD with Agile/Scrum

PDD is designed to complement existing Agile workflows.

- **Backlog Refinement**: Use the Persona-to-Backlog Bridge to prioritize the product backlog.
- **Sprint Planning**: Use Task Specifications (Template D) as the basis for user stories.
- **Sprint Review**: Use the persona's "Uncomfortable Questions" as the acceptance criteria for the demo.
- **Definition of Done**: A story is not done until it passes the automated verification defined in Step 8.

---

## The PDD Maturity Model

Organizations can track their PDD adoption through four levels of maturity.

### Level 1: Ad-Hoc
- Personas are marketing sketches.
- Testing is "happy path" only.
- No "Before" state documentation.

### Level 2: Structured
- Standardized persona templates used.
- Role-based evaluations performed.
- Basic migration tables created.

### Level 3: Executable
- CIA-legend depth personas.
- Generative-Critical loops for generation.
- Prioritized backlog linked to personas.

### Level 4: Automated
- Software Factory in place.
- Automated verification against persona requirements.
- Real-time "Mold Satisfaction" tracking.

---

## PDD for Different Team Sizes

### Solo Developer
- **Focus**: Use AI agents to generate personas and run verification tests.
- **Benefit**: Provides a "virtual team" of critics to prevent tunnel vision.

### Small Team (2-10)
- **Focus**: Assign one person as the "Persona Architect" to maintain the mold.
- **Benefit**: Ensures consistency across features and reduces rework.

### Large Organization (100+)
- **Focus**: Create a "Persona Library" that can be reused across different product lines.
- **Benefit**: Standardizes the user experience and ensures institutional knowledge is captured.

---

## PDD and the Human-Review Boundary

In AI-driven development, it is critical to define where the AI stops and the human begins. PDD uses the **Golden Module** concept to define this boundary.

- **Zone 1 (Human Only)**: Critical logic, fiduciary math, security protocols.
- **Zone 2 (AI with Human Review)**: Complex UI, data migrations, service integrations.
- **Zone 3 (AI Autonomous)**: Simple UI components, documentation, unit tests.

---

## Case Study: The Evolution of a Feature

### Phase 1: The Request
A user asks for a "Dashboard."

### Phase 2: The PDD Evaluation
The "Admin" persona (Sarah) attempts to use the dashboard. She finds that she can't see who changed the data.

### Phase 3: The Software Deformation
The "Dashboard" is reshaped to include an "Audit Log" and "Change Tracking," satisfying Sarah's "Uncomfortable Question."

---

## PDD for Different Industries

While PDD was born in the complex world of Real Estate Private Equity, it is applicable across many domains.

### Healthcare
- **Personas**: Surgeons, Nurses, Billing Specialists.
- **Legacy Tools**: Paper charts, legacy EMRs, pagers.
- **Critical Math**: Dosage calculations, patient vitals.

### Finance / Fintech
- **Personas**: Traders, Compliance Officers, Retail Investors.
- **Legacy Tools**: Bloomberg Terminal, Excel, legacy banking portals.
- **Critical Math**: Risk models, interest calculations, tax lot tracking.

### Manufacturing / Supply Chain
- **Personas**: Floor Managers, Logistics Coordinators, Procurement Officers.
- **Legacy Tools**: Whiteboards, legacy ERPs, phone calls.
- **Critical Math**: Inventory levels, lead times, shipping costs.

---

## PDD and the Ethics of AI Personas

As we use AI to simulate human behavior, we must consider the ethical implications.

1.  **Bias Mitigation**: Ensure personas represent a diverse range of backgrounds and abilities.
2.  **Authenticity vs. Stereotype**: Avoid falling into lazy stereotypes when creating backstories.
3.  **Data Privacy**: Do not use real user data to train or generate personas without explicit consent.

---

## PDD for Legacy System Modernization

PDD is the ultimate tool for "strangler pattern" migrations.

1.  **Map the Legacy**: Use Step 2 to create a high-fidelity mold of the legacy system.
2.  **Build the Bridge**: Use Step 5 to identify which legacy features are "load-bearing" and which are "vestigial."
3.  **Verify the Fit**: Use Step 8 to ensure the new system satisfies the legacy mold before decommissioning the old one.

---

## PDD and the Future of Work

As software becomes more specialized, the "one size fits all" approach is dying. PDD paves the way for **Hyper-Personalized Software**.

1.  **Role-Specific Interfaces**: Software that morphs based on the user's persona.
2.  **Adaptive Workflows**: Systems that learn from the user's "Physical Habits" and adjust accordingly.
3.  **AI Co-Pilots**: Agents that understand the user's "Emotional Arc" and provide support during high-stress tasks.

---

## PDD and the Future of AI Agents

As AI agents become more capable, PDD will evolve from a manual methodology to an automated system.

1.  **Synthetic User Testing**: AI agents will "live" in the software for weeks, simulating months of usage and identifying long-term friction points.
2.  **Real-Time Requirement Evolution**: As real users interact with the software, the "mold" will automatically update to reflect new habits and needs.
3.  **Generative UI**: The software will "deform" itself in real-time to fit the specific persona of the user currently logged in.

---

## PDD and the Concept of "Software as a Solution" (SolS)

PDD moves us away from "Software as a Service" (SaaS) toward "Software as a Solution" (SolS).

- **SaaS**: Provides a set of tools that the user must learn to use.
- **SolS**: Provides a solution that fits into the user's existing life with zero friction.

PDD is the engine that drives this transition by ensuring that the software is built to solve the user's *actual* problems, not just provide a set of generic features.

---

## The Importance of the "Critical Reviewer"

In Step 4, the Critical Reviewer is the most important role. Without a cynical, precision-obsessed critic, the personas will default to "happy path" users who are too easy to please.

### Critical Reviewer Checklist:
1.  **Genericism**: Is the legacy workflow too vague? (e.g., "checks email" vs "reviews the RFI queue").
2.  **Softness**: Are the uncomfortable questions actually uncomfortable?
3.  **Redundancy**: Does this persona identify a NEW gap?
4.  **Authenticity**: Does the backstory feel like a real human life?

---

## The Power of "Uncomfortable Questions"

Uncomfortable questions are the "executable specifications" of PDD. They are the sharp points of the mold that press against the software.

### Anatomy of a Good Uncomfortable Question:
- **Voice**: Written in the persona's unique internal monologue style.
- **Grounded**: References a specific page, button, or data field in the codebase.
- **Pointed**: Targets a gap that prevents the user from completing their core task.
- **Cynical**: Assumes the software is failing until proven otherwise.

---

## The Concept of "The Golden User Story"

In Step 1, we define the "Golden User Story" for each role. This is the minimum viable utility required for that role to adopt the software.

### Examples of Golden User Stories:
- **Finance**: "Perform a monthly period close across 15 entities and generate audited financial statements." [adapt for your role]
- **Investor**: "Log in via magic link to view real-time capital account balance and download tax documents." [insert your story]
- **Admin**: "Manage firm-wide user access and monitor data integrity across all active projects." [replace with your story]

---

## Glossary of Terms

- **CIA-Legend**: A high-fidelity persona backstory with professional and psychological depth.
- **Golden User Story**: The minimum viable utility required for a role to adopt the software.
- **Migration Completeness**: A measure of how well the new software replaces the legacy workflow.
- **Software Factory**: The validation infrastructure that protects core logic from agent-generated code.
- **Golden Module**: A set of critical files that are protected from automated modification.
- **Uncomfortable Question**: A pointed question asked by a persona that targets a specific product gap.
- **Score Decline**: A phenomenon where high-fidelity personas reveal more gaps, leading to a lower (but more accurate) product score.
- **Persona Saturation**: The point at which adding new personas no longer identifies new product gaps.
- **Mold Satisfaction**: The degree to which the software fills the requirements defined by the persona mold.
- **Software Deformation**: The process of changing the software's shape to fit the persona mold.
- **Requirement Fidelity**: The degree to which a software requirement accurately reflects the user's reality.
- **The Read-Only Trap**: A common product gap where users can see data but cannot perform the actions they are responsible for.
- **The Three-Page Prison**: A common product gap where a role is restricted to a tiny subset of the application's functionality.

---

## FAQ

**How many personas do I need?**
Start with 3 per role. You have reached "Persona Saturation" when new personas stop identifying new gaps. For most roles, this occurs between 3 and 5 personas. If the 3rd persona finds the same gaps as the first two, you are done.

**What if there are no legacy tools?**
Every user has a "Before" state. If there is no software, the "Legacy Tool" is a legal pad, a whiteboard, a phone call, or a mental model. Document the *friction* of that manual process. The "Time (Legacy)" might be the time spent in meetings or on the phone.

**Can I skip the Software Factory?**
Only if your software has no "critical math" or "fiduciary logic." If a bug in your code can cost a user money, legal trouble, or physical harm, you need a Golden Module.

**How long does this take?**
A full PDD cycle for a new feature takes about 1 week of planning and 1-2 weeks of execution. The initial setup for a codebase takes 3-5 days. It is an investment that pays off by reducing rework and increasing adoption.

**Do I need multiple AI agents?**
You need at least two "perspectives." You can use one LLM with different system prompts for the Creative and Critical roles. The friction between these roles is what creates the "CIA-legend" quality.

**Can I use this for mobile apps?**
Yes. In Step 3 (Creative Direction), focus on "Thumb-Reach Zones" and "Interruption Frequency" instead of "Screen-Loading Behaviors" and "Dual Monitors."

**What if the persona score is 5.0?**
If a persona gives a 5.0, your mold is too shallow. Go back to Step 3 and add more "Physical Habits" or "Emotional Arcs" to find the friction points. A 5.0 in PDD is usually a sign of a "Happy Path" bias.

**Is PDD only for AI-driven development?**
No. While PDD is highly effective for guiding AI agents, it is equally valuable for human development teams who want to build more user-centric software.

**How do I handle conflicting persona requirements?**
PDD exposes these conflicts early. Use **Step 5 (Bridge)** to prioritize based on business value or create role-specific views to satisfy both requirements.

**Can I use PDD for marketing?**
While PDD is a development methodology, the high-fidelity backstories are excellent for creating targeted marketing copy and sales scripts.

**What is the difference between PDD and User-Centered Design (UCD)?**
PDD is an implementation-focused evolution of UCD. While UCD focuses on the interface, PDD focuses on the *executable specification* and the *migration completeness* of the entire workflow.

**How do I sell PDD to my stakeholders?**
Focus on the "Cost of Rework." Show them how PDD identifies critical gaps *before* they are built, saving thousands of dollars in development time and preventing user churn.

**Can PDD be used for hardware products?**
Yes. The "mold" would include the physical environment and ergonomic constraints of the user.

**What is the most important step in PDD?**
Step 5 (The Bridge). Without operationalizing the insights, PDD is just expensive documentation.

**How do I know if my persona is "CIA-legend" depth?**
If a critical reviewer can't find a single "fluff" sentence and the backstory includes a specific professional failure with a dollar amount, you are there.
