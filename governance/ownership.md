---
title: Ownership
description: Ownership model for knowledge governance and review responsibilities.
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
  - ./review-policy.md
  - ./knowledge-lifecycle.md

tags:
  - ownership
  - governance
---

# Ownership

Ownership ensures that relevant people can decide what is authoritative, reviewable, and current.

## Ownership model

A file should declare:

- owner: the team or role accountable for the content
- last_reviewed: when the file was evaluated
- review_by: when it should be reviewed again
- status: whether it is active, review, draft, deprecated, or archived

## Who owns knowledge?

Ownership should be assigned to a functional area such as:

- design
- UX research
- product design
- content design
- design systems
- accessibility
- engineering/product partnership

If the repository is used across multiple groups, the owner should reflect the relevant accountable role, not just the file author.

## Ownership responsibilities

Owners are responsible for:

- validating whether the guidance is still correct
- confirming provenance and evidence
- reviewing changes that affect active guidance
- keeping file metadata current
- coordinating with governance when the rule changes materially

## Related governance

- [review-policy.md](./review-policy.md)
- [knowledge-lifecycle.md](./knowledge-lifecycle.md)
- [../governance/README.md](../governance/README.md)
