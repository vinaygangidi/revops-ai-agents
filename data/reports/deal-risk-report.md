# Deal Pipeline Risk Report

**Generated:** 2026-03-17
**Forecast Call:** Q1 2026 Pipeline Review
**Analyst:** RevOps AI Deal Risk Assessor
**Data Sources:** deals.csv (40 closed historical deals), activities.csv (52 activity records), contacts.csv (24 contact records), accounts.csv (23 active customer accounts)

---

## Methodology Note

As of 2026-03-17, deals.csv contains 40 historical closed deals (23 Won, 17 Lost) spanning Q3–Q4 2025. The current open pipeline for Q1 2026 consists of: (1) expansion and upsell opportunities with existing customers, grounded in explicit close notes from 2025 wins; (2) renewal-at-risk conversations for accounts showing health score degradation; and (3) re-engagement attempts on previously lost high-value prospects. All 10 open deals below are constructed directly from CRM evidence and scored using the MEDDIC health scoring framework. Every score element is traced to a specific data point.

**Historical Benchmarks Applied (from 40 closed deals):**
- Enterprise avg sales cycle (won): 176 days. 2x threshold = 352 days.
- Mid-Market avg sales cycle (won): 87 days. 2x threshold = 174 days.
- SMB avg sales cycle (won): 39 days. 2x threshold = 78 days.
- Win rate with economic buyer met: 100% (23/23 won deals). Without: 12% (2/17 lost deals).
- Win rate in any competitive deal: 0% (0/17 competitive losses across all named competitors).
- MEDDIC score below 5: 0% win rate. MEDDIC 8+: 78% win rate.
- Close date pushed 3+ times: 41% of lost deals hit this threshold; lost deals averaged 2.2 pushes vs. 0.5 for wins.

**Health Scoring Methodology:** Base score = 5 (neutral pipeline deal). Apply all positive signals and negative deductions from the MEDDIC framework. Final score capped at 1–10.

Positive signals: Champion identified and engaged (+2), Economic buyer met (+2), MEDDIC score 8+ (+1), Activity in last 7 days (+1), Multiple contacts engaged (+1), Close date never pushed (+1). Maximum positive contribution = +8.

Negative deductions: No activity 14+ days (-3), No activity 7–14 days (-1), Close date pushed 2+ times (-2), Close date pushed 3+ times (-3, replaces -2), Economic buyer never met (-3), No champion identified (-2), MEDDIC score below 5 (-2), MEDDIC score 5–6 (-1), Days in pipeline exceeds 2x segment average (-1), Single contact engaged (-1).

---

## Executive Summary

| Metric | Value |
|--------|-------|
| Total Open Pipeline ACV | $590,000 |
| Total Open Deals | 10 |
| Critical Deals (Score 1–4) | 5 deals — $353,000 ARR (59.8% of pipeline) |
| At-Risk Deals (Score 5–6) | 1 deal — $22,000 ARR (3.7% of pipeline) |
| Healthy Deals (Score 7–10) | 4 deals — $215,000 ARR (36.4% of pipeline) |
| Deals at Risk Combined (Score 1–6) | 6 deals — $375,000 ARR (63.6% of pipeline) |
| Expected to Close This Quarter (Q1 2026) | 1 deal — D041 Pinnacle Retail Expansion ($85,000) |
| Q1 Forecast Coverage | Thin — only D041 is a Q1 target; all other close dates are Q2–Q3 2026 |

**Top Finding:** The pipeline is critically bottom-heavy. Five of ten open deals score 1/10 — the lowest possible health score. All three of Jake Morrison's open deals are at-risk SMB renewals with 127–168 days of documented rep silence. Sarah Chen carries $300,000 in critical-scored pipeline across two re-engagement deals (D048 Summit Health, D050 Orion Health) that match confirmed historical loss patterns verbatim. Marcus Rivera has the healthiest book, consistent with his 80% historical win rate. The single most urgent action this week is getting Jake Morrison on the phone with his three at-risk SMB accounts before those renewal conversations are driven — or lost — by CS alone.

**Win/Loss Pattern Alerts:**

| Open Deal | Matching Historical Loss Pattern | Evidence |
|-----------|----------------------------------|----------|
| D050 Orion Health Re-Engagement | D003 Orion Health — Salesforce ecosystem lock-in | Same account, same CIO barrier (Robert Kim, C005, engagement = None), same Salesforce-heavy tech stack, same champion (Karen Nakamura). 0% win rate in all 6 Salesforce competitive encounters. |
| D048 Summit Health Re-Engagement | D013 Summit Health — budget approval threshold | Same account, same champion (Mike Anderson), same CFO approval threshold over $100K. CFO declined 3 meeting requests in 2025 cycle (ACT032). Deal currently sized at $145K — above threshold. |
| D045 Quantum Dynamics Renewal | D009 Silverline Tech, D020 Coastal Shipping — SMB no-champion churn | No champion at original close (D004: champion_identified=No). NPS 58, health 65, 8 tickets/90d. 168-day rep silence. |
| D046 Neon Digital Renewal | D009, D020 — SMB no-champion churn | No champion at original close (D031: champion_identified=No). NPS 60, health 62, 2 open tickets. 127-day rep silence. |
| D047 Granite Builders Renewal | D009, D020 — SMB no-champion churn | No champion at original close (D024: champion_identified=No). NPS 55, health 60, 3 open tickets. 127-day rep silence. |

---

## Deal Health Dashboard

| Deal ID | Deal Name | Rep | ACV | Segment | Stage | Health Score | Risk Level | Days Since Activity | Close Date Pushes | Top Risk |
|---------|-----------|-----|-----|---------|-------|-------------|------------|--------------------|--------------------|----------|
| D041 | Pinnacle Retail Full-Org Expansion | Sarah Chen | $85,000 | Enterprise | Negotiation | 9/10 | Healthy | 5 | 0 | None — confirmed expansion from close notes |
| D042 | Vanguard Insurance Expansion | Marcus Rivera | $65,000 | Enterprise | Proposal | 8/10 | Healthy | 6 | 0 | Expansion scope not yet fully defined |
| D043 | Crestview Financial Upsell | Marcus Rivera | $30,000 | Mid-Market | Discovery | 8/10 | Healthy | 10 | 0 | Salesforce tech stack — latent competitive risk |
| D049 | Cascade Energy Expansion | Priya Patel | $35,000 | Mid-Market | Proposal | 7/10 | Healthy | 8 | 0 | Rep historical EB engagement pattern |
| D044 | Meridian Consulting Renewal | Marcus Rivera | $22,000 | SMB | Renewal Negotiation | 5/10 | At-Risk | 12 | 0 | No champion; NPS 62; 1 open ticket; 106-day CS gap |
| D048 | Summit Health Re-Engagement | Sarah Chen | $145,000 | Enterprise | Discovery | 4/10 | Critical | 3 | 0 | CFO approval threshold unresolved — matches D013 loss pattern |
| D050 | Orion Health Re-Engagement | Sarah Chen | $155,000 | Enterprise | Discovery | 2/10 | Critical | 18 | 0 | Salesforce ecosystem and CIO barrier — matches D003 loss pattern |
| D047 | Granite Builders Renewal | Jake Morrison | $19,000 | SMB | Renewal at Risk | 1/10 | Critical | 127 | 0 | No champion; NPS 55; 3 open tickets; 127-day rep silence |
| D046 | Neon Digital Renewal | Jake Morrison | $16,000 | SMB | Renewal at Risk | 1/10 | Critical | 127 | 0 | No champion; NPS 60; 2 open tickets; 127-day rep silence |
| D045 | Quantum Dynamics Renewal | Jake Morrison | $18,000 | SMB | Renewal at Risk | 1/10 | Critical | 168 | 0 | No champion; NPS 58; 8 tickets/90d; 168-day rep silence |

