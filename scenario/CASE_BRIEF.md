# IdentityBreak — Senior Case Brief

**Case:** WB-IR-026  
**Organization:** Westbridge Logistics — fictional training organization  
**Evidence date:** 2026-09-23  
**Canonical investigation time:** UTC  
**Initial report:** 10:20 UTC  
**Classification:** Suspected Identity Compromise / Data Breach / Encryption Event

The SOC receives an alert after an unexpected permissions change to a finance share. Minutes earlier, a privileged Active Directory identity was observed authenticating from a normal employee workstation rather than the designated administration segment. During the same investigation window, selected sensitive files were accessed, staging-like artifacts appeared, unusual outbound traffic was recorded, and several files later became unreadable.

The legitimate account owner reports performing approved morning maintenance from ADMIN-01. That statement is an investigative lead and must be corroborated.

Several sources contain benign activity designed to resemble suspicious behavior. One telemetry source also has a documented clock offset. Some potentially useful records are absent. Analysts must not fill evidence gaps with assumptions.

## Mission

Determine:
- the earliest defensible suspicious activity;
- the identities and systems involved;
- the confirmed lateral movement;
- Active Directory and permission modifications;
- what sensitive data was discovered or accessed;
- whether data staging occurred;
- whether the evidence supports attempted or confirmed exfiltration;
- the scope and sequence of selective encryption;
- whether anti-forensic behavior is supported;
- the defensible breach scope and response priorities.

All names, addresses, data labels, and events are synthetic. No real enterprise is represented.
