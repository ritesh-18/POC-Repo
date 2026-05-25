---
marp: true
theme: default
paginate: true
title: "MedFinder — Unified Healthcare Discovery Platform"
---

# MedFinder
### One search. Every doctor, clinic, lab, and pharmacy. Across networks.

**Investor Pitch — v1.0 (May 2026)**

*Markets: India + United States*

> Tip: render this deck with Marp (`marp HealthcarePlatform-PitchDeck.md`), Reveal.js (`reveal-md`), Slidev, or paste each `---`-separated section into a Google Slides / PowerPoint slide.

---

## 1. The Problem We're Solving

**Finding the right care is fragmented, opaque, and slow — in both India and the USA.**

- Patients juggle **5+ apps** to do one care journey: search a doctor, book a slot, order a prescription, schedule a lab test, follow up.
- Each network is a walled garden — Apollo's app doesn't show Fortis doctors; Zocdoc doesn't tell you a cheaper pharmacy for the prescription you just got.
- Listings are biased by **paid placement**, not clinical fit or price.
- Reviews are gameable; pricing is hidden until checkout; insurance coverage is unclear.
- Health records live in **silos** — every new provider starts from scratch.

> "The same patient is invisible to themselves across the system."

---

## 2. Why Now — Three Tailwinds Converging in 2026

1. **Infrastructure is finally open.**
   - 🇮🇳 ABDM: 848M ABHA IDs created, 827M health records linked, 451K facilities, 761K professionals on a UPI-style open network (UHI).
   - 🇺🇸 21st Century Cures Act + FHIR/USCDI mandates force payers and providers to expose APIs.

2. **AI crossed the usability threshold.**
   - Multimodal GenAI (text + image + vitals) now feasible at consumer scale.
   - 2026 = year of *implementation*, not pilots (per industry analysts).

3. **Consumer behavior shifted permanently post-COVID.**
   - India projects **600M e-health users by 2026**.
   - 33 US states have telehealth payment parity laws — insurer reimbursement on par with in-person.

---

## 3. The Solution — MedFinder

**One search bar. Cross-network. Price-transparent. AI-guided. Record-portable.**

A consumer healthcare super-app that:
1. **Aggregates** doctors, clinics, labs, and pharmacies across competing networks into one searchable index.
2. **Triages** the user with an AI symptom checker before they pick a provider.
3. **Compares** price, distance, wait time, and insurance acceptance side-by-side.
4. **Books, pays, and unifies** records under one ABHA / patient ID — portable across providers.
5. **Closes the loop** — refills, lab follow-ups, second opinions, all surfaced proactively.

*Think Skyscanner × Truecaller × ChatGPT, but for healthcare.*

---

## 4. Market Size — Global & Regional

### Global Virtual Healthcare Platforms
- $10.7B (2025) → **$34.9B by 2033**, CAGR 15.8%

### 🇮🇳 India Digital Health
- $19.1B (2025) → **~$107B by 2033**, CAGR ~25%
- Online pharmacy alone: $3.71B → **$14.1B by 2034** (CAGR 16%)
- 600M projected e-health users by 2026

### 🇺🇸 USA Digital Health
- **$98.7B (2026)** → $238.7B by 2034, CAGR 11.67%
- US telehealth: $42.6B (2024) → **$359B by 2034**, CAGR 23.84%
- Telehealth = 35% of US digital health share (2024)

---

## 5. TAM / SAM / SOM

| Layer | India | USA |
|---|---|---|
| **TAM** (total digital health) | $107B by 2033 | $239B by 2034 |
| **SAM** (search + booking + e-pharmacy + diagnostics aggregation) | ~$25B by 2030 | ~$45B by 2030 |
| **SOM** (5-yr realistic capture, ~1.5% of SAM) | **~$370M ARR** | **~$675M ARR** |

> Even a 1% sliver of the aggregator layer in either geography is a unicorn-scale outcome.

---

