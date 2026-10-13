<div align="center">
  <img src="https://raw.githubusercontent.com/Centinell2025/the-last-evidence-standing/main/branding/BEACON_SEAL.png" alt="Beacon of the Eagle LLC — logotipo corporativo" width="165" />
  <p><strong>BEACON OF THE EAGLE LLC</strong><br/><strong>CENTINELL SUITE DEFENSE</strong></p>
</div>

# IdentityBreak — Active Directory Compromise

> **Advanced Senior DFIR Training Scenario**  
> Active Directory • Identity Compromise • Data Breach • Data Exfiltration Analysis • Selective Encryption • Digital Forensics • Incident Response

**IdentityBreak — Active Directory Compromise** is a fictional enterprise investigation designed to train cybersecurity technicians, SOC analysts, incident responders, and digital forensic investigators in the analysis of a complex Active Directory compromise and suspected data breach.

The challenge is intentionally evidence-driven. Students are not expected to identify a single suspicious event and stop. They must correlate multiple forensic sources, reconstruct the incident timeline, distinguish legitimate administration from unauthorized activity, determine the scope of affected data, evaluate evidence of staging and outbound transfer, analyze selective encryption, identify evidence gaps, and produce a defensible incident conclusion.

---

## Training & Educational Use Notice

This repository is intended **exclusively for cybersecurity education, technical training, DFIR exercises, and authorized laboratory use**.

Westbridge Logistics and every employee, account, document, event, IP address, domain, system, alert, and incident represented in this challenge are fictional or synthetically generated for training.

This scenario:

- does **not** represent or disclose an incident involving a real company or individual;
- contains no real customer or employee information;
- contains no real credentials or confidential enterprise information;
- contains no production infrastructure;
- contains no executable ransomware or credential-stealing malware;
- does not require students to attack or access any third-party system.

Students should analyze only the evidence and authorized laboratory resources supplied with the exercise.

---

## Scenario

The SOC receives an alert after an unexpected permissions change is detected on a sensitive finance share.

During initial triage, investigators discover that a privileged Active Directory identity has authenticated from a standard employee workstation rather than the designated administrative segment.

The legitimate administrator reports performing approved maintenance earlier that morning from **ADMIN-01**.

As the investigation expands, additional evidence indicates:

- anomalous endpoint activity;
- privileged authentication from an unexpected source;
- Active Directory group modifications;
- access to multiple enterprise servers;
- discovery of sensitive business information;
- creation of a possible staging artifact;
- outbound network communications;
- deletion and logging gaps;
- selective encryption of business files.

Management wants to know:

> **Was sensitive information actually stolen, what systems and identities were compromised, what was encrypted, and what can the forensic evidence prove?**

The student must answer those questions without treating assumptions, attacker claims, or isolated alerts as facts.

---

## Difficulty

**Target level:** Hard / Senior  
**Primary discipline:** DFIR  
**Secondary disciplines:** Active Directory, SOC Investigation, Network Forensics, Incident Response, Data Breach Analysis

This challenge is designed to require correlation across multiple evidence families rather than simple keyword searches.

---

## Investigation Objectives

By completing IdentityBreak, the analyst should be able to:

1. establish evidence provenance and limitations;
2. normalize timestamps across different sources;
3. identify the earliest defensible suspicious activity;
4. distinguish legitimate administration and automation from anomalous behavior;
5. investigate privileged Active Directory identity misuse;
6. reconstruct confirmed lateral movement;
7. analyze directory and permission modifications;
8. identify sensitive-data discovery and access;
9. distinguish data access from data staging;
10. assess attempted versus confirmed exfiltration;
11. analyze the forensic effects of selective encryption;
12. identify potential anti-forensic behavior and evidence gaps;
13. reconstruct activity when local logs are incomplete;
14. determine breach scope using confidence levels;
15. recommend evidence-preserving containment, eradication, recovery, and monitoring.

---

## Evidence Set

The repository contains synthetic training evidence representing several enterprise telemetry sources:

| Evidence family | Investigative purpose |
| --- | --- |
| Windows Security-like events | Authentication and directory activity |
| Sysmon-like events | Endpoint process correlation |
| Active Directory audit | Group and identity changes |
| Server audit | Share, ACL, and server activity |
| DNS telemetry | Name-resolution correlation |
| Firewall / flow telemetry | Internal and outbound connections |
| Cisco ASA-like logs | Network security correlation |
| NetFlow-like records | Communication timing and volume |
| Proxy records | Application-layer outbound activity |
| File-system timeline | File access, creation, deletion, and modification |
| MFT/USN-like records | File-system forensic reconstruction |
| Collection telemetry | Sensitive-data discovery and staging |
| Encryption telemetry | Safe simulation of selective encryption effects |
| Anti-forensic observations | Log gaps, deletion, and metadata changes |
| Acquisition records | Evidence handling and provenance |

