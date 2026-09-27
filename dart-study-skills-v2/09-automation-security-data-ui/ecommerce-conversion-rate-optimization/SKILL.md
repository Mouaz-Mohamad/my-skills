---
name: ecommerce-conversion-rate-optimization
description: "Audit the e-commerce funnel, prioritize conversion blockers, and create a measurable experimentation backlog."
version: 2.0.0
---

# ecommerce-conversion-rate-optimization

## Purpose
Audit the e-commerce funnel, prioritize conversion blockers, and create a measurable experimentation backlog.

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

## CRO Order of Operations
- Verify tracking before interpreting funnel loss.
- Segment by device/source/new-vs-returning before broad conclusions.
- Fix broken or confusing UX before testing cosmetic variants.
- Each experiment needs one primary metric and guardrail metrics (refunds, support contacts, margin, speed).

## Focus Areas
- ecommerce CRO
- funnel
- checkout
- product page
- experiments

## Output Checklist
- Scope is explicit.
- Assumptions are labeled and unverifiable facts are not invented.
- The user gets an actionable next step or deliverable.
- Edge cases and failure modes relevant to the task were considered.
- The output can be checked against evidence or a clear success criterion.

## Origin
Adapted from concepts in finsilabs/awesome-ecommerce-skills. This file is original wording for this pack, not a verbatim copy of upstream content.
- Upstream reference: https://github.com/finsilabs/awesome-ecommerce-skills
