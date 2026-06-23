# Phase 01: Idea to Feature Description

Most feature ideas are too vague for implementation.

This phase turns an idea into a Feature Description, or FD. The FD is the foundation for every later artifact.

## Input

A rough idea, complaint, opportunity or request.

Examples:

- "We need automatic product-planogram association."
- "Users keep recreating similar surveys."
- "The export flow is painful."

## Output

One markdown file containing a Feature Description.

Use [template.md](template.md).

## What The FD Must Do

The FD must explain:

- What problem exists
- Why the problem matters
- What outcome users or the business need
- What already exists today
- What behavior is expected after the feature exists
- What must not break
- What assumptions are being made

Write behavior, not implementation.

Bad:

```txt
Create a background worker that recalculates associations.
```

Good:

```txt
Associations should be generated automatically based on user-defined rules.
```

## How To Write It

Start with the painful part.

Ask:

- What is repetitive?
- What is confusing?
- What is causing mistakes?
- What are users complaining about?
- What does the product fail to support today?

Then describe the desired outcome without naming technical components unless they are hard constraints.

## Done When

The FD is good enough when a reader can answer:

- What problem are we solving?
- Who or what is affected?
- What should become true?
- What must remain true?
- What is intentionally not decided yet?

If those answers are unclear, keep refining the FD.

## Common Mistakes

- Describing tables, endpoints or workers too early
- Mixing multiple unrelated ideas into one FD
- Forgetting current behavior
- Forgetting constraints
- Writing a feature pitch instead of a problem description

## Prompts

Use [prompts.md](prompts.md) to draft or refine an FD with an AI agent.
