# GTM Strategy & Success Dashboard (Module 6)

## Get your prior work ready
- **The feature you're launching from your M4 PRD, one feature, not a list:** Decline reason and retry hint shown in the app
- **What your M5 experiment will test your hypothesis, primary metric and ship / iterate rule, the evidence the launch rests on:** Based on N-06’s account of an unexplained bakery decline that sent her back to her debit card within the week, and an in-store decline rate of 8.7% in Month 4 (against 3.5% overall), I believe that showing a clear reason and retry hint on in-store declines for Alexandra, the active BNPL user who wants pay later in shops, will result in her retrying on Riverty instead of reverting to her debit card, as measured by a 15-point increase in the share of in-store declines followed by a successful Riverty purchase within 7 days. I will protect heavy-user purchases per active month (currently 5.82) and will make a go/no-go decision after 90 days or 100 logged in-store declines, whichever comes later.
Share of in-store declines followed by a successful Riverty purchase within 7 days. Baseline is not in the data pack; it has to be measured in the first weeks.
 We will SHIP if the share of in-store declines followed by a successful Riverty purchase within 7 days improves by ≥ 10 percentage points (my proposed floor, with +15 as the target) at p < 0.05 (95% confidence, two-sided; my assumption), and heavy-user purchases per active month do not fall below 5.82 and the overall decline rate does not exceed 3.5% after 90 days plus the 7-day follow-up window.
- **Your persona pull your M2 persona, this anchors your audience:** Alexandra, the heavy BNPL user who wants Riverty in the shop. Goal: Use pay later at the supermarket and other shops, without a new thing to check before payday (N-04, N-02). Strategy: Riverty extends from a checkout-only pay later option into a card the consumer carries, so heavy BNPL users can pay later anywhere they shop, and Riverty keeps the transaction and the relationship that would otherwise go to her bank card.

## Set your goal, then your audience
- **Primary GTM goal awareness · engagement · conversion, pick one:** Conversion
- **Why this goal? what makes this the right goal for this feature right now:** primary metric (the share of in-store declines followed by a successful Riverty purchase within 7 days) is a conversion metric. The feature exists to stop Alexandra from switching to her debit card at the till, so success is her paying with Riverty, not seeing or opening something.
- **Target audience the specific segment your goal implies, be precise:** active Riverty Card holders who are heavy pay-later users, and who have an in-store payment declined during the test window.

## Size your launch
- **Launch tier S (minimal) · M (targeted) · L (multi-channel) · XL (full GTM):** S
- **Justification reach + revenue impact + what silence would risk:** Users affected: Only active card holders who get an in-store decline. The PRD logs 48 in-store declines (T-101) with no period attached.	S
Revenue impact: No direct revenue. No pricing, limit or approval change. The value is indirect: keeping heavy users (5.82 purchases per active month) from drifting to debit. I have no revenue figure for this, so any number would be invented.	S
Risk of silence: Today every decline is silent, which is the pain (T-101, N-06). That is a sharp problem for the few it hits. The risk in the fix is wrong or legally sensitive copy, mainly for fraud and credit declines.
- **Is this a launch or a release? does it need go-to-market, or can it just ship?:** It’s a release, not a launch. It can just ship, with a small amount of internal readiness and no go-to-market.

## Choose your top three channels and plan assets
- **Channel 1 owned / earned / paid, and why it reaches your audience:** Lock-screen push notification (the treatment)
Owned - The only channel that reaches her within seconds of the decline. T-108 shows pushes can arrive minutes late, so delivery speed is the risk.
- **Channel 2 owned / earned / paid, and why:** Customer support (chat and phone scripts)
Owned - The people she contacts after an unexplained decline (N-06’s bakery decline, T-101). They need to say the same thing the notice says.
- **Channel 3 owned / earned / paid, and why:** In-app release note and help-centre entry
Owned - Cheap and findable. It tells existing card holders what the notice means, without a campaign.
- **Enablement & assets what Sales / CS / Support need, plus the assets to build (one-pager, demo, etc.):** Support and CS carry most of the enablement. Sales needs almost nothing, because the feature is customer-facing, has no merchant-side messages, and doesn’t change terms or pricing. The prototype can serve as the demo.
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

