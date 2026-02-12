# V7 Capital - Fees & Carry Calculation

**Sursă:** SHA (Jan 2026), Clause 8

---

## Overview Fees

| Component | Cap | Detalii |
|-----------|-----|---------|
| **Base Remuneration** | 2% Assets/an | Include toate cheltuielile |
| **Performance Carry** | 20% + 10% | Peste hurdle, în SOP shares |
| **Hurdle Rate** | EURIBOR3M + 5% | Minimum return pentru carry |
| **High-Water Mark** | Da | Protecție shareholders |

---

## 1. Company Expenses

### 1.1 Operating Expenses
Cheltuieli acoperite de Company:
- Legal și accounting
- Admin și domiciliation
- Audit și valuation
- Banking și custodian
- Travel Supervisory/Management Board
- Insurance
- Litigation
- Taxes și regulatory
- GMS expenses

### 1.2 Transaction Expenses
- Due diligence
- Brokerage și investment banking
- Transfer taxes
- Consultanți, avocați, contabili
- Exit-related costs

**NU include:** monitoring post-investiție (suportat de Portfolio Projects)

### 1.3 Abort Expenses
- Cheltuieli pentru deals eșuate
- Max **1% Assets/an**
- Necesită aprob IC + LOI signed
- Peste limit → aprobare Supervisory Board

### 1.4 Fee Income (Offsetting)
Se deduc din Remuneration:
- Arrangement, syndication, closing fees
- Monitoring fees
- Advisory, consultancy fees
- Break-up fees
- Finder's fees

**Reporting:** Quarterly la Supervisory Board

---

## 2. Base Remuneration

### 2.1 Formula
```
Base Remuneration = min(2% × Assets, Total Costs)
```

### 2.2 Calculul Assets
- La **31 decembrie** anul precedent
- Conform **IFRS 13**

### 2.3 Limitări
- Total costuri (Operating + Transaction + Abort - Fee Income) = **Aggregate Expenses**
- Dacă Aggregate Expenses > 2% Assets → aprobare **Supervisory Board** + justificare

### 2.4 Transparență
- Raport anual detaliat la GMS

---

## 3. Performance Remuneration (Carry)

### 3.1 Formă de Plată
- **Exclusiv SOP** (stock option plan)
- Aprobat de Supervisory Board
- Annual SOP Award decis de GMS

### 3.2 Eligibilitate
- **Executive Management Team**
- Split între membri decis de GM în 20 zile
- Confirmat de Supervisory Board

### 3.3 Hurdle Rate
```
Hurdle Rate = EURIBOR 3M + 5%
```
- Calculat în moneda situațiilor financiare
- Dacă IRR < Hurdle → **zero carry**

### 3.4 Carry Rates

| IRR realizat | Carry Rate |
|--------------|------------|
| < Hurdle | **0%** |
| Hurdle - 25% | **20%** din Excess Return |
| > 25% | 20% + **10%** din porțiunea peste 25% |

**Exemplu:**
- IRR realizat: 30%
- Hurdle: 8%
- Excess Return = 30% - 8% = 22%
- Carry = 20% × 22% + 10% × (30% - 25%) = 4.4% + 0.5% = **4.9%**

### 3.5 High-Water Mark (HWM)

**Definiție:** IRR maxim pentru care s-a plătit carry anterior

**Mecanism:**
- Dacă IRR curent < HWM → **zero carry**
- Carry se plătește **doar** pentru porțiunea peste HWM
- HWM protejează shareholders de plată dublă

**Exemplu:**
- 2025: IRR 28%, carry plătit → HWM = 28%
- 2026: IRR 25% → **zero carry** (sub HWM)
- 2027: IRR 32% → carry doar pe (32% - 28%) = 4%

---

## 4. Formule detaliate de calcul

### 4.1 Variabile

| Simbol | Definiție |
|--------|-----------|
| NAV_start(i) | NAV shareholder la începutul perioadei |
| NAV_end(i) | NAV shareholder la sfârșitul perioadei (înainte de carry) |
| CF_k | Cash flow k (subscripție/redemption) |
| t_k | Ziua cash flow k |
| r_daily | Hurdle Rate / 365 |
| Δdays | Zile de la CF până la sfârșit perioadă |

### 4.2 Hurdle Accrual
```
Hurdle Accrual = [NAV_start × (1 + r_daily)^days] 
              + Σ CF_k × (1 + r_daily)^Δdays 
              - [NAV_start + Σ CF_k]
```

### 4.3 Excess Return
```
Excess Return(i) = max{0, [NAV_end - (NAV_start + Σ CF_k + Hurdle Accrual)]}
```

### 4.4 Excess cu HWM
```
HWM_base(i) = max{prior HWM, NAV_start + Σ CF_k + Hurdle Accrual}
Excess_HWM(i) = max{0, NAV_end - HWM_base}
```

### 4.5 Performance Remuneration
```
Performance = 20% × min{Excess Return, Excess_HWM}
```

Pentru IRR > 25%:
```
Performance = 20% × base_excess + 10% × (IRR - 25%) portion
```

---

## 5. IRR Calculation Method

### 5.1 Standard
- **XIRR** (Excel function)
- Consideră timing exact al fiecărui cash flow

### 5.2 Cash Flows incluse
- Toate Contributions (negative)
- Toate distributions (positive)
- NAV final (positive, pentru calcul)

### 5.3 Exemplu (din SHA Appendix 4)

| Data | Cash Flow (€) | Descriere |
|------|---------------|-----------|
| 07.01.2022 | -100,000 | Initial investment |
| 26.04.2022 | -100,000 | Follow-on |
| 15.07.2023 | +20,000 | Dividend |
| 01.08.2024 | -100,000 | Follow-on |
| 16.10.2025 | +40,000 | Dividend |
| 01.06.2026 | +600,000 | Exit value |

**XIRR = 25.9%**

---

## 6. SOP Award Terms (Appendix 6)

| Element | Termen |
|---------|--------|
| **Eligible** | Executive Management Team |
| **Grant Price** | Fair Market Value la grant |
| **Vesting** | 12 luni |
| **Exercise Price** | Fair Market Value la exercise |
| **Put Option** | Beneficiary poate vinde înapoi la Company |

### Put Option Schedule
- 2031: max 50%
- 2032: max 15%
- 2033: max 15%
- 2034: max 20%

### Clawback
- Termination for Cause → Shares din ultimii 5 ani la valoare nominală
- Performance scăzută ulterioară → ajustare pe baza de 5 ani

---

## 7. Summary Calculator

**Input:**
- NAV start: 10M EUR
- NAV end: 13M EUR
- No cash flows
- Hurdle: 8%
- Prior HWM: 12%

**Calcul:**
1. Return = (13-10)/10 = 30%
2. Hurdle Accrual = 10M × 8% = 0.8M
3. Required for hurdle = 10.8M
4. Excess = 13M - 10.8M = 2.2M (22%)
5. Above HWM? 13M > 12M → da, calcul carry
6. Excess_HWM = 13M - 12M = 1M
7. Carry base = 20% × 1M = 200K
8. Above 25%? 30% - 25% = 5% portion
9. Carry accelerated = 10% × 0.5M = 50K
10. **Total Carry = 250K EUR**

---

*Actualizat: 2026-02-06*
*Sursă: SHA Clause 8, Appendix 4, 6*
