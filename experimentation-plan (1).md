# A/B Experiment Brief, Riverty BU Pay & Credit, First Consumer Card

## Parameters
| Parameter | Decision |
|---|---|
| Feature under test | Decline reason and retry hint shown in the app |
| Persona | Alexandra, the heavy BNPL user who wants Riverty in the shop. Goal: Use pay later at the supermarket and other shops, without a new thing to check before payday (N-04, N-02). Strategy: Riverty extends from a checkout-only pay later option into a card the consumer carries, so heavy BNPL users can pay later anywhere they shop, and Riverty keeps the transaction and the relationship that would otherwise go to her bank card. |
| Expected outcome | after an in-store decline, Alexandra sees the reason and one next step, fixes it on the spot and retries with her Riverty Card, instead of reaching for her debit card and drifting away from Riverty. |
| Primary success metric | Share of in-store declines followed by a successful Riverty purchase within 7 days. Baseline is not in the data pack; it has to be measured in the first weeks. |
| Baseline rate | is not in the data pack and must be measured in the first week, currently we take 30% as an assumptions |
| Guardrail metric | Heavy-user purchases per active month must stay at or above 5.82. Also watch that the overall decline rate does not exceed its Month 4 high of 3.5%. |
| Guardrail boundary | Also watch that the overall decline rate does not exceed its Month 4 high of 3.5%. |
| Second guardrail | · |
| Minimum Detectable Effect | +10 points over the measured baseline, with +15 kept as the target |
| Sample size per arm | 356 |
| Traffic split | 50/50 |
| Test duration | 90 |
| Significance threshold | p < 0.05 |

## Control vs. Variant
- **Control (A):** Current workaround , the external tool or manual process they rely on (M2): Fall back to the debit card at the till, Pay again with another card after a late notification
- **Variant (B):** Decline notice delivered while she is still at the till. A reason that arrives after she has paid with her debit card does not change what happened at the bakery. -Reason and retry hint in the notification text itself. She can read it on the lock screen without opening the app, so no detail screen is needed in the first sprint. -Plain-language reasons for the most common decline codes. Cover only the codes that account for most declines. Each reason names the Riverty card, so she knows it was the card and not the shop or the terminal. -One next step per reason. For example “try again”, “use PIN” or “check your available limit in the app”. This is the retry hint, and without it the reason is only information. -A generic fallback for any decline we can’t explain or can’t legally disclose. It still says the payment was declined and what to try next. This guarantees no decline is silent (T-101). -Risk and legal approved copy, in German. This is wording, not terms, so it does not trigger the approval cycle in N-11. Fraud and credit-related declines need cautious text that doesn’t reveal how checks work.
- **Held constant (isolation check):** - Card approval, decline rules, limits and pricing. The PRD says the change is to what the app shows, not to how the card is approved or priced.
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

## Hypothesis
> I believe that Decline reason and retry hint shown in the app for Alexandra, the heavy BNPL user who wants Riverty in the shop. Goal: Use pay later at the supermarket and other shops, without a new thing to check before payday (N-04, N-02). Strategy: Riverty extends from a checkout-only pay later option into a card the consumer carries, so heavy BNPL users can pay later anywhere they shop, and Riverty keeps the transaction and the relationship that would otherwise go to her bank card. will result in after an in-store decline, Alexandra sees the reason and one next step, fixes it on the spot and retries with her Riverty Card, instead of reaching for her debit card and drifting away from Riverty., as measured by a +10 points over the measured baseline, with +15 kept as the target change in Share of in-store declines followed by a successful Riverty purchase within 7 days. Baseline is not in the data pack; it has to be measured in the first weeks. within 90. We will protect Heavy-user purchases per active month must stay at or above 5.82. Also watch that the overall decline rate does not exceed its Month 4 high of 3.5%. throughout the test.

## Shipping criteria
> We will **ship** if Share of in-store declines followed by a successful Riverty purchase within 7 days. Baseline is not in the data pack; it has to be measured in the first weeks. improves by ≥ +10 points over the measured baseline, with +15 kept as the target at p < 0.05 and Heavy-user purchases per active month must stay at or above 5.82. Also watch that the overall decline rate does not exceed its Month 4 high of 3.5%. does not reach Also watch that the overall decline rate does not exceed its Month 4 high of 3.5%. after 90.
> We will **iterate** if direction is positive but lift is below the MDE.
> We will **kill** if the primary metric shows no improvement or moves negatively.
> The read date is fixed at the end of 90, no results reviewed before this date.
