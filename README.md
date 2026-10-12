# Purpose
This is a living changelog of governance documents, compliance configuration, and risk assessment for the purpose of personal accountability and skill demonstration. Me, Me, &amp; Me, SP is an undocumented, sole proprietorship currently located in Louisiana and operating within cloud and on-prem environments. This repository will hold real documents to be used to govern the operations of my independent, professional, and personal endeavors. However, these public facing documents will be sanitized for privacy and security and will not contain any identifiable information of employees, clients, or entities unless otherwise approved in writing. Below is the internal and external structure of Me, Me, & Me, SP's documentation as identified and synthesized by AI.  

All documents in this repository are created using human and AI collaboration. To demonstrate remediation from a baseline, starting documents are generated and submit to this repository without review using the following prompt:

```
I want to create the starting documents of our organization. This will be the start of the portfolio and we will show my skills in
this portfolio by updating the documentation to the proper standards we need. I would like you to rewrite the documentation that
you've created, this time I'd like you to make the organization's governance and existing documentation based on the conversations
we've had in the past; the information that you know about my business(es), working style, and goals; usage and task history, and
the current setup of the OS, our existing MCP connections and tools, and organization (or disorganization) or my workstation.

Do not do documentation for ISO 42001, HIPAA, CMS, etc. Just make the ISMS documents and we will iterate from there. Since this will
be a portfolio, some if not all of these documents will be available in a GitHub repository. As such, we'll need CONFIDENTIAL and
PUBLIC versions of the documents you create. Public versions of documents should be free of any sensitive information, PII,
credentials, etc. All documents need to be in a Word, PDF, and markdown form.
```

Remediation will be documented as completed.

# Me & Me & Me, SP / Apex Cyber & Advisory, SP

**Governing Entity:** Me & Me & Me, SP (Sole Proprietorship, State of Louisiana)  
**Public Portfolio Alias:** Apex Cyber & Advisory, SP  
**Lead Auditor & Executive Principal:** Raquel Blue (Certified ISO/IEC 27001 Lead Auditor, Certified ISO/IEC 42001 Lead Auditor, Licensed Louisiana Medicare Insurance Producer, GRC Specialist)  
**Host Environment:** Hardened Windows 11 Pro Workstation (`[REDACTED]`)  
**Standard Baseline:** ISO/IEC 27001:2022 (Information Security, Cybersecurity and Privacy Protection)  
**Statutory Frameworks:** HIPAA Security & Privacy Rules (45 CFR §§ 160/164), CMS Regulations (42 CFR §§ 422/423), Louisiana Insurance Data Security Law (La. R.S. §§ 22:2501–2511), NIST AI RMF (SP 1270), ISO/IEC 42001:2023.

---

## 1. Executive Portfolio Overview

This directory contains the complete, audit-ready **ISO/IEC 27001:2022 Information Security Management System (ISMS) Documentation Suite** engineered for **Me & Me & Me, SP**. 

The enterprise operates as a high-assurance **Synthetic Enterprise**, combining the certified fiduciary governance of an executive Lead Auditor (Raquel Blue) with an autonomous eleven-department artificial intelligence workforce operating under deterministic Human-in-the-Loop (HITL), Maker-Checker, and Separation of Duties (SoD) frameworks.

### The Multi-Track Publication Architecture
To satisfy rigorous external certification audits while simultaneously providing a sanitized, defensible portfolio for public display, vendor assessment, and prospective client diligence, this suite is maintained in a **synchronized dual-track structure**:

```
isms/
├── README.md                                  # Portfolio index, architecture, and ISO mapping
├── scripts/
│   └── compile_isms_artifacts.py              # Multi-format compiler (.md -> .docx & .typ -> .pdf)
├── confidential/                              # Certified Internal Track (Real Names, Paths, Host)
│   ├── markdown/                              # Canonical version-controlled Markdown sources (5 docs)
│   ├── docx/                                  # Executive-styled Word documents with institutional palette
│   └── pdf/                                   # Publication-grade Typst compiled PDFs
└── public/                                    # Sanitized External Track (Normalized Aliases & Paths)
    ├── markdown/                              # Sanitized Markdown sources (5 docs)
    ├── docx/                                  # Executive-styled Word documents
    └── pdf/                                   # Publication-grade Typst compiled PDFs
```

---

## 2. Dual-Track Comparison Matrix

