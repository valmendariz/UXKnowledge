---
title: Agent Instructions
description: Required operating instructions for AI agents using the repository.
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
  - ./intake-processing.md
  - ./generation-rules.md
  - ../UX.md

tags:
  - agents
  - instructions
---

# AI Agent Instructions

AI working with this repository must follow a conservative and traceable process.

## Required workflow

1. Start with [../UX.md](../UX.md).
2. Determine which UX knowledge is relevant to the task.
3. Retrieve the appropriate detailed files.
4. Prefer validated and current guidance.
5. Check provenance when a decision depends on evidence.
6. Distinguish established knowledge from inference.
7. Never treat [../intake/README.md](../intake/README.md) as authoritative.
8. Identify contradictions instead of silently selecting one side.
9. Avoid inventing product behavior or unsupported assumptions.
10. Use glossary terminology consistently.
11. Cite or reference relevant repository files when explaining consequential UX decisions.
12. Flag missing knowledge.
13. Recommend additions when repeated knowledge gaps appear.
14. Respect deprecated guidance.
15. Consider relevant eval cases before finalizing significant UX generation.

## Questions the repository is designed to help answer

- What do we know?
- What evidence supports it?
- What UX rules apply?
- What do we not know?
- What am I inferring?
- What should I read before making this design decision?

## Operational expectations

- Do not present AI-generated inference as established knowledge.
- Do not silently convert raw evidence into active policy.
- Do not fill gaps with invented product details.
- If the repository lacks the needed knowledge, say so and recommend a concrete next step.
- Keep answers linked to the specific files and evidence that matter.
