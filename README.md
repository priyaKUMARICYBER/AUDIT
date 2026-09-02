# Botium Toys — Security Controls & Compliance Audit

## 📌 Project Overview

This project is a cybersecurity audit I conducted for **Botium Toys**, a fictional mid-sized toy retailer with an online storefront, physical retail location, and adjoining warehouse. The audit evaluates the organization's existing security posture against industry-standard controls and compliance frameworks, identifies gaps, and delivers prioritized recommendations to reduce risk.

This project demonstrates a foundational cybersecurity audit workflow: defining scope and goals, assessing assets, evaluating controls, checking compliance alignment, and communicating actionable recommendations to stakeholders.

> *Note: This was completed as part of a guided cybersecurity coursework exercise. In line with academic honor code policies, the original assignment templates/answer sheets are not reproduced here — this repo presents my own independent write-up of the audit process, findings, and recommendations.*

---

## 🎯 Scope & Goals

**Scope:** The entire security program at Botium Toys — including employee equipment/devices, the internal network, business systems (accounting, ecommerce, inventory management, telecommunications, database, security), and physical assets (storefront, warehouse).

**Goal:** Assess existing assets and controls, and determine which controls and compliance best practices need to be implemented to improve the organization's overall security posture.

---

## 🧩 Methodology

The audit followed a structured process aligned with the **NIST Cybersecurity Framework (CSF)**, starting with the *Identify* function:

1. **Asset inventory review** — cataloged all IT-managed assets (devices, systems, software, network, data storage, legacy systems).
2. **Risk assessment** — evaluated the impact and likelihood of risks tied to inadequate controls and non-compliance, resulting in a documented risk score.
3. **Controls assessment** — evaluated existing Administrative/Managerial, Technical, and Physical/Operational controls against control types (Preventative, Corrective, Detective, Deterrent).
4. **Compliance evaluation** — assessed alignment with **PCI DSS**, **GDPR**, and **SOC (Type 1/2)** requirements.
5. **Recommendations** — prioritized remediation steps based on risk severity.

---

## ⚠️ Key Findings

- **Overall Risk Score: 8/10** — driven primarily by a lack of access controls and incomplete compliance alignment.
- All employees currently have unrestricted access to internally stored data, including cardholder data and customer PII/SPII.
- No encryption is applied to stored or transmitted credit card data.
- No intrusion detection system (IDS), no disaster recovery plan, and no data backups are currently in place.
- Password policy exists but does not meet modern complexity standards, and there is no centralized password management system.
- Legacy systems are monitored, but without a defined schedule or clear intervention process.
- Physical security controls (locks, CCTV, fire detection/prevention) are strong and fully in place.

---

## ✅ Controls Assessment Summary

| Control | Status | Type |
|:---|:---:|:---|
| Password policies | ✅ In place (weak) | Preventative |
| Firewall | ✅ In place | Preventative |
| Antivirus software | ✅ In place | Preventative |
| Locks (offices/storefront/warehouse) | ✅ In place | Preventative |
| CCTV surveillance | ✅ In place | Preventative/Detective |
| Fire detection/prevention | ✅ In place | Detective/Preventative |
| Least privilege | ❌ Missing | Preventative |
| Separation of duties | ❌ Missing | Preventative |
| Disaster recovery plan | ❌ Missing | Corrective |
| Intrusion detection system (IDS) | ❌ Missing | Detective |
| Backups | ❌ Missing | Corrective |
| Encryption | ❌ Missing | Deterrent |
| Password management system | ❌ Missing | Preventative |
| Legacy system monitoring schedule | ❌ Undefined | Preventative |

## 📋 Compliance Summary

| Framework | Requirements Met | Requirements Not Met |
|:---|:---:|:---:|
| PCI DSS | 0 / 4 | 4 / 4 |
| GDPR | 2 / 4 | 2 / 4 |
| SOC (Type 1/2) | 2 / 4 | 2 / 4 |

---

## 🛠 Recommendations (Prioritized by Risk)

1. **Implement encryption** for cardholder data and **enforce least privilege / separation of duties** — closes the highest-risk PCI DSS and SOC gaps.
2. **Deploy an IDS** and establish **documented disaster recovery and backup procedures** to protect business continuity.
3. **Adopt a centralized password management system** and strengthen password policy requirements.
4. **Conduct a full asset inventory and classification exercise** (per NIST CSF *Identify*) so data — including E.U. customer data under GDPR — can be properly protected.
5. **Establish a regular monitoring and maintenance schedule** for legacy systems.

---

## 📚 Frameworks & Standards Referenced

- NIST Cybersecurity Framework (CSF)
- PCI DSS (Payment Card Industry Data Security Standard)
- GDPR (General Data Protection Regulation)
- SOC (System and Organization Controls, Type 1 & 2)

---

## 🧰 Skills Demonstrated

`Risk Assessment` · `Security Controls Evaluation` · `Compliance Auditing (PCI DSS, GDPR, SOC)` · `NIST CSF` · `Technical Writing & Reporting` · `Stakeholder Communication`
