# EMAIL_OS — Rules and Triage Anchors v0.1

Date: 2026-03-23
Status: Canonical draft imported from Batch I
Source class: selected Email-OS operational extraction aligned with account canon

## Purpose
Record the minimum rules/triage anchors that make Email-OS a workflow system rather than a static inbox mirror.

## Imported anchors

### Anchor R1 — rules are first-class objects
Email-OS contains explicit rule objects rather than only row-level tags.
Rules are expected to decide or help decide:
- category
- urgency
- next action
- follow-up timing
- archival/ignore state

### Anchor R2 — triage is machine-readable
Triage state is intended to be computable from explicit fields and rules.
At minimum, priority and status must be representable independently of raw email text.

### Anchor R3 — daily actionability
Email-OS is not only for storage.
It is intended to surface what requires action today, what can wait, and what is blocked or informational.

### Anchor R4 — human-in-the-loop but structured
The human operator may still review or override, but overrides should land on structured fields rather than free-text chaos.

### Anchor R5 — report-oriented state
Triage and rule outputs should support recurring machine-readable reports over inbox condition, not just ad hoc manual inspection.

### Anchor R6 — policy drift is a risk
If rule logic and table fields drift apart, the system degrades into inconsistent bookkeeping.
Therefore Email-OS requires an explicit law linking rules, fields, and reporting outputs.

## Boundary of this import
This import does NOT promote:
- every individual Airtable field as frozen canon
- every temporary rule experiment as locked law
- implementation code for every automation path

It promotes only the minimum rules/triage anchors needed to keep Email-OS operationally coherent.

## Canonical interpretation
These anchors now live in `EMAIL_OS` as the dedicated semantic home of the family.