| Dimension | Confidential Track (`confidential/`) | Public Track (`public/`) |
| :--- | :--- | :--- |
| **Intended Audience** | Accredited Certification Bodies (CABs), State Insurance Regulators (LDI), CMS Auditors, Internal Audits. | Public GRC portfolio, prospective clients, commercial vendor reviews, open-source reference. |
| **Legal Entity** | `Me & Me & Me, SP` | `Apex Cyber & Advisory, SP` |
| **Principal Identity** | Raquel Blue (Lead Auditor, Licensed Medicare Agent) | Raquel B., Lead Auditor (GRC Specialist) |
| **Filesystem Paths** | Real host paths: `[REDACTED]` | Normalized paths: `[REDACTED]` |
| **Download Directory** | Real path: `[REDACTED]` | Normalized: `[REDACTED]` |
| **Communications** | Internal enterprise email & verified host routing | Masked: `governance@enterprise-isms.internal` |
| **Sensitive Records** | Explicit mapping to firewalled `medicare/` silo | Generalized to firewalled client/regulatory records silo |
| **Security Rigor** | 100% full technical and control specification | 100% full technical and control specification (identical controls) |

---

## 3. ISO/IEC 27001:2022 Document Index & Clause Mapping

The suite consists of five foundational governance documents comprehensively covering the standard:

| Document | Title | Primary ISO/IEC 27001:2022 Clauses & Controls | Key Subject Matter & Enforced Safeguards |
| :---: | :--- | :--- | :--- |
| **Doc 01** | **ISMS Scope & Context Document**<br>`01_ISMS_Scope_and_Context.md` | **Clause 4**<br>• 4.1 Org Context<br>• 4.2 Interested Parties<br>• 4.3 Scope Boundaries<br>• 4.4 ISMS Processes | • Internal & External issues (single-operator synthetic synergy, CMS, HIPAA, AI risks)<br>• Legal & Regulatory Register mapping<br>• Enclave boundaries (`[REDACTED]/Me & Me & Me, SP/`)<br>• Explicit Clause 4.3 carve-outs (Gaming, Discord, Steam, ring-0 anti-cheat drivers, `storytelling/` D&D sandbox)<br>• Regulated `medicare/` firewall isolation. |
| **Doc 02** | **Information Security Policy Manual**<br>`02_Information_Security_Policy.md` | **Clauses 5, 6 & 7**<br>• 5.1 Leadership<br>• 5.2 Policy Statement<br>• 5.3 RACI Roles<br>• 6.1 Risk Methodology<br>• 6.2 Objectives / KPIs | • Executive commitment statement by Lead Auditor Raquel Blue<br>• RACI governance matrix across all 11 synthetic departments<br>• Maker-Checker & Separation of Duties (SoD) framework<br>• Measurable security KPIs (zero ePHI spills, MTTD < 15 min, 100% BitLocker)<br>• 5x5 ISO 27005 risk assessment methodology. |
| **Doc 03** | **Acceptable Use Policy (AUP) — Workstation, AI & MCPs**<br>`03_Acceptable_Use_Policy.md` | **Annex A Controls**<br>• A.5.10 Acceptable Use<br>• A.8.1 Endpoint Devices<br>• A.8.7 Malware Protection<br>• A.8.9 Configuration<br>• A.8.12 Data Leakage | • Hardened Windows 11 host baseline (BitLocker XTS-AES-256, TPM 2.0, EDR)<br>• Subagent execution whitelist (`self`, `research`, `improvement_planner`, `script_auditor`, `system_troubleshooter`)<br>• Prompt injection defense & passive data boundary<br>• MCP token custody (Composio hub, Playwriter, env var storage)<br>• Download folder accumulation quarantine & 30-day purge<br>• OS root scratch script lifecycle & 48h eradication<br>• Approved SaaS roster (Notion, Trello, Obsidian, Google Workspace, GitHub, Vanta, Terraform). |
| **Doc 04** | **Information Classification & Handling Standard**<br>`04_Information_Classification_and_Handling_Standard.md` | **Annex A Controls**<br>• A.5.12 Classification<br>• A.5.13 Labelling<br>• A.5.14 Info Transfer<br>• A.8.10 Deletion<br>• A.8.11 Data Masking<br>• A.8.24 Cryptography | • Four-Tier Classification taxonomy: Public, Internal, Confidential-Business, Restricted-Silo<br>• LLM prompt data minimization & Safe Harbor pseudonymization<br>• Absolute ban on consumer LLM chatbots for Tier 3/4 data<br>• NIST SP 800-88 Rev 1 media sanitization (Clear, Purge, Destroy)<br>• Statutory retention schedules: CMS 10-year mandate for Medicare records (42 CFR § 422.504), IRS 7-year financial rules. |
| **Doc 05** | **Statement of Applicability (SoA) Baseline**<br>`05_Statement_of_Applicability.md` | **Clause 6.1.3 & Annex A**<br>• A.5 Organizational (37)<br>• A.6 People (8)<br>• A.7 Physical (14)<br>• A.8 Technological (34)<br>*(All 93 Controls)* | • Complete evaluation of all 93 Annex A controls<br>• 84 Fully Implemented controls<br>• 7 Scope-Constrained controls<br>• 2 Justified Exclusions (A.7.4 Physical monitoring of external facilities; A.8.30 Outsourced development)<br>• Detailed workstation-tailored implementation mechanisms for every single control. |

