# Evidence Guide

IdentityBreak is intentionally multi-source. No single artifact should be treated as the complete truth.

## Source families
- Endpoint process telemetry: process lineage and execution context.
- Authentication / directory audit: logons and AD object changes.
- File-system timeline: file creation, reads, deletes, renames and metadata.
- Server audit: share and permission activity.
- DNS: hostname resolution.
- Proxy: application-layer outbound request metadata.
- Firewall / NetFlow: observed network sessions and byte counts.
- Collection telemetry: synthetic DLP-style observation of file collection.
- Encryption telemetry: safe simulation of selective encryption effects.
- Forensic integrity: acquisition notes and hashes.

## Known limitations
- Process telemetry does not identify the human operator.
- Some command payloads were not retained.
- Proxy telemetry has a known clock offset; determine it from the evidence rather than assuming every displayed time is canonical.
- File reads show access, not necessarily disclosure.
- Flow byte counts do not prove which file contents crossed the network.
- A missing log is not proof that an event did not occur.

All artifacts are synthetic training records.
