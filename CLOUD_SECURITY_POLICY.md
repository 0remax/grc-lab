---
layout: default
title: README
nav_order: 2
---

# Information Security Policy: Cloud Storage & Access Control

## 1. Purpose
This policy establishes the minimum baseline security requirements for provisioning, configuring, and managing cloud-based storage assets. The objective is to mitigate data leakage risks, prevent unauthorized access, and ensure compliance with regulatory data protection requirements.

## 2. Scope
This policy applies to all cloud infrastructure environments (including but not limited to AWS, Azure, and Google Cloud Platform) owned, managed, or operated by this organization, as well as all personnel with architectural or administrative access to these environments.

## 3. Technical & Administrative Controls

### 3.1 Access Control & Exposure
* **Default Deny:** All cloud storage buckets and object storage containers must be configured to block public read/write access by default.
* **Explicit Exceptions:** Any cloud storage asset requiring public exposure for business operations must obtain a documented policy exception signed off by the GRC team and the CISO.

### 3.2 Identity & Access Management (IAM)
* **Mandatory MFA:** Multi-Factor Authentication (MFA) must be strictly enforced for all identity accounts accessing cloud management consoles and CLI interfaces.
* **Least Privilege:** Developer and administrative accounts must be provisioned with the minimum necessary permissions required to fulfill their job functions.

### 3.3 Vulnerability Remediation SLAs
When a cloud misconfiguration or vulnerability is identified via security scanning tools, the following Service Level Agreements (SLAs) for remediation apply:

| Vulnerability Severity | Definition | Remediation Window |
| :--- | :--- | :--- |
| **Critical** | Publicly exposed production data, unencrypted storage, or leaked root credentials. | **Within 24 Hours** |
| **Medium / Low** | Missing asset tags, legacy software versions, or internal misconfigurations. | **Within 30 Days** |

## 4. Enforcement
Non-compliance with this policy may result in the automated decommissioning of non-compliant cloud infrastructure, revocation of administrative access, and potential disciplinary action.
