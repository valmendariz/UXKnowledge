---
title: Intake Processing Instructions
description: Operational guidance for an AI agent processing new UX evidence.
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
    reference: repository-agent-guide

related:
  - ./README.md
  - ./instructions.md
  - ../intake/README.md

tags:
  - agents
  - intake
---

# Intake Processing

This file instructs an AI agent on how to process unreviewed UX source material before it becomes structured knowledge.

## Required steps

1. Inspect the new source.
2. Summarize what the source contains.
3. Identify relevant knowledge categories.
4. Search existing UX knowledge before creating new content.
5. Detect duplicate information.
6. Detect contradictions.
7. Identify potentially outdated information.
8. Preserve provenance.
9. Determine whether an existing file should be updated or a new file should be created.
10. Never silently replace established guidance.
11. Clearly identify proposed changes requiring human review.
12. Record significant approved changes.
13. Move or recommend moving the source to [../intake/processed](../intake/processed) only after processing.

## Classify the source

The agent should classify the source by likely repository home, for example:

- research
- standard
- pattern
- terminology
- user model
- world model
- reference

## Check for duplication and contradiction

Before making a recommendation, the agent should compare the content with relevant repository files and note:

- whether it duplicates an existing record
- whether it conflicts with current active guidance
- whether it contradicts previous research or design decisions
- whether the contradiction implies a governance decision is needed

## Preserve provenance

The agent should document:

- source origin
- whether the item is raw, synthesized, or inferred
- any known limitations or assumptions
- how it relates to existing knowledge

## Human review requirement

Any proposed change that would alter active UX guidance should be clearly marked as requiring human review before approval.

## Important rule

Processing a file is not the same as approving it. The repository should explicitly track that distinction.
