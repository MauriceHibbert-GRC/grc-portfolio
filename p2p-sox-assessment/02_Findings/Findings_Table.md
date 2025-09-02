# Findings Summary – P2P SOX Readiness

| Gap | Risk (plain English) | SOX / ITGC Mapping | Recommendation |
|---|---|---|---|
| Auto-approved requisitions | Unauthorized/unnecessary purchases → wasted funds, misstated financials | **SOX:** Authorization • **Process:** P2P approvals • **ITGC:** Access to Programs & Data | Multi-level approvals; disable auto-approval; review approval logs |
| Missing 3-way match | Unordered items, altered prices, duplicates paid | **SOX:** Completeness & Accuracy • **Process:** 3-way match • **ITGC:** ERP config | Enforce PO–GR–Invoice match; document limited exceptions |
| Shared GL passwords | Fraud/erroneous entries untraceable; broken audit trail | **SOX:** Validity & Authorization • **Process:** Invoice validation accountability • **ITGC:** Unique IDs, password policy | Unique users, strong passwords, audit logging, periodic access review |
| One person requests–processes–signs checks | Fraud/misappropriation; no oversight | **SOX:** Segregation of Duties & Authorization • **Process:** Disbursement approvals | Dual signatures (≥ threshold); split duties; mgmt review of disbursements |
| Admin via verbal approval | No evidence of authorization; undetected manipulation | **SOX:** Authorization & Integrity • **ITGC:** Privileged access control | Formal request workflow; documented approval; admin activity logging |
| Access by email request | Unauthorized access; P2P manipulation | **SOX:** Authorization & Validity • **ITGC:** Provisioning/least privilege | Formal workflow; RBAC; documented approvals; periodic access reviews |