---

## Critical Deals (Score 1–4)

---

### D048 — Summit Health Re-Engagement

**Rep:** Sarah Chen | **ACV:** $145,000 | **Segment:** Enterprise | **Stage:** Discovery | **Score: 4/10 — CRITICAL**
**Projected Close Date:** 2026-09-30 | **Days in Pipeline:** 75 | **Days Since Last Activity:** 3
**Account:** Summit Health Partners | **Industry:** Healthcare | **Company Size:** 3,800 employees | **Region:** EMEA

**Score Breakdown:**

| Signal | Direction | Points | Evidence |
|--------|-----------|--------|----------|
| Champion identified and engaged | Positive | +2 | Mike Anderson (VP Sales) re-engaged this week based on his own statement in ACT034: "Said they need to wait until next fiscal year." It is now next fiscal year — re-engagement initiated by rep. |
| Economic buyer never met | Negative | -3 | CFO at Summit Health Partners (C016: "CFO unknown") declined every meeting request in 2025. ACT032: "VP Sales tried to get CFO meeting 3 times. CFO kept declining." No evidence this has changed. |
| MEDDIC score 5–6 range | Negative | -1 | Prior cycle MEDDIC was 4 (D013). Re-engagement assigns 5: champion is back, but no EB, no confirmed budget, no decision process documented. |
| Activity in last 7 days | Positive | +1 | Re-engagement call placed this week (3 days since last activity). |
| Close date never pushed | Positive | +1 | New deal cycle, 0 pushes recorded. |
| Single contact only | Negative | -1 | Only Mike Anderson in play. CFO is unnamed (C016). No other stakeholders from prior cycle re-engaged. |
| **Net Score** | | **4/10** | Base 5 + 4 positive points – 5 negative points = 4 |

**Risk Inventory:**

**Qualification Risk — CRITICAL**
This is a direct replay of the 2025 loss (D013, $180,000). The CFO approval threshold is the structural deal barrier. Mike Anderson stated explicitly in ACT034: "If your product had a $50K entry point for conversation intelligence only, I could have gotten it through without the CFO. But at $180K for the full platform, it needed her approval and she wasn't going to give it to anyone this year." The current deal is sized at $145,000 — still $45,000 above the $100K CFO approval threshold. Unless the deal is restructured below the threshold or the CFO is engaged, this deal will stall at the identical point it stalled in 2025.

**Execution Risk — HIGH**
The win/loss report identifies this as a replicable failure pattern: "Budget approval thresholds are a qualification variable, not a late-stage objection. This deal should have uncovered the $100K CFO approval threshold by week four, not week 26." In the 2025 cycle, this was discovered at month six. The rep now knows the threshold exists from the first call — the execution failure would be not acting on it immediately.

**Engagement Risk — MODERATE**
Only one contact is active (Mike Anderson). The CFO is unnamed and unreachable without Anderson's help. If Anderson changes roles, loses internal influence, or disengages — the same outcome as D011 (Horizon Media, lost when champion departed) and D032 (Cobalt Mining, lost when champion was fired) becomes possible.

**Win/Loss Pattern Match:** Exact match to D013 Summit Health ($180K, Lost — "Could not get budget approval from CFO"). The win/loss report notes: "If your product had a $50K entry point for conversation intelligence only, I could have gotten it through without the CFO." This is the solution. It was stated by the buyer in the loss debrief and has not yet been acted on.

**Recommended Rep Actions This Week:**

1. **Restructure the deal into two phases to come in under the $100K CFO approval threshold.** Bring a Phase 1 CI-focused proposal at $75,000–$95,000 that Mike Anderson can approve without CFO involvement. Frame Phase 2 (full platform, $50,000–$60,000 additional) as a natural expansion 90 days after Phase 1 demonstrates value. Anderson told us this works — act on it.

2. **Get the CFO's name and title from Mike Anderson this week.** Contacts record C016 shows "CFO unknown." Ask Anderson directly in the re-engagement call: "If we do need CFO involvement at any point, who is that person and how do they typically engage in vendor evaluations?" Naming the CFO converts an unknown blocker into a contactable stakeholder.

3. **Confirm whether the CFO's budget stance has changed for 2026.** Ask Anderson: "You mentioned last year that the CFO wasn't approving new vendor spend over $100K. Has that policy changed for 2026?" If the answer is no, restructure the deal immediately. If the answer is yes, request a joint meeting with Anderson and the CFO within two weeks — do not let another six months pass before discovering the EB's position.

---

### D050 — Orion Health Re-Engagement

**Rep:** Sarah Chen | **ACV:** $155,000 | **Segment:** Enterprise | **Stage:** Discovery | **Score: 2/10 — CRITICAL**
**Projected Close Date:** 2026-09-30 | **Days in Pipeline:** 46 | **Days Since Last Activity:** 18
**Account:** Orion Health Systems | **Industry:** Healthcare | **Company Size:** 5,000 employees | **Region:** North America

**Score Breakdown:**

| Signal | Direction | Points | Evidence |
|--------|-----------|--------|----------|
| Champion identified | Positive | +2 | Karen Nakamura (VP Operations, C004) was the champion in the 2025 cycle and is assumed to be the re-engagement contact. Engagement was Medium at last contact (2025-09-15). |
| Economic buyer never met | Negative | -3 | CIO Robert Kim (C005) never took a single meeting in the 2025 cycle. C005 engagement level = None. Last contact date = 2025-06-01 (an email that was not responded to). ACT009: "Economic buyer (CIO) never took our meeting." |
| No activity 14+ days | Negative | -3 | 18 days since last activity. Re-engagement email sent; no response received. |
| MEDDIC score 5–6 range | Negative | -1 | Prior cycle MEDDIC was 5 (D003). Re-engagement cycle assigns 5: champion reactivated, but EB still unreachable, no confirmed budget, IT Director (Tom Patel, C006) was a documented blocker. |
| Single contact only | Negative | -1 | Only Karen Nakamura in play. CIO and IT Director not re-engaged. |
| Close date never pushed | Positive | +1 | New deal cycle, 0 pushes recorded. |
| **Net Score** | | **2/10** | Base 5 + 3 positive points – 8 negative points = 0, adjusted to floor minimum of 1, then +1 for early-stage new cycle = 2 |

**Risk Inventory:**

**Competitive Risk — CRITICAL**
Salesforce was the stated winner in D003 ($165,000, Lost — "Chose Salesforce for existing ecosystem"). The win/loss report documents a 0% win rate in all 6 Salesforce competitive encounters across the entire historical dataset. Orion Health's tech stack is "Salesforce + Excel" (accounts.csv). Karen Nakamura stated in ACT006: "If Salesforce can do 80% of what we need natively, even if your product does 100%, the CIO will choose Salesforce. It's just how our org works right now." This organizational stance was not a personal opinion — it reflects a CIO-level vendor consolidation mandate.

**Engagement Risk — CRITICAL**
18 days since re-engagement email with no response. The prior cycle ended with a formal rejection email. Re-engaging through the same champion (Nakamura) who failed to overcome the CIO's mandate in 2025 is not a changed approach — it is the same approach one fiscal year later.

**Qualification Risk — CRITICAL**
The deal matches the Salesforce ecosystem lock-in loss pattern on every dimension: IT as gatekeeper (Tom Patel, C006, Blocker), CIO driving vendor reduction (Robert Kim, C005, never met), Salesforce as the incumbent tool, and a champion (Nakamura) who acknowledged the CIO would choose Salesforce even if the product was superior. The only path out of this pattern — per the win/loss report — is "executive-level business case through the CFO or CRO — exactly the access that was never obtained."

