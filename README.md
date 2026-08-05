#  KisanPay — B2B Agricultural Supply Chain Payment & Credit Infrastructure

<p align="center">
  <img src="https://img.shields.io/badge/Course-MGT%20589%20Payment%20Technology-green?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/University-COMSATS%20Islamabad-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Semester-Spring%202026-gold?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Status-Capstone%20Submitted-brightgreen?style=for-the-badge"/>
</p>

<p align="center">
  <strong>FinTech Payment Strategy Capstone Project Report</strong><br/>
  Department of Management Sciences — Bachelors of Business Data (2023–2027)
</p>

---

##  Project Overview

**KisanPay (Pvt.) Ltd.** is a B2B Agri-FinTech payment orchestration platform designed to eliminate Pakistan's **PKR 459+ billion annual cost of agricultural payment inefficiency**.

The platform targets the **Arthi–Farmer–Input Supplier triangle** across Punjab and Sindh, serving:

| Segment | Size | Key Pain |
|---|---|---|
| Smallholder Farmers | 3.2 million | 90% cash/cheque; no digital credit history |
| Arthis / Commission Agents | 45,000+ | Manual ledger; PKR 5–15K/day cash logistics cost |
| Input Suppliers / Agri Dealers | 15,000+ | 25–30% default rate; no transactional data |

### Key Metrics

```
PKR 459B+    →   Annual market inefficiency addressable
0% MDR       →   RAAST payment cost (PKR 3.5B SBP subsidy FY2025)
< 30 seconds →   End-to-end settlement time (Authorization → Settlement)
3.2 Million  →   Target smallholder farmers (Punjab + Sindh)
PKR 10B      →   Year 3 transaction volume target
214%         →   5-Year cumulative ROI (internal rate of return)
```

---

## ❗ The Problem We Solve

Pakistan's agricultural sector contributes **23% of GDP** and employs **38% of the labour force**, yet remains almost entirely cash-dependent.

### Three Root Causes of PKR 459B Loss

| # | Pain Point | Annual Cost (PKR) | Primary Victim |
|---|---|---|---|
| 1 | Informal credit interest excess (60% APR vs 15% formal) | PKR 360 billion | Smallholder Farmers |
| 2 | Payment delay arbitrage (30–60 day post-dated cheques) | PKR 36–72 billion | Smallholder Farmers |
| 3 | Arthi cash logistics (transportation + reconciliation) | PKR 27 billion | 45,000+ Arthis |

**KisanPay's solution:** A thin intelligent orchestration layer routing SBP RAAST through USSD/voice channels (accessible on feature phones) combined with AI credit scoring and embedded working capital financing.

---

## 📁 Repository Structure

```
kisanpay/
│
├──  README.md                          
│
├──  kisanpay-app.html                  
│
├──  Payment_Tech_Project.xlsx          
│
├──  KisanPay_Final_Report_PMT.pdf      
```

---

## 🌐 App Features

The `kisanpay-app.html` is a **fully functional single-file web application** with 6 interactive pages:

### Pages

| Page | Description |
|---|---|
| 🏠 **Landing** | Hero section, phone mockups, features, how-it-works, arthi dashboard demo, trust badges, CTA |
| 📊 **Dashboard** | Arthi overview — daily volume, farmer settlements, transaction ledger, quick actions, KPI progress |
| 💸 **Send Payment** | RAAST / Agent OTC / BNPL payment selection, numpad amount entry, CNIC farmer lookup, payment processing |
| 👨‍🌾 **Farmer Registry** | Searchable farmer list with AI credit scores, crop history, banked/unbanked status |
| 🛡️ **Compliance** | Live gap analysis — 4 HIGH, 4 MEDIUM, 1 LOW gaps with remediation actions |
| ℹ️ **About** | Problem statement, quantified impact, team profiles, academic submission details |

### Interactive Features
-  Fully working payment numpad with formatted PKR display
-  CNIC / name lookup auto-populates farmer details
-  Payment processing simulation with RAAST confirmation toast
-  Farmer search and filter by name, CNIC, crop, village
-  Sidebar navigation with active state
-  Toast notifications for all actions
-  Year 1 KPI progress bars
-  SHA-256 hashed transaction ledger display
-  Responsive design (mobile + desktop)

### How to Deploy on Lovable