## 6. Competitive Landscape — 🇮🇳 India

| Player | Core Strength | Key Gap |
|---|---|---|
| **Practo** | Doctor discovery, 100K+ providers, telecons | Single-network bias, weak pharmacy/lab loop, paid-rank reviews |
| **Tata 1mg** | E-pharmacy + diagnostics, Tata brand trust | Doctor search is thin; locked to 1mg labs |
| **PharmEasy** | Pharmacy + diagnostics scale, post-funding crunch | No real discovery layer, post-Thyrocare integration friction |
| **Apollo 24/7** | Apollo hospital network + pharmacy | Locked to Apollo ecosystem — by design |
| **MediBuddy / MFine** | Corporate insurance tie-ins | B2B2C, weak direct consumer brand |
| **Netmeds (Reliance)** | Reliance distribution muscle | Pharmacy-first, no cross-network discovery |

**The gap:** No player is *network-neutral* — each one optimizes for their own clinic/pharmacy/lab.

---

## 7. Competitive Landscape — 🇺🇸 USA

| Player | Core Strength | Key Gap |
|---|---|---|
| **Zocdoc** | Doctor booking ($1.8B val, $3K/yr provider subscription, 30% CAGR) | No pharmacy/lab; doctor-only; subscription tilts supply-side |
| **Healthgrades** | Reviews + ratings depth | Discovery-only; no booking/transactions; ad-funded |
| **GoodRx** | Pharmacy price transparency, mass consumer brand | Pharmacy-only; doctor search is afterthought |
| **Teladoc / Amwell / MDLIVE** | Telehealth scale, payer contracts | Virtual-only; competes *with* providers, not for them |
| **Capsule** | Pharmacy delivery in major metros | Geo-limited, single vertical |
| **HealthTap, Doctor on Demand** | Virtual visits | Closed-network, narrow vertical |

**Top 4 (Amwell, Teladoc, CVS, UnitedHealth) hold ~40% of US virtual care.** But none of them solve *cross-network discovery* — they ARE the networks.

---

## 8. Why Existing Players Can't Pivot Here

- **Strategic conflict.** Apollo 24/7 will never surface Fortis doctors. Zocdoc's revenue comes from providers paying $3K/year — they can't list non-paying competitors fairly.
- **Vertical lock-in.** GoodRx is a pharmacy ad business. Zocdoc is a booking SaaS. 1mg's economics are pharmacy-margin-driven. Cross-network discovery cannibalizes their cash cow.
- **Trust deficit.** Aggressive upselling, paid-placement listings, and opaque pricing have eroded user trust in incumbents (multiple regulatory complaints in India press in 2024–25).
- **No unified record.** Even within a single app, lab results don't talk to prescriptions.

**An independent, network-neutral, AI-native, records-portable platform is structurally hard for incumbents to build.**

---

## 9. Product — Core User Journeys

1. **Search & Compare** — "I have lower back pain, near 110001, covered by Star Health."
   → Doctors + clinics ranked by *clinical fit × price × distance × in-network insurance × real wait time*.

2. **Triage First** — Optional AI symptom checker before search narrows specialty and urgency (GP vs. ortho vs. ER).

3. **Book + Pay + Records** — Single checkout. Receipt, prescription, and consultation notes auto-attach to the user's ABHA / unified profile.

4. **Lab + Pharmacy in One Flow** — Prescribed a test? We surface 3 nearest labs with prices side-by-side. Prescribed a medicine? Cheapest verified pharmacy delivery, no separate app.

5. **Care Continuity** — Refill nudges, lab follow-up reminders, second-opinion suggestions for high-stakes diagnoses.

---

## 10. AI Strategy — Three Layers, Defensible Over Time

### Layer 1 — Discovery AI (Day-1 differentiator)
- Natural-language search ("a female gynecologist near me, Hindi-speaking, evening slots")
- Semantic specialty mapping (symptom → specialty → provider sub-niche)
- Personalized ranking that learns from outcomes, not clicks