## Make it executable
- **Ownership named owner per key activity, individual, not department:** Beta:
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
- **Budget & resource gaps what costs extra, and any asset you can't currently build:** Beta:  get an estimate or "absorbed in current budget"): German translation and legal review (Legal reviewer); engineering build and any latency fix (Engineering lead); experiment tooling if none exists (Data analyst); usability participants (Design owner); support briefing time (Support lead).
Launch moment: 
engineering and support standby time for the day.
Post-launch: 
 analyst time for weekly checks; engineering fixes; support handling of new contacts; legal re-review; help article and release note with translation (ship only); full rollout engineering (ship); next-test design (iterate); extra run time if extended.
- **Timeline Phase 1 beta → Phase 2 launch moment → Phase 3 post-launch:** Beta: 6 weeks
Launch moment: 1 day
Post-launch: 6 weeks

## Define how you'll know it worked
- **Success metrics 2 to 3 metrics that match your GTM goal:** 1. Share of in-store declines followed by a successful Riverty purchase within 7 days (variant minus control).
Worked if: at least +10 points over control, 95% confidence interval lower bound above 0.
2. Share of in-store declines followed by a successful Riverty payment at the same merchant within 30 minutes (variant minus control).
Worked if: clearly higher in the variant. This shows the misery at the till was resolved, not just that she bought something later
- **Bad signal to watch for e.g. high reach, zero signups = message-market mismatch:** 1. - Control rate is already high (for example above 60%). Heavy users may buy again within 7 days whatever we show, so there is little headroom. Next step: tighten the definition to in-store card purchases only and add the same-day metric below.
- Lift is positive but under +10, or the interval is wide. Sample too small (about 48 declines at 12 a week, assumption). Next step: ITERATE or use the one pre-agreed extension. Don't call it a win.
- Lift is zero or negative. Next step: KILL, then review the notice text with the usability results before any new test.
2. - The 7-day metric rises but this one is flat. The gain comes from unrelated purchases, not from the notice. Next step: don't ship on the 7-day result alone.
- It is flat for mapped codes too. The next step or wording doesn't work. Next step: iterate the copy.
- **Most likely post-launch decision double-down · iterate · pivot · deprioritize, and what would trigger it:** MOST LIKELY POST-LAUNCH DECISION: ITERATE

Why: sample is too small to prove +10 points at day 35, so a directional read is the most probable outcome.

TRIGGERS BY DECISION (all thresholds are my proposals)

DOUBLE-DOWN (ship, roll out to 100%, extend to the detail screen, online declines or wider eligibility)
Trigger: primary metric at least +10 points over control with the 95% interval lower bound above 0, and the same-day recovery metric also clearly up, and all guardrails held (purchases per active month at or above 5.82 and no more than 0.3 below control, decline rate at or below 3.5%), 0 unsafe notices, validity checks pass.
Least likely at this volume. Also possible if real decline volume is well above 12 a week.

ITERATE (change the copy, the next-step wording, the code map or the delivery speed, then retest or use the one pre-agreed extension)
Trigger: lift positive but under +10, or at least +10 but not significant, or the sample target not reached.
Also: lift concentrated in mapped declines but weak in fallback ones (add codes to the map); notices late against the 95% within 5 seconds target (fix latency first, then rerun); testers or taps show people read the notice but don't act on the step (rewrite the step).

PIVOT (change the approach, not the wording)
Trigger: the lift is zero overall, but the same-day recovery or a segment shows a pattern pointing to a different cause. Examples: most declines are fraud, credit or unmapped so a reason can't be shown (the problem is the decline itself, which is out of scope for this PRD); the control arm already recovers most declines (no headroom, so the pain is not at the till); declines cluster at one merchant type or terminal (a merchant or processor fix, also out of scope).
Next step: take the finding back to discovery before building anything else.

DEPRIORITIZE (kill or park)
Trigger: lift zero or negative, or the interval upper bound below +5, with the sample adequate; or the volume of in-store declines is too small to ever matter (for example under about 5 a week); or a guardrail harm that can't be fixed with copy.
Action: switch the variant off, keep the decline log, revisit only if volume or the decline rate (8.7% in-store in Month 4) grows.

WHAT TO CHECK FIRST AT THE READ
1. Real weekly in-store decline volume, and whether each arm reached its target.
2. Control-arm recovery rate (is there headroom?).
3. Same-day recovery versus 7-day recovery (did the notice fix the moment at the till?).
4. Results by reason class.
5. Guardrails and validity checks.
