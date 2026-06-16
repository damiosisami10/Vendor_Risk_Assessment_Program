# Vendor Risk Assessment Program For NorthPay Financial (Simulation) - Using MetricStream Concepts

> A structured third-party vendor risk assessment program built using open-source GRC templates and MetricStream workflow concepts, producing a repeatable process that identifies, scores, and reports vendor risk against ISO 27001 and NIST CSF controls. The program covers the full vendor risk lifecycle: scoping, tiering, assessment, scoring, findings documentation, and executive reporting.

---

## What's in This Repo

### 1. TPRM Program Scope Document
[`NorthPay_TPRM_Program_Scope_v1.0.docx`](https://docs.google.com/document/d/1oc5cmbzCxvnAEHwXQ6-VfO_9Wa7qzyAKOUCdxkGxKXQ/edit?usp=sharing)

The foundational governance document for the program covers:
- Program scope and in-scope/out-of-scope criteria
- Vendor risk tiering model (Tier 1 Critical to Tier 3 Low)
- RACI matrix across GRC, Legal, IT/SecOps, and Procurement
- Control mapping across NIST CSF 2.0, ISO 27001:2022, PCI DSS v4.0, and SOC 2
- Current-state gap analysis with P1–P3 prioritisation
- Six-phase assessment lifecycle workflow
- Audit artifact retention schedule

### 2. Vendor Assessment Questionnaire
[`NorthPay_Vendor_Assessment_Questionnaire_v1.0.docx`](https://docs.google.com/document/d/1HEKYuEDSLuEBsQ_Xv35tZKeo90THfS94dvrd7dPVNCM/edit?usp=sharing)

A 15-question vendor assessment questionnaire structured across five domains, used for Tier 1 and Tier 2 vendors. Covers Information Security Governance, Access Control, Data Protection and Encryption, Incident Response, and Business Continuity. Includes a Document Request List requiring SOC 2 Type II or ISO certificate, penetration test executive summary, and cyber insurance evidence.
A 3-question self-attestation form scoped to data scope confirmation only, used for Tier 3 vendors.

| Domain | Framework |
|---|---|
| Information Security Governance | ISO 27001:2022 Clauses 5–8, NIST CSF GV/ID |
| Data Privacy & Handling | ISO 27001 A.5.12–19, GDPR Art.28, PCI DSS 3 & 4 |
| Business Continuity & Resilience | ISO 27001 A.5.29, NIST RC.RP |
| Access Control & Identity Management | ISO 27001 A.5.15–18, PCI DSS 7 & 8 |
| Incident Response & Reporting | ISO 27001 A.5.24–28, NIST RS.RP, GDPR Art.33 |

Includes a vendor profile and attestation section, completion instructions,
and an internal GRC analyst scoring rubric (0–2 per question, composite rating thresholds with analyst action).

### 3. Self-Attestation DDQ

A 3-question self-attestation form scoped to data scope confirmation only,
used for Tier 3 vendors. Vendors attest to whether they store, process, or
transmit NorthPay cardholder data, whether they access NorthPay customer PII,
and whether any security incidents affecting NorthPay staff have occurred in
the last 12 months. Scored on a Pass/Fail basis only.


### 4. Mock Assessment Results
[`NorthPay_MockAssessment_Results_v1.0.xlsx`](https://docs.google.com/spreadsheets/d/1iEIRZB_u2x-R4P4d_gh2p9FWsIU8ckxlKEEfI7CUDHE/edit?usp=sharing)

Populated assessment results for three vendors across all three risk tiers:

| Vendor | Tier | Score | Rating |
|---|---|---|---|
| CloudVault Inc. | Tier 1 — Critical | 23/30 (77%) | High Risk |
| PayAnalytics Co. | Tier 2 — Significant | 14/30 (47%) | Significant Risk |
| OfficeComms Ltd. | Tier 3 — Low | 2P / 1F | Low Risk |

Each vendor tab includes question-level responses, scores, color-coded
findings, and recommended controls. Summary dashboard with finding counts
by severity (P1/P2/P3) and live formula totals.

### 5. Q1 2025 Executive Risk Report
[`NorthPay_Vendor_Risk_Assessment_Report_Q1_2025.docx`](https://docs.google.com/document/d/1QNCNkFb6g2FmDIee9IzVUSYd78vesDY_VltVkycuZ6o/edit?usp=sharing)

Executive-facing quarterly report structured for CISO, CRO, and Board Risk
Committee consumption. Covers:
- Program snapshot: vendors assessed, high risk ratings, open P1 findings
- Headline finding narrative in plain language
- Findings at a glance table
- Seven structured findings (F-0001 through F-0005) with observation, risk
  statement, recommendation, target date, and owner
- Risk treatment recommendations mapped to ISO 27001 Annex A controls:

| Finding | ISO 27001 Control |
|---|---|
| CloudVault - no breach notification SLA | A.5.26 Response to information security incidents |
| CloudVault - BCP untested 26 months | A.5.29 Information security during disruption |
| PayAnalytics - MFA absent | A.8.5 Secure authentication |
| PayAnalytics - pen test lapsed 18 months | A.8.8 Management of technical vulnerabilities |

- Program metrics baseline: total vendors assessed, open High findings,
  vendors overdue for reassessment, average assessment score

---

## Frameworks Applied

- **ISO 27001:2022** - Clause 8.4 (supplier relationships), Annex A controls
  A.5.1, A.5.15, A.5.18, A.5.24, A.5.26, A.5.29, A.8.5, A.8.8, A.8.24
- **NIST CSF 2.0** - ID.SC (supply chain risk), PR.AA (identity management),
  GV.PO (policy), RS.RP (incident response), RC.RP (recovery)
- **PCI DSS v4.0** - Requirements 3, 4, 8, 12
- **SOC 2** - CC9.2 (vendor and business partner management)
- **GDPR** - Article 28 (processor agreements), Article 33 (breach notification)
- **PIPEDA** - Breach notification obligations

---

## Skills Demonstrated

**Control mapping** - Assessment questions, findings, and treatment
recommendations are each tied to a specific framework clause or Annex A
control, not a general category.

**Risk tiering** - Vendors classified using a three-tier model based on data
access, operational criticality, and regulatory exposure. Assessment depth,
DDQ format, and cadence vary by tier.

**Gap analysis** - Current-state gaps documented with P1-P3 prioritisation,
remediation owners, and target dates.

**Finding documentation** - Findings weere structured with observation, risk
statement, recommendation, target date, and owner which is consistent with how
findings are recorded in GRC platforms.

**Executive reporting** - Risk findings translated into plain-language
summaries for non-technical stakeholders, with a defined monthly metrics
baseline for ongoing program tracking.

**Spreadsheet-based GRC tooling** - Excel workbooks with dropdown validation,
conditional formatting and SUMIF scoring formulas for easy tracking.

---

## Tools Used

- **Google Docs** - All program documents produced in Google Docs:
  - TPRM Program Scope Document (NorthPay_TPRM_Program_Scope_v1.0)
  - Vendor Assessment Questionnaire - 15 questions across 5 domains, scored 0–2 (NorthPay_Vendor_Assessment_Questionnaire_v1.0)
  - Q1 2025 Executive Risk Report including structured findings F-0001 through F-0005, risk treatment recommendations, and program metrics (NorthPay_Vendor_Risk_Assessment_Report_Q1_2025)


- **Google Sheets** — All spreadsheet-based artifacts:
  - Vendor inventory register with risk tier classification and assessment status tracking
  - Self-attestation DDQ with dropdown response validation and GRC scoring tracker (NorthPay_SelfAttestation_DDQ_v1.0)
  - Mock assessment results across three vendors with scoring, finding documentation. (NorthPay_MockAssessment_Results_v1.0)
  - 5x5 risk heat map scored by likelihood and impact with conditional formatting bands

---

Q1 2025 Executive Risk Report is complete. Additional assessment cycles will be added as the program builds out.


