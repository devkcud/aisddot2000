This project uses an AI-assisted Specification Driven Development flow:

```txt
Idea -> FD -> Outline -> Specs -> Review -> Implementation Plan -> Implementation
```

Do not skip a phase unless the required artifact already exists.

## Artifacts

`N-fd.md` - Where N is a number.

The Feature Description, or FD, explains the problem and desired outcome. It should describe what should become true, not how to build it.

`outline/`

Outline files split the FD into independently specifiable feature areas. Split by responsibility, not by technical layer.

Good: `Rule Management`, `Association Generation`, `Manual Overrides`.

Bad: `Frontend`, `Backend`, `Database`.

`specs/`

Specs describe expected behavior for each outlined feature area: actors, rules, flows, states, edge cases, visibility and acceptance criteria.

Specs are not implementation plans.

`implementation-plan.md`

The implementation plan translates reviewed specs into concrete work: affected areas, sequencing, data/interface changes, compatibility risks, tests and verification.

`implementation-notes.md`

Implementation notes record what changed, what was verified, what could not be verified and any remaining follow-up. This is optional as long everything is well defined.

## Working Rules

- Read the previous phase artifact before creating or changing the next one.
- Keep each artifact focused on its phase.
- Do not put implementation details in the FD, outline or specs unless they are hard constraints.
- Before implementation, read `implementation-plan.md`, relevant specs and the actual code.
- During implementation, stay inside the plan, preserve reviewed behavior, follow existing code patterns and avoid unrelated refactors.
- If implementation reveals a product behavior problem, update the spec or review notes before changing behavior. Always notify user.
- All artifacts, excluding FD, should be placed under a new directory called `.<fd-number>-<feature>/`
