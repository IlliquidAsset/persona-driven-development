# Persona Legends: Admin
**Project**: NorthStar Dealflow OS User Testing
**Version**: 2.0 (Expanded — CIA-Legend Depth with Legacy Workflow Mapping)

---

## PERSONA 1: SARAH CHEN — Admin / COO (COO)

### PART A: THE LEGEND

**Identity & Background**
- **Name**: Sarah Chen, age 44.
- **Education**: BA Economics from UC Berkeley (2003), MBA from Wharton (2009).
- **Career Arc**: Started as an analyst at Marcus & Millichap (2003-2006). Moved to Greystar Real Estate Partners as Associate (2006-2009). Post-MBA, joined Starwood Capital Group as VP of Operations (2009-2014). Recruited to Brookfield Asset Management as SVP, running ops for a $1.2B multifamily portfolio (2014-2019). Joined Tri-Star Capital as COO in 2019.
- **Defining Failure**: At Brookfield, she greenlit a $45M development based on incomplete construction budget data. Cost overruns hit 22% because subcontractor change orders weren't tracked centrally. This made her obsessed with audit trails and data integrity.
- **Defining Triumph**: Scaled Tri-Star from 4 employees to 18 in three years while maintaining under-2% turnover. Built the firm's first standardized deal approval workflow.
- **Why Tri-Star**: She wanted to build something from scratch. At Tri-Star, she *is* the operating system.

**Personal Life**
- **Family**: Married to Kevin (orthopedic surgeon), two kids: Ethan (11) and Maya (8). Handles school pick-up at 5:45pm sharp.
- **Routine**: 6am Peloton. 11pm calendar review.
- **Technology**: Power user. Built Tri-Star's original tracking in Airtable. Inspects browser dev tools when things look wrong.
- **Workspace**: Corner office, dual 27" Dell monitors. Physical notebook for sensitive notes.
- **Stress**: Mother in Taipei diagnosed with early-stage dementia. Sarah flies back quarterly; the guilt is constant.

**Behavioral Psychology**
- **MBTI**: ENTJ ("The Commander"). Leads meetings, drives decisions.
- **Big Five**: High Conscientiousness, High Extraversion, Low Agreeableness, Low Neuroticism.
- **Decision Style**: Data-driven but impatient. "Give me the number and a recommendation."
- **Software Reaction**: Screenshots bugs and sends them to dev with a terse "ETA?"
- **Incomplete Feature Tolerance**: 3/10. Placeholders offend her.
- **Cognitive Biases**: Anchoring (fixates on the first number seen), Authority bias (trusts CPAs over analysts).

### PART B-0: BEFORE NORTHSTAR — A Day in Sarah's Life

Sarah arrives at 7:48am. The office smells of industrial carpet cleaner and the faint, metallic tang of the HVAC system kicking into high gear. She likes this window of silence—the only time the firm’s "operating system" isn't being poked by twenty different fingers.

She opens Chrome and the first tab is always Airtable. This isn't just a database; it's her brain externalized. Over three years, she has built a sprawling architecture of 14 linked tables and 47 custom views. She clicks into "Pipeline - BD Source" to see if James added the Phoenix lead. He hasn't. She checks "LP Commitments" and cross-references it with a mental note from yesterday's call with Marcus. The schema is complex—relations between SPVs, LPs, and Capital Calls that only she truly understands. It’s a source of immense pride, but also a heavy burden; if she’s out for a day, the firm’s data pulse stops.

By 10:30am, the "Single Source of Truth" problem begins its daily grind. She gets an email from David with a "Final" Excel attachment for the Belfast Road project. She opens it, then opens her Airtable view, then opens Marcus’s GHL dashboard in a third window. Airtable says 8 active deals. James’s whiteboard says 9. GHL has 12 contacts tagged as "Active Deal Related." She spends 20 minutes reconciling the delta, tracing a dead deal that James forgot to move and a prospect Marcus over-tagged. It’s a tax she pays every single day.

The afternoon is swallowed by the "PowerPoint Ritual." It’s the end of the quarter, which means three days of manual labor for the board deck. She pulls data from four different silos: David’s financial reports (Excel), Marcus’s IR summary (Google Sheet), James’s pipeline (Excel), and Lisa’s project updates (emailed PDFs). She manually types numbers into PowerPoint charts, her eyes darting between monitors. She checks every sum twice. Last quarter, a pie chart didn't add to 100% and the Managing Partner noticed. The embarrassment still stings.

