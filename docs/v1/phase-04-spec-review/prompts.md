# Phase 04 Prompts

## Review Specs: File

```txt
Review the specs under @<SPECS_DIR>.

Use these source documents:

- Feature Description: @<FD_PATH>
- Outline directory: @<OUTLINE_DIR>

Do not rewrite the specs yet.

Review for:

- Alignment with the FD
- Alignment with outline boundaries
- Ambiguous behavior
- Missing rules
- Missing states and edge cases
- Contradictions between specs
- Untestable acceptance criteria
- Scope creep
- Open questions that block implementation planning

For each finding, include:

- Severity: Blocker, Major or Minor
- Location
- Problem
- Required change

End with one result:

- Approved
- Approved With Notes
- Needs Revision
```

## Review One Spec: File

```txt
Review the spec at @<SPEC_PATH>.

Use these source documents:

- Feature Description: @<FD_PATH>
- Outline item: @<OUTLINE_PATH>

Do not rewrite the spec yet.

Report:

- Behavior gaps
- Scope boundary problems
- Missing edge cases
- Missing or weak acceptance criteria
- Contradictions with the source documents
- Questions that block implementation planning

End with one result:

- Approved
- Approved With Notes
- Needs Revision
```

## Apply Review Notes

```txt
Read the spec at @<SPEC_PATH>.
Read the review notes at @<REVIEW_PATH>.

Update the spec to address all required changes.

Rules:

- Preserve the original FD intent
- Do not add new scope beyond the review notes
- Keep behavior separate from implementation details
- Keep unresolved questions explicit if they cannot be answered from the source documents

Return the revised spec and a short list of what changed.
```

## Final Approval Check

```txt
Read the reviewed specs under @<SPECS_DIR>.
Read the review notes at @<REVIEW_PATH>.

Check whether all required changes were addressed.

Return:

- Remaining blockers
- Remaining major issues
- Notes that should be carried into Phase 05
- Final review result: Approved, Approved With Notes or Needs Revision
```
