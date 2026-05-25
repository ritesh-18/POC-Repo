---
marp: true
theme: default
paginate: true
title: "LocalKart — ONDC-Native Hyperlocal Commerce for Tier 2/3 India"
---

# LocalKart
### The ONDC-native hyperlocal commerce stack that lets 13 million kiranas fight back.

**Investor Pitch — v1.0 (May 2026)**
*Market: India (Tier 2/3 first, then ONDC-rails to Tier 1 & Bharat)*

> Render with Marp (`marp HyperlocalCommerce-PitchDeck.md -o deck.pptx`), Reveal.js, or paste each `---`-separated block into Google Slides/Canva.

---

## 1. The 30-Second Pitch

> **We're building the operating system for India's 13 million kirana stores — discovery, ordering, delivery, inventory, and AI — riding on ONDC's open network rails. Not another dark-store Blinkit clone.**

- **Who pays:** kiranas (subscription + low commission), customers (delivery fee), brands (visibility).
- **The wedge:** Tier 2/3 India where Blinkit/Zepto are unprofitable and ONDC is already winning.
- **Why now:** ONDC hit 10M+ monthly transactions; 84% of kiranas are actively adopting digital tools; payment + identity rails are solved.

---

## 2. The Problem

### For 13 million kirana stores
- Trapped between quick-commerce platforms eating their lunch and walking customers staying loyal to "trust + credit + familiarity"
- **Zero digital visibility** — Google Maps listing at best
- **No inventory system** — running stock counts in their head
- Forced into 20–25% commissions on Swiggy / Zomato Stores or shut out entirely

### For Tier 2/3 customers
- Blinkit / Zepto / Instamart don't operate or are unreliable in their city
- BigBasket is slow; Amazon Fresh is metro-only
- They want **the local store, but with an app** — not a dark store run by strangers

### For brands & distributors
- No clean SKU-level demand data from kirana ecosystem
- Cash-and-carry / Udaan partial solutions, no consumer-side loop

---

## 3. Why Existing Solutions Fail

**Quick commerce (Blinkit, Zepto, Instamart):**
- 3 players control **~90% of QC market** — head-on competition is suicide.
- Dark store ≈ ₹50L capex, unprofitable below dense metro demand.
- They **replace** kiranas, they don't **enable** them — politically and structurally fragile in Bharat.

**Big-box e-commerce (Amazon, Flipkart):**
- Built for non-perishable, scheduled delivery — not daily fresh groceries.
- Distance from customer kills freshness and economics.

**Kirana-tech (Khatabook, Bharatpe, Udaan, Jumbotail):**
- Solve one layer (ledger, payments, B2B sourcing) — none stitch the full consumer-vendor-delivery loop.

**Plain ONDC buyer apps (Paytm, MagicPin, Mystore):**
- Generic UI, no deep kirana enablement, weak last-mile.

---

## 4. Why Now — Three Rails Just Got Built

1. **ONDC has crossed the chasm.**
   - **7 lakh+ sellers**, **1,200+ cities**, **150M+ cumulative transactions**, ~**10M transactions/month** (April 2026). 60%+ growth driven by Tier 2/3.
   - Open protocol means we don't need to onboard sellers one-by-one — they're already on-network.

2. **Kiranas are *ready*.**
   - **84% have started adopting digital tools** (up from 3% in 2018).
   - **80%** want online operations.
   - Accenture: digitized kiranas see **20–300% revenue growth, 30–400% profit growth**.

3. **Unit economics work in Tier 2/3.**
   - Lower rent (kirana = free dark store).
   - Lower rider cost.
   - QC players burning ₹50L/store building parallel infra we don't need.

---

## 5. The Solution — Three Apps, One Network

