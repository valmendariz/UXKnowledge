---
title: Agent Operating Guide
description: High-level instructions for AI agents operating in the UX knowledge repository.
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
  - ../UX.md
  - ./instructions.md
  - ./intake-processing.md
  - ./generation-rules.md

tags:
  - agents
  - ai-operating-guide
---

# Agent Operating Guide

This folder defines how AI agents should behave when working inside the repository.

## Purpose

The repository is not meant to be a passive knowledge dump. It is a governed system that supports retrieval, reasoning, evaluation, and review while keeping provenance and uncertainty visible.

## Entry point

AI agents should begin with [../UX.md](../UX.md), then move to the relevant detail files needed for the task.

## Core principles

- Prefer the relevant detailed files over top-level summaries.
- Distinguish evidence from synthesis and inference.
- Treat intake as non-authoritative.
- Respect the knowledge hierarchy.
- Ask for human input when a decision is consequential but under-specified.

## Related operational files

- [instructions.md](./instructions.md)
- [intake-processing.md](./intake-processing.md)
- [generation-rules.md](./generation-rules.md)