---

## 4. Multi-Format Compilation Pipeline

The suite includes an automated compilation engine located at `scripts/compile_isms_artifacts.py`.

```
                        +--------------------------------+
                        |  Markdown Sources (.md)        |
                        |  5 Confidential + 5 Public     |
                        +--------------------------------+
                                        |
                 +----------------------+----------------------+
                 |                                             |
                 v                                             v
   +---------------------------+                 +---------------------------+
   |  python-docx Engine       |                 |  Typst 0.11 Engine        |
   |  - Custom XML Borders     |                 |  - Typst Intermediate     |
   |  - Institutional Palette  |                 |  - Proportional Tables    |
   |  - Header / Footer Fields |                 |  - Dynamic Page Numbering |
   +---------------------------+                 +---------------------------+
                 |                                             |
                 v                                             v
   +---------------------------+                 +---------------------------+
   |  Word Documents (.docx)   |                 |  Publication PDFs (.pdf)  |
   |  10 Verified Artifacts    |                 |  10 Verified Artifacts    |
   +---------------------------+                 +---------------------------+
```

### Running the Compiler
To recompile all 20 artifacts from the markdown sources:
```powershell
python "[REDACTED]\Me & Me & Me, SP\isms\scripts\compile_isms_artifacts.py"
```

### Compiler Specifications:
* **DOCX Output:** Generates clean, corporate-styled Word documents featuring Navy `#1F4E79` and Steel `#2B6CB0` headings, white-on-navy table headers, alternating row fills (`#F7FAFC`), cell padding, blockquote left-callouts, code block shading, and running headers/footers with document IDs and classification tags.
* **PDF Output:** Compiles via the local Typst binary (`typst.exe`), utilizing native vector table rendering, automated page breaking, elegant running headers/footers (`Page X of Y`), and typography optimized for executive reading.

---

## 5. Workstation Hygiene & Security Boundary Summary

As evaluated in the ISMS Scope and Statement of Applicability, the host workstation enforces strict operational controls:

1. **Physical Host Baseline:** Windows 11 Pro 64-bit, BitLocker XTS-AES-256 full volume encryption, TPM 2.0 validation, Secure Boot enabled, Microsoft Defender Antivirus with Cloud Protection and Tamper Protection active.
2. **Download Accumulation Quarantine:** Inbound files landing in `Downloads/` are treated as quarantined until hash-verified and scanned with Microsoft Defender (`mpcmdrun.exe`). Unvetted installers are blocked from direct execution. A monthly purge cron maintains hygiene.
3. **Scratch Script Eradication:** Ad-hoc test scripts and throwaway snippets are strictly confined to designated `scratch/` directories and subject to automated eradication within 48 hours. The enterprise root workspace remains immutably clean.
4. **Regulated `medicare/` Silo Firewall:** General synthetic agents (`research`, `improvement_planner`, Claude Code runners) are strictly barred from indexing or reading the `medicare/` subfolder. Only dedicated HIPAA-attested execution routines with human-in-the-loop validation may access this silo.
5. **Recreational & Creative Carve-Outs:** Personal gaming (Steam, Epic, Discord, ring-0 anti-cheat drivers) and creative fiction (`storytelling/` D&D campaign notes) are formally carved out of the ISMS audit scope under Clause 4.3, residing in segregated directories with zero access to enterprise credentials or client records.

---

## 6. Document History & Revision Control

| Version | Date | Author / Title | Changes / Comments |
| :---: | :---: | :--- | :--- |
| **1.0** | October 12, 2026 | **Raquel Blue**, Certified ISO 27001 Lead Auditor | Initial formal authoring, dual-track bifurcation, and multi-format compilation of complete ISO/IEC 27001:2022 ISMS suite. |

*Approved and Adopted for Me & Me & Me, SP and Apex Cyber & Advisory, SP.*