```
┌────────────────────┐    ┌────────────────────┐    ┌────────────────────┐
│  Customer App      │    │  Vendor App        │    │  Rider App         │
│  (Flutter)         │    │  (Flutter, Hindi/  │    │  (Flutter)         │
│  Browse · Order ·  │◄──►│   regional first)  │◄──►│  Pickup · Navigate │
│  Pay · Track       │    │  Catalog · Orders· │    │  · Confirm · Earn  │
└────────────────────┘    │  Stock · Ledger    │    └────────────────────┘
            ▲             └────────────────────┘             ▲
            │                       ▲                        │
            └───────────────────────┼────────────────────────┘
                                    │
                       ┌────────────▼─────────────┐
                       │  LocalKart Core (NestJS) │
                       │  Auth · Orders · Pay ·   │
                       │  AI · Geo · Notif        │
                       └────────────┬─────────────┘
                                    │
                       ┌────────────▼─────────────┐
                       │  ONDC / Beckn Adapter    │
                       │  (BAP + BPP roles)       │
                       └──────────────────────────┘
```

We are simultaneously a **BAP** (buyer-side, our consumer app discovers any ONDC seller) and a **BPP** (seller-side, our kiranas are discoverable from any ONDC buyer app).

---

## 6. Market Size

### India Quick Commerce
- **$3.65B (2026) → $12.97B by 2029** (CAGR ~23.6%)
- Top 3 (Blinkit, Instamart, Zepto) = ~90% share
- But: <100 cities deep. Tier 2/3 mostly unserved.

### Indian Retail (kirana-dominated)
- **13 million kirana stores · $800B+ annual revenue**
- Only **<5% digitally transacted today** → 95% greenfield

### Total addressable
- **TAM:** $800B (Indian retail)
- **SAM:** $120B (Tier 2/3 + edges of Tier 1 grocery + daily essentials)
- **SOM (5-yr):** ~$1.2B GMV in 30 cities → ~$60M net revenue

---

## 7. Competitive Landscape

| Player | Model | Coverage | Where they're weak |
|---|---|---|---|
| **Blinkit** | Dark stores | ~40 metro cities | Unprofitable below density; no Tier 3 |
| **Zepto** | Dark stores | ~25 cities | Burn-heavy; 25–30% contribution margin in metros only |
| **Swiggy Instamart** | Dark stores | ~100 cities, 1,100+ stores | -2.6% contribution loss; competing internally with Swiggy Food |
| **BigBasket / JioMart** | Scheduled + QC hybrid | Pan-India | Slow last-mile, weak SKU breadth in Tier 3 |
| **Dunzo / MagicPin / Paytm (ONDC BAPs)** | Aggregator | Pan-India via ONDC | No deep vendor enablement, weak retention |
| **Khatabook / Bharatpe / Udaan** | Vendor tools only | Pan-India | Don't close consumer loop |

**Our white space:** Consumer-facing + vendor-enabling + ONDC-native + Tier 2/3 first.

---

## 8. Why Incumbents Can't Copy This

1. **Strategic conflict.** Blinkit/Zepto's whole moat is dark stores. Empowering kiranas cannibalizes their model.
2. **Cost structure mismatch.** Their fixed cost per city is ~₹2–5 Cr/month. Ours is ~₹15L/month — they can't go below dense metros without breaking unit economics.
3. **Cultural distance.** Tier 2/3 vendor onboarding in vernacular is a field-sales + design discipline metro-native companies struggle with.
4. **ONDC ambivalence.** The big QC players are reluctant ONDC participants — it commoditizes them. We're ONDC-native, which **is** our product.
5. **Trust positioning.** "Local store, but better" is the opposite story from "10-minute dark-store delivery."

---

## 9. Business Model

| Stream | Pricing | Notes |
|---|---|---|
| **Vendor SaaS subscription** | ₹299–₹999/month | Catalog, orders, inventory, ledger, analytics, ONDC presence |
| **Order commission** | 2–5% (vs. 18–25% on Swiggy/Zomato) | The "we're on your side" pricing |
| **Delivery fee** | ₹15–₹40 per order | Customer pays; rider gets 70% |
| **Brand/FMCG ads** | CPM + sponsored placement | Disclosed; non-search-ranking |
| **Credit & working capital** | Partner with NBFC (Lending-as-a-Service) | Take 1–2% on disbursed loan |
| **LocalKart+ (consumer)** | ₹149/month | Free delivery, priority, family vault |

