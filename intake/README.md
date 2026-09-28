---
title: Intake Lifecycle
description: Rules for adding, classifying, and processing raw UX evidence before it can become governed knowledge.
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
    reference: repository intake process

related:
  - ../UX.md
  - ../governance/knowledge-lifecycle.md
  - ../agent/intake-processing.md

tags:
  - intake
  - provenance
  - evidence
---

# Intake

The intake area holds unreviewed source material. These files are evidence, not authoritative UX guidance.

## Non-authoritative status

Files in [new/](./new) are not approved knowledge. They may contain useful research notes, exported documentation, workshop notes, meetings, transcripts, design notes, design system material, product documentation, references, or other UX evidence.

Processing a file does not validate it. A file can be processed and still be rejected or remain unapproved.

## Lifecycle

SOURCE ADDED
↓
INSPECT
↓
CLASSIFY
↓
CHECK EXISTING KNOWLEDGE
↓
DETECT DUPLICATES / CONTRADICTIONS
↓
SYNTHESIZE
↓
PROPOSE KNOWLEDGE CHANGES
↓
REVIEW
↓
UPDATE STRUCTURED KNOWLEDGE
↓
AUDIT
↓
MOVE SOURCE TO PROCESSED

## Required handling

When a new file arrives:

1. Inspect the source and summarize what it contains.
2. Identify relevant knowledge categories.
3. Search existing materials before creating new knowledge.
4. Detect duplicates and contradictions.
5. Check whether the source is outdated or superseded.
6. Preserve provenance and source references.
7. Determine whether an existing file should be updated or a new file should be created.
8. Record proposed changes requiring human review.
9. Move the source to [processed/](./processed) only after it has been processed and classified.

## Intake folders

- [new/](./new): inbox for raw sources before processing.
- [processed/](./processed): files that have been processed but are not necessarily approved.
- [rejected-or-duplicate/](./rejected-or-duplicate): sources rejected as duplicates or irrelevant.

## Important rules

- Raw intake material never overrides validated guidance.
- A file in processed does not imply approval.
- AI-generated summaries are not source evidence.
- New findings should be linked to the relevant structured knowledge and review status.
- Human review must be recorded for any meaningful proposed change.

## Processing instructions for AI agents

See [../agent/intake-processing.md](../agent/intake-processing.md).

## Related knowledge areas

- [../ux/README.md](../ux/README.md)
- [../governance/knowledge-lifecycle.md](../governance/knowledge-lifecycle.md)
- [../governance/review-policy.md](../governance/review-policy.md)
