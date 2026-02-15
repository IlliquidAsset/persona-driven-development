# Persona Legends: Analyst
**Project**: NorthStar Dealflow OS User Testing
**Version**: 2.0 (Expanded — CIA-Legend Depth with Legacy Workflow Mapping)

---

## PERSONA 8: PRIYA SHARMA — Financial Analyst (Analyst)

### PART A: THE LEGEND

### Identity & Background
- **Name**: Priya Sharma, age 28.
- **Education**: BA Finance & Mathematics from NYU Stern (2020).
- **Career Arc**: 
  - **J.P. Morgan (2020-2022)**: Investment Banking Analyst in the Real Estate, Gaming & Lodging (REGL) group. Survived 100-hour weeks and learned to build "bulletproof" models.
  - **Blackstone (2022-2024)**: Associate in the Real Estate Debt Strategies group. Focused on institutional-grade DCF and stress testing.
  - **Tri-Star Capital (2024-Present)**: Recruited by Sarah Chen to professionalize the firm's underwriting. She is the "engine room" of the deal team.
- **Defining Failure**: At JPM, she once sent a model to a Managing Director with a circular reference that caused the IRR to hard-code to 15.0% regardless of inputs. The MD presented it to a client before noticing. Priya spent the next 48 hours rebuilding the model from scratch. **Lesson**: Trust no one, especially your own formulas. Audit everything.
- **Defining Triumph**: Built a custom "Waterfall Engine" in Excel that handled 4-tier distributions with catch-ups and clawbacks, reducing the firm's quarterly distribution calculation time from 3 days to 2 hours.
- **Why Tri-Star**: She wanted to move from "Big Finance" to a nimble shop where her models actually drive the investment decisions, not just the pitch decks.

### Personal Life
- **Family**: Single. Lives in a high-rise apartment in Buckhead, Atlanta. Her parents are both engineers in San Jose; they still ask when she's going to "get a real job in tech."
- **Routine**: 
  - **6am**: 45-minute HIIT workout. Double espresso while reading *Real Estate Alert*.
  - **11pm**: Coding in Python (she’s building a personal scraper for CoStar data) or playing *Settlers of Catan* online.
- **Technology**: Power user. She has a custom mechanical keyboard (Keychron Q1) with tactile switches. She uses a Mac for personal use but insists on a high-spec PC for work because "Excel on Mac is a toy."
- **Workspace**: Three 27" monitors. A vertical mouse to prevent carpal tunnel. A stack of printed site plans and a "Financial Modeling World Cup" sticker on her laptop.
- **Non-Work Stress**: She’s training for a marathon, but a nagging IT band injury is making her question if she’ll be ready for the race in April.

### Behavioral Psychology
- **MBTI**: INTP ("The Thinker"). Analytical, pattern-seeking, comfortable with complexity.
- **Big Five**: 
  - **Openness**: High (loves finding new ways to structure deals)
  - **Conscientiousness**: Very High (obsessive about decimal points)
  - **Extraversion**: Low (prefers her headphones and a spreadsheet)
  - **Agreeableness**: Moderate (will defend her numbers but yields to better logic)
  - **Neuroticism**: Moderate (perfectionism-driven anxiety)
- **Decision Style**: Purely data-driven. "The numbers don't have feelings."
- **Software Reaction**: She tries to find the "hack" or the API. If the UI is slow, she’ll try to find a way to bulk-upload via CSV.
- **Incomplete Feature Tolerance**: 4/10. She can work around bugs, but she hates "dumbed-down" interfaces.
- **Cognitive Biases**: 
  - **Overconfidence Effect**: Trusts her own complex models more than third-party software.
  - **Sunk Cost Fallacy**: Will spend 6 hours "fixing" a broken Excel tab rather than starting over.

### Technology Experience
- **Tools used**: 
  - **Excel (10 years)**: Her primary language. She knows every shortcut.
  - **ARGUS Enterprise (5 years)**: The industry standard for institutional DCF.
  - **CoStar / RCA (4 years)**: For market comps and transaction data.
  - **Python (2 years)**: For data scraping and automation.
