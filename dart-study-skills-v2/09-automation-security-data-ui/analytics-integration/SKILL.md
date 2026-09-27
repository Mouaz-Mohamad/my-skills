---
name: analytics-integration
description: "Design reliable e-commerce analytics across GA4, Meta Pixel/CAPI, GTM, and server-side order events with deduplication."
version: 2.0.0
---

# analytics-integration

## Purpose
Design reliable e-commerce analytics across GA4, Meta Pixel/CAPI, GTM, and server-side order events with deduplication.

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

## E-commerce Event Contract
- `view_item` / product view
- `add_to_cart`
- `begin_checkout`
- `purchase` only after order acceptance rule chosen by the business
- Returns/refunds as separate lifecycle events
- Stable order/item IDs for deduplication
- Server/client dedupe keys where both paths fire

## Focus Areas
- GA4
- Meta Pixel
- Conversions API
- GTM
- ecommerce events

## Output Checklist
- Scope is explicit.
- Assumptions are labeled and unverifiable facts are not invented.
- The user gets an actionable next step or deliverable.
- Edge cases and failure modes relevant to the task were considered.
- The output can be checked against evidence or a clear success criterion.

## Origin
Adapted from concepts in finsilabs/awesome-ecommerce-skills. This file is original wording for this pack, not a verbatim copy of upstream content.
- Upstream reference: https://github.com/finsilabs/awesome-ecommerce-skills
