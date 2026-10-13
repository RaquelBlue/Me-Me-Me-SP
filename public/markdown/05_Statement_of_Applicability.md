# ISO/IEC 27001:2022 Statement of Applicability (SoA) Baseline
**Document Identifier:** ISMS-PUB-05-SOA  
**Version:** 1.0  
**Effective Date:** October 12, 2026  
**Status:** Approved & Audit-Ready  
**Classification:** Public - External Version  
**Author / Executive Principal:** Raquel B. (Certified ISO/IEC 27001 Lead Auditor, Certified ISO/IEC 42001 Lead Auditor, GRC Specialist)  
**Governing Entity:** Apex Cyber & Advisory, SP (Sole Proprietorship)  
**Host Environment:** Windows 11 Pro Workstation (Secured Enclave: `C:\Users\<OPERATOR>\`)  
**Inquiries:** `governance@enterprise-isms.internal`  

---

## 1. Executive Overview & Methodology

This Statement of Applicability (SoA) documents the evaluation, applicability decisions, justifications, and implementation mechanisms for all **93 security controls** specified in **ISO/IEC 27001:2022 Annex A**.

As an audit-ready **Synthetic Enterprise**, Apex Cyber & Advisory, SP operates under a hybrid control framework bridging physical workstation security, enterprise cloud SaaS governance, and autonomous multi-agent AI execution pipelines. Each control has been assessed against the enterprise risk profile, statutory healthcare requirements (HIPAA, CMS 42 CFR §§ 422/423), state data security laws, and the operational boundaries established in `01_ISMS_Scope_and_Context.md`.

### Applicability Summary
* **Total Annex A Controls:** 93
* **Applicable (Fully Implemented):** 84
* **Partially Applicable (Scope Constrained):** 7
* **Justified Exclusions:** 2 (A.7.4 Physical monitoring of external facilities; A.8.30 Outsourced development)

---

## 2. Section A.5: Organizational Controls (37 Controls)

| Control ID | Control Name | Applicability | Justification for Inclusion / Exclusion | Implementation Mechanism & Workstation Control (Apex Cyber & Advisory, SP) | Status |
| :--- | :--- | :---: | :--- | :--- | :---: |
| **A.5.1** | Policies for information security | Applicable | Core ISMS governance mandate. | Formal policy suite authored by Lead Auditor Raquel B. (`ISMS-PUB-01` through `05`), reviewed annually. | Implemented |
| **A.5.2** | Information security roles & responsibilities | Applicable | Defines accountability across principal and agents. | RACI matrix defined in Doc 02; Raquel B. holds executive fiduciary role; 11 synthetic departments assigned operational charters. | Implemented |
| **A.5.3** | Segregation of duties | Applicable | Prevents unilateral unauthorized actions or fraud. | Maker-Checker protocol: synthetic agents draft/propose; human principal or automated gate must verify before external action or financial execution. | Implemented |
| **A.5.4** | Management responsibilities | Applicable | Leadership engagement and compliance enforcement. | Direct fiduciary oversight by Raquel B.; continuous monitoring via Vanta and Antigravity execution transcripts. | Implemented |
| **A.5.5** | Contact with authorities | Applicable | Required for regulatory reporting and breach response. | Documented contact protocols with State Insurance Regulators, CMS, OCR, and local law enforcement. | Implemented |
| **A.5.6** | Contact with special interest groups | Applicable | Threat intelligence and professional competence. | Active membership in ISO/IEC TC JTC1/SC27 mirror groups, GRC associations, and cybersecurity professional bodies. | Implemented |
| **A.5.7** | Threat intelligence | Applicable | Proactive defense against evolving AI & cyber threats. | Weekly automated ingestion of CISA advisories, OWASP LLM Top 10 updates, and model vendor vulnerability bulletins via Dept 03. | Implemented |
| **A.5.8** | Information security in project management | Applicable | Integrates security into development and GRC sprints. | Security reviews embedded into all departmental sprint roadmaps, script developments, and model deployment pipelines. | Implemented |
| **A.5.9** | Inventory of information and other associated assets | Applicable | Visibility of all enterprise assets and models. | Comprehensive asset inventory maintained across hardware, cloud tenants, agent manifests, and data repositories. | Implemented |
| **A.5.10** | Acceptable use of information and other associated assets | Applicable | Controls user and agent actions on enterprise assets. | Acceptable Use Policy (`ISMS-PUB-03-AUP`) enforced across Windows 11 host, mobile endpoints, SaaS tools, and MCP daemons. | Implemented |
| **A.5.11** | Return of assets | Applicable | Asset protection upon relationship termination. | Offboarding checklists for cloud API keys, SaaS seats, and contractor credentials (if any engaged). | Implemented |
| **A.5.12** | Classification of information | Applicable | Mandatory taxonomy for data protection. | Four-tier classification standard (Public, Internal, Confidential-Business, Restricted-Silo) defined in `ISMS-PUB-04-CLS`. | Implemented |
| **A.5.13** | Labelling of information | Applicable | Ensures clear sensitivity markings on all assets. | Header/metadata classification banners enforced in markdown, code manifests, and outbound client deliverables. | Implemented |
| **A.5.14** | Information transfer | Applicable | Safeguards data moving across network boundaries. | TLS 1.3 enforced for all web APIs; encrypted email gateways; zero unencrypted data transfer. | Implemented |
| **A.5.15** | Access control | Applicable | Restricts unauthorized access to systems and data. | Least-privilege NTFS ACLs on Windows 11; multi-factor authentication (MFA) on all SaaS portals; API token segregation. | Implemented |
| **A.5.16** | Identity management | Applicable | Unique identification and lifecycle tracking. | Unique user accounts on Windows 11; enterprise passkeys; discrete agent execution IDs in Antigravity runtime. | Implemented |
| **A.5.17** | Authentication information | Applicable | Protects passwords, passkeys, and cryptographic keys. | Password manager vault for secret custody; biometric authentication; FIDO2 physical security keys. | Implemented |
| **A.5.18** | Access rights | Applicable | Dynamic provisioning and revocation of access. | Quarterly access reviews conducted by Raquel B. across GitHub, Google Workspace, cloud foundries, and Vanta. | Implemented |
| **A.5.19** | Information security in supplier relationships | Applicable | Vendor risk management across AI & SaaS providers. | Formal vendor security evaluations for Anthropic, OpenAI, Google Cloud, Composio, Vanta, and Squarespace. | Implemented |
| **A.5.20** | Addressing information security within supplier agreements | Applicable | Enforces contractual security commitments. | Executed Business Associate Agreements (BAAs) with cloud providers; enterprise terms with zero data retention clauses for AI APIs. | Implemented |
| **A.5.21** | Managing information security in the ICT supply chain | Applicable | Protects against software supply chain poisoning. | GitHub Dependabot vulnerability scanning; pip requirements lockfiles; local scanning of agent skills via `scan-skill`. | Implemented |
| **A.5.22** | Monitoring, review and change management of supplier services | Applicable | Continuous oversight of third-party SLAs and security. | Monthly audit of SaaS SOC 2 Type II reports and API uptime/security notices via Dept 04. | Implemented |
| **A.5.23** | Information security for use of cloud services | Applicable | Secures cloud configurations and shared responsibility. | Cloud hardening baselines; Terraform IaC drift detection; MFA enforcement across all cloud administrative consoles. | Implemented |
| **A.5.24** | Information security incident management planning and preparation | Applicable | Preparation for prompt detection and containment. | Incident Response Plan (`03_security/incident_response/`) establishing roles, severity levels, and automated alerting channels. | Implemented |
| **A.5.25** | Assessment and decision on information security events | Applicable | Triage and severity assignment for anomalies. | Event classification protocol assessing CIA impact, regulatory breach triggers, and escalation paths. | Implemented |
| **A.5.26** | Response to information security incidents | Applicable | Containment, eradication, and recovery procedures. | Standardized containment runbooks: network isolation, API key revocation, process termination via EDR, forensic snapshotting. | Implemented |
| **A.5.27** | Learning from information security incidents | Applicable | Post-incident reviews and root-cause remediation. | Mandatory Post-Mortem Incident Review reports stored in `03_security/incident_response/` within 5 business days of incident closure. | Implemented |
| **A.5.28** | Collection of evidence | Applicable | Forensic integrity and chain of custody. | Windows Event Logs, Antigravity execution transcripts (`transcript.jsonl`), and git commit histories preserved immutably. | Implemented |
| **A.5.29** | Information security during disruption | Applicable | Business continuity and operational resilience. | Decentralized git backups, cloud mirror repositories, offsite encrypted cold backups of critical vaults. | Implemented |
| **A.5.30** | ICT readiness for business continuity | Applicable | High availability and recovery time objectives. | Recovery Time Objective (RTO) < 4 hours; Recovery Point Objective (RPO) < 24 hours verified via quarterly restoration drills. | Implemented |
| **A.5.31** | Legal, statutory, regulatory and contractual requirements | Applicable | Core compliance obligation across healthcare & AI. | Comprehensive Legal & Regulatory Register maintained in `governance/Legal_Regulatory_Register.md`. | Implemented |
| **A.5.32** | Intellectual property rights | Applicable | Protection of enterprise IP and third-party licenses. | Copyright notices on proprietary agent architectures; strict adherence to open-source software licenses (MIT/Apache 2.0). | Implemented |
| **A.5.33** | Protection of records | Applicable | Statutory retention and tamper-resistance. | CMS 10-year retention rule for regulated records; tax 7-year retention; immutable cloud storage with object lock. | Implemented |
| **A.5.34** | Privacy and protection of PII | Applicable | Protection of personal and health data. | Statutory Privacy compliance; strict pseudonymization of client details before AI ingestion; firewalled records silo. | Implemented |
| **A.5.35** | Independent review of information security | Applicable | Objective audit verification of ISMS. | Annual independent external ISO/IEC 27001 surveillance audits conducted by accredited Conformity Assessment Body. | Implemented |
| **A.5.36** | Compliance with policies and standards for information security | Applicable | Internal verification of procedural adherence. | Continuous automated checks via Vanta; internal audit reviews conducted semi-annually by Lead Auditor Raquel B. | Implemented |
| **A.5.37** | Documented operating procedures | Applicable | Repeatable, secure operational execution. | Comprehensive Standard Operating Procedures (SOPs) maintained in each of the 11 departmental workspaces. | Implemented |

---

## 3. Section A.6: People Controls (8 Controls)

| Control ID | Control Name | Applicability | Justification for Inclusion / Exclusion | Implementation Mechanism & Workstation Control (Apex Cyber & Advisory, SP) | Status |
| :--- | :--- | :---: | :--- | :--- | :---: |
| **A.6.1** | Screening | Applicable | Trustworthiness verification of personnel. | Comprehensive background screening, credential verification, and professional background checks for Principal. | Implemented |
| **A.6.2** | Terms and conditions of employment | Applicable | Legal confidentiality and security obligations. | Fiduciary covenants documented in Enterprise Charter; contractor agreements incorporate mandatory NDAs and security schedules. | Implemented |
| **A.6.3** | Information security awareness, education and training | Applicable | Ongoing human and agent competence. | Annual healthcare compliance certifications for Principal; continuous alignment prompts and skill testing for synthetic agents. | Implemented |
| **A.6.4** | Disciplinary process | Applicable | Consequences for policy violations. | Formal escalation framework: agent skill deprecation/quarantine for agent failures; regulatory self-reporting for human non-compliance. | Implemented |
| **A.6.5** | Responsibilities after termination or change of employment | Applicable | Post-employment asset and secret protection. | Revocation checklists for third-party access; permanent non-disclosure obligations enforced under applicable contract law. | Implemented |
| **A.6.6** | Confidentiality or non-disclosure agreements | Applicable | Contractual confidentiality enforcement. | Mutual NDAs executed with all enterprise consulting clients, commercial partners, and third-party service providers. | Implemented |
| **A.6.7** | Remote working | Applicable | Secures home office / mobile operations. | Hardened office environment; VPN / secure TLS connections; no public Wi-Fi usage without encrypted tunnel; physical screen privacy. | Implemented |
| **A.6.8** | Information security event reporting | Applicable | Timely reporting of security anomalies. | Automated alerting channels to Principal; instant incident logging in `03_security/incident_response/`. | Implemented |

---

## 4. Section A.7: Physical Controls (14 Controls)

| Control ID | Control Name | Applicability | Justification for Inclusion / Exclusion | Implementation Mechanism & Workstation Control (Apex Cyber & Advisory, SP) | Status |
| :--- | :--- | :---: | :--- | :--- | :---: |
| **A.7.1** | Physical security perimeters | Applicable | Secures primary operational premises. | Physical perimeter security of primary office premises: deadbolts, exterior perimeter cameras, alarm system. | Implemented |
| **A.7.2** | Physical entry | Applicable | Restricts unauthorized physical access. | Keycard / physical key control; visitors logged and escorted; zero unescorted access to workstation hardware. | Implemented |
| **A.7.3** | Securing offices, rooms and facilities | Applicable | Secures specific rooms housing hardware. | Dedicated office suite locked when unoccupied; workstation positioned away from exterior-facing windows. | Implemented |
| **A.7.4** | Physical monitoring | Justified Exclusion | Excluded for external cloud facilities; residential environment. | **Justified Exclusion:** Primary host workstation is housed in a private secured office; physical monitoring of external cloud data centers is delegated to SOC 2 Type II certified providers. | Excluded |
| **A.7.5** | Protecting against physical and environmental threats | Applicable | Protects against fire, surge, and weather. | Surge-protected Uninterruptible Power Supply (UPS); smoke detectors; climate-controlled environment. | Implemented |
| **A.7.6** | Working in secure areas | Applicable | Prevents eavesdropping and visual snooping. | Workstation screen privacy filters; strict rule prohibiting client telephonic encounters in public spaces. | Implemented |
| **A.7.7** | Clear desk and clear screen | Applicable | Prevents unauthorized visual observation. | Automatic 10-minute workstation screen lock; zero physical paper storage of client data (100% digital encrypted enclave). | Implemented |
| **A.7.8** | Equipment siting and protection | Applicable | Minimizes environmental and physical hazards. | Workstation sited off-floor on stabilized desk; cable management; protected from liquid hazards. | Implemented |
| **A.7.9** | Security of assets off-premises | Applicable | Protects mobile devices outside office. | Mobile devices encrypted with biometrics/passcode; remote wipe enabled via device management. | Implemented |
| **A.7.10** | Storage media | Applicable | Secures removable media from tampering/theft. | USB storage drives restricted; any authorized removable media must be encrypted with AES-256. | Implemented |
| **A.7.11** | Supporting utilities | Applicable | Ensures reliable power and network feed. | Dual-line internet connectivity (primary fiber + cellular hotspot fallback); battery backup UPS. | Implemented |
| **A.7.12** | Cabling security | Applicable | Protects network and power wiring. | Internal conduit and interior routing for power and ethernet cabling; zero exposed exterior network cabling. | Implemented |
| **A.7.13** | Equipment maintenance | Applicable | Prevents hardware degradation and failure. | Scheduled hardware diagnostics, dust eradication, thermal monitoring via host hardware utilities. | Implemented |
| **A.7.14** | Secure disposal or re-use of equipment | Applicable | Prevents data recovery from retired hardware. | NIST SP 800-88 Rev 1 cryptographic erase / physical drive destruction before equipment retirement. | Implemented |

---

## 5. Section A.8: Technological Controls (34 Controls)

| Control ID | Control Name | Applicability | Justification for Inclusion / Exclusion | Implementation Mechanism & Workstation Control (Apex Cyber & Advisory, SP) | Status |
| :--- | :--- | :---: | :--- | :--- | :---: |
| **A.8.1** | User endpoint devices | Applicable | Primary control for workstation host. | Hardened Windows 11 Pro configuration: BitLocker XTS-AES-256, TPM 2.0, Secure Boot, Defender EDR, 10-min screen lock. | Implemented |
| **A.8.2** | Privileged access rights | Applicable | Prevents abuse of administrative privileges. | Standard user account for daily execution; UAC elevation required for system alterations; zero persistent root agent execution. | Implemented |
| **A.8.3** | Information access restriction | Applicable | Enforces confidentiality boundaries. | Filesystem permissions isolate enterprise enclave; sub-silo `medicare/` locked to general agents. | Implemented |
| **A.8.4** | Access to source code | Applicable | Protects proprietary agent logic and tools. | Git repository access restricted via SSH keys with passphrase; branch protection rules on GitHub; no public repos for proprietary code. | Implemented |
| **A.8.5** | Secure authentication | Applicable | Ensures robust identity verification. | FIDO2 WebAuthn hardware passkeys; Authenticator TOTP; biometric authentication. | Implemented |
| **A.8.6** | Capacity management | Applicable | Prevents system exhaustion and downtime. | Disk space monitoring on system drive; RAM utilization alarms; API quota monitoring across model foundries. | Implemented |
| **A.8.7** | Protection against malware | Applicable | Detects and neutralizes malicious code. | Microsoft Defender Antivirus with real-time cloud protection; download quarantine protocol; local skill scanner for agents. | Implemented |
| **A.8.8** | Management of technical vulnerabilities | Applicable | Patches vulnerabilities in OS and software. | Operating system automatic installation; monthly third-party software patch audit; GitHub Dependabot for Python packages. | Implemented |
| **A.8.9** | Configuration management | Applicable | Maintains known, secure baseline configurations. | Standardized workstation baseline; automated configuration scripts; version-controlled agent manifests. | Implemented |
| **A.8.10** | Information deletion | Applicable | Secure disposal of expired data and scripts. | Scheduled purge scripts for downloads and `scratch/`; NIST SP 800-88 cryptographic shredding for sensitive records. | Implemented |
| **A.8.11** | Data masking | Applicable | Protects sensitive data in AI prompts/logs. | Automated Safe Harbor pseudonymization script replacing client names with UUIDs and redacting statutory identifiers. | Implemented |
| **A.8.12** | Data leakage prevention | Applicable | Prevents unauthorized egress of sensitive data. | EDR network inspection; strict ban on consumer LLM copy-paste; firewalled records folder inaccessible to external APIs. | Implemented |
| **A.8.13** | Information backup | Applicable | Ensures disaster recovery capabilities. | Automated daily incremental encrypted backups to secure cloud repository with 3-2-1 backup architecture. | Implemented |
| **A.8.14** | Redundancy of information processing facilities | Applicable | Maintains operational resilience. | Multi-cloud model fallback; secondary workstation hot-standby configuration. | Implemented |
| **A.8.15** | Logging | Applicable | Tracks security events and operational actions. | System Event Logs, Antigravity execution transcripts (`transcript.jsonl`), Git commit logs, and Vanta compliance telemetry. | Implemented |
| **A.8.16** | Monitoring activities | Applicable | Detects anomalous system and agent behavior. | Real-time monitoring via Defender EDR, Vanta security agent, and Antigravity subagent process telemetry. | Implemented |
| **A.8.17** | Clock synchronization | Applicable | Ensures accurate audit trail correlation. | Network Time Protocol (NTP) synchronized to reliable time servers with UTC timestamp normalization across all logs. | Implemented |
| **A.8.18** | Use of privileged utility programs | Applicable | Prevents bypass of controls via system utilities. | Utility programs (PowerShell, Registry Editor) restricted by UAC and monitored via EDR command-line logging. | Implemented |
| **A.8.19** | Installation of software on operational systems | Applicable | Controls installation of unapproved software. | Mandatory download quarantine in `Downloads/`; hash verification; prohibition of unapproved gaming/freeware in OS enclave. | Implemented |
| **A.8.20** | Networks security | Applicable | Secures network infrastructure and traffic. | WPA3 encrypted Wi-Fi; hardware firewall on perimeter router; Endpoint Firewall active on all network profiles. | Implemented |
| **A.8.21** | Security of network services | Applicable | Secures consumed network and cloud services. | TLS 1.3 enforced for all SaaS and API endpoints; DNS over HTTPS (DoH) configured to prevent DNS spoofing. | Implemented |
| **A.8.22** | Segregation of networks | Applicable | Isolates untrusted traffic from work environment. | Dedicated enterprise VLAN for business devices; guest network for IoT and personal recreational gear. | Implemented |
| **A.8.23** | Web filtering | Applicable | Blocks access to malicious and phishing domains. | SmartScreen filtering enabled; DNS-level blocking of malicious domains via secure upstream DNS. | Implemented |
| **A.8.24** | Use of cryptography | Applicable | Implements robust encryption across data states. | BitLocker XTS-AES-256 (at rest); AES-GCM-256 for Tier 4 vaults; TLS 1.3 with Perfect Forward Secrecy (in transit). | Implemented |
| **A.8.25** | Secure development life cycle | Applicable | Secures custom agent skills and tools. | Secure SDLC: requirements -> threat modeling -> safe skill scanning -> maker-checker verification -> git release. | Implemented |
| **A.8.26** | Application security requirements | Applicable | Establishes security criteria for new tools. | Security checklist completed before approving new desktop tools (e.g., Notion, Obsidian, BlitzIt, Taska). | Implemented |
| **A.8.27** | Secure system architecture and engineering principles | Applicable | Enforces zero trust and modularity. | Modular departmental directories with relative pathing; strict enclave boundary isolating personal recreation and gaming. | Implemented |
| **A.8.28** | Secure coding | Applicable | Prevents vulnerabilities in custom Python scripts. | Automated code audits using `script_auditor`; banning hardcoded secrets, dangerous `eval()`, and unvalidated inputs. | Implemented |
| **A.8.29** | Security testing in development and acceptance | Applicable | Validates security before deployment. | Unit tests, synthetic agent prompt-injection testing, and static analysis of all scripts in `10_research_development`. | Implemented |
| **A.8.30** | Outsourced development | Justified Exclusion | Enterprise does not outsource software coding. | **Justified Exclusion:** All agent prompt engineering, code synthesis, and infrastructure scripting are conducted internally. Zero outsourced dev. | Excluded |
| **A.8.31** | Separation of development, test and production environments | Applicable | Prevents untested code impacting live operations. | Segregated directory structures: `10_research_development` (dev/test) vs. operational departmental folders (prod). | Implemented |
| **A.8.32** | Change management | Applicable | Controlled updates to infrastructure and code. | Git version control for all code/docs; pull request reviews; formal change records in ticketing systems / GitHub Releases. | Implemented |
| **A.8.33** | Test information | Applicable | Prevents real client PII in test environments. | Synthetic data generators used exclusively for agent testing; zero production client data allowed in dev/test scripts. | Implemented |
| **A.8.34** | Protection of information systems during audit testing | Applicable | Prevents operational disruption during audits. | Read-only audit accounts; isolated transcript exports; audit activities scheduled to avoid operational downtime. | Implemented |

---

## 6. Document Sign-Off & Executive Approval

**Approved and Formally Adopted By:**

__________________________________________________  
**Raquel B.**, Executive Principal & Lead Auditor  
*ISO/IEC 27001 Lead Auditor (IRCA/PECB Equivalent)*  
*ISO/IEC 42001 Lead Auditor | GRC Specialist*  
**Apex Cyber & Advisory, SP**  
**Date:** October 12, 2026
