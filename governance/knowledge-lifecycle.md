---
title: Knowledge Lifecycle
description: Lifecycle states for UX knowledge from raw source to archive.
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
  - ./ownership.md

tags:
  - lifecycle
  - provenance
---

# Knowledge Lifecycle

UX knowledge should move through a clear lifecycle from raw evidence to known, reviewable guidance.

## Lifecycle states

RAW
→ SYNTHESIZED
→ REVIEWED
→ VALIDATED
→ DEPRECATED
→ ARCHIVED

### RAW

Material collected from intake or external evidence. This state indicates that a source exists but has not been evaluated as established knowledge.

### SYNTHESIZED

A source has been classified and summarized, and a preliminary interpretation has been created. At this point, the content is likely useful but not yet approved.

### REVIEWED

A synthesis or document has been checked by a human or designated reviewer. It may still need broader validation before becoming active guidance.

### VALIDATED

The document is accepted as current and relevant guidance. It has sufficient provenance and review history to be trusted in active UX work.

### DEPRECATED

The guidance is still in the repository but should no longer be treated as active. It may be retained for historical context or to explain why a decision changed.

### ARCHIVED

The document is retained only for historical or compliance reasons. It is intentionally no longer active guidance and should not be used unless explicitly required.

## Status vs evidence level

These concepts should remain separate:

- status = whether guidance is currently in use
- evidence_level = how strongly the knowledge has been reviewed or validated

For example, a file may be active but still only synthesized if the team has not completed full review. Another file may be deprecated but have high provenance because it is still useful for historical understanding.

## Related governance

- [review-policy.md](./review-policy.md)
- [ownership.md](./ownership.md)
- [../UX.md](../UX.md)
