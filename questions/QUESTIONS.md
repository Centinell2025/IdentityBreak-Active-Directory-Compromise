# IdentityBreak — 15 Senior DFIR Questions

**Required answer format:** cite artifact filename, event/record ID, normalized UTC time, reasoning, and confidence. Where evidence is insufficient, say so.

1. **Initial anomaly:** What is the earliest endpoint activity that merits escalation? Corroborate it with at least one independent source and explain why earlier events are less significant.
2. **Identity attribution:** Which user context is associated with the initial sequence, and what prevents attribution of those actions to the human account owner?
3. **Administrative baseline:** Establish the legitimate privileged administrator's normal source and approved activity using at least two evidence families.
4. **Privileged identity abuse:** Identify the earliest anomalous attempt to use the privileged identity from a non-administrative source. Was the first attempt successful? What happened next?
5. **Lateral movement:** Reconstruct the confirmed path from the suspicious workstation to enterprise servers. Distinguish proven hops from inferred ones.
6. **Active Directory manipulation:** Identify the temporary membership change and the later directory changes that create a separate access path. Explain their security significance without assuming motive.
7. **Persistence assessment:** Does the evidence support persistence? Identify the strongest artifact(s), alternative explanations, and your confidence level.
8. **Sensitive-data discovery:** Which records demonstrate that potentially sensitive business information was located or enumerated before the encryption event?
9. **Data staging:** What evidence supports preparation or aggregation of data for transfer? Identify the source paths, staging artifact, approximate size, and relevant timestamps.
10. **Exfiltration assessment:** Determine whether the evidence proves successful data exfiltration, an attempted transfer, or only suspicious outbound communication. Correlate DNS, proxy, firewall/flow, staging, and collection evidence.
11. **Selective encryption:** Determine the first supported encryption-related event, affected dataset, and approximate scope. Do not rely solely on file extensions.
12. **Anti-forensics:** Which records suggest deletion, log clearing, timestomping, or another attempt to reduce visibility? Which independent artifacts still preserve evidence of the activity?
13. **Clock normalization:** One source is offset from canonical UTC. Identify it, calculate the offset, and explain how correcting it changes the incident timeline.
14. **Breach scope:** Classify relevant identities, hosts, and data into **Confirmed Compromised**, **Potentially Exposed**, **Observed but Unconfirmed**, or **No Evidence of Compromise**. Justify each classification.
15. **Senior incident decision:** Provide an executive conclusion addressing identity compromise, data breach, exfiltration status, encryption, and evidentiary limitations. Prioritize preservation, containment, eradication, recovery, and monitoring actions without destroying evidence.

## Evidence discipline

Do not treat an account name as proof of the human operator. Do not treat an archive as proof of theft. Do not treat outbound bytes as proof that the staged files were transmitted. Do not treat an attacker claim as proof. Your conclusion must be reproducible from the supplied evidence.
