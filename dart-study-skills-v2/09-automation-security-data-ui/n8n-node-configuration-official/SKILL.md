---
name: n8n-node-configuration-official
description: "Configure n8n nodes operation-by-operation without guessing hidden parameters or dependencies."
version: 2.0.0
---

# n8n-node-configuration-official

## Purpose
Configure n8n nodes operation-by-operation without guessing hidden parameters or dependencies.

## Use When
- Building, reviewing, debugging, or securing an n8n workflow.
- A node, expression, credential, Data Table, agent, or workflow lifecycle decision is involved.

## n8n Operating Rules
- Treat current n8n node operations and parameter dependencies as version-sensitive; inspect the live node/tool schema when available.
- Do not guess credentials, hidden node fields, or expression context.
- Identify side effects before testing; a “test” can still send messages, write to databases, or call external APIs.
- Prefer reusable stateless sub-workflows for repeated multi-step logic.
- Validate data shape at each boundary and add an explicit error path for production workflows.

## Workflow
1. Define trigger, inputs, outputs, side effects, and failure behavior.
2. Reuse an existing workflow/sub-workflow where appropriate.
3. Configure one node at a time with known operation parameters.
4. Validate expressions against realistic sample data.
5. Add credential/security boundaries and error handling.
6. Test safely, inspect execution evidence, then publish or hand off.

## Focus Areas
- n8n nodes
- operations
- parameters
- validation
- configuration

## Output Checklist
- Scope is explicit.
- Assumptions are labeled and unverifiable facts are not invented.
- The user gets an actionable next step or deliverable.
- Edge cases and failure modes relevant to the task were considered.
- The output can be checked against evidence or a clear success criterion.

## Origin
Adapted from concepts in n8n-io/skills. This file is original wording for this pack, not a verbatim copy of upstream content.
- Upstream reference: https://github.com/n8n-io/skills
