---
name: supabase-postgres-best-practices
description: "Review PostgreSQL/Supabase schema and queries for correctness, performance, indexing, RLS, concurrency, and maintainability."
version: 2.0.0
---

# supabase-postgres-best-practices

## Purpose
Review PostgreSQL/Supabase schema and queries for correctness, performance, indexing, RLS, concurrency, and maintainability.

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

## Database Checks
- Query plans and indexes
- RLS correctness and cost
- Constraints and data integrity
- Connection behavior
- Pagination strategy
- Concurrency and idempotency
- Migration safety

## Focus Areas
- Postgres
- Supabase
- indexes
- RLS
- query performance

## Output Checklist
- Scope is explicit.
- Assumptions are labeled and unverifiable facts are not invented.
- The user gets an actionable next step or deliverable.
- Edge cases and failure modes relevant to the task were considered.
- The output can be checked against evidence or a clear success criterion.

## Origin
Adapted from concepts in Supabase agent skills / JetBrains mirror reference. This file is original wording for this pack, not a verbatim copy of upstream content.
- Upstream reference: https://github.com/supabase/agent-skills
