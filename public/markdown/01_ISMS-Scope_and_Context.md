# ISO/IEC 27001:2022 ISMS Scope & Context Document
**Document Identifier:** ISMS-PUB-01-SCP  
**Version:** 1.0  
**Effective Date:** October 12, 2026  
**Status:** Approved & Audit-Ready  
**Classification:** Public - External Version  
**Author / Executive Principal:** Raquel B. (Certified ISO/IEC 27001 Lead Auditor, Certified ISO/IEC 42001 Lead Auditor, GRC Specialist)  
**Governing Entity:** Apex Cyber & Advisory, SP (Sole Proprietorship)  
**Host Environment:** Windows 11 Pro Workstation (Secured Enclave: `C:\Users\<OPERATOR>\`)  
**Inquiries:** `governance@enterprise-isms.internal`  

---

## 1. Executive Summary & Purpose

This document formally establishes the organizational context, interested party requirements, physical and logical boundaries, interfaces, and explicit exclusions of the Information Security Management System (ISMS) for **Apex Cyber & Advisory, SP** in strict alignment with **ISO/IEC 27001:2022 Clauses 4.1, 4.2, 4.3, and 4.4**.

Apex Cyber & Advisory, SP operates as a high-assurance **Synthetic Enterprise**. The enterprise unifies the executive fiduciary oversight of a credentialed GRC professional (Raquel B., Lead Auditor) with an autonomous eleven-department agentic workforce operating under a deterministic Human-in-the-Loop (HITL), Maker-Checker, and Separation of Duties (SoD) framework.

This Scope & Context document serves as the public reference for external conformity assessment bodies, commercial partners, prospective clients, and regulatory authorities evaluating the enterprise security posture.

---

## 2. Clause 4.1: Understanding the Organization and Its Context

Apex Cyber & Advisory, SP systematically analyzes external and internal factors influencing the achievement of ISMS objectives.

### 2.1 Organizational Mission and Operational Model
* **Legal Entity:** Apex Cyber & Advisory, SP (Specialized Sole Proprietorship).
* **Principal / Lead Auditor:** Raquel B., Lead Auditor.
* **Core Business Activities:**
  1. **GRC & AI Advisory:** Enterprise information security architecture, ISO/IEC 27001 and ISO/IEC 42001 audit readiness, and continuous compliance automation.
  2. **Regulated Insurance & Healthcare Advisory:** Professional brokerage, advisory, and enrollment services operating under statutory health marketing regulations.
  3. **Synthetic Agent Architecture & Orchestration:** Engineering, auditing, and executing autonomous multi-agent workflows, model evaluation harnesses, and secure Model Context Protocol (MCP) tool integrations.

### 2.2 External Issues and Environmental Drivers
* **Healthcare & Consumer Regulatory Mandates:** Compliance with federal and state privacy statutes (HIPAA Security & Privacy Rules 45 CFR Parts 160/164, CMS Marketing Regulations 42 CFR §§ 422/423, and State Insurance Data Security Laws), requiring strict data protection and up to 10-year audit trail retentions.
* **AI Governance & Emerging Threat Landscape:** Rapidly evolving regulatory frameworks (EU AI Act, FTC Act Section 5, NIST AI RMF, ISO/IEC 42001:2023). External risk vectors include direct and indirect prompt injection, API credential exposure, software supply chain tampering, and automated tool hallucination.
* **Cloud & SaaS Supply Chain Dependencies:** Engagement of commercial cloud model foundries (Anthropic, OpenAI, Google Cloud Vertex AI), orchestration middleware (Composio hub, Playwriter), and enterprise SaaS platforms (Google Workspace, Notion, GitHub, Vanta, ServiceNow, Terraform, Squarespace).

### 2.3 Internal Issues and Organizational Drivers
* **Single-Operator Synthetic Synergy:** The enterprise is steered by a single executive principal who directs eleven autonomous, role-segregated synthetic departments. This creates high operational agility while demanding rigid logical access controls, cryptographic separation, and Maker-Checker validation to prevent single-point-of-failure or unauthorized autonomous execution.
* **Hardened Workstation Environment:** The operational host is an enterprise-grade Windows 11 workstation (`C:\Users\<OPERATOR>\`) running the primary AI Operating System enclave, Antigravity runtime, Claude Code CLI, Python SDK, and connected MCP daemons alongside productivity and development applications.
* **Segregated Workloads:** Multiple functional domains coexist on the physical host, requiring rigid directory enclaves and firewalling to isolate regulated client records, enterprise GRC data, development workspaces, and personal recreational sandboxes.

---

## 3. Clause 4.2: Understanding the Needs and Expectations of Interested Parties

The enterprise maintains an active Legal & Regulatory Register mapping interested party expectations to internal security controls:

| Interested Party | Category | Needs & Expectations | Mandatory Requirements & References |
| :--- | :--- | :--- | :--- |
| **Clients & Beneficiaries** | External / Data Subjects | Absolute confidentiality of PII/PHI, transparent consent, accurate advisory representations. | Statutory Privacy Rules (HIPAA / State Insurance Codes); Zero-Spill Standard. |
| **Federal & State Regulators** | External / Regulators | Fiduciary compliance, statutory disclaimers, required record retention, zero deceptive marketing. | 42 CFR § 422.2267; Insurance Data Security Laws; NAIC Standards. |
| **Carriers & Partners** | External / Business Partners | Protection of proprietary contracts, portal credential integrity, strict compliance with BAAs. | Business Associate Agreements (BAAs); Commercial Partner NDAs. |
| **Conformity Assessment Bodies (CABs)** | External / Certifiers | Objective audit evidence, transparent Statement of Applicability (SoA), verifiable internal audit cycles. | ISO/IEC 27001:2022; ISO/IEC 17021-1; ISO/IEC 27006. |
| **AI Model Foundries & Cloud Vendors** | External / Sub-processors | Adherence to Acceptable Use Policies, API quota compliance, zero prompt injection exploitation. | Commercial API Terms of Service, Enterprise Zero Data Retention (ZDR) Terms. |
| **Raquel B. (Lead Auditor / Principal)** | Internal / Governance | Defensible risk posture, audit readiness, operational resilience, automated compliance workflows. | ISMS Objectives; Enterprise Charter; Executive Accountability. |
| **Synthetic Agent Workforce (`01`-`11`)** | Internal / Synthetic Assets | Deterministic instruction boundaries, authenticated tool tokens, isolated execution memory, clear error-recovery. | Agent Charters; Departmental SOPs; Antigravity Runtime Policies. |

---

## 4. Clause 4.3: Determining the Scope of the ISMS

### 4.1 Physical and Logical Boundary Definition

The formal scope of the Apex Cyber & Advisory, SP ISMS encompasses all information assets, synthetic agents, automated workflows, development toolchains, customer data repositories, and supporting logical infrastructure operating within the dedicated enterprise enclave:

```
C:\Users\<OPERATOR>\.gemini\OS\Apex Cyber & Advisory, SP\
```
*(and upon planned enterprise root graduation, directly within: `C:\Users\<OPERATOR>\.gemini\OS\`)*

#### In-Scope Departmental Subsystems:
1. `01_administration_executive`: Executive decision records, strategic roadmaps, corporate charter.
2. `02_legal_compliance`: Legal registers, regulatory filings, BAA agreements, contractual covenants.
3. `03_security`: ISMS policies, vulnerability scan reports, threat models, incident logs, access control lists.
4. `04_information_technology`: Workstation configuration scripts, patch logs, infrastructure manifests.
5. `05_agentic_resources`: Agent manifests, prompt templates, system instructions, model routing policies.
6. `06_operations`: Daily execution schedules, operational monitoring logs, delivery workflows.
7. `07_accounting_finance`: General ledgers, tax filings, partner commission statements, banking integrations.
8. `08_marketing_sales`: Educational breakdowns, published GRC whitepapers, approved marketing collateral.
9. `09_customer_service`: Client intake logs, appointment disclaimers, support workflows.
10. `10_research_development`: Benchmark harnesses, prototype scripts, agent skill experiments.
11. `11_human_resources`: Synthetic role descriptions, performance audit logs, human training records.
12. `governance/` and `isms/`: Root governance vault, ISO policies, Statement of Applicability, audit trails.

#### In-Scope Workstation Tools & Integration Endpoints:
* **Operating System & Runtime:** Windows 11 Pro (`C:\Users\<OPERATOR>\`), Antigravity IDE, Claude Code CLI, Python 3.12+ execution environments.
* **Autonomous Subagents:** `self`, `research`, `improvement_planner`, `script_auditor`, `system_troubleshooter`.
* **Model Context Protocol (MCP) Daemons:** Composio hub, Playwriter, and associated authenticated sidecar processes.
* **Enterprise Productivity & GRC Cloud Services:** Google Workspace (Gmail, Drive), Notion (workspace vault), Trello, BlitzIt, Taska, Obsidian (local knowledge base), iOS Journal (mobile encrypted endpoint), GitHub (version-controlled repositories), Squarespace (web hosting), Vanta (automated GRC monitoring), ServiceNow (change tracking), Terraform (IaC).

---

### 4.2 Explicit Boundary Carve-Outs and Sandbox Justifications

Pursuant to ISO/IEC 27001:2022 Clause 4.3, an organization has the explicit prerogative to determine its ISMS boundaries provided that exclusions do not impact its ability to meet security requirements or satisfy customer expectations.

```
+----------------------------------------------------------------------------------------------------+
|                                    PHYSICAL HOST WORKSTATION                                       |
|                                       Windows 11 Pro 64-bit                                        |
|                                                                                                    |
|  +------------------------------------------------------+  +------------------------------------+  |
|  |             ENTERPRISE OS ENCLAVE (IN-SCOPE)         |  |   PERSONAL RECREATION (EXCLUDED)   |  |
|  |  C:\Users\<OPERATOR>\.gemini\OS\Apex Cyber\          |  |   D:\Games\, Steam, Epic, Discord  |  |
|  |                                                      |  |   Ring-0 Anti-Cheat Drivers        |  |
|  |  * 11 Departmental Agent Subsystems                 |  |   Personal Browsing & Streaming    |  |
|  |  * Central Governance & ISO 27001 ISMS Vault         |  |                                    |  |
|  |  * Antigravity IDE, Claude Code, Python SDK          |  |  +--------------------------------+  |
|  |  * MCP Daemons (Composio, Playwriter)                |  |  | CREATIVE SANDBOX (EXCLUDED)    |  |
|  |  * FIDO2 Enterprise Tokens, Cloud Workspaces         |  |  | storytelling/ (Creative Fiction)|  |
|  |                                                      |  |  | Zero Client PII / Zero Keys    |  |
|  |  +------------------------------------------------+  |  |  +--------------------------------+  |
|  |  | FIREWALLED SUB-ENCLAVE: medicare/              |  |  |                                    |  |
|  |  | Restricted Tier 4 ePHI / PHI Silo              |  |  |  STRICT CARVE-OUT:                 |  |
|  |  | Isolated from general synthetic agents         |  |  |  - No access to ISMS Enclave       |  |
|  |  +------------------------------------------------+  |  |  - Zero ePHI, zero API secrets     |  |
|  +------------------------------------------------------+  +------------------------------------+  |
|                             \                                                /                     |
|                              === ENCLAVE SECURITY BOUNDARY (ISOLATION) ======                      |
|                                  BitLocker XTS-AES-256 / TPM 2.0 / Defender EDR                    |
+----------------------------------------------------------------------------------------------------+
```

#### Carve-Out 1: Personal Recreation, Gaming, and Kernel Anti-Cheat Drivers
* **Excluded Assets:** Personal gaming software, launchers, personal communications platforms (e.g., Discord), personal streaming media, and third-party ring-0 kernel-level anti-cheat drivers residing outside the enterprise path (e.g., `D:\Games\`).
* **Technical Justification:** These applications serve zero enterprise commercial function. To prevent compliance contamination, the enterprise enclave enforces strict logical filesystem separation, dedicated browser profiles, and zero credential cross-pollination.
* **Host Baseline Hygiene:** While excluded from the ISMS audit scope, the underlying host workstation maintains robust baseline defenses: hardware-backed TPM 2.0 validation, full volume BitLocker XTS-AES-256 encryption, Microsoft Defender Antivirus with Cloud-Delivered Protection, and Secure Boot enabled.

#### Carve-Out 2: Creative Storytelling and Sandbox (`storytelling/`)
* **Excluded Assets:** Local creative writing repositories, tabletop campaign notes, character sheets, and unmanaged draft fiction residing in dedicated non-production folders (`storytelling/`).
* **Technical Justification:** These files represent pure creative fictional assets. They contain zero customer data, zero beneficiary ePHI, zero enterprise financial details, and zero API credentials. They are decoupled from the 11 departmental operational workflows.

#### Mandatory Firewalled Sub-Enclave: Regulated Healthcare Records Silo (`medicare/`)
* **Status:** In-scope for enterprise regulatory compliance, but **strictly isolated** from general-purpose synthetic agents.
* **Control Mechanism:** The `medicare/` data silo contains Tier 4 Restricted ePHI/PII. General synthetic subagents (`research`, `improvement_planner`, general Claude Code runners) are strictly prohibited from indexing, ingesting, or scanning this directory. Only dedicated HIPAA-attested execution routines under direct, real-time Human-in-the-Loop oversight by the Lead Auditor may access this silo.

---

## 5. Clause 4.4: Information Security Management System

Apex Cyber & Advisory, SP has established, implements, maintains, and continually improves an ISMS in accordance with ISO/IEC 27001:2022.

### 5.1 Process Interactions and Continuous Lifecycle
The ISMS follows the deterministic **Plan-Do-Check-Act (PDCA)** model adapted for an autonomous synthetic enterprise:

```
[PLAN] 
  - Risk Assessment & Treatment (ISO 27001 Cl. 6.1)
  - Security Objectives & KPI Formulation (Cl. 6.2)
  - Statement of Applicability (SoA) Baselines
         |
         v
[DO] 
  - Implementation of Annex A Controls (A.5 through A.8)
  - Enclave Isolation & Agent Invocation Whitelisting
  - Data Classification Marking & Token Sanitization
         |
         v
[CHECK] 
  - Continuous Monitoring via Vanta & Windows Defender EDR
  - Department 03_security Internal Audits (Cl. 9.2)
  - Lead Auditor Formal Management Review (Cl. 9.3)
         |
         v
[ACT] 
  - Nonconformity Corrective Action Tracking (Cl. 10.1)
  - Departmental SOP Refinements & Continuous Learning (Cl. 10.2)
  - Re-alignment of Risk Register & Model Guardrails
```

### 5.2 Verification and Document Control
* This document is maintained under version control in the central `governance/` and `isms/` repositories.
* Formal review occurs annually or immediately upon major architectural modification to the workstation, changes in statutory mandates, or integration of new autonomous agent capabilities.

---

## 6. Document Sign-Off & Executive Approval

**Approved and Formally Adopted By:**

__________________________________________________  
**Raquel B.**, Executive Principal & Lead Auditor  
*ISO/IEC 27001 Lead Auditor (IRCA/PECB Equivalent)*  
*ISO/IEC 42001 Lead Auditor | GRC Specialist*  
**Apex Cyber & Advisory, SP**  
**Date:** October 12, 2026
