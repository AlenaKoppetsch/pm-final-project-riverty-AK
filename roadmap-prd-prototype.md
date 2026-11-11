# Roadmap, PRD & Prototype (Module 4)

## Your strategic anchors
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