Files identified as **`*_like`** reproduce useful investigative structure for training; they are not represented as native exports from real customer systems.

---

## Senior Investigation Questions

The Sherlock contains **15 senior-level investigation questions** covering:

- initial anomaly;
- identity attribution;
- administrative baseline;
- privileged identity abuse;
- lateral movement;
- Active Directory manipulation;
- persistence assessment;
- sensitive-data discovery;
- data staging;
- exfiltration assessment;
- selective encryption;
- anti-forensics;
- clock normalization;
- breach scope;
- senior incident decision.

See **`questions/QUESTIONS.md`** for the complete student question set.

---

## Practical Laboratory Track

IdentityBreak includes a progressive practical training path with **14 laboratories**:

| Lab | Focus |
| --- | --- |
| LAB-01 | Evidence Intake & Chain of Custody |
| LAB-02 | Windows Endpoint Triage |
| LAB-03 | Active Directory Identity Investigation |
| LAB-04 | Lateral Movement Reconstruction |
| LAB-05 | Cisco / Network Forensics |
| LAB-06 | Sensitive Data Discovery & Staging |
| LAB-07 | Exfiltration Assessment |
| LAB-08 | Selective Encryption Forensics |
| LAB-09 | Anti-Forensics & Timeline Recovery |
| LAB-10 | Breach Scope & Senior Incident Response |
| LAB-11 | Windows Event & Sysmon-like Correlation |
| LAB-12 | MFT/USN-like File-System Forensics |
| LAB-13 | Cisco / NetFlow Correlation |
| LAB-14 | Forensic Engineering Capstone |

The final capstone requires the analyst to move from evidence intake through technical investigation and finish with a defensible executive incident decision.

See **`lab/README.md`** for the laboratory track.

---

## Evidence Discipline

IdentityBreak deliberately teaches analysts not to overstate conclusions.

A successful logon does not prove which human used the account.

A file read does not prove the information left the organization.

Creation of an archive does not prove that archive was exfiltrated.

Outbound bytes do not identify the content of those bytes.

An HTTP success status does not independently prove that a complete sensitive dataset was received externally.

An attacker or extortion claim is not independent forensic proof.

Missing logs do not prove that an event did not occur.

**The strongest acceptable conclusion is the strongest conclusion supported by the evidence — no more.**

---

## Student Deliverables

Students may be required to produce:

- answers to the 15 investigation questions;
- an evidence register;
- normalized UTC master timeline;
- identity-compromise assessment;
- confirmed and hypothetical incident-path diagrams;
- network correlation matrix;
- data-staging assessment;
- exfiltration assessment;
- encryption impact report;
- recovered timeline across evidence gaps;
- breach-scope matrix;
- containment and recovery plan;
- technical incident report;
- executive summary.

Reusable templates are provided under **`reports/`** and **`lab/`**.

---

## Repository Structure

```text
IdentityBreak-Active-Directory-Compromise/
├── artifacts/
│   ├── data/
│   ├── encryption/
│   ├── endpoint/
│   ├── filesystem/
│   ├── forensics/
│   ├── identity/
│   ├── incident/
│   ├── network/
│   ├── server/
│   ├── time/
│   └── windows/
├── lab/
├── questions/
├── reports/
├── scenario/
├── validation/
├── README.md
└── TRAINING_NOTICE.md
```

---

## Analyst Standard

Every material finding should identify:

**Artifact → Record/Event ID → Timestamp → Observation → Corroboration → Interpretation → Confidence → Limitation**

Students must clearly distinguish:

- **Observed Fact**
- **Analyst Inference**
- **Investigative Hypothesis**
- **Unsupported Claim**

---

## Safety

No executable malware is required or provided.

Encryption activity is represented through safe synthetic forensic artifacts. The challenge is about investigating the effects of an incident, preserving evidence, determining scope, and planning recovery — not reproducing destructive behavior.

Laboratory work must remain within authorized, isolated training environments.

---

## Development Status

**Status: Development / Playtest**

Before a final platform submission, the evidence set should be frozen, cryptographic hashes generated, all 15 questions independently playtested, the private answer key validated, and the final challenge package checked against the current platform requirements.

The public repository intentionally contains **student-facing material only**. The instructor solution and validated answer key must remain private.

---

## Organization

**Beacon of the Eagle LLC**  
**Centinell Suite Defense**

IdentityBreak is part of the Centinell Suite Defense cybersecurity training and digital-forensics research portfolio.


---
**Ethical and educational use / Uso ético y educativo:** This is a fictional or simulated defensive cybersecurity training exercise. Test only systems you own or are explicitly authorized to assess. / Ejercicio de ciberseguridad defensiva ficticio o simulado. Realice pruebas solo en sistemas propios o con autorización expresa. See / Consulte [Educational Purpose Notice](EDUCATIONAL_PURPOSE_NOTICE.md).
