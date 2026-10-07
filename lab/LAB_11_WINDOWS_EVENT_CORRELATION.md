# LAB-11 — Windows Event & Sysmon-like Correlation

**Role:** Senior Windows forensic analyst

## Objective
Work with event-shaped JSONL records rather than relying only on simplified CSV summaries.

## Tasks
- Correlate Windows Security-like 4624/4625 records with Sysmon-like process events.
- Explain what logon type and source address add to the investigation.
- Correlate directory group events with the simplified directory audit.
- Identify the synthetic log-clear event and determine what other sources survive it.
- Build a normalized event table containing record ID, UTC time, host, identity, event class, interpretation, and confidence.
- Compare your findings with the higher-level CSVs and identify any information lost by summarization.

## Deliverable
Windows Evidence Correlation Table plus a 300–500 word analyst note.

## Pass criteria
The analyst correlates sources rather than treating a Windows event ID as a verdict.
