# IdentityBreak — Active Directory Compromise

**Hack The Box Sherlock candidate | Hard / Senior DFIR | Synthetic Training Scenario**

IdentityBreak is an advanced enterprise digital-forensics exercise centered on an identity compromise that develops into a suspected data breach. The analyst must reconstruct what can actually be proven about privileged account abuse, lateral movement, sensitive-data discovery, staging, selective encryption, possible exfiltration, anti-forensic activity, and incident scope.

## TRAINING & EDUCATIONAL USE NOTICE

IdentityBreak — Active Directory Compromise is a fictional cybersecurity training scenario developed exclusively for technical education, DFIR training, SOC analyst development, and incident-response exercises.

All organizations, employees, accounts, domains, IP addresses, systems, documents, events, logs, and attack activity represented in this exercise are fictional or synthetically generated. The scenario does not represent, reproduce, or disclose an incident involving any real company or individual. No real customer, employee, credential, confidential information, or production infrastructure is included.

Students must perform analysis only against evidence and laboratory resources specifically provided with the exercise. No executable malware, credential-stealing payload, or operational intrusion tooling is supplied.

## Senior learning objectives

- Build a normalized cross-source forensic timeline.
- Separate legitimate administration and automation from anomalous behavior.
- Analyze Active Directory identity and group changes.
- Scope lateral movement and privileged access.
- Distinguish sensitive-data discovery, staging, transfer attempts, and confirmed exfiltration.
- Analyze selective encryption without executing ransomware.
- Detect evidence gaps and possible anti-forensic activity.
- State findings using defensible confidence levels.
- Preserve evidence while recommending containment and recovery.

## Student workflow

1. Read the case brief, evidence guide, asset inventory, and time notes.
2. Verify the evidence manifest.
3. Correlate endpoint, identity, directory, server, DNS, proxy, firewall/NetFlow, file-system, encryption, and collection records.
4. Answer the 15 senior questions using exact artifact/event IDs.
5. Produce the incident report and breach-scope matrix.

**Critical rule:** an attacker claim, successful logon, file read, archive creation, or outbound connection is not by itself proof that data was exfiltrated.

## Status

Development / playtest stage. The public repository contains student-facing material only. The validated answer key and author write-up must remain private. Final HTB packaging has not yet been completed.

Beacon of the Eagle LLC — Centinell Suite Defense.
