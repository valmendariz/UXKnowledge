---
title: Eval Cases
description: Repository for evaluation scenarios and regression cases.
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
    reference: repository-evaluation-framework

related:
  - ../README.md
  - ../rubrics/README.md
  - ../../governance/templates/eval-case-template.md

tags:
  - evals
  - cases
---

# Eval Cases

This directory contains evaluation scenarios designed to test whether the repository supports real UX reasoning and generation.

## Categories

- [interaction-patterns/](./interaction-patterns): cases about interaction design patterns.
- [terminology/](./terminology): cases about consistent product language and glossary usage.
- [research-grounding/](./research-grounding): cases testing whether an AI uses evidence appropriately.
- [user-models/](./user-models): cases testing assumptions about users and context.
- [regression/](./regression): repeated failure cases that should not silently recur.

## Case template

Use [../../governance/templates/eval-case-template.md](../../governance/templates/eval-case-template.md).

## Important rules

- Evals are for testing applied knowledge, not rote recall.
- A passing eval does not prove a standard is correct.
- A failing eval should prompt a diagnosis of knowledge gaps, contradictions, or retrieval failures.
- Regression cases should capture repeated mistakes and help prevent recurrence.
