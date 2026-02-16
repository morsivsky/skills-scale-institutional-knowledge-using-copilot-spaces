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
  - For UI changes, UX/UI Designer reviews design implementation
  - For significant changes, QA/Test Engineer verifies test coverage
  - Security/Compliance Lead reviews security-sensitive changes
  - Technical Writer reviews user-facing documentation changes

## Quality & Testing
- Unit tests for new logic (typically written by Developers)
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI (coordinated with Security/Compliance Lead)
- Manual QA for feature acceptance when needed (led by QA/Test Engineer)
- QA/Test Engineers design and execute comprehensive test plans
- Developers and QA/Test Engineers collaborate on test automation strategy
- UX/UI Designers validate implemented features against design specifications

**Note:** See [octoacme-roles-and-personas.md](octoacme-roles-and-personas.md) for detailed responsibilities of QA/Test Engineers, Developers, and UX/UI Designers in the testing process.

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup (coordinated by Project Manager or Scrum Master)
- Level 2: Product Manager escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

**Role-specific escalations:**
- Quality issues: QA/Test Engineer → Product Manager → Quality Lead
- Security concerns: Security/Compliance Lead → Engineering Lead → CTO/CISO
- Customer impact: Support Engineer → Product Manager → Customer Success Lead

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
