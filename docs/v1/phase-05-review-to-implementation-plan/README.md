# Phase 05: Review to Implementation Plan

This phase turns approved specs into concrete implementation work.

This is where technical planning belongs.

## Input

Reviewed specs and review notes.

## Output

One implementation plan.

Use [template.md](template.md).

## What The Plan Must Do

The implementation plan must tell an engineer or AI agent:

- What to build
- Where to look first
- Which behavior matters most
- What order to work in
- What compatibility risks exist
- What tests to add or update
- What verification proves the work is done

## How Technical To Be

Be concrete enough that implementation can start.

Good:

```txt
Add persisted association source metadata so manual and generated associations can be distinguished.
```

Too vague:

```txt
Update backend.
```

Too early or too rigid:

```txt
Create table ProductPlanogramRuleV2 with exactly these columns.
```

Exact table names, endpoints and components are fine when they are already known or required. Otherwise, tell the implementer where to inspect and what contract must be preserved.

## Done When

The plan is good enough when another engineer or agent can implement it without making product decisions.

Technical decisions are allowed during implementation. Product behavior decisions should already be settled.

## Common Mistakes

- Planning from unapproved specs
- Reopening product scope in the plan
- Forgetting migrations or backwards compatibility
- Forgetting tests
- Treating the plan as a vague TODO list

## Prompts

Use [prompts.md](prompts.md) to create or refine implementation plans.
