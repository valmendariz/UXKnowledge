---
title: Audit System
description: Audit framework for repository and knowledge quality.
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
  - ../governance/README.md
  - ./rules/README.md
  - ./reports/README.md

tags:
  - audits
  - governance
---

# Audit System

The audit framework evaluates repository health and UX knowledge health. Its purpose is to ensure that knowledge remains reviewable, traceable, and usable by humans and AI agents.

## Types of audit

### Deterministic audits

These checks can be automated safely:

- missing required metadata
- invalid metadata values
- missing owner
- overdue review dates
- broken relative links
- missing source references
- orphaned knowledge files
- duplicate glossary terms
- deprecated guidance still referenced as active
- intake files remaining unprocessed
- files that are excessively large

### Semantic audits

These checks require human or AI judgment:

- contradictions between guidance files
- duplicate guidance that is not obvious from metadata
- unclear or weak rules
- weak provenance
- potentially stale knowledge
- ambiguous standards with insufficient evidence

## Standard audit workflow

AUDIT REQUESTED
↓
DEFINE SCOPE
↓
RUN DETERMINISTIC CHECKS
↓
RUN SEMANTIC REVIEW
↓
DOCUMENT FINDINGS
↓
RECOMMEND NEXT ACTION
↓
HUMAN REVIEW IF NEEDED

## Important rule

Audit results should not automatically rewrite UX guidance. They should surface issues and give the team a basis for review.

## Related areas

- [rules/](./rules/README.md)
- [reports/](./reports/README.md)
- [../governance/README.md](../governance/README.md)
