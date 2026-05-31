# Vocallabs.ai — Product Teardown

> Product Intern → PPO task. **5 sharpest feedbacks** across the product pillars, from actually using the product as a new customer.

**The one-liner:** The technology looks strong (99.9% uptime, sub-300ms, multi-model routing) — but **a brand-new user cannot actually use it.** Activation is broken before value is ever seen. So this teardown isn't a website review; I signed up, tried to build an agent and make a call, hit a wall, and *that journey* is the finding.

## 📦 Deliverables

| | What | Open it |
|---|---|---|
| 📄 **Report** | The full teardown — 5 feedbacks, Observed → Problem → Ship-instead, prioritized | **[VOCALLABS_PRODUCT_TEARDOWN.md](VOCALLABS_PRODUCT_TEARDOWN.md)** |
| 🖥️ **Deck** | Walkthrough slides (open in any browser) | **[deck/index.html](deck/index.html)** |
| 🎨 **Figures & mockups** | Activation-funnel diagram, impact/effort matrix, and **design mockups** of the proposed `/pricing` page + first-run flow | [figures/](figures/) |
| 📸 **Evidence** | Screenshots behind every observed claim | [screenshots/](screenshots/) |
| 🔬 **Research** | Competitor benchmark, collaboration theses, API findings | [research/](research/) |

## The 5 feedbacks (TL;DR)

1. 🔴 **Features / Activation** — New self-serve users hit **"Feature Locked"** on Agent Studio *and* Templates; Quick Call needs an agent that can't be created. The core loop is unreachable. *(Time-to-first-value = ∞.)*
2. 🔴 **GTM / Pricing** — `/pricing` **404s**, yet the app's Wallet shows a real **₹1 = 1 credit** model. And there are **two separate paywalls** (credits *and* "plan access") — pay ₹100 and you still can't build.
3. 🟠 **Competition** — "India-first" is **asserted but never quantified**, while Sarvam (22 langs, govt-backed), Gnani (40+/12 Indic, 30M daily calls), and Smallest (<100ms) out-gun it on paper.
4. 🟡 **UX** — Post-login is **14-item nav overload + a premature passkey nag**, not guidance — compounding the locked dead-end.
5. 🟡 **Collaborations** — A real **n8n node + Chrome extension** exist but are buried; the **India AI stack** (Bhashini/Sarvam/AI4Bharat) is unused.

## How this was produced
Logged into `app.vocallabs.ai` as a fresh account (v2.1.6) and traced the activation funnel; read `docs.vocallabs.ai` for the monetization model the site hides; benchmarked 8 competitors incl. India-native players. Every claim is screenshotted or cited — no invented numbers.

---
*Working notes / full session log live in `plan/` (not part of the submission).*