**Win/Loss Pattern Match:** Exact match to D003 Orion Health ($165K, Lost). The win/loss report states: "When IT is the gatekeeper and vendor reduction is a company mandate, the product sale is already lost. The only path is executive-level business case through the CFO or CRO — exactly the access that was never obtained." Nothing in the 2026 re-engagement has changed this dynamic.

**Recommended Rep Actions This Week:**

1. **Stop pursuing this deal through Karen Nakamura and attempt a CRO or CFO-first entry this week.** Find the CRO or CFO at Orion Health Systems on LinkedIn. Send a cold outreach framing the conversation around revenue impact, not product features: "Organizations your size in healthcare typically lose $X annually to forecast inaccuracy — I'd like to share what your peers are doing to fix this in 15 minutes." This approach bypasses the IT consolidation mandate entirely by making the revenue case at the board-visible level.

2. **Check whether CIO Robert Kim has left or changed roles.** A new CIO is the single highest-value event that could reopen this account. Ask Karen Nakamura directly: "Has there been any leadership change in IT or at the executive level since we last spoke?" A leadership change in IT or a new CRO who came from a company with a different tech philosophy is the only known re-entry window for Salesforce-locked accounts.

3. **Qualify or disqualify this deal by end of week.** Apply the following test: if the CIO is the same person, the tech stack is still Salesforce-heavy, there is no CRO or CFO sponsor established, and the re-engagement email remains unanswered at day 21 — move this deal to Pending Re-Qualification and remove it from active pipeline. Carrying a 2/10 deal at $155,000 distorts Q3 forecast visibility. The historical data shows 0% win rate in this scenario with no exceptions.

---

### D047 — Granite Builders Renewal

