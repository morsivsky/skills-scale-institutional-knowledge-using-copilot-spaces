# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans (verified by Security/Compliance Lead)
- QA/Test Engineer confirms all test plans executed and critical bugs resolved
- Release notes drafted (by Technical Writer with input from Product Manager)
- Rollback / mitigation plan documented
- Smoke tests prepared and reviewed by QA/Test Engineer
- Support Engineer/Customer Success team briefed on changes and potential impact

## Deployment Checklist
- [ ] Deployment window scheduled (if needed) - coordinated by Project Manager
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests (executed by QA/Test Engineer)
- [ ] Security validation performed (by Security/Compliance Lead for sensitive changes)
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications (QA/Test Engineer validates critical flows)
- [ ] Announce release to stakeholders and Support team
- [ ] Support Engineer/Customer Success team monitors for issues
- [ ] Update user-facing documentation (Technical Writer publishes release notes)

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call (Project Manager coordinates)
  - Rollback to last known-good release if necessary (executed by Developers)
  - Security/Compliance Lead notified if security implications exist
  - Support Engineer/Customer Success tracks customer impact
  - Triage root cause and capture action items
  - QA/Test Engineer validates rollback success
  
**Note:** See [octoacme-roles-and-personas.md](octoacme-roles-and-personas.md) for detailed role responsibilities during incidents.

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
