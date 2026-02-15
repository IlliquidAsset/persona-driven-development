# Persona Legends: Internal Power & Behavioral Psychology
**Project**: NorthStar Dealflow OS User Testing
**Version**: 1.0 (Internal Draft)

---

## PERSONA 1: SARAH CHEN — Admin / COO

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

### PART B: A DAY IN SARAH'S LIFE

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
| Role Fit | 3 | Has full access, but admin tools are placeholders |
| UX & Navigation | 3 | Clean design; dead ends frustrate |
| Would She Adopt? | 2 | Not until reporting and audit trail exist |
| **Average** | **2.4** | **CONDITIONAL PASS** |

---

## PERSONA 2: MARCUS WILLIAMS — IR (Investor Relations)

### PART A: THE LEGEND

**Identity & Background**
- **Name**: Marcus Williams, age 36.
- **Education**: BA Finance from Morehouse College (2011). Series 7 and 63 licensed.
- **Career Arc**: Merrill Lynch advisor trainee (2011-2013). JLL Capital Markets analyst (2013-2015). CrowdStreet IR Associate to VP (2015-2020). Joined Tri-Star Capital as VP of IR in 2020.
- **Defining Failure**: At CrowdStreet, he managed a $12M deal where the sponsor stopped reporting. He was left fielding calls from 200+ investors with no data. He learned that IR without transparency is just "professional lying."
- **Defining Triumph**: Closed a $5M single-check commitment from Moore Family Office for Fund III. It took 14 months of relationship-building: quarterly dinners, site visits, and a meticulously crafted data room. Catherine Moore told him, "You're the first person in this industry who didn't lie to me about risk."
- **Why Tri-Star**: He wanted to be the #1 IR person, not one of twelve. At Tri-Star, the capital raising function is his to build from scratch.

**Personal Life**
- **Status**: Single, dating. Midtown Atlanta condo with a view of Piedmont Park.
- **Routine**: 6am F45 Training. 11pm review of his "touch cadence" Google Sheet — who he called, who he owes a callback.
- **Technology**: Proficient but not a power user. He doesn't read error messages; he screenshots them. Frustrated by lack of integration between tools.
- **Workspace**: Open plan desk. AirPods always in. Talks too loudly on investor calls.
- **Stress**: Younger brother Darius dropped out of Georgia Tech sophomore year. Marcus sends $800/month and worries constantly about whether he's enabling or helping.

