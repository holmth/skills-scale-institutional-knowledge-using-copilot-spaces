# OctoAcme Project Management Processes

## Overview

OctoAcme follows a structured, customer-focused project management approach designed to deliver value iteratively while maintaining clear ownership, transparency, and continuous improvement. Our methodology emphasizes five core principles:

- **Customer-first:** Prioritize customer value and usability in all decisions
- **Iterative delivery:** Deliver small, testable increments frequently
- **Clear ownership:** Each project has named Project Manager (PM) and Product Lead
- **Data-informed decisions:** Measure impact and iterate based on evidence
- **Psychological safety:** Encourage feedback, learning, and blameless retrospectives

## Process Documents

Navigate the complete OctoAcme project management framework:

- [**Project Management Overview**](octoacme-project-management-overview.md) — Foundational guide to our approach, roles, artifacts, and lifecycle
- [**Project Initiation**](octoacme-project-initiation.md) — Validate business need, align stakeholders, and create a lightweight plan
- [**Project Planning**](octoacme-project-planning.md) — Turn approved initiatives into actionable plans and backlog for delivery
- [**Execution and Tracking**](octoacme-execution-and-tracking.md) — Manage day-to-day execution and track progress toward milestones
- [**Risks and Communication**](octoacme-risks-and-communication.md) — Identify, manage, and communicate risks and dependencies
- [**Release and Deployment**](octoacme-release-and-deployment.md) — Standardize how we release features to production
- [**Retrospective and Continuous Improvement**](octoacme-retrospective-and-continuous-improvement.md) — Capture learnings and convert them into actionable improvements
- [**Roles and Personas**](octoacme-roles-and-personas.md) — Define typical roles and responsibilities in OctoAcme projects

---

## Key Process Summary

### Project Lifecycle Phases

OctoAcme operates through five core phases that ensure structured delivery and alignment:

**1. Initiation**
During initiation, teams validate the business need and create a lightweight Project One-pager that captures the problem statement, success metrics, stakeholders, and initial timeline. Once approved by the Product Lead and sponsor, the project receives a go/no-go decision to move into planning.

**2. Planning**
The project moves from concept to actionable plan. Work is broken into shippable increments with prioritized backlogs, clear acceptance criteria, and a Definition of Done. The team identifies dependencies, risks, and integration points to create a realistic release plan and milestone map.

**3. Execution**
Teams follow a structured rhythm during execution. Daily standups (15 min) focus on progress and blockers, weekly delivery syncs track advancement, and sprint-based iterations are managed on a project board with columns for Backlog, Ready, In Progress, In Review, QA, and Done. Pull requests remain small (≤400 lines) and require at least one approval before merging, with automated testing and linting enforced in CI.

**4. Release & Deployment**
Controlled releases reduce risk and improve observability. Pre-release requirements include all acceptance criteria met, passing CI and security scans, drafted release notes, and a documented rollback plan. Teams deploy to staging, run smoke tests, then move to production with post-deploy verification. If critical issues occur, incident response is triggered and rollback procedures are executed.

**5. Retrospective & Continuous Improvement**
After each sprint, release, or significant milestone, teams reflect on what went well and what could improve. 2–3 prioritized action items are documented with clear owners and due dates. This feedback loop drives iterative process improvements and cultural learning.

### Core Roles & Responsibilities

**Project Manager (PM)**
Coordinates delivery activities, manages schedules, risks, and communications. Maintains project documentation, facilitates meetings (kickoff, planning, retrospectives), and ensures stakeholder alignment. Owns escalation paths and cross-team coordination.

**Product Manager (PdM)**
Defines what should be built to deliver customer and business value. Owns the product vision, prioritizes the backlog, validates solutions through user research, and measures success against defined metrics.

**Developers**
Design, build, test, and deliver software components. Collaborate on acceptance criteria, maintain tests and documentation, participate in code reviews, and help identify technical risks.

**QA/Testing**
Validate quality and acceptance criteria. Execute test plans, manage end-to-end smoke tests, and ensure features meet Definition of Done before release.

### Communication Cadence

- **Daily:** Standups (15 min) with delivery team focusing on progress, blockers, and dependencies
- **Twice-weekly:** Standup meetings or as agreed by the team
- **Weekly:** PM and PdM sync for strategic alignment and risk review
- **Weekly:** Delivery syncs to show progress and flag risks
- **Monthly:** Stakeholder updates on project status and milestones
- **Ad-hoc:** Escalations for blockers or critical issues

### Quality Assurance Practices

Quality is embedded throughout OctoAcme's execution:

- **Code Quality:** Small PRs (≤400 lines), mandatory approvals, automated testing and linting in CI
- **Testing Strategy:** Unit tests for new logic, integration tests where applicable, end-to-end smoke tests for critical flows, security scanning in CI
- **Acceptance:** Manual QA for feature acceptance when needed; all PRs must include issue link and acceptance criteria
- **Pre-release:** Security scans pass, acceptance criteria met, release notes drafted, rollback plan documented
- **Post-release:** Smoke tests run, post-deploy verifications executed, stakeholders notified

### Risk Management

Risks are managed throughout the project lifecycle:

- **Identification:** During planning and ongoing execution
- **Assessment:** Impact and likelihood estimated (High/Med/Low)
- **Mitigation:** Reduced via actions and contingency plans
- **Monitoring:** Reviewed at weekly syncs with status updates
- **Escalation:** Team-level → PM → Product Lead → Sponsor (or Security on-call for security incidents)

---

## Getting Started

1. **New to OctoAcme?** Start with the [Project Management Overview](octoacme-project-management-overview.md)
2. **Starting a new project?** Follow the [Project Initiation](octoacme-project-initiation.md) guide
3. **In active delivery?** Reference [Execution and Tracking](octoacme-execution-and-tracking.md) and [Risks and Communication](octoacme-risks-and-communication.md)
4. **Preparing for release?** See [Release and Deployment](octoacme-release-and-deployment.md)
5. **Wrapping up?** Run a retrospective using [Retrospective and Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)

For role-specific guidance, see [Roles and Personas](octoacme-roles-and-personas.md).

---

## Contributing to This Documentation

Have feedback or want to suggest improvements to these process docs? Please open an issue using the [Add Content to Project Management Process Docs](../.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml) template.