Workflow is managed through "Email Reply-All" chains. Her Gmail is a fortress of 23 labels. "Approvals-Pending" has 14 unread messages. She clicks one: *“David, approved, proceed.”* She then has to manually update the "Status" field in Airtable and move a file in Google Drive. The Drive is a 4TB labyrinth. She spent a full Saturday once renaming folders to "YYYY-MM-DD_ProjectName," but today she finds a folder named "Final Final v3 (2)" uploaded by an intern. She sighs, renames it, and logs the change in her physical notebook.

At 6:15pm, after the school run and dinner, she opens her 14th physical notebook. She crosses off "Reconcile Belfast" and adds "Board Deck - Slide 12 Chart Fix." The legacy tools are her friends, but they are demanding, fragmented friends that require her constant mediation to keep the firm from flying apart.

### PART B: A DAY IN SARAH'S LIFE (NorthStar)

Sarah parks her Tesla at 7:48am. She likes the quiet before the office opens.

She opens Chrome. The NorthStar bookmark is third from left. The dashboard loads in two seconds. Her eyes go immediately to the top row. **AUM: $203.4M. Active Projects: 7. Portfolio IRR: 14.2%.** She pauses. Last Monday it was 13.8%. Who touched the model? She hovers over the number, hoping for a tooltip or a click-through. Nothing. The card is static. No audit breadcrumb. She writes in her notebook: *"IRR changed. Ask David if he re-ran the pro forma."*

She scrolls. The dashboard sections load in her admin order: planned projects first. She clicks "Riverside BTR Phase II." The waterfall breakdown renders beautifully. She thinks: *"This is better than anything we had at Brookfield."*

Back to dashboard. She sees a "New Capabilities" card: **"Deal Ideas Canvas."** She clicks it. The Kanban board loads with seed data. She frowns—she can't tell which are real. She navigates to **Settings → Admin Console**.

The Admin Console loads. She clicks **Users & Roles**. She adds the "ir" role to Marcus Williams. A toast notification appears: *"Role linked successfully. Full implementation pending."* She stares at it. *Full implementation pending.* What does that mean? She screenshots it for the dev channel.

She navigates to **Accounting → Overview**. She likes the cash-in-bank trend, but needs the position for a specific SPV—Belfast Road LLC. There's no entity filter here. She goes to the **General Ledger**, finds an architect payment for $78,500. It's dated January 3rd. David said the books were closed. She clicks the entry and sees an "Edit" button. There is no period lock. She calls David immediately: "We have a problem. Anyone with edit access can change January entries."

At 10:15am, she wants to share a pipeline summary. She pulls up the **Capital Pipelines** widget. She tries to drill into the $7.4M "Committed" bucket. The chart is static. She alt-tabs to Airtable to get the actual names for the meeting.

At 2pm, the weekly deal review. She opens the **Deal Pipeline** page. Four deals sit in columns. She can drag them between stages — this is smooth. But she tries to add a note to "Phoenix Garden 240" and realizes there's no comment thread or activity log on the deal card. Just the data James entered.

At 4:30pm, she's preparing the quarterly board deck. She needs:
1. Portfolio summary by asset class — **not available** (no grouping/filter on portfolio page)
2. Capital deployment vs. plan — **not available** (no budget-to-actual view)
3. Investor concentration — **not available** (no LP analytics)

She exports what she can to CSV and spends 45 minutes in PowerPoint. The same 45 minutes she spent last quarter.

### PART C: THE UNCOMFORTABLE QUESTIONS

1. "The IRR on my dashboard jumped 40bps and I have no way to know who changed it. How am I supposed to present this to the board?"
2. "I just discovered there's no period lock. Do you understand the audit implications of allowing edits to closed months?"
3. "Your Admin Console says 'Full implementation pending' after I assign a role. Am I an admin or a beta tester?"
4. "I can see $7.4M committed, but I can't click through to see the LPs. Why does NorthStar exist if I'm still using Airtable for meetings?"
5. "Where is the integration health dashboard? If GHL sync fails, who tells me?"
6. "I need three slides for the board. Portfolio by asset class, capital deployment vs. plan, investor concentration. NorthStar can produce zero of these. What exactly is my ROI on this platform?"

### PART D: SCORECARD

| Capability | Score (0-5) | Notes |
|------------|-------------|-------|
| Daily Workflow Coverage | 2 | Dashboard + deal review works; admin/reporting gaps |
| Data Completeness | 2 | Static cards, no drill-through, no audit trail |
| Audit & Controls | 1 | No period locks, no activity logs, placeholder admin tools |
| Role Fit | 3 | Has full access, but admin tools are placeholders |
| Adoption Likelihood | 2 | Not until reporting and audit trail exist |
| **Average** | **2.0** | **FAIL** |

