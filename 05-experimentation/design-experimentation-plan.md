# Experimentation Plan (Module 5)

## Get your documents ready
- **From M3, your hypothesis sentence:** Based on N-06’s account of an unexplained bakery decline that sent her back to her debit card within the week, and an in-store decline rate of 8.7% in Month 4 (against 3.5% overall), I believe that showing a clear reason and retry hint on in-store declines for Alexandra, the active BNPL user who wants pay later in shops, will result in her retrying on Riverty instead of reverting to her debit card, as measured by a 15-point increase in the share of in-store declines followed by a successful Riverty purchase within 7 days. I will protect heavy-user purchases per active month (currently 5.82) and will make a go/no-go decision after 90 days or 100 logged in-store declines, whichever comes later.
- **From M3, your primary success metric & guardrail metric:** Share of in-store declines followed by a successful Riverty purchase within 7 days. Baseline is not in the data pack; it has to be measured in the first weeks & Heavy-user purchases per active month must stay at or above 5.82. Also watch that the overall decline rate does not exceed its Month 4 high of 3.5%.
- **From M4, the feature you scoped in your PRD this is what you're testing:** Decline reason and retry hint shown in the app

## Define your experiment parameters
- **Feature under test pull from your M4 PRD:** Decline reason and retry hint shown in the app
- **Persona pull your M2 persona:** Alexandra, the heavy BNPL user who wants Riverty in the shop. Goal: Use pay later at the supermarket and other shops, without a new thing to check before payday (N-04, N-02). Strategy: Riverty extends from a checkout-only pay later option into a card the consumer carries, so heavy BNPL users can pay later anywhere they shop, and Riverty keeps the transaction and the relationship that would otherwise go to her bank card.
- **Expected outcome the behaviour change you expect, from your M3 hypothesis:** after an in-store decline, Alexandra sees the reason and one next step, fixes it on the spot and retries with her Riverty Card, instead of reaching for her debit card and drifting away from Riverty.
- **Primary success metric the one number that defines success, from M3:** Share of in-store declines followed by a successful Riverty purchase within 7 days. Baseline is not in the data pack; it has to be measured in the first weeks.
- **Baseline rate today's rate of your primary metric, from your M3 data:** is not in the data pack and must be measured in the first weeks, we will go with 30%
- **Guardrail metric & boundary what must not break, and how far it can move before you investigate:** Heavy-user purchases per active month must stay at or above 5.82. Also watch that the overall decline rate does not exceed its Month 4 high of 3.5%.
- **Minimum Detectable Effect (MDE) the smallest improvement worth shipping, your floor:** +10 points over the measured baseline, with +15 kept as the target
- **Sample size per arm use the calculator in the builder, baseline + MDE:** 356
- **Traffic split & test duration 50/50 standard · cover ≥ 2 weekly cycles:** 50/50, 90 days
- **Significance threshold p < 0.05 is standard, explain any deviation:** p < 0.05