**Behavioral Psychology**
- **MBTI**: ESFJ ("The Consul"). Relationship-oriented, remembers birthdays, maintains a mental CRM.
- **Big Five**: Very High Extraversion, High Agreeableness, Moderate Conscientiousness, Low Openness to Experience.
- **Decision Style**: Relationship-informed. Will trust a tool if someone he respects recommends it.
- **Software Reaction**: Finds workarounds immediately. Files tickets later (maybe). Builds parallel spreadsheets as insurance.
- **Incomplete Feature Tolerance**: 5/10. But if it makes him look bad to an LP, it drops to 0/10.
- **Cognitive Biases**: Availability heuristic (overweights recent LP conversations), Reciprocity bias (if an LP is responsive, he assumes they'll commit).

### PART B: A DAY IN MARCUS'S LIFE

Marcus walks in at 8:30am with a cold brew from Revelator Coffee. He opens Gmail first — three overnight inquiries from a Nashville family office about Fund IV terms. He replies using a Gmail template he built himself. He doesn't trust the NorthStar CRM email function yet because the last time he tried, the email went out without the attachment.

He opens NorthStar. His landing page is `/crm/contacts`. It's a **GoHighLevel iframe** embedded in the NorthStar shell. He searches for "Moore" and finds Catherine Moore's contact card. He updates her stage to "Committed." He knows from experience that GHL and NorthStar don't reliably sync investor stages, so he navigates to the **Funds** page to verify.

**Fund III: Committed $18.4M.** Catherine's $2M isn't there. The sync hasn't run. Or it failed silently. He sighs and opens his manual Google Sheet — the one he swore he'd stop using three months ago. He updates "Moore Family Office: $2M committed, 2024-11-15." This is the third system tracking the same data.

At 9:30am, he pulls up the **Offerings** page. He sees the Fund IV offering card with its target raise of $15M. He clicks into it. The investor list shows 8 names. He needs to send a follow-up email to the 3 who attended last week's webinar. There's no "filter by last activity" or "bulk email" function. He opens GHL in another tab.

At 10am, he checks **CRM → Campaigns**. He sees the "Fund IV Launch" campaign card. He likes the visual tracker — it shows stages and a progress bar. But he can't send emails from here. He can't even see which investors opened the last blast. He alt-tabs to GHL to queue the email and checks open rates there.

**The moment of rage**: At 11:15am, Catherine Moore calls. "Marcus, I'm looking at the portal and it shows my commitment as $0. I wired $2M three weeks ago." Marcus's stomach drops. He clicks **Dashboard**, sees "Investor Network: 312 Active Investors" in the summary card, but he can't see what Catherine sees. He tries to navigate to `/portal/investor`, but he's logged in as "ir" — the portal is filtered out of his sidebar. He can't preview her experience. He tells her: "Let me have the team send you a fresh link. We're updating the system." He hangs up and Slacks the dev channel: *"URGENT: What does an LP actually see when they log into the portal right now? Catherine Moore just called and her commitment shows $0. I need to know if this is a sync issue or a display issue before she calls back."*

At 2pm, he attends the deal review with Sarah and James. James presents the Phoenix Garden 240 deal using the Napkin Calculator projections. Marcus thinks: *"I could use those numbers for the Fund IV deck."* But he has no way to pull underwriting outputs into investor materials. He takes a photo of the screen.

Marcus has no idea the full **Underwriting Studio** exists. His sidebar filters it out. He assumes the deal projections he gets from BD are made in Excel, like everywhere else he's worked.

At 4:30pm, he's building the Fund IV pitch deck. He needs:
1. Current Fund III performance summary — **available** on Funds page, but no export
2. Portfolio asset photos — **not in NorthStar** (stored in Google Drive)
3. Distribution history — **available** on Distributions page, but no investor-specific view
4. Return attribution — **not available**

He screenshots two NorthStar pages, pastes them into PowerPoint, and manually recreates the rest from his Google Sheet.

### PART C: THE UNCOMFORTABLE QUESTIONS

1. "I raise the capital. I'm the face of this firm to every LP. Why is `canEditData` set to `false` for my role? Do you want me to raise money or file support tickets every time I need to update a note?"
2. "When I update a contact stage in GHL, how long until NorthStar reflects it? Is it real-time? Hourly? Never? My pipeline meeting uses three different sources for the same data."
3. "Catherine Moore wired $2M and she's still showing as a 'Prospect' in the portal. From her perspective, we lost her money. This isn't a software bug — it's a relationship-ending event."
4. "What exactly is a 'campaign management' tool that can't send emails? I can see the campaign, but every action requires me to leave NorthStar."
5. "Why can't I preview the investor portal? I'm selling a product I've never been able to test. If I were selling cars, this would be like never test-driving the vehicle."
6. "I have 312 investors in the system. I can't segment them by commitment size, investment history, or communication preference. How is this better than my Google Sheet?"

### PART D: SCORECARD

| Capability | Score (0-5) | Notes |
|------------|-------------|-------|
| Daily Workflow Coverage | 2 | CRM lives in GHL iframe; can't send emails, can't segment |
| Data Completeness | 3 | Fund/offering data exists but sync with GHL is unreliable |
| Role Fit | 2 | `canEditData: false` blocks basic IR tasks; can't preview portal |
| UX & Navigation | 3 | GHL iframe is functional but feels disconnected from NorthStar |
| Would He Adopt? | 2 | Not until he can send emails, preview portal, and trust sync |
| **Average** | **2.4** | **FAIL** — IR role is blocked by permissions and missing features |

---

## PERSONA 3: JAMES OKAFOR — BD (Business Development)

### PART A: THE LEGEND

**Identity & Background**
- **Name**: James Okafor, age 41.
- **Education**: BS Civil Engineering from UT Austin (2006), MS Real Estate from NYU Schack Institute (2010).
- **Career Arc**: Structural engineer at Kiewit Corporation (2006-2008). The money was good but the work was boring — he wanted to own the deals, not just build them. Analyst at Trammell Crow Company (2010-2012), where he learned to read markets. Associate at CBRE Capital Markets (2012-2015), sourcing $200M+ in acquisition opportunities. VP of Acquisitions at NexPoint Advisors (2015-2019), managing a $400M multifamily pipeline. SVP of Business Development at Tri-Star Capital since 2019.
- **Defining Failure**: At NexPoint, he underwrote a 320-unit deal in suburban Memphis at a 5.25% exit cap. He was so confident in the submarket thesis that he pushed for aggressive leverage — 75% LTV. Then new supply flooded the market; effective rents dropped 8% in 18 months. The deal returned 0.6x. He keeps the original underwriting printout in his desk drawer. Written on it in red pen: *"The market can always surprise you."*
- **Defining Triumph**: Sourced a 4.2-acre parcel in East Nashville that every other buyer passed on due to zoning complications. He spent 4 months in entitlement hearings, personally presenting to the planning commission three times. Got 18 units/acre approved when the base zoning allowed 8. The deal returned 2.1x in 26 months. Sarah calls it "the James Deal."
- **Why Tri-Star**: At NexPoint, he sourced deals but someone else decided. At Tri-Star, if he finds it and underwrites it, he can champion it all the way to closing. He wanted to own the outcome, not just the pitch.

**Personal Life**
- **Family**: Married to Adaeze (pediatrician at Vanderbilt), three kids: Chidi (7), Amara (5), Obiora (2). The two-year-old doesn't sleep. Neither does James.
- **Routine**: 6am baby feeding while scanning LoopNet on his phone. 6:30am gym if Adaeze is home. In the office by 7:45am.
- **Technology**: Competent. Engineer mindset — he reads error messages and tries to understand them. He trusts Excel over any software because he can see every formula. He'll use NorthStar if it's faster than Excel, and not a second longer.
- **Workspace**: Open plan desk near the window. Left monitor for NorthStar/web, right monitor permanently showing his master Excel model. Physical whiteboard behind his chair with the pipeline drawn in four colors (green=active, yellow=diligence, red=dead, blue=watching).
- **Stress**: Parents in Houston are aging. Father had a minor stroke last year. James drives 3.5 hours each way every other weekend. He hasn't told anyone at work how exhausted he is.

**Behavioral Psychology**
- **MBTI**: ESTP ("The Entrepreneur"). Acts fast, decides fast, course-corrects faster.
- **Big Five**: High Extraversion, Low Agreeableness (blunt, doesn't sugarcoat), High Openness to Experience, Moderate Conscientiousness.
- **Decision Style**: Gut-first, data-to-confirm. He'll know within 5 minutes if a deal "feels" right, then spends 2 days trying to disprove his gut.
- **Software Reaction**: Doesn't complain about bugs — just routes around them with Excel workarounds. If a feature doesn't work, he builds a spreadsheet tab for it. His master Excel file has 23 tabs.
- **Incomplete Feature Tolerance**: 7/10. He's a builder. He understands things take time. But if a feature actively misleads him (wrong number, stale data), tolerance drops to 1/10.
- **Cognitive Biases**: Optimism bias (consistently underestimates construction timelines by 15-20%), Anchoring (fixates on the first price he sees for a comparable).

### PART B: A DAY IN JAMES'S LIFE

James is in the office at 7:45am. Overnight, a broker in Phoenix pitched a 240-unit garden-style complex. $52M ask. He opens the email, scans the flyer, and decides this is worth 30 minutes.

He opens NorthStar and navigates to **Underwriting → Deal Ideas**. The Kanban board loads. He clicks **"+ New Idea"** and creates a "Phoenix Garden 240" card. He enters the property address, unit count, and asking price. He likes this — quick capture without opening Excel. He drags it to "Initial Review."

He clicks the card and sees **"Run Deal Check"** — the Napkin Calculator. He selects "Vertical" product type. The input form is clean: purchase price, unit count, rent assumptions, expense ratio, cap rate. He punches in numbers from the broker flyer. **Projected IRR: 11.2%. Equity Multiple: 1.8x. Cash-on-Cash: 7.4%.** He tweaks the exit cap from 5.5% to 5.75%. The live analysis panel updates instantly. IRR drops to 10.1%. He nods — sensitivity is working. **This is genuine delight.** *"This is better than my Excel for a quick look,"* he thinks.

He saves three scenarios: Base Case, Optimistic (5.0% exit cap, 3% rent growth), Conservative (6.0% exit cap, 1% rent growth). He navigates to **Scenario Comparison**. The side-by-side table renders all three with deltas highlighted. *"Better than Argus for a quick look,"* he thinks. He screenshots this for the 2pm deal review.

But then he needs to know: does Tri-Star have the capital for this deal? He opens the **Funds** page. He sees Fund III with its committed capital number. But the **commitment detail is hidden** — `canViewCommitments: false` for the BD role. He can see the fund exists and the total, but he can't drill into who committed what, or how much dry powder remains. He Slacks Marcus: *"How much is committed in Fund III? I need it for the 2pm review. Also, how much can we call?"* He sticks Marcus's reply on a Post-it.

At 10am, he checks the **Entitlements** page for the Nashville build-to-rent project. This is "the James Deal" — the one he sourced, entitled, and is now watching through construction. He sees the milestone tracker: "Building Permit" is "Under Review," "Site Plan Approval" is "Approved." There's a Gantt-style timeline. This page works well — it's where his world and Lisa's (PM) world overlap. He notes that the permit approval date slipped by 2 weeks and makes a mental note to call the city.

At 11:30am, he opens the **Dead Deals** page. He killed a Charlotte deal last week — cap rate compression made the basis too high. The deal shows up in the list with the date and status. But there's no "reason for death" field. No tags. No pattern analysis. He's killed 14 deals in the last quarter and can't quickly pull up *why*. He maintains a separate "Deal Autopsy" tab in his Excel for this.

At 2pm, the deal review meeting with Sarah and the team. He presents the Phoenix Garden 240 analysis. He shares his screen — the Napkin Calculator and Scenario Comparison pages look professional. Sarah asks about the capital stack. James navigates to the **Capital Stack Builder** and puts together a simple 65/35 debt-equity split. The waterfall visualization renders. Sarah nods. But when she asks "What's our all-in basis per unit?" James has to pull up his Excel — NorthStar doesn't aggregate the per-unit metrics he needs.

At 5:15pm, he gets a 40-page offering memorandum PDF for an Austin multifamily deal. He needs to get the key numbers into NorthStar for a quick screen. He opens the Napkin Calculator and starts typing: unit count, purchase price, avg rent, expense ratio, cap rate... He's manually transcribing 15 numbers from a PDF. He makes a typo on the expense ratio — 42% instead of 47%. The IRR swings 200bps. He catches it when the number looks too good, backtracks, and fixes it. But he thinks: *"If I could just drag this PDF into NorthStar and have it pull the numbers..."*

### PART C: THE UNCOMFORTABLE QUESTIONS

1. "I spend 20 hours underwriting a deal and I have no idea if we have the capital to close it. Why is fund commitment data hidden from BD? I'm not asking for bank account numbers — I need to know if there's dry powder before I spend a month on due diligence."
2. "I just manually retyped 15 numbers from a PDF and made a typo that shifted the IRR by 200bps. A human error in underwriting is a firm-level risk. When do we get document ingestion?"
3. "I can't share a link to my scenario comparison with Sarah. She's sitting in the same office but I have to screenshot my analysis and paste it into Slack. How do I present to the IC without screenshots?"
4. "The Dead Deals page is just a list. I killed 14 deals last quarter and I can't tell you why without opening my Excel file. Where are the 'reason for death' tags? Where's the pattern analysis that tells me 'we keep dying on exit cap assumptions in secondary markets'?"
5. "I can see Entitlements, but I can't see the construction budget. How do I know if I should source Phase II if I don't know what Phase I is costing? BD and PM are supposed to be connected, but in NorthStar, we're in different universes."
6. "My Napkin Calculator results are great for a quick screen, but they don't flow into the full pro forma. I have to re-enter everything when a deal moves to detailed underwriting. Why is there a wall between Deal Ideas and the full model?"

### PART D: SCORECARD

| Capability | Score (0-5) | Notes |
|------------|-------------|-------|
| Daily Workflow Coverage | 4 | Napkin calc + deal ideas + entitlements cover core BD needs |
| Data Completeness | 3 | Underwriting data is strong; fund/capital data is hidden |
| Role Fit | 4 | Best-served role; most features align with BD daily tasks |
| UX & Navigation | 4 | Clean, professional, good information density |
| Would He Adopt? | 4 | Already using it daily for screening; Excel remains for deep analysis |
| **Average** | **3.8** | **CONDITIONAL PASS** — Best role experience in the platform |

---

## CROSS-ROLE THEMES (Internal Power Roles)

| Theme | Sarah (Admin) | Marcus (IR) | James (BD) |
|-------|---------------|-------------|------------|
| Primary Tool Today | Airtable + PowerPoint | GHL + Google Sheets | NorthStar + Excel |
| Biggest NorthStar Gap | No audit trail / reporting | Can't preview portal / send emails | Hidden fund data |
| Workaround Count | 3-4 daily | 5+ daily | 2-3 daily |
| Would Recommend? | "Not yet" | "Not for IR" | "Yes, for screening" |
| Emotional State | Frustrated professional | Anxious relationship-builder | Pragmatic builder |
