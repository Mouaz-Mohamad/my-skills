---
name: mcp-builder
description: "Design MCP servers and tools with narrow schemas, permission boundaries, observable errors, and safe action semantics."
version: 2.0.0
---

# mcp-builder

## Purpose
Design MCP servers and tools with narrow schemas, permission boundaries, observable errors, and safe action semantics.

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

## MCP Design Rules
- One tool = one clear action or read contract.
- Use narrow schemas with explicit required fields and bounded enums.
- Separate read tools from write tools and make high-impact writes confirmable.
- Return structured, inspectable errors instead of swallowing failures.
- Never place secrets inside tool arguments or logs if a credential store exists.

## Focus Areas
- MCP
- tool schemas
- permissions
- errors
- integration

## Output Checklist
- Scope is explicit.
- Assumptions are labeled and unverifiable facts are not invented.
- The user gets an actionable next step or deliverable.
- Edge cases and failure modes relevant to the task were considered.
- The output can be checked against evidence or a clear success criterion.

## Origin
Adapted from concepts in Developer skills ecosystem / adapted. This file is original wording for this pack, not a verbatim copy of upstream content.