## Define your control and variant
- **Control (A) the current experience, reference your M2 moment of misery and M3 funnel/workflow data:** Declined at the till with no explanation" A participant was declined at a bakery, the app didn’t say why, and she went back to her debit card that week (N-06)
She gets to the till and the card fails. A bakery declines her with no reason shown (N-06, T-101), in public, and she goes back to her debit card that same week. 48 in-store declines were logged, and the in-store decline rate reached 8.7% in Month 4. Caveat: N-06 is a participant with no stated age or BNPL profile, so combining her with N-01/N-02 is a composite.
Current workaround , the external tool or manual process they rely on (M2): Fall back to the debit card at the till, Pay again with another card after a late notification
- **Variant (B) your single change, copy the relevant screens & functional requirements from your M4 PRD:** Decline notice delivered while she is still at the till. A reason that arrives after she has paid with her debit card does not change what happened at the bakery. -Reason and retry hint in the notification text itself. She can read it on the lock screen without opening the app, so no detail screen is needed in the first sprint. -Plain-language reasons for the most common decline codes. Cover only the codes that account for most declines. Each reason names the Riverty card, so she knows it was the card and not the shop or the terminal. -One next step per reason. For example “try again”, “use PIN” or “check your available limit in the app”. This is the retry hint, and without it the reason is only information. -A generic fallback for any decline we can’t explain or can’t legally disclose. It still says the payment was declined and what to try next. This guarantees no decline is silent (T-101). -Risk and legal approved copy, in German. This is wording, not terms, so it does not trigger the approval cycle in N-11. Fraud and credit-related declines need cautious text that doesn’t reveal how checks work.
- **Isolation check, what has NOT changed? list everything identical between arms (app version, eligibility rules, notifications, onboarding). If something changed inadvertently, your test is compromised.:** - Card approval, decline rules, limits and pricing. The PRD says the change is to what the app shows, not to how the card is approved or priced.
- No approve-anyway or limit-increase option in either arm.
- No fixes to why declines happen (processor, terminal, merchant category).
- No wallet setup (B2), balance view (B3) or due date (B8), and no credit-score messaging (T-107).
- No merchant-facing or terminal-side messages.
- Online declines: no notification in either arm, logged separately and excluded from the metric.
- Late notifications on successful payments (T-108) are not fixed, except where they block the 5-second target.
-The metric definition: the same numerator (a successful Riverty purchase within 7 days), the same denominator (in-store declines, including those with push off), the same 7-day window.
- App version and release train: the same build for both arms, and no other release touching payments, notifications or home screens during the test.
- Eligibility: who counts as a card customer, how arms are assigned (randomise by customer, not by week or merchant), and no overlap between arms in a household.
- Notifications: the same push infrastructure, the same opt-in prompt, and the same push-off rate in both arms. A gap in push opt-in alone would shift the result.
- Onboarding and activation flows: no change for either arm during the window.
- Marketing and incentives: no campaigns, cashback or reminders that aimed at in-store use in only one arm.
- Risk and credit policy: no changes to limits, approval rules or the decline-code mapping on the processor side.
- Terminals and merchants: no processor, terminal or merchant-mix change, since this changes the decline types customers see.
- Logging: the control arm must log declines with the same fields as FR8 (time, reason class, notified, recovered), or the arms aren’t comparable.
- Timing: both arms run over the same weeks. With a before/after design this can’t be satisfied, because seasonality, paydays and other releases differ between the periods.

## Formalize your hypothesis & shipping criteria
- **Your hypothesis (filled in):** I believe that showing a clear reason and one next step on in-store Riverty Card declines (a lock-screen notification, a decline detail screen and a retry confirmation) for Alexandra, the active pay-later user who wants to pay later in shops, will result in her fixing the problem at the till and retrying on Riverty instead of reverting to her debit card, as measured by a +15 percentage point change in the share of in-store declines followed by a successful Riverty purchase within 7 days within 90 days plus a 7-day follow-up window.
- **Your shipping criteria (filled in):** We will SHIP if the share of in-store declines followed by a successful Riverty purchase within 7 days improves by ≥ 10 percentage points (my proposed floor, with +15 as the target) at p < 0.05 (95% confidence, two-sided; my assumption), and heavy-user purchases per active month do not fall below 5.82 and the overall decline rate does not exceed 3.5% after 90 days plus the 7-day follow-up window.

We will ITERATE if the direction is positive but the lift is below +10 points, or the lift is at or above +10 but not statistically significant. In either case the effect is plausible but unproven. Examples of what to change are the copy, the step wording, or a notification-only version.

We will KILL if the primary metric shows no improvement or moves negatively (lift of 0 or below). A guardrail breach also blocks shipping whatever the primary result: it triggers a stop and review, not an automatic iterate.

The read date is fixed at the end of 90 days plus the 7-day follow-up (day 97), and no primary-metric results are reviewed before this date.
- **Hardest parameter to define, and did it change your hypothesis? quick debrief:** he baseline rate of the primary metric. It’s the one number the data pack doesn’t have, and the MDE, sample size and duration all depend on it. The 8.7% looks like a baseline but measures something else (how often in-store payments are declined, not how often a decline is followed by a Riverty purchase). All my figures for it (the 30% placeholder and the sample-size table) are assumptions until you measure it.
