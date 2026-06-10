# Vendor Risk Assessment Program Build Using a Free GRC Template and MetricStream Concepts

> A structured third-party vendor risk assessment program built using open-source GRC templates and MetricStream workflow concepts, producing a repeatable process that identifies, scores, and reports vendor risk against ISO 27001 and NIST CSF controls.

## Overview

Third-party vendor risk is one of the most persistent challenges in financial services GRC. Organizations like Moneris rely on dozens of vendors with access to sensitive payment data, cardholder information, and critical infrastructure. Without a structured assessment program, that exposure is nearly invisible.

I built this project to simulate a production-grade vendor risk assessment workflow using freely available GRC templates and the process logic behind MetricStream, one of the most widely deployed GRC platforms in enterprise environments. The result is a repeatable, documentation-driven program that any GRC team could adapt and operationalize.

The program covers the full assessment lifecycle: vendor intake and tiering, questionnaire-based control evaluation, risk scoring, remediation tracking, and executive-ready risk reporting. Every artifact is mapped to either ISO 27001 Annex A controls or NIST CSF functions, making the outputs immediately useful for audit evidence or board-level reporting.

This project is directly relevant to the GRC Analyst role at Moneris, where third-party risk management, regulatory alignment, and platform familiarity are core expectations. It demonstrates that I can contribute from day one without a lengthy ramp-up on process design.

## What I Built / Key Features

- **Vendor Intake and Tiering Model:** A structured intake form and tiering matrix that classifies vendors as Critical, High, Medium, or Low risk based on data access, business criticality, and regulatory exposure.
- **Risk Assessment Questionnaire:** A 60-question vendor questionnaire mapped to ISO 27001 Annex A control domains and NIST CSF categories, covering access control, incident response, data handling, and business continuity.
- **Automated Risk Scoring Workbook:** A spreadsheet-based scoring engine that calculates inherent risk, control effectiveness, and residual risk per vendor, with conditional formatting to flag high-risk items for immediate review.
- **MetricStream-Aligned Workflow Documentation:** Process diagrams and workflow documentation that mirror how MetricStream structures vendor risk tasks, approvals, and escalation paths, providing a reference for platform configuration.
- **Remediation Tracking Register:** A living register that logs identified gaps, assigns remediation owners, sets target dates, and tracks closure status through to re-assessment.
- **Executive Risk Report Template:** A polished, one-page risk summary template designed for board or senior management consumption, summarizing vendor risk posture, trend indicators, and open action items.

## Skills and Tools Demonstrated

**GRC Frameworks and Standards**
- ISO 27001:2022 Annex A control mapping
- NIST Cybersecurity Framework (Identify, Protect, Detect, Respond, Recover)
- Third-party risk management lifecycle (TPRM)

**GRC Platform Knowledge**
- MetricStream process and workflow design concepts
- Spreadsheet-based GRC tooling as a free alternative for smaller programs

**Documentation and Reporting**
- Vendor questionnaire design and control mapping
- Risk scoring methodology and residual risk calculation
- Executive reporting and risk register maintenance

**Core Tools**
- Microsoft Excel and Google Sheets for scoring workbooks and registers
- Microsoft Word and Google Docs for policy and questionnaire templates
- Draw.io for workflow and process diagrams
- NIST and ISO publicly available control catalogs as reference sources

## Architecture and Approach

The program is organized around four phases that mirror how enterprise GRC platforms like MetricStream structure third-party risk modules: Intake, Assessment, Remediation, and Reporting.

```text
[ Vendor Intake Form ]
        |
        v
[ Tiering Matrix ] --> Critical / High / Medium / Low
        |
        v
[ Risk Questionnaire ] --> Mapped to ISO 27001 + NIST CSF
        |
        v
[ Scoring Workbook ] --> Inherent Risk + Control Score = Residual Risk
        |
        v
[ Remediation Register ] --> Gap Owner + Target Date + Status
        |
        v
[ Executive Risk Report ] --> One-page summary for leadership
```

I designed each phase to be modular so that a team using MetricStream, ServiceNow GRC, or a manual process could adopt individual components without needing the full stack. The scoring methodology uses a weighted 1-5 scale for likelihood and impact, consistent with common financial services risk appetite frameworks.

## Suggested Repository Structure

```text
vendor-risk-assessment-program/
├── 01-intake/
│   ├── vendor-intake-form.docx
│   └── tiering-matrix.xlsx
├── 02-assessment/
│   ├── vendor-risk-questionnaire.xlsx
│   └── control-mapping-reference.xlsx
├── 03-scoring/
│   └── risk-scoring-workbook.xlsx
├── 04-remediation/
│   └── remediation-tracking-register.xlsx
├── 05-reporting/
│   ├── executive-risk-report-template.docx
│   └── sample-completed-report.pdf
├── workflows/
│   └── vrm-process-diagram.drawio
├── reference/
│   ├── iso27001-annex-a-mapping.xlsx
│   └── nist-csf-control-crosswalk.xlsx
└── README.md
```

## What This Demonstrates to Employers

- **Shows ability to design and operationalize a full TPRM lifecycle**, from vendor intake through risk reporting, without relying on a pre-built enterprise platform to do the thinking.
- **Demonstrates familiarity with MetricStream workflow logic**, making it easier to configure, administer, or extend an existing deployment in a financial services environment.
- **Demonstrates practical knowledge of ISO 27001 and NIST CSF**, including how to map controls to real vendor risk scenarios rather than treating them as abstract checklists.
- **Shows ability to produce audit-ready documentation**, including scored risk registers and executive reports that align with what regulators and internal audit teams expect to see.
- **Demonstrates readiness for third-party risk responsibilities at Moneris**, where payment processing vendor relationships carry significant regulatory and operational risk under frameworks like PCI DSS and OSFI guidelines.

## Getting Started

**Prerequisites:** Microsoft Excel or Google Sheets, Microsoft Word or Google Docs, and Draw.io (free, browser-based) for viewing workflow diagrams.

```bash
# Clone the repository
git clone https://github.com/your-username/vendor-risk-assessment-program.git

# Navigate into the project directory
cd vendor-risk-assessment-program
```

Open `01-intake/vendor-intake-form.docx` to begin a new vendor assessment. Follow the phase order in the directory structure. The `risk-scoring-workbook.xlsx` in `03-scoring/` is self-contained and includes instructions on the first tab.
