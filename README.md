# Decline reason and retry hint shown in the app

> When your Riverty Card is declined at the till, you see why and what to try next within seconds, so you can pay with Riverty instead of reaching for your debit card

**Alena Koppetsch** · https://github.com/AlenaKoppetsch/pm-final-project-riverty-AK

Prototype: 04-roadmap/prototype.html

---

## Final Project Deliverables

### Slide 5 · Strategy
- **Problem:** ## Responses
- **Chosen path, which Riverty business-unit case are you using?:** Riverty's First Consumer Card
- **Strategic crisis, based on the brief, if the company does nothing for 12 months, what happens to its market position?:** Riverty is a two-sided business that owns only one side. It wins merchants, but consumers meet it only at checkout and only where a merchant offers it. Lena knows Riverty and doesn’t prefer it, so she picks whichever option appears. In that situation the checkout button is the whole relationship.
- **Moment of misery, what is the user likely doing outside the product (Google, spreadsheets, a competitor) because your tool isn’t serving them?:** Switching provider based on availability, Paying by debit or credit card, then regretting it, Tracking return windows and due dates by hand, Googling to compare, Skipping or delaying the purchase
- **Problem hook, summarize the business risk and user pain into one urgent sentence.:** Riverty is losing the people who use it most, because the moment Lena wants to decide-then-pay in a shop or at a non-partner merchant, Riverty isn’t there and Klarna or PayPal gets the sale and the relationship, which, left alone, erodes the consumer pull that makes Riverty worth a merchant’s checkout.
- **Value proposition, based on the initiative in your assigned Riverty case, what is the new value and why is it urgent to launch now?:** For Lena and users like her, who shop on their phones, use BNPL on most non-trivial purchases, and want money to leave their account only after they’ve decided to keep the item,

we will give them a Riverty card (friends-and-family test in Germany first) that brings decide-then-pay to every shop, online and in-store, not just Riverty merchants’ checkouts,

because today Riverty disappears exactly when she needs it, and she defaults to Klarna or PayPal, which erodes the consumer pull that makes Riverty valuable to merchants.

