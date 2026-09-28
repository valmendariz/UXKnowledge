---
title: UX Knowledge Contract
description: Entry point for AI and human readers to the governed UX knowledge repository.
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
  - ./README.md
  - ./ux/README.md
  - ./governance/README.md
  - ./agent/README.md

tags:
  - ux-knowledge
  - ai-context
  - repository-map
---

# UX Knowledge Contract

## Purpose

UX.md is the primary UX knowledge contract for this repository. It acts as the repository entry point, navigation layer, map, and interpretation guide for AI agents and human contributors.

UX.md is not intended to replace the underlying knowledge files. It does not hold every rule, evidence source, or decision record. Instead, it tells readers what the repository contains, how to interpret it, and where to look for authoritative guidance.

## How AI should use this repository

AI systems should use this repository in a layered way:

1. Start with UX.md to understand the repository context and the knowledge hierarchy.
2. Identify the task and determine which knowledge areas are relevant.
3. Retrieve the specific files needed for the decision, such as standards, patterns, research, terminology, or models.
4. Read the most relevant source material rather than summarizing from a single top-level entry.
5. Respect status, provenance, and evidence levels before making recommendations.
6. Surface uncertainty and missing knowledge instead of silently inventing UX rules.

This repository is meant to support application of knowledge, not to replace critical thinking. An AI agent should prefer precise, relevant evidence over general patterns.

## Knowledge hierarchy

When guidance conflicts, the repository should be interpreted in this order of authority:

1. Validated UX standards
2. Approved UX patterns
3. Research findings
4. User models
5. World or domain models
6. Glossary definitions
7. References
8. Raw intake material
9. AI inference

Important rules:

- Raw intake material never automatically overrides validated guidance.
- AI-generated inference must never be represented as established UX knowledge.
- The repository must preserve provenance so it is clear which statements are validated, evidence-backed, inferred, or speculative.
- If no validated guidance exists, the system should say so explicitly and present the gap.

## Required reading by task

| Task | Consult |
| --- | --- |
| Designing a form | relevant standards, patterns, and research |
| Creating an error state | error-handling standards, patterns, and terminology |
| Using domain terminology | glossary, standards, and references |
| Making assumptions about users | user models and research findings |
| Understanding domain relationships | world models and references |
| Proposing a new pattern | existing standards, patterns, and research findings |
| Reviewing repository quality | audits, governance, and ownership guidance |
| Evaluating AI output | eval cases, rubrics, and regression cases |

## Repository map

The repository is organized by knowledge type and operating system function.

- [ux/](./ux/README.md): structured UX knowledge areas.
  - [ux/research/](./ux/research/README.md): research summaries and evidence syntheses.
  - [ux/standards/](./ux/standards/README.md): approved standards and rules.
  - [ux/patterns/](./ux/patterns/README.md): reusable interaction patterns.
  - [ux/models/](./ux/models/README.md): user and domain/world models.
  - [ux/glossary/](./ux/glossary/README.md): controlled terminology.
  - [ux/references/](./ux/references/README.md): external and internal reference material.
- [intake/](./intake/README.md): inbox of unreviewed raw sources.
- [governance/](./governance/README.md): review policy, lifecycle, ownership, and documentation standards.
- [audits/](./audits/README.md): repository and knowledge health checks.
- [evals/](./evals/README.md): evaluation procedures, rubrics, and results.
- [agent/](./agent/README.md): instructions for AI agents.

## AI behavior

When operating in this repository, AI agents should behave in the following ways:

### Information is missing

- State clearly that the repository does not currently contain a relevant rule or model.
- Recommend the specific knowledge type that should be created or researched.
- Avoid inventing product behavior, user needs, or domain assumptions without evidence.

### Sources disagree

- Identify the disagreement explicitly.
- Explain which source has higher authority according to the knowledge hierarchy.
- Distinguish evidence, inference, and unresolved uncertainty.
- Recommend human review when the conflict affects product decisions.

### Guidance is outdated

- Honor deprecated or archived status markers.
- Do not treat outdated guidance as active unless a human explicitly re-validates it.
- Flag stale guidance when it appears in active design or generation flows.

### Guidance is ambiguous

- Surface the ambiguity.
- Identify the missing fact or decision needed to resolve it.
- Recommend a safe default only when that default is explicitly indicated and traceable to established guidance.

### Only raw evidence exists

- Treat the evidence as supporting material, not authoritative UX guidance.
- Summarize the evidence without elevating it to an established rule.
- Indicate what additional review or synthesis would be needed before it becomes valid guidance.

### The agent is making an inference

- Label the inference as inferred, speculative, or unvalidated.
- Identify the assumptions behind it.
- Clearly separate inference from evidence and approved knowledge.
- Do not present the inference as established UX guidance.

## Governance expectations

AI agents working in this repository should:

- start from relevant repository files instead of relying only on this document
- prefer validated, current guidance over unreviewed or speculative content
- distinguish evidence from interpretation
- cite or reference relevant repository files when explaining consequential UX decisions
- flag missing knowledge and recommend additions when repeated gaps appear
- respect deprecated guidance and provenance markers
- consider relevant eval cases for significant UX generation tasks

## Summary

The repository’s purpose is not to make every answer absolute. It is to support better, more traceable, and more reviewable UX decision-making. The system works when AI agents answer four questions clearly:

- What do we know?
- What evidence supports it?
- What UX rules apply?
- What do we not know?

When that is done consistently, the repository becomes a trustworthy knowledge layer for product, research, design, and AI assistance.
