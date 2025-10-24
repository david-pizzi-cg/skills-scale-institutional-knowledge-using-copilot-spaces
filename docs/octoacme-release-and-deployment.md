# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted
- Rollback / mitigation plan documented
- Smoke tests prepared

**Release Manager Responsibilities:**
- Coordinate release timeline and stakeholder communication
- Ensure all pre-release requirements are validated
- Manage release artifacts and version control
- Oversee deployment execution and post-release verification

*For detailed release coordination, see [Release Checklist Template](templates/release-checklist.md).*

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support

**Release Manager Leadership:**
- Coordinate deployment activities across teams
- Make go/no-go decisions based on readiness criteria
- Manage deployment timeline and communications
- Oversee rollback procedures if issues arise

*Use the comprehensive [Release Checklist Template](templates/release-checklist.md) for step-by-step coordination.*

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
