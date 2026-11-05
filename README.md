# RMG | Governed Autonomous Systems

A software architecture portfolio project examining how autonomous
software actions can be constrained by explicit authorization,
execution-state controls, and auditable decisions.

## Engineering problem

An autonomous agent may propose an action that changes external
state. A natural-language instruction alone does not establish
whether that action is authorized, current, or safe to execute.

This project explores a separation between proposed actions,
authorization decisions, and execution.

## Architecture concepts

- Explicit authorization before protected actions
- Binding authorization to the reviewed action
- Fail-closed behavior when required controls are unavailable
- Audit records associated with action decisions
- Controlled handling of interrupted or uncertain execution
- Testable rejection of unauthorized action requests

## Demonstration status

A private Python implementation was exercised through a local
automated test suite. The recorded run completed 30 tests
successfully.

This result does not establish production readiness, complete
security coverage, or independent certification.

## Portfolio materials

- `architecture/OVERVIEW.md`: conceptual system architecture
- `evidence/VALIDATION_SUMMARY.md`: observed validation evidence
- `recruiter/PROJECT_BRIEF.md`: engineering project description

## Disclosure boundary

This repository is intended to contain public-facing descriptions
and selected evidence. Proprietary implementation code, internal
control specifications, and private development records are excluded.

## Limitations

The architecture is a demonstration and engineering study.
No claim of exclusive invention, comprehensive prior-art clearance,
formal verification, or production certification is made.