# Architecture Overview

## Objective

Separate an autonomous system's proposed actions from the
authority required to execute those actions.

## Conceptual flow

1. An agent or operator proposes an action.
2. The system identifies the action and its relevant context.
3. A control boundary determines whether authorization is required.
4. The action is reviewed against the applicable authorization.
5. An execution component performs an allowed action.
6. The system records the decision and resulting execution state.

## Control principles

**Authorization binding:** Approval should apply to the action
reviewed, not to an unrelated or subsequently altered request.

**Fail-closed behavior:** Missing authorization or unavailable
required controls should prevent a protected action from proceeding.

**Auditability:** The system should retain evidence of decisions
and execution outcomes sufficient for subsequent examination.

**Execution uncertainty:** Interrupted execution must not
automatically be interpreted as proof of successful completion.

## Scope

This is a conceptual description. It intentionally excludes
private algorithms, implementation details, control thresholds,
internal schemas, and unpublished engineering specifications.

## Evidence boundary

These principles describe the intended control model.
Observed test results are documented separately. A passing
unit test is not proof that every deployment failure mode
has been addressed.