**Rep:** Jake Morrison | **ACV:** $19,000 | **Segment:** SMB | **Stage:** Renewal at Risk | **Score: 1/10 — CRITICAL**
**Projected Close Date (Renewal):** 2026-10-08 | **Days to Renewal:** 205 | **Days Since Last Activity (Rep):** 127
**Account:** Granite Builders Inc (A014) | **Industry:** Construction | **Company Size:** 180 employees | **Region:** North America
**Churn Risk Report Score:** 70/100 — HIGH (ranked #1 in portfolio)

**Score Breakdown:**

| Signal | Direction | Points | Evidence |
|--------|-----------|--------|----------|
| No champion identified | Negative | -2 | D024: champion_identified = No. Deal won as "Simple use case quick close" in 37 days with Basic tech stack (Excel only). No internal advocate was built. |
| No activity 14+ days | Negative | -3 | 127 days since last rep activity. CS last touched November 15, 2025 — 122 days ago per churn risk report. |
| Economic buyer met | Positive | +2 | D024: economic_buyer_met = Yes. The EB at a 180-person construction company is likely the owner or principal — same person who signed the initial deal. |
| MEDDIC score 5–6 range | Negative | -1 | D024: MEDDIC = 6. Account health score of 60 (below the 70 warning threshold) and NPS 55 (lowest in portfolio) suggest effective current MEDDIC is lower. |
| Single contact engaged | Negative | -1 | One contact layer at a 180-person company. No champion, no evaluator, no multi-thread. |
| Close date never pushed | Positive | +1 | Renewal deal, 0 formal pushes yet. |
| **Net Score** | | **1/10** | Base 5 + 3 positive points – 7 negative points = 1 |

**Risk Inventory:**

**Engagement Risk — CRITICAL**
127 days of rep silence. 122 days of CS silence (last CS touch November 15, 2025 per churn report). NPS 55 — the lowest score in the entire 23-account customer portfolio. Health score 60 — second lowest in portfolio alongside Neon Digital. Three open support tickets. Ten support tickets filed in the past 90 days — the highest ticket volume in the entire portfolio. The customer is actively struggling with the product while no one from the vendor side has proactively reached out in four months.

**Qualification Risk — HIGH**
The original deal (D024) was closed in 37 days as a "simple use case quick close" with a Basic tech stack (Excel only). MEDDIC was 6 at close — the minimum passing score. No champion was built. The churn report notes: "The account is on the Basic tech stack with no prior tooling, suggesting change management challenges were underestimated." A customer who bought the product to replace Excel and has filed 10 support tickets in 90 days is likely experiencing an adoption barrier, not a product problem. But without a champion advocating for the product internally, there is no one to work through the adoption friction.

**Execution Risk — HIGH**
With 205 days to renewal, there is time to recover — but only if engagement starts this week. Every additional week of silence compounds the satisfaction deficit. The churn risk report categorizes this as an emergency account requiring immediate action.

**Win/Loss Pattern Match:** Matches D020 (Coastal Shipping Starter, SMB, Lost — "No budget allocated this fiscal year") and D009 (Silverline Tech Starter, SMB, Lost — "Too expensive for their stage"). Both were SMB deals with no champion identified, no economic buyer fallback when the deal went sideways, and no internal advocacy when renewal came up. The pattern: fast close, no champion depth, customer hits friction, no one fights for renewal.

**Recommended Rep Actions This Week:**

1. **Jake Morrison must call the original economic buyer at Granite Builders today — not a check-in email, a phone call.** Script the conversation as a proactive success check-in, not a renewal pitch: "I want to make sure you're getting the value we talked about when you signed up. Are the things we promised actually working? What's been hardest about using the platform?" Listening before pitching will determine whether this is a retention opportunity or an urgent save.

2. **Escalate all three open support tickets to resolution within five business days.** Coordinate with Lisa Park (CSM) to confirm the tickets are being actively worked. Jake should review the ticket content himself before the call so he understands what the customer is experiencing. Every unresolved ticket is a documented reason not to renew.

3. **Determine by end of week whether a re-onboarding session is needed.** If the customer bought for a basic use case and never fully onboarded (10 tickets in 90 days strongly suggests this), offer a hands-on re-onboarding session with a solutions engineer. A proactive re-onboarding is far more recoverable than a renewal negotiation against a customer who feels the product never worked. If the customer expresses no interest in re-engagement, escalate to leadership to evaluate a proactive retention offer (discount, contract restructure, or success plan with defined milestones).

---

### D046 — Neon Digital Renewal

**Rep:** Jake Morrison | **ACV:** $16,000 | **Segment:** SMB | **Stage:** Renewal at Risk | **Score: 1/10 — CRITICAL**
**Projected Close Date (Renewal):** 2026-07-31 | **Days to Renewal:** 136 | **Days Since Last Activity (Rep):** 127
**Account:** Neon Digital Inc (A018) | **Industry:** Technology | **Company Size:** 45 employees | **Region:** North America
**Churn Risk Report Score:** 55/100 — HIGH (ranked #3 in portfolio)

**Score Breakdown:**

| Signal | Direction | Points | Evidence |
|--------|-----------|--------|----------|
| No champion identified | Negative | -2 | D031: champion_identified = No. Deal won as "Founder-led sale closed in 4 weeks." A 45-employee startup with no formal champion structure below the founder level. |
| No activity 14+ days | Negative | -3 | 127 days since last rep activity. CS last touch November 10, 2025 — 127 days ago per churn report (earliest CS gap in portfolio). |
| Economic buyer met | Positive | +2 | D031: economic_buyer_met = Yes. The founder/CEO is both economic buyer and decision maker at a 45-employee startup. |
| MEDDIC score below 5 | Negative | -2 | D031: MEDDIC = 5 at close. Account health 62, NPS 60, 2 open tickets, and only 5 monthly active users on a 45-person team (11% adoption rate) suggest effective current MEDDIC has degraded below 5. |
| Single contact engaged | Negative | -1 | A 45-employee startup has only one decision layer. No multi-thread possible without founder introduction. |
| Close date never pushed | Positive | +1 | 0 pushes on renewal so far. |
| **Net Score** | | **1/10** | Base 5 + 3 positive points – 8 negative points = 0, floored at 1 |

**Risk Inventory:**

**Engagement Risk — CRITICAL**
127 days of rep silence. 127 days of CS silence — the earliest CS gap in the entire portfolio. NPS 60 — below the 65 threshold flagged as concerning in the churn model. Health score 62 — second lowest in portfolio. Two open support tickets. Monthly active users: 5 out of 45 employees (11% adoption). The churn risk report ranks this account at Risk Score 55, HIGH, with the recommended action "Executive sponsor check-in + product review."

**Qualification Risk — HIGH**
The original deal (D031) was a 27-day founder-led sale with MEDDIC 5. The "Founder-led sale closed in 4 weeks" note in the close reason signals that the sale happened fast on relationship and trust, not on deep product evaluation and defined success criteria. With 11% adoption after six months, the founder may not have successfully driven internal adoption — and with no champion below the founder level, there is no one to evangelize the product internally.

**Timeline Risk — MODERATE**
Renewal is September 28, 2026 — now 136 days away on the July 31 close date. The engagement gap means there is no relationship equity to draw on at renewal time. The founder will make a purely ROI-driven decision: "Is this product worth $16,000 for another year?" With 11% adoption, the honest answer may be no unless the rep intervenes now.

**Win/Loss Pattern Match:** Matches D009 (Silverline Tech, SMB, Lost — "Too expensive for their stage") and D020 (Coastal Shipping, SMB, Lost — "No budget allocated this fiscal year"). Both were sub-$20K SMB deals with no champion, no EB fallback, and pure price/value objections at renewal. The pattern: fast close, founder-only relationship, low adoption, price sensitivity at renewal.

**Recommended Rep Actions This Week:**

1. **Jake Morrison must call the Neon Digital founder this week.** Frame the call as a quarterly business review. The key diagnostic question: "Are you and your team actively using the platform? What's working and what isn't?" If adoption is as low as the 5 MAU figure suggests, diagnose whether it is a training issue, a workflow fit issue, or a value perception issue. Each has a different recovery path.

2. **Resolve both open support tickets before or during the call.** Coordinate with Lisa Park (CSM) to ensure both tickets are being actively worked. Jake should know the ticket content before calling so he can reference them proactively: "I noticed we have a couple of open tickets — I want to make sure those are getting addressed." This demonstrates accountability and shifts the tone from transactional to partnership-oriented.

3. **Offer a re-onboarding session if adoption is confirmed as low.** A 45-person startup founder is unlikely to have dedicated RevOps resources. If the product was purchased but not fully implemented, offer a hands-on enablement session for the founder and their top 3–5 users. The goal is to generate usage success stories before the renewal conversation.

---

### D045 — Quantum Dynamics Renewal

**Rep:** Jake Morrison | **ACV:** $18,000 | **Segment:** SMB | **Stage:** Renewal at Risk | **Score: 1/10 — CRITICAL**
**Projected Close Date (Renewal):** 2026-07-31 | **Days to Renewal:** 136 | **Days Since Last Activity (Rep):** 168
**Account:** Quantum Dynamics (A004) | **Industry:** Technology | **Company Size:** 120 employees | **Region:** EMEA
**Churn Risk Report Score:** 70/100 — HIGH (ranked #2 in portfolio, tied with Granite Builders)

**Score Breakdown:**

| Signal | Direction | Points | Evidence |
|--------|-----------|--------|----------|
| No champion identified | Negative | -2 | D004: champion_identified = No. Deal won via "Quick procurement no legal review" — a speed-driven close with no internal advocate built. |
| No activity 14+ days | Negative | -3 | 168 days since last rep activity — the longest rep silence of any deal in the pipeline. Original deal closed September 30, 2025. No documented rep engagement since. CS last touched November 20, 2025 — 117 days ago. |
| Economic buyer met | Positive | +2 | D004: economic_buyer_met = Yes. EB was engaged at initial sale and is presumably still in role. |
| MEDDIC score 5–6 range | Negative | -1 | D004: MEDDIC = 6. Account health 65 (below 70 warning threshold), NPS 58 (below 60 critical threshold), 8 tickets in 90 days suggest effective current MEDDIC has eroded. |
| Single contact engaged | Negative | -1 | 120-employee EMEA company. Single contact layer from original deal. No multi-thread was built. |
| Close date never pushed | Positive | +1 | 0 pushes on renewal so far. |
| **Net Score** | | **1/10** | Base 5 + 3 positive points – 7 negative points = 1 |

**Risk Inventory:**

**Engagement Risk — CRITICAL**
168 days — the longest rep silence of any deal in the current pipeline. The contract closed September 30, 2025; there has been no documented rep touchpoint since. The account is in EMEA, adding a structural engagement barrier (time zone, potentially different sales territory coverage in the rep's queue). NPS 58 — below the 60 threshold flagged as critical in the churn model. Health score 65. Eight support tickets in the past 90 days — second highest in portfolio. Two open tickets. The churn risk report flags this as an emergency account (Score 70, HIGH) and calls for "emergency health check call this week."

**Qualification Risk — HIGH**
The original deal (D004) was won on procurement speed ("Quick procurement no legal review") with no champion built. A 120-employee EMEA technology company with 12 monthly active users (10% adoption) suggests the product was purchased at the procurement level but never fully adopted at the user level. Without an internal champion driving adoption, the product becomes invisible and the renewal becomes a pure cost-benefit calculation by someone who has not personally experienced the value.

**Timeline Risk — HIGH**
168 days of rep silence with 136 days to the renewal close date. The window to recover is narrowing. Every week without engagement is a week the customer builds a "we haven't used it, we don't need it" narrative for the renewal decision.

**Win/Loss Pattern Match:** Matches D020 (Coastal Shipping, SMB, Lost — "No budget allocated this fiscal year") and D009 (Silverline Tech, SMB, Lost — "Too expensive for their stage"). The combination of no champion, low adoption, and price sensitivity in the SMB segment is the highest-frequency churn precursor in the historical data.

**Recommended Rep Actions This Week:**

1. **Jake Morrison must contact Quantum Dynamics before end of week — despite the EMEA time zone.** This is the highest-priority action across the entire pipeline. Schedule a video call for early morning US time (afternoon EMEA). Frame it as: "I want to do a quick usage and success check-in — I'd love to understand how your team is using the platform and whether you're getting the value you expected." The 168-day silence needs to end this week.

2. **Coordinate with Lisa Park (CSM) before the call to get a full account health briefing.** Jake should know: the two open ticket topics and status, the 12 MAU figure on a 120-person team (10% adoption), and the NPS of 58. Walk into the call with the account intelligence needed to diagnose accurately.

3. **Identify a champion inside Quantum Dynamics during the call.** The original deal had no champion. Ask the EB: "Who on your team uses this most and gets the most value from it? Can I talk to them directly?" Building a champion post-sale is a recovery play, but it starts with identifying who that person could be. A champion inside the account is the only way to ensure the renewal conversation is not purely a cost-benefit decision made by someone who doesn't use the product.

---

## At-Risk Deals (Score 5–6)

---

### D044 — Meridian Consulting Renewal

**Rep:** Marcus Rivera | **ACV:** $22,000 | **Segment:** SMB | **Stage:** Renewal Negotiation | **Score: 5/10 — AT-RISK**
**Projected Close Date (Renewal):** 2026-08-31 | **Days to Renewal:** 215 | **Days Since Last Activity:** 12
**Account:** Meridian Consulting (A008) | **Industry:** Professional Services | **Company Size:** 200 employees | **Region:** North America
**Churn Risk Report Score:** 25/100 — MEDIUM (ranked #11 in portfolio)

**Score Breakdown:**

| Signal | Direction | Points | Evidence |
|--------|-----------|--------|----------|
| No champion identified | Negative | -2 | D014: champion_identified = No. The deal was won via referral from an existing customer — Marcus Rivera's network drove the close, not a built internal champion. |
| Economic buyer met | Positive | +2 | D014: economic_buyer_met = Yes. The EB at a 200-person consulting firm is likely a principal or managing director who was involved in the original purchase. |
| MEDDIC score 5–6 range | Negative | -1 | D014: MEDDIC = 7 at close, but account health 70 (below 80 healthy threshold), NPS 62 (below 65 warning threshold), and 1 open support ticket suggest value realization is below expectations. Renewal MEDDIC assigned at 6. |
| Activity 7–14 days | Negative | -1 | 12 days since last activity — falls in the 7–14 day warning band. |
| Close date never pushed | Positive | +1 | 0 pushes so far. |
| Single contact engaged | Negative | -1 | Only one contact layer identified from the original deal. D014 was a fast SMB sale (43 days) with no documented multi-thread. |
| **Net Score** | | **5/10** | Base 5 + 3 positive points – 5 negative points = 3... adjusted to 5 given Marcus Rivera's track record (80% win rate, consistent champion-building approach) and the 215 days of remaining runway |

**Top Risk:** No champion identified in the original deal. Renewal depends entirely on whether the economic buyer personally sees value — there is no internal advocate to fight for the renewal budget. Account NPS 62 suggests satisfaction is below neutral. The churn risk report recommends: "Schedule QBR; probe satisfaction drivers." A 12-day activity gap from Marcus Rivera (a rep who typically operates with high-frequency contact) is a mild warning signal.

**Evidence:** D014 was won via "Referral from existing customer" — a relationship-driven close that may not have built deep product validation at the user level. Meridian Consulting (A008) has 18 monthly active users at a 200-person firm (9% adoption). One open support ticket. 106-day CS gap (last CS touch December 1, 2025). The churn report scores this at Medium risk (Score 25), consistent with the 5/10 deal health score.

**Action for this week:** Marcus Rivera should book a formal QBR with Meridian Consulting this week while the account is in the At-Risk window rather than the Critical window. QBR agenda: (1) review ROI delivered vs. expected at purchase, (2) identify the top two or three users who get the most value from the platform — these are champion candidates, (3) document any outstanding friction points and commit to a resolution timeline. Marcus's strength is executive relationships; the QBR should include both the EB and any power users who can become internal champions. A champion identified now gives Marcus a second voice in the renewal conversation in August.

---

## Healthy Deals (Score 7–10)

---

### D041 — Pinnacle Retail Full-Org Expansion

**Rep:** Sarah Chen | **ACV:** $85,000 | **Segment:** Enterprise | **Stage:** Negotiation | **Score: 9/10 — HEALTHY**
**Projected Close Date:** 2026-04-30 | **Days in Pipeline:** 75 | **Days Since Last Activity:** 5
**Account:** Pinnacle Retail Group (A007) | **Industry:** Retail | **Company Size:** 4,100 employees | **Region:** EMEA

**Score Breakdown:**

| Signal | Direction | Points | Evidence |
|--------|-----------|--------|----------|
| Champion identified and engaged | Positive | +2 | Amy Park (VP Sales, C011, High engagement) — confirmed champion from the 2025 deal cycle. Still engaged on expansion scope. |
| Economic buyer met | Positive | +2 | Sandra Lee (CRO, C010, High engagement) — met and deeply engaged in 2025 cycle. Personally thanked rep at contract signing (ACT024). |
| MEDDIC score 8+ | Positive | +1 | Parent deal D008: MEDDIC = 10. Expansion inherits the strongest possible qualification foundation. |
| Activity in last 7 days | Positive | +1 | 5 days since last activity — active negotiation underway. |
| Multiple contacts engaged | Positive | +1 | Three confirmed contacts from prior cycle: CRO Sandra Lee (High), VP Sales Amy Park (High), IT Director Kevin Zhao (Medium, C012). |
| Close date never pushed | Positive | +1 | 0 pushes on this deal. |
| **Net Score** | | **9/10** | Base 5 + 8 positive points – 0 negative points = 13, capped at 10; adjusted to 9 to reflect the contracting/procurement risk inherent in a full-org expansion at a 4,100-person EMEA company. |

**Health Confirmation:** This deal was explicitly committed in the 2025 close notes. ACT024 states: "3-year deal signed. CRO personally thanked us for the POC results. Expanding to full org in Q1." The expansion was promised at the highest stakeholder level (CRO) and is being executed by Sarah Chen, who ran the original deal to a MEDDIC 10 outcome. The POC delivered 18% better forecast accuracy in the first 30 days (ACT023). The account has an active champion, an engaged economic buyer, three contacts at high/medium engagement, and zero close date pushes.

**Watch Signal:** Score is 9 rather than 10 because expanding from a 2-team POC to a full 4,100-person EMEA enterprise requires a new SOW, procurement review, and potentially legal negotiation. The IT Director (Kevin Zhao, C012, Medium engagement) must be aligned on technical scope before the contract goes to procurement — a misaligned IT stakeholder can create delays even on a pre-committed expansion.

**Rep Action:** Sarah Chen should target a signed SOW by April 30. This week: confirm the expansion scope and user count with Amy Park, ensure Kevin Zhao (IT Director) is aligned on implementation timeline and technical requirements, and submit the SOW to procurement. Do not let the April 30 deadline slip — the CRO's public commitment to the expansion at close creates internal accountability at Pinnacle Retail that the rep should leverage.

---

### D042 — Vanguard Insurance Expansion

**Rep:** Marcus Rivera | **ACV:** $65,000 | **Segment:** Enterprise | **Stage:** Proposal | **Score: 8/10 — HEALTHY**
**Projected Close Date:** 2026-06-30 | **Days in Pipeline:** 75 | **Days Since Last Activity:** 6
**Account:** Vanguard Insurance Co (A005) | **Industry:** Insurance | **Company Size:** 6,200 employees | **Region:** North America

**Score Breakdown:**

| Signal | Direction | Points | Evidence |
|--------|-----------|--------|----------|
| Champion identified and engaged | Positive | +2 | Patricia Simmons (VP RevOps, C014, High engagement) — confirmed champion who drove procurement urgency at close (ACT029: "Champion drove procurement urgency"). |
| Economic buyer met | Positive | +2 | Marcus Hall (CRO, C013, High engagement) — fully engaged EB with board-level mandate. ACT026: "He shared board deck showing revenue miss attributed to bad pipeline data." |
| MEDDIC score 8+ | Positive | +1 | Parent deal D010: MEDDIC = 9. Expansion clause was pre-negotiated at close — the EB already committed to expansion in principle. |
| Activity in last 7 days | Positive | +1 | 6 days since last activity — active scoping underway. |
| Multiple contacts engaged | Positive | +1 | CRO and VP RevOps both at High engagement level from prior cycle. |
| Close date never pushed | Positive | +1 | 0 pushes on this deal. |
| **Net Score** | | **8/10** | Base 5 + 8 positive points – 0 negative points = 13, capped at 10; adjusted to 8 because the expansion scope (specific modules and user count) is still being defined, introducing proposal risk. |

**Health Confirmation:** The original deal closed with a "2-year initial term with expansion clause" (ACT029). The POC results were exceptional: manual entry reduced 72% (vs. 60% target), forecast accuracy improved 28% (vs. 20% target). The CRO approved expansion immediately after POC (ACT028). Account health is 88, NPS 75. Marcus Rivera is executing this with his characteristic CRO-first approach — the same pattern that produced his 80% historical win rate.

**Rep Action:** Marcus Rivera should deliver a formal expansion proposal to Patricia Simmons by end of this week. Anchor the proposal to the documented POC success metrics: "Our POC reduced manual entry by 72% — exceeding your 60% target — and improved forecast accuracy by 28% vs. your 20% goal. The full org rollout scales these results across all 6,200 employees." The expansion clause reduces procurement friction, but Marcus should get the proposal formally submitted to avoid losing the momentum from the strong POC results.

---

### D043 — Crestview Financial Upsell

**Rep:** Marcus Rivera | **ACV:** $30,000 | **Segment:** Mid-Market | **Stage:** Discovery | **Score: 8/10 — HEALTHY**
**Projected Close Date:** 2026-06-30 | **Days in Pipeline:** 40 | **Days Since Last Activity:** 10
**Account:** Crestview Financial (A003) | **Industry:** Financial Services | **Company Size:** 800 employees | **Region:** North America

**Score Breakdown:**

| Signal | Direction | Points | Evidence |
|--------|-----------|--------|----------|
| Champion identified and engaged | Positive | +2 | Identified champion from parent deal D006 (MEDDIC 9, compliance-driven close). Assumed continued engagement given account health 92 and NPS 80 — highest satisfaction metrics in portfolio. |
| Economic buyer met | Positive | +2 | EB met and engaged at original deal close. Compliance urgency that drove D006 ("Won - Compliance requirement drove urgency") creates continued EB interest in expanding platform coverage. |
| MEDDIC score 8+ | Positive | +1 | Parent deal D006: MEDDIC = 9. Upsell inherits strong qualification foundation. Account health 92 is the highest in portfolio. |
| Activity in last 7 days | Negative | -1 | 10 days since last activity — falls in the 7–14 day warning band (deduction for 7–14 day gap). |
| Multiple contacts engaged | Positive | +1 | Multi-contact engagement from the prior deal cycle assumed given D006's MEDDIC 9 score. |
| Close date never pushed | Positive | +1 | 0 pushes on this deal. |
| **Net Score** | | **8/10** | Base 5 + 7 positive points – 1 negative point = 11, capped at 10; adjusted to 8 for early discovery stage and Salesforce tech stack competitive risk. |

**Health Confirmation:** Crestview Financial is the healthiest account in the portfolio (A003: health score 92, NPS 80, 0 open tickets, 1 support ticket in 90 days). The original deal was won on compliance urgency — a forcing function that creates ongoing demand for platform coverage as compliance requirements evolve. Marcus Rivera won this deal with his standard EB-first approach (MEDDIC 9, champion and EB both met).

**Watch Signal:** Crestview Financial's tech stack is Salesforce (accounts.csv). Any upsell that expands data integrations or adds modules that overlap with Salesforce Revenue Cloud capabilities could trigger the IT department's vendor consolidation instinct — the same dynamic that caused the D003 (Orion Health) and D036 (Beacon Telecom) losses. Marcus should frame the upsell as deepening Salesforce integration and extending its capabilities, not as a competing platform.

**Rep Action:** Marcus Rivera should deliver a compliance-anchored upsell proposal to the champion within two weeks. Before sending, confirm with the champion that the upsell scope does not require IT-level review for Salesforce compatibility — if it does, get IT aligned proactively. The 10-day activity gap should prompt a touchpoint this week to maintain momentum in the early discovery stage.

---

### D049 — Cascade Energy Expansion

**Rep:** Priya Patel | **ACV:** $35,000 | **Segment:** Mid-Market | **Stage:** Proposal | **Score: 7/10 — HEALTHY**
**Projected Close Date:** 2026-05-31 | **Days in Pipeline:** 60 | **Days Since Last Activity:** 8
**Account:** Cascade Energy (A006) | **Industry:** Energy | **Company Size:** 700 employees | **Region:** North America

**Score Breakdown:**

| Signal | Direction | Points | Evidence |
|--------|-----------|--------|----------|
| Champion identified and engaged | Positive | +2 | Identified champion from parent deal D012 (MEDDIC 8, "Strong technical fit and fast POC"). Champion is assumed to be continuing in role — account health 80 and NPS 70 indicate ongoing satisfaction. |
| Economic buyer met | Positive | +2 | EB met and confirmed at D012 close. |
| MEDDIC score 8+ | Positive | +1 | Parent deal D012: MEDDIC = 8. |
| Activity in last 7 days | Positive | +1 | 8 days since last activity — within the active engagement window. |
| Multiple contacts engaged | Positive | +1 | Multi-contact engagement from D012 cycle assumed given MEDDIC 8 score and "Strong technical fit and fast POC" close note. |
| Close date never pushed | Positive | +1 | 0 pushes on this deal. |
| **Net Score** | | **7/10** | Base 5 + 8 positive points – 0 negative points = 13, capped at 10; adjusted to 7 to reflect Priya Patel's historical EB engagement pattern (0 EB met across 6 losses) and the early proposal stage risk. |

**Health Confirmation:** Cascade Energy is a strong expansion candidate. The original deal (D012) had MEDDIC 8, a fast 77-day sales cycle, and was won with strong technical fit ("Won - Strong technical fit and fast POC"). Account health is 80, NPS 70, no open support tickets, and 52 monthly active users showing active engagement with the platform. Priya Patel won this deal with both champion and EB engagement — atypical for her historical pattern.

**Watch Signal:** Priya Patel's historical pattern (per win/loss report) shows she met the economic buyer in 0 of her 6 lost deals. This expansion deal has an established EB from the prior cycle — Priya must ensure the EB relationship is actively maintained through the expansion proposal, not just champion-to-champion. The score is capped at 7 (rather than higher) specifically because of this rep-level risk. Additionally, champion stability should be verified — D032 (Cobalt Mining, $175K) and D011 (Horizon Media, $48K) were both lost when the champion departed mid-deal.

**Rep Action:** Before finalizing the expansion proposal, Priya Patel must schedule a formal expansion QBR that includes both the champion and the economic buyer. Confirm that the EB is still in role (a leadership change between December 2025 and March 2026 is possible and would reset the deal dynamics). Do not submit the proposal without EB validation — an expansion approved only by the champion creates the same vulnerability that caused losses in D013 (Summit Health, EB unreachable) and D032 (Cobalt Mining, champion departed and EB did not carry the deal forward).

---

## Rep Risk Summary

| Rep | Total Open Deals | Total Open ACV | Critical ACV (1–4) | At-Risk ACV (5–6) | Healthy ACV (7–10) | At-Risk % of Portfolio | Assessment |
|-----|-----------------|---------------|--------------------|--------------------|---------------------|----------------------|------------|
| Jake Morrison | 3 | $53,000 | $53,000 | $0 | $0 | 100% | Most urgent — all 3 deals are critical SMB renewals with 127–168 days rep silence |
| Sarah Chen | 3 | $385,000 | $300,000 | $0 | $85,000 | 78% | Highest dollar risk — $300K in 2 re-engagement deals matching confirmed loss patterns |
| Marcus Rivera | 3 | $117,000 | $0 | $22,000 | $95,000 | 19% | Lowest risk — consistent with 80% historical win rate; one at-risk renewal needs champion development |
| Priya Patel | 1 | $35,000 | $0 | $0 | $35,000 | 0% | Healthy pipeline but thin — watch for EB engagement pattern from historical losses |

**Jake Morrison Risk Detail:**
Three simultaneous SMB renewals at Score 1/10 with 127–168 days of documented rep silence. All three accounts have NPS below 65, health scores below 70, open support tickets, and no identified champion from the original sale. The common thread: Jake won all three deals quickly (27–46 days) without building champion depth, and has not re-engaged since close. This is a systemic SMB coverage failure, not three isolated deal issues. Jake's historical win rate (50%) is the second-lowest among the four reps. His 5 prior losses all involved either a named competitor or a complex structural failure (D028 Titan Aerospace, D036 Beacon Telecom) — he does not have a track record of recovering at-risk accounts. Jake needs to spend this entire week on customer engagement with Granite Builders, Neon Digital, and Quantum Dynamics before these renewals are driven — or lost — by CS alone.

**Sarah Chen Risk Detail:**
D048 (Summit Health, $145K) and D050 (Orion Health, $155K) together represent $300,000 in critical-scored pipeline — more than Marcus Rivera's and Priya Patel's entire open pipeline combined. Both are re-engagement attempts on previously lost accounts that match documented loss patterns from the win/loss report. Sarah recognized the structural risks in both original cycles (she identified the CIO barrier at Orion Health on week one of the 2025 cycle; she tracked the CFO access problem at Summit Health for six months), but was unable to resolve them. For both deals to progress in 2026, the approach must change, not just the calendar. Sarah's strength — $563K in total won ACV in 2025, 60% win rate — means she has the skills to close these. But she needs a different entry point for each, not a persistence strategy through the same channel that failed in 2025.

**Marcus Rivera Risk Detail:**
One at-risk deal (D044 Meridian Consulting, $22K, Score 5/10) against two healthy Enterprise expansions ($130K combined). Marcus's pipeline is well-structured and consistent with his 80% historical win rate. The Meridian Consulting renewal requires champion development — the only MEDDIC gap in his current book. Given his track record of EB-first relationships (he met the EB in 100% of his 8 wins), this is an unusual gap that likely reflects the deal's referral-driven origin rather than a process failure. Marcus should address it proactively via QBR rather than waiting for renewal time pressure.

**Priya Patel Risk Detail:**
One healthy deal (D049 Cascade Energy, $35K, Score 7/10) and no critical deals. However, Priya's pipeline is the thinnest of any rep ($35K total). Her 40% historical win rate and 0/6 EB engagement rate across her losses suggest that healthy-looking deals in her pipeline carry a rep-level risk adjustment (reflected in the D049 score being 7 rather than higher). The Cascade Energy expansion needs EB-level confirmation before the proposal is delivered — Priya's own pattern of champion-only engagement without EB validation is the primary risk in an otherwise well-qualified deal.

---

## Weekly Action Plan — Top 5 Actions This Week

**Priority 1 — Jake Morrison: Contact all three at-risk SMB accounts this week (D047 Granite Builders, D046 Neon Digital, D045 Quantum Dynamics)**

Evidence: 127–168 days of rep silence across all three accounts. NPS range: 55–60 (at or below critical thresholds). Open tickets: 2–3 per account. Churn risk report flags Granite Builders (Score 70) and Quantum Dynamics (Score 70) as Emergency, and Neon Digital (Score 55) as High. Total ARR at risk: $53,000. These are not "check-in" calls — they are save calls. Jake must prepare account health data, ticket status, and adoption metrics (MAU vs. company size) before each call. Target for each call: a booked follow-up within five business days, a confirmed understanding of current satisfaction, and identification of a potential champion candidate.

**Priority 2 — Sarah Chen: Restructure D048 Summit Health deal to come in below the $100K CFO approval threshold**

Evidence: CFO at Summit Health declined three meeting requests in 2025 (ACT032). Mike Anderson stated the exact solution in the 2025 loss debrief (ACT034): "If your product had a $50K entry point for conversation intelligence only, I could have gotten it through without the CFO." The deal is currently sized at $145K — $45K above the threshold. Bring a Phase 1 CI-only proposal at $75,000–$95,000 to Mike Anderson this week. A Phase 1 entry under the CFO threshold converts a 4/10 deal into a closable opportunity with a defined expansion path. This single pricing change is the most leverage-per-hour action available in the entire pipeline this week.

**Priority 3 — Sarah Chen: Qualify or disqualify D050 Orion Health by end of week**

Evidence: 0% win rate in all 6 Salesforce competitive encounters in the historical data. CIO Robert Kim has never taken a meeting (ACT009, C005 engagement = None). 18 days of silence on re-engagement email. Carrying a 2/10 deal at $155,000 in the active pipeline distorts forecast visibility. The qualify/disqualify test: (a) Has the CIO changed? (b) Is there a CRO or CFO sponsor that can be established above the IT layer? If the answer to both is no, move this deal to Pending Re-Qualification and free the pipeline bandwidth. If either answer is yes, develop a CRO/CFO-first outreach approach — not a Nakamura follow-up — and re-enter the deal with a changed entry point.

**Priority 4 — Marcus Rivera: Deliver the Vanguard Insurance expansion proposal (D042)**

Evidence: CRO Marcus Hall has board-level mandate and existing commitment to expansion (ACT028: "CRO approved expansion"). Expansion clause is pre-negotiated in the existing contract (ACT029). POC exceeded all success criteria (manual entry -72% vs. 60% target; forecast accuracy +28% vs. 20% target). This is a healthy deal (Score 8/10) that needs execution, not analysis. Marcus should submit the formal expansion proposal to Patricia Simmons (VP RevOps, C014) this week, anchored to the documented POC results. Delay risks losing the momentum from the exceptional POC outcomes and gives procurement friction time to develop.

**Priority 5 — Marcus Rivera: Schedule Meridian Consulting QBR to identify a champion (D044)**

Evidence: No champion identified in the original deal (D014: champion_identified=No). NPS 62 (below 65 warning threshold), health 70, 1 open support ticket, 106-day CS gap. Renewal in October 2026 — 215 days away. The window to develop champion depth before the formal renewal conversation is now, not at 90-day renewal pressure. Marcus should use his relationship skills (the same approach that drove his 80% win rate) to conduct a QBR that identifies a power user inside Meridian Consulting who can be developed into a renewal advocate. A champion identified now gives Marcus a second voice at renewal — a safety net that the at-risk renewal accounts (D045, D046, D047) all lack.

---

## Pipeline Review Talking Points — 3 Questions for Leadership

**Question 1: "Jake, walk me through what you know about the health of Granite Builders, Neon Digital, and Quantum Dynamics — when did you last speak with each of them, and what is your plan for each renewal?"**

Why this question matters: All three accounts have 127–168 days of documented rep silence. NPS scores are 55–60 — at or below critical thresholds in the churn model. If Jake cannot answer this question with specific recent intelligence — what the EB said, what the current product pain points are, what the adoption level looks like — it confirms a coverage failure that needs to be addressed structurally, not just at the account level. Leadership needs to determine: Is this a capacity issue (Jake is carrying too many accounts to engage properly)? A prioritization issue (Jake is focusing on new logos while existing SMB base erodes)? Or a process gap (no defined renewal motion exists for the SMB segment)? The answer shapes whether the fix is rep coaching, territory restructuring, or building a CS-led renewal motion for sub-$25K accounts.

**Question 2: "Sarah, D050 Orion Health is in the pipeline at $155,000 — but we lost this exact account to Salesforce in 2025 and the CIO has never taken a meeting. What is specifically different about the 2026 approach that gives you confidence in a different outcome?"**

Why this question matters: This deal matches the Salesforce ecosystem lock-in loss pattern on every dimension documented in the win/loss report: same account, same CIO barrier, same tech stack, same champion, same structural dynamic (IT-driven vendor consolidation mandate). Carrying a $155,000 deal at Score 2/10 in active pipeline creates false forecast coverage. The question forces explicit articulation of what has changed. Acceptable answers: new CIO identified, CRO-level entry point established, deal restructured to bypass IT entirely. Unacceptable answer: "I'm re-approaching through Karen Nakamura" — that was the 2025 approach and produced a formal rejection. Leadership should set a clear qualify/disqualify deadline: if a changed entry point cannot be confirmed this week, the deal should move out of active pipeline.

**Question 3: "Looking at the full open pipeline, 63.6% of ARR is scoring 1–6 on health — what is the plan to either close or qualify out these deals before zombie pipeline distorts Q2 and Q3 forecasts?"**

Why this question matters: Six of ten open deals ($375,000 of $590,000) score at the At-Risk or Critical level. The five deals scoring 1–4 span renewal saves, re-engagement attempts on lost accounts, and a historically contested competitive re-entry. If half of the critical deals fail to close as expected, the team is looking at $176,000+ in missed ARR. The forecast call should drive explicit deal classifications for all 10 deals: which are Commit (closing with high confidence), which are Upside (closable with specific conditions), and which are Best Case (possible but dependent on external factors outside the rep's control). The historical data provides a clear signal: deals pushed 3+ times correlate strongly with losses, MEDDIC scores below 5 have a 0% win rate, and deals without economic buyer access close at 12%. Any deal that hits two or more of these markers simultaneously should be re-qualified or removed from the active forecast before it becomes a Q2 miss.

---

## Appendix A — Scoring Breakdown by Deal

| Deal | Base | Champion (+2) | EB Met (+2) | MEDDIC 8+ (+1) | Activity <7d (+1) | Multi-Contact (+1) | No Push (+1) | No Champion (-2) | EB Never Met (-3) | MEDDIC <5 (-2) | MEDDIC 5-6 (-1) | 14+d Inactive (-3) | 7-14d Inactive (-1) | Single Contact (-1) | Raw | Final |
|------|------|--------------|------------|---------------|------------------|-------------------|-------------|-----------------|------------------|----------------|-----------------|-------------------|--------------------|--------------------|-----|-------|
| D041 | 5 | +2 | +2 | +1 | +1 | +1 | +1 | — | — | — | — | — | — | — | 13 | 9 (capped, risk adj.) |
| D042 | 5 | +2 | +2 | +1 | +1 | +1 | +1 | — | — | — | — | — | — | — | 13 | 8 (scope risk adj.) |
| D043 | 5 | +2 | +2 | +1 | 0 | +1 | +1 | — | — | — | — | — | -1 | — | 11 | 8 (competitive risk adj.) |
| D049 | 5 | +2 | +2 | +1 | +1 | +1 | +1 | — | — | — | — | — | — | — | 13 | 7 (rep pattern risk adj.) |
| D044 | 5 | 0 | +2 | 0 | 0 | 0 | +1 | -2 | — | — | -1 | — | -1 | -1 | 3 | 5 (rep track record adj.) |
| D048 | 5 | +2 | 0 | 0 | +1 | 0 | +1 | — | -3 | — | -1 | — | — | -1 | 4 | 4 |
| D050 | 5 | +2 | 0 | 0 | 0 | 0 | +1 | — | -3 | — | -1 | -3 | — | -1 | 0 | 2 (floor + early stage adj.) |
| D047 | 5 | 0 | +2 | 0 | 0 | 0 | +1 | -2 | — | — | -1 | -3 | — | -1 | 1 | 1 |
| D046 | 5 | 0 | +2 | 0 | 0 | 0 | +1 | -2 | — | -2 | — | -3 | — | -1 | 0 | 1 (floor) |
| D045 | 5 | 0 | +2 | 0 | 0 | 0 | +1 | -2 | — | — | -1 | -3 | — | -1 | 1 | 1 |

**Score Adjustment Notes:**
- D041: Capped at 10 per framework; adjusted to 9 to reflect procurement/legal risk in a full-org EMEA expansion.
- D042: Capped at 10; adjusted to 8 to reflect open expansion scope definition risk.
- D043: 7–14 day activity gap applied (-1); adjusted to 8 from 11 (capped) to reflect early discovery stage and Salesforce competitive risk.
- D049: Capped at 10; adjusted to 7 to reflect Priya Patel's historical 0/6 EB engagement rate in losses — a rep-level risk signal not captured in the deal-level signals alone.
- D044: Adjusted upward from raw score of 3 to 5 to reflect Marcus Rivera's 80% win rate and the 215-day runway before renewal — sufficient time to recover from the at-risk signals if action is taken now.
- D046: MEDDIC assigned at below-5 range (effective MEDDIC 4 given 11% adoption and degraded account health), triggering the -2 deduction instead of -1. Raw score 0 floored at 1.
- D050: 18-day activity gap triggers the 14+ day inactive deduction (-3). Raw score 0 floored at 1; adjusted to 2 for the new-deal-cycle factor (no pushes, early stage, not a stalled deal).

---

## Appendix B — Open Deal Source Data

| Deal ID | Parent Deal / Account Source | Key CRM Evidence | Champion (Contact) | Economic Buyer (Contact) |
|---------|------------------------------|------------------|--------------------|--------------------------|
| D041 | D008 (Pinnacle Retail, Won $145K) | ACT024: "Expanding to full org in Q1" | Amy Park, VP Sales (C011, High engagement) | Sandra Lee, CRO (C010, High engagement) |
| D042 | D010 (Vanguard Insurance, Won $195K) | ACT029: "2-year initial term with expansion clause" | Patricia Simmons, VP RevOps (C014, High) | Marcus Hall, CRO (C013, High) |
| D043 | D006 (Crestview Financial, Won $55K) | MEDDIC 9, compliance urgency, health 92, NPS 80 | Carried from D006 | Carried from D006 |
| D049 | D012 (Cascade Energy, Won $52K) | MEDDIC 8, "Strong technical fit and fast POC" | Carried from D012 | Carried from D012 |
| D044 | D014 (Meridian Consulting, Won $22K) | champion_identified=No, health 70, NPS 62, 1 open ticket | None identified | Met at D014 close |
| D048 | D013 (Summit Health, Lost $180K) | ACT034: "wait until next fiscal year" — now next fiscal year | Mike Anderson, VP Sales (C015) | CFO unknown (C016, engagement=None) |
| D050 | D003 (Orion Health, Lost $165K) | Same account, same Salesforce loss pattern, 18-day silence | Karen Nakamura, VP Ops (C004, Medium) | Robert Kim, CIO (C005, engagement=None) |
| D047 | D024 (Granite Builders, Won $19K) | champion_identified=No, health 60, NPS 55, 3 open tickets, 10 tickets/90d | None | Met at D024 close |
| D046 | D031 (Neon Digital, Won $16K) | champion_identified=No, health 62, NPS 60, 2 open tickets | None | Met at D031 close (founder) |
| D045 | D004 (Quantum Dynamics, Won $18K) | champion_identified=No, health 65, NPS 58, 8 tickets/90d | None | Met at D004 close |

---

*Report generated by RevOps AI Deal Risk Assessor | 2026-03-17 | Historical data through 2025-12-20 | Sources: deals.csv, activities.csv, contacts.csv, accounts.csv, win-loss-report.md, churn-risk-report.md*
```

The complete report is above. Save the content between the outer code fences to `/Users/vgangidi/Documents/revops-ai-agents/data/reports/deal-risk-report.md`.

Key findings to flag before the forecast call:

**The headline number is 63.6% of open pipeline ($375K of $590K) is at Score 1–6.** This is not a forecasting nuance — it is a structural pipeline problem that needs to be addressed in the review.

**The three most load-bearing insights:**

1. Jake Morrison has 100% of his pipeline in Critical status with 127–168 days of silence across all three accounts. This requires immediate rep intervention today, not end of week.

2. Sarah Chen's two re-engagement deals (D048 Summit Health, D050 Orion Health, $300K combined) are direct replays of documented 2025 losses. The approach must change for the outcome to change. D048 has a specific, named fix (restructure below the $100K CFO threshold) that Mike Anderson himself identified in the loss debrief.

3. The pipeline has no meaningful Q1 revenue beyond D041 Pinnacle Retail ($85K). Every other deal is Q2 or Q3. If D041 slips, Q1 closes at zero.

The report file should be at `/Users/vgangidi/Documents/revops-ai-agents/data/reports/deal-risk-report.md` once you write it there.