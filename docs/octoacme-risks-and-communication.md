# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain a simple table with:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner
- Mitigation plan
- Status

## Risk Lifecycle
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support, customers)
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status
- Product Manager and Project Manager coordinate overall stakeholder communication
- Technical Writer maintains user-facing communication and documentation
- Support Engineer/Customer Success represents customer needs and feedback
- Security/Compliance Lead provides security and compliance updates to stakeholders

## Communication Templates
Weekly Status Template:
- Progress this week:
- Next steps:
- Risks & blockers:
- Ask / decisions needed:

Incident Communication
- Triage summary (coordinated by Project Manager)
- Actions being taken (executed by Developers with support from relevant specialists)
- Expected timeline
- Customer impact assessment (provided by Support Engineer/Customer Success)
- Security implications (assessed by Security/Compliance Lead if applicable)
- Post-incident blameless retrospective scheduled

## Escalation Paths
- Team-level → Project Manager → Product Lead → Sponsor
- For security incidents, Security/Compliance Lead follows the security incident runbook and notifies Security on-call
- For customer-impacting issues, Support Engineer escalates to Product Manager and Customer Success Lead
- For quality concerns, QA/Test Engineer escalates to Project Manager and Quality Lead
- For compliance issues, Security/Compliance Lead escalates directly to executive leadership

**Note:** See [octoacme-roles-and-personas.md](octoacme-roles-and-personas.md) for role-specific escalation responsibilities.
