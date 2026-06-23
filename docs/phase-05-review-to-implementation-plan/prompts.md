# Phase 05 Prompts

## Specs To Implementation Plan: File

```txt
Create an implementation plan from the reviewed specs.

Source documents:

- Feature Description: @<FD_PATH>
- Outline directory: @<OUTLINE_DIR>
- Specs directory: @<SPECS_DIR>
- Review notes: @<REVIEW_PATH>

Before writing the plan, inspect the relevant project files to understand the current implementation.

Create the implementation plan at @<PLAN_OUTPUT_PATH>.

Use this structure:

- Summary
- Source Documents
- Implementation Goals
- Non-Goals
- Current System Context
- Proposed Approach
- Work Plan
- Interfaces And Data
- Compatibility And Migration Notes
- Testing Plan
- Verification Checklist
- Risks And Open Questions

Rules:

- Do not reopen product scope
- Preserve all reviewed behavior
- Carry forward approved review notes
- Be concrete enough for implementation
- Name likely affected areas after inspecting the repo
- Include tests and verification
- Keep unresolved technical questions explicit

Do not implement the feature.
```

## Specs To Implementation Plan: Inline

```txt
Create an implementation plan from the reviewed spec material below.

Before writing the plan, inspect the relevant project files to understand the current implementation.

Use this structure:

- Summary
- Source Documents
- Implementation Goals
- Non-Goals
- Current System Context
- Proposed Approach
- Work Plan
- Interfaces And Data
- Compatibility And Migration Notes
- Testing Plan
- Verification Checklist
- Risks And Open Questions

Rules:

- Do not reopen product scope
- Preserve all reviewed behavior
- Carry forward approved review notes
- Be concrete enough for implementation
- Name likely affected areas after inspecting the repo
- Include tests and verification
- Keep unresolved technical questions explicit

Do not implement the feature.

Reviewed material:

<PASTE_REVIEWED_SPECS_AND_NOTES_HERE>
```

## Refine An Implementation Plan

```txt
Read the implementation plan at @<PLAN_PATH>.
Read the reviewed specs under @<SPECS_DIR>.

Improve the plan so it is implementation-ready.

Focus on:

- Missing work units
- Work that is out of order
- Missing data or interface changes
- Missing migration or compatibility notes
- Missing tests
- Vague verification steps
- Product decisions that should not be left to implementation

Do not implement the plan.
Return the revised implementation plan.
```

## Plan Quality Review

```txt
Review the implementation plan at @<PLAN_PATH>.

Check whether an engineer or AI agent could implement it without making product decisions.

Report:

- Missing implementation context
- Missing sequencing
- Missing interface or data contract notes
- Missing compatibility or migration risks
- Missing tests
- Open questions that block implementation
- Any plan item that conflicts with the reviewed specs

Do not rewrite unless asked.
```