1. Go to [lovable.dev](https://lovable.dev)
2. Create a new project → **"Import HTML"**
3. Upload `kisanpay-app.html`
4. Lovable will generate a live `https://kisanpay.lovable.app` link

### How to Deploy on Netlify (30 seconds)

1. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag and drop `kisanpay-app.html`
3. Get instant `https://` link — free, no account needed

---

## Excel Workbook Guide

`Payment_Tech_Project.xlsx` contains **7 sheets**, all with live formulas (41 formulas, 0 errors):

### Sheet 1 — Tech Scoring Matrix
- 9 front-end technologies scored across 5 criteria
- Weights: Cost 30% | Speed 25% | Security 20% | Scalability 15% | UX 10%
- Live `SUMPRODUCT` weighted score formulas + `RANK` formulas
- Embedded bar chart showing weighted scores
- Green = Top-2 (RAAST, NADRA eKYC) | Red = Bottom-2 (Agent Cash, BNPL)

### Sheet 2 — Compliance Map
- 19 regulatory dimensions across AML/KYC, Licensing, Data Protection, Crypto/VASP, Cross-Border
- Status: ✓ Compliant | ◑ Partial | ✗ Gap | N/A
- Risk: HIGH / Medium / Low with colour-coded cells

### Sheet 3 — Gap Analysis
- 9 compliance gaps sorted HIGH → Medium → Low
- Each gap: description, remediation action, timeline, PKR cost, responsible function
- Total remediation cost: ~PKR 13M

### Sheet 4 — Implementation Gantt
- 18 initiatives across 12 months (M1–M12)
- Colour-coded by category: Blue=Compliance | Green=Tech | Orange=Commercial | Purple=Product
- Owner and priority (CRITICAL / HIGH / MEDIUM) for each initiative

### Sheet 5 — KPI Dashboard
- 10 KPIs: Baseline → Year 1 (2027) → Year 3 (2029)
- Includes farmers onboarded, transaction volume, settlement time, NPL rate, NPS

### Sheet 6 — Payment Flow Diagram
- Full 12-step RAAST Variant A flow (Banked Farmer Crop Sale)
- Authorization (Steps 1–4) | Clearing (Steps 5–8) | Settlement (Steps 9–12)
- All 6 parties labelled: Arthi → KisanPay → Issuing Bank → RAAST Switch → Acquiring Bank → Farmer

### Sheet 7 — Financial Projections (3-Year)
- Revenue: 0.5% platform fee on Working Capital Advances + PKR 500/month arthi subscription (Year 2+)
- **Year 1 Total Revenue: PKR 5M** (fee only — subscription free in Year 1)
- Year 2: PKR 132M | Year 3: PKR 290M | 5-Year CAGR: 52.3%
- All figures formula-driven — change assumptions in blue cells

---

## Payment Flow Architecture

KisanPay routes all transactions through three variants based on farmer profile:

```
                    ┌─────────────────────────────────────────┐
                    │         KisanPay Orchestration Layer      │
                    │   (USSD *123# + Flutter App + ISO 20022)  │
                    └──────────────────┬──────────────────────┘
                                       │
               ┌───────────────────────┼──────────────────────┐
               ▼                       ▼                       ▼
    ┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐
    │  VARIANT A      │     │  VARIANT B      │     │  VARIANT C      │
    │  RAAST Instant  │     │  Agent OTC      │     │  BNPL Credit    │
    │                 │     │                 │     │                 │
    │  Banked farmer  │     │  Unbanked       │     │  70% advance    │
    │  Any phone      │     │  farmer         │     │  at delivery    │
    │  SBP RAAST P2P  │     │  JazzCash /     │     │  RAAST +        │
    │  < 30 seconds   │     │  Easypaisa OTC  │     │  KisanPay BNPL  │
    │  0% MDR         │     │  ~30 minutes    │     │  18% APR        │
    └─────────────────┘     └─────────────────┘     └─────────────────┘
```

### RAAST Variant A — Step by Step

```
Step 1   Arthi initiates payment (CNIC + amount) via Flutter app or USSD *123#
Step 2   KisanPay validates: CNIC match, daily limit (PKR 500K), AML screening
Step 3   ISO 20022 auth request → Arthi's bank (Meezan Bank) → RAAST switch
Step 4   Authorization confirmed; transaction locked at RAAST switch          ← AUTHORIZATION COMPLETE (2–5s)

Step 5   RAAST switch forwards ISO 20022 transaction data → Farmer's bank
Step 6   Farmer's bank (UBL/MCB) validates account is active
Step 7   Interbank obligation computed at SBP settlement ledger
Step 8   KisanPay PostgreSQL ledger: SHA-256 hash recorded                    ← CLEARING COMPLETE (5–15s)

Step 9   SBP debits Meezan Bank settlement account; credits UBL/MCB
Step 10  Farmer receives PKR credit + Urdu SMS confirmation
Step 11  Settlement confirmation (pacs.002) sent back to KisanPay
Step 12  AI credit score updated; arthi daily dashboard refreshed             ← SETTLEMENT COMPLETE (<30s total)
```

---

## Technology Stack

| Technology | Score | Status | Recommendation |
|---|---|---|---|
| RAAST P2P / P2M (SBP Rail) | 4.90 / 5.00 | Core Platform Rail | ADOPT — Primary |
| NADRA eKYC API | 4.40 / 5.00 | MoU Required | ADOPT — Priority 1 |
| USSD / IVR Interface (*123#) | 4.35 / 5.00 | Planned Q3 2026 | ADOPT — Priority 2 |
| Flutter Cross-Platform App | 4.25 / 5.00 | MVP Development | ADOPT — Q3 2026 |
| RAAST P2M QR Code | 3.95 / 5.00 | Year 2 Planned | ADOPT — Year 2 |
| AI Credit Scoring Engine (ML) | 3.85 / 5.00 | Prototype Phase | BUILD — Year 1 |
| Open Banking APIs | 3.60 / 5.00 | Regulatory Pending | BUILD — Year 2 |
| Agent Cash Network | 3.15 / 5.00 | Active via Partners | INTEGRATE |
| Embedded BNPL | 3.05 / 5.00 | PSP Pending | LAUNCH post-PSP |

**Scoring weights:** Cost 30% | Speed 25% | Security 20% | Scalability 15% | UX 10%

### Key Technology Decisions

- **Blockchain: DEFER** — KisanPay's PostgreSQL + SHA-256 + RAAST outperforms on throughput (10,000+ TPS vs 15 TPS Ethereum), cost (PKR 0 vs gas fees), and SBP regulatory recognition
- **CBDC: MONITOR** — SBP pilot is consultation-stage only; no deployment timeline
- **NADRA eKYC: PRIORITY 1** — Reduces onboarding from 3 days → 5 minutes; PKR 7.5M hardware investment for 500 pilot arthis

---

## Regulatory Compliance

### Compliance Status Summary

| Category | Compliant | Partial | Gap (HIGH) | Gap (Medium) |
|---|---|---|---|---|
| AML / KYC | — | CDD, Tiered KYC, Record Retention | Transaction Monitoring, SAR Filing, Arthi EDD | — |
| Licensing | SECP Registration | RAAST MoU | PSP Licence | EMI Licence (Year 2), NADRA MoU |
| Data Protection | SBP Data Localization | — | — | PDPA 2023 / DPO |
| Crypto / VASP | SBP Circular 2021 | — | — | — |
| Cross-Border | N/A (domestic only) | — | — | — |

### Priority Remediation (Before Commercial Launch)

```
CRITICAL — Month 1:   File SBP PSP Licence application (PKR 2–3M)
CRITICAL — Month 1-2: Integrate FMU API for SAR filing (PKR 1.5M)
CRITICAL — Month 2-4: Deploy transaction monitoring AI system (PKR 2.5M)
CRITICAL — Month 1-3: Define Arthi EDD programme (PKR 500K)
MEDIUM   — Month 2:   Appoint DPO; complete PDPA privacy notices (PKR 600K)
MEDIUM   — Month 1-6: Initiate NADRA eKYC MoU engagement (PKR 8M total)
```

---

## Financial Projections

| Metric | Year 1 (2027) | Year 2 (2028) | Year 3 (2029) |
|---|---|---|---|
| Registered Arthis | 5,000 | 20,000 | 45,000 |
| Active Digital Farmers | 50,000 | 150,000 | 200,000 |
| Total Transaction Volume | PKR 2.5B | PKR 6.0B | PKR 10.0B |
| Working Capital Advances | PKR 1.0B | PKR 2.4B | PKR 4.0B |
| Platform Fee Revenue (0.5%) | PKR 5M | PKR 12M | PKR 20M |
| Arthi Subscription Revenue | PKR 0 (free) | PKR 120M | PKR 270M |
| **Total Revenue** | **PKR 5M** | **PKR 132M** | **PKR 290M** |
| Farmer Interest Savings | PKR 420M | PKR 1.008B | PKR 1.680B |

> **Note:** Arthi subscription is free in Year 1 (customer acquisition). PKR 500/month subscription activates from Year 2 onward.

---

## How to Run the App

### Option 1 — Open Directly in Browser (Zero Setup)
```bash
# Just double-click kisanpay-app.html
# Or open with any browser:
open kisanpay-app.html        # macOS
start kisanpay-app.html       # Windows
xdg-open kisanpay-app.html    # Linux
```

### Option 2 — Serve Locally
```bash
# Python (built-in)
python -m http.server 8080
# Then open: http://localhost:8080/kisanpay-app.html

# Node.js
npx serve .
```

### Option 3 — Deploy to Lovable
1. Visit [lovable.dev](https://lovable.dev)
2. New Project → Import HTML → upload `kisanpay-app.html`
3. Live link generated automatically

### Option 4 — Deploy to Netlify Drop
1. Visit [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag & drop `kisanpay-app.html`
3. Instant `https://` link, no signup required

---

## Declaration

> *The candidate confirm that the work submitted is their own and appropriate credit has been given where reference has been made to the work of others.*

---

## Key References

- State Bank of Pakistan. (2025). *Governor's Annual Report 2024–2025.* SBP Publications.
- State Bank of Pakistan. (2023). *E-Money Institution Regulations.* SBP Publications.
- FATF. (2023). *FATF Recommendations 2023.* Financial Action Task Force.
- BIS CPMI. (2024). *Fast payments: Enhancing the speed and availability of retail payments.* Bank for International Settlements.
- World Bank. (2024). *Global Findex Database 2024.* World Bank Group.
- Chishti, S., Craddock, T., & Courtneidge, R. (2020). *The PAYTECH Book.* John Wiley & Sons.

---

<p align="center">
  <strong>KisanPay (Pvt.) Ltd.</strong> · Built on SBP RAAST Rails · ISO 20022 · NADRA eKYC · FATF Compliant<br/>
  <em>Eliminating Pakistan's PKR 459B+ agricultural payment inefficiency — one mandi at a time.</em>
</p>
