# ISO/IEC 27001:2022 Information Classification & Handling Standard
**Document Identifier:** ISMS-PUB-04-CLS  
**Version:** 1.0  
**Effective Date:** October 12, 2026  
**Status:** Approved & Audit-Ready  
**Classification:** Public - External Version  
**Author / Executive Principal:** Raquel B. (Certified ISO/IEC 27001 Lead Auditor, Certified ISO/IEC 42001 Lead Auditor, GRC Specialist)  
**Governing Entity:** Apex Cyber & Advisory, SP (Sole Proprietorship)  
**Host Environment:** Windows 11 Pro Workstation (Secured Enclave: `C:\Users\<OPERATOR>\`)  
**Inquiries:** `governance@enterprise-isms.internal`  

---

## 1. Purpose & Standards Alignment

This Standard establishes the mandatory data classification scheme, labelling conventions, cryptographic protection requirements, storage lifecycles, and handling protocols for **Apex Cyber & Advisory, SP**.

This Standard directly implements controls pursuant to:
* **ISO/IEC 27001:2022 Annex A.5.12:** Classification of information.
* **ISO/IEC 27001:2022 Annex A.5.13:** Labelling of information.
* **ISO/IEC 27001:2022 Annex A.5.14:** Information transfer.
* **ISO/IEC 27001:2022 Annex A.8.10:** Information deletion.
* **ISO/IEC 27001:2022 Annex A.8.11:** Data masking.
* **ISO/IEC 27001:2022 Annex A.8.24:** Use of cryptography.
* **Statutory Healthcare & Consumer Rules:** Technical safeguards for personal data.
* **CMS Regulations (42 CFR § 422.504(d)):** 10-year record retention mandate.

---

## 2. Four-Tier Classification Taxonomy

Information assets across the enterprise are categorized into four distinct classification tiers based on the potential impact of unauthorized disclosure, alteration, or destruction:

```
+----------------------------------------------------------------------------------------------------+
|                                  4-TIER DATA CLASSIFICATION MATRIX                                 |
|                                                                                                    |
|  TIER 4: RESTRICTED - SILO (REST-PHI)                                                              |
|  - Impact: Catastrophic / Statutory fines, license revocation, breach reporting                    |
|  - Content: Beneficiary ePHI, MBIs, SSNs, Scope of Appointments, Recorded Consultations            |
|  - Storage: Encrypted Silo (medicare/) / App-layer AES-GCM-256 / Strictly ZDR Local or BAA AI      |
|                                                                                                    |
|  TIER 3: CONFIDENTIAL - BUSINESS (CONF-BUS)                                                        |
|  - Impact: Severe / Financial damage, competitive loss, breach of NDA                              |
|  - Content: General ledger, partner contracts, API tokens, security threat models                  |
|  - Storage: BitLocker Enclave / Least Privilege RBAC / Enterprise ZDR APIs Only                     |
|                                                                                                    |
|  TIER 2: INTERNAL (INT)                                                                            |
|  - Impact: Moderate / Operational disruption, internal friction                                    |
|  - Content: SOPs, departmental manifests, IT system inventories, internal meeting notes            |
|  - Storage: Enterprise Enclave / General Synthetic Agent Processing Permitted                      |
|                                                                                                    |
|  TIER 1: PUBLIC (PUB)                                                                              |
|  - Impact: None / Zero harm upon public exposure                                                   |
|  - Content: Published marketing collateral, GRC whitepapers, educational YouTube scripts           |
|  - Storage: Public release folders, website, external distribution                                 |
+----------------------------------------------------------------------------------------------------+
```

### 2.1 Tier 1: Public (PUB)
* **Definition:** Information that has been formally reviewed, approved, and released for public consumption. Unauthorized disclosure causes zero damage to enterprise operations, finances, or reputation.
* **Examples:** Approved marketing copy, public website pages, educational video scripts, published GRC whitepapers, statutory consumer disclaimers.
* **Labelling:** Optional; default classification for files stored in public release directories.

### 2.2 Tier 2: Internal (INT)
* **Definition:** Proprietary operational information intended solely for internal execution by the Lead Auditor and synthetic workforce. Not intended for public release, but unauthorized disclosure would cause minimal or moderate business friction without regulatory penalties.
* **Examples:** Department charters, Standard Operating Procedures (SOPs), IT infrastructure manifests, synthetic agent skill configurations, meeting notes, project roadmaps.
* **Labelling:** Header banner: `CLASSIFICATION: INTERNAL - APEX CYBER & ADVISORY, SP`.

### 2.3 Tier 3: Confidential - Business (CONF-BUS)
* **Definition:** Highly sensitive commercial, financial, strategic, and intellectual property assets. Unauthorized disclosure would cause severe financial harm, competitive injury, or legal liability.
* **Examples:** General ledger, banking credentials, partner commission agreements and remittances, proprietary AI prompt chaining logic, unfiled tax returns, NDAs, trade secrets, vulnerability scan findings.
* **Labelling:** Header banner: `CLASSIFICATION: CONFIDENTIAL - BUSINESS // PROPRIETARY`.

### 2.4 Tier 4: Restricted - Silo / ePHI / PII (REST-PHI)
* **Definition:** Strictly regulated personal and healthcare data protected under federal and state statutes. Unauthorized disclosure triggers mandatory breach notification protocols, state/federal fines, and potential license revocation.
* **Examples:** Beneficiary legal names, Social Security Numbers (SSNs), healthcare identifiers, dates of birth, medical histories, prescription drug lists, Scope of Appointment (SOA) signed forms, enrollment applications, telephonic encounter recordings and transcripts.
* **Labelling:** Mandatory prominent header: `CLASSIFICATION: RESTRICTED - ePHI / PII // STRICT STATUTORY CONTROLS APPLY`.

---

## 3. Classification & Handling Specifications Matrix

| Control Dimension | Tier 1: Public (PUB) | Tier 2: Internal (INT) | Tier 3: Confidential (CONF-BUS) | Tier 4: Restricted Silo (REST-PHI) |
| :--- | :--- | :--- | :--- | :--- |
| **Primary Custodian** | `08_marketing_sales` | `01_administration`, `04_it` | `01_administration`, `07_finance` | Raquel B. / Licensed Advisory Silo |
| **Physical / Logical Path** | `.../released/`, Web | Enclave root & depts | Enclave secure vaults | `C:\Users\<OPERATOR>\...\medicare\` |
| **Encryption at Rest** | Default filesystem | BitLocker (XTS-AES-256) | BitLocker + App/Vault AES-256 | BitLocker + App-level AES-GCM-256 |
| **Encryption in Transit** | HTTPS (TLS 1.2+) | TLS 1.3 / SSH v2 | TLS 1.3 with PFS | FIPS 140-3 validated TLS 1.3 (PFS) |
| **Access Rights** | Unrestricted | All authenticated agents | Need-to-know / Authenticated | Principal (Raquel B.) + HIPAA Silo Agent |
| **LLM Processing** | Any model / Web agent | Enterprise APIs / Local | Enterprise ZDR APIs / Local | **Local Offline Only OR Enterprise BAA** |
| **Consumer LLM Ingestion** | Permitted | Prohibited | **STRICTLY FORBIDDEN** | **ABSOLUTELY FORBIDDEN (Statutory Breach)** |
| **Retention Mandate** | Current version | 3 years post-obsolescence | 7 years (Tax / Financial) | **10 Years Mandatory (CMS 42 CFR § 422.504)** |
| **Sanitization Method** | Standard file delete | Single-pass zero overwrite | NIST SP 800-88 Clear | NIST SP 800-88 Purge / Crypto-Eradication |

---

## 4. Artificial Intelligence & LLM Prompt Data Minimization

The processing of enterprise data by artificial intelligence models introduces specific data spill risks governed under **ISO/IEC 42001:2023** and statutory privacy frameworks.

### 4.1 Permissible Model Routing
1. **Tier 1 (Public):** May be processed by any commercial, web-search, or open-source model.
2. **Tier 2 (Internal):** May be processed by enterprise API endpoints with verified "no model training on customer data" terms or locally executed models.
3. **Tier 3 (Confidential - Business):** Permitted only on enterprise Zero Data Retention (ZDR) endpoints or offline local models running in isolated memory.
4. **Tier 4 (Restricted - Silo / ePHI):** Strictly restricted to:
   - Locally deployed offline models running entirely on host hardware with disabled network sockets; OR
   - Enterprise cloud model providers with an active, fully executed **Business Associate Agreement (BAA)** and verified Zero Data Retention guarantees.
   - **Consumer AI Ban:** Under no circumstance shall Tier 3 or Tier 4 data ever be pasted into consumer web chatbots.

### 4.2 De-Identification & Pseudonymization Protocol
Before any client scenario or advisory optimization analysis is routed to an AI model:
1. **Safe Harbor Pseudonymization:** All direct identifiers must be sanitized:
   - Client Name $\rightarrow$ `CLIENT_ID_[RANDOM_UUID]`
   - Identifier Numbers $\rightarrow$ `ID_REDACTED`
   - Street Address $\rightarrow$ Generalized to 3-digit Zip Code / County
   - Exact Date of Birth $\rightarrow$ Age in years
2. **Re-identification Key Custody:** The lookup table mapping pseudo-IDs to real client identities must be encrypted using AES-GCM-256 and stored exclusively inside the firewalled `medicare/` silo, inaccessible to any external API or general subagent.

---

## 5. Media Sanitization & Disposal Standard (NIST SP 800-88 Rev 1)

When data reaches the end of its statutory lifecycle, or when hardware components are decommissioned, sanitization must follow **NIST Special Publication 800-88 Revision 1 (Guidelines for Media Sanitization)**:

```
+----------------------------------------------------------------------------------------------------+
|                                    MEDIA SANITIZATION PROTOCOL                                     |
|                                                                                                    |
|    [CLEAR]  ---> Logical Overwrite                                                                 |
|                  Applied to non-sensitive files, temporary scratch scripts, Tier 2 records.        |
|                  Action: Single-pass zero or random byte overwrite prior to unlinking.             |
|                                                                                                    |
|    [PURGE]  ---> Cryptographic Eradication & SSD ATA Secure Erase                                  |
|                  Applied to Tier 3 Confidential and Tier 4 Restricted Silo data.                   |
|                  Action: Destruction of AES-GCM encryption keys (instant crypto-shredding),        |
|                  followed by NVMe/SSD Cryptographic Erase or multi-pass overwrite.                 |
|                                                                                                    |
|    [DESTROY] ---> Physical Destruction                                                             |
|                  Applied to retired physical drives, USB tokens, or decommissioned host storage.   |
|                  Action: Physical degaussing, disintegration, incineration, or shredding.          |
+----------------------------------------------------------------------------------------------------+
```

* **Scratch & Temp Script Disposal:** Ephemeral test scripts and output artifacts in `scratch/` directories are sanitized using secure file unlinking with zero-fill.
* **Cryptographic Eradication:** For encrypted Tier 4 silos, deletion of the unique file/volume encryption key renders all underlying ciphertext permanently unrecoverable, satisfying NIST Purge requirements.

---

## 6. Mandatory Retention Schedules & Legal Holds

Apex Cyber & Advisory, SP strictly enforces retention schedules dictated by statutory authorities:

* **Regulated Healthcare & Beneficiary Records (Tier 4):** Pursuant to **CMS 42 CFR § 422.504(d)(2)(iii)**, all Scope of Appointment (SOA) forms, applications, telephonic encounter recordings, and electronic chat transcripts must be retained for **a minimum of ten (10) years** from the end of the calendar year in which they were created.
* **Financial & Tax Records (Tier 3):** All general ledgers, bank statements, commission remittances, and tax filings must be retained for **seven (7) years**.
* **ISMS Audit Evidence & Logs (Tier 2/3):** Compliance telemetry, internal audit reports, access logs, and management review minutes must be retained for **three (3) years** to support ISO/IEC 27001 surveillance and recertification cycles.
* **Legal Holds:** Upon receipt of formal notice of litigation, regulatory investigation, or carrier audit, the Lead Auditor shall issue an immediate Legal Hold suspending all automated purges and retention rollovers for relevant data categories.

---

## 7. Executive Endorsement

**Approved By:**

__________________________________________________  
**Raquel B.**, Executive Principal & Lead Auditor  
*ISO/IEC 27001 Lead Auditor | ISO/IEC 42001 Lead Auditor*  
*GRC Specialist*  
**Apex Cyber & Advisory, SP**  
**Date:** October 12, 2026
