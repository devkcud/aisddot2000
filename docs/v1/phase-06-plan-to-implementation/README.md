# Phase 06: Plan to Implementation

This phase executes the implementation plan in the real project.

Now code can be written.

## Input

An approved implementation plan from Phase 05.

## Output

Implemented changes, tests, verification notes and any follow-up issues.

Use [checklist.md](checklist.md).

## How To Execute

The implementer must read the plan and inspect the actual codebase before editing.

Do not blindly apply the plan. Plans are written before the final code inspection, so the implementer may need to adapt technical details while preserving the approved behavior.

## Implementation Rules

- Stay inside the plan
- Preserve reviewed behavior
- Avoid unrelated refactors
- Prefer existing project patterns
- Add or update tests based on risk
- Document verification results
- Record any behavior question that blocks implementation

## What Can Change During Implementation

Technical details can change if code inspection shows a better local fit.

Examples:

- Reusing an existing service instead of creating a new one
- Adding a field to an existing model instead of creating a new object
- Testing through an existing integration test harness instead of a new test type

Product behavior should not change without returning to the spec.

## Done When

Implementation is done when:

- Planned behavior is implemented
- Tests or checks were run, or blockers are documented
- The final notes explain what changed
- Any incomplete work is explicit

## Common Mistakes

- Treating the plan as permission for unrelated cleanup
- Changing behavior because implementation is easier
- Skipping tests
- Hiding blocked verification
- Failing to mention deviations from the plan

## Prompts

Use [prompts.md](prompts.md) to drive implementation with an AI agent.
