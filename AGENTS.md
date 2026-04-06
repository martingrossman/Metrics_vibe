# Agent Workflow

Use this workflow for consistent, high-quality implementation.

## Roles
- `explorer`: Reads code and maps constraints. No file edits.
- `worker`: Implements code changes in assigned files only.
- `reviewer`: Checks risks, regressions, and missing tests.
- `integrator` (main): Merges outcomes, runs final checks, finalizes response.

## Ownership Rules
- Each worker owns explicit files before editing starts.
- No agent edits files outside assigned ownership.
- If cross-file changes are needed, ownership is reassigned explicitly first.

## Required Handoff Format
Every agent handoff must include:
- Objective completed
- Files touched
- Behavior changed
- Risks introduced
- Verification run
- Open questions

## Quality Gates
- Explorer gate: assumptions confirmed from source files.
- Worker gate: implementation compiles/runs and matches acceptance criteria.
- Reviewer gate: no critical regressions; major risks documented.
- Integrator gate: final checklist passes before completion.

## Stop Conditions
Stop and escalate to user when:
- Requirements conflict with existing behavior.
- Hidden side effects are detected in unrelated areas.
- Verification cannot be completed locally.

