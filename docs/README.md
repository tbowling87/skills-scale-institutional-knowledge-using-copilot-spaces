# OctoAcme Project Management Docs

## Project Management Processes Overview

OctoAcme follows a structured lifecycle approach to project management that emphasizes customer value, iterative delivery, and clear ownership. The methodology consists of five core phases:

- **Initiation**: Project ideas are validated through a lightweight One-pager that confirms business need and stakeholder alignment
- **Planning**: Approved projects are broken into shippable increments with prioritized backlogs, acceptance criteria, and risk identification
- **Execution**: Teams follow a defined workflow using GitHub Projects and adhere to pull request standards, automated testing, and quality gates
- **Release**: Features are deployed to production following standardized checklists, smoke tests, and rollback procedures
- **Close & Retrospective**: Learnings are captured and converted into actionable improvements for continuous enhancement

### Key Principles

- **Customer-first**: Prioritize customer value and usability
- **Iterative delivery**: Deliver small, testable increments
- **Clear ownership**: Each project has a named Project Manager (PM) and Product Manager (PdM)
- **Data-informed decisions**: Measure impact and iterate based on evidence
- **Psychological safety**: Encourage feedback and learning

### Core Roles & Communication

OctoAcme uses clearly defined roles to ensure accountability and smooth collaboration:

- **Project Managers (PMs)** coordinate delivery activities, manage schedules, risks, and stakeholder communications
- **Product Managers (PdMs)** define outcomes, prioritize the backlog, and measure success through data-driven metrics
- **Developers** implement features, write tests, and collaborate on design decisions
- **QA/Testing** validates quality and acceptance criteria

Communication is structured through regular cadences: daily standups (15 minutes), weekly delivery syncs, and end-of-sprint demos. Risk escalation follows a three-level model: team-level triage, PM escalation to Product Lead and dependent teams, and sponsor-level escalation for business-impacting issues.

### Quality Assurance & Delivery Discipline

Quality assurance and delivery discipline are embedded throughout the process:

- Pull Request workflow emphasizes small, reviewable changes (≤400 lines) with at least one approval before merging
- Unit tests, integration tests, and end-to-end smoke tests for critical flows
- Security scanning in CI and manual QA for feature acceptance
- Velocity and burndown tracking with dashboards for key signals (errors, latency, usage)

## Available Documents

Navigate to the documentation most relevant to your needs:

| Document | Purpose |
|----------|---------|
| [Project Management Overview](octoacme-project-management-overview.md) | Concise introduction to OctoAcme's approach, roles, and key artifacts |
| [Project Initiation](octoacme-project-initiation.md) | Initial steps to validate and authorize work, align stakeholders, and create a lightweight plan |
| [Project Planning](octoacme-project-planning.md) | Turn an approved initiative into an actionable plan and backlog for delivery |
| [Execution and Tracking](octoacme-execution-and-tracking.md) | Guidance for managing day-to-day execution and tracking progress toward milestones |
| [Risks and Communication](octoacme-risks-and-communication.md) | How to identify, manage, and communicate risks and dependencies |
| [Release and Deployment](octoacme-release-and-deployment.md) | Standardize how OctoAcme releases features to production |
| [Retrospective and Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) | Capture learnings and convert them into actionable improvements |
| [Roles and Personas](octoacme-roles-and-personas.md) | Definitions of typical roles and responsibilities in OctoAcme projects |

## Getting Started

1. **New to OctoAcme?** Start with [Project Management Overview](octoacme-project-management-overview.md) for a high-level introduction
2. **Starting a new project?** Follow the [Project Initiation](octoacme-project-initiation.md) guide
3. **In execution?** Reference [Execution and Tracking](octoacme-execution-and-tracking.md) and [Risks and Communication](octoacme-risks-and-communication.md)
4. **Preparing to release?** Use the [Release and Deployment](octoacme-release-and-deployment.md) guide
5. **After a project or sprint?** Conduct a retrospective using [Retrospective and Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)

## Contributing to These Docs

To request updates, clarifications, or new content for OctoAcme process documentation, use the [Add Content to Project Management Process Docs](../.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml) issue template.