## Cold-read your own hook
- **Is the business risk high enough to justify a new initiative, a high-stakes threat, or a minor inconvenience?:** I would say its a high risk with a great potential
- **Is the moment of misery a systemic problem or just an edge case?:** Its a systematic problem
- **Does the value proposition actually remove the obstacle you identified, or is it a generic feature?:** Yes, it would remove the obstacle
- **Value proposition:** When an in-store payment with the Riverty Card is declined, the app sends a lock-screen notice within seconds. It gives one plain-language reason and one next step: try again, enter your PIN, check your limit in the app, or pay another way. If the reason can't be shared (for example fraud- or credit-related declines, or an unknown code), the notice still says the payment was declined and what to try next, so no decline is ever silent. If the retry works, she gets a confirmation. The change is to what the app shows. Card approval, limits, pricing and terms stay as they are.
For the customer: a declined card at the till, with a queue behind her, currently comes with no reason and no next step. She can't tell whether the card, the shop or the terminal failed, so she reaches for her debit card. With a reason and a step she can fix it on the spot and keep paying with Riverty.
For Riverty: heavy pay-later users are the people the card is meant for, and an unexplained decline sends them back to their bank card (N-06's bakery decline, T-101). In-store declines ran at 8.7% in Month 4 against 3.5% overall. Turning a failed payment into a successful Riverty purchase keeps the transaction and the relationship that would otherwise go to her bank.
- **Hypothesis:** ## Pre-work · Hypothesis check
- **Role , who you are solving for (from M2):** Alexandra, the heavy BNPL user who wants Riverty in the shop. Goal: Use pay later at the supermarket and other shops, without a new thing to check before payday (N-04, N-02). Strategy: Riverty extends from a checkout-only pay later option into a card the consumer carries, so heavy BNPL users can pay later anywhere they shop, and Riverty keeps the transaction and the relationship that would otherwise go to her bank card.
- **Goal , what this user is ultimately trying to achieve:** Use pay later at the supermarket and other shops, without a new thing to check before payday (N-04, N-02).
- **Friction / moment of misery , the specific pain blocking their goal:** She gets to the till and the card fails. A bakery declines her with no reason shown (N-06, T-101), in public, and she goes back to her debit card that same week. 48 in-store declines were logged, and the in-store decline rate reached 8.7% in Month 4. Caveat: N-06 is a participant with no stated age or BNPL profile, so combining her with N-01/N-02 is a composite.
- **Current workaround , the external tool or manual process they rely on (M2):** Fall back to the debit card at the till, Pay again with another card after a late notification
- **Problem Hook , your one-sentence framing of the business crisis (M1):** Riverty is losing the people who use it most, because the moment Lena wants to decide-then-pay in a shop or at a non-partner merchant, Riverty isn’t there and Klarna or PayPal gets the sale and the relationship, which, left alone, erodes the consumer pull that makes Riverty worth a merchant’s checkout.
- **Value Proposition , the outcome your initiative promised to deliver (M1):** For Lena and users like her, who shop on their phones, use BNPL on most non-trivial purchases, and want money to leave their account only after they’ve decided to keep the item,

## Read the evidence in your case
- **Where does your case say people stall or leave? Does that match the friction you wrote in Module 2?:** First purchase to habit (27.7%). Of 350 people who bought once, only 253 made three or more purchases in their activation month. The highest rate of loss is here, which fits N-03 and N-06: the card doesn’t become the one she reaches for.
- **What got better or worse in the case, and does that support the workaround your persona uses?:** Overall: the picture is growth that stalled in Month 4, with decline rates and cohort retention moving the wrong way
Better:
In-store declines fell sharply from Month 1 to Month 3
Spend per active card rose to EUR 233
Instalment use crept up
Worse:
Each cohort retains fewer people than the one before it by month 1.
Retention keeps decaying.
Does this support Alexandra’s workaround?

Directionally yes, but it doesn’t prove it. The workaround is a fallback to the debit card after an unexplained decline. Riverty never sees that payment, so the data can’t show it directly. The only direct evidence is still N-06, one participant.
- **Which user in the case is carrying the pain, and is that the person your Module 2 persona describes?:** The data shows who uses the card in shops, but it has no decline rates by segment, so it can’t show who actually feels the declines. What it does show is that the person most likely carrying the in-store pain is not quite Alexandra.
She matches the high-value segment. Heavy users have the best activation, highest spend (EUR 320.88 a month) and most purchases.
She doesn’t match the in-store behavior. Heavy users have the lowest in-store share of any segment (12.1%), and the 25-34 age band has the lowest of any age band (14.8%). Alexandra is the user who wants shop use but does it least.
Her goal quote comes from a different person. The supermarket wish (N-04) is an 18-24 heavy user. N-01 and N-02, the 25-34 users who give her profile, talk about online use and app fatigue, not shops.
The bakery moment has no profile. N-06 states no age or BNPL profile, so we don’t know who it happened to.
The habit-reversion pain looks more like N-03. That’s a regular user, 35-44, who taps the bank card by reflex. Regular users are the largest in-store group in the data, so my earlier Persona 2 may carry the in-store pain better than Alexandra.

## Step 2 · Craft your hypothesis
- **Qualitative evidence (from M2) , quote the specific friction / moment of misery for your persona:** N-06: “The card was declined at a bakery and the app did not say why. I went back to my debit card the same week.” Backed by T-101 (in-store decline, no reason shown) and N-03 (“In a shop I tap my bank card without thinking”).
- **Quantitative evidence (from M3) , name the metric or data point that confirms the pain; cite the number:** The in-store decline rate was 8.7% in Month 4, against 3.5% overall, about 2.5 times higher (206 in-store attempts, so roughly 18 declines). 48 in-store declines were logged across the pilot. The Month 3 cohort kept only 64.0% of its cards active in month 1, against 69.2% for the Month 2 cohort, and that month is when declines rose.
- **Persona , role, goal, and the friction you confirmed in the reconciliation steps:** Alexandra, an active BNPL user (heavy or regular) who already pays later online and wants it in shops without another thing to check before payday (N-04, N-02). The confirmed friction is an unexplained decline at the till. Composite of N-01, N-02, N-03, N-04 and N-06.
- **Problem you are solving , one sentence describing the specific friction this initiative removes:** When an in-store payment is declined, Alexandra gets no reason and no way to recover, so she pays with her debit card and stops trying Riverty in shops.
- **Strategic outcome , what behaviour change do you expect, and how does it map to retention / revenue / churn?:** After a decline she understands the cause, retries on Riverty, and keeps the in-store habit. Retention: more cards stay active past month 1 (64–69% now). Revenue: more in-store purchases (17.0% of purchases now) on a card averaging EUR 233 a month. Churn: fewer silent exits to the debit card. Churn itself can’t be measured in four months, so this is an expected effect, not an observed one.
- **Primary success metric (initiative signal) , the leading indicator that tells you the gap is closing:** Share of in-store declines followed by a successful Riverty purchase within 7 days. Baseline is not in the data pack; it has to be measured in the first weeks.
- **Guardrail metric (product signal) , the metric that must NOT drop; it protects your existing base:** Heavy-user purchases per active month must stay at or above 5.82. Also watch that the overall decline rate does not exceed its Month 4 high of 3.5%.
- **Decision window , how much time or data before you scale, pivot, or kill? minimum threshold to proceed?:** 90 days, which lets one cohort reach month 2, with at least 100 in-store declines logged. Scale if recovery improves 15 or more points over baseline and the guardrail holds. Pivot if it improves under 5 points but the in-store decline rate is falling. Kill if there is no movement after 90 days and 100 declines.
- **Draft your full hypothesis sentence , one to three sentences; quote the metric, name the persona, name the outcome:** Based on N-06’s account of an unexplained bakery decline that sent her back to her debit card within the week, and an in-store decline rate of 8.7% in Month 4 (against 3.5% overall), I believe that showing a clear reason and retry hint on in-store declines for Alexandra, the active BNPL user who wants pay later in shops, will result in her retrying on Riverty instead of reverting to her debit card, as measured by a 15-point increase in the share of in-store declines followed by a successful Riverty purchase within 7 days. I will protect heavy-user purchases per active month (currently 5.82) and will make a go/no-go decision after 90 days or 100 logged in-store declines, whichever comes later.

### Slide 6 · Research
- **Competitive analysis:** ## Responses
- **Role, who are you solving for? (the specific user segment or profile):** Alexandra, the heavy BNPL user who wants Riverty in the shop
- **Goal, what is this user ultimately trying to achieve?:** Use pay later at the supermarket and other shops, without a new thing to check before payday (N-04, N-02).
- **Friction, the main barrier (moment of misery) stopping them from succeeding:** She gets to the till and the card fails. A bakery declines her with no reason shown (N-06, T-101), in public, and she goes back to her debit card that same week. 48 in-store declines were logged, and the in-store decline rate reached 8.7% in Month 4. Caveat: N-06 is a participant with no stated age or BNPL profile, so combining her with N-01/N-02 is a composite.
- **External tools, the outside platforms or tools the user is forced to use:** Fall back to the debit card at the till,
Pay again with another card after a late notification
- **The process, the 3 to 5 manual steps the user takes to get the job done:** 1. Taps or presents the Riverty card at the till (e.g., the bakery).
2. The payment is declined and the app shows no reason (T-101).
3. She has no way to tell whether the problem is the card, the shop, her limit, or the terminal, so she cannot retry with any confidence.
4. She pays with her debit card instead, in front of the queue.
5. Within the week, she stops trying the Riverty card in-store and defaults to the debit card (N-06).

1. Pays in-store with the Riverty card.
2. No confirmation arrives, so she assumes the payment failed.
3. She pays again with another card.
- **Core frustration, the exact moment the process feels most “broken”:** 1. It costs her the benefit she wanted. Her goal is to pay later in shops. The debit card pays now, so she loses the deferral 
2. It adds the “one more thing to check” burden that she explicitly wants to avoid, because she now has to reconcile two charges across two accounts.
- **The evidence, a specific quote or behavior from the research that proves this:** 1. (N-01, N-04).
2. (N-02)
- **Your journey map file name (e.g. journey-map.html):** alexandra_future_state_journey.md
- **Journey map:** open > scan > hesitate (no message) > bounce to debit card > drift
new: open > scan > hesitate (notice in 5 s) > read > retry > recover > return

### Slide 7 · Blueprint
- **Roadmap:** ## Your strategic anchors
- **Persona (M2), who are you solving for?:** Alexandra, the heavy BNPL user who wants Riverty in the shop. Goal: Use pay later at the supermarket and other shops, without a new thing to check before payday (N-04, N-02). Strategy: Riverty extends from a checkout-only pay later option into a card the consumer carries, so heavy BNPL users can pay later anywhere they shop, and Riverty keeps the transaction and the relationship that would otherwise go to her bank card.
- **Primary success metric (M3), your leading indicator:** Share of in-store declines followed by a successful Riverty purchase within 7 days. Baseline is not in the data pack; it has to be measured in the first weeks.
- **Moment of misery (M2), the specific friction blocking the goal:** She gets to the till and the card fails. A bakery declines her with no reason shown (N-06, T-101), in public, and she goes back to her debit card that same week. 48 in-store declines were logged, and the in-store decline rate reached 8.7% in Month 4. Caveat: N-06 is a participant with no stated age or BNPL profile, so combining her with N-01/N-02 is a composite.
- **Guardrail metric (M3), what must not drop or break:** Heavy-user purchases per active month must stay at or above 5.82. Also watch that the overall decline rate does not exceed its Month 4 high of 3.5%.

## Scan the backlog & set a human baseline
- **My instinctive “quick wins” before touching the AI (2 to 3 feature IDs + why):** I believe that showing a clear reason and retry hint on in-store declines for Alexandra will result in her retrying on Riverty instead of reverting to her debit card

## Audit, override & decide
- **Where did you override the AI? (feature + old vs. new score + why):** One balance view for card and pay later orders, it was 3 and 4 and I switched to 4 and 3, because I think value is higher and effort lower and I will not cut it but do it later
- **Did the AI over-value a Sales/Eng request your M2 interviews don’t support?:** Over-valued

B5, partner offers (Sales ask): I gave it value 2, but the only support is N-08 and N-09, which are merchant interviews, not consumer ones. N-09 is also conditional (“if the card came with offers that send people to us”). No consumer note asks for it, and it doesn’t touch the declined payment, so the persona-based score should be 1. The outcome is unaffected because it is already cut.
B7, physical card: I gave it value 2, but no M2 note mentions a physical card. It is a backlog idea, so it should also be 1. It is cut as well, so nothing changes in the roadmap.
- **Did it underweight something your M3 cohort/funnel data strongly supports?:** The funnel’s two biggest experience drops have no feature aimed at them:

Approved to activated: 155 of 586 people (26.5%) never activate. This is the largest loss of people who wanted the card and passed checks.
First purchase to 3+ purchases: 97 of 350 (27.7%), the highest drop rate after approval.

## Generate your interactive roadmap
- **My “Now” lane (this sprint), the 2 to 3 quick wins I’ll build first:** -B1 Decline reason and retry hint shown in the app, It is the bakery moment itself (N-06, T-101) and directly drives the primary metric. It changes only the app display, not terms.
-B2 Add to phone wallet from the approval screen, 143 of 431 cards never reached the wallet (T-102), so those cards can’t compete with the bank card she taps (N-03). Effort is borderline because the cause of the failures is unknown.
- **What I cut, and the “no” I’m protecting the scope from:** -B4 Choose pay now or later per purchase after paying, It matches the value prop, but it’s an unobserved need (only N-01) and changes credit and pricing terms, which means months of approval (N-11).
- B5 Partner offers inside the card app, Merchants asked for this (N-08, N-09), but it does nothing for a declined payment. It’s a Sales preference.
- B6 Cashback on every purchase, Cashback drives trial, not retention (N-12), and affects margin and terms.
- B7 Physical card, It gives a path around wallet failures but doesn’t fix declines, adds one more thing to carry, and needs production and logistics.
- B8 One due date for card and pay later orders, It fixes the mismatched reminders (T-104), but changing due dates is a terms and collections change (N-11), and it doesn’t affect the primary metric.
- **Prototype/roadmap screenshot link (paste into your deliverables):** 04-roadmap/Backlog.png
04-roadmap/Cut-List.png
- **PRD highlights:** ## Pick & scope with MoSCoW
- **The “Now” feature I’m scoping (name + one-line core description):** Decline reason and retry hint shown in the app
It changes only the app display, no terms
- **My finalized Must-Haves (after overriding the AI):** -Decline notice delivered while she is still at the till. A reason that arrives after she has paid with her debit card does not change what happened at the bakery.
-Reason and retry hint in the notification text itself. She can read it on the lock screen without opening the app, so no detail screen is needed in the first sprint.
-Plain-language reasons for the most common decline codes. Cover only the codes that account for most declines. Each reason names the Riverty card, so she knows it was the card and not the shop or the terminal.
-One next step per reason. For example “try again”, “use PIN” or “check your available limit in the app”. This is the retry hint, and without it the reason is only information.
-A generic fallback for any decline we can’t explain or can’t legally disclose. It still says the payment was declined and what to try next. This guarantees no decline is silent (T-101).
-Risk and legal approved copy, in German. This is wording, not terms, so it does not trigger the approval cycle in N-11. Fraud and credit-related declines need cautious text that doesn’t reveal how checks work.
- **What I demoted from Must → Should/Won’t, and why:** Should have:
-Decline detail screen opened from the notification. It shows merchant, amount, time, reason and next step.
-Declines listed in the transaction history. This helps her tell a decline from the late-notification confusion in T-108.
-In-app banner for users without push. Only about 25% of the assumed base allows push (an assumed practice figure, not pilot data). If that holds, I would move this to Must.
-Online declines using the same reasons. I estimated earlier that more than half of declines may be online. That estimate is unverified.

Could have:
-Action buttons on the notification (“Retry”, “Open app”).
-Hints based on her history, such as a merchant type that often declines.
-A link from the decline screen to support.
-English copy.
-Copy variants for testing.

Won’t have (now):
-Any change to decline rules, limits or approval policy. That is terms and approval, which takes months (N-11).
-Approving or retrying a payment for her. This includes an “approve anyway” option or a limit increase.
-Fixing why declines happen. This covers processor, terminal and merchant-category causes.
-Wallet setup (B2), one balance view (B3) and one due date (B8). Each is a separate roadmap item.
-Credit-score messaging (T-107). This is a different pain from the one at the till.
-Merchant-facing or terminal-side messages.
-Fixing late notifications for successful payments (T-108). This is a separate bug, but it overlaps with the first Must (see below).

## Generate your Simplified PRD
- **One thing my PRD makes explicit that a vague brief would have missed:** A vague brief would say “show the decline reason” and leave out that some reasons can’t be shown.

Your PRD handles this in two places. Requirement 6 sends any unmapped code, and any fraud- or credit-related code, to a fallback that says the payment was declined and what to try, but never states the cause. The safety guard under Edge cases then limits all copy to a closed list of approved strings keyed by decline code, so nothing is generated or guessed at runtime.

Without that, a team could easily build “always tell her why” and then discover in legal review that it exposes how fraud and credit checks work. The reason is the core of the feature, so this is the part most likely to be redone late.

One gap remains: the data pack doesn’t say which decline codes the processor returns or which ones are non-disclosable. Risk and legal have to supply that list before the map can be finished.

## Prompt-to-prototype sprint
- **Where did the prototype reveal a gap in my PRD logic? (what I had to update):** I just had some technical errors in the beginning, so prototype was not working before it got adjusted
- **My prototype: save Claude's HTML as prototype.html in 04-roadmap/, open it in your browser, and add a screenshot:** 04-roadmap/prototype.html
- **Prototype:** 04-roadmap/prototype.html

### Slide 8 · Validation
## Parameters
| Parameter | Decision |
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

### Slide 9 · Launch
- **GTM:** # GTM Launch Plan, Riverty BU Pay & Credit, First Consumer Card

| Field | Value |
| Feature | Decline reason and retry hint shown in the app |
| Goal | Conversion |
| Launch tier | S, Minimal |

## Goal & Audience
- **Goal:** Conversion, primary metric (the share of in-store declines followed by a successful Riverty purchase within 7 days) is a conversion metric. The feature exists to stop Alexandra from switching to her debit card at the till, so success is her paying with Riverty, not seeing or opening something.
- **Target audience:** active Riverty Card holders who are heavy pay-later users, and who have an in-store payment declined during the test window.

## Launch Tier
- **S, Minimal**, Risk of silence: Today every decline is silent, which is the pain (T-101, N-06). That is a sharp problem for the few it hits. The risk in the fix is wrong or legally sensitive copy, mainly for fraud and credit declines.

## Channels
1. **Owned: Lock-screen push notification (the treatment) Owned - The only channel that reaches her within seconds of the decline. T-108 shows pushes can arrive minutes late, so delivery speed is the risk.**
2. **Owned: Customer support (chat and phone scripts) Owned - The people she contacts after an unexplained decline (N-06’s bakery decline, T-101). They need to say the same thing the notice says.**
3. **Owned: In-app release note and help-centre entry Owned - Cheap and findable. It tells existing card holders what the notice means, without a campaign.**

## Enablement & Assets
Support and CS carry most of the enablement. Sales needs almost nothing, because the feature is customer-facing, has no merchant-side messages, and doesn’t change terms or pricing. The prototype can serve as the demo.
Support: The exact notice wording, what each next step means, and how to handle customers who got no notice (push off, online, late, or control arm). A macro and an escalation path for wrong or confusing notices.
CS: The one-line positioning, the say/don’t-say list, and the result after the read date.
Sales: A short FYI: consumer-only, no merchant or terminal messages, no change to approval or pricing.
Assets:
1. Approved German notification strings (closed list). Owner: Risk and legal, product.
2. Code-to-string map and fallback rules. Owner: Product, engineering.
3. One-pager (internal): what it is and isn't, the four next steps, fallback rule, who to ask. Owner: Product.
4. Say / don't say card (above). Owner: Product, legal.
5. Notice cheat sheet: each approved string next to its decline code and next step. Owner: Product, support.
6. Support macros and FAQ: "Why was I declined?", "I got no message", "My message came late", "The notice says pay another way". Owner: Support.
7. Escalation path for wrong, confusing or unsafe notices, with a named response owner. Owner: Product, support.
8. Demo: the clickable prototype (riverty-decline-prototype.html), fictional data only. Owner: Product.
9. 5-minute walkthrough of the demo for support and CS, including the loop rule and fallback. Owner: Product.
10. Metric and arm definition sheet. Owner: Data.

## Ownership, Budget & Timeline
- **Ownership & budget:** Ownership
Beta:
Wk 1: Confirm weekly in-store decline volume and the period behind the 48 declines; decide the sample-size option. Owner: Data analyst, with @Alena.
Wk 1-2: Back-fill baseline; fix metric and "heavy user" rule. Owner: Data analyst.
Wk 1-2: Closed code-to-string map and fallback rules. Owner: @Alena.
Wk 2-5: German strings approved (no implied change to limits, terms or approval). Owner: Legal reviewer, Risk reviewer co-signs.
Wk 2-5: Build notification, delivery logging, decline log, 5-second check. Owner: Engineering lead.
Wk 3-4: Arm assignment built and tested. Owner: Data analyst.
Wk 4-5: Usability test with 5 people. Owner: Design owner.
Wk 5: Scripted check of 12 cases plus legal read. Owner: Engineering lead.
Wk 5-6: Internal dogfood on staff cards. Owner: Engineering lead.
Wk 5-6: Support pack. Owner: Support lead.
Wk 5-6: One-pager, say/don't say card, demo walkthrough, CS and Sales FYI. Owner: @Alena; CS lead and Sales contact acknowledge.
Wk 6: Freeze list agreed. Owner: @Alena.
Launch moment: Switch on the variant for 50% of eligible customers. Owner: Engineering lead.
Confirm the split and that the decline log is recording. Owner: Data analyst.
Support on standby with macros and escalation path. Owner: Support lead.
No external messaging. Owner: Comms owner.
Post-launch:
Wk 1-4: Stop rule for any guardrail breach or unsafe notice. Owner: @Alena.
Wk 1-6: Tag and count decline-related contacts. Owner: Support lead.
Wk 1-6: Log wrong, late or confusing notices; fix the map (new strings need legal re-approval). Owner: Engineering lead; Legal reviewer.
Wk 5: Follow-up week, no new enrolment. Day 35 READ against the shipping criteria. Owner: Data analyst.
Wk 6: Record the decision (ship, iterate, extend once, or kill) with reasons. Owner: @Alena.
Wk 6: Results summary to Support, CS, Sales and Risk. Owner: @Alena.
Wk 6: If SHIP: roll out to 100%, publish help article and release note. Owners: Engineering lead; Support lead; Comms owner.
Wk 6: If ITERATE or EXTEND: scope the next test or the extension. Owner: Design owner.
Wk 6: If KILL: switch the variant off and close the log. Owner: Engineering lead.
Wk 6 onward: Review flagged notices and new decline codes; set up a standing string review. Owner: Legal reviewer.
Budget:
Beta:  get an estimate or "absorbed in current budget"): German translation and legal review (Legal reviewer); engineering build and any latency fix (Engineering lead); experiment tooling if none exists (Data analyst); usability participants (Design owner); support briefing time (Support lead).
Launch moment: 
engineering and support standby time for the day.
Post-launch: 
 analyst time for weekly checks; engineering fixes; support handling of new contacts; legal re-review; help article and release note with translation (ship only); full rollout engineering (ship); next-test design (iterate); extra run time if extended.
