# 🏢 Vendor & Third-Party Risk Management (TPRM)
## Third-Party Risk Assessment Register — Enterprise Risk Management

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python) ![Pandas](https://img.shields.io/badge/Pandas-2.0-150458?logo=pandas) ![NIST](https://img.shields.io/badge/Framework-NIST_CSF-darkblue) ![OCC](https://img.shields.io/badge/Framework-OCC_TPRM_Guidance-navy) ![Domain](https://img.shields.io/badge/Domain-Enterprise_Risk_Management-critical)

---

> *Every organisation outsources critical functions to third parties — cloud hosting, payment processing, logistics, professional services — and every one of those relationships carries risk that the organisation cannot fully control but remains fully accountable for. This project builds a third-party risk assessment register for 40 simulated vendors, scoring each across five risk dimensions, tiering the portfolio by residual risk, and generating the due diligence framework that procurement and enterprise risk teams use to manage vendor exposure.*

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Regulatory & Framework Basis](#-regulatory--framework-basis)
- [Dataset](#-dataset)
- [Project Structure](#-project-structure)
- [Risk Scoring Methodology](#-risk-scoring-methodology)
- [Analysis Sections](#-analysis-sections)
- [Key Findings](#-key-findings)
- [Due Diligence Framework](#-due-diligence-framework)
- [Tools & Libraries](#-tools--libraries)
- [How to Run](#-how-to-run)

---

## 🎯 Overview

Third-party risk management has become one of the fastest-growing functions in enterprise risk — driven by increasing outsourcing, cloud dependency, and regulatory scrutiny of vendor relationships following high-profile supply chain breaches. Regulators including the OCC, Federal Reserve, and Basel Committee now treat vendor risk management as a core supervisory expectation, not an optional control.

This project replicates the **third-party risk assessment workflow** used by procurement, enterprise risk management, and vendor management functions. For 40 synthetic vendors — spanning IT services, cloud infrastructure, payment processing, logistics, and professional services — the analysis:

1. **Scores each vendor across five risk dimensions**: financial stability, cybersecurity posture, regulatory compliance, geographic risk, and concentration risk
2. **Applies a contract-criticality multiplier** so that residual risk reflects not just the vendor's inherent profile but the operational importance of the relationship
3. **Tiers the full portfolio** into Critical / High / Medium / Low risk categories
4. **Generates tier-specific due diligence checklists** mirroring the risk-tiered oversight intensity mandated by OCC and Basel guidance
5. **Produces a full operational dashboard suite** — 7 visual panels covering portfolio risk, dimension analysis, due diligence workload, and business continuity exposure

> ⚠️ *All vendor names, financial figures, and risk indicators are entirely synthetic and created solely for portfolio demonstration purposes.*

---

## 📐 Regulatory & Framework Basis

| Framework | Application |
|---|---|
| **NIST Cybersecurity Framework** | Cybersecurity posture scoring methodology (certification, breach history, data access) |
| **ISO 31000 Risk Management** | Overall risk scoring architecture and tiering approach |
| **OCC Third-Party Risk Management Guidance** | Risk-tiered due diligence intensity (Bulletin 2013-29 / 2017-21 principles) |
| **Basel Committee Outsourcing Principles** | Concentration risk and business continuity assessment |

---

## 📊 Dataset

All data is **synthetically generated** within the notebook — no external file required:

| Attribute | Details |
|---|---|
| **Vendors** | 40 simulated vendor relationships |
| **Categories** | 15 categories including IT Services, Cloud Infrastructure, Payment Processing, Logistics, Cybersecurity |
| **Countries** | 15 jurisdictions including 4 classified as higher-risk |
| **Risk Dimensions Scored** | 5 (Financial · Cyber · Compliance · Geographic · Concentration) |
| **Contract Criticality Tiers** | Critical · Important · Standard |
| **Onboarding Period** | 2018–2024 |

---

## 🗂️ Project Structure

```
vendor-third-party-risk/
│
├── vendor_third_party_risk.ipynb         # Fully executed analysis notebook
│                                          # (no external data file required)
├── charts/
│   ├── portfolio_dashboard.png           # Vendor portfolio risk overview
│   ├── dimension_analysis.png            # Risk dimension deep-dive
│   ├── operational_dashboard.png         # Operational risk management summary
│   ├── risk_heatmap_certification.png    # Certification gap & dimension heatmap
│   └── continuity_risk.png              # Business continuity & exit strategy risk
│
└── README.md
```

---

## 📐 Risk Scoring Methodology

| Dimension | Weight | Key Inputs |
|---|---|---|
| **Cybersecurity Posture** | 30% | ISO 27001 / SOC 2 certification, breach history, data access level |
| **Financial Stability** | 25% | Credit rating, years in business, financial distress signals |
| **Regulatory Compliance** | 20% | Compliance violations, licensing status, GDPR relevance |
| **Concentration Risk** | 15% | Sole-source dependency, % of category spend |
| **Geographic Risk** | 10% | Operating jurisdiction risk classification |

**Contract Criticality Multiplier:** Critical contracts ×1.15 · Important ×1.05 · Standard ×1.0 — ensuring that residual risk reflects the operational consequence of vendor failure, not just the vendor's inherent risk profile.

**Risk Tier Thresholds:**
- Score ≥ 65 → **Critical**
- Score 45–64 → **High**
- Score 25–44 → **Medium**
- Score < 25 → **Low**

---

## 🔍 Analysis Sections

### 1️⃣ Vendor Register Generation
40 synthetic vendor profiles with realistic attributes across financial, cybersecurity, compliance, geographic, and operational dimensions.

### 2️⃣ Five-Dimension Risk Scoring Engine
Rule-based scoring functions for each risk dimension, weighted composite scoring, contract-criticality adjustment, and tier assignment.

### 3️⃣ Vendor Portfolio Risk Dashboard
Risk tier distribution, spend by risk tier, risk tier by category, average score by dimension, geographic risk by country, and contract criticality vs risk tier.

### 4️⃣ Risk Dimension Deep-Dive
Cybersecurity posture indicators, data access level vs cyber score, compliance violations distribution, credit rating distribution, concentration risk scatter, and SLA breaches by risk tier.

### 5️⃣ Due Diligence Checklist Generator
Tier-specific due diligence requirements (10 items for Critical down to 3 for Low) mirroring OCC risk-tiered oversight principles, with review frequency assignment per vendor.

### 6️⃣ Operational Risk Management Dashboard
Top 15 highest-risk vendors, due diligence workload by frequency, sole-source critical vendor count, risk-vs-spend bubble matrix, KPI summary table, and onboarding trend by risk tier.

### 7️⃣ Certification Gap & Risk Heatmap *(additional dashboard)*
Multi-dimension heatmap for top 15 riskiest vendors, certification gap by data access level, risk score distribution, tenure vs financial risk, category risk ranking, and financial distress impact comparison.

### 8️⃣ Business Continuity & Exit Strategy Risk *(additional dashboard)*
Sole-source vendors by category, top concentration-risk vendors, critical contract risk tier mix, SLA breach trend vs risk score, tenure by risk tier, and backup supplier coverage gap.

---

## 💡 Key Findings

### 🔐 Cybersecurity Drives the Largest Share of Portfolio Risk
With a 30% weighting, cybersecurity posture is the single largest contributor to composite vendor risk. Vendors with **Extensive data access and no ISO 27001 or SOC 2 certification** represent the highest-priority remediation targets — the certification gap analysis shows this combination is concentrated in a small but high-impact subset of the portfolio.

### ⚠️ Sole-Source Critical Vendors Are Single Points of Failure
Vendors that are simultaneously sole-source **and** tagged Critical contract criticality represent the portfolio's highest continuity risk — regardless of their composite score. These relationships require a documented exit plan and identified backup supplier as a standing control, not a reactive response to vendor failure.

### 🌍 Geography Compounds Other Risk Factors
Vendors operating in higher-risk jurisdictions show elevated composite scores even when financial and cyber indicators are favourable — confirming that geographic risk acts as a risk multiplier rather than an independent, easily offset factor.

### 💰 Concentration Risk Is Invisible to Spend-Based Review Alone
Several vendors representing a high percentage of their category's total spend would not be flagged by traditional spend-ranking — the concentration risk dimension surfaces a dependency exposure that conventional procurement review misses entirely.

### 📊 Risk-Tiered Oversight Creates a 10x Resourcing Differential
Critical-tier vendors require **quarterly** due diligence review; Low-tier vendors require only **biennial** review — a tenfold difference in oversight intensity. This is by design: it ensures vendor management resources are concentrated where residual risk is highest rather than spread evenly regardless of exposure.

---

## ✅ Due Diligence Framework

| Tier | Review Frequency | Example Requirements |
|------|------------------|----------------------|
| 🔴 **Critical** | Quarterly | On-site audit, SOC 2 Type II review, Board approval for renewal, BCP/DR testing, exit plan documented |
| 🟠 **High** | Semi-Annual | Annual audit, security certification verified, senior management approval, incident response plan reviewed |
| 🟡 **Medium** | Annual | Self-assessment questionnaire, standard contract review, basic security questionnaire |
| 🟢 **Low** | Biennial | Standard onboarding questionnaire, light-touch relationship review |

---

## 🛠️ Tools & Libraries

| Library | Application |
|---------|------------|
| **Pandas** | Vendor register generation, risk score aggregation, tier assignment |
| **NumPy** | Synthetic data generation, weighted scoring calculations |
| **Matplotlib / Seaborn** | 36+ visualisations across 5 dashboard panels — heatmaps, scatter matrices, boxplots, pie charts, stacked bars |
| **Python (native)** | 5-dimension risk scoring engine, due diligence checklist generator, tier assignment logic |

---

## ▶️ How to Run

1. Clone the repository and navigate to the project folder
2. Install dependencies:
```bash
pip install pandas numpy matplotlib seaborn
```
3. Open and run the notebook — **no external data file required**, all data is generated internally:
```bash
jupyter notebook vendor_third_party_risk.ipynb
```

> ✅ All cells are pre-executed with embedded outputs. No re-running required.

---

## 📌 About This Project

This project demonstrates applied knowledge of third-party risk management — the scoring methodology, regulatory frameworks, and risk-tiered due diligence approach that a vendor risk analyst, procurement risk specialist, or enterprise risk management professional would apply when assessing and managing a vendor portfolio.

**Skills demonstrated:**
- Multi-dimensional risk scoring and weighted composite methodology
- Risk-tiered due diligence framework design
- Concentration and business continuity risk analysis
- Applied knowledge of NIST CSF, ISO 31000, OCC, and Basel TPRM guidance
- Enterprise risk dashboard design for non-technical stakeholders

---

*Part of a 23-project data analytics portfolio spanning HR analytics, financial forecasting, NLP, e-commerce, supply chain, public health, real estate, credit risk, aviation, media, cybersecurity, clinical healthcare, urban analytics, ESG risk scoring, financial crime compliance, and enterprise third-party risk management.*
