# Competitor Research, Vocallabs.ai (voice AI agents)

**Date:** 2026-05-31. All figures are publicly published rates as of search date; per-minute "all-in" figures are third-party estimates (cited), not vendor list prices. Where a vendor does not publish a number, it is marked **not disclosed**.

> Note: Vocallabs publishes **no** pricing and **no** latency benchmark on its public site (verified: `vocallabs.ai/pricing` returns 404). So Vocallabs' own row below is mostly "not disclosed," which is itself a finding.

---

## Comparison table

| Platform | Positioning (own words / category) | Published price | Indian-language depth | Latency claim |
|---|---|---|---|---|
| **Vocallabs** | "Voice AI infrastructure built to scale" | **Not disclosed** (404 pricing page; wallet/credit model implied by API) | Claimed "India-first" but **not quantified** on site | "Sub-300ms" marketing claim; no benchmark |
| **Vapi** | "Build advanced voice AI agents" (dev platform) | About $0.05/min platform fee; all-in about $0.14 to $0.33/min with third-party STT/LLM/TTS | Inherits from chosen providers; not India-specialized | Not formally benchmarked publicly |
| **Retell AI** | "AI phone agents" | From **$0.07/min**, pay-as-you-go, no platform fee; enterprise to about $0.05/min; $10 free credits | Inherits from providers | Markets low-latency; no public number |
| **Bland AI** | Self-serve outbound/inbound voice | **$0.09/min** connected (plan-based); plus $0.015/outbound attempt, plus $0.02/SMS | Inherits from providers | Not disclosed |
| **Smallest.ai (Atoms/Waves)** | "Real-time Voice AI, built to scale" (India HQ) | Free, then **$49/mo**, then **$1,999/mo**, then enterprise | 30+ languages including Indic; "Lightning V2" | **Under 100ms** TTS latency claim |
| **Sarvam AI (Samvaad)** | "India's full-stack sovereign AI platform" | Not disclosed (API/usage) | **22 Indian languages** (STT), 11 for agents, 10+ TTS voices; govt-backed (GoI, Yotta, Nvidia) | "Sub-second" |
| **Gnani.ai** | "Voice AI agents for enterprises" | Enterprise-procured, custom INR, 6 to 9 month cycles | **40+ languages including 12+ Indic**; voice biometrics (Inya Shield); 30M+ daily conversations | Not disclosed |
| **Skit.ai (ex-Vernacular.ai)** | Conversational AI for **accounts receivable / collections** | Enterprise; raised about $28.1M | Indic plus global; collections-specialized | Not disclosed |
| **Twilio (Programmable Voice / ConversationRelay)** | Global CPaaS telephony plus voice AI relay | Telephony per-min plus usage; broad global rails | Telephony in 100+ countries; not Indic-tuned | Not disclosed |

---

## Where Vocallabs genuinely wins
- **Bundled full-stack plus India tuning versus global dev platforms.** Vapi/Retell/Bland are LLM-agnostic "bring-your-own-provider" platforms: cheap headline rates, but the buyer assembles STT/LLM/TTS and eats the integration plus Indic-accent quality risk. Vocallabs' "full-stack ownership" plus "India-first" is a real wedge against the global players for an Indian SMB that doesn't want to stitch Deepgram, GPT, and ElevenLabs and pray it handles Hindi-English code-mixing.
- **Distribution surface.** The n8n node, Chrome extension, and SDK (per the brief) make a wider low-code distribution footprint than most enterprise India players (Gnani/Skit are sales-led, not self-serve).

## Where Vocallabs is vulnerable
- **The "India-first" moat is contested, not owned.** Sarvam (22 Indian languages, government-backed, Nvidia/Yotta partners), Smallest.ai (30+ languages, under 100ms, India HQ), and Gnani (40+ langs, 12+ Indic, 30M daily convos, voice biometrics) all credibly claim India-first. Vocallabs' site doesn't even quantify its language coverage, so the moat is asserted, not demonstrated. **This is the single biggest competitive gap to close in the teardown.**
- **Price opacity is a disadvantage where rivals are transparent.** Retell ($0.07/min plus $10 free), Bland ($0.09/min), and Smallest ($49/$1,999) all let a buyer self-qualify in seconds. Vocallabs forces a sales conversation, fine for enterprise, fatal for the self-serve developer the SDK/n8n/Chrome-extension strategy is courting. (This directly reinforces teardown finding #2.)
- **Squeezed in the middle.** Too self-serve to win Tier-1 BFSI the way Gnani does (voice biometrics, 6 to 9 month procurement, compliance depth); not as cheap or frictionless as Retell/Bland for global indie developers. Needs a sharp ICP.

---

## Porter's Five Forces, Vocallabs in Indian voice AI

- **Rivalry: HIGH.** Crowded with both global dev platforms (Vapi/Retell/Bland) and well-funded India incumbents (Sarvam, Gnani, Skit, Smallest). Differentiation is muddy.
- **Threat of substitutes: HIGH.** Vapi/Retell are commoditizing the orchestration layer; a buyer can assemble a "good enough" Hindi agent on a global platform plus Sarvam/AI4Bharat models.
- **Supplier power: MEDIUM-HIGH.** If Vocallabs relies on third-party LLM/TTS/ASR, margins are exposed; "Bring your own models / Host your AI models" on the site suggests they're trying to internalize this (a good defensive move).
- **Buyer power: MEDIUM-HIGH.** Transparent rivals make buyers price-sensitive; enterprises run competitive bake-offs.
- **New entrants: HIGH.** Low barrier at the app layer; the durable barrier is proprietary Indic conversation data (the "data flywheel" moat) plus carrier/compliance integration. Vocallabs should lean here.

**Strategic read:** Vocallabs' defensible ground is Indic-data flywheel plus full-stack/owned-model economics plus low-code distribution, NOT generic "scalable infrastructure" (where Twilio/Vapi win) or raw price (where Retell/Bland win). The teardown should push them to prove the India moat with numbers and pick a side of the self-serve versus enterprise line.

---

## Sources
- [Vapi pricing](https://vapi.ai/pricing) • [Synthflow: Vapi pricing 2025](https://synthflow.ai/blog/vapi-ai-pricing) • [CloudTalk: Vapi pricing](https://www.cloudtalk.io/blog/vapi-ai-pricing/) • [Telnyx: VAPI pricing](https://telnyx.com/resources/vapi-pricing)
- [Retell AI pricing](https://www.retellai.com/pricing) • [Retell pricing comparison 2025](https://www.retellai.com/resources/voice-ai-platform-pricing-comparison-2025)
- [Bland AI pricing](https://www.bland.ai/pricing) • [Bland billing docs](https://docs.bland.ai/platform/billing) • [Zeeg: Bland pricing](https://zeeg.me/en/blog/post/bland-ai-pricing)
- [Smallest.ai pricing](https://smallest.ai/pricing) • [Smallest.ai home](https://smallest.ai/) • [Atoms docs](https://atoms-docs.smallest.ai/)
- [Sarvam conversational agents](https://www.sarvam.ai/products/conversational-agents) • [Sarvam home](https://www.sarvam.ai/) • [Sarvam STT API](https://www.sarvam.ai/apis/speech-to-text)
- [Gnani.ai home](https://www.gnani.ai/) • [Gnani AI voice agent](https://gnani.ai/ai-voice-agent) • [Gnani Crunchbase](https://www.crunchbase.com/organization/gnani-ai)
- [Skit / Vernacular.ai (CB Insights)](https://www.cbinsights.com/company/vernacularai)
