---
title: Knowledge Provenance
description: Rules for distinguishing canonical, evidence-backed, inferred, and speculative UX knowledge.
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
  - ../UX.md
  - ../README.md
  - ./knowledge-lifecycle.md

tags:
  - provenance
  - governance
---

# Knowledge Provenance

Traceability is a core requirement for this repository. Important guidance should make it possible to understand where the information came from, how it was reviewed, and what other knowledge depends on it.

## Provenance concepts

### CANONICAL

Established, approved knowledge that has been reviewed and accepted for active use.

### EVIDENCE

Research, observations, documentation, interviews, and other material that supports a decision or claim.

### INFERRED

A reasonable interpretation or synthesis that has not been formally established as a rule.

### SPECULATIVE

A hypothesis or assumption that requires validation before it should be trusted as guidance.

## Representation rules

This repository should distinguish these concepts without making every document unnecessarily complex.

- Use the document status and evidence_level fields to communicate governance-level trust.
- Use a sources section or evidence section when the document is based on underlying evidence.
- Mark inferred or speculative content in plain language when it is presented in a document.
- Never present AI-generated inference as source evidence.
- Keep raw evidence and synthesized content separate from approved guidance.

## Minimal representation pattern

```markdown
## Evidence

- Source A: studied behavior or internal document
- Source B: approved terminology reference

## Interpretation

This is an inferred conclusion and should not be treated as established guidance until reviewed.
```

## Why this matters

Without provenance, an AI agent may treat intake notes, synthesis, or assumptions as official policy. This repository avoids that by preserving the distinction between:

- canonical knowledge
- supporting evidence
- inferred conclusions
- unvalidated speculation

## Related governance

- [./knowledge-lifecycle.md](./knowledge-lifecycle.md)
- [./review-policy.md](./review-policy.md)
- [../UX.md](../UX.md)
