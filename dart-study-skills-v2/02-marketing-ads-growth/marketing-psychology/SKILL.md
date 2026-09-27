---
name: marketing-psychology
description: Apply behavioral science responsibly to marketing decisions.
---

# marketing-psychology

## Purpose
Apply behavioral science responsibly to marketing decisions.

## Use When
- The request directly involves: social proof, loss aversion, cognitive load, defaults, trust, ethical persuasion.
- A change could affect revenue, customer experience, security, operations, or brand consistency.
- The task needs a repeatable workflow instead of an ad-hoc answer.

## Dart Context
Dart is a youth-focused menswear e-commerce brand. Treat the storefront, admin dashboard, database, APIs, customer communications, logistics, analytics, finance rules, and brand system as one connected product. Preserve existing business rules unless the user explicitly changes them.

## Workflow
1. Restate the concrete goal and identify the affected Dart domains.
2. Inspect current evidence, code, data, analytics, or assets before assuming behavior.
3. Define the smallest safe change and its acceptance criteria.
4. Check dependencies: data model, API contract, permissions, UI state, analytics, notifications, and financial impact where relevant.
5. Implement or propose the change with backwards compatibility in mind.
6. Validate happy paths, edge cases, failure paths, mobile behavior, and security implications.
7. Report what changed, what was verified, and any remaining uncertainty.

## Focus Areas
- social proof
- loss aversion
- cognitive load
- defaults
- trust
- ethical persuasion

## Guardrails
- Never invent live metrics, customer facts, product attributes, prices, margins, or campaign results.
- Do not silently override Dart discount, inventory, order, return, or permission rules.
- Server-side authorization and database constraints are the source of truth for sensitive operations.
- Prefer simple, observable, reversible changes over hidden complexity.
- Keep mobile performance and low-friction customer experience as first-class requirements.
- When money is involved, show the formula and preserve historical transaction values.

## Output Checklist
- Goal and scope are explicit.
- Dependencies and affected domains are listed.
- Acceptance criteria are testable.
- Security/privacy implications were checked where relevant.
- Analytics/measurement is defined when the change affects customer behavior or marketing.
- Rollback or recovery path exists for production-impacting changes.

## Origin
Adapted for Dart from concepts in `coreyhaines31/marketingskills`; this file is a Dart-focused implementation, not a byte-for-byte copy.
