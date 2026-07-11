# Incident Response & Regulatory Notification Governance Matrix

## 1. Purpose
This governance playbook establishes the critical reporting timelines, regulatory obligations, and communications workflows required following a verified security incident or data breach. The objective is to bridge technical incident response with international and state compliance mandates.

## 📊 Regulatory Notification Matrix

| Incident Type / Scope | Impacted Data Class | Primary Applicable Regulation | Mandatory Reporting Window | Core Governance Actions Required |
| :--- | :--- | :--- | :--- | :--- |
| **Exfiltration of European Union (EU) Citizen Records** | Personally Identifiable Information (PII) | **GDPR (Article 33)** | **Within 72 Hours** | Notify the lead supervisory authority with details of the breach, likely consequences, and mitigation steps taken. |
| **Exfiltration of Electronic Health Records (EHR)** | Protected Health Information (PHI) | **HIPAA Breach Notification Rule** | **Within 60 Days** | Notify affected individuals and the HHS Secretary. If the breach affects $>500$ individuals, immediate prominent media notice is required. |
| **Compromise of Active Cardholder Transaction Data** | Primary Account Numbers (PAN) / CVV | **PCI-DSS (Req 12.10)** | **Immediate / Varies** | Alert the acquiring financial institution and major card brands (Visa/Mastercard) immediately; initiate an independent forensic audit. |

## 📐 Non-Technical Escalation Workflow
1. **Triage & Classification:** Upon technical confirmation of data exfiltration, the Incident Commander must immediately loop in the GRC and Legal Counsel teams.
2. **Evidence Preservation:** All system logs, firewall configurations, and data access records relating to the breach must be cryptographically hashed and preserved for regulatory auditing.
3. **Continuous Notification Updates:** If full breach details cannot be verified within the 72-hour window (e.g., under GDPR), a phased disclosure must be submitted to the regulator detailing the ongoing forensic investigation.
