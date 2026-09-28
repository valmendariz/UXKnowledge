---
title: Regression Eval Cases
description: Cases for repeated AI failures and ambiguous UX decisions.
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
    reference: evaluation-framework

related:
  - ../README.md
  - ../../README.md

tags:
  - evals
  - regression
---

# Regression Eval Cases

Use this area to capture repeated UX failures and AI mistakes before they silently reappear.

## Lifecycle

AI GENERATION
↓
EVAL FAILURE
↓
DIAGNOSE FAILURE

Determine whether the failure came from:

- missing knowledge
- ambiguous knowledge
- contradictory knowledge
- retrieval failure
- reasoning failure
- outdated knowledge
- unsupported inference

Then determine whether to:

- improve documentation
- improve agent instructions
- add or change an eval
- flag for human UX decision

## Important rule

Do not automatically change UX guidance simply to make an eval pass.
