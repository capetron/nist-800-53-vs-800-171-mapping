# NIST SP 800-53 Rev. 5 to SP 800-171 Rev. 2 Complete Control Mapping

This document provides the complete control-by-control mapping between NIST SP 800-171 Rev. 2 security requirements and their parent NIST SP 800-53 Rev. 5 controls. The mapping is derived from Appendix D of SP 800-171 Rev. 2.

Last Reviewed: March 2026

---

## How to Read This Mapping

- **800-171 Req**: The 800-171 Rev. 2 requirement number
- **800-171 Description**: Summary of the requirement
- **800-53 Parent(s)**: The 800-53 Rev. 5 control(s) from which this requirement was derived
- **800-53 Baseline**: Which 800-53 baseline includes this control (L=Low, M=Moderate, H=High)
- **SPRS Weight**: The weighted value used in SPRS scoring (higher = more critical)

---

## 3.1 Access Control (22 Requirements)

| 800-171 Req | Description | 800-53 Parent(s) | Baseline | SPRS Weight |
|---|---|---|---|---|
| 3.1.1 | Limit system access to authorized users, processes, and devices | AC-2, AC-3, AC-17 | L/M/H | 5 |
| 3.1.2 | Limit system access to the types of transactions and functions that authorized users are permitted to execute | AC-2, AC-3, AC-17 | L/M/H | 5 |
| 3.1.3 | Control the flow of CUI in accordance with approved authorizations | AC-4 | M/H | 5 |
| 3.1.4 | Separate the duties of individuals to reduce the risk of malevolent activity | AC-5 | M/H | 1 |
| 3.1.5 | Employ the principle of least privilege, including for specific security functions and privileged accounts | AC-6, AC-6(1), AC-6(2), AC-6(5) | M/H | 5 |
| 3.1.6 | Use non-privileged accounts or roles when accessing nonsecurity functions | AC-6(2) | M/H | 1 |
| 3.1.7 | Prevent non-privileged users from executing privileged functions and capture the execution of such functions in audit logs | AC-6(9), AC-6(10) | M/H | 3 |
| 3.1.8 | Limit unsuccessful logon attempts | AC-7 | L/M/H | 3 |
| 3.1.9 | Provide privacy and security notices consistent with applicable CUI rules | AC-8 | L/M/H | 1 |
| 3.1.10 | Use session lock with pattern-hiding displays to prevent access and viewing of data after a period of inactivity | AC-11, AC-11(1) | M/H | 1 |
| 3.1.11 | Terminate (automatically) a user session after a defined condition | AC-12 | M/H | 1 |
| 3.1.12 | Monitor and control remote access sessions | AC-17(1), AC-17(2) | M/H | 3 |
| 3.1.13 | Employ cryptographic mechanisms to protect the confidentiality of remote access sessions | AC-17(2) | M/H | 5 |
| 3.1.14 | Route remote access via managed access control points | AC-17(3) | M/H | 3 |
| 3.1.15 | Authorize remote execution of privileged commands and remote access to security-relevant information | AC-17(4) | M/H | 5 |
| 3.1.16 | Authorize wireless access prior to allowing such connections | AC-18, AC-18(1) | L/M/H | 1 |
| 3.1.17 | Protect wireless access using authentication and encryption | AC-18(1) | M/H | 5 |
| 3.1.18 | Control connection of mobile devices | AC-19 | L/M/H | 3 |
| 3.1.19 | Encrypt CUI on mobile devices and mobile computing platforms | AC-19(5) | M/H | 5 |
| 3.1.20 | Verify and control/limit connections to and use of external systems | AC-20, AC-20(1) | L/M/H | 1 |
| 3.1.21 | Limit use of portable storage devices on external systems | AC-20(2) | M/H | 1 |
| 3.1.22 | Control CUI posted or processed on publicly accessible systems | AC-22 | L/M/H | 5 |

## 3.2 Awareness and Training (3 Requirements)

| 800-171 Req | Description | 800-53 Parent(s) | Baseline | SPRS Weight |
|---|---|---|---|---|
| 3.2.1 | Ensure that managers, systems administrators, and users of organizational systems are made aware of the security risks | AT-2, AT-2(2) | L/M/H | 3 |
| 3.2.2 | Ensure that personnel are trained to carry out their assigned information security-related duties and responsibilities | AT-3 | L/M/H | 3 |
| 3.2.3 | Provide security awareness training on recognizing and reporting potential indicators of insider threat | AT-2(2) | M/H | 1 |

