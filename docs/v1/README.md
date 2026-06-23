# AISDDOT2000 Guide v1

This is a practical workflow for turning a vague idea into implemented software with AI agents.

The point is not to create paperwork. The point is to stop asking an agent to implement something before the problem, behavior, scope and plan are clear.

## The Flow

```txt
Idea
  -> Phase 01: Feature Description
  -> Phase 02: Outline
  -> Phase 03: Specs
  -> Phase 04: Review
  -> Phase 05: Implementation Plan
  -> Phase 06: Implementation
```

Each phase produces the input for the next phase.

If a phase feels hard, that usually means an earlier artifact is weak. Go back and fix it instead of forcing the next step.

## Recommended Artifact Shape

You can store the work anywhere, but this shape works well:

```txt
features/<feature-slug>/
  01-fd.md
  outline/
    <feature-area>.md
  specs/
    <feature-area>.spec.md
  reviews/
    spec-review.md
  implementation-plan.md
  implementation-notes.md
```

Keep artifacts small. One giant spec usually means the feature has not been split correctly.

## Phase Index

- [Phase 01: Idea to Feature Description](phase-01-idea-to-fd/README.md)
- [Phase 02: Feature Description to Outline](phase-02-fd-to-outline/README.md)
- [Phase 03: Outline to Specs](phase-03-outline-to-specs/README.md)
- [Phase 04: Spec Review](phase-04-spec-review/README.md)
- [Phase 05: Review to Implementation Plan](phase-05-review-to-implementation-plan/README.md)
- [Phase 06: Plan to Implementation](phase-06-plan-to-implementation/README.md)

## Artifact Definitions

**Feature Description (FD)**

The FD explains the problem, why it matters, desired outcome, current behavior, constraints and assumptions. It should describe what should become true, not how to build it.

**Outline**

The outline splits one FD into a small set of independently specifiable feature areas. It splits by responsibility, not technical layer.

**Spec**

A spec describes expected behavior for one outlined feature area. It should be clear enough that reviewers can find missing rules, edge cases and scope problems before implementation planning starts.

**Review**

The review is a quality gate for specs. It is not a code review. It checks whether the specs are complete, consistent and safe to plan from.

**Implementation Plan**

The implementation plan translates reviewed specs into concrete work. It names affected areas, sequencing, compatibility risks, tests and verification steps.

**Implementation**

Implementation executes the plan in the actual project. The agent should inspect the real codebase first, make scoped changes, run checks and report what changed.

## Basic Rule

Do not let an agent skip phases unless the artifact already exists.

Skipping from idea to implementation is how vague product intent becomes random code.
