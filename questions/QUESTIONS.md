# Sherlock — Ten investigation questions

For every answer, reference the event ID, UTC timestamp, and source file. Separate observation from inference.

1. Which workstation exhibits the earliest unusual process behavior and at what time?
2. Which user context is associated with that process? Why does this not by itself establish who operated the workstation?
3. Identify the administrator's normal source and corroborate approved activity with two sources.
4. Which earliest authentication attempt suggests privileged identity use from a different workstation, and was it successful?
5. Which two servers were accessed with the privileged account from the unusual source? Compare authentication and network artifacts.
6. Which temporary membership change was reversed and which subsequent group operations warrant further examination?
7. Which finance-share permission change is evidenced, and what later file activity followed?
8. Which suspicious-looking scripting activity has a plausible routine engineering or automation explanation?
9. Does the evidence prove data exfiltration, or only access? Explain the evidentiary limits.
10. Recommend three proportionate containment and evidence-preservation steps supported by the evidence.

Do not assume the name of an account identifies the person who used it.
