# Phase 03 Prompts

## Outline To Spec: File

```txt
Read the Feature Description at @<FD_PATH>.
Read the outline file at @<OUTLINE_PATH>.

Create a behavior specification at @<SPEC_OUTPUT_PATH>.

Use this structure:

- Summary
- Goals
- Non-Goals
- Actors
- Current Behavior
- Expected Behavior
- User Flows
- Rules
- States And Edge Cases
- Visibility And Feedback
- Acceptance Criteria
- Open Questions

Rules:

- Specify behavior, not implementation
- Stay inside the outline item's responsibility
- Use the FD as context but do not expand scope
- Include permissions, empty states, invalid states and failure behavior when relevant
- Add acceptance criteria in Given/When/Then style
- Keep open questions explicit instead of guessing

Do not create an implementation plan.
Do not write code.
```

## Outline To Spec: Inline

```txt
Create a behavior specification from the Feature Description and outline below.

Use this structure:

- Summary
- Goals
- Non-Goals
- Actors
- Current Behavior
- Expected Behavior
- User Flows
- Rules
- States And Edge Cases
- Visibility And Feedback
- Acceptance Criteria
- Open Questions

Rules:

- Specify behavior, not implementation
- Stay inside the outline item's responsibility
- Use the FD as context but do not expand scope
- Include permissions, empty states, invalid states and failure behavior when relevant
- Add acceptance criteria in Given/When/Then style
- Keep open questions explicit instead of guessing

Feature Description:

<PASTE_FD_HERE>

Outline:

<PASTE_OUTLINE_HERE>
```

## Refine A Spec

```txt
Read the spec at @<SPEC_PATH>.
Read the source outline at @<OUTLINE_PATH>.
Read the Feature Description at @<FD_PATH>.

Improve the spec without expanding scope.

Focus on:

- Ambiguous behavior
- Missing rules
- Missing states and edge cases
- Weak acceptance criteria
- Behavior that belongs to another outline item
- Implementation details that should be removed

Return the revised spec.
```

## Spec Completeness Check

```txt
Review the spec at @<SPEC_PATH>.

Do not rewrite it.

Report:

- Ambiguous behavior
- Missing user flows
- Missing rules
- Missing edge cases
- Missing acceptance criteria
- Open questions that block implementation planning
- Scope that appears to exceed the outline

Keep findings actionable.
```
