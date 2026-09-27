---
name: azhar-exam-generator
description: "Generate realistic Azhar-style practice exams from supplied syllabus material while keeping an explicit answer key and marking logic."
version: 2.0.0
---

# azhar-exam-generator

## Purpose
Generate realistic Azhar-style practice exams from supplied syllabus material while keeping an explicit answer key and marking logic.

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

## Exam Construction
1. Build a coverage map before writing questions.
2. Mix recall, understanding, application, and multi-step questions in proportions supported by the supplied source or user instruction.
3. Keep an answer key separate from the student paper.
4. Do not claim the paper matches an official Azhar distribution unless that distribution was provided or verified.
5. After marking, feed errors into `azhar-error-log` and generate a targeted re-test.

## Focus Areas
- exam generation
- coverage
- difficulty
- marking
- source grounding

## Output Checklist
- Scope is explicit.
- Assumptions are labeled and unverifiable facts are not invented.
- The user gets an actionable next step or deliverable.
- Edge cases and failure modes relevant to the task were considered.
- The output can be checked against evidence or a clear success criterion.

## Origin
Custom skill created for Mouaz's Dart & Study workflow.
