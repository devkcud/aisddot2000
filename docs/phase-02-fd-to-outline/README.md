# Phase 02: Feature Description to Outline

The FD says what problem we are solving.

The outline splits that feature into a small set of independently specifiable feature areas.

Do not skip this phase. Skipping it is how one FD turns into a huge spec that mixes unrelated responsibilities.

## Input

One Feature Description from Phase 01.

## Output

Two to five outline files.

Use [template.md](template.md) for each outline file.

## How To Split

Split by responsibility.

Bad:

- Frontend
- Backend
- Database
- Mobile

Good:

- Rule Management
- Association Generation
- Manual Overrides
- Association Visibility

Technical layers belong in the implementation plan, not the outline.

## Done When

The outline is good enough when each item can be specified independently.

Ask:

```txt
Could I write a complete spec for this item without describing the entire system?
```

If the answer is no, the boundary is probably wrong.

## Common Mistakes

- Creating too many outline items
- Splitting by technical layer
- Creating tiny items that cannot stand alone
- Turning outline files into specs
- Losing the original FD intent

If you get more than five outline items, the FD may be too large. Consider splitting the FD first.

## Prompts

Use [prompts.md](prompts.md) to create or refine outline files.
