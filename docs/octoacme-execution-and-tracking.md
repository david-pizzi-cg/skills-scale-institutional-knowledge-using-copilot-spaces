# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

### UX Integration Points
- **Feature Planning**: UX Designer creates wireframes and user flow documentation before development begins
- **Development**: Progressive UX reviews during implementation to ensure design compliance
- **Pre-Release**: Usability testing and UX sign-off required for user-facing features
- Use [UX Review Checklist](templates/ux-review-checklist.md) for comprehensive UX validation

### Security Integration Points
- **Pre-Development**: Security Lead conducts threat modeling for new features
- **Development**: Security scanning in CI with Security Lead review for security-sensitive changes
- **Pre-Release**: Security validation and sign-off required before deployment
- Use [Security Checklist](templates/security-checklist.md) for comprehensive security validation

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

### UX/Security Blocker Escalation
- **UX Issues**: UX Designer escalates usability blockers to Product Manager; accessibility compliance issues escalate to project sponsor
- **Security Issues**: Security Lead escalates vulnerabilities based on severity; critical security issues require immediate project sponsor notification
- **Cross-Functional**: PM coordinates escalation when UX or security issues impact project timeline or scope

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
