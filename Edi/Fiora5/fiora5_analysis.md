# FIORA5 — V7 Capital Investment Analysis

> **Date:** 18.02.2026
> **Analyst:** VS Code / Robert Framework
> **Prompts used:** FM #4 (Comps), FM #7 (IC Memo), MC #1 (TAM), MC #2 (Competitive Landscape), MC #4 (Industry Trends), MC #5 (SWOT + Porter's Five Forces), MC #9 (Unit Economics), MC #10 (Risk Assessment), MC #12 (Executive Synthesis)
> **Prompts skipped:** FM #1 (DCF — pre-revenue), FM #2 (Three-Statement — pre-revenue), FM #3 (LBO — VC equity deal), FM #5 (Credit — no debt), MC #3 (Customer Personas — B2B enterprise, single decision-maker type), MC #7 (GTM — insufficient data), MC #8 (Customer Journey — B2B complex sale, insufficient data), MC #11 (Market Entry — not primary question)

---

## 1. EXECUTIVE SUMMARY

Fiora5 is a Romanian deep-tech startup building proprietary CPU intellectual property (IP) on the RISC-V open-source architecture, targeting ultra-low power applications in wearables, edge AI devices, and explicitly — defense/aerospace systems. The core technical claim is a ~50% power reduction versus ARM Cortex-M equivalents. The company is pre-revenue, pre-MVP, at demo stage, with a team of four (CEO, CTO, VP Software/PhD, Strategic Advisor). They are raising €500K at an implied cap of €8M (SAFE per deck; CLA with 8M cap + 20% discount per Edi's meeting notes — discrepancy unresolved).

**The investment case has three structural problems for V7 Capital specifically.** First, Fiora5 explicitly targets defense contractors (Lockheed Martin, BAE Systems, Rheinmetall) as primary customers — a direct conflict with V7's SHA weapons restriction. Second, the €8M cap is priced for a post-MVP company, not a demo: comparable European RISC-V IP startups raised at €3–6M caps pre-product, making this 2–3× overpriced for stage. Third, the time-to-exit in semiconductor IP is structurally 10–15 years (Arteris: 2003→2021; Codasip: 2014→still private), incompatible with any realistic NAV event for V7's investors.

**Recommendation: PASS.** Fiora5 may be an interesting opportunity for a specialized deep-tech fund (NATO-aligned defense fund, EU Chips Act grant recipient, or a strategic corporate venture arm). It is not the right deal for V7 Capital at this stage, at this price, or given the SHA constraints.

---

## 2. ANALYSIS BY PILLAR

### 2.1 Founders — Score: 6.5/10

*Informed by: FM #7 (IC Memo — Founders section), V7 parameters F1–F12*

| Parameter | Score | Evidence |
|-----------|:-----:|---------|
| **F1 — Technical competence** | 9/10 | Petru: 10+ years semiconductor IP (rare globally). Ciprian: EPFL PhD + ex-iNoCs (acquired by Arteris — a verified exit). Combined, arguably the strongest technical duo a Romanian startup could assemble in this domain |
| **F2 — Track record / 0→1** | 5/10 | Ciprian has an exit (iNoCs→Arteris). But iNoCs was academic spinout in Switzerland, not a commercial 0→1 venture in CEE. Darian (CEO) — zero verifiable commercial track record in semiconductor sales or enterprise BD |
| **F3 — Integrity** | n/a | No red flags. No reference checks available. Cannot score |
| **F4 — Authenticity** | 6/10 | Tone in Edi's meeting is honest about difficulty. No overselling of traction |
| **F5 — Learning velocity** | 7/10 | EPFL PhD + 10-year domain expert = technical learning capacity very high. Commercial learning = unknown |
| **F6 — Realism** | 4/10 | "6 months FPGA MVP, 18 months final product" — optimistic by 2–3× for hardware IP. TRL claim of 4–5 likely 3–4. Cap 8M at demo stage = disconnected from comparable benchmarks |
| **F7 — Culture / team** | n/a | Insufficient data |
| **F8 — Resilience** | 6/10 | Staying in semiconductor IP (one of the hardest possible domains) implies resilience. No evidence of crisis navigation |
| **F9 — Vision** | 7/10 | Low-power edge computing thesis is coherent and well-timed. Defense addition to the vision is strategically opportunistic but SHA-problematic |
| **F10 — Talent attraction** | 3/10 | Romania has no semiconductor IP hub. Hiring Petru equivalents is a global talent problem. No evidence of pipeline |
| **F11 — Skin in the game** | 6/10 | Presumed full-time. No data on personal capital invested or equity distribution |
| **F12 — Complementarity** | 6/10 | Strong on technical (CTO + VP Soft). Weak on commercial execution. Darian's ability to navigate 18–36 month B2B enterprise sales cycles in semiconductor = unproven |

**Key founder asset:** Ciprian's exit (iNoCs → Arteris) is the single most valuable signal. Arteris is a public company ($200M+ market cap) that licenses NoC (Network-on-Chip) IP — directly comparable domain to Fiora5's ambition. He knows how processor IP gets commercialized.

**Key founder risk:** The CEO role in semiconductor IP licensing requires building relationships at the VP Engineering / CTO level at companies like Qualcomm, NXP, or Rheinmetall over 2–3 years before a purchase order. There is no evidence Darian has this network or has done this before.

**Impact on asymmetry:**
- P(win) contribution: **Moderate-positive.** Technical depth is genuine. Commercial execution capacity = biggest unknown.

---

### 2.2 Company / Business Model — Score: 3/10

*Informed by: MC #9 (Unit Economics), FM #7 (IC Memo — Company section), V7 parameters C1–C16*

**Business model:** Fiora5 is a pure IP licensor. Revenue comes from two sources: (1) one-time licensing fees paid when a customer adopts the IP for their SoC design, and (2) royalties per chip shipped, paid annually. This is how Arm, MIPS, Codasip, and Arteris operate.

#### Target Unit Economics (Pre-Revenue — Modeled)

| Metric | Target | Assumption | Risk |
|--------|--------|-----------|------|
| **One-time license fee** | €100K–€500K | Low end (startup discount); Arm Cortex-M licenses at $1–5M | They will undercut to win first customers |
| **Royalty per chip** | €0.01–€1.00 | Wide range; wearables = low vol, high royalty; IoT = high vol, low royalty | Volume forecasting impossible pre-design win |
| **Sales cycle** | 12–36 months | Industry standard for semiconductor IP adoption | First design win = minimum 18 months after IP is proven |
| **Gross margin at scale** | 80–90% | IP business = near-zero COGS per license | Only achievable post-R&D recovery |
| **CAC analog** | €100–250K | FTE sales + FAE + conference + travel per customer | Requires dedicated BizDev hire immediately |
| **LTV per customer** | €1.0–2.5M | License + 5-year royalty stream (1M chips × €0.20/yr) | Assumes they actually win chip design |
| **LTV:CAC** | 5–15x | Target range (at scale) | Cannot be validated — zero customers |
| **Break-even** | Year 4–5 | At €1–1.5M ARR | Requires 3–5 paying customers with royalty ramp |

**Revenue projection (Base Case — if no SHA block):**

| Year | Event | Revenue |
|------|-------|---------|
| 2026 | FPGA MVP demo → first prospect conversations | €0 |
| 2027 | IP tape-out → 1 LOI, no payments yet | €0 |
| 2028 | First license deal closed | €150K one-time |
| 2029 | 2nd license + royalties from deal 1 | €350K |
| 2030 | 3 customers, royalty ramp | €800K |

**Burn rate and runway:**
- Team (4 FTE + 2 hires needed): €700K–1.0M/year
- Tools (Synopsys/Cadence full commercial): €150–300K/year (they currently have €10K/yr non-commercial — this scales dramatically)
- €500K raise = **5–7 months runway at minimum viable burn.** Severely insufficient. Immediate follow-on needed.

**Margin of Safety: ZERO.**
The company does not generate revenue, has no recurring contracts, and cannot survive without continuous external capital. There is no floor.

**Impact on asymmetry:**
- P(win) contribution: **Negative.** No validation of any commercial claim. Business model is correct (IP licensing works), but the path from demo to first paying customer is 2+ years and capital-intensive.
- R (return) contribution: **Neutral-positive.** IP business at scale has exceptional economics. But "at scale" is 7–10 years away.

---

### 2.3 Industry — Score: 5.5/10

*Informed by: MC #1 (TAM), MC #2 (Competitive Landscape), MC #4 (Industry Trends), MC #5 (SWOT + Porter's Five Forces)*

#### Market Sizing (MC #1)

**Top-down approach:**

| Layer | Size | Notes |
|-------|:----:|-------|
| Global Semiconductor IP market (2024) | $8.5B | All IP types — CPU, GPU, NoC, memory controllers |
| Processor / CPU IP segment | ~$5.0B | ARM ~$2.5B, rest split across MIPS, RISC-V, others |
| RISC-V commercial IP | ~$600M (est.) | Codasip, SiFive, Andes, Nuclei + Arm competitive response |
| Low-power RISC-V (Fiora5's target) | ~$150–200M | Ultra-low power sub-segment (wearables, IoT, edge AI) |

**CAGR projections:**
- Global semiconductor IP market: +9% CAGR (2024–2029)
- RISC-V commercial market: +25–30% CAGR (2024–2028), driven by EU/India mandates, US CHIPS Act diversification, and ARM IPO premium creating cost pressure
- Low-power edge AI: +35% CAGR (2024–2028)

**Bottom-up approach (Wearables segment):**
- Global wearable devices shipped (2024): ~600M units
- Wearables using custom SoC with licensed CPU IP: ~15–20% = 90–120M units
- If Fiora5 captures 0.1% market share in 5 years (realistic): ~90–120K chips/year
- At €0.30 royalty/chip: €27–36K/year — too small to matter
- Needs **1%+ market share** to generate meaningful royalties: €270–360K/year

**Bottom-up approach (Defense/Aerospace):**
- Global defense electronics IP licensing: ~$500M/year (estimated, not public)
- Contracts: 2–3 license deals at €300–500K each = €600K–1.5M/year
- But: SHA conflict blocks this segment for V7

**TAM verdict:** The addressable market is real and growing. However, Fiora5's realistic SOM in a 5-year horizon (wearables only, no defense) is €500K–2M ARR — small enough that the company's strategic value is primarily as an acquisition target, not a standalone business.

---

#### Competitive Landscape (MC #2)

| Player | Market Share | Revenue | Funding | Threat to Fiora5 |
|--------|:---:|:---:|:---:|:---:|
| **ARM Holdings** | ~90% (embedded) | $2.5B | Public (NASDAQ: ARM) | 🔴 CRITICAL |
| **SiFive** (USA) | ~5% (RISC-V) | ~$100M est. | $175M+ raised | 🔴 HIGH |
| **Codasip** (CZ/DE) | ~2–3% (RISC-V) | ~$30M est. | $25M Series A | 🔴 HIGH |
| **Andes Technology** (Taiwan) | ~1–2% | ~$30M | Public (Taiwan) | 🟡 MED |
| **Nuclei System** (China) | ~1% | unknown | Chinese gov't backed | 🟡 MED (China market) |
| **MIPS/Imagination** (UK) | <1% | declining | Private equity owned | 🟡 LOW-MED |
| **Arm Cortex-M0+** (free) | dominant low-power | embedded in Arm fee | — | 🔴 FREE ALTERNATIVE |

**Fiora5's claimed white space:** Ultra-low power RISC-V CPU IP with demonstrated 50% power reduction vs. ARM Cortex-M. If proven, this is a real gap — ARM's Cortex-M family hasn't had fundamental efficiency architecture rethink since M0+. SiFive focuses on high-performance, Codasip on automotive. The low-power wearables/edge-AI segment is underserved by serious commercial players.

**White space assessment:** Potentially real, but verification requires independent benchmarking. Founders' claims cannot be relied on without third-party silicon validation.

**Competitive moat analysis:**
- Fiora5 has: IP uniqueness (if 50% claim holds) + first-mover in sub-segment
- Fiora5 lacks: Ecosystem (toolchain, OS ports, reference designs), customer references, EDA tool certification, certification for safety-critical uses (ISO 26262, DO-178C)
- ARM's moat is 30 years of ecosystem lock-in — not power efficiency — so a genuine efficiency breakthrough does not need to beat ARM's ecosystem to find customers. It needs to find 3–5 early adopters willing to take ecosystem risk.

---

#### Industry Trends (MC #4)

| Trend | Impact | Timeline | Impact Rating (1–10) |
|-------|--------|:--------:|:--------------------:|
| RISC-V global adoption acceleration (India RISC-V mandate, EU CHIPS Act, US DoD diversification away from ARM) | Tailwind | 1–3 yr | 9 |
| Edge AI proliferation → ultra-low power compute demand explodes (inference at sensor level) | Strong tailwind | 1–2 yr | 8 |
| ARM IPO (2023) → higher licensing costs push OEMs to evaluate alternatives | Tailwind | ongoing | 7 |
| CHIPS Act subsidies (US/EU) for semiconductor startups including IP | Potential non-dilutive capital for Fiora5 | 1–3 yr | 6 |
| Wearables market slowdown (2023-2024 weak demand) | Headwind near-term | 0–1 yr | -5 |
| China-Taiwan geopolitical risk → demand for Western-sourced CPU IP | Tailwind (long-term) | 3–5 yr | 7 |
| ARM pricing increase post-IPO creates pricing pressure | Tailwind | ongoing | 6 |
| VC funding contraction in deep tech (2023–2025) | Headwind for follow-on raises | 0–2 yr | -6 |

**"So what" for Fiora5:**
The macro trend is genuinely favorable. RISC-V is having its moment. The EU CHIPS Act and similar programs provide grant capital pathways that Fiora5 should be pursuing aggressively (non-dilutive) before raising venture capital. The timing on wearables is harder short-term (softening demand 2023-2024), but the edge AI thesis supersedes wearables specifically.

---

#### SWOT + Porter's Five Forces (MC #5)

**SWOT:**

| | Strengths | Weaknesses |
|--|-----------|-----------|
| **Internal** | 1. Ciprian's exit (iNoCs→Arteris): domain credibility<br>2. Petru's 10+ years: rare technical depth<br>3. Proprietary architecture: no open-source encumbrance<br>4. RISC-V ISA: no royalty to pay upstream<br>5. Genuine market timing (edge AI tailwind)<br>6. IP business model: 80-90% gross margins at scale | 1. Zero revenue, zero clients, zero MVP<br>2. CEO commercial track record = unproven<br>3. Romania: no semiconductor talent pool<br>4. €500K raise = 5-7 months runway only<br>5. Cap 8M = overpriced for demo stage<br>6. Defense targeting = SHA conflict (for V7 specifically)<br>7. 50% power claim = unverified externally |
| **External** | **Opportunities** | **Threats** |
| | 1. EU CHIPS Act grants (non-dilutive capital pathway)<br>2. ARM post-IPO pricing increases alienating OEMs<br>3. Edge AI inference creating new demand for ultra-low power CPU<br>4. RISC-V community growth → ecosystem building in progress<br>5. India RISC-V mandate creates new geographic market<br>6. Defense budget increases in NATO countries (if SHA resolved)<br>7. Potential acquisition target for SiFive, Codasip, or large OEM | 1. ARM responds with aggressive low-power core (Cortex-M55, Helium extensions)<br>2. RISC-V community develops open-source ultra-low power solution that commoditizes Fiora5's IP<br>3. Talent acquisition failure → technical roadmap delays<br>4. EDA tool cost (Synopsys/Cadence) scales to €1M+/year for commercial development<br>5. First customer takes 36 months, not 18 → cash crisis<br>6. IP litigation from ARM (ISA is open, implementation may still face claims) |

**Cross-analysis:**
- **SO strategy:** Use Ciprian's Arteris network to get introductions to 3–5 potential design-win customers; apply for EU CHIPS Act grants to extend runway without dilution
- **WT risk:** Technical delays + slow first customer = cash runs out before validation → fatal

**Porter's Five Forces:**

| Force | Score (1–10) | Assessment |
|-------|:---:|---------|
| **Competitive rivalry** | 9/10 HIGH | ARM's 90% market share + SiFive + Codasip = intense. Fiora5 needs to carve a niche, not fight head-on |
| **Supplier power** | 7/10 HIGH | Synopsys and Cadence are a duopoly for EDA tools. Non-commercial licenses = €10K/yr; commercial = €200–500K/yr. This cost jump is a significant barrier |
| **Buyer power** | 8/10 HIGH | OEMs buying CPU IP have significant power: they can stick with ARM (known), wait for community RISC-V (free), or shop multiple vendors. Long sales cycles, RFQ process, internal teams can build their own |
| **Threat of substitution** | 7/10 HIGH | Open-source RISC-V cores (CVA6, PicoRV32, SERV) are free. Premium value must be clearly demonstrated. If open-source catches up on power efficiency, Fiora5's moat erodes |
| **Threat of new entry** | 4/10 LOW | Semiconductor IP requires 3–5 years of R&D and domain expertise before producing a credible core. High barrier to entry (but Fiora5 itself IS the new entrant) |

**Industry attractiveness score: 4/10.** High rivalry, high supplier power, high buyer power — classic "tough industry." Opportunity exists in niche positioning but is narrow and requires flawless execution.

---

### 2.4 Deal Structure — Score: 2/10

*Informed by: FM #4 (Comps), FM #7 (IC Memo — Returns), V7 parameters D1–D11*

#### Instrument & Terms

| Element | Deck (SAFE) | Notes (CLA) | Assessment |
|---------|:---:|:---:|---------|
| Instrument | SAFE | CLA | Discrepancy unresolved. SAFE = simpler, CLA = more investor-friendly. Must clarify before any diligence |
| Amount | €500K | €500K | Insufficient for 18-month runway (only 5-7 months at realistic burn) |
| Cap | Not stated | €8M | High for demo stage — see comps below |
| Discount | Not stated | 20% | Standard |
| Protective provisions | None stated | None stated | No LP, no anti-dilution, no pro-rata, no information rights — all standard terms missing from what was shared |

#### Comparable Company Valuations (FM #4 — Pre-Revenue RISC-V IP)

| Company | Stage at First Raise | Cap / Post-Money | Year | Notes |
|---------|:---:|:---:|:---:|------|
| Codasip | Pre-product academic spinout | ~€2–4M | 2014 | Czech/German, strong uni background |
| SiFive | MVP + first customer LoI | ~$10M | 2015 | Silicon Valley, stronger team brand |
| Andes Technology | Product in market | Higher | 2005 | Taiwan, bootstrapped first |
| iNoCs (Ciprian's company) | Research proto, academic | ~€1–3M est. | 2010s | Acquired by Arteris — exit value unknown |
| **Fiora5 ask** | Demo, zero customers | **€8M** | 2026 | 2–4× premium vs. comparable stage |

**Implied valuation range by methodology:**

| Methodology | Low | Mid | High |
|-------------|:---:|:---:|:---:|
| Stage-comparable (pre-product CEE/EU deep tech) | €2M | €3M | €5M |
| Team quality premium (Ciprian exit) | +€0.5M | +€1M | +€1.5M |
| Technology premium (if 50% power claim verified) | +€1M | +€2M | +€3M |
| **Fair value range** | **€3.5M** | **€6M** | **€9.5M** |

**Assessment:** The €8M cap sits at the very top of a generous range, *only* if the technology claim is independently verified and the team premium is fully credited. At demo stage without external validation, €3.5–5M is the defensible range.

**Discrepancy flag:** SAFE vs. CLA is a material difference. In a SAFE without a cap explicitly stated, conversion dynamics at Seria A could be unfavorable to investor. This must be resolved before any term sheet discussion.

**Missing protective provisions (standard for this stage):**
- Liquidation preference 1× non-participating
- Pro-rata rights for follow-on
- Information rights (quarterly at minimum)
- MFN clause
- Anti-dilution (broad-based weighted average minimum)
- Board observer right

None of these were mentioned in available materials.

---

## 3. ASYMMETRY ASSESSMENT

*Informed by: V7 formula: Return = P(win/lose) × Expected Return × Portfolio Allocation*

### P(win/lose) Estimate

| Factor | Weight | Score | Weighted |
|--------|:------:|:-----:|:--------:|
| Technical team quality | 25% | 7/10 | 1.75 |
| Commercial execution capacity | 25% | 3/10 | 0.75 |
| Market timing | 15% | 7/10 | 1.05 |
| Competitive positioning | 15% | 4/10 | 0.60 |
| Capital sufficiency | 10% | 2/10 | 0.20 |
| SHA compatibility (for V7) | 10% | 0/10 | 0.00 |
| **Total P(win) score** | 100% | | **4.35/10** |

**P(win) in 7 years, independent of V7 SHA: ~20–25%**
**P(win) for V7 specifically (SHA blocker): <5%** (requires fundamental business model pivot away from defense)

### Expected Return (if win scenario, no SHA block)

| Scenario | Probability | Revenue Year 7 | Exit Multiple | Exit Value | V7 Share (~4%) | V7 Return | MOIC |
|----------|:-----------:|:--------------:|:-------------:|:----------:|:----------------:|:---------:|:----:|
| 🔴 **Fail** | 35% | €0 | 0× | €0 | €0 | -€500K | 0.0× |
| 🟠 **Stagnation** | 30% | €500K ARR | 4× revenue | €2M | €80K | -€420K | 0.2× |
| 🟡 **Base** | 20% | €2M ARR | 5× revenue | €10M | €400K | -€100K | 0.8× |
| 🟢 **Bull** | 10% | €5M ARR | 7× revenue | €35M | €1.4M | +€900K | 2.8× |
| 🟢🟢 **M&A exit** | 5% | Strategic asset | — | €50–100M | €2–4M | +€1.5–3.5M | 3–7× |

**Expected MOIC (probability-weighted, no SHA block, V7 ~4% at €500K investment):**

```
E[MOIC] = 0.35×0 + 0.30×0.2 + 0.20×0.8 + 0.10×2.8 + 0.05×5.0
        = 0 + 0.06 + 0.16 + 0.28 + 0.25
        = 0.75×
```

**Expected MOIC: 0.75× — negative expected value even before SHA constraint.**

The math doesn't work even in the scenario where V7 could legally invest. The combination of high failure probability + long timeline + small revenue at exit + thin ownership stake = negative expected value at €500K entry.

### Asymmetry Map

```
═══════════════════════════════════════════════════════════════
           P(win/lose)              Expected Return (R)
═══════════════════════════════════════════════════════════════

  🟢 Technical team: genuine depth   🟢 IP model: 80-90% GM at scale
  🔴 SHA conflict: BLOCKER           🔴 Negative EV at current cap
  🔴 Zero commercial validation      🔴 Timeline 10-15 years
  🔴 Underfunded (5-7 mo runway)     🔴 Small SOM → small exit unless M&A
  🔴 GTM unproven in hard domain     🟡 RISC-V tailwind is real
  🔴 P(win) overall ~20-25%          🟡 M&A optionality exists (SiFive,
  🔴 P(win) for V7 <5%                  Codasip, defense primes)
═══════════════════════════════════════════════════════════════

  Expected MOIC (no SHA block): 0.75× — NEGATIVE EV
  Expected MOIC (with SHA block): ~0× — investment not possible

  🔴 ASYMMETRY NEGATIVE — downside dominates
═══════════════════════════════════════════════════════════════
```

---

## 4. RISK ANALYSIS

*Informed by: MC #10 (Risk Assessment & Scenario Planning)*

### Risk Matrix — Top 15 Risks

| # | Risk | Category | Prob (1–5) | Impact (1–5) | Score | EWI | Mitigation |
|---|------|----------|:---:|:---:|:---:|------|-----------|
| 1 | SHA conflict — defense customers incompatible with V7 SHA | Regulatory | 5 | 5 | **25** | Fiora5 names Lockheed/BAE/Rheinmetall in deck | V7 cannot invest without fundamental pivot by Fiora5 |
| 2 | Semiconductor talent scarcity — cannot hire in Romania | Operational | 5 | 5 | **25** | Immediate: no engineers beyond founding team | Global remote hiring; explore university partnerships |
| 3 | First design win takes 36+ months (not 18) | Financial | 4 | 5 | **20** | No LOI / LoI after 12 months post-raise | Bridge financing; grant capital; pivot to smaller customer |
| 4 | EDA tool costs scale to €300K+/year for commercial tapeout | Financial | 4 | 4 | **16** | Tool cost grows rapidly past demo phase | Apply for EDA vendor startup programs (Cadence CDNLive, Synopsys ARC) |
| 5 | €500K runway insufficient — cash crisis at month 6 | Financial | 4 | 4 | **16** | Burn rate exceeds €80K/month | Raise alongside non-dilutive (EU CHIPS Act grants) |
| 6 | Technical claim (50% power reduction) fails independent benchmark | Technical | 3 | 5 | **15** | 3rd party review before closing | Require independent power analysis as diligence condition |
| 7 | ARM responds with ultra-low power Cortex-M variant | Market | 3 | 5 | **15** | ARM product announcements | Monitor ARM roadmap; Fiora5 needs 2-3 year head start |
| 8 | ITAR/export control compliance for any defense customer | Regulatory | 4 | 4 | **16** | First defense customer discussion | Legal opinion on ITAR exposure before engaging defense |
| 9 | Founding team split (4 co-founders, no vesting mentioned) | Operational | 3 | 4 | **12** | Early disagreements on direction | Require vesting schedule with 1-year cliff as deal term |
| 10 | Open-source RISC-V catches up on power efficiency | Market | 2 | 5 | **10** | Community energy reporting for low-power cores | Maintain 18-month lead on open-source alternatives |
| 11 | IP infringement claim by ARM on implementation (not ISA) | Regulatory | 2 | 5 | **10** | ARM legal threats to RISC-V companies | Freedom-to-operate IP analysis before commercialization |
| 12 | Next venture round fails — bridge or down round needed | Financial | 3 | 3 | **9** | Slow traction signals | Customer LOI before Series A; grant capital bridge |
| 13 | Overestimated TRL (founders say 4-5, likely 3-4) | Technical | 4 | 3 | **12** | Demo fails under scrutiny | Independent technical review of architecture |
| 14 | Synopsys/Cadence license dependency — cost control risk | Operational | 2 | 3 | **6** | Contract renewals | Explore open-source EDA (OpenROAD) for initial development |
| 15 | Romania regulatory risk (IP ownership, talent mobility laws) | Regulatory | 2 | 2 | **4** | No immediate signal | Legal structure review; IP held in Swiss/Luxembourg holding |

### Kill Scenarios

**Scenario 1 — Technical (most likely): Power claim fails.** If independent silicon benchmarking reveals the 50% claim is closer to 15-20% (common in semiconductor marketing), Fiora5 loses its only differentiator. ARM Cortex-M0+ becomes a credible substitute. Company has no path to first design win.

**Scenario 2 — Commercial (likely): First customer doesn't close by month 18.** Company burns through €500K in 6-7 months. Next raise fails because there is nothing to show. Unable to pay EDA licenses. Technical team fragments. Company dissolves.

**Scenario 3 — Structural (certain for V7): SHA conflict never resolved.** Fiora5 chooses to continue targeting defense (highest margin, strongest differentiation on defense electronics). V7 cannot follow without violating SHA. Investment blocked before it starts.

### Scenario Planning

| Scenario | Revenue Y5 | Exit | V7 MOIC | Probability |
|----------|:---:|:---:|:---:|:---:|
| **Best case** | €3–5M ARR | M&A by SiFive/Codasip at €30–50M | 2.4–4.0× | 10% |
| **Base case** | €800K–1.2M ARR | Long journey, possible M&A at €8–15M | 0.6–1.2× | 25% |
| **Worst case** | €0 | Company dissolves, capital loss | 0× | 40% |
| **Black swan** | Fiora5 IP becomes standard in EU defense electronics | EU defense prime acquisition at €100–200M | 8–16× | 5% |

**Black swan note:** If EU defense sovereignty push (German Zeitenwende, EU Defence Industrial Strategy) accelerates demand for non-ARM, non-US processor IP in defense electronics — and Fiora5 is the only European RISC-V IP company with a defense-grade product — an acquisition at a large premium is plausible. However, this scenario requires: (a) EU defense funding, (b) Fiora5 surviving 5+ more years, (c) V7 SHA being amended (which requires LP consent). Extremely speculative.

---

## 5. VALUATION

*Informed by: FM #4 (Comps), FM #7 (IC Memo — Valuation)*

**Note:** FM #1 (DCF) and FM #2 (Three-Statement) are not applicable — zero revenue, no financial statements. FM #3 (LBO) not applicable — equity-only VC round, no debt.

### Method 1: Stage-Based Comparable Transactions

| Company | Stage | Geography | Year | Valuation | Adj. for 2026 |
|---------|-------|-----------|:----:|:---:|:---:|
| Codasip seed round | Pre-product, academic | CZ | 2014 | €2–4M | €3–5M (inflation-adj.) |
| SiFive seed | MVP + LOI | US | 2015 | ~$8M | $12M (inflation-adj.) |
| Syntacore early rounds | Pre-product | Russia | 2015 | est. €3–5M | €4–6M (CEE peer) |
| Generic EU deep-tech pre-revenue | Demo stage | EU | 2024-25 | €3–8M | — |
| **Implied range** | | | | | **€3–7M** |

### Method 2: Team / IP Premium Adjustment

| Factor | Premium | Justification |
|--------|:-------:|--------------|
| Base (generic deep-tech demo) | €3M | Median EU pre-revenue deep-tech seed |
| Ciprian exit premium | +€1.5M | iNoCs→Arteris = validated path in same domain |
| Petru 10yr experience premium | +€0.5M | Hard-to-replicate technical depth |
| RISC-V timing premium | +€0.5M | Market tailwind |
| Zero customers discount | -€0.5M | No commercial validation |
| Romania location discount | -€0.5M | Non-hub location, talent risk |
| **Adjusted fair value** | | **€4.5–5.5M** |

### Method 3: Future Value Back-Solve

If bull case exit is €35M in year 7, and V7 needs 3× MOIC:
- V7 must own at minimum: €1.5M / (€35M) = 4.3%
- At €500K investment: implied max cap = €500K / 4.3% = **€11.6M**
- At a 30% discount to account for failure probability: **€8.1M**

This is the *only* methodology that justifies €8M — and it requires the bull case to materialize (20% probability) with no dilution.

### Valuation Football Field

```
Method                          Low          Mid          High
────────────────────────────────────────────────────────────
Stage Comps (CEE adjusted)      €3.0M  ████████░░░░  €7.0M
Team/IP Premium Adj.            €4.0M  ░░████████░░  €6.5M
Back-solve (3× target)          €6.0M  ░░░░████████  €11.6M
────────────────────────────────────────────────────────────
Defensible range                €3.5M  ████████████  €8.0M
Fiora5 ask                                       ▲ €8.0M
V7 recommended (if investing)   €4.0M — €5.5M
```

**Conclusion:** €8M cap is defensible *only* at the high end of a generous range, and only if: (a) power claim is independently verified, (b) no SHA conflict, (c) €500K is bridge to near-term MVP milestone. At demo stage with no external validation, V7 would negotiate to €4–5.5M cap.

---

## 6. RECOMMENDATION

### ⛔ PASS — Three structural blockers

**Verdict: PASS (Not Watchlist)**

This is not a "come back later with more traction" — two of the three blockers are structural for V7 specifically.

---

**Blocker 1 — SHA Conflict (FATAL for V7):**

The SHA prohibits investment in weapons, with an exception for non-lethal defense. Fiora5 explicitly targets Lockheed Martin, BAE Systems, and Rheinmetall — manufacturers of lethal weapons systems. CPU IP embedded in guided munitions, combat drones, or fire control systems is not "non-lethal defense." This cannot be resolved without:

1. Fiora5 removing all defense customers from their business plan and marketing materials, OR
2. V7 LPs consenting to amend the SHA weapons restriction

Neither is realistic in the near term. **Investment is blocked.**

**Blocker 2 — Negative Expected Value at €8M cap:**

Even in a no-SHA-conflict scenario, the probability-weighted expected return is 0.75×. The combination of high failure probability (35% zero), long time horizon (7+ years), thin ownership at €500K entry, and small realistic exit size (most likely <€15M) produces negative EV. Only the low-probability M&A or defense-prime acquisition scenarios justify the investment, and those require the SHA to be amended.

**Blocker 3 — V7 Cannot Add Value:**

V7's stated value proposition is to be an "investor of choice" — a partner that adds operational, strategic, and network value. V7 has no semiconductor IP industry network, no engineering talent pipeline in this domain, and no experience navigating the 18–36 month semiconductor design-win sales cycle. Fiora5 would receive capital and nothing else. The best investors for this deal are: IMEC (EU chip research), EIF (European Investment Fund) via CHIPS Act, NATO Innovation Fund, or a corporate CVC from a defense or semiconductor prime.

---

**What would need to change for a reconsideration:**

| Condition | Current State | Required State |
|-----------|:---:|:---:|
| SHA compatibility | ❌ Defense customers | ✅ Clear business plan excluding lethal applications |
| Technology validation | ❌ Internal claim | ✅ 3rd party power benchmark on FPGA |
| Revenue traction | ❌ Zero | ✅ ≥1 LOI or paying pilot |
| Cap | ❌ €8M at demo | ✅ €4–5M, or €8M post-MVP validation |
| Runway | ❌ 5–7 months | ✅ ≥18 months post-raise |
| V7 value-add | ❌ Capital only | ✅ Connector to wearables OEM or edge AI customer |

If Fiora5 pivots away from defense, validates power claims independently, closes one pilot, and comes back at a lower cap — V7 could reconsider as a small €100–150K ticket into a larger round led by a specialist investor.

---

## 7. STRATEGY FILE IMPROVEMENTS

*Informed by: gaps identified by applying MC #10 (Risk Assessment), FM #4 (Comps), MC #1 (TAM) to V7's existing files*

The following gaps were identified when applying Robert's institutional framework to a real deal. These are proposed improvements to V7's strategy files.

---

**PROPOSED CHANGE #1:**
```
File: strategy/asymmetry_parameters.md
Section: Pilon 3 — Industrie / I1: TAM
Current: Single qualitative rating (🟢/🟡/🔴) per parameter
Proposed: Require both top-down AND bottom-up TAM calculation for every new deal.
          Format: TAM (top-down) / SAM / SOM (bottom-up) with explicit math.
          Add: 5-year CAGR and source (analyst report or methodology stated).
Rationale: Fiora5's TAM looks large ($5B processor IP) but Fiora5's realistic SOM
           (wearables only, 5-year) is €500K–2M ARR — a 99%+ reduction. Without
           bottom-up math, TAM ratings are misleading. The Aqurate analysis had the
           same gap (TAM of €7B for personalization, SOM unstated).
```

---

**PROPOSED CHANGE #2:**
```
File: strategy/asymmetry_parameters.md
Section: Pilon 2 — Companie / Risk subsection (missing)
Current: No structured risk scoring matrix in the framework
Proposed: Add a Risk Matrix section to every deal analysis:
          15 risks minimum, scored on Probability (1-5) × Impact (1-5) = Risk Score.
          Require: Early Warning Indicator + Mitigation per risk.
          Top 5 risks presented in IC Memo summary.
Rationale: Applying MC #10 to Fiora5 revealed the SHA conflict (Risk Score 25/25)
           and talent scarcity (25/25) immediately — two risks that should have been
           called out in Edi's initial analysis before any meeting time was spent.
           A structured risk matrix would have surfaced the SHA conflict in
           pre-screening.
```

---

**PROPOSED CHANGE #3:**
```
File: strategy/investment_analysis_flow.md
Section: Stage 2 — Valuation (currently marked "de dezvoltat")
Current: Stage 2 is a placeholder with no methodology specified.
Proposed: Stage 2 Valuation must include:
          a) Comps analysis: 5+ comparable companies with funding/valuation data
          b) Stage-based benchmarks: what do similarly-staged companies in same
             domain raise at? (CEE-adjusted)
          c) Back-solve: what cap allows V7 to hit target MOIC if bull case
             materializes?
          d) Football field: present all three as a range, not a single number.
          e) Instrument analysis: SAFE vs. CLA vs. equity — which is better for V7?
Rationale: The Fiora5 €8M cap required three distinct methodologies to assess.
           Having a defined Stage 2 process would prevent V7 from anchoring on a
           founder-stated valuation without independent benchmarking.
```

---

**PROPOSED CHANGE #4:**
```
File: strategy/criteria.md
Section: SHA Compliance — Pre-Screening Checklist (missing)
Current: criteria.md does not include SHA restriction screening.
Proposed: Add a mandatory SHA pre-screen as Step 0 before any analysis begins:
          □ Weapons / lethal defense systems? (SHA: NO, except non-lethal defense)
          □ Gambling? (SHA: NO)
          □ Tobacco? (SHA: NO)
          □ Crypto/digital assets as primary business? (SHA: NO)
          □ Real estate as primary business? (SHA: NO)
          □ Adult entertainment? (SHA: NO)
          If any check fails → PASS immediately. No analysis required.
Rationale: Fiora5 required full analysis (Edi's meeting + pitch deck review +
           analysis file) before the SHA conflict was formally called out. A
           2-minute SHA pre-screen would have saved that time.
```

---

**PROPOSED CHANGE #5:**
```
File: strategy/investment_framework.md
Section: Post-Mortem Template
Current: Template includes "ce am scris la pre-investiție?" and "ce s-a întâmplat?"
Proposed: Add a "Deals We Passed" section alongside portfolio post-mortems:
          - Why did we pass? (specific reasons, not generic)
          - What happened to the company in 1-2-3 years?
          - Was our reasoning correct?
          - What would we do differently?
Rationale: Workshop noted this explicitly: "și companiile pe care le REFUZĂM trebuie
           documentate." The framework doesn't currently have a structured template
           for tracking refused deals. Fiora5 should be filed in a Deals Refused
           tracker with a review date of 18.02.2027.
```

---

## 8. HOW THIS ANALYSIS HELPS V7 CAPITAL

### What was unclear before — what is clear now

| Question | Before (Edi analysis) | After (Robert framework) |
|----------|----------------------|--------------------------|
| Is the SHA conflict real? | ✅ Flagged | ✅ Quantified as Risk Score 25/25 — highest possible |
| Is the €8M cap fair? | "Suprapreț" qualitative | Benchmarked against 5 comps. Fair range: €3.5–5.5M. Overpriced by 45–130% |
| What is the expected return? | Described as "negative" | Calculated: E[MOIC] = 0.75× — negative EV even without SHA |
| How big is Fiora5's real market? | "Piață în creștere" | SOM (wearables, Y5) = €500K–2M ARR. Small without defense |
| What are the kill scenarios? | "Orizont 10-15 ani" | 3 kill scenarios identified with triggers and early warning indicators |
| Who should invest in Fiora5 instead? | Not addressed | NATO Innovation Fund, EU CHIPS Act grants, defense CVC (Airbus Ventures, BAE Systems Digital) |

### Which strategy files should be updated

1. **`criteria.md`** — Add SHA pre-screen checklist (immediate action, 30 min work)
2. **`asymmetry_parameters.md`** — Add bottom-up TAM requirement + risk matrix
3. **`investment_analysis_flow.md`** — Build out Stage 2 Valuation methodology
4. **`investment_framework.md`** — Add Deals Refused tracker template

### Information gaps — what remains unknown

| Gap | Owner | How to close |
|-----|-------|-------------|
| Is the 50% power reduction claim real? | Technical | Independent review: share architecture with semiconductor academic (TU Dresden, IMEC) |
| What is Darian's commercial background? | Edi | LinkedIn deep-dive + reference call with someone who has worked with him |
| SAFE vs. CLA — which is the actual instrument? | Edi | Ask Fiora5 directly in next touchpoint |
| iNoCs → Arteris exit terms (Ciprian's actual payout) | Robert | AngelList, Crunchbase, court filings in CH if public |
| EU CHIPS Act grant eligibility for Fiora5 | Elena legal | 30-min call with EU funding advisor |
| NATO Innovation Fund interest in RISC-V IP | — | Would only be relevant if V7 co-invests alongside or refers |

### Referral recommendation

**Refer Fiora5 to:**
1. **NATO Innovation Fund** (NIF, Luxembourg) — specifically invests in dual-use deep tech. RISC-V defense electronics is core mandate.
2. **EIF via EU CHIPS Act** — non-dilutive grant capital for European semiconductor IP startups
3. **Underline Ventures** (Bogdan already in contact per notes) — Romanian VC with higher risk appetite and smaller tickets
4. **Airbus Ventures / BAE Systems Digital** — CVC arms that can absorb SHA-incompatible defense bets

Referring well, even on a pass, is part of V7's "investor of choice" positioning.

---

*Analysis produced using Robert's Deep Analysis framework (Robert/notes/prompt.md). Financial Models prompts: FM #4, FM #7. Management Consulting prompts: MC #1, MC #2, MC #4, MC #5, MC #9, MC #10, MC #12. Underlying data: Pitch Deck Fiora5 (feb 2026), Notițe Edi (meeting fondatori), SHA V7 Capital, V7 strategy files (asymmetry_parameters.md v3.1, investment_framework.md, investment_analysis_flow.md). All financial projections are estimates based on comparable transactions and stated assumptions — not audited data.*
