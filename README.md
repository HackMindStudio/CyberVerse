# CyberVerse


![Project Status: In Progress](https://img.shields.io/badge/Project%20Status-In%20Progress-orange)

> **Development status: Work in Progress (WIP).** CyberVerse is actively being developed and is not yet complete or production-ready.


> **Learn → Practice → Build → Create → Deploy → Grow**

CyberVerse is an AI-powered technology learning platform and developer ecosystem. Its intended learning scope spans programming, computer science, cybersecurity, networking, Linux, web development, and mobile development, from beginner to advanced levels.

## Vision

CyberVerse aims to bring technology learning and building workflows into one ecosystem. Learners should be able to study concepts, practise skills, build projects, receive AI guidance, track progress, and grow a portfolio.

The long-term vision includes learning, research, development, collaboration, portfolio building, certifications, career opportunities, and technology business capabilities. These are product goals, not claims that every capability is currently implemented.

## Learning experience

The intended learning experience combines:

- Structured lessons and learning paths
- Quizzes, practical exercises, and projects
- AI-assisted doubt solving and learning guidance
- Progress tracking and personalized recommendations
- Gamified progression through XP, levels, achievements, and streaks

The AI experience is intended to support four roles: **Teacher, Mentor, Coach, and Reviewer**.

## Current project scope

The current review scope is limited to the following existing phases:

| Phase | Area |
|---|---|
| 1 | Foundation & Identity System |
| 2 | Home Dashboard |
| 3 | AI Mentor Core |
| 4 | Programming Academy |
| 5 | Computer Science Academy |
| 6 | Linux Academy |
| 7 | Networking Academy |
| 8 | Web Development Academy |
| 8.5 | Backend & Progression Integrity |
| 9 | Real AI Provider Layer |
| 9.1 | AI Production Verification |
| 10 | Mobile Development Academy |

**Phase 11 is explicitly out of scope** until the Phase 1–10 audit and verified recovery work are complete.

## Development status

**CyberVerse is a work in progress (WIP).** The application is still under active development and must not be described as complete or production-ready. Features and phase completion must be assessed from the actual source and runtime evidence.

The related BodyForge application is also a separate work-in-progress project; it is not part of this CyberVerse repository or its Phase 1–10 audit scope.

## Audit status

This repository is currently being prepared to host the CyberVerse source and its audit records. At the time of the initial repository inspection, it contained only the starter README. The application source code, dependency manifests, database migrations, and test suite were not present.

Therefore:
- No phase is currently marked as verified complete by this repository.
- No implementation, runtime behavior, security control, or database policy is claimed to have been tested.
- Phase completion percentages will be assigned only after inspecting the actual code and running relevant checks.

See [the master audit plan](docs/audit/MASTER_AUDIT_PLAN.md), [phase audit matrix](docs/audit/PHASE_AUDIT_MATRIX.md), and [recovery tracker](docs/audit/RECOVERY_TRACKER.md).

## Technology stack

The implementation stack has **not yet been confirmed from source files**. Frameworks, providers, database versions, deployment targets, and setup commands will be documented after the project source is added and inspected.

Do not add secrets, API keys, service-role credentials, private tokens, or production environment files to Git.

## Repository structure

Current repository documentation structure:

```text
.
├── .github/
│   ├── ISSUE_TEMPLATE/
│   └── PULL_REQUEST_TEMPLATE.md
├── .gitignore
├── CONTRIBUTING.md
├── README.md
├── SECURITY.md
└── docs/
    └── audit/
        ├── MASTER_AUDIT_PLAN.md
        ├── PHASE_AUDIT_MATRIX.md
        ├── PHASE_REPORT_TEMPLATE.md
        └── RECOVERY_TRACKER.md
```

This describes documentation and repository support files only; it does not describe the not-yet-imported application architecture.

## Contributing and security

Read [CONTRIBUTING.md](CONTRIBUTING.md) before proposing changes. For security concerns, follow [SECURITY.md](SECURITY.md).

## Project principles

1. Inspect before changing.
2. Preserve existing working functionality and user data.
3. Never reset the database as an audit shortcut.
4. Never overwrite an existing migration.
5. Add a new migration only when evidence shows it is required.
6. Keep changes small, reviewable, and backward-compatible.
7. Distinguish implemented, tested, partially verified, mocked, and unverified behavior.
8. Do not start Phase 11 during the current audit and recovery scope.

---

**CyberVerse** — an AI-powered technology learning and developer ecosystem.