- **Timeline:** Beta: 6 weeks
Launch moment: 1 day
Post-launch: 6 weeks
Beta:
Wk 1: Confirm weekly in-store decline volume and the period behind the 48 declines; decide the sample-size option. Owner: Data analyst, with @Alena.
Wk 1-2: Back-fill baseline; fix metric and "heavy user" rule. Owner: Data analyst.
Wk 1-2: Closed code-to-string map and fallback rules. Owner: @Alena.
Wk 2-5: German strings approved (no implied change to limits, terms or approval). Owner: Legal reviewer, Risk reviewer co-signs.
Wk 2-5: Build notification, delivery logging, decline log, 5-second check. Owner: Engineering lead.
Wk 3-4: Arm assignment built and tested. Owner: Data analyst.
Wk 4-5: Usability test with 5 people. Owner: Design owner.
Wk 5: Scripted check of 12 cases plus legal read. Owner: Engineering lead.
Wk 5-6: Internal dogfood on staff cards. Owner: Engineering lead.
Wk 5-6: Support pack. Owner: Support lead.
Wk 5-6: One-pager, say/don't say card, demo walkthrough, CS and Sales FYI. Owner: @Alena; CS lead and Sales contact acknowledge.
Wk 6: Freeze list agreed. Owner: @Alena.
Launch moment: Switch on the variant for 50% of eligible customers. Owner: Engineering lead.
Confirm the split and that the decline log is recording. Owner: Data analyst.
Support on standby with macros and escalation path. Owner: Support lead.
No external messaging. Owner: Comms owner.
Post-launch:
Wk 1-4: Stop rule for any guardrail breach or unsafe notice. Owner: @Alena.
Wk 1-6: Tag and count decline-related contacts. Owner: Support lead.
Wk 1-6: Log wrong, late or confusing notices; fix the map (new strings need legal re-approval). Owner: Engineering lead; Legal reviewer.
Wk 5: Follow-up week, no new enrolment. Day 35 READ against the shipping criteria. Owner: Data analyst.
Wk 6: Record the decision (ship, iterate, extend once, or kill) with reasons. Owner: @Alena.
Wk 6: Results summary to Support, CS, Sales and Risk. Owner: @Alena.
Wk 6: If SHIP: roll out to 100%, publish help article and release note. Owners: Engineering lead; Support lead; Comms owner.
Wk 6: If ITERATE or EXTEND: scope the next test or the extension. Owner: Design owner.
Wk 6: If KILL: switch the variant off and close the log. Owner: Engineering lead.
Wk 6 onward: Review flagged notices and new decline codes; set up a standing string review. Owner: Legal reviewer.
Beta:  get an estimate or "absorbed in current budget"): German translation and legal review (Legal reviewer); engineering build and any latency fix (Engineering lead); experiment tooling if none exists (Data analyst); usability participants (Design owner); support briefing time (Support lead).
Launch moment: 
engineering and support standby time for the day.
Post-launch: 
 analyst time for weekly checks; engineering fixes; support handling of new contacts; legal re-review; help article and release note with translation (ship only); full rollout engineering (ship); next-test design (iterate); extra run time if extended.

