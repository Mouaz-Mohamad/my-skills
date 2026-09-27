---
name: arabic-rtl-best-practices
description: "Implement Arabic and RTL web interfaces using semantic direction, logical CSS properties, robust mixed-language handling, and mobile testing."
version: 2.0.0
---

# arabic-rtl-best-practices

## Purpose
Implement Arabic and RTL web interfaces using semantic direction, logical CSS properties, robust mixed-language handling, and mobile testing.

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

## RTL Rules
- Use `dir="rtl"` on the relevant document or container boundary.
- Prefer logical CSS properties such as margin-inline and padding-inline.
- Test mixed Arabic/English, numbers, prices, email addresses, and product codes.
- Do not mirror icons whose meaning is not directional.
- Test forms, tables, modals, maps, and charts separately; RTL is more than text alignment.

## Focus Areas
- Arabic
- RTL
- BiDi
- CSS logical properties
- mixed language

## Output Checklist
- Scope is explicit.
- Assumptions are labeled and unverifiable facts are not invented.
- The user gets an actionable next step or deliverable.
- Edge cases and failure modes relevant to the task were considered.
- The output can be checked against evidence or a clear success criterion.

## Origin
Adapted from concepts in Arabic AI skills ecosystem / adapted. This file is original wording for this pack, not a verbatim copy of upstream content.