---

## PERSONA 2: ELENA RODRIGUEZ — Admin (Office Manager)

### PART A: THE LEGEND

**Identity & Background**
- **Name**: Elena Rodriguez, age 36.
- **Education**: BA in Communications from Florida State University (2012).
- **Career Arc**: Executive Assistant at a mid-sized law firm (2012-2017). Office Manager at a Series B tech startup (2017-2022). Office Manager at Tri-Star Capital since 2022.
- **Defining Failure**: At the tech startup, she accidentally shared a "Confidential" salary spreadsheet with the entire company via a Slack link intended for a lunch menu. It led to a week of HR fires, two resignations, and a permanent fear of "Share" buttons.
- **Defining Triumph**: Organized a 3-day firm retreat for 50 people in the Bahamas on a $40K budget, coming in $5K under while securing a 5-star resort. Sarah told her it was "the most efficient operation she'd ever seen."
- **Why Tri-Star**: She likes the stability of real estate compared to the "move fast and break things" tech world. She enjoys being the person everyone goes to when they need something fixed.

**Personal Life**
- **Family**: Married to Marco (a chef), one daughter (Sofia, 4).
- **Routine**: 6:00am: Making school lunch and checking her personal "To-Do" list. 11:00pm: Scrolling Pinterest for home renovation ideas.
- **Technology**: Competent with consumer-grade tools (Google Workspace, Slack, Canva). Intimidated by anything that looks like a "database" or has too many acronyms (GL, IRR, NOI).
- **Workspace**: A desk in the reception/lobby area. Single 24" monitor. A physical "In-Box" tray that is always organized. A framed photo of Sofia at the beach.
- **Non-Work Stress**: Her parents in Miami are pressuring her to move back home, but Marco's restaurant is in New York. The "where do we live" conversation is a weekly source of tension.