## 3.3 Audit and Accountability (9 Requirements)

| 800-171 Req | Description | 800-53 Parent(s) | Baseline | SPRS Weight |
|---|---|---|---|---|
| 3.3.1 | Create and retain system audit logs and records to the extent needed to enable the monitoring, analysis, investigation, and reporting of unlawful or unauthorized system activity | AU-2, AU-3, AU-3(1), AU-6, AU-12 | L/M/H | 5 |
| 3.3.2 | Ensure that the actions of individual system users can be uniquely traced to those users so they can be held accountable | AU-2, AU-3, AU-6, AU-12 | L/M/H | 5 |
| 3.3.3 | Review and update logged events | AU-2(3) | M/H | 1 |
| 3.3.4 | Alert in the event of an audit logging process failure | AU-5 | L/M/H | 1 |
| 3.3.5 | Correlate audit record review, analysis, and reporting processes for investigation and response to indications of unlawful, unauthorized, suspicious, or unusual activity | AU-6(3) | M/H | 3 |
| 3.3.6 | Provide audit record reduction and report generation to support on-demand analysis and reporting | AU-7 | M/H | 1 |
| 3.3.7 | Provide a system capability that compares and synchronizes internal system clocks with an authoritative source to generate time stamps for audit records | AU-8, AU-8(1) | L/M/H | 1 |
| 3.3.8 | Protect audit information and audit logging tools from unauthorized access, modification, and deletion | AU-9 | L/M/H | 3 |
| 3.3.9 | Limit management of audit logging functionality to a subset of privileged users | AU-9(4) | M/H | 1 |

## 3.4 Configuration Management (9 Requirements)

| 800-171 Req | Description | 800-53 Parent(s) | Baseline | SPRS Weight |
|---|---|---|---|---|
| 3.4.1 | Establish and maintain baseline configurations and inventories of organizational systems | CM-2, CM-6, CM-8, CM-8(1) | L/M/H | 5 |
| 3.4.2 | Establish and enforce security configuration settings for IT products employed in organizational systems | CM-6 | L/M/H | 5 |
| 3.4.3 | Track, review, approve or disapprove, and log changes to organizational systems | CM-3, CM-3(2) | M/H | 3 |
| 3.4.4 | Analyze the security impact of changes prior to implementation | CM-4 | L/M/H | 3 |
| 3.4.5 | Define, document, approve, and enforce physical and logical access restrictions associated with changes to organizational systems | CM-5 | M/H | 3 |
| 3.4.6 | Employ the principle of least functionality by configuring organizational systems to provide only essential capabilities | CM-7 | L/M/H | 5 |
| 3.4.7 | Restrict, disable, or prevent the use of nonessential programs, functions, ports, protocols, and services | CM-7(1), CM-7(2) | M/H | 5 |
| 3.4.8 | Apply deny-by-exception (blacklisting) policy to prevent the use of unauthorized software or deny-all, permit-by-exception (whitelisting) policy to allow the execution of authorized software | CM-7(4), CM-7(5) | M/H | 3 |
| 3.4.9 | Control and monitor user-installed software | CM-11 | M/H | 3 |

## 3.5 Identification and Authentication (11 Requirements)

| 800-171 Req | Description | 800-53 Parent(s) | Baseline | SPRS Weight |
|---|---|---|---|---|
| 3.5.1 | Identify system users, processes acting on behalf of users, and devices | IA-2, IA-5 | L/M/H | 5 |
| 3.5.2 | Authenticate (or verify) the identities of users, processes, or devices, as a prerequisite to allowing access to organizational systems | IA-2, IA-5 | L/M/H | 5 |
| 3.5.3 | Use multifactor authentication for local and network access to privileged accounts and for network access to non-privileged accounts | IA-2(1), IA-2(2) | M/H | 5 |
| 3.5.4 | Employ replay-resistant authentication mechanisms for network access to privileged and non-privileged accounts | IA-2(8) | M/H | 3 |
| 3.5.5 | Prevent reuse of identifiers for a defined period | IA-4 | L/M/H | 1 |
| 3.5.6 | Disable identifiers after a defined period of inactivity | IA-4(4) | M/H | 1 |
| 3.5.7 | Enforce a minimum password complexity and change of characters when new passwords are created | IA-5(1) | L/M/H | 3 |
| 3.5.8 | Prohibit password reuse for a specified number of generations | IA-5(1) | L/M/H | 1 |
| 3.5.9 | Allow temporary password use for system logons with an immediate change to a permanent password | IA-5(1) | L/M/H | 1 |
| 3.5.10 | Store and transmit only cryptographically-protected passwords | IA-5(1) | L/M/H | 5 |
| 3.5.11 | Obscure feedback of authentication information | IA-6 | L/M/H | 1 |