**Anti-pattern we refuse:** paid rank manipulation in search. This is the #1 complaint against incumbent aggregators.

---

## 10. AI Strategy — Five Layers Built Right

### Layer 1 — Vendor AI Copilot (Day 1 differentiator)
- "Speak in Hindi, I'll update your stock." → Voice-driven catalog & inventory.
- WhatsApp-native order taking, auto-converted into platform orders.
- Demand forecast: "Order 12 kg potatoes tomorrow — Tuesdays you sell out by 6pm."

### Layer 2 — Customer Discovery AI
- Natural language search: "atta near me under ₹250, organic"
- Multi-modal: snap a product photo → find nearest seller stocking it
- Vernacular intent mapping (Hindi, Telugu, Tamil, Bengali first)

### Layer 3 — Smart Routing & Batching
- Multi-pickup routing for riders (one ride, three stores, four drops)
- Live ETA from real GPS + traffic + historical store-prep time

### Layer 4 — Fraud & Quality
- COD fraud detection (return rate prediction at checkout)
- Anomaly detection on inventory (theft, spoilage)

### Layer 5 — Brand Insights (B2B revenue)
- SKU-level kirana demand data (anonymized) → sold to FMCG brands

> **AI principle:** every model output flows through a deterministic guardrail. We never let an LLM auto-execute a financial action.

---

## 11. Technical Architecture (High-Level)

```
[Flutter Customer]  [Flutter Vendor]  [Flutter Rider]
        \              |              /
         \             |             /
          ▼            ▼            ▼
        ─────── API Gateway (NestJS) ───────
         |        |        |        |
       Auth    Orders   Catalog   Geo
        |        |        |        |
        └────►  PostgreSQL (RDS) + PostGIS
                Redis (cache + queues, BullMQ)
                S3 (media)  ·  Pinecone (embeddings)
                ─────────────────────
                ONDC Adapter (BAP + BPP)
                Razorpay / UPI · FCM · Twilio
```

**Stack:** Flutter · NestJS · PostgreSQL + PostGIS · Redis · BullMQ · Docker · Kubernetes (EKS) · GitHub Actions · Prometheus + Grafana.

**MVP infra cost:** ₹35–60K/month (AWS, 3 microservices, single region). Scales linearly per city.

---

## 12. Go-To-Market

### Phase 1 — Pilot City (Month 0–6)
- **Pick one Tier 2 city** (e.g., Indore, Coimbatore, Vizag — high smartphone, moderate QC presence)
- Onboard **300 kiranas + 5 vegetable markets + 50 riders**
- Sub-goal: 5K MAU, 25K orders/month, ₹1.5 Cr GMV

### Phase 2 — Cluster Expansion (Month 6–18)
- 5 cities in one state (one-state focus reduces ops, legal, marketing cost)
- 5K kiranas · 100K MAU · ₹15 Cr GMV run-rate
- Plug into ONDC fully — start serving inbound buyer-app traffic

### Phase 3 — National via ONDC (Month 18–36)
- 25 cities, but most kiranas onboarded **lightly** via ONDC rails — we don't need door-to-door sales for everyone
- AI copilot + WhatsApp interface lowers onboarding cost to ~₹150/vendor

### Customer wedges
- Festival packs · monthly subscription baskets · family-account credit · UPI Lite for sub-₹100 orders

---

## 13. Unit Economics (Illustrative, Tier 2 city)

| Metric | Target |
|---|---|
| Avg order value | ₹380 |
| Take rate (commission + delivery + ads) | ₹52 (~13.7%) |
| Rider cost / order | ₹22 |
| Variable ops / order | ₹8 |
| **Contribution per order** | **₹22** |
| Orders / customer / month | 4.5 |
| Revenue / customer / month | ₹234 |
| CAC (Tier 2 blended) | ₹95 |
| Payback period | ~3 months |
| 12-month LTV | ~₹720 |
| **LTV / CAC** | **~7.5x** |

Vendor SaaS (~₹599 ARPU) adds ₹7K/year per kirana at 75% gross margin. At 5K vendors → ₹2.6 Cr ARR pure SaaS.

