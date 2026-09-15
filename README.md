# 10-Minute Engineering Challenge

## SOC Incident Response Simulation

A premium, browser-based cybersecurity decision simulation designed to test how an analyst reasons under a ten-minute incident-response constraint.

**Live challenge:** https://sakilurrashid1-star.github.io/10-Minute-Engineering-Challenge/

### What it evaluates

- Cross-source alert triage
- IOC and telemetry correlation
- Containment with business-risk awareness
- Volatile evidence preservation
- Threat-hunting scope expansion
- Identity / endpoint / network pivots
- MITRE ATT&CK-oriented reasoning
- Executive incident communication
- Decision quality under time pressure

### Scenario

A finance workstation (`FIN-WS-042`) shows suspicious outbound beaconing. Shortly afterward, a privileged finance service account authenticates from the same environment. The analyst must determine what to investigate, what to contain, what evidence to preserve, how to scope the incident, and what leadership should be told.

### Architecture

```text
Telemetry
   ↓
Triage & Correlation
   ↓
Containment Decision
   ↓
Evidence Preservation
   ↓
Threat Hunting / Scope
   ↓
Executive Decision
   ↓
Readiness Score
```

### Engineering principles

1. **Evidence before certainty** — distinguish observations from hypotheses.
2. **Contain without unnecessary destruction** — reduce attacker reach while preserving investigative value.
3. **Scope systematically** — pivot across identity, endpoint, process, DNS and network dimensions.
4. **Communicate uncertainty explicitly** — a blocked indicator is not the same as eradication.
5. **Optimize for decision quality** — the objective is not to click the fastest answer; it is to make the safest defensible decision.

### Technical implementation

- Single-page HTML/CSS/JavaScript application
- Client-side state machine for the five-stage workflow
- Countdown timer with pressure states
- Deterministic scoring and readiness metrics
- Immediate evidence/decision feedback
- Responsive SOC-style interface
- Final incident handoff report generated in-browser
- No backend or external data dependency

> **Simulation notice:** all hosts, identities, indicators, timestamps and telemetry are synthetic and created for demonstration/education. They do not represent a real incident or real threat infrastructure.

## Project positioning

This project is intended as a flagship cybersecurity engineering artifact in Alkamah Sakilur Rashid's portfolio: a compact demonstration of security operations, analytical reasoning, evidence discipline and product-quality frontend engineering.
