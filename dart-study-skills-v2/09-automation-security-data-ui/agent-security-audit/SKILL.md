---
name: agent-security-audit
description: "Audit AI-agent permissions, prompt-injection surfaces, MCP/tool access, secrets, data-exfiltration paths, and excessive agency."
version: 2.0.0
---

# agent-security-audit

## Purpose
Audit AI-agent permissions, prompt-injection surfaces, MCP/tool access, secrets, data-exfiltration paths, and excessive agency.

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

## Agent Security Checks
- Tool permissions and least privilege
- Prompt/tool injection surfaces
- Secrets and connector boundaries
- Data exfiltration paths
- User confirmation for high-impact actions
- Auditability and reversible actions
- MCP server/tool schema abuse cases

## Focus Areas
- agent security
- prompt injection
- MCP
- permissions
- exfiltration

## Output Checklist
- Scope is explicit.
- Assumptions are labeled and unverifiable facts are not invented.
- The user gets an actionable next step or deliverable.
- Edge cases and failure modes relevant to the task were considered.
- The output can be checked against evidence or a clear success criterion.

## Origin
Adapted from concepts in OWASP/secure-agent-playbook. This file is original wording for this pack, not a verbatim copy of upstream content.
- Upstream reference: https://github.com/OWASP/secure-agent-playbook
