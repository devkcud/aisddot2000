# Implementation Checklist

## Before Editing

- [ ] Read the implementation plan.
- [ ] Read the source specs if behavior is unclear.
- [ ] Inspect the relevant project files.
- [ ] Identify existing patterns to reuse.
- [ ] Check current worktree state if the project uses git.

## During Implementation

- [ ] Keep edits scoped to the plan.
- [ ] Preserve reviewed behavior.
- [ ] Avoid unrelated refactors.
- [ ] Update interfaces, data, UI or docs consistently.
- [ ] Add or update tests based on the plan.
- [ ] Keep compatibility requirements in mind.

## Verification

- [ ] Run relevant unit tests.
- [ ] Run relevant integration or end-to-end tests if available.
- [ ] Run lint, typecheck or build checks if they are part of the project.
- [ ] Manually verify key acceptance criteria if automated coverage is not available.
- [ ] Document any check that could not run and why.

## Final Notes

- [ ] Summarize implemented changes.
- [ ] List verification performed.
- [ ] List known gaps or follow-up work.
- [ ] Mention any intentional deviation from the implementation plan.
