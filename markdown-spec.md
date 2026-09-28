---
title: Markdown Engineering Standards
description: Repository standards for documentation structure, style, and machine-readable metadata.
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
    reference: repository-docs-standards

related:
  - ./README.md
  - ./UX.md
  - ./governance/README.md

tags:
  - markdown
  - documentation
---

# Markdown Engineering Standards

This document defines the repository's Markdown conventions so that files are readable for humans and retrievable for AI agents.

## General conventions

- Use semantic Markdown headings.
- Include one H1 per file.
- Keep headings predictable and consistent.
- Prefer short sections over very large documents.
- Use descriptive filenames and relative links where appropriate.
- Keep documents focused on a single concern when possible.
- Use accessible tables when they improve comprehension.
- Use fenced code blocks with a language identifier when showing samples or markup.

## Heading hierarchy

Use a clear, stable heading structure:

# Title
## Purpose or overview
## Core rules or guidance
## Evidence or provenance
## Related knowledge
## Review notes or open questions

Do not skip levels arbitrarily. Keep a consistent pattern across the repository so AI retrieval and human browsing remain predictable.

## Frontmatter

Important knowledge files should use YAML frontmatter when the metadata adds value to retrieve, review, or govern the document.

```yaml
---
title: Workflow Error Handling
description: Guidance for communicating and recovering from workflow execution errors.
knowledge_type: standard
status: draft
owner: UX
version: 0.1.0
created: YYYY-MM-DD
last_updated: YYYY-MM-DD
last_reviewed: YYYY-MM-DD
review_by: YYYY-MM-DD

evidence_level: synthesized

sources:
  - type: research
    reference: placeholder

related:
  - ../patterns/example.md

tags:
  - errors
  - workflows
---
```

## Controlled values

### knowledge_type

- research
- standard
- pattern
- terminology
- user-model
- world-model
- reference

### status

- draft
- review
- active
- deprecated
- archived

### evidence_level

- raw
- synthesized
- reviewed
- validated

## When to use frontmatter

Use frontmatter for documents that are intended to become meaningful knowledge artifacts or governance records. README and operational documents may use lighter metadata, but still benefit from a consistent minimal pattern.

## Required vs optional fields

### Recommended for important knowledge files

- title
- description
- knowledge_type
- status
- owner
- version
- created
- last_updated
- last_reviewed
- review_by
- evidence_level
- sources

### Optional or situational

- related
- tags
- additional governance metadata

## Linking standards

- Prefer relative links over absolute links.
- Link to the nearest relevant file instead of repeating the same detail in multiple places.
- Link to UX or governance files when the content is part of the same decision path.
- Keep links stable and human-readable.

## Machine-readability and AI consumption

To improve AI retrieval and repository maintenance:

- use short, explicit headings
- avoid decorative markdown that does not improve comprehension
- keep sections reasonably scoped
- prefer explicit labels such as Summary, Evidence, Risks, and Related Knowledge
- keep metadata names stable across files

## Accessibility

- use descriptive link text
- avoid relying on color alone to communicate status
- use tables that remain readable in plain text
- keep lines readable and avoid unnecessary decorative formatting

## Documentation quality

A document should be easy to review in a Git diff. This repository favors clear structure, stable patterns, and minimal duplication over decorative formatting.