**Behavioral Psychology**
- **MBTI**: ISFJ ("The Defender"). Helpful, process-following, avoids conflict. She'd rather ask a colleague for help than "experiment" and risk breaking something.
- **Big Five**: High Conscientiousness, Moderate Extraversion, High Agreeableness, Moderate Neuroticism, Low Openness (prefers established routines).
- **Decision Style**: Process-driven. "Tell me the steps and I'll follow them perfectly."
- **Software Reaction**: If she gets an error message, she closes the tab and tries again. If it happens twice, she calls Sarah or David.
- **Incomplete Feature Tolerance**: 4/10. She expects software to "just work" like Gmail does.
- **Cognitive Biases**: Availability heuristic (judges the system's quality based on the last thing that broke), Omission bias (prefers to do nothing rather than take an action that might cause a problem).

**Software History**
- **Before NorthStar**: Google Workspace (Admin), Airtable (basic user), Excel (templates only), Slack, Outlook, Canva.
- **Tabs open**: Gmail, Google Calendar, Tri-Star Vendor List (Google Sheet), Slack, NorthStar.
- **Keyboard shortcuts**: Ctrl+C, Ctrl+V, Ctrl+Z (her favorite).
- **Screen**: Single 24" Dell.

### PART B-0: BEFORE NORTHSTAR — A Day in Elena's Life

**Morning Arrival (8:30-9:00am):**
- Elena checks the physical mail. She sorts it into "David" (invoices), "Sarah" (legal), and "General."
- She opens her "Tri-Star Operations" Google Sheet. It has tabs for Vendors, Office Supplies, Birthdays, and User Logins.

**Vendor Setup (9:00-10:30am):**
- Sarah tells her to "get the new cleaning crew set up in the system."
- Elena opens her Google Sheet. She adds "Sparkle Clean LLC" to the list. She types in their EIN, address, and contact info.
- She then has to create a new folder in Google Drive: `Operations > Vendors > Sparkle Clean`. She uploads their W-9.
- She then emails David: "Hey David, I added Sparkle Clean to the sheet. Can you add them to Yardi so we can pay them?" She has to wait for David to find time to do the "real" setup.

**User Provisioning (11:00am-12:00pm):**
- A new summer intern is starting. Elena needs to give them access to everything.
- She goes to Google Workspace Admin. Adds the user.
- She goes to Slack. Adds the user.
- She goes to Airtable. Adds the user.
- She has to remember 5 different passwords and 5 different "Invite" workflows. She keeps a "New Hire Checklist" in a physical notebook to make sure she doesn't miss one.

**Report Pulling (2:00-3:00pm):**
- Sarah asks for a "list of all vendors we've paid more than $5,000 this year."
- Elena can't do this. She doesn't have access to Yardi. She has to ask David.
- David is busy. He says "I'll get it to you by Friday." Elena has to tell Sarah she's waiting on David. It makes her feel like a bottleneck.

**End of Day (5:00pm):**
- She tidies her desk. She checks her physical notebook. "Intern access - done." "Sparkle Clean - waiting on David."

### PART B: A DAY IN ELENA'S LIFE (NorthStar)

Elena logs in at 8:30am. Sarah has sent her a Slack: *"Elena, please add 'Highline Security' as a new vendor so David can post their first invoice."*

Elena opens NorthStar. She's in the **Admin** role. She looks at the sidebar. She sees: **Dashboard, Portfolio, Underwriting, Capital, Accounting, Reports, Settings.**

*“Okay, Vendors... where would that be?”* she thinks. She clicks **Settings**. She sees "Profile," "Organization," and "Admin Console." She clicks **Admin Console**. It shows "Users & Roles" and "System Logs." No Vendors.

She clicks **Accounting**. A submenu appears: **Overview, General Ledger, Bank Reconciliation, Vendors & AP, Cash Flow.**

*“Ah, there it is!”* She clicks **Vendors & AP**. She sees the list of vendors. She clicks **"Add Vendor."** She fills out the form. It's easy. She hits Save. *“Wait, did I upload their W-9?”* She looks for a "Documents" or "Attachments" tab on the vendor record. There isn't one. She has to go back to Google Drive to store the W-9.

At 11:00am, the new intern arrives. Sarah says: *"Get them set up in NorthStar."*

Elena goes to **Settings → Admin Console → Users & Roles**. She sees a list of current users. She looks for a **"New User"** or **"Add User"** button. It's not there. She sees a "Roles" tab, but it just defines what roles can do, not who is in them.

*“How do I add a person?”* she wonders. She clicks every button in the Admin Console. Nothing. She finally asks David.

David sighs. *"Oh, you can't do that in the app. You have to log into the Supabase dashboard, go to Authentication, and manually invite them there. Then you have to go into the 'profiles' table in the database and assign their role."*

Elena stares at him. *“The database? David, I don't even know what a Supabase is.”*

David has to do it for her. Elena feels like she's failed at the most basic part of her job. She adds a note to her physical notebook: *"Can't add users. Ask David every time."*

At 2:00pm, Sarah asks for a "Portfolio Summary by Asset Class" for a quick meeting. Elena goes to **Portfolio**. She sees a list of projects. She looks for a "Group by" or "Filter" button. She finds a search bar, but no way to filter by "Multifamily" or "Industrial."

*“I'll just export it,”* she thinks. She hits **Export**. She gets a CSV. She opens it in Excel. She has to manually sort the rows and create a subtotal for each asset class. It takes her 20 minutes.

*“I thought NorthStar was supposed to do this for me,”* she mutters.

She leaves at 5:00pm. She's added a vendor, but she's also added three things to David's to-do list that she should have been able to handle herself.

### PART C: THE UNCOMFORTABLE QUESTIONS

1. "Why is 'Vendors' hidden under the Accounting menu? I'm not an accountant, but I manage the vendor relationships. It took me 10 minutes just to find where to add a new company."
2. "I tried to add a new user for our intern, but there's no 'Add User' button in the Admin Console. David says I have to use something called 'Supabase.' Why can't I just manage our team directly in NorthStar?"
3. "I added a new vendor, but I couldn't find a place to upload their W-9 or contract. Do I really have to keep using Google Drive for all our documents?"
4. "Sarah asked for a list of our multifamily projects, but I couldn't filter the Portfolio page by asset class. I had to export everything to Excel and do it manually. Isn't that what the system is for?"
5. "The Admin Console has a 'System Logs' page, but it's just a bunch of technical code. Can't it just show me a simple list like 'David updated the Nashville budget' or 'Sarah changed a role'?"

### PART D: SCORECARD

| Capability | Score (0-5) | Notes |
|------------|-------------|-------|
| Daily Workflow Coverage | 2 | Can add vendors, but can't manage users or documents. |
| Data Completeness | 2 | Portfolio view is too basic; requires Excel for simple grouping. |
| Audit & Controls | 1 | User management is external (Supabase); no in-app activity log for non-techies. |
| Role Fit | 2 | Admin tools are either missing (User Add) or too technical (Logs). |
| Adoption Likelihood | 3 | She'll use it for vendors, but she'll keep her Google Sheets for everything else. |
| **Average** | **2.0** | **FAIL** — Not a true "Admin" tool for non-technical staff. |

### Question Gap Coverage — Admin

| Gap Targeted | Sarah Q# | Elena Q# |
|---|---|---|
| No Audit Trail | Q1 | - |
| No Period Lock | Q2 | - |
| Incomplete Admin Tools | Q3 | - |
| No Drill-Through / Static Cards | Q4 | - |
| No Integration Monitoring | Q5 | - |
| No Reporting / Export | Q6 | - |
| No In-App User Management | - | Q2 |
| No Vendor Document Support | - | Q3 |
| No Portfolio Filtering | - | Q4 |
| No Activity Log for Non-Techies | - | Q5 |

---

## MIGRATION COMPLETENESS TABLE — Admin

| Workflow Step | Legacy Tool | Time (Legacy) | NorthStar Equivalent | Status | Time (NorthStar) | Delta | Legacy Pain Score (1-5) | Innovation Opportunity |
|---------------|-------------|---------------|---------------------|--------|-------------------|-------|------------------------|----------------------|
| Firm-wide dashboard review | Airtable | 15 min | Dashboard page | Partial | 5 min | +10 min | 2 | Reimagine (Drill-down) |
| Deal pipeline tracking | Airtable | 20 min | Deal Ideas Kanban | Replaced | 5 min | +15 min | 3 | Replicate |
| Board deck preparation | PowerPoint | 3 days | (none) | Missing | N/A | N/A | 5 | Reimagine (Auto-gen) |
| Capital deployment tracking | Airtable + Marcus's Sheet | 45 min | Funds page | Partial | 10 min | +35 min | 4 | Replicate |
| User/role management | Email to dev | 2 days | Admin Console | **Broken** | **N/A** | **N/A** | 4 | **Replicate (In-app User Add)** |
| Document management | Google Drive | 30 min/day | (none) | Missing | N/A | N/A | 4 | Reimagine (Contextual) |
| Approval workflows | Email | 1 hour/day | (none) | Missing | N/A | N/A | 3 | Reimagine (In-app) |
| Integration monitoring | Manual checks | 15 min | (none) | Missing | N/A | N/A | 3 | Replicate |
| Investor analytics | Airtable + Marcus | 1 hour | (none) | Missing | N/A | N/A | 4 | Replicate |
| **Vendor Setup** | **Google Sheets** | **10 min** | **Vendors & AP** | **Partial** | **5 min** | **+5 min** | **2** | **Replicate (Add Doc Upload)** |
| **Portfolio Filtering** | **Airtable** | **2 min** | **Portfolio Page** | **Partial** | **15 min** | **-13 min** | **2** | **Replicate (Add Filters)** |

---

## CROSS-PERSONA COMPARISON — Admin

| Dimension | Sarah Chen | Elena Rodriguez |
|-----------|------------|-----------------|
| MBTI | ENTJ | ISFJ |
| Seniority | COO (20+ yr) | Office Manager (12+ yr) |
| Primary Device | Desktop dual-monitor | Laptop (single) |
| Emotional Arc | The Frustrated Perfectionist | The Helpful Bottleneck |
| Screen-Loading Behavior | The Number Scanner | The Button Searcher |
| Legacy Tool Dependency | High (Airtable) | High (Google Workspace) |
| NorthStar Score | 2.0 | 2.0 |
| NEW GAP Identified | No Period Lock | User Management not In-App |

---

## EXECUTIVE SUMMARY — Admin

**Personas Evaluated**: 2
**Platform Score Range**: 2.0 - 2.0 (Average: 2.0)
**Verdict**: FAIL

### Top 3 Critical Findings:
1. **Administrative Bottleneck**: User management is not integrated into the application, requiring direct database/Supabase access. This forces non-technical admins to rely on technical staff for basic provisioning.
2. **Missing Document Context**: While vendors can be added, there is no mechanism to attach critical compliance documents (W-9s, contracts), forcing a fragmented workflow between NorthStar and Google Drive.
3. **Reporting Rigidity**: The lack of basic filtering and grouping (e.g., by asset class) on the Portfolio and Dashboard pages forces admins back into manual Excel/PowerPoint work for routine requests.

### New Gaps Discovered:
- **User Management not In-App**: Provisioning requires external tools (Supabase), making it inaccessible to non-technical admins — discovered by Elena Rodriguez.
- **No Vendor Document Support**: No way to upload W-9s or contracts to vendor records — discovered by Elena Rodriguez.
- **No Period Lock**: Allows editing of closed months, creating massive audit risk — discovered by Sarah Chen.

### Recommendation:
NorthStar must bring user management and document attachments into the core UI. The "Admin Console" needs to evolve from a technical log viewer into a functional management suite. Without these, the platform remains a "viewer" for admins rather than a "management" tool.
