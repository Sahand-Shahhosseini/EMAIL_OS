# EMAIL_OS

Canonical home of the Email-OS family.

## Purpose
This repository is the semantic home for:
- Email-OS operational model
- ingestion and stable message identity doctrine
- rules and triage law
- backfill, pipeline, and reporting canon

## Role in the constellation
This repo exists to remove the Email-OS family from long-term provisional concentration in `sahand-account-core`.
It is a family-specific operational canon repo, not an account-wide routing repo.

## In scope
- Email-OS semantics
- message identity and dedup doctrine
- triage and rules law
- backfill/pipeline/reporting canon
- future Email-OS schema and implementation hardening

## Out of scope
- account-wide routing law
- unrelated automation families
- raw inbox exports as source of truth by themselves
- generic project-registry or DB-core doctrine

## Source of migration
The initial canon of this repo is migrating from `sahand-account-core`.
After migration, `sahand-account-core` should keep only bridge/reference stubs.

## Canonical direction
This repo should become the unique semantic home of the Email-OS family.