## 3.6 Incident Response (3 Requirements)

| 800-171 Req | Description | 800-53 Parent(s) | Baseline | SPRS Weight |
|---|---|---|---|---|
| 3.6.1 | Establish an operational incident-handling capability for organizational systems that includes preparation, detection, analysis, containment, recovery, and user response activities | IR-2, IR-4, IR-5, IR-6, IR-7 | L/M/H | 5 |
| 3.6.2 | Track, document, and report incidents to designated officials and/or authorities both internal and external to the organization | IR-6, IR-6(1) | L/M/H | 5 |
| 3.6.3 | Test the organizational incident response capability | IR-3, IR-3(2) | M/H | 3 |

## 3.7 Maintenance (6 Requirements)

| 800-171 Req | Description | 800-53 Parent(s) | Baseline | SPRS Weight |
|---|---|---|---|---|
| 3.7.1 | Perform maintenance on organizational systems | MA-2 | L/M/H | 1 |
| 3.7.2 | Provide controls on the tools, techniques, mechanisms, and personnel used to conduct system maintenance | MA-3, MA-3(1), MA-3(2) | M/H | 3 |
| 3.7.3 | Ensure equipment removed for off-site maintenance is sanitized of any CUI | MA-3(3) | H | 1 |
| 3.7.4 | Check media containing diagnostic and test programs for malicious code before the media are used in organizational systems | MA-3(2) | M/H | 1 |
| 3.7.5 | Require multifactor authentication to establish nonlocal maintenance sessions via external network connections and terminate such connections when nonlocal maintenance is complete | MA-4, MA-4(1) | L/M/H | 3 |
| 3.7.6 | Supervise the maintenance activities of maintenance personnel without required access authorization | MA-5 | L/M/H | 3 |

## 3.8 Media Protection (9 Requirements)

| 800-171 Req | Description | 800-53 Parent(s) | Baseline | SPRS Weight |
|---|---|---|---|---|
| 3.8.1 | Protect (i.e., physically control and securely store) system media containing CUI, both paper and digital | MP-2, MP-4 | L/M/H | 3 |
| 3.8.2 | Limit access to CUI on system media to authorized users | MP-2 | L/M/H | 3 |
| 3.8.3 | Sanitize or destroy system media containing CUI before disposal or release for reuse | MP-6 | L/M/H | 5 |
| 3.8.4 | Mark media with necessary CUI markings and distribution limitations | MP-3 | M/H | 1 |
| 3.8.5 | Control access to media containing CUI and maintain accountability for media during transport outside of controlled areas | MP-5, MP-5(4) | M/H | 3 |
| 3.8.6 | Implement cryptographic mechanisms to protect the confidentiality of CUI stored on digital media during transport unless otherwise protected by alternative physical safeguards | MP-5(4) | M/H | 5 |
| 3.8.7 | Control the use of removable media on system components | MP-7, MP-7(1) | L/M/H | 3 |
| 3.8.8 | Prohibit the use of portable storage devices when such devices have no identifiable owner | MP-7(1) | M/H | 1 |
| 3.8.9 | Protect the confidentiality of backup CUI at storage locations | CP-9 | L/M/H | 5 |

## 3.9 Personnel Security (2 Requirements)

| 800-171 Req | Description | 800-53 Parent(s) | Baseline | SPRS Weight |
|---|---|---|---|---|
| 3.9.1 | Screen individuals prior to authorizing access to organizational systems containing CUI | PS-3, PS-6 | L/M/H | 3 |
| 3.9.2 | Ensure that organizational systems containing CUI are protected during and after personnel actions such as terminations and transfers | PS-4, PS-5 | L/M/H | 5 |

## 3.10 Physical Protection (6 Requirements)

