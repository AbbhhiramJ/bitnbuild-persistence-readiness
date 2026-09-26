# Post-Compromise Persistence Readiness Checker

A defensive readiness and verification workspace for reviewing common account-level persistence paths after a suspected compromise.

## MVP
- Guided checklist for sessions, recovery methods, app grants, mailbox rules, roles/devices, and post-action sign-in
- Evidence notes and explicit verification state
- Search/filter and review workflow
- Downloadable closure report

## Live demo
https://bitnbuild-persistence-readiness.vercel.app

## Demo walkthrough
1. Review the seeded readiness checks and filter/search.
2. Open the evidence register.
3. Add a short evidence note and mark an item verified when appropriate for the demo.
4. Generate the closure report and review unresolved items.

## Scope and limitations
The demo uses synthetic records and browser-local state. It does not inspect or modify real accounts, remove persistence mechanisms, or attest that an account is clean. Closure status is a demo summary for human review, not a security certification.

## Local run
Open `index.html` in a modern browser. No backend is required.

See [project brief](docs/PROJECT_BRIEF.md).
