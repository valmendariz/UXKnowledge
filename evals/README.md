---
title: UX Evaluation Framework
description: Framework for measuring whether repository knowledge improves AI-generated UX work.
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
  - ../governance/README.md
  - ./cases/README.md
  - ./rubrics/README.md
  - ./results/README.md

tags:
  - evals
  - ai-evaluation
---

# Evaluation Framework

This folder defines how the repository is evaluated as a system for improving AI-assisted UX work.

## Intended purpose

Evals should not mainly test whether an AI can quote documentation. They should test whether an AI can apply repository knowledge correctly in realistic scenarios.

## Evaluation principles

- Measure behavior, not memorization.
- Prefer realistic prompts and scenarios over synthetic trivia.
- Test whether the AI retrieves relevant knowledge and applies it correctly.
- Keep evaluation dimensions explicit.
- Treat eval success as evidence of learning, not proof of correctness.

## Evaluation structure

- [cases/](./cases/README.md): evaluation scenarios and fixtures.
- [rubrics/](./rubrics/README.md): reusable scoring criteria.
- [fixtures/](./fixtures): support files for scenario setup and expected outputs.
- [results/](./results): evaluation outcomes and prior findings.

## Minimum case structure

Each case should include:

- ID
- title
- purpose
- scenario/input
- required context
- expected behaviors
- prohibited behaviors
- evaluation rubric
- failure severity
- related UX knowledge
- result/status

## Simple scoring model

Prefer a small, explicit score set such as:

- pass
- fail
- partial
- deferred

For dimension-level scoring, use a limited scale such as:

- 0 = not demonstrated
- 1 = partially demonstrated
- 2 = demonstrated

## Related documentation

- [cases/README.md](./cases/README.md)
- [rubrics/README.md](./rubrics/README.md)
- [../agent/README.md](../agent/README.md)