## Success Metrics
- **Metrics:** 1. Share of in-store declines followed by a successful Riverty purchase within 7 days (variant minus control).
Worked if: at least +10 points over control, 95% confidence interval lower bound above 0.
2. Share of in-store declines followed by a successful Riverty payment at the same merchant within 30 minutes (variant minus control).
Worked if: clearly higher in the variant. This shows the misery at the till was resolved, not just that she bought something later
- **Bad signal to watch for:** 1. - Control rate is already high (for example above 60%). Heavy users may buy again within 7 days whatever we show, so there is little headroom. Next step: tighten the definition to in-store card purchases only and add the same-day metric below. - Lift is positive but under +10, or the interval is wide. Sample too small (about 48 declines at 12 a week, assumption). Next step: ITERATE or use the one pre-agreed extension. Don't call it a win. - Lift is zero or negative. Next step: KILL, then review the notice text with the usability results before any new test. 2. - The 7-day metric rises but this one is flat. The gain comes from unrelated purchases, not from the notice. Next step: don't ship on the 7-day result alone. - It is flat for mapped codes too. The next step or wording doesn't work. Next step: iterate the copy.
- **Likely post-launch decision:** MOST LIKELY POST-LAUNCH DECISION: ITERATE  Why: sample is too small to prove +10 points at day 35, so a directional read is the most probable outcome.  TRIGGERS BY DECISION (all thresholds are my proposals)  DOUBLE-DOWN (ship, roll out to 100%, extend to the detail screen, online declines or wider eligibility) Trigger: primary metric at least +10 points over control with the 95% interval lower bound above 0, and the same-day recovery metric also clearly up, and all guardrails held (purchases per active month at or above 5.82 and no more than 0.3 below control, decline rate at or below 3.5%), 0 unsafe notices, validity checks pass. Least likely at this volume. Also possible if real decline volume is well above 12 a week.  ITERATE (change the copy, the next-step wording, the code map or the delivery speed, then retest or use the one pre-agreed extension) Trigger: lift positive but under +10, or at least +10 but not significant, or the sample target not reached. Also: lift concentrated in mapped declines but weak in fallback ones (add codes to the map); notices late against the 95% within 5 seconds target (fix latency first, then rerun); testers or taps show people read the notice but don't act on the step (rewrite the step).  PIVOT (change the approach, not the wording) Trigger: the lift is zero overall, but the same-day recovery or a segment shows a pattern pointing to a different cause. Examples: most declines are fraud, credit or unmapped so a reason can't be shown (the problem is the decline itself, which is out of scope for this PRD); the control arm already recovers most declines (no headroom, so the pain is not at the till); declines cluster at one merchant type or terminal (a merchant or processor fix, also out of scope). Next step: take the finding back to discovery before building anything else.  DEPRIORITIZE (kill or park) Trigger: lift zero or negative, or the interval upper bound below +5, with the sample adequate; or the volume of in-store declines is too small to ever matter (for example under about 5 a week); or a guardrail harm that can't be fixed with copy. Action: switch the variant off, keep the decline log, revisit only if volume or the decline rate (8.7% in-store in Month 4) grows.  WHAT TO CHECK FIRST AT THE READ 1. Real weekly in-store decline volume, and whether each arm reached its target. 2. Control-arm recovery rate (is there headroom?). 3. Same-day recovery versus 7-day recovery (did the notice fix the moment at the till?). 4. Results by reason class. 5. Guardrails and validity checks.
- **Metrics:** PRIMARY METRIC
Share of in-store declines followed by a successful Riverty purchase within 7 days (variant minus control).
Success: at least +10 points, 95% interval lower bound above 0.
Bad signals and next step:
- Control rate is already very high (for example above 60%): little headroom. Tighten the definition to in-store card purchases and rely on the same-day metric.
- Lift positive but under +10, or a wide interval: sample too small (about 48 declines at 12 a week, an unconfirmed assumption). Iterate or use the one pre-agreed extension.
- Lift zero or negative: kill, then review the notice text before any new test.