---

## 14. 18-Month Roadmap

| Month | Milestone |
|---|---|
| 0–2 | MVP: customer + vendor apps (Flutter), order, payment, GPS tracking |
| 2–4 | Pilot Indore: 300 kiranas, 5K MAU |
| 4–6 | ONDC BPP certification + go-live |
| 6–9 | Inventory + AI vendor copilot v1 (Hindi voice) |
| 9–12 | ONDC BAP — discover non-LocalKart sellers in our app |
| 12–18 | 5-city expansion · brand-ads product · LocalKart+ subscription |
| 18 | Series A: 1M+ MAU, ₹40 Cr ARR, 5K kiranas |

---

## 15. Defensibility

1. **Local supply graph.** Once 5K kiranas in 5 cities run their daily ops on us, that data + workflow lock-in is hard to dislodge.
2. **ONDC compliance + tooling.** BAP+BPP dual-role + certified flows take 12–18 months to replicate.
3. **Vernacular vendor UX.** A Hindi-voice catalog editor is a real engineering moat — most competitors ship English-only.
4. **Anti-positioning.** "We're the kirana's app, not the kirana's competitor" — defensible brand the QC players can't claim.
5. **Multi-sided data flywheel.** Customer demand → vendor inventory → brand insights → vendor credit → customer offers. Each strengthens the next.

---

## 16. Risks & Mitigations

| Risk | Mitigation |
|---|---|
| **Blinkit/Zepto move into Tier 2/3** | Their dark-store unit economics break below metro density; we built around their cost ceiling, not their pricing |
| **Kirana churn / weak retention** | Ledger + credit features create switching cost; commission far below alternatives |
| **ONDC slowdown or policy shift** | We're not exclusively ONDC — direct architecture works standalone; ONDC is upside, not a single point of failure |
| **Rider supply in small cities** | Hybrid model: kirana's own delivery boy as first option, gig riders as overflow |
| **Payment fraud (COD returns)** | ML fraud scoring at checkout; cap COD limits for new users |
| **Compliance: FSSAI, GST, DPDPA** | Compliance lead from Month 6; FSSAI auto-fetch into vendor onboarding |

---

## 17. Team & Hiring (Year 1)

- **Founder/CEO** — Product + GTM
- **Co-founder/CTO** — Flutter + distributed systems
- **VP Field Ops** (Month 3) — Kirana onboarding, vernacular sales
- **Head of Design** — Bilingual UX
- **Compliance Lead** (Month 6) — DPDPA + GST + FSSAI
- 6 engineers (mobile, backend, ML), 1 PM, 1 data analyst, 4 city managers by Month 12

**Advisory:** 1 ex-FMCG distribution leader · 1 ex-ONDC contributor · 1 fintech founder

---

## 18. The Ask

**Seed round: $2.5M** for 18 months runway

**Use of funds:**
- 45% Engineering & AI
- 25% Field ops & vendor onboarding (2 cities)
- 15% Customer acquisition
- 10% Compliance & licensing
- 5% G&A

**Series A milestones (Month 18):**
- 5,000 onboarded kiranas across 5 cities
- 1M+ MAU
- ₹40 Cr ARR (commission + SaaS + ads)
- 7.5x LTV/CAC sustained
- ONDC BAP+BPP certified, top-5 BPP by transaction volume

---

## 19. Why This Bet Wins

> Quick commerce won the metro. **ONDC + kirana enablement is going to win Bharat.**

- 13M kiranas. $800B GMV. 95% still offline.
- A 3-player oligopoly that *cannot* serve this market profitably.
- Open public infrastructure (UPI for payments, ONDC for commerce, ABDM for adjacent verticals) that makes the wedge possible for the first time in 2026.

We're not building "another grocery app."
We're building **the operating system of Indian retail's next decade** — and the rails happen to be already laid.

---

## 20. Appendix — Sources & Further Reading

