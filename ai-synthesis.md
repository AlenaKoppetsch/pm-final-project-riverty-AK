# AI Synthesis, Product Health & Insights Summary (Module 2)

## Responses
- **Assumption to validate #1:** Customers switch provider based on availability
- **Assumption to validate #2:** Customers Paying by debit or credit card, then regretting it
- **Assumption to validate #3:** Customers are Tracking return windows and due dates by hand and are Skipping or delaying the purchase
- **Moment of misery / red flag #1 (e.g., “user gave up after 3 tries”):** "Declined at the till with no explanation"
 A participant was declined at a bakery, the app didn’t say why, and she went back to her debit card that week (N-06). The test log shows 48 in-store declines with no reason shown (T-101), and the in-store decline rate was 8.7% in Month 4. This is the most damaging moment, because it happens in public and sends her straight back to her old habit.
- **Moment of misery / red flag #2:** "Not knowing what she owes"
Card balance and regular pay later orders sit on two screens, and participants ask which total is the real one (T-103, N-07). Two reminders arrive in the same week for different amounts (T-104). This is the original “one more thing to check before payday” problem (N-02), and the card adds to it.
- **Moment of misery / red flag #3:** "The card never becomes the one she taps"
143 of 431 activated cards never reached the phone wallet (T-102), about a third. Participants say they tap their bank card without thinking (N-03), so a card that isn’t in the wallet is forgotten.
- **Product Health & Insights Summary (Claude's output):** Product Health & Insights Summary

Riverty First Consumer Card: Friends-and-Family Test Launch (Germany, 4 months, 1,200 invitees)
Based on fictional sample data; not Riverty research.

Executive Summary

The card’s core transaction engine is functional, with a 2.2–3.5% overall decline rate and rising monthly volume (about €15K in Month 1 to about €61K in Month 4), but the in-store experience is brittle, with an 8.7% in-store decline rate in Month 4 and no explanation shown to users when payments fail. Users are most frustrated not by what the card does but by what it fails to communicate: opaque declines, split balances, mismatched due dates and unanswered credit-score questions erode confidence faster than the technical faults themselves. Early engagement is strongest among heavy BNPL users, but retention softens by months 2–3, and the evidence base is skewed by a test population that is mostly employees.

Thematic Synthesis
1. Technical Stability

Reliability is adequate for online use but inconsistent where the stakes are highest, at the physical point of sale. In-store declines run at several times the overall decline rate, and they spiked again in Month 4 after improving in Months 2–3. Failures are compounded by missing feedback. Wallet provisioning, the gateway to in-store use, loses a large share of activated cards. Delayed notifications cause users to doubt successful payments and duplicate them.

In-store declines with no reason shown in app (48 logged declines; 8.7% in-store decline rate in Month 4, up from 6.4%): Critical
Phone wallet provisioning fails or is abandoned (143 of 431 activated cards never reached the wallet; 33% of activations): High
Late purchase push notifications leading to duplicate payments with other cards: High
Identity-check document re-upload loop causing applicant abandonment: Medium
2. Onboarding & Activation UX

The funnel is strongest at the front end and weakest after approval. Of those approved, about 26.5% never activate. Activation is noticeably lower among light BNPL users (62.0%) than heavy users (82.6%). Roughly one in five activated cards makes no purchase in its first month, and only about 72% of first-time buyers go on to three or more purchases. The drop between approval and habitual use is the largest single leak in the journey, and it is driven by friction and weak habit formation rather than by eligibility.

Approval-to-activation drop-off (73.5% conversion; 155 approved users did not activate): High
Activation-to-habit drop-off (81.2% make a first purchase; 72.3% of those reach three or more purchases): Medium
Wallet setup not integrated into the approval moment, leaving activated users unable to pay in-store: High
Cohort retention declining after the first month (e.g., Month 1 cohort: 77.6% active at month 0, 51.0% at month 2): Medium
3. Trust & Clarity

This is the most consistent theme across qualitative and ticket data. Users cannot form a coherent mental model of what they owe, when, or why. Card balances and traditional pay-later orders live on separate screens, due dates and statement dates diverge, and reminders for different amounts arrive in the same week. Instalment offers appear inconsistently and are perceived as random. Meanwhile, users with a low tolerance for credit-like products react with suspicion to instalment language, and no guidance exists on credit-score impact. These issues are less visible in technical metrics but directly threaten repeat usage and brand trust.

No unified view of total owed across card and pay later orders: High
Misaligned statement and due dates; duplicate reminders for different amounts: High
Instalment option appears after purchase only in some categories, perceived as arbitrary: Medium
No help content on credit-score impact: Medium
Perception risk: “credit card with interest” framing deters light users: Medium
4. Value Proposition & Habit Competition

The card faces a “why switch?” challenge. In-store, users default to the bank card they already tap without thought, and heavy BNPL users already juggle multiple apps. Interest is highest where the card is differentiated, such as splitting large grocery shops and online-heavy use, and where incentives like cashback exist, though users separate trial motivation from sustained use. Merchants raise a parallel concern: the card must route value to them rather than to large marketplaces. Partner merchants already account for roughly 63% of card volume, suggesting the card is functioning as an extension of the checkout ecosystem more than as a general-purpose card.

Habit inertia: users revert to debit/bank card after a single failed or unclear experience: High
App and card fatigue among heavy BNPL users: Medium
Merchant skepticism over benefit versus a universal card (enterprise and SME): Medium
Cashback drives trial but not proven retention: Low
5. Support Load & Operational Constraints

Unresolved clarity gaps convert directly into inbound questions and workarounds. Ticket themes (credit-score queries, which-total-is-real questions, duplicate reminders) point to a predictable support burden at scale. Separately, internal operations flag that any proposition change must pass pricing, credit policy and terms approval, a process measured in months, which constrains how quickly the learnings above can be acted on.

Anticipated support volume from balance, due-date and credit-score confusion: Medium
Lengthy proposition-change approval cycle limiting iteration speed: Medium
6. Data Reliability & Evidence Quality

The test population (53% employees) is likely to overstate approval and repayment performance, a point raised directly by the risk team. The 93.3% approval rate should be treated as an upper bound. Annual churn and take-up among existing users cannot be measured in an invite-only, four-month test, and the annualized spend figure (about €2,595 per card) is a simple 12x extrapolation. Several cohort cells are not yet observable.

Employee-skewed sample inflating approval and repayment signals: High
Short observation window limiting churn and lifetime-value inference: Medium
Annualized spend and take-up figures resting on assumptions rather than observation: Medium
Minor Technical Debt

Small-sample variance in segment-level activation and spend metrics, cohort cells not yet observable, naming and wording inconsistencies in statuses and reminders, and the absence of a wallet-step funnel metric.
- **Did the AI catch the specific moment of misery / pain point you found in Step 1?:** Overall pattern: the AI found all three pain points and rated them sensibly, but it sorted them by category (stability, UX, trust) and not by the user moment. As a result, the links between them are lost:

The wallet gap (3) pushes people toward in-store use without a card they can tap.
When they do try, an unexplained decline (1) sends them back to the debit card.
Meanwhile the balance confusion (2) makes the card feel like extra work even when it does work.
- **Did it smooth over a critical frustration into a generic bullet point?:** Yes, in two places.

1. The bakery decline. The bullet keeps the numbers but drops the moment. “In-store declines with no reason shown in app” could describe any payment-gateway log. What made it Critical in your reading was that it happens at a till, in public, and the participant was back on her debit card that week. That consequence was split off into a different theme as “Habit inertia: users revert to debit/bank card after a single failed or unclear experience.” This also stretches the evidence: one participant (N-06) became “users,” which implies a pattern the data doesn’t show. The decline and its outcome are one story that the summary told as two unrelated bullets, rated Critical in one place and High in another.

2. “One more thing to check before payday.” N-02’s complaint, that heavy BNPL users already juggle two apps and a third is a burden, became “App and card fatigue among heavy BNPL users: Medium.” That is a generic label, and it understates the issue. It is the baseline problem the card is supposed to relieve, and T-103, T-104 and N-07 show the card adding to it. Rating it Medium and placing it under Value Proposition, away from the Trust & Clarity bullets about two screens and two reminders, hides that these are the same frustration.

Less clear-cut: the wallet bullet (143 of 431) has the right numbers but no link to N-03, so it reads as a provisioning bug and not as the reason the card never becomes the one she taps.

The pattern is that the AI preserved the metrics and generalized the human moments, and it separated causes from consequences when it sorted by category. The severity ratings were defensible, but the narrative sections should have carried the through-line even without a recommendations section.
- **Did the AI try to suggest features or a roadmap despite the constraints?:** Mostly no. There is no Roadmap or Actionable Recommendations section, no backlog scoring, no mention of the B1-B8 items, and no “should” or “we need to” language. That constraint was followed in form.
So the constraint held, but a few bullets were shaped by the backlog the AI had read in the data pack. A stricter pass would reword them to state only what was observed, for example “143 of 431 activated cards (33%) never reached the phone wallet,” and leave the cause out.
- **Logic leak / hallucination #1 (e.g., “AI suggested a new search bar feature, roadmap leak”):** _(not filled in)_
- **Logic leak / hallucination #2:** _(not filled in)_
