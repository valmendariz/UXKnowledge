---
title: Audit Reports
description: Repository for audit findings and issue tracking.
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
  - ../rules/README.md
  - ../../governance/templates/audit-report-template.md

tags:
  - audits
  - reports
---

# Audit Reports

This directory holds audit reports and issue documentation.

## Purpose

Audit reports identify repository or knowledge health issues and recommend the next actions. They should remain reviewable and actionable without rewriting guidance automatically.

## Typical audit findings

- missing metadata
- stale review dates
- broken links
- unsupported assumptions
- orphaned or duplicate knowledge
- overlap between standards and patterns
- unprocessed intake items

## Report workflow

- run the audit
- record findings
- label severity and owner
- assign recommended action
- require human review for any guidance change

## Template

Use [../../governance/templates/audit-report-template.md](../../governance/templates/audit-report-template.md).
