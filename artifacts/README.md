# IdentityBreak Evidence

All artifacts in this directory are **synthetic training evidence**. Files named `*_like` imitate the structure or investigative purpose of common telemetry but are not raw exports from a real Windows, Cisco, NTFS, EDR, proxy, or customer environment.

## Why this matters
A student should learn realistic correlation concepts without being misled about artifact authenticity. A real enterprise investigation would require validation of native formats, acquisition tooling, system configuration, retention, clock synchronization, and cryptographic integrity.

## Major evidence families
- endpoint and Windows event-shaped telemetry;
- Active Directory authentication and directory audit;
- DNS, firewall, proxy, Cisco-ASA-like, and NetFlow-like network records;
- server audit;
- MFT/USN-like file-system metadata;
- data collection/staging telemetry;
- safe selective-encryption observations;
- anti-forensic observations and evidence gaps;
- acquisition records.

No executable malware or real confidential data is included.
