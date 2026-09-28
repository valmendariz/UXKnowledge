---
title: Audit Rules
description: Rule catalog for repository and knowledge health checks.
knowledge_type: reference
status: active
owner: UX
version: 0.1.0
created: 2026-09-28
last_updated: 2026-09-28
last_reviewed: 2026-09-28
review_by: 2026-10-28

evidence_level: validated

sources:
  - type: reference
    reference: repository-audit-framework

related:
  - ../README.md
  - ../../governance/README.md

tags:
  - audits
  - rules
---

# Audit Rules

This directory contains guidance for auditing repository health and knowledge integrity.

## Deterministic rules

- Every important document should include a required metadata set when needed.
- Every file should have a valid owner and status when it is in active use.
- Review dates should be refreshed before they become stale.
- Relative links should resolve to existing files.
- Source references should exist when provenance is required.
- A glossary should not contain duplicate terms without a clear reason.
- Deprecated guidance should not continue to be presented as active.
- Intake files should be processed or explicitly triaged.

## Semantic rules

- Document contradictions when two files imply different guidance.
- Flag weak provenance or unsupported claims.
- Check whether a rule is clear enough to be applied consistently.
- Flag knowledge that may be stale due to changed product context or newer evidence.
- Check whether a document is becoming too large or too broad for its stated purpose.

## Example issue categories

- missing metadata
- invalid status values
- missing source references
- contradictory rules
- generic but unsupported guidance
- orphaned documents
- stale review dates
- intake backlog

## Related files

- [../reports/README.md](../reports/README.md)
- [../../governance/templates/audit-report-template.md](../../governance/templates/audit-report-template.md)
