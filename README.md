---
title: UX Knowledge Repository
description: Human-facing orientation for the governed UX knowledge repository.
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
    reference: repository-architecture

related:
  - ./UX.md
  - ./CONTRIBUTING.md
  - ./governance/README.md
  - ./agent/README.md

tags:
  - repository
  - governance
  - ux-knowledge
---

# UX Knowledge Repository

This repository is a governed UX knowledge system for both humans and AI agents. It is designed to collect raw UX evidence, classify and synthesize it, and turn it into structured knowledge that can be reviewed, audited, and used responsibly in product design and AI-assisted generation.

## Purpose

The repository does not simply store UX documentation. It creates a controlled pipeline:

raw sources
→ intake
→ classification and synthesis
→ structured UX knowledge
→ human review
→ audits
→ evaluations
→ trusted context for AI generation

This makes the system useful for:

- UX designers and researchers
- product managers and design leads
- developers implementing product experiences
- design system contributors
- AI agents that need grounded UX context

## README vs UX.md

- README.md is the human orientation layer. It explains goals, participants, governance, contribution flow, and repository structure.
- UX.md is the primary knowledge entry point for AI agents and human contributors working with UX guidance. It is the repository contract and navigation layer, not a container for all knowledge.

## Repository architecture

- [intake/](./intake/README.md): unreviewed source material and intake workflow.
- [ux/](./ux/README.md): structured UX knowledge by domain type.
- [governance/](./governance/README.md): lifecycle, review policy, ownership, and documentation standards.
- [audits/](./audits/README.md): repository and knowledge quality checks.
- [evals/](./evals/README.md): application-focused AI evaluations and regression tracking.
- [agent/](./agent/README.md): instructions for AI agents operating in the repository.

## Who this is for

This repository is intended for teams that want a durable, reviewable, and AI-readable foundation for UX knowledge. It supports reuse across documentation, design work, product decisions, and AI-assisted generation without turning raw evidence or AI inference into treated fact.

## How intake works

New material enters through [intake/README.md](./intake/README.md). Intake files are evidence, not authoritative guidance. They must be inspected, classified, checked against existing knowledge, and processed before being accepted into structured UX knowledge.

## How governance works

Governance is defined in [governance/README.md](./governance/README.md), [governance/review-policy.md](./governance/review-policy.md), [governance/knowledge-lifecycle.md](./governance/knowledge-lifecycle.md), and [governance/ownership.md](./governance/ownership.md). This includes how knowledge types move from raw input to active guidance and when guidance should be deprecated or archived.

## How audits work

Audits evaluate repository health and knowledge health. They help detect missing metadata, stale review dates, weak provenance, contradictions, broken links, and outdated references. See [audits/README.md](./audits/README.md).

## How evals work

Evals test whether the repository improves real AI performance when applying UX knowledge, not whether an AI can quote documentation without context. See [evals/README.md](./evals/README.md).

## How AI agents should enter the repository

AI agents should begin with [UX.md](./UX.md). They should then retrieve the relevant detailed knowledge files needed for the task, apply provenance rules, distinguish established guidance from inference, and call out missing or conflicting information instead of silently inventing UX rules.

## Contribution model

See [CONTRIBUTING.md](./CONTRIBUTING.md) for a lightweight workflow covering sources, established knowledge, decision records, active guidance changes, audits, and regression evals.

## Important constraints

- Do not invent product-specific UX guidance.
- Intake is never authoritative.
- AI-generated inference must not be treated as validated knowledge.
- Maintain a single source of truth and avoid near-duplicate guidance.
- Preserve provenance and uncertainty explicitly.

## Change log

See [CHANGELOG.md](./CHANGELOG.md).