### Quick Commerce Market
- [India Quick Commerce $12.97B by 2029 — GlobeNewswire](https://www.globenewswire.com/news-release/2026/04/20/3277255/28124/en/india-quick-commerce-report-2026-market-to-reach-12-97-billion-by-2029-blinkit-zepto-and-swiggy-instamart-lead-surge-as-jiomart-and-bigbasket-scale-competitive-entry.html)
- [Quick Commerce Market in India — Mordor Intelligence](https://www.mordorintelligence.com/industry-reports/q-commerce-industry-in-india)
- [Quick Commerce Brand Market Share — Statista](https://www.statista.com/statistics/1463659/india-quick-commerce-brands-market-share/)
- [India's Quick Commerce Key Players — India Briefing](https://www.india-briefing.com/news/quick-commerce-market-in-india-and-key-players-35348.html/)
- [Evolution of Quick Commerce — IBEF](https://www.ibef.org/research/case-study/the-evolution-of-quick-commerce-in-india-a-sectoral-analysis)

### Unit Economics
- [Blinkit FY25 GOV & Market Share — Quash](https://quashbugs.com/blog/blinkit-surpasses-zomato-in-quick-commerce)
- [Zepto Unit Economics 2025 — Zomefy](https://zomefy.com/startup-unicorn/zeptos-2025-quick-commerce-boom-unit-economics-and-path-to-10b-valuation)
- [Dark Stores Explained — Storyboard18](https://www.storyboard18.com/trending/dark-stores-explained-how-blinkit-zepto-are-building-dense-networks-for-quick-commerce-growth-95233.htm)
- [Zepto vs Blinkit vs Instamart — CIIM](https://www.ciim.in/zepto-vs-blinkit-vs-instamart-market-share-revenue-profit-a-case-study-2024-20265/)
- [India's Quick-Commerce 2025–26 — Akoi](https://www.akoi.in/blog/https-www-akoi-in-blog-india-quick-commerce/)

### ONDC / Open Network
- [ONDC Official](https://www.ondc.org/)
- [ONDC 1 Crore Monthly Transactions — HDFC Fund](https://www.hdfcfund.com/knowledge-stack/deep-dives/tuesdays-talking-points/ondc-touches-1-crore-transactions-month-upi-moment-digital-commerce)
- [ONDC Sellers & Apps 2026 — Shiprocket](https://www.shiprocket.in/blog/top-ondc-apps-in-india/)
- [What is ONDC — IBM](https://www.ibm.com/think/topics/ondc)
- [ONDC Impact on Small Retailers — IJCSRR](https://ijcsrr.org/wp-content/uploads/2025/05/25-1305-2025.pdf)
- [ONDC Retailers Guide — VasyERP](https://vasyerp.com/the-retail-guru/what-is-ondc-retailers-guide)

### Kirana Digitization
- [India's 13M Kirana Stores — CB Insights](https://www.cbinsights.com/research/kirana-store-india-retail/)
- [Kirana Digitalisation amid QC — Indian Retailer](https://www.indianretailer.com/news/kirana-stores-india-turn-digitalisation-amid-rising-quick-commerce-competition)
- [Digital Pull Revolution — Cornell Business](https://business.cornell.edu/article/2026/05/indias-digital-pull-revolution/)
- [Digitising Indian Retail — ORF](https://www.orfonline.org/research/digitising-indian-retail-analysing-challenges-and-exploring-growth-models)

---

## Speaker Notes — How to Pitch This

- **Slide 1 → 4 is the most important arc.** Set up: 13M kiranas, 90% QC oligopoly, ONDC just hit critical mass. If they don't buy "why now," nothing else matters.
- **Slide 8 ("Why incumbents can't copy"):** this is the slide investors will probe hardest. Be explicit about cost structure and strategic conflict.
- **Slide 10 (AI):** lead with **vendor copilot**, not customer chatbot. Investors are saturated on consumer AI; vendor productivity AI is differentiated.
- **Slide 13 (unit economics):** show one table. Don't over-explain. Note that contribution-positive is unusual in hyperlocal — defend the assumptions live.
- **Slide 16 (risks):** start with the Blinkit/Zepto risk — investors expect it. Owning it builds trust.
- **Always pivot back to the thesis:** "QC won metros. We're winning Bharat."