| 800-171 Req | Description | 800-53 Parent(s) | Baseline | SPRS Weight |
|---|---|---|---|---|
| 3.10.1 | Limit physical access to organizational systems, equipment, and the respective operating environments to authorized individuals | PE-2, PE-6 | L/M/H | 5 |
| 3.10.2 | Protect and monitor the physical facility and support infrastructure for organizational systems | PE-2, PE-3, PE-6 | L/M/H | 5 |
| 3.10.3 | Escort visitors and monitor visitor activity | PE-2, PE-3 | L/M/H | 1 |
| 3.10.4 | Maintain audit logs of physical access | PE-2, PE-6 | L/M/H | 1 |
| 3.10.5 | Control and manage physical access devices | PE-3 | L/M/H | 1 |
| 3.10.6 | Enforce safeguarding measures for CUI at alternate work sites | PE-17 | M/H | 1 |

## 3.11 Risk Assessment (3 Requirements)

| 800-171 Req | Description | 800-53 Parent(s) | Baseline | SPRS Weight |
|---|---|---|---|---|
| 3.11.1 | Periodically assess the risk to organizational operations, organizational assets, and individuals, resulting from the operation of organizational systems and the associated processing, storage, or transmission of CUI | RA-3 | L/M/H | 5 |
| 3.11.2 | Scan for vulnerabilities in organizational systems and applications periodically and when new vulnerabilities affecting those systems and applications are identified | RA-5, RA-5(5) | L/M/H | 5 |
| 3.11.3 | Remediate vulnerabilities in accordance with risk assessments | RA-5 | L/M/H | 5 |

## 3.12 Security Assessment (4 Requirements)

| 800-171 Req | Description | 800-53 Parent(s) | Baseline | SPRS Weight |
|---|---|---|---|---|
| 3.12.1 | Periodically assess the security controls in organizational systems to determine if the controls are effective in their application | CA-2, CA-2(1) | L/M/H | 5 |
| 3.12.2 | Develop and implement plans of action designed to correct deficiencies and reduce or eliminate vulnerabilities in organizational systems | CA-5 | L/M/H | 5 |
| 3.12.3 | Monitor security controls on an ongoing basis to ensure the continued effectiveness of the controls | CA-7 | L/M/H | 5 |
| 3.12.4 | Develop, document, and periodically update system security plans that describe system boundaries, system environments of operation, how security requirements are implemented, and the relationships with or connections to other systems | PL-2 | L/M/H | 5 |

Note: Requirement 3.12.4 maps to PL-2 despite the PL (Planning) family being generally excluded as FED. The SSP requirement was retained because DFARS 252.204-7012(c)(2) explicitly requires it.

## 3.13 System and Communications Protection (16 Requirements)

| 800-171 Req | Description | 800-53 Parent(s) | Baseline | SPRS Weight |
|---|---|---|---|---|
| 3.13.1 | Monitor, control, and protect communications at the external boundaries of organizational systems and at key internal boundaries | SC-7 | L/M/H | 5 |
| 3.13.2 | Employ architectural designs, software development techniques, and systems engineering principles that promote effective information security | SA-8 | L/M/H | 3 |
| 3.13.3 | Separate user functionality from system management functionality | SC-2 | M/H | 3 |
| 3.13.4 | Prevent unauthorized and unintended information transfer via shared system resources | SC-4 | M/H | 5 |
| 3.13.5 | Implement subnetworks for publicly accessible system components that are physically or logically separated from internal networks | SC-7 | L/M/H | 5 |
| 3.13.6 | Deny network communications traffic by default and allow network communications traffic by exception | SC-7(5) | M/H | 5 |
| 3.13.7 | Prevent remote devices from simultaneously establishing non-remote connections with organizational systems and communicating via some other connection to resources in external networks (split tunneling) | SC-7(7) | M/H | 5 |
| 3.13.8 | Implement cryptographic mechanisms to prevent unauthorized disclosure of CUI during transmission unless otherwise protected by alternative physical safeguards | SC-8, SC-8(1) | M/H | 5 |
| 3.13.9 | Terminate network connections associated with communications sessions at the end of the sessions or after a defined period of inactivity | SC-10 | M/H | 1 |
| 3.13.10 | Establish and manage cryptographic keys for cryptography employed in organizational systems | SC-12 | L/M/H | 5 |
| 3.13.11 | Employ FIPS-validated cryptography when used to protect the confidentiality of CUI | SC-13 | L/M/H | 5 |
| 3.13.12 | Prohibit remote activation of collaborative computing devices and provide indication of devices in use to users present at the device | SC-15 | L/M/H | 1 |
| 3.13.13 | Control and monitor the use of mobile code | SC-18 | M/H | 1 |
| 3.13.14 | Control and monitor the use of Voice over Internet Protocol (VoIP) technologies | SC-19 | M/H | 1 |
| 3.13.15 | Protect the authenticity of communications sessions | SC-23 | M/H | 3 |
| 3.13.16 | Protect the confidentiality of CUI at rest | SC-28 | M/H | 5 |

