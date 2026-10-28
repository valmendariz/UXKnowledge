---
title: "Task Flow Guidelines"
id: task-flow-guidelines
status: draft
version: 0.1.0
last_updated: 2026-10-28
source_status: source-derived
description: "A lightweight reference for creating clear, consistent, user-friendly task flows."
---

# Task Flow Guidelines

*A lightweight reference for creating clear, consistent, user-friendly task flows.*

## Contents

1. [Principles](#principles)
2. [Plan](#1-plan)
3. [Build](#2-build)
4. [Polish](#3-polish)

## Principles

### Align with user goals and processes

Structure task flows around user goals while aligning with business process flows. Start with a clear purpose statement.

### Enable visibility

Make the task flow's logic transparent and easy to understand at a glance.

### Keep it simple

Design task flows with the minimum number of steps necessary. **Five to twelve steps is ideal.** Every additional step increases complexity.

---

# 1. Plan

**Define the purpose, audience, and structure before writing.**

## 1.1 Start with why: Know your user and outcome

Use this statement from the Jobs-to-be-Done (JTBD) framework to keep the task flow on track:

> As a **[task performer]**, when **[situation]**, I want to **[motivation]**, so I can **[expected outcome]**.

### Examples

- As a **Supply Planner**, when demand signals change, I want to identify items at risk so I can adjust the plan and resolve shortages.
- As a **Supply Planner**, on a monthly cadence, when supply exceptions occur, I want to identify parts at risk so I can expedite, push out, transfer, or find alternate sources.
- As an **Inventory Planner**, when performing inventory planning and optimization activities, I want to configure new safety stock candidate parts, for example, when a new product line has been introduced at one of the site locations, so I can generate safety stock recommendations for those parts.
- As a **Brand Owner Outsourcing Manager**, when excess supply at contract manufacturers may not be consumed by demand, I want to identify where on-hand or firm supply exceeds demand, so I can understand my inventory exposure and reduce carrying costs and obsolescence risk.
- As a **Demand Manager**, when contract manufacturers and factories provide new supply commitments while allocating to priority customers, I want to identify which SKUs require a reassessment of supply allocations, so I can redistribute supply appropriately across fulfillment locations, ensure the aggregate supply plan reflects the latest commitments, and avoid deficits, shortages, or excesses.

**Reference:** Userverse - Persona Hub

## 1.2 Define structure

- Align with business process charts when available, such as Level 1, Level 2, or Level 3 process flows.
- Consult Product Managers if process charts are not available.
- Example: Align the task flow with the Level 3 **Review Demand Plan** process flow for the Life Sciences template.
- Create a flowchart or mind map first. Identify the inputs, steps, and intended outcome to reveal gaps.
- Break complex processes into multiple task flows when they exceed 5-12 steps.
- Determine the appropriate level of detail based on the user's expertise.
- Identify required inputs, prerequisites, and related resources.
- Consider using the typical step analysis from the JTBD framework.

### Typical JTBD step analysis

1. Define
2. Locate
3. Prepare
4. Confirm
5. Execute
6. Monitor
7. Modify
8. Conclude

### Related patterns

- Progressive Disclosure
- Everything Is Not a User Story
- Task Flows Embody the Process

---

# 2. Build

**Create task-flow content with standardized naming, structure, and clarity.**

## 2.1 Name the task flow

Task-flow names must use title case and be action-oriented.

### Naming pattern

```text
[Optional: Top-level process] + [Infinitive verb] + [Object/task] - [Optional: Role specifier]
```

Example:

```text
Inventory Optimization - Aggregate Supply Planning - Finance
```

### Do

- Start with an infinitive verb, such as **Review**, **Analyze**, or **Create**.
- Include the top-level and subprocess name when adjacent processes need context.
- State a clear outcome.
- Include a role specifier when needed, such as **S&OP Process - Finance**.

### Don't

- Use gerunds, such as **Reviewing Short-Term Demand**.
- Use vague titles.
- Repeat the words **Task Flow** in the title.

## 2.2 Craft the introduction

Every task flow should begin with an introduction containing six elements.

### 1. Purpose or problem statement

**Question:** What problem does this task flow solve?

> The goal of aggregate supply planning is to identify and resolve deficits, shortages, and excesses that may affect the ability to meet demand.

### 2. Audience

**Question:** Who should use this task flow? Include the main audience and collaborators.

> This task flow guides supply planners through analyzing supply metrics, resolving issues, and updating the plan.

### 3. Prerequisites

**Question:** What must be done before starting?

- Configuration settings are complete.
- A planning scenario is created and selected.
- Current supply and demand data is available.

### 4. Outcome or output

**Question:** What will the user produce by the end?

> A refined and finalized aggregate supply plan that reflects issue resolutions and validated adjustments.

### 5. Related information

- Provide parent and child process context for process task flows.
- Reference related task flows or resources.

### 6. Revision and compatibility information

Add revision and compatibility information to support users and track versions.

Example:

```text
Revision: 3. Release 8.1.0 and higher.
```

## 2.3 Add typical required steps when applicable

Some task flows require standard system steps to maintain data integrity and make the process complete, auditable, and repeatable.

| If the task flow... | Add this step... | Consequence if skipped |
|---|---|---|
| Modifies data | **Create a Scenario** before any step where data is modified | Changes may be applied to unrelated live data, causing unintended impacts on orders or inventory. |
| Works within a scenario | **Select the Correct Scenario** when opening a resource | Updates may be made in the wrong scenario; reviewers may see inconsistent results and metrics may not align with the plan. |
| Makes updates | **Save Changes** after updates | Data may be lost; users may assume changes were saved, creating rework and audit gaps. |
| Finalizes changes | **Commit Scenario** after reviewing the outcome of a simulation | Downstream teams may not see the changes, creating governance issues. |
| Is a sub-task flow | **Close the Task Flow** as the final step | The user may be unable to proceed to the next step in the parent task flow or process. |

- Add these steps only when the condition applies.
- Place each step where it logically belongs, before or after the relevant actions.
- Document differences between the web and Java clients when their behavior differs.

## 2.4 Detail each step

### 2.4.1 Use action-oriented naming

Use an action-oriented naming convention for step names, similar to task-flow names.

```text
[Optional marker] + [Action verb] + [Resource name OR specific outcome]
```

Example:

```text
(Optional) Cleanse Historical Data
```

- If a step is optional, explicitly mark it, for example: **5. (Optional) Cleanse Historical Data**.
- Use action-oriented titles.
- Use the resource type and name when opening or using that resource is the only task in the step.
- Otherwise, name the specific outcome, especially when the step includes multiple actions.

### 2.4.2 Write clear step content

- Write for a user with no prior knowledge.
- Briefly state **why** the user must complete the task.
- Use short, digestible sentences. Target less than one minute of reading per step.
- Use active, descriptive language.
- Replace unclear pronouns such as *it*, *that*, and *they* with specific nouns.
- Use present tense.
