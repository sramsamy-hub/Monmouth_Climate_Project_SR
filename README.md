# MonmouthClimateRiskPipeline
How a 1 foot rise in sea level impacts insurance premiums. Relevant to P/C, Life, and Retirement Insurance

# Monmouth County Climate Risk & Capital Analytics Pipeline
## Enterprise Model Governance & Audit Documentation (ASOP 56 Compliant Blueprint)

This repository houses an automated, multi-lingual data pipeline designed to stress-test a multi-line insurance portfolio against localized climate stressors in Monmouth County, NJ.

### 🗄️ 1. Pipeline Architecture & Data Flow
1. **Data Layer (Excel/CSV):** Ground-level environmental risk metrics and segregated business portfolios.
2. **Integration Layer (SQLite):** Relational schema joining data assets on `ZipCode` into a unified master view.
3. **Analytics Engine (R):** Vector-accelerated underwriting logic calculating contingent asset and liability exposures.
4. **Reporting Layer (Python):** Object-oriented aggregation and presentation-grade executive dashboard rendering.

### 🧠 2. Actuarial Risk Matrices & Threshold Assumptions
* **P&C Underwriting (NJM Focus):** Properties with a `BaseElevation` < 10.0 ft AND `HistoricFloodCount` >= 3 face a severe 40% structural loss exposure shock; otherwise, a baseline 5% structural risk applies.
* **Life & Health (New York Life Focus):** Policyholders with `PolicyholderAge` > 65 AND `ProjectedHeatDays` > 10 trigger an excess thermal mortality risk factor of 3%, which doubles to 6% if a `ComorbidityFlag` is present; otherwise, a baseline 0.5% risk applies.
* **RIS Asset Management (MetLife Focus):** Real estate backing assets sitting at a `BaseElevation` < 5.0 ft undergo a severe 25% capital depreciation shock due to sea-level rise; otherwise, a baseline 2% market drift risk applies.

### 🔍 3. Production Control Totals & Audit Sign-Off
The production data pipeline has been fully compiled, executed, and mathematically audited. The final portfolio metrics are verified as follows:
* **Total P&C Loss Exposure:** $769,000.00
* **Total Life Risk Score Exposure:** $23,500.00
* **Total RIS Asset Depreciation Exposure:** $644,000.00
* **Consolidated Enterprise Capital-at-Risk:** $1,436,500.00

**Audited & Compiled By: Selvan Ramsamy