## 3.14 System and Information Integrity (7 Requirements)

| 800-171 Req | Description | 800-53 Parent(s) | Baseline | SPRS Weight |
|---|---|---|---|---|
| 3.14.1 | Identify, report, and correct system flaws in a timely manner | SI-2 | L/M/H | 5 |
| 3.14.2 | Provide protection from malicious code at designated locations within organizational systems | SI-3 | L/M/H | 5 |
| 3.14.3 | Monitor system security alerts and advisories and take action in response | SI-5 | L/M/H | 3 |
| 3.14.4 | Update malicious code protection mechanisms when new releases are available | SI-3 | L/M/H | 3 |
| 3.14.5 | Perform periodic scans of organizational systems and real-time scans of files from external sources as files are downloaded, opened, or executed | SI-3 | L/M/H | 3 |
| 3.14.6 | Monitor organizational systems, including inbound and outbound communications traffic, to detect attacks and indicators of potential attacks | SI-4, SI-4(4), SI-4(5) | L/M/H | 5 |
| 3.14.7 | Identify unauthorized use of organizational systems | SI-4 | L/M/H | 3 |

---

## Excluded 800-53 Families (Not Mapped to 800-171)

| 800-53 Family | Exclusion Reason | Controls Excluded | Notes |
|---|---|---|---|
| CP (Contingency Planning) | NFO | 13 Moderate controls | Protects availability, not CUI confidentiality. Still critical for business operations. |
| PL (Planning) | FED | 4 Moderate controls | Federal planning requirements. Exception: PL-2 (SSP) is retained via 3.12.4. |
| PM (Program Management) | FED | 16 controls | Agency-level program management. |
| PT (PII Processing and Transparency) | Out of Scope | 8 controls | New in Rev. 5; privacy-specific. |
| SA (System and Services Acquisition) | Partially FED | ~14 Moderate controls | SA-8 retained via 3.13.2. Acquisition governance is federal. |
| SR (Supply Chain Risk Management) | New in Rev. 5 | 5 controls | Not in 800-171 Rev. 2. Addressed in 800-172 for CMMC Level 3. |

---

## SPRS Score Summary

| Family | Max Points | Number of Requirements | Average Weight |
|---|---|---|---|
| 3.1 Access Control | 68 | 22 | 3.1 |
| 3.2 Awareness and Training | 7 | 3 | 2.3 |
| 3.3 Audit and Accountability | 21 | 9 | 2.3 |
| 3.4 Configuration Management | 35 | 9 | 3.9 |
| 3.5 Identification and Authentication | 31 | 11 | 2.8 |
| 3.6 Incident Response | 13 | 3 | 4.3 |
| 3.7 Maintenance | 12 | 6 | 2.0 |
| 3.8 Media Protection | 25 | 9 | 2.8 |
| 3.9 Personnel Security | 8 | 2 | 4.0 |
| 3.10 Physical Protection | 14 | 6 | 2.3 |
| 3.11 Risk Assessment | 15 | 3 | 5.0 |
| 3.12 Security Assessment | 20 | 4 | 5.0 |
| 3.13 System and Communications Protection | 57 | 16 | 3.6 |
| 3.14 System and Information Integrity | 27 | 7 | 3.9 |

Total possible SPRS score: **110**
Minimum possible SPRS score: **-203** (all controls unimplemented)

---

## Sources

- [NIST SP 800-53 Rev. 5](https://csrc.nist.gov/publications/detail/sp/800-53/rev-5/final)
- [NIST SP 800-171 Rev. 2](https://csrc.nist.gov/publications/detail/sp/800-171/rev-2/final)
- [NIST SP 800-171 Rev. 2, Appendix D (Mapping)](https://csrc.nist.gov/publications/detail/sp/800-171/rev-2/final)
- [NIST SP 800-171A (Assessment Procedures)](https://csrc.nist.gov/publications/detail/sp/800-171a/final)
- [DoD SPRS Scoring Methodology](https://www.acq.osd.mil/asda/dpc/cp/cyber/docs/safeguarding/NIST-SP-800-171-Assessment-Methodology-Version-1.2.1-6.24.2020.pdf)

---

Maintained by [Petronella Technology Group, Inc.](https://petronellatech.com) | Call 919-348-4912 for compliance assessment
