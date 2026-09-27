---
name: webapp-ui-skill
description: "Build or audit dense dashboard and admin interfaces with explicit loading, empty, error, selection, focus, and mobile states."
version: 2.0.0
---

# webapp-ui-skill

## Purpose
Build or audit dense dashboard and admin interfaces with explicit loading, empty, error, selection, focus, and mobile states.

## Use When
- The request directly involves the capability described by this skill.
- The task affects Dart code, data, security, analytics, UI, automation, or customer experience.

## Workflow
1. Define scope, source of truth, and measurable acceptance criteria.
2. Inspect current code/data/configuration before proposing changes.
3. Choose the smallest safe change with explicit failure behavior.
4. Implement or specify the change with security, observability, and rollback in mind.
5. Validate normal, empty, error, unauthorized, duplicate, and mobile states where relevant.
6. Report evidence, remaining uncertainty, and next actions.

## State Coverage Matrix
- loading
- empty
- error
- unauthorized
- disabled
- selected
- focus/keyboard
- submitting
- success
- offline/retry where relevant
- mobile/narrow viewport

## Focus Areas
- dashboard
- admin UI
- tables
- filters
- state coverage
- accessibility

## Output Checklist
- Scope is explicit.
- Assumptions are labeled and unverifiable facts are not invented.
- The user gets an actionable next step or deliverable.
- Edge cases and failure modes relevant to the task were considered.
- The output can be checked against evidence or a clear success criterion.

## Origin
Adapted from concepts in sergekostenchuk/ui-ux-agent-skill-system. This file is original wording for this pack, not a verbatim copy of upstream content.
- Upstream reference: https://github.com/sergekostenchuk/ui-ux-agent-skill-system
