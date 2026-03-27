# NIST SP 800-53 vs. SP 800-171 Control Mapping

A comprehensive mapping between NIST SP 800-53 Rev. 5 (the master federal security control catalog with 1,000+ controls across 20 families) and NIST SP 800-171 Rev. 2/Rev. 3 (the derived CUI protection standard with 110 security requirements across 14 families). This repository explains exactly how 800-171 requirements trace back to their 800-53 parent controls, which controls were excluded and why, and when each standard applies to your organization.

**Full reference page:** [https://petronellatech.com/compliance/nist-800-53-vs-800-171/](https://petronellatech.com/compliance/nist-800-53-vs-800-171/)

Last Reviewed: March 2026

---

## Table of Contents

1. [What Is NIST SP 800-53?](#what-is-nist-sp-800-53)
2. [What Is NIST SP 800-171?](#what-is-nist-sp-800-171)
3. [The Derivation Relationship](#the-derivation-relationship)
4. [20 Families vs. 14 Families](#20-families-vs-14-families)
5. [NFO and FED Exclusions Explained](#nfo-and-fed-exclusions-explained)
6. [Complete Family-Level Mapping](#complete-family-level-mapping)
7. [Control-Level Mapping Examples](#control-level-mapping-examples)
8. [When Each Standard Applies](#when-each-standard-applies)
9. [Key Differences at a Glance](#key-differences-at-a-glance)
10. [How CMMC Connects Both Standards](#how-cmmc-connects-both-standards)
11. [Practical Compliance Strategy](#practical-compliance-strategy)
12. [Common Mistakes Organizations Make](#common-mistakes-organizations-make)
13. [About PTG](#about-ptg)
14. [License](#license)

---

## What Is NIST SP 800-53?

NIST Special Publication 800-53 Revision 5, "Security and Privacy Controls for Information Systems and Organizations," is the master control catalog published by the National Institute of Standards and Technology. It contains over 1,000 individual security and privacy controls organized into 20 control families. Originally developed for federal information systems under FISMA, 800-53 Rev. 5 removed the "federal-only" scope limitation, making it applicable to any organization regardless of sector.

The 20 control families in 800-53 Rev. 5 are:

| ID | Family Name |
|----|-------------|
| AC | Access Control |
| AT | Awareness and Training |
| AU | Audit and Accountability |
| CA | Assessment, Authorization, and Monitoring |
| CM | Configuration Management |
| CP | Contingency Planning |
| IA | Identification and Authentication |
| IR | Incident Response |
| MA | Maintenance |
| MP | Media Protection |
| PE | Physical and Environmental Protection |
| PL | Planning |
| PM | Program Management |
| PS | Personnel Security |
| PT | PII Processing and Transparency |
| RA | Risk Assessment |
| SA | System and Services Acquisition |
| SC | System and Communications Protection |
| SI | System and Information Integrity |
| SR | Supply Chain Risk Management |

800-53 controls are assigned to three baselines: Low, Moderate, and High. Each baseline adds progressively more controls. The Moderate baseline is the critical one for understanding the 800-171 derivation because 800-171 is derived primarily from 800-53 Moderate controls.

Source: [NIST SP 800-53 Rev. 5](https://csrc.nist.gov/publications/detail/sp/800-53/rev-5/final)

## What Is NIST SP 800-171?

NIST Special Publication 800-171, "Protecting Controlled Unclassified Information in Nonfederal Systems and Organizations," defines 110 security requirements (Rev. 2) for protecting CUI when it resides on nonfederal systems. If your organization handles CUI for a federal contract, especially Department of Defense contracts governed by DFARS 252.204-7012, you must implement 800-171.

800-171 organizes its 110 requirements into 14 families:

| ID | Family Name |
|----|-------------|
| 3.1 | Access Control |
| 3.2 | Awareness and Training |
| 3.3 | Audit and Accountability |
| 3.4 | Configuration Management |
| 3.5 | Identification and Authentication |
| 3.6 | Incident Response |
| 3.7 | Maintenance |
| 3.8 | Media Protection |
| 3.9 | Personnel Security |
| 3.10 | Physical Protection |
| 3.11 | Risk Assessment |
| 3.12 | Security Assessment |
| 3.13 | System and Communications Protection |
| 3.14 | System and Information Integrity |

The numbering is not arbitrary. Each 800-171 requirement traces directly to one or more 800-53 Moderate baseline controls. Appendix D of 800-171 Rev. 2 provides this complete mapping.

Source: [NIST SP 800-171 Rev. 2](https://csrc.nist.gov/publications/detail/sp/800-171/rev-2/final)

## The Derivation Relationship

800-171 is not an independent standard. It was derived from 800-53 through a deliberate tailoring process documented in NIST SP 800-171 Appendix D. The process worked as follows:

1. Start with the 800-53 Moderate baseline (approximately 325 controls).
2. Remove controls that are uniquely federal in nature (FED tailoring criteria), meaning they apply only when the federal government operates the system.
3. Remove controls that are not directly related to protecting the confidentiality of CUI (NFO tailoring criteria).
4. Express the remaining controls as security requirements using nonfederal language.

This means every 800-171 requirement has a parent 800-53 control. If you already comply with 800-53 Moderate, you have addressed the vast majority of 800-171. Conversely, if you are implementing 800-171, you are implementing a curated subset of 800-53 Moderate.

Understanding this derivation is essential for organizations that must satisfy multiple frameworks simultaneously. Rather than treating 800-53 and 800-171 as separate compliance efforts, smart organizations implement the 800-53 Moderate baseline once and then demonstrate 800-171 compliance as a natural byproduct.

## 20 Families vs. 14 Families

The most visible difference between the two standards is the family count: 800-53 has 20 families, while 800-171 has 14. Six entire 800-53 families have no direct counterpart in 800-171:

| 800-53 Family | Why It Is Not in 800-171 |
|---|---|
| CP (Contingency Planning) | Classified as NFO; contingency planning protects availability, not CUI confidentiality directly. Organizations still need contingency plans, but 800-171 focuses specifically on CUI confidentiality. |
| PL (Planning) | Classified as FED; security planning activities like system security plans are federal management requirements. Nonfederal organizations have different governance structures. |
| PM (Program Management) | Classified as FED; program-level management controls like CISO appointment and capital planning are uniquely federal. |
| PT (PII Processing and Transparency) | New in 800-53 Rev. 5; did not exist when 800-171 Rev. 2 was published. Privacy-specific controls outside 800-171 scope. |
| SA (System and Services Acquisition) | Partially mapped. Some SA controls appear in 800-171 under other families, but the family as a whole is excluded because acquisition governance is primarily a federal responsibility. |
| SR (Supply Chain Risk Management) | New in 800-53 Rev. 5; supply chain controls were not part of 800-171 Rev. 2. Note: 800-172 (Enhanced Security) does address supply chain. |

The remaining 14 families map directly, though the naming sometimes differs slightly between 800-53 and 800-171.

## NFO and FED Exclusions Explained

Two tailoring criteria drive the exclusions:

**NFO (Not directly related to protecting the confidentiality of CUI)**

NFO controls protect availability, integrity, or organizational governance rather than CUI confidentiality. Examples include:

- CP-2 (Contingency Plan): Protects availability, not confidentiality
- CP-10 (System Recovery and Reconstitution): Availability focused
- IR-8 (Incident Response Plan): Administrative planning control; however, the operational incident handling controls (IR-2 through IR-6) ARE included in 800-171

Important: NFO exclusions do not mean these controls are unimportant. They mean 800-171 chose to focus narrowly on confidentiality. Any organization with serious security posture should implement contingency planning regardless of whether 800-171 requires it.

**FED (Expected to be satisfied by the federal government, not nonfederal contractors)**

FED controls are responsibilities that remain with the federal agency, not the contractor. Examples include:

- PL-2 (System Security Plan): Federal agencies maintain SSPs for their authorization boundary. Contractors document their own security through different mechanisms.
- PM-1 (Information Security Program Plan): Agency-level program management
- CA-6 (Authorization): The federal ATO process is a government responsibility

However, this creates a practical problem: CMMC Level 2 assessors expect contractors to have an SSP even though 800-171 technically excludes PL-2. DFARS 252.204-7012 paragraph (c)(2) explicitly requires an SSP. This disconnect catches many contractors off guard.

## Complete Family-Level Mapping

See [mapping.md](mapping.md) for the complete control-by-control mapping table covering all 110 requirements in 800-171 Rev. 2 traced to their 800-53 Rev. 5 parent controls.

The summary mapping by family is:

| 800-171 Family | 800-53 Parent Family | 800-171 Requirements | 800-53 Moderate Controls (approx.) | Coverage |
|---|---|---|---|---|
| 3.1 Access Control | AC | 22 | 47 | 47% of AC Moderate |
| 3.2 Awareness and Training | AT | 3 | 5 | 60% of AT Moderate |
| 3.3 Audit and Accountability | AU | 9 | 17 | 53% of AU Moderate |
| 3.4 Configuration Management | CM | 9 | 18 | 50% of CM Moderate |
| 3.5 Identification and Authentication | IA | 11 | 19 | 58% of IA Moderate |
| 3.6 Incident Response | IR | 3 | 10 | 30% of IR Moderate |
| 3.7 Maintenance | MA | 6 | 6 | 100% of MA Moderate |
| 3.8 Media Protection | MP | 9 | 8 | 100%+ (includes enhancements) |
| 3.9 Personnel Security | PS | 2 | 8 | 25% of PS Moderate |
| 3.10 Physical Protection | PE | 6 | 20 | 30% of PE Moderate |
| 3.11 Risk Assessment | RA | 3 | 5 | 60% of RA Moderate |
| 3.12 Security Assessment | CA | 4 | 9 | 44% of CA Moderate |
| 3.13 System and Communications Protection | SC | 16 | 25 | 64% of SC Moderate |
| 3.14 System and Information Integrity | SI | 7 | 14 | 50% of SI Moderate |
| **Totals** | | **110** | **~211** | **~52%** |

This means 800-171 covers roughly 52% of the 800-53 Moderate baseline. Organizations that implement only 800-171 have significant security gaps in contingency planning, supply chain risk management, and program-level governance.

## Control-Level Mapping Examples

Here are representative mappings showing how 800-171 requirements trace to their 800-53 parents:

| 800-171 Requirement | Description | 800-53 Parent Control(s) |
|---|---|---|
| 3.1.1 | Limit system access to authorized users | AC-2, AC-3, AC-17 |
| 3.1.2 | Limit system access to authorized functions | AC-2, AC-3, AC-17 |
| 3.5.1 | Identify system users and processes | IA-2, IA-5 |
| 3.5.2 | Authenticate users and processes | IA-2, IA-5 |
| 3.5.3 | Use multifactor authentication | IA-2(1), IA-2(2) |
| 3.13.1 | Monitor communications at external boundaries | SC-7 |
| 3.13.11 | Employ FIPS-validated cryptography | SC-13 |
| 3.14.1 | Identify and correct system flaws | SI-2 |
| 3.14.2 | Provide malicious code protection | SI-3 |
| 3.14.6 | Monitor organizational systems | SI-4 |

Notice that a single 800-171 requirement often maps to multiple 800-53 controls, and vice versa. This many-to-many relationship is why organizations benefit from working with an advisor who understands both standards deeply.

## When Each Standard Applies

**You need 800-53 if:**
- You are a federal agency or operate federal information systems under FISMA
- You are pursuing FedRAMP authorization (FedRAMP requires 800-53 High with additional parameters)
- Your contract specifically references 800-53 compliance
- You want the most comprehensive security control catalog available as a reference framework

**You need 800-171 if:**
- You handle Controlled Unclassified Information (CUI) for the Department of Defense
- Your contract includes DFARS 252.204-7012 (virtually all DoD contracts since 2017)
- You are pursuing CMMC Level 2 certification (CMMC Level 2 maps directly to 800-171)
- You are a subcontractor to a prime that handles CUI (the flow-down requirement applies)

**You may need both if:**
- You are a federal contractor that both operates federal systems (800-53 via FISMA/FedRAMP) AND handles CUI on your own systems (800-171)
- You are pursuing FedRAMP Moderate or High AND have DoD contracts with CUI

## Key Differences at a Glance

| Dimension | 800-53 Rev. 5 | 800-171 Rev. 2 |
|---|---|---|
| Total Controls | 1,000+ across 20 families | 110 across 14 families |
| Scope | All information systems, all sectors | Nonfederal systems handling CUI |
| Baselines | Low, Moderate, High | Single baseline (derived from Moderate) |
| Assessment Method | 800-53A (formal assessment procedures) | 800-171A (110 assessment objectives, 320 determination statements) |
| Certification Program | FedRAMP (for cloud), FISMA ATO (for agencies) | CMMC (for DoD supply chain) |
| Governing Law/Regulation | FISMA (44 U.S.C. 3551 et seq.) | DFARS 252.204-7012 |
| Self-Assessment Scoring | N/A | SPRS (Supplier Performance Risk System), -203 to +110 |
| Enhanced Version | 800-53 High baseline | 800-172 (Enhanced Security Requirements) |
| Published By | NIST | NIST |
| Current Version Date | September 2020 (Rev. 5) | February 2020 (Rev. 2); Rev. 3 published May 2024 |

## How CMMC Connects Both Standards

The Cybersecurity Maturity Model Certification (CMMC) 2.0 creates a direct bridge:

- **CMMC Level 1**: 17 practices derived from FAR 52.204-21 (basic safeguarding). These are a subset of 800-171.
- **CMMC Level 2**: All 110 security requirements from 800-171 Rev. 2. A CMMC Level 2 assessment IS an 800-171 assessment.
- **CMMC Level 3**: 800-171 plus selected controls from 800-172 (Enhanced Security Requirements), which itself pulls from 800-53 High baseline controls.

This means CMMC Level 3 effectively requires controls spanning both 800-171 and portions of 800-53 beyond the Moderate baseline. Organizations planning for Level 3 should implement against 800-53 rather than treating 800-171 as their ceiling.

## Practical Compliance Strategy

1. **Start with 800-53 Moderate as your foundation.** Even if your immediate requirement is only 800-171, implementing the full Moderate baseline positions you for FedRAMP, CMMC Level 3, and other frameworks that derive from 800-53.

2. **Use the SPRS Calculator to score your 800-171 posture.** Every DoD contractor must submit a self-assessment score to SPRS. PTG offers a free SPRS calculator at [https://petronellatech.com/tools/sprs-calculator/](https://petronellatech.com/tools/sprs-calculator/).

3. **Map once, satisfy many.** Because 800-171 traces directly to 800-53, and CMMC maps to 800-171, a single well-documented implementation can satisfy all three requirements simultaneously.

4. **Do not ignore the excluded families.** Contingency planning (CP), supply chain risk management (SR), and program management (PM) may not be in 800-171, but they are critical to actual security. CMMC assessors frequently ask about business continuity even though it is not a scored practice.

5. **Engage a CMMC Registered Practitioner.** A qualified practitioner can help you navigate the overlap between these standards and avoid the common trap of implementing the same control twice under different names.

## Common Mistakes Organizations Make

1. **Treating 800-171 and 800-53 as separate compliance projects.** They share the same DNA. Implementing them as separate efforts doubles your cost and creates documentation inconsistencies.

2. **Ignoring the NFO controls.** Just because 800-171 excludes contingency planning does not mean you can skip disaster recovery. Your CMMC assessor, your cyber insurance underwriter, and your customers all expect it.

3. **Not tracking the 800-53 parent for each 800-171 requirement.** When an assessor asks for evidence, understanding the parent control helps you provide deeper, more credible documentation.

4. **Assuming Rev. 2 and Rev. 3 are interchangeable.** 800-171 Rev. 3 (published May 2024) restructured the requirements significantly and aligns with 800-53 Rev. 5 more directly. CMMC 2.0 currently references Rev. 2, but organizations should prepare for the transition.

5. **Not calculating their SPRS score.** DFARS 252.204-7019 requires a current SPRS score. Scores range from -203 (no controls implemented) to +110 (full implementation). Many contractors have never submitted a score, which puts them at risk of losing contracts.

## About PTG

This repository is maintained by **Petronella Technology Group, Inc. (PTG)**, a cybersecurity, compliance, and AI services firm headquartered in Raleigh, North Carolina.

**Craig Petronella**, PTG's founder, brings the following credentials to compliance advisory:

- CMMC Registered Practitioner (RP)
- Licensed Digital Forensic Examiner #604180
- Cisco CCNA and CWNE certifications
- MIT Artificial Intelligence Certificate
- Amazon #1 Best-Selling Author of 14+ cybersecurity books
- 23+ years of cybersecurity experience

**What makes PTG different:**

- **AI-Powered Compliance.** PTG uses its own private AI fleet, including on-premise LLMs and custom GPU infrastructure, to accelerate compliance assessments, automate control mapping, and continuously monitor security posture. No other firm in the Triangle has this capability.
- **Patented Technology Stack.** PTG's proprietary and patented security tools automate what competitors do manually.
- **Licensed Digital Forensic Examiner.** When compliance fails and a breach occurs, PTG has the forensic expertise to investigate, preserve evidence, and support legal proceedings.
- **AI + Cybersecurity Combined.** PTG is one of the only firms combining AI development (custom AI agents, private LLMs, GPU hosting) with cybersecurity and compliance.
- **SMB Focus.** PTG makes enterprise-grade compliance accessible to small and mid-size businesses.

**Contact PTG:**

- Phone: 919-348-4912
- Web: [https://petronellatech.com](https://petronellatech.com)
- Compliance Services: [https://petronellatech.com/compliance/packages/](https://petronellatech.com/compliance/packages/)
- NIST Hub: [https://petronellatech.com/nist/](https://petronellatech.com/nist/)
- CMMC Hub: [https://petronellatech.com/compliance/cmmc/](https://petronellatech.com/compliance/cmmc/)
- SPRS Calculator: [https://petronellatech.com/tools/sprs-calculator/](https://petronellatech.com/tools/sprs-calculator/)

**Address:** 5540 Centerview Dr. Suite 200, Raleigh, NC 27606

Call 919-348-4912 or visit [petronellatech.com/compliance/packages/](https://petronellatech.com/compliance/packages/) to schedule a free compliance assessment.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
