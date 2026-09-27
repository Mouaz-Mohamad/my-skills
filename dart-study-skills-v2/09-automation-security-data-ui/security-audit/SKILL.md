---
name: security-audit
description: "Run a defensive, source-first security review focused on real trust boundaries, evidence, severity, and smallest effective fixes."
version: 2.0.0
---

# security-audit

## Purpose
Run a defensive, source-first security review focused on real trust boundaries, evidence, severity, and smallest effective fixes.

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

## Defensive Audit Rules
- Start from trust boundaries and affected principals/resources.
- A suspected issue is not a confirmed finding without source evidence and a bounded impact.
- Prefer safe reproduction and minimal proof over destructive testing.
- Rank remediation by real impact and exploit preconditions, not by dramatic wording.

## Focus Areas
- security review
- trust boundaries
- evidence
- vulnerabilities
- remediation

## Output Checklist
- Scope is explicit.
- Assumptions are labeled and unverifiable facts are not invented.
- The user gets an actionable next step or deliverable.
- Edge cases and failure modes relevant to the task were considered.
- The output can be checked against evidence or a clear success criterion.

## Origin
Adapted from concepts in cloudflare/security-audit-skill. This file is original wording for this pack, not a verbatim copy of upstream content.
- Upstream reference: https://github.com/cloudflare/security-audit-skill
