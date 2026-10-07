# Student Evidence Matrix

This matrix identifies useful source families without providing the solution.

| Investigation area | Primary evidence | Corroborating evidence |
| --- | --- | --- |
| Initial endpoint anomaly | endpoint/process_events.csv | network/dns_queries.csv, network/firewall_flows.csv |
| Admin baseline | identity/authentication.csv | endpoint/process_events.csv, server/server_audit.csv |
| Privileged identity anomaly | identity/authentication.csv | network/flow_records.csv |
| AD modifications | identity/directory_audit.csv | identity/persistence_review.csv |
| Server access | server/server_audit.csv | filesystem/file_timeline.csv |
| Sensitive-data discovery | data/collection_events.csv | filesystem/file_timeline.csv |
| Staging | filesystem/file_timeline.csv | data/collection_events.csv |
| Outbound transfer | network/firewall_flows.csv | network/proxy_requests.csv, network/dns_queries.csv |
| Encryption | encryption/encryption_events.csv | filesystem/file_timeline.csv |
| Anti-forensics | forensics/anti_forensics.csv | forensics/evidence_gaps.csv |
| Time normalization | time/source_time_notes.csv | matching request IDs in firewall/proxy |
| Breach scope | all relevant sources | reports/BREACH_SCOPE_TEMPLATE.csv |

The matrix is a navigation aid. It does not establish that an event is malicious or that exfiltration occurred.
