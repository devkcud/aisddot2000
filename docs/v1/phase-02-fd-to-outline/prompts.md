# Phase 02 Prompts

## FD To Outline: File

```txt
Read the Feature Description at @<FD_PATH>.

Split it into a maximum of five independently specifiable feature areas.

Create one markdown file per feature area under @<OUTLINE_DIR>/.

Each file must use this structure:

- Summary
- Responsibility
- Why This Feature Exists
- Relationship With Other Outlined Features
- Boundaries
- Notes For Specification

Rules:

- Split by responsibility, not technical layer
- Avoid frontend/backend/database/mobile splits
- Avoid implementation details
- Preserve the original FD intent
- Keep boundaries clear
- Each outlined feature must be specifiable on its own
- If the FD is too large, say so before creating too many outline files

Do not write specs.
Do not create an implementation plan.
```

## FD To Outline: Inline

```txt
Read the Feature Description below.

Split it into a maximum of five independently specifiable feature areas.

For each feature area, produce markdown using this structure:

- Summary
- Responsibility
- Why This Feature Exists
- Relationship With Other Outlined Features
- Boundaries
- Notes For Specification

Rules:

- Split by responsibility, not technical layer
- Avoid frontend/backend/database/mobile splits
- Avoid implementation details
- Preserve the original FD intent
- Keep boundaries clear
- Each outlined feature must be specifiable on its own
- If the FD is too large, say so before creating too many outline items

Do not write specs.
Do not create an implementation plan.

Feature Description:

<PASTE_FD_HERE>
```

## Refine An Outline

```txt
Review the outline files under @<OUTLINE_DIR>/ against the Feature Description at @<FD_PATH>.

Improve the outline boundaries.

Focus on:

- Responsibilities that overlap
- Missing feature areas
- Items that are too small to specify independently
- Items that are too broad
- Technical-layer splits that should be replaced
- Places where the FD intent was lost

Do not write specs.
Return the revised outline files or a clear list of required changes.
```

## Outline Quality Review

```txt
Review the outline files under @<OUTLINE_DIR>/.

Report:

- Whether each item can be specified independently
- Whether the set has too many or too few items
- Any overlapping responsibilities
- Any missing responsibility from the FD
- Any implementation detail that should be removed

Do not rewrite unless asked.
```
