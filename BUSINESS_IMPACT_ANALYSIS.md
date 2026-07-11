---
layout: default
title: Business Impact Analysis (BIA) & Continuity Matrix
nav_order: 1
---

# Business Impact Analysis (BIA) & Continuity Matrix

## 1. Executive Summary
This Business Impact Analysis (BIA) establishes recovery priorities, Recovery Time Objectives (RTO), and Recovery Point Objectives (RPO) for core organizational assets. The objective is to provide the Disaster Recovery (DR) and engineering teams with explicit business-driven operational targets following a disruptive event (e.g., ransomware, infrastructure failure).

## 📊 Core Business Impact Matrix

| System / Asset Name | Business Function | Operational Impact of Outage | Target RTO | Target RPO | Priority Tier |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Customer Billing System** | Processes customer payments and handles real-time transactions. | Immediate financial loss, severe reputational damage, and potential contractual SLA violations. | **4 Hours** | **1 Hour** | **Tier 1 (Critical)** |
| **Employee Payroll System** | Manages bi-weekly employee compensation and tax records. | Delayed payroll causing employee dissatisfaction and minor regulatory compliance reporting friction. | **72 Hours** | **24 Hours** | **Tier 2 (Medium)** |
| **Internal Knowledge Base (Wiki)** | Stores internal documentation, policy copies, and team wikis. | Decreased internal collaboration efficiency; workarounds are readily available via local files. | **7 Days** | **48 Hours** | **Tier 3 (Low)** |

## 📐 Definition of Metrics
* **Recovery Time Objective (RTO):** The maximum tolerable duration of downtime before acceptable operational degradation shifts into catastrophic business failure.
* **Recovery Point Objective (RPO):** The maximum acceptable age of data that can be permanently lost or must be manually re-entered following data restoration from backups.

## 🛡️ Continuity Strategy & Backup Mandates
1. **Tier 1 Infrastructure:** Must utilize highly available, multi-region hot-standby architectures with continuous data replication to satisfy the strict 1-hour RPO.
2. **Tier 2/3 Infrastructure:** Backups must be taken daily, encrypted at rest, and stored in an isolated, immutable cloud bucket (air-gapped from the primary production directory) to prevent lateral ransomware tampering.
