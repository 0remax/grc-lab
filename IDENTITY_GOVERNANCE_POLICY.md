---
layout: default
title: Identity Governance Policy
nav_order: 5
---
# Identity Governance Policy
Enforcing the Principle of Least Privilege (PoLP).

## Core Principles
* **Default-Deny:** All access is denied unless explicitly granted.
* **Access Reviews:** Mandatory quarterly reviews of all privileged user accounts to prevent privilege creep.

# Corporate Policy: Identity Governance & Access Control Baseline

## 1. Purpose
This policy defines the core principles governing user identity lifecycle management, provisioning, and authorization boundaries. The objective is to enforce the Principle of Least Privilege, prevent unauthorized internal data exposure, and mitigate the risk of lateral movement by insider threats.

## 2. Scope
This policy applies to all employees, contractors, third-party vendors, and service accounts requesting or holding access to internal enterprise environments, localized servers, and cloud directories.

## 3. Core Policy Statements

### 3.1 The Principle of Least Privilege (PoLP)
* **Default Deny:** All user accounts created within corporate directories (e.g., Active Directory, Okta, IAM) must default to a "no access" status. 
* **Minimum Operational Access:** Personnel shall only be granted the minimum system privileges and data access boundaries required to successfully perform their immediate, documented job functions.

### 3.2 Role-Based Access Control (RBAC) Architecture
Access to sensitive directories, file shares, and database schemas must be abstracted into predefined, role-specific security groups. 

| Standard Persona / Role | Permitted Access Boundaries | Restrictions & Prohibitions |
| :--- | :--- | :--- |
| **HR Specialist (Mid-Tier)** | Access to mid-level employee profiles, basic contact directories, and general benefit files. | Blocked from Executive payroll data, executive performance reviews, and corporate financial folders. |
| **Software Engineer** | Read/write access to code repositories and isolated staging/testing environments. | Strictly prohibited from accessing live customer production databases or root configurations. |
| **Financial Analyst** | Full read/write access to corporate accounting tools, invoice folders, and tax tracking. | Prohibited from accessing source code repositories or employee medical history documents. |

### 3.3 User Access Reviews (UAR)
* **Audit Cadence:** Business managers and the GRC team must conduct a formal User Access Review **quarterly** to audit privileges.
* **Revocation Policy:** Any identified "privilege creep" (e.g., historical access left over from a previous job role) must be automatically revoked within 5 business days of discovery.