### Layer 2 — Triage & Symptom Assessment AI
- Multimodal symptom checker (text + photo of skin/eye + uploaded report)
- Routes user to right care level: self-care, GP teleconsult, in-person specialist, ER
- Calibrated for *safety over engagement* — explicitly de-risked from over-diagnosis

### Layer 3 — Longitudinal Health Copilot
- "Summarize my health in 60 seconds" from records
- Drug interaction & duplicate-test detection across providers
- Proactive nudges: "Your last HbA1c was 6.7 — due for a recheck."

---

## 11. AI — Concrete Models & Build Plan

| Capability | Approach | Build vs Buy |
|---|---|---|
| Symptom checker | Fine-tuned LLM + clinical guideline RAG + human-in-loop review | Buy base model (Claude/GPT), build clinical RAG layer |
| Provider ranking | Learning-to-rank on engagement + verified outcomes | Build (proprietary data moat) |
| Voice search (vernacular) | Speech-to-text in 10+ Indian languages | Buy (Sarvam/Bhashini/Whisper), wrap with healthcare ontology |
| Records summarization | LLM with FHIR-structured input | Buy + heavy guardrails |
| Drug interaction check | Rule-based + LLM cross-check | Hybrid — never LLM-only for safety-critical |

> **AI safety stance:** Every clinical output is labeled as decision-support, never diagnosis. Red-team protocol + clinician advisory board from Day 1. This is also a moat — incumbents move slowly here.

---

## 12. Business Model — Multi-Sided, Trust-Aligned

| Revenue stream | Pricing | Why it doesn't compromise trust |
|---|---|---|
| **Pharmacy commission** | 8–12% on fulfilled orders | Multiple pharmacies bid → user gets cheaper, we still earn |
| **Lab commission** | 10–15% on bookings | Same dynamic |
| **Provider subscription** (optional) | ₹15K–₹50K / $999–$3K per year for *tools* (calendar, EMR-lite, no-show reduction) — **never for ranking** | Ranking stays merit-based |
| **Insurance partner referrals** | Per-qualified-lead fee | Disclosed in UI |
| **Premium consumer (MedFinder+)** | ₹299/mo or $9.99/mo: AI copilot, family records, priority slots | Aligned — users pay us, not providers |

**Anti-pattern we refuse:** Paid placement in search results. This is the single biggest complaint against incumbents.

---

## 13. Go-to-Market

### Phase 1 (Months 0–9) — One city, one vertical, India first
- **Bengaluru + Hyderabad**, doctor discovery + teleconsult only.
- Seed supply via direct outreach to 2K independent clinics outside large hospital chains.
- Demand via paid social + SEO on long-tail symptom queries.

### Phase 2 (Months 9–18) — Add labs, pharmacy; expand to top-10 Indian metros
- Integrate with ABDM/UHI from Day 1 — instant provider onboarding via open network.

### Phase 3 (Months 18–30) — US launch, NYC + Bay Area
- Different wedge: **price transparency** (post–No Surprises Act + Hospital Price Transparency rule). US users hate surprise bills more than they hate fragmentation.

### Why India first?
- Lower CAC, faster integration via open ABDM rails, willingness-to-pay for convenience proven.
- US is the monetization market; India is the *learning + AI training data* market.

---

## 14. 18-Month Roadmap & MVP Scope

**MVP (Month 0–4):**
- Doctor + clinic search (Bengaluru), filters, profile pages with verified credentials
- Booking + payment + post-visit notes upload
- AI symptom checker (v1, conservative — always routes to a human)

**v1 (Month 4–9):**
- Lab booking + price compare
- E-pharmacy with delivery partners
- ABHA-linked health records vault

**v2 (Month 9–18):**
- AI health copilot (records summarization, refill nudges, drug interaction)
- Insurance verification in-flow
- Multi-language voice search
- US pilot launch

---

