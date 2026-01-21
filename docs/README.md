# OctoAcme Project Management Guide

Welcome to OctoAcme! This guide provides an overview of how we manage projects from initiation to release and continuous improvement. Whether you're a new teammate or stakeholder, this document will help you understand our processes, workflows, and practices.

## Table of Contents

- [Overview](#overview)
- [Core Principles](#core-principles)
- [Roles and Responsibilities](#roles-and-responsibilities)
- [Project Lifecycle](#project-lifecycle)
- [Key Workflows](#key-workflows)
- [Communication Strategies](#communication-strategies)
- [Quality Assurance Practices](#quality-assurance-practices)
- [Key Artifacts](#key-artifacts)
- [Additional Resources](#additional-resources)

## Overview

OctoAcme follows a structured yet flexible approach to project management that emphasizes customer value, iterative delivery, and continuous improvement. Our processes apply to all cross-functional projects that deliver product features, services, or integrations.

## Core Principles

Our project management approach is built on these foundational principles:

- **Customer-first**: Prioritize customer value and usability in every decision
- **Iterative delivery**: Deliver small, testable increments to enable rapid feedback
- **Clear ownership**: Each project has a named Project Manager (PM) and Product Lead
- **Data-informed decisions**: Measure impact and iterate based on evidence
- **Psychological safety**: Encourage feedback, learning, and blameless retrospectives

## Roles and Responsibilities

### Project Manager (PM)
**Coordinates delivery, schedules, risk, and communications**

- Creates and maintains project plans and timelines
- Manages risks, dependencies, and resource constraints
- Facilitates meetings (kickoff, planning, retrospectives)
- Ensures consistent project documentation and status reporting
- Coordinates cross-team and stakeholder communication

**Communication**: Weekly status updates, risk registers, decision logs, project boards

### Product Manager (PdM)
**Defines what should be built to deliver customer and business value** *(also referred to as Product Lead)*

- Defines problem statements and success metrics
- Prioritizes the roadmap and backlog
- Collaborates with stakeholders and engineering on trade-offs
- Validates solutions through user research and metrics

**Communication**: Weekly alignment with PM and engineering leads, roadmap updates, acceptance criteria

### Developers
**Design, build, test, and deliver software components**

- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

**Communication**: Daily standups, sprint planning, PR descriptions, code review comments

### QA/Testing
**Validate quality and acceptance criteria**

- Execute test plans and validate features
- Report issues and track resolution
- Collaborate on test automation

### Business Analyst
**Bridge the gap between business and technical teams**

- Gather and refine requirements from stakeholders
- Translate business needs into actionable user stories
- Support UAT planning and execution

### Change Manager
**Coordinate project changes and assess impacts**

- Evaluate change requests and their impacts
- Document and communicate changes to stakeholders
- Maintain project stability while enabling adaptations

### Release Coordinator
**Manage deployment activities and release readiness**

- Plan and schedule releases
- Verify pre-release requirements are met
- Coordinate deployment communications

### Stakeholders
**Provide inputs, feedback, and approvals**

- Review project progress and provide guidance
- Make key decisions and remove obstacles
- Stay informed through regular updates

📖 [Learn more about all roles and personas →](octoacme-roles-and-personas.md)

## Project Lifecycle

Our projects follow a five-phase lifecycle:

### 1. Initiation
**Goal**: Validate and authorize work, align stakeholders, create lightweight plan

**Key Activities**:
- Confirm business need and measurable outcome
- Identify stakeholders and champions
- Create Project One-pager (Problem, Goal, Success Metrics)
- Define initial timeline and key milestones
- Conduct initial risk assessment

**Decision Gate**: Move to planning when success metrics are clear, stakeholders agree on priority, and team availability is confirmed.

📖 [Learn more about project initiation →](octoacme-project-initiation.md)

### 2. Planning
**Goal**: Turn approved initiative into actionable plan and backlog

**Key Activities**:
- Hold kickoff meeting with stakeholders and delivery team
- Create prioritized backlog with acceptance criteria
- Estimate scope (T-shirt sizing or story points)
- Define Definition of Done (DoD)
- Identify dependencies and integration points
- Create release plan and milestone map

📖 [Learn more about project planning →](octoacme-project-planning.md)

### 3. Execution & Tracking
**Goal**: Build, test, review, and iterate toward project milestones

**Key Activities**:
- Manage day-to-day execution using project boards
- Follow PR workflow with automated testing
- Run daily standups and weekly delivery syncs
- Track velocity and burndown
- Update risk register weekly
- Demo progress at end of each sprint

📖 [Learn more about execution and tracking →](octoacme-execution-and-tracking.md)

### 4. Release & Deployment
**Goal**: Deploy to production safely with minimal risk

**Key Activities**:
- Ensure all acceptance criteria met and PRs merged
- Verify passing CI and security scans
- Draft release notes
- Deploy to staging and run smoke tests
- Deploy to production (automated pipeline preferred)
- Run post-deploy verifications
- Announce release to stakeholders

📖 [Learn more about release and deployment →](octoacme-release-and-deployment.md)

### 5. Close & Retrospective
**Goal**: Capture learnings and convert them into actionable improvements

**Key Activities**:
- Review what went well and what could be improved
- Document action items with owners and due dates
- Follow up on previous action items
- Celebrate successes and close project

📖 [Learn more about retrospectives →](octoacme-retrospective-and-continuous-improvement.md)

## Key Workflows

### Pull Request Workflow
1. Create small PRs (≤ 400 lines when possible)
2. Include issue link and acceptance criteria in PR description
3. Run automated tests and linting in CI before requesting review
4. Require at least one approval before merging
5. Merge to main branch

### Risk Management Workflow
1. **Identify**: Capture risks during planning and ongoing execution
2. **Assess**: Estimate impact and likelihood (High/Med/Low)
3. **Mitigate**: Develop contingency plans and actions
4. **Monitor**: Review at weekly syncs and update status

### Blocker Escalation
- **Level 1**: Team-level triage in daily standup
- **Level 2**: PM escalates to Product Lead and dependent teams
- **Level 3**: Sponsor-level escalation for business-impacting issues

📖 [Learn more about risk management and communication →](octoacme-risks-and-communication.md)

## Communication Strategies

### Communication Cadence

| Meeting | Frequency | Participants | Purpose |
|---------|-----------|--------------|---------|
| PM + PdM Sync | Weekly | PM, Product Manager | Alignment on priorities, risks, decisions |
| Team Standup | Daily or twice-weekly (as agreed) | Delivery team | Progress, blockers, dependencies |
| Delivery Sync | Weekly | Delivery team, PM | Show progress, updates, flagged risks |
| Demo/Review | End of sprint | Team + stakeholders | Demonstrate completed work |
| Stakeholder Updates | Monthly | PM, stakeholders | Project status and upcoming milestones |

### Communication Templates

**Weekly Status Update**:
- Progress this week
- Next steps
- Risks & blockers
- Ask / decisions needed

**Incident Communication**:
- Triage summary
- Actions being taken
- Expected timeline
- Post-incident retrospective scheduled

### Escalation Paths
Team-level → PM → Product Lead → Sponsor

For security incidents, follow the security incident runbook and notify Security on-call.

## Quality Assurance Practices

### Testing Strategy
- **Unit tests**: Required for new logic
- **Integration tests**: Applied where applicable
- **End-to-end smoke tests**: Run for critical flows before release
- **Security scanning**: Automated in CI pipeline
- **Manual QA**: Conducted for feature acceptance when needed

### Definition of Done
Each team defines their own DoD, but typically includes:
- Code complete and reviewed
- Tests written and passing
- Documentation updated
- Acceptance criteria met
- No critical bugs
- Security scans passing

### Quality Gates
- All tests must pass in CI before PR merge
- At least one code review approval required
- Security scans must pass
- Smoke tests must pass in staging before production deployment

## Key Artifacts

Throughout a project, teams maintain these key documents:

| Artifact | Owner | Purpose |
|----------|-------|---------|
| Project Charter / One-pager | PM + PdM | Define problem, goals, success metrics |
| Roadmap and Release Plan | PdM | Timeline and feature prioritization |
| Sprint/Iteration Backlog | Team | Current work in progress |
| Acceptance Criteria & DoD | PdM + Team | Quality standards and success criteria |
| Risk Register | PM | Track and manage risks |
| Retrospective Notes | PM + Team | Capture learnings and action items |
| Release Notes | PM + PdM | Document changes for stakeholders |

## Additional Resources

- [Project Management Overview](octoacme-project-management-overview.md) - Concise introduction to our approach
- [Roles and Personas](octoacme-roles-and-personas.md) - Detailed role definitions including new personas
- [Stakeholder Responsibility Matrix](octoacme-stakeholder-responsibility-matrix.md) - RACI matrix for clear accountability
- [Project Initiation](octoacme-project-initiation.md) - How to start a new project
- [Project Planning](octoacme-project-planning.md) - Planning process and templates
- [Execution and Tracking](octoacme-execution-and-tracking.md) - Day-to-day execution guidance
- [Release and Deployment](octoacme-release-and-deployment.md) - Release process and checklists
- [Release Readiness Checklist](octoacme-release-readiness-checklist.md) - Comprehensive pre-release verification
- [Change Management Process](octoacme-change-management-process.md) - Structured approach for managing changes
- [Retrospective and Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) - Learning and improvement practices
- [Risk Management and Communication](octoacme-risks-and-communication.md) - Risk and stakeholder communication

---

## Quick Start for New Team Members

1. **Understand your role**: Review the [Roles and Responsibilities](#roles-and-responsibilities) section
2. **Learn the lifecycle**: Familiarize yourself with our [Project Lifecycle](#project-lifecycle)
3. **Join the communication channels**: Connect with your PM to get added to standups and syncs
4. **Review current projects**: Check project boards and recent updates
5. **Ask questions**: Our culture values psychological safety—don't hesitate to ask!

## Getting Help

- **For project-specific questions**: Contact your Project Manager
- **For product questions**: Contact your Product Manager
- **For process questions**: Refer to the detailed documentation linked throughout this guide
- **For technical blockers**: Escalate in daily standup or reach out to your tech lead

---

**Last Updated**: January 2026

*This documentation is maintained by the OctoAcme Project Management team. For suggestions or updates, please open an issue or submit a PR.*
