# Phase 06 Prompts

## Implement From Plan

```txt
Implement the feature described in @<PLAN_PATH>.

Instructions:

- Read the full implementation plan first
- Read the source specs if behavior is unclear
- Inspect the relevant project files before editing
- Follow existing project patterns
- Keep edits scoped to the plan
- Do not introduce unrelated refactors
- Preserve all reviewed behavior and constraints
- Add or update tests according to the testing plan
- Run relevant checks

When finished, report:

- What changed
- What tests or checks were run
- Any checks that could not run
- Any deviations from the plan
- Any remaining risks or follow-ups
```

## Continue Implementation After Feedback

```txt
Continue implementing @<PLAN_PATH>.

Also account for this feedback:

<PASTE_FEEDBACK_HERE>

Instructions:

- Inspect the current worktree before editing
- Preserve existing user changes
- Keep edits scoped to the implementation plan and feedback
- Do not reopen product scope
- Run relevant checks after changes

When finished, report what changed and what was verified.
```

## Fix Failed Verification

```txt
The implementation for @<PLAN_PATH> has failing verification.

Failure details:

<PASTE_FAILURE_OUTPUT_HERE>

Debug and fix the issue.

Instructions:

- Inspect the failing test or check first
- Identify whether the failure is caused by the implementation, the test, or the environment
- Fix only what is needed for the planned behavior
- Do not add unrelated refactors
- Re-run the relevant verification

When finished, report:

- Root cause
- Fix
- Verification result
- Any remaining blocker
```

## Final Implementation Review

```txt
Review the completed implementation against @<PLAN_PATH>.

Check:

- Planned work was completed
- Reviewed behavior was preserved
- Tests match the testing plan
- Compatibility notes were handled
- No unrelated scope was introduced
- Any deviations are documented

Return findings first, ordered by severity.
If there are no issues, say that clearly and mention remaining test gaps or residual risk.
```
