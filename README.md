# FY26 Service KPI & Incentive Automation System

## Overview

Built an enterprise-scale KPI scoring and incentive automation system integrating multiple ERPNext modules to evaluate field service engineer performance across quarterly operational metrics.

The system automated KPI consolidation, role-based scoring, validation workflows, and incentive computation for large-scale field operations.

---

## Business Problem

Quarterly incentive computation and KPI evaluation were previously dependent on manual consolidation across multiple ERPNext reports and operational datasets.

Operational challenges included:

- Data fragmentation across ERP modules
- Manual KPI consolidation
- Inconsistent scoring logic
- Difficulty validating duplicate and edge-case records
- High reporting complexity across multiple employee roles
- Large operational effort for quarterly processing

The workflow required extensive manual reconciliation and validation before incentive release.

---

## Solution

Developed a Python-based automation framework that:

- Integrated data from 9 ERPNext modules
- Processed KPI records for 314 field employees
- Implemented role-based weighted scoring models
- Calculated quarterly performance scores
- Applied target-based proportional KPI capping
- Automated validation and anomaly detection workflows
- Reduced codebase complexity through modular architecture optimization

---

## Workforce Scope

The system processed quarterly KPI evaluation for:

- 157 Service Engineers (SEs)
- 8 Senior Service Engineers (Sr SEs)
- 137 Associate Service Engineers (ASEs)
- 12 Area Service Managers (ASMs)

Total Workforce Evaluated: 314 Employees

---

## KPI Framework

The weighted KPI model evaluated performance across:

- Productivity
- FTF %
- Serial Intelligence
- NPS
- Attendance
- Opportunity Conversion

The scoring framework supported role-specific KPI applicability and weighted contribution logic.

---

## Weighted Scoring Model

Performance scoring was based on a weighted 100-point KPI framework.

Role-specific target achievement was proportionally capped to standardize incentive computation across operational categories.

---

## System Workflow

```text
ERPNext APIs
      ↓
Multi-Module Data Extraction
      ↓
Pagination & Retry Handling
      ↓
KPI Consolidation Engine
      ↓
Role-Based Scoring Logic
      ↓
Target-Based KPI Evaluation
      ↓
Validation Pipeline
      ↓
Duplicate & Edge-Case Detection
      ↓
Quarterly Score Computation
      ↓
Excel Report Generation
```

## Key Features

- Multi-module ERPNext API integration
- Retry and pagination handling
- Role-based KPI scoring
- Weighted 100-point evaluation model
- Quarterly incentive computation
- Validation and anomaly detection pipeline
- Duplicate record handling
- Role-specific edge-case processing
- Automated Excel report generation
- Modularized processing architecture

---

## Engineering Challenges Solved

- Consolidated fragmented ERP datasets into unified KPI pipelines
- Standardized scoring across multiple employee roles
- Built reusable weighted KPI computation logic
- Handled pagination and retry failures during API extraction
- Designed validation workflows for duplicate and edge-case records
- Reduced operational complexity through modular code restructuring

---

## Tech Stack

- Python
- Pandas
- Requests
- ERPNext REST API
- OpenPyXL
- n8n

---

## Project Metrics

| Metric | Value |
|---|---|
| ERP Modules Integrated | 9 |
| Employees Processed | 314 |
| Employee Roles Covered | 4 |
| KPI Categories | 6 |
| Reporting Frequency | Quarterly |
| Codebase Optimization | ~5,100 → ~971 lines |

---

## Validation Framework

The validation pipeline included:

- Duplicate detection
- KPI range validation
- Missing record handling
- Role-specific edge-case validation
- Scoring consistency checks
- API response integrity verification

---

## Scalability Considerations

The system architecture was designed to support:

- Additional KPI categories
- Expanded workforce coverage
- Dynamic role-based configurations
- Scalable quarterly processing
- Modular scoring enhancements
- Additional ERP module integrations

---

## Future Enhancements

- Interactive KPI dashboards
- Real-time performance tracking
- Automated anomaly alerting
- Database-backed historical KPI storage
- Cloud deployment pipelines
- Predictive incentive analytics

---

## Business Impact

- Automated enterprise-scale KPI consolidation
- Reduced manual reconciliation effort significantly
- Improved scoring consistency and auditability
- Standardized quarterly incentive computation
- Improved operational reporting efficiency
- Enhanced maintainability through modular architecture redesign

---

## Disclaimer

This repository is a portfolio representation of work completed during an internship.

Source code, credentials, internal ERP configurations, and business-sensitive scoring logic have been excluded to comply with company confidentiality policies.
