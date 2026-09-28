---
title: Contribution Workflow
description: Lightweight contribution process for humans and AI working in the UX knowledge repository.
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
  - ./governance/README.md
  - ./governance/knowledge-lifecycle.md
  - ./agent/intake-processing.md

tags:
  - contribution
  - workflow
  - governance
---

# Contribution Workflow

This repository is intentionally lightweight. It favors clarity, traceability, and practical value over bureaucratic process.

## Primary workflow

NEW SOURCE
→ intake

NEW ESTABLISHED KNOWLEDGE
→ appropriate /ux location

MEANINGFUL UX DECISION
→ decision record when necessary

CHANGE TO ACTIVE GUIDANCE
→ update version + provenance + relevant references

NEW AI FAILURE
→ consider regression eval

REPOSITORY HEALTH ISSUE
→ audit

## Contributor responsibilities

### Humans

- Add raw material to [intake/](./intake/README.md) when it may contain useful evidence.
- Prefer updating existing knowledge rather than creating near-duplicate files.
- Keep assumptions explicit and separate from validated guidance.
- Add or update provenance as needed.
- Flag repository health issues to governance and audits.

### AI agents

- Start with [UX.md](./UX.md) and the relevant detailed files.
- Verify whether the task is relevant to existing guidance before creating anything new.
- Distinguish evidence, synthesized knowledge, and inference.
- Recommend changes requiring human review rather than silently modifying validated content.
- Use evals and regression cases when significant UX guidance is affected.

## Documenting new knowledge

When a source is relevant to structured UX guidance, place it in the most appropriate [ux/](./ux/README.md) area. Common categories include:

- research summaries
- standards
- patterns
- glossary terms
- user models
- world or domain models
- references

Use the related templates in [governance/templates/](./governance/templates/README.md) when starting a new document.

## Making meaningful changes

A change should trigger a decision record only when the reasoning behind the decision is important to preserve and not obvious from the related knowledge files or Git history.

Do not create a decision record for trivial wording or formatting updates.

## Updating active guidance

When changing active guidance:

- update the document version when the change is meaningful
- update provenance with the new evidence or rationale
- adjust related references and linked knowledge
- confirm whether a regression eval or audit should also be updated
- keep the change reviewable in Git and PRs

## Regression and evaluation follow-up

If a new AI failure or product issue emerges:

- add or update a relevant eval case in [evals/](./evals/README.md)
- diagnose whether the cause is missing knowledge, ambiguity, contradiction, retrieval failure, or outdated guidance
- make the smallest correct corrective action
- do not automatically rewrite standards to satisfy an eval without human review

## Repository health follow-up

When a repository health issue is found:

- run the relevant audit checks
- document the issue and corrective action
- update metadata or governance files as needed
- decide whether the issue is purely operational or requires a UX decision

## Contribution principles

- Prefer a single source of truth.
- Avoid duplicate guidance and redundant documents.
- Preserve traceability.
- Keep uncertainty explicit.
- Prefer focused files over large monoliths.
- Maintain human readability alongside AI readability.

## Related files

- [intake/README.md](./intake/README.md)
- [governance/README.md](./governance/README.md)
- [audits/README.md](./audits/README.md)
- [evals/README.md](./evals/README.md)
- [agent/README.md](./agent/README.md)
