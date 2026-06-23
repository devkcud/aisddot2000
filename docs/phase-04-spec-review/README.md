# Phase 04: Spec Review

This phase reviews specs before implementation planning.

The goal is to catch unclear behavior, contradictions and scope problems while they are still cheap to fix.

## Input

The FD, outline files and spec files from the previous phases.

## Output

One review document or comment thread containing required changes and approval notes.

Use [checklist.md](checklist.md).

## What To Review

Review behavior first.

Ask:

- Does the spec solve the FD problem?
- Does each spec stay inside its outline boundary?
- Are rules precise enough?
- Are edge cases covered?
- Are permissions and visibility clear?
- Are acceptance criteria testable?
- Are there contradictions between specs?

## Review Outcomes

Use one of these outcomes:

- **Approved**: The spec is ready for implementation planning.
- **Approved With Notes**: The spec is good enough, but the notes must be carried into the implementation plan.
- **Needs Revision**: The spec must be updated before planning.

## Done When

The specs are ready when implementation planning no longer requires product guessing.

Some technical discovery may still happen in Phase 05, but behavior should not be vague anymore.

## Common Mistakes

- Treating review as grammar cleanup
- Reviewing implementation details that do not exist yet
- Approving specs with unresolved behavior questions
- Allowing scope creep because it sounds useful
- Forgetting compatibility constraints from the FD

## Prompts

Use [prompts.md](prompts.md) for review assistance.
