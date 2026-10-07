# Cisco-based enterprise topology

```text
          [EDGE-01 Cisco]
                 |
          [SW-CORE-01]
            /    |    \
      VLAN 10 VLAN 20 VLAN 30
       USERS   SERVERS  ADMIN/SOC
        |        |         |
 FIN/HR/ENG   DC-01/02  ADMIN-01
              FILE-01    SOC-01
              APP-01
              AUT-01
```

- VLAN 10 — 10.20.10.0/24 — Employee workstations.
- VLAN 20 — 10.20.20.0/24 — Domain controllers, application and file servers.
- VLAN 30 — 10.20.30.0/24 — Administrative and SOC workstations.

This diagram is a conceptual design, not a deployed production topology. Use the supplied network flow evidence to establish observed connections, not to assume policy enforcement.
