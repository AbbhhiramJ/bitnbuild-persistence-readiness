# Project brief — Post-Compromise Persistence Readiness Checker

## User and problem
**Primary user:** a solo IT administrator or incident responder who needs to verify that account recovery and containment are complete after an identity compromise.

Community incident reports describe response efforts that reset passwords and revoke sessions but later discover mailbox rules, OAuth grants, unknown authentication methods, or device registrations. These are anecdotal reports, not statistical estimates.

## Product promise
Help responders systematically review persistence-relevant account artifacts, record evidence, assign follow-up actions, and verify completion rather than closing an incident after one containment step.

## MVP workflow
1. Choose a seeded compromise scenario.
2. Review checks grouped by identity/session, recovery/MFA, app consent, mailbox forwarding/rules, and roles/devices.
3. Inspect synthetic evidence and mark each check verified, needs action, or unknown.
4. Record a simulated remediation.
5. Re-run the checklist and produce a closure-readiness summary.

## Acceptance criteria
- Unknown evidence remains visibly unresolved.
- Checklist distinguishes evidence review from remediation.
- Findings link to a concrete next step and verification condition.
- Demo includes a password reset/session revocation scenario with a remaining OAuth grant or mailbox rule.

## Boundaries
Synthetic data only for MVP. No real tenant access, mailbox access, or account modification. Future integrations require explicit authorization, narrow permissions, and audit logging.

## Research leads
- Microsoft compromised identity response SOP includes reviewing/removing inbox rules, OAuth consent, auth methods, role assignments, and sessions: https://learn.microsoft.com/en-us/defender-xdr/sop-documentation-template
- Community report describing OAuth access surviving password reset/session cleanup: https://www.reddit.com/r/EmailSecurity/comments/1un9fw6/i_almost_closed_a_mailbox_compromise_while_mail/
- Community incident response discussion covering rules, forwarding, OAuth grants, and MFA methods: https://www.reddit.com/r/msp/comments/1rro9k7/wrote_up_how_i_investigate_a_suspected_m365/
