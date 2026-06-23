# Phase 03: Outline to Specs

This phase turns each outline item into a behavior specification.

A spec should be clear enough that someone can review the behavior before anyone plans implementation.

## Input

One outline file from Phase 02, plus the original FD for context.

## Output

One spec file per outline item.

Use [template.md](template.md).

## What A Spec Is

A spec describes expected behavior.

It answers:

- Who uses this feature area?
- What can they do?
- What rules apply?
- What states exist?
- What edge cases matter?
- What must be visible or explainable?
- What acceptance criteria prove the behavior?

## What A Spec Is Not

A spec is not an implementation plan.

Avoid:

- Database table design
- Endpoint design
- Component structure
- Worker names
- Library choices
- Task sequencing

Include technical detail only when it is required to describe externally visible behavior or a hard constraint.

## Done When

The spec is good enough when a reviewer can find behavior bugs without reading code.

It should be possible to say:

```txt
If the implementation behaves like this spec, the feature area is correct.
```

## Common Mistakes

- Hiding hard decisions in vague language
- Mixing multiple outline items into one spec
- Writing implementation tasks
- Forgetting permissions, empty states or failure states
- Missing acceptance criteria

## Prompts

Use [prompts.md](prompts.md) to create or refine specs.
