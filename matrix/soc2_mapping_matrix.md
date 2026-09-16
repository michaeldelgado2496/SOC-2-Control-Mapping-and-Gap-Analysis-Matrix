# SOC 2 Trust Services Criteria (TSC) Control Mapping & Gap Analysis Matrix

* **System Scope:** Cloud Infrastructure & Data Hosting Platform
* **Assessment Standard:** AICPA SOC 2 (2017 Trust Services Criteria - Security, Availability, Confidentiality)
* **Status:** Active Gap Remediation

---

## Control Mapping Overview

| Control ID | Trust Services Criteria | Control Description | Implementation Status | Evidence / Artifact Ref | Gap / Risk Level | Remediation Plan & Target Date |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **CC6.1** | Security / Logical Access | The entity restricts logical access to software, data, and infrastructure. | Implemented | `configs/okta_mfa_policy.json` | Low | Periodic quarterly review enforced (Target: 2026-10-01) |
| **CC6.3** | Security / Access Provisioning | Access is authorized and provisioned based on role-based access control (RBAC). | Partially Implemented | `tickets/access_request_sample.json` | Medium | Automate offboarding provisioning sync by 2026-10-15 |
| **CC7.1** | Security / Vulnerability Mgmt | Infrastructure vulnerabilities are scanned, identified, and remediated. | Implemented | `reports/vuln_scan_q3.csv` | Low | Monthly scans automated via AWS Inspector |
| **CC8.1** | Security / Change Management | Changes to production undergo formal testing, peer review, and approval. | Implemented | `prs/change_approval_log.md` | Low | Enforced via GitHub branch protection rules |
