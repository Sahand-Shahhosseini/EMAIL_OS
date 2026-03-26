# EMAIL_OS — Canonical Anchors v0.1

Date: 2026-03-23
Status: Canonical draft imported from Batch I
Source class: selected Email-OS operational extraction aligned with account canon

## Purpose
Record the minimum canonical anchors for Email-OS before a dedicated `EMAIL_OS` repo is created.

## Imported anchors

### Anchor E1 — Email-OS role
Email-OS is a live operational module, not a conceptual note.
Its purpose is to ingest Gmail-derived state into structured storage and make inbox state machine-readable.

### Anchor E2 — main object family
The central object family includes at minimum:
- email records keyed by stable message identity
- rule objects
- classification / priority / status fields
- due / follow-up timing fields
- sync / backfill state objects

### Anchor E3 — stable message identity
A stable email identity such as `gmail_message_id` is required as the core dedup/upsert key.
This is one of the main reasons Email-OS can behave as an operational system rather than a pile of rows.

### Anchor E4 — live ingestion exists
Email-OS is one of the few account systems explicitly described as already operating on live data.
This distinguishes it from purely speculative modules.

### Anchor E5 — rules are structural, not decorative
Rules are not merely metadata.
They are intended to become executable or at least translatable into executable logic over incoming email state.

### Anchor E6 — reporting requirement
Email-OS requires recurring report output over inbox state rather than subjective summaries.
This includes at minimum daily or weekly machine-readable status reporting.

## Boundary of this import
This import does NOT promote:
- the entire Airtable grid export as canon
- all rows in the email table as account truth
- all future automation code as already complete

It promotes only the minimum anchors needed to treat Email-OS as a real account-level module.

## Canonical interpretation
These anchors now live in `EMAIL_OS` as the dedicated semantic home of the family.
