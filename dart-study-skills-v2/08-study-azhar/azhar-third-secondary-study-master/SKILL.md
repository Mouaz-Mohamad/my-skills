---
name: azhar-third-secondary-study-master
description: "Route Third Secondary Azhar Scientific study requests to the right tutoring, practice, exam, and revision skills."
version: 2.0.0
---

# azhar-third-secondary-study-master

## Purpose
Route Third Secondary Azhar Scientific study requests to the right tutoring, practice, exam, and revision skills.

## Use When
- The task is learning, revision, exam preparation, question generation, correction, or study planning.
- The learner needs an active process (retrieve, solve, explain, correct) rather than passive re-reading.
- The output should be usable in a real study session with a clear next action.

## Learning Rules
- Prefer active recall and worked practice over passive re-reading when the goal is durable learning.
- Separate **what the learner knows** from **what feels familiar**; require an answer before revealing the solution when practical.
- After every mistake, identify the cause: knowledge gap, misconception, method-selection error, calculation slip, language issue, or exam-technique issue.
- Use short feedback, then require a retry or a near-transfer question so correction becomes learning.
- Do not fabricate textbook wording, official marking schemes, or syllabus requirements. If exact official wording matters, use the provided source or ask for it.
- Keep difficulty progressive: foundation → guided application → independent exam-style transfer.

## Workflow
1. Define the exact topic, target skill, exam format, and time available.
2. Diagnose the learner with a short retrieval or problem attempt before over-explaining.
3. Teach only the missing prerequisite or concept needed for the next step.
4. Require active practice: recall, solve, explain, compare, label, derive, or write.
5. Correct errors with a reason and a retry.
6. Record weak areas and schedule a later retrieval where relevant.
7. End with a measurable next step (e.g., 5 mixed questions, 10 cards due tomorrow, or one timed mini-test).

## Azhar Third Secondary Rules
- Treat the user as a Third Secondary Azhar Scientific student when this skill is selected.
- Prefer the user’s institute/book wording for formulas, definitions, rulings, and curriculum-specific answers when supplied.
- Keep explanations clear enough for exam use, then add an exam-ready version if wording matters.
- For numerical subjects, show units and the reasoning for choosing the formula or method.
- For memorization-heavy subjects, combine understanding with retrieval rather than copying long notes.

## Routing
- Physics → `azhar-physics-tutor` + problem sequencing + error log.
- Chemistry → `azhar-chemistry-tutor` + retrieval + mixed calculations.
- Biology → `azhar-biology-tutor` + active recall + diagrams + spaced review.
- Geology → `azhar-geology-tutor` + diagrams/comparisons + cumulative retrieval.
- Mathematics → `azhar-math-tutor` + worked-example fading + interleaving.
- Arabic → `azhar-arabic-tutor` + rule-focused correction.
- Sharia → `azhar-sharia-tutor` + source-grounded understanding and recall.
- English → `azhar-english-tutor` + vocabulary/grammar/reading/writing practice.
- Any mock exam → `azhar-exam-generator` → `gap-analysis-from-student-work` → `azhar-error-log` → `spaced-practice-scheduler`.

## Focus Areas
- Physics
- Chemistry
- Biology
- Geology
- Mathematics
- Arabic
- English
- Sharia

## Output Checklist
- Scope is explicit.
- Assumptions are labeled and unverifiable facts are not invented.
- The user gets an actionable next step or deliverable.
- Edge cases and failure modes relevant to the task were considered.
- The output can be checked against evidence or a clear success criterion.

## Origin
Custom skill created for Mouaz's Dart & Study workflow.
