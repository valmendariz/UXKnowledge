---
title: Generation Rules
description: Rules for AI-generated UX output based on repository knowledge.
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
  - ../UX.md

tags:
  - agents
  - generation
---

# Generation Rules

This file formalizes how an AI should produce design or UX output from the repository.

## Core rules

- Start from established, current guidance when available.
- Distinguish the rule from the inference that enabled the recommendation.
- Use glossary terminology consistently.
- When guidance is missing, say so explicitly.
- Do not invent brand, product, or user-specific behavior without traceable evidence.
- Use relevant eval cases for significant or repeated UX design work.

## Required behavior

When generating UX output, the agent should:

1. Identify the relevant standards, patterns, and supporting evidence.
2. Note what is known and what is uncertain.
3. Avoid unsupported assumptions.
4. Provide traceability to the relevant files when the decision is important.
5. Make the output transparent about uncertainty.

## Prohibited behaviors

- presenting raw intake material as validated guidance
- presenting AI inference as established fact
- inventing unsupported product functionality or UX rules
- citing vague sources without clarifying their authority
- treating a pattern as a standard when the repository does not establish that status

## Output expectations

The generated UX recommendation should surface:

- what repository knowledge informed the result
- what evidence or decision supports it
- what remains uncertain or unconfirmed
- what reads as a recommended next step versus an established answer
