# Vocallabs.ai, Product Teardown

> Product Intern to PPO task. **5 sharpest feedbacks** across the product pillars, from actually using the product as a new customer.

**The one-liner:** the technology looks strong (99.9% uptime, sub-300ms, multi-model routing), but **a brand-new user cannot actually use it.** Activation is broken before value is ever seen. So this teardown isn't a website review; I signed up, tried to build an agent and make a call, hit a wall, and that journey is the finding.

## Deliverables

| | What | Open it |
|---|---|---|
| Report | The full teardown: 5 feedbacks, Observed, Problem, Ship-instead, prioritized | **[VOCALLABS_PRODUCT_TEARDOWN.md](VOCALLABS_PRODUCT_TEARDOWN.md)** |
| Deck (PDF) | Submission-ready slides, one per page | **[deck/vocallabs-teardown.pdf](deck/vocallabs-teardown.pdf)** |
| Deck (live) | Same slides as an interactive HTML deck | [deck/index.html](deck/index.html) |
| Figures and mockups | Activation-funnel diagram, impact/effort matrix, and design mockups of the proposed `/pricing` page plus first-run flow | [figures/](figures/) |
| Evidence | Screenshots behind every observed claim | [screenshots/](screenshots/) |
| Research | Competitor benchmark, collaboration theses, API findings | [research/](research/) |

## The 5 feedbacks (TL;DR)

1. **Features / Activation** `[Critical]`: New self-serve users hit **"Feature Locked"** on Agent Studio and Templates; Quick Call needs an agent that can't be created. The core loop is unreachable, so time-to-first-value is infinite.
2. **GTM / Pricing** `[Critical]`: `/pricing` **404s**, yet the app's Wallet shows a real **₹1 = 1 credit** model. The lock copy implies **two separate paywalls** (credits and "plan access"), so credits alone likely won't unlock the builder.
3. **Competition** `[High]`: "India-first" is **asserted but never quantified**, while Sarvam (22 langs, govt-backed), Gnani (40+/12 Indic, 30M daily calls), and Smallest (under 100ms) out-gun it on paper.
4. **UX** `[Med]`: Post-login is **14-item nav overload plus a premature passkey nag**, not guidance, compounding the locked dead-end.
5. **Collaborations** `[Med]`: A real **n8n node plus Chrome extension** exist but are buried; the **India AI stack** (Bhashini/Sarvam/AI4Bharat) is unused.

## How this was produced
Logged into `app.vocallabs.ai` as a fresh account and traced the activation funnel; read `docs.vocallabs.ai` for the monetization model the site hides; benchmarked 8 competitors including India-native players. Every observed claim is screenshotted; competitor figures are cited; inferences (e.g., the credit-vs-plan paywall split) are labelled as such, not asserted as tested.

---
*Working notes and full session log live in `plan/` (not part of the submission).*