SECONDARY METRIC (THE MOMENT AT THE TILL)
Share of in-store declines followed by a successful Riverty payment at the same merchant within 30 minutes.
Success: clearly higher in the variant.
Bad signals and next step:
- 7-day metric up but this one flat: the gain comes from unrelated purchases. Don't ship on the 7-day result alone.
- Flat for mapped codes too: the step or wording doesn't work. Iterate the copy.

### Slide 10 · Story
- **Friction + aha:** 1. No baseline (biggest)
The primary metric has no measured baseline, and 30% is a placeholder. The target, the sample size and the "+10 floor" all depend on it. The 8.7% decline rate is easy to mistake for it.
Unblock: back-fill from the 48 logged declines in Week 1, and use the control arm as the baseline at the read.

2. Volume may be too small to read
At about 12 in-store declines a week (assumption, the period behind the 48 is unknown), a 6-week window gives about 48 declines against 356 per arm needed. A significant result is unlikely.
Unblock: confirm weekly volume in Week 1, then pick one: widen eligibility, accept a larger MDE, or run it as a directional pilot with one pre-agreed extension.

3. The experiment is bigger than the feature
The release is size S, but the test needs about 712 declines. Over-investing here costs as much as under-investing.
Unblock: say up front that the first read is directional, and keep the build to the notification.
- **Takeaways / next:** 1. The idea is sound and small. A reason and one next step at a decline fixes a real, evidenced pain (N-06's unexplained bakery decline, T-101's 48 silent in-store declines, 8.7% in-store decline rate in Month 4). It is a size S release, not a launch, and needs no go-to-market campaign.
2. The metric is conversion. Success is a failed in-store payment becoming a successful Riverty purchase (primary: within 7 days; secondary: same merchant within 30 minutes). Opens and taps are diagnostics only.
3. The baseline is the biggest gap. It isn't in the data pack, 30% is a placeholder, and the 8.7% is the decline rate, not the baseline.
4. The experiment is bigger than the feature. 356 per arm means about 712 declines. At about 12 a week (an unconfirmed assumption) a 6-week window gives about 48, so a significant read is unlikely and "iterate" is the most likely decision.

---

Submitted to the Product Management Certification learning platform · Product School.