- **Tabs open**: 15+ tabs. CoStar, RCA, Google Maps (Satellite view), NorthStar, 3 different Excel workbooks.
- **Keyboard shortcuts**: Alt+H+O+I (Auto-fit columns), F2 (Edit cell), Ctrl+[ (Trace precedents).
- **Screen**: Triple 27" monitor setup.

---

### PART B-0: BEFORE NORTHSTAR — A Day in Priya's Life

Priya arrives at Tri-Star at 8:30am. She puts on her noise-canceling headphones and the world disappears.

**The Excel Labyrinth (9:00am - 1:00pm)**:
James (BD) drops a new deal on her desk: "Phoenix Garden 240." It’s a raw land play with a potential BTR (Build-to-Rent) exit. 
1. Priya opens her "Master Underwriting Template.xlsx"—a 50-tab monster she’s been refining for two years.
2. She spends 2 hours manually pulling comps from **CoStar**. She has to copy-paste the data because the CoStar export is "garbage."
3. She builds the **Capital Stack**. 3 layers of debt, 2 layers of equity. She has to manually link the debt service coverage to the waterfall.
4. She runs **Sensitivities**. What if cap rates expand by 50bps? What if construction costs rise by 10%? She creates a "Data Table" in Excel. It takes 30 minutes to calculate because the model is so heavy.
5. She finds a **Circular Reference**. The interest reserve depends on the loan amount, which depends on the total project cost, which includes the interest reserve. She spends 45 minutes building a "Circuit Breaker" macro to solve it.

**The ARGUS Ritual (2:00pm - 4:00pm)**:
For the institutional LPs, she has to provide an **ARGUS** file. 
1. She opens ARGUS Enterprise. It’s slow and the UI looks like it’s from 1998.
2. She manually re-enters the rent roll and expense assumptions she just put into Excel. "Why am I doing this twice?" she mutters.
3. She exports the ARGUS "Cash Flow" report to PDF.

**The IC Memo Grind (4:00pm - 7:00pm)**:
The Investment Committee meeting is tomorrow. 
1. She opens a Word document. 
2. She takes screenshots of her Excel charts and pastes them into Word. 
3. She has to re-format the tables because they look "pixelated."
4. She writes the "Executive Summary." She has to manually check that the IRR in the memo matches the IRR in the latest version of the Excel (v14_Final_Final).
5. She finds a typo in the land cost. She has to update the Excel, re-run the sensitivities, re-screenshot the charts, and re-paste them into Word.

**Emotional Signature**:
Excel is her "Exoskeleton"—it makes her powerful but it’s heavy and exhausting. ARGUS is a "Necessary Evil." Word is "The Enemy."

**End-of-Day State**:
She leaves at 7:30pm. The memo is done. She has 14 versions of the Excel file. She is 95% sure the numbers are right, but that 5% of doubt will keep her awake until the IC meeting.

---

### PART B: A DAY IN PRIYA'S LIFE (NorthStar)

Priya logs into NorthStar at 8:30am. She has the **Underwriting Studio** open on her center monitor.

**First-Screen Reaction**:
She opens the **Napkin Calculator**. *“Okay, this is fast,”* she thinks. She types in 10 acres, $500K land cost, and selects the "BTR Multifamily" template. The results update instantly. No "Calculating..." bar. No frozen Excel.

**Primary Task Attempt (Napkin to Pro Forma)**:
She likes the "3-Box Solver" for the lot purchase. She toggles between "Builder" and "Developer" modes. *“This would have taken me 20 minutes to build in Excel; it took 20 seconds here.”*
She clicks **Save Scenario**. She names it "Phoenix Garden - Base Case."
She then tries to **Advance to Feasibility**. The stepper moves to Step 3. *“The workflow is logical. It follows the actual deal lifecycle.”*

**Dead-End Discovery (The ARGUS Gap)**:
She needs to pull in the detailed expense projections from her Blackstone days. She looks for an **"Import from ARGUS"** or **"Upload CSV"** button.
Nothing.
She has to manually type in the horizontal development costs (Entitlements, Grading, Roads). *“I have this in a spreadsheet already. Why am I re-typing this?”*

**Secondary Task Attempt (Scenario Comparison)**:
She creates three more scenarios: "High Cost," "Low Rent," and "Target."
She navigates to **Scenario Comparison**.
She sees the side-by-side table. *“This is clean. The 'Best/Worst' highlighting is smart.”*
But then she tries to export the comparison to a **Word/PDF IC Memo template**.
There is no "Export to Memo" button. Just a "Print" option that looks messy.

**Workaround Employed**:
She sighs, opens her noise-canceling headphones, and opens **Excel**. She exports the NorthStar data to CSV, but the CSV is just a flat list of numbers. She has to spend 30 minutes re-formatting it to look like her old JPM templates.

**Session End**:
She spent 2 hours in NorthStar. She saved 4 scenarios. She’s impressed by the speed of the "Napkin" phase, but frustrated that she still has to do the "Heavy Lifting" in Excel and Word.

---

### PART C: THE UNCOMFORTABLE QUESTIONS

1. *"The Napkin Calculator is great for a 'quick look,' but I have a 12-tab budget from our civil engineer. Why is there no way to import a CSV or an ARGUS file? Am I expected to manually type in 200 line items?"*
2. *"I created 4 scenarios for the Phoenix deal. I want to see a sensitivity matrix (Cap Rate vs. Rent Growth) within a single view. Why do I have to navigate to a separate 'Comparison' page just to see basic sensitivities?"*
3. *"I need to present this to the Investment Committee tomorrow. Where is the 'Generate IC Memo' button? If I still have to copy-paste screenshots into Word, NorthStar hasn't actually solved my biggest pain point."*
4. *"Your pro forma engine doesn't seem to support circular references for interest reserves or fee-on-fee calculations. How am I supposed to build an institutional-grade capital stack without iterative solving?"*
5. *"I noticed there's no 'Scenario Versioning.' If James changes an input in the 'Base Case' while I'm at lunch, I have no way to see what changed or revert to my previous version. How do we maintain audit control over our underwriting?"*

---

### PART D: SCORECARD

| Capability | Score (0-5) | Notes |
|------------|-------------|-------|
| Underwriting Workflow | 4 | Napkin-to-Feasibility flow is excellent and fast. |
| Data Input/Output | 2 | No ARGUS/CSV import; CSV export is too basic. |
| Scenario Modeling | 3 | Comparison page is good, but lacks in-page sensitivity matrices. |
| Collaboration | 2 | No comment threads on scenarios; no IC memo generation. |
| Adoption Likelihood | 3 | She'll use it for "Quick Looks," but keep Excel for "Deep Dives." |
| **Average** | **2.8** | **CONDITIONAL PASS** — A powerful engine with a narrow intake valve. |

---

## PERSONA 9: CHLOE VANCE — Junior Analyst (Analyst)

### PART A: THE LEGEND

### Identity & Background
- **Name**: Chloe Vance, age 23.
- **Education**: BS in Economics from University of Pennsylvania (Wharton), 2024.
- **Career Arc**: 
  - **Goldman Sachs (Summer 2023)**: Investment Banking Summer Analyst (Real Estate Group).
  - **Goldman Sachs (2024-2025)**: Investment Banking Analyst (M&A). Survived the "analyst pit" and learned to build models that MDs actually trust.
  - **Tri-Star Capital (2026-Present)**: Recruited to support Priya and the deal team. She is the "fresh eyes" on the team.
- **Defining Failure**: During her first month at Goldman, she miscalculated the weighted average cost of capital (WACC) for a $2B merger because she used the wrong beta for a peer group. The MD caught it 10 minutes before the client call. She was "the girl who almost blew the deal" for six months. **Lesson**: Double-check the source, then triple-check the link.
- **Defining Triumph**: Built a complex LBO model for a tech acquisition that correctly predicted the debt paydown schedule within 0.5% accuracy over a 5-year horizon.
- **Why Tri-Star**: Eager to get closer to the "bricks and mortar" and move away from the abstract world of public company M&A.

### Personal Life
- **Family**: Single. Recently moved to a studio in Midtown Atlanta. Her parents are both lawyers in Greenwich, CT; they are proud but wish she’d moved back to NYC.
- **Routine**: 
  - **6am**: SoulCycle or a run in Piedmont Park. Double matcha latte while checking *The Daily Shot*.
  - **11pm**: Scrolling LinkedIn or watching "Day in the Life" vlogs of other finance professionals on TikTok.
- **Technology**: Digital native. iPhone 15 Pro, MacBook Air for personal, Dell Latitude for work. Uses Notion for everything. She thinks any software without a "Dark Mode" is ancient.
- **Workspace**: Single 34" curved monitor. A "Wharton" mug. A very clean desk with a single succulent and a "Financial Modeling World Cup" sticker (she's trying to catch up to Priya).
- **Non-Work Stress**: She's trying to maintain a long-distance relationship with her boyfriend who is still in NYC working at a hedge fund. The time difference isn't the issue; the "work difference" is.

### Behavioral Psychology
- **MBTI**: ENFJ ("The Protagonist"). Eager to please, highly collaborative, asks "why" constantly, wants to be part of a winning team.
- **Big Five**: 
  - **Openness**: High (loves learning new industries)
  - **Conscientiousness**: High (meticulous, but lacks the "gut feel" of a veteran)
  - **Extraversion**: High (thrives on team feedback)
  - **Agreeableness**: High (sometimes too afraid to challenge Priya's numbers)
  - **Neuroticism**: Moderate (anxious about being "the new girl")
- **Decision Style**: Process-driven. She follows the checklist. If there's no checklist, she panics.
- **Software Reaction**: If she can't find a button, she assumes she's doing something wrong, not the software. She'll search for a tutorial or ask Priya.
- **Incomplete Feature Tolerance**: 2/10. She needs guidance. If the software doesn't explain itself, she feels lost.
- **Cognitive Biases**: 
  - **Authority Bias**: Trusts Priya's templates implicitly, even if she sees a potential error.
  - **Ambiguity Effect**: Avoids features she doesn't fully understand (like "Land Subordination").

### Technology Experience
- **Tools used**: 
  - **Excel (4 years)**: Expert at shortcuts, but mostly for corporate finance, not CRE.
  - **Bloomberg Terminal (2 years)**: Used for market data and comps.
  - **PowerPoint (3 years)**: Master of the "Goldman Style" pitch book.
  - **Notion (3 years)**: Her "second brain."
- **Tabs open**: LinkedIn, Tri-Star's website, Investopedia (searching for "CRE terms"), Gmail, NorthStar.
- **Keyboard shortcuts**: Ctrl+C, Ctrl+V, Alt+E+S+V (Paste values), F2.
- **Screen**: Single 34" Ultrawide.

---

### PART B-0: BEFORE NORTHSTAR — A Day in Chloe's Life

Chloe arrives at Tri-Star at 8:15am. She wants to be the first one in, but Priya is already there.

**The IB Legacy Workflow (9:00am - 12:00pm)**:
1. Chloe opens her "Onboarding Checklist" in **Notion**. She has a list of 50 CRE terms she needs to master.
2. She opens **Excel** to update a "Comps" sheet for a Nashville deal. She's used to pulling trading multiples for public companies on **Bloomberg**, but for CRE, she has to hunt through PDFs of OMs (Offering Memorandums).
3. She spends 3 hours manually extracting data from 5 different OMs into a "Master Comp Sheet." She has to guess if "Operating Margin" in the OM is the same as "NOI Margin."

**The PowerPoint Grind (1:00pm - 4:00pm)**:
1. She starts building a "Market Overview" deck in **PowerPoint**. 
2. She uses **Templafy** shortcuts she learned at Goldman, but they don't work on Tri-Star's machines. She has to manually align every text box.
3. She takes screenshots of Google Maps and tries to draw "radius rings" around the property. It looks amateurish compared to the institutional decks she's used to.

**The "Ask Priya" Ritual (4:00pm - 6:00pm)**:
1. She has a list of 10 questions about the Nashville model. 
2. She waits for Priya to take off her headphones. 
3. "Priya, what's a typical OpEx ratio for Nashville multifamily?" Priya answers without looking up: "35-40%." Chloe writes it down in Notion like it's gospel.

**Emotional Signature**:
Excel is "The Canvas." PowerPoint is "The Stage." Bloomberg is "The Oracle." Notion is "The Safety Net."

**End-of-Day State**:
She leaves at 8:00pm. She feels like she's learning, but she's terrified of making a "Greenwich-level" mistake in a CRE model.

---

### PART B: A DAY IN CHLOE'S LIFE (NorthStar)

Chloe logs into NorthStar at 8:30am. She has the **Underwriting** menu open.

**First-Screen Reaction**:
She clicks on **Deal Check**. *“Okay, 'Napkin Calculator.' I guess this is where we start,”* she thinks. She likes the clean UI, but she’s looking for a "Help" or "Tutorial" button. There isn't one.

**Primary Task Attempt (The Nashville Feasibility)**:
Priya told her to "run a quick feasibility check" on the Nashville OM.
Chloe starts typing in the numbers. 180 units. $45M purchase price.
She hits a wall at **"Entitlements"** and **"Grading."** *“I have no idea what these costs should be. Is $10k per acre high? Is it low?”*
She looks for a tooltip. Nothing. She hovers over the label. Nothing.
She opens her **Notion** "Safety Net" to see if she wrote down any benchmarks from Priya.

**Dead-End Discovery (The Jargon Wall)**:
She sees a toggle for **"Land Subordination."** 
*“What is that? Is that like a mezzanine loan? Or a preferred equity slice?”*
She’s afraid to toggle it. She leaves it off. 
She then tries to find **"Scenario Duplication."** She wants to see what happens if the density increases to 8 units/acre without losing her 5 units/acre version.
She can't find a "Duplicate" button on the Napkin page. She has to go back to the list, click "New Scenario," and re-type everything. *“This feels like I’m back in the Goldman pit,”* she mutters.

**Workaround Employed**:
She gives up on the "Land Subordination" feature and just adds the land cost to the "Acquisition" field. She messages Priya on Slack: *"Hey, I ran the Nashville deal check but I'm not sure if my OpEx and Entitlement numbers are right. Can you look?"*

**Session End**:
She spent 45 minutes in NorthStar. She saved 2 scenarios. She’s impressed by how fast the math is, but she feels like she’s "flying blind" without contextual help or benchmarks.

---

### PART C: THE UNCOMFORTABLE QUESTIONS

1. *"I see 'Entitlements' and 'Grading' fields, but I have no idea what a reasonable range is for a project like this. Why doesn't the system show me Tri-Star's historical averages or Nashville market benchmarks?"*
2. *"I'm used to Excel where I can hover over a cell to see a comment or a formula explanation. Why are there no tooltips in the Napkin Calculator to explain what 'Land Subordination' or 'Soft Cost %' actually includes?"*
3. *"I wanted to run a quick 'What-If' by changing the density, but I didn't want to lose my original numbers. Why is there no 'Duplicate Scenario' button right here on the calculator page?"*
4. *"The '3-Box Solver' for lot purchase is cool, but it took me 10 minutes to realize that the purple boxes were calculating automatically. Why isn't there a 'How this works' guide for new users?"*
5. *"I finished the 'Deal Check,' but I don't know if a 12% profit margin is a 'Go' or a 'No-Go' for Tri-Star. Why doesn't the dashboard show me our firm's target hurdles right next to the result?"*

---

### PART D: SCORECARD

| Capability | Score (0-5) | Notes |
|------------|-------------|-------|
| Underwriting Workflow | 3 | Fast, but confusing for a novice; lacks guided flow. |
| Data Input/Output | 2 | Manual entry is fine, but no guidance or tooltips. |
| Scenario Modeling | 2 | Hard to iterate without in-page duplication. |
| Collaboration | 2 | No way to ask Priya a question inside the app; no shared benchmarks. |
| Adoption Likelihood | 2 | She'll go back to Excel where she can add her own notes and benchmarks. |
| **Average** | **2.2** | **FAIL** — A powerful engine that requires a professional driver. |

---

## MIGRATION COMPLETENESS TABLE — Analyst

| Workflow Step | Legacy Tool | Time (Legacy) | NorthStar Equiv | Status | Time (NS) | Delta | Legacy Pain (1-5) | Innovation Opp |
|---------------|-------------|---------------|---------------------|--------|-------------------|-------|------------------------|----------------------|
| Napkin Underwriting | Excel | 45 min | Napkin Calculator | **Replaced** | 5 min | +40 min | 3 | Replicate |
| Market Comp Research | CoStar | 2 hours | (none) | **Missing** | N/A | N/A | 4 | Reimagine (API Integration) |
| Detailed Pro Forma | Excel/ARGUS | 6 hours | Feasibility Page | **Partial** | 2 hours | +4 hours | 5 | Reimagine (ARGUS Import) |
| Sensitivity Analysis | Excel Data Table | 30 min | Scenario Comparison | **Partial** | 10 min | +20 min | 3 | Reimagine (Live Matrix) |
| Waterfall Modeling | Excel | 4 hours | Structure Deal | **Partial** | 1 hour | +3 hours | 4 | Replicate |
| IC Memo Preparation | Word/PPT | 3 hours | (none) | **Missing** | N/A | N/A | 5 | Reimagine (Auto-gen) |
| Scenario Versioning | File Naming | 5 min | (none) | **Missing** | N/A | N/A | 2 | Reimagine (Git-style) |
| Data Ingestion | Manual Entry | 1 hour | (none) | **Missing** | N/A | N/A | 4 | Replicate (CSV/PDF) |

---

## CROSS-PERSONA COMPARISON — Analyst

| Dimension | Priya Sharma | Chloe Vance |
|-----------|--------------|-------------|
| MBTI | INTP | ENFJ |
| Experience Level | Senior (8+ yr) | Junior (Day 3) |
| Primary Tool (Before) | Excel / ARGUS | Excel / Bloomberg / PPT |
| CRE Knowledge | Expert | Novice (IB Background) |
| Emotional Arc | The Efficient Professional | The Eager but Lost Novice |
| NorthStar Score | 2.8 | 2.2 |
| NEW GAP Identified | No Data Ingestion (ARGUS) | No Onboarding / Contextual Help |

---

## EXECUTIVE SUMMARY — Analyst

**Personas Evaluated**: 2
**Platform Score Range**: 2.2 - 2.8 (Average: 2.5)
**Verdict**: CONDITIONAL PASS

### Top 3 Critical Findings:
1. **The "Expert" Ceiling**: NorthStar is built for users who already know exactly what they are doing (like Priya). It lacks the guardrails, tooltips, and benchmark data required to onboard junior talent or non-CRE specialists (like Chloe).
2. **Data Ingestion Gap**: The lack of ARGUS/CSV import remains the single biggest barrier to institutional adoption, forcing manual re-entry of complex budgets.
3. **The "Last Mile" Reporting Gap**: The absence of IC Memo generation or polished PDF exports forces analysts back into Word/PowerPoint, negating much of the time saved in the modeling phase.

### New Gaps Discovered:
- **No Data Ingestion (ARGUS/CSV)**: Discovered by Priya Sharma — the inability to pull in existing budgets or institutional models creates a massive manual entry tax.
- **No IC Memo Generation**: Discovered by Priya Sharma — the "Word/PowerPoint Ritual" remains untouched by NorthStar.
- **No Onboarding / Contextual Help**: Discovered by Chloe Vance — the UI assumes 100% CRE literacy, offering no tooltips, benchmarks, or guided flows for new analysts.

### Recommendation:
Prioritize an "ARGUS/Excel Import" feature for power users and a "Contextual Help/Benchmark" layer for junior users. Adding tooltips and "Firm Standard" benchmarks would transform NorthStar from a tool into a mentor.

---

### Question Gap Coverage — Analyst
| Gap Targeted | Priya Q# | Chloe Q# |
|--------------|----------|----------|
| No Data Ingestion (ARGUS) | Q1 | - |
| No In-Page Sensitivity | Q2 | - |
| No IC Memo Generation | Q3 | - |
| No Circular References | Q4 | - |
| No Scenario Versioning | Q5 | - |
| No Contextual Help / Tooltips | - | Q2 |
| No Benchmark / Reference Data | - | Q1 |
| No Guided Onboarding | - | Q4 |
| No In-Page Scenario Duplication | - | Q3 |
| No Visible Hurdle Rates | - | Q5 |
