# Operational Duties & Segregation of Responsibilities

## Roles & Separation of Concerns

No single agent may hold conflicting roles in any execution lifecycle:

- An agent assigned the maker role cannot perform verification or auditing
- An agent assigned the checker role cannot perform plan generation or execution
- An agent assigned the executor role cannot perform compliance auditing
- An agent assigned the auditor role cannot perform action execution

## Handoff Workflows

1. The maker agent generates the initial diagnostic assessment and candidate remediation strategy.
2. The checker agent audits evidence quality, checks policy constraints, and validates invariants.
3. The auditor agent signs the cryptographic trace and verifies that no sensitive data is leaked.
4. The executor agent delivers the approved intervention to the target runtime environment.

## Isolation Policy

- **State isolation:** full
- **Credential segregation:** separate

## Enforcement

strict
