# Contributing to CyberVerse

Thank you for contributing to CyberVerse. The current engineering priority is to inspect and verify the existing Phase 1–10 implementation before making changes.

## Before changing code

1. Read the [Master Audit Plan](docs/audit/MASTER_AUDIT_PLAN.md).
2. Inspect the relevant implementation, tests, database objects, and call sites.
3. Confirm whether the requested behavior already exists.
4. Record the evidence and the smallest safe change that addresses the issue.
5. Check for compatibility with existing users and persisted data.

## Non-negotiable project rules

- Do not rebuild working modules.
- Do not remove existing working functionality.
- Do not reset or wipe any database or user data.
- Do not overwrite, rename, or edit an already-applied migration.
- Create a new migration only when the need is demonstrated and the migration is safe to roll forward.
- Do not introduce unrelated features.
- Do not begin Phase 11 while Phase 1–10 audit and recovery are open.
- Never commit secrets, API keys, tokens, private keys, or production environment files.
- Do not describe mock, stub, or demo behavior as production functionality.

## Execution and approval boundaries

Work should proceed independently when the task is clearly within the agreed Phase 1–10 audit scope and is safe, reversible, and evidence-based. Do not interrupt the owner for routine documentation, repository organization, read-only inspection, test execution, or small isolated fixes that preserve existing behavior.

Ask the owner for approval before:
- Destructive or irreversible operations.
- Any database reset, deletion, destructive migration, or action that could alter production/user data.
- Changing production credentials, secrets, authentication settings, billing, deployment, or access permissions.
- Making a repository public/private or otherwise changing who can access project code.
- Removing or replacing existing functionality when the impact is not fully established.
- Expanding scope beyond the agreed Phase 1–10 audit and recovery.

When approval is needed, explain the exact action, why it is needed, the expected impact, and the safe alternative. Do not ask repeatedly for approval for work already authorized.

## Safe change workflow

1. Identify the affected phase and user journey.
2. Capture the current behavior and relevant baseline.
3. Implement one focused change at a time.
4. Add or update tests for the affected behavior.
5. Run the narrowest relevant tests first.
6. Run TypeScript, lint, production build, and broader tests when the project toolchain is available.
7. Review the final diff for unrelated changes, data-loss risks, and secret exposure.
8. Report exactly what was changed and what remains unverified.

## Pull request expectations

A pull request should include:

- Problem statement and evidence
- Affected phase(s)
- Root cause
- Files changed
- Database/migration impact (or explicitly state none)
- Tests and commands run, with actual results
- Security and backward-compatibility considerations
- Manual verification still required

Avoid claims such as "fixed" or "verified" unless the relevant behavior was actually tested.

## Unknown project setup

The application source and its stack-specific commands must be inspected before prescribing package installation, formatting, test, or build commands. Do not assume a framework or package manager.
