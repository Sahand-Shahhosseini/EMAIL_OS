# EMAIL_OS

Governed public source home of the Email-OS family.

## Purpose
This repository is the versioned public-source home for:
- Email-OS operational-model specifications
- ingestion and stable-message-identity doctrine
- rules and triage specifications
- backfill, pipeline and reporting specifications

## Role in the constellation
This repo removes the Email-OS family from long-term provisional concentration in `sahand-account-core`.
It is a family-specific public documentation/source repo, not an account-wide routing repo and not a mailbox data store.

## In scope
- Email-OS semantics
- message identity and dedup doctrine
- triage and rules specifications
- backfill/pipeline/reporting specifications
- future schema and implementation hardening that contains no private mailbox payload

## Out of scope
- account-wide routing law
- unrelated automation families
- raw inbox exports as source of truth by themselves
- generic project-registry or DB-core doctrine
- credentials, tokens, email bodies, attachments, personal mailbox metadata or private user conversations

## Source of migration
The initial source set is migrating from `sahand-account-core`.
After reviewed migration, `sahand-account-core` should keep bridge/reference stubs without duplicating family ownership.

## Repository authority boundary
This public repository is source authority for its observed versioned files only. Gmail or the relevant mail provider remains authoritative for live messages and labels; user permission remains authoritative for mail actions.

```text
Public repository != private mailbox
Repository source home != Canon_N
Email specification != executed mail action
Airtable projection != Gmail live state
Draft/triage rule != send/delete permission
Architecture != implementation != validation
```

No message send, forward, archive, delete, label mutation or bulk processing is authorized by repository content alone. Those actions require current mailbox context, explicit permission, privacy checks, operation-specific evidence and backcheck.

Airtable control: `GH_WRITEBACK_PATCH_EMAIL_OS_README_AUTHORITY_20260716_V1`  
GitHub audit WAL: `GH_WAL_20260716_ACCOUNT_REPO_AUDIT_W11_001`
