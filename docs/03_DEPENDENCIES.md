# 03 Dependencies

Date: 2026-03-27
Status: Bootstrap scaffold
Purpose: record the minimum dependency surface of `EMAIL_OS`.

## Internal dependencies
- Email-OS canonical anchors
- rules and triage anchors
- backfill, pipeline, and reporting anchors

## External constellation dependencies
- account-law and routing references from `sahand-account-core`
- reporting or execution integrations may bridge outward
- inbox/connectors/tooling may vary without changing Email-OS semantic law

## Hard boundary
Email-OS may connect to external automation systems, but those systems do not become the semantic home of Email-OS.
