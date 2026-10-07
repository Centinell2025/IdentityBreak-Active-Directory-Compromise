# IdentityBreak — Case Brief

**Case:** WB-IR-026 | **Organization:** Westbridge Logistics (fictional)
**Evidence date:** 2026-09-23 | **Time zone:** UTC
**Reported:** 10:20 UTC

A SOC analyst receives an alert after the permissions of a finance share on FILE-01 change unexpectedly. A privileged identity has authenticated from a workstation outside the designated administration VLAN. The account owner reports routine maintenance from ADMIN-01 that morning.

The analyst must distinguish normal activity from a potential identity compromise, reconstruct an evidence-backed timeline, identify changes to directory groups and server access, and state which conclusions remain unproven.

All event records are fictional training material. A successful logon does not identify the human at the keyboard.

## Enterprise assets

| Asset | Role | IPv4 |
| --- | --- | --- |
| WIN-FIN-04 | Finance workstation | 10.20.10.14 |
| WIN-HR-02 | HR workstation | 10.20.10.22 |
| WIN-ENG-09 | Engineering workstation | 10.20.10.39 |
| ADMIN-01 | Admin workstation | 10.20.30.11 |
| DC-01 | Primary domain controller | 10.20.20.10 |
| DC-02 | Secondary domain controller | 10.20.20.11 |
| FILE-01 | File server | 10.20.20.20 |
| APP-01 | Application server | 10.20.20.25 |
| AUT-01 | Deployment automation | 10.20.20.40 |
| SOC-01 | Analyst workstation | 10.20.30.15 |

**Domain:** westbridge.example
