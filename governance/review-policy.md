---
title: Review Policy
description: Standards for how UX knowledge is reviewed, approved, and refreshed.
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
    reference: repository-governance

related:
  - ./README.md
  - ./knowledge-lifecycle.md
  - ./ownership.md

tags:
  - review
  - governance
---

# Review Policy

This repository uses lightweight, meaningful review practices. Reviews should focus on whether the knowledge is still correct, useful, and traceable.

## Review expectations

A knowledge file should be reviewed when:

- it is first added as structured knowledge
- it changes materially
- evidence or assumptions change
- the owning area or governance context changes
- the file is close to becoming stale

## Review triggers

A document may require review because of:

- new contradictory evidence
- outdated guidance
- missing provenance
- a significant product or UX change
- a new AI failure or evaluation result

## Review cadence

The team should define a cadence that fits the repository. A general default is a periodic review at a set interval, with more frequent review when the guidance is actively used in generation or product work.

## Review decision

A review may result in:

- no change needed
- update to a file
- status change to deprecated or archived
- request for additional research
- recommendation for a decision record

## Important principle

Review does not automatically transform raw evidence into approved guidance. Review is a governance checkpoint, not a replacement for traceability.

## Related governance

- [knowledge-lifecycle.md](./knowledge-lifecycle.md)
- [ownership.md](./ownership.md)
- [../audits/README.md](../audits/README.md)
