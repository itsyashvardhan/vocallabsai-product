# Docs / API Deep-Dive, Vocallabs.ai

**Source:** `https://docs.vocallabs.ai/vocallabs` (JS-rendered SPA, captured via accessibility-tree snapshot of the live docs on 2026-05-31; the page is not fetchable as static HTML). Endpoints below are what was actually observed in the left nav and rendered panels. Not exhaustive; only what was visible is recorded, nothing invented.

## Observed API surface (left-nav sections)
`Overview` • `auth` • `wallet` • `sip` • `call` • `agents` • `Analytics` • `contacts and groups` • `Library` • `Identity` • `Dashboard` • `Campaign` • `Marketplace` • `Conference`

Environment toggle present: **"Environment: Production"** plus a "Base Environment," implying a sandbox/prod split for developers.

### Auth (observed endpoint: "Create Authentication Token")
- Request params: **`clientId`**, **`clientSecret`** (strings).
- Response: `status`, **`auth_token`**, `id`.
- Header: `Content-Type: application/json`. cURL example provided.

### Wallet (observed: "Get Wallet Balance")
- A wallet/credit-balance endpoint exists.

## Non-obvious insights a real evaluator would surface

1. **Two parallel, inconsistent identity models.** The developer API authenticates with `clientId`/`clientSecret` to an `auth_token` (standard machine-to-machine, OAuth-style), while the consumer app (app.vocallabs.ai) logs in with **phone plus OTP only**. There's also a dedicated **`Identity`** API section. Three identity surfaces with no visible unification: this is the API-side mirror of the onboarding-friction finding and a sign the developer product and the business-user product were built on different rails.

2. **Billing is wallet/credit-based per the API, yet there is NO public pricing page** (`/pricing` 404s). The `wallet` plus "Get Wallet Balance" endpoints prove a metered, prepaid-credit monetization model exists in the product, but a prospect cannot discover the rate that depletes that wallet anywhere public. For an API-native product courting self-serve developers, the price of a credit being invisible is a direct conversion blocker (reinforces teardown finding #2 with evidence from their own API).

3. **The product is far broader than the marketing site admits.** The docs expose `Campaign` (outbound campaign orchestration), `Marketplace`, `Conference` (multi-party calling), and `Library`, none of which are surfaced or explained on the homepage. The marketing site sells "infrastructure"; the API reveals a near-complete **outbound-calling CRM/campaign suite**. This is the strongest evidence for teardown finding #4 (the real product, Call Flow Builder, campaigns, marketplace, is hidden behind generic infra messaging). There is a whole **`Marketplace`** the public site never mentions: a potential distribution/collaboration asset left invisible.

4. **Developer-experience signal:** docs include "Try It Out," per-endpoint Copy buttons, cURL examples, and a production/sandbox environment switch, a credible API DX baseline. But the absence of a visible SDK quickstart or language tabs beyond cURL in the sections observed is a gap for the "SDK plus n8n plus Chrome extension" developer story.

## Caveat
Only the `auth` and `wallet` endpoint details were read in full; the `agents`, `Campaign`, `Marketplace`, `Conference`, and `Identity` sections were observed by name in the nav but their individual endpoint schemas were not exhaustively expanded. A logged-in pass should expand these and screenshot the actual Call Flow Builder UI.
