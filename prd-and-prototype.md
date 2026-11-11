# PRD & Prototype Sprint (Module 4)

## Pick & scope with MoSCoW
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
