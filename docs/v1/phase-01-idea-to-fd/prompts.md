# Phase 01 Prompts

## Idea To FD: Inline

```txt
Turn the idea below into a Feature Description.

Use this structure:

- Summary
- Problem
- Why It Matters
- Desired Outcome
- Existing Behavior
- Expected Behavior
- Impacted Areas
- Constraints
- Assumptions
- Out Of Scope

Rules:

- Describe the problem before the solution
- Focus on behavior, not implementation
- Do not invent technical architecture
- Keep implementation details only if they are explicit constraints
- Make weak or vague parts visible instead of hiding them
- Use direct, practical language

Idea:

<PASTE_IDEA_HERE>
```

## Idea To FD: File

```txt
Read the rough feature idea at @<IDEA_PATH>.

Create a Feature Description at @<FD_OUTPUT_PATH>.

Use this structure:

- Summary
- Problem
- Why It Matters
- Desired Outcome
- Existing Behavior
- Expected Behavior
- Impacted Areas
- Constraints
- Assumptions
- Out Of Scope

Rules:

- Describe the problem before the solution
- Focus on behavior, not implementation
- Do not invent technical architecture
- Keep implementation details only if they are explicit constraints
- Make weak or vague parts visible instead of hiding them
- Use direct, practical language
```

## Refine A Weak FD

```txt
Read the Feature Description at @<FD_PATH>.

Improve it without changing its intent.

Focus on:

- Making the problem more concrete
- Separating desired outcome from implementation details
- Clarifying existing behavior
- Making constraints explicit
- Identifying assumptions
- Removing vague language

Do not create an outline, spec or implementation plan.
Return only the improved Feature Description.
```

## FD Quality Review

```txt
Review the Feature Description at @<FD_PATH>.

Do not rewrite it yet.

Report:

- Missing context
- Ambiguous desired outcomes
- Hidden implementation assumptions
- Constraints that should be explicit
- Scope that may be too large
- Questions that must be answered before Phase 02

Keep the review short and actionable.
```