## 15. Defensibility — Why This Won't Get Crushed

1. **Network neutrality is a strategic position, not a feature.** Incumbents can't copy without cannibalizing.
2. **Data flywheel.** Each booking + outcome strengthens ranking and AI triage — compounding.
3. **Records portability lock-in.** Once a user's 5-year history lives with us, switching cost is high.
4. **Open-network integration depth.** Deep ABDM/UHI + FHIR plumbing takes 18–24 months to replicate.
5. **AI safety reputation.** Built carefully early = trust premium incumbents will struggle to match after one bad headline.

---

## 16. Unit Economics (Illustrative — India)

| Metric | Target |
|---|---|
| CAC (blended, paid + organic) | ₹180 |
| Average bookings/user/year | 4.5 |
| Take rate per booking (blended) | ₹95 |
| Annual revenue / user | ₹427 |
| Gross margin | ~62% |
| **Payback period** | ~8 months |
| LTV (3-yr horizon, 70% retention) | ~₹900 |
| **LTV/CAC** | **~5.0x** |

Premium subscription (~10% conversion @ ₹299/mo) pushes ARPU to ₹770 and LTV/CAC to ~8x.

---

## 17. Risks & Mitigations

| Risk | Mitigation |
|---|---|
| **Regulatory** (DPDPA in India, HIPAA in US) | Privacy-by-design, on-shore storage, ISO 27001 + HITRUST from Year 1 |
| **Clinical liability** from AI | Decision-support framing only, clinician advisory board, malpractice insurance |
| **Supply-side cold start** (doctors won't join) | Open-network rails (ABDM/UHI) let us list without explicit onboarding for India; for US, start with independent practices ignored by Zocdoc |
| **Incumbent retaliation** | We're a B2C aggregator they refer patients *from*; we partner where possible |
| **Trust erosion** if a missed diagnosis goes public | Conservative triage, transparent disclaimers, fast escalation paths |
| **Insurance API gaps** (US) | Start price-transparent for cash-pay; layer insurance verification as it stabilizes |

---

## 18. Team & Hiring Plan (Year 1)

- **Founder/CEO** — Product + healthtech
- **Co-founder/CTO** — AI/ML + distributed systems
- **Clinical Advisor** (Day 1) — Practicing MD with EMR/digital health experience
- **Head of Design** — Healthcare UX is its own discipline
- **Compliance Lead** (Month 6) — DPDPA + HIPAA dual-jurisdiction
- 8–10 engineers (ML, mobile, backend), 2 PMs, 3 ops, 2 growth, by Month 12

---

## 19. The Ask

**Seed round: $3.5M** for 18 months of runway to:
- Ship MVP + reach 250K MAU in two Indian metros
- Hit ₹4 Cr annualized run-rate by Month 18
- Build ABDM-native technical moat
- De-risk AI triage with 10K+ human-reviewed sessions

**Use of funds:** 55% engineering & AI · 20% growth & supply · 15% compliance & clinical · 10% G&A

**Milestones for Series A (Month 18):**
- 1M MAU, ₹15 Cr ARR
- LTV/CAC > 4x sustained
- ABDM integration as a quoted reference design

---

## 20. Appendix — Sources & Further Reading

### Market Size
- [India Digital Health Market — Custom Market Insights](https://www.custommarketinsights.com/report/india-digital-health-market/)
- [India Digital Health Market to reach USD 84B — Medical Buyer](https://medicalbuyer.co.in/india-digital-health-market-to-reach-usd-84076-5m/)
- [India Online Pharmacy Market — IMARC](https://www.imarcgroup.com/india-online-pharmacy-market)
- [U.S. Digital Health Market — Towards Healthcare](https://www.towardshealthcare.com/insights/us-digital-health-market-sizing)
- [Telehealth Market — Market.us](https://market.us/report/telemedicine-market)
- [U.S. Virtual Care Market — Global Market Insights](https://www.gminsights.com/industry-analysis/us-virtual-care-market)

### Competitors
- [Tata 1mg's Journey — Inc42](https://inc42.com/features/tata-1mg-journey-classifieds-full-stack-healthcare-ecosystem/)
- [Top 10 Medicine Delivery Apps — Shiprocket](https://www.shiprocket.in/blog/instant-medicine-delivery-apps/)
- [Zocdoc Business Model — Daffodil](https://insights.daffodilsw.com/blog/how-zocdoc-works-business-model-and-revenue-streams)
- [Zocdoc $1.8B Profitability Story — Inc.com](https://www.inc.com/annabel-burba/this-strategy-nearly-killed-zocdoc-how-it-recovered-and-became-a-1-8-billion-business/91210543)
- [Zocdoc vs Healthgrades — 6sense](https://6sense.com/tech/other-healthcare-tech/zocdoc-vs-healthgrades)
- [Zocdoc Alternatives 2025 — RightPatient](https://www.rightpatient.com/guest-blog-posts/top-15-zocdoc-alternatives-for-healthcare-providers-in-2025-complete-comparison-guide/)

### Infrastructure (ABDM / UHI / Open Networks)
- [ABDM Official — National Health Authority](https://abdm.gov.in/)
- [ABDM Three-Year Journey — Ministry of Health](https://www.mohfw.gov.in/?q=en/pressrelease-87)
- [ABDM Adoption Study — PMC/NIH](https://pmc.ncbi.nlm.nih.gov/articles/PMC13078079/)
- [India unveils digital health aggregator (UHI) — Healthcare IT News](https://www.healthcareitnews.com/news/asia/india-unveils-digital-health-aggregator-platform)

### AI in Healthcare
- [AI better than doctors at diagnosis (study) — NPR](https://www.npr.org/2026/04/30/nx-s1-5804474/ai-doctors-openai-patient-care-diagnosis)
- [GenAI Healthcare Use Cases — John Snow Labs](https://www.johnsnowlabs.com/generative-ai-healthcare/)
- [25 Healthcare AI Use Cases — AIMultiple](https://research.aimultiple.com/healthcare-ai-use-cases/)
- [Build AI Symptom Checker — Appinventiv](https://appinventiv.com/blog/build-ai-symptom-checker-app/)
- [GenAI Patient Engagement — TechTarget](https://www.techtarget.com/patientengagement/feature/Promising-patient-engagement-use-cases-for-GenAI-chatbots)

### Pain Points & Trust Issues
- [Online Health Aggregators public health risk — National Herald](https://www.nationalheraldindia.com/india/unregulated-operations-by-unscrupulous-online-health-service-aggregators-pose-grave-risk-to-public-health)
- [Doctor Aggregator Website Mistakes — Medium](https://medium.com/@rajeshtn07/3-most-common-mistakes-of-medical-doctors-aggregator-websites-5d186d281e77)
- [Health Data Aggregator Challenges — Technology Rivers](https://technologyrivers.com/blog/how-to-build-a-health-data-aggregator-app-challenges-and-best-practices/)

---

## Speaker Notes (Quick Reference)

- **Lead with the user pain**, not the tech. Open by asking the room: "When was the last time you booked a doctor, ordered the prescription, and got the lab test in one app — and trusted the ranking?"
- **Slides 4–5 are the "is this market big enough" gate.** Don't rush. Quote two independent sources per number.
- **Slide 8** ("why incumbents can't pivot") is the single most important slide for an investor. Make sure to explicitly name the *strategic conflict*.
- **Slide 10–11 (AI)**: emphasize *safety as moat*, not novelty. Investors have AI fatigue; differentiation comes from clinical guardrails.
- **Slide 12 (business model)**: deliberately call out the *anti-pattern* (no paid ranking) — it signals integrity and a long-term thesis.
- **Slide 17 (risks)**: never skip. Showing you've thought about regulation and liability is the #1 trust signal for healthtech investors.
