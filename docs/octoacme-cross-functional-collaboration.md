# OctoAcme — Cross-Functional Collaboration Guide

## Purpose
Define interaction patterns, communication workflows, and accountability structures between roles to ensure effective project delivery and minimize delays and ambiguity.

## Core Collaboration Patterns

### Product Manager ↔ Project Manager
- **Frequency:** Weekly sync + ad-hoc as needed
- **Key Topics:**
  - Scope changes and priority adjustments
  - Risk and dependency identification
  - Stakeholder communication and alignment
- **Deliverables:**
  - Updated backlog and roadmap
  - Risk register
  - Status reports and escalations

### Product Manager ↔ Developers
- **Frequency:** Sprint planning, backlog refinement, code review
- **Key Topics:**
  - Acceptance criteria clarification
  - Technical feasibility and trade-offs
  - Definition of Done alignment
- **Deliverables:**
  - Refined user stories
  - Acceptance test cases
  - Design and architecture decisions

### Developers ↔ DevOps Engineers
- **Frequency:** Planning, pre-release, and incidents
- **Key Topics:**
  - CI/CD pipeline requirements
  - Deployment strategy and rollback plans
  - Environment configuration and secrets management
- **Deliverables:**
  - Deployment automation scripts
  - Infrastructure as Code changes
  - Release runbooks

### UX Designers ↔ Developers
- **Frequency:** Design phase, implementation, and UAT
- **Key Topics:**
  - Design specification fidelity
  - Accessibility and responsive design
  - Component library and reusability
- **Deliverables:**
  - Design system components
  - Implemented UI/UX features
  - Accessibility audit results

### UX Designers ↔ Product Manager
- **Frequency:** Discovery, design reviews, user testing
- **Key Topics:**
  - User research findings and insights
  - Design trade-offs and feasibility
  - User satisfaction metrics
- **Deliverables:**
  - User personas and journey maps
  - Design prototypes and feedback
  - Usability test results

### Subject Matter Experts (SME) ↔ All Roles
- **Frequency:** As-needed advisory, key reviews, acceptance checkpoints
- **Key Topics:**
  - Domain-specific requirements and constraints
  - Compliance, security, or business rule validation
  - Quality and correctness assurance
- **Deliverables:**
  - Requirements clarifications
  - Acceptance sign-offs
  - Risk identification and mitigation advice

### QA / Testing ↔ Developers
- **Frequency:** Sprint planning, implementation, pre-release
- **Key Topics:**
  - Test coverage strategy
  - Defect triage and root cause
  - Release readiness validation
- **Deliverables:**
  - Test plans and test cases
  - Defect reports
  - Quality metrics and dashboards

### QA / Testing ↔ Product Manager
- **Frequency:** Acceptance criteria refinement, UAT planning
- **Key Topics:**
  - Test scenario definition
  - Acceptance criteria validation
  - User workflow verification
- **Deliverables:**
  - User acceptance test plans
  - Acceptance sign-offs
  - Quality gate approvals

### Project Manager ↔ All Roles
- **Frequency:** Daily standups, weekly syncs, issue escalation
- **Key Topics:**
  - Progress tracking and blockers
  - Dependency and risk management
  - Timeline and milestone adjustments
- **Deliverables:**
  - Status reports
  - Risk and dependency logs
  - Escalation summaries

---

## Communication Workflows by Phase

### Planning Phase
1. **Product Manager** defines requirements and acceptance criteria
2. **Subject Matter Experts** validate requirements against domain constraints
3. **Developers** and **DevOps** estimate technical scope
4. **Project Manager** consolidates into timeline and resource plan
5. **UX Designer** (if applicable) reviews user workflows and design approach

**Key Synchronization Points:**
- Kickoff meeting (all roles)
- Backlog refinement (PM, PdM, Devs, SME if needed)
- Release planning (PM, PdM, DevOps, Developers)

### Execution Phase
1. **Developers** implement features with acceptance criteria and test coverage
2. **UX Designers** review design implementation and fidelity
3. **Subject Matter Experts** review deliverables for correctness and compliance
4. **QA / Testing** validates acceptance criteria and identifies defects
5. **Project Manager** tracks progress and escalates blockers
6. **DevOps** prepares deployment infrastructure and automation

**Key Synchronization Points:**
- Daily standups (all roles or representatives)
- Design reviews (Devs, UX, PdM)
- Code reviews (Developers + SME/Security review if needed)
- Pre-release QA sign-off (QA, PdM, Developers)

### Release & Deployment Phase
1. **DevOps** deploys to staging and coordinates smoke tests
2. **QA** executes smoke test scenarios
3. **Product Manager** validates feature behavior
4. **DevOps** coordinates production deployment
5. **Project Manager** communicates status to stakeholders

**Key Synchronization Points:**
- Release readiness review (all)
- Production deployment window (PM, DevOps, on-call support)
- Post-deployment verification (QA, DevOps, Developers)

### Post-Release Phase
1. **Developers** assist with production issues and hot fixes
2. **DevOps** monitors systems and alerts on anomalies
3. **QA** validates fixes
4. **Product Manager** gathers user feedback
5. **Project Manager** leads retrospective

**Key Synchronization Points:**
- Incident response (on-call, DevOps, Developers)
- Post-release retrospective (all core team)
- Success metric review (PdM, PM, Developers, QA)

---

## Escalation & Decision-Making

### Dependency Blocking
**Scenario:** Team A cannot proceed without input from Team B.

1. **Level 1:** Identify in daily standup; owners attempt direct resolution (4 hours)
2. **Level 2:** Project Manager facilitates sync between teams (same day)
3. **Level 3:** Escalate to Product Lead or sponsor for prioritization

### Quality or Scope Concern
**Scenario:** QA identifies a gap in acceptance criteria; SME flags a compliance risk.

1. **Level 1:** QA/SME raises with Developers and Product Manager
2. **Level 2:** Product Manager decides: fix now, defer, or redesign
3. **Level 3:** Escalate to Product Lead if impacts timeline or business goal

### Resource Constraint
**Scenario:** A critical skill (e.g., specific SME expertise) is unavailable.

1. **Level 1:** Team identifies during planning; Project Manager flags as risk
2. **Level 2:** Project Manager explores alternatives (cross-training, external resource)
3. **Level 3:** Escalate to sponsor for budget or timeline adjustment

---

## Accountability Matrix (RACI)

| Activity | PM | PdM | Dev | UX | QA | SME | DevOps |
|----------|----|----|-----|----|----|-----|--------|
| Define Requirements | I | R/A | C | C | I | C | I |
| Design Solution | C | R/A | C | R/A | C | C | C |
| Implement Feature | I | C | R/A | C | C | C | C |
| Code Review | I | I | R/A | I | I | C | I |
| User Testing | I | R/A | C | R/A | C | I | I |
| QA & Testing | I | C | C | C | R/A | C | C |
| Deployment Planning | R/A | C | C | I | C | I | R/A |
| Production Deploy | C | I | C | I | I | I | R/A |
| Incident Response | I | I | A | I | I | I | R/A |

**RACI Legend:**
- **R**esponsible: Does the work
- **A**ccountable: Approves or makes final decision
- **C**onsulted: Provides input
- **I**nformed: Kept in the loop

---

## Communication Best Practices

1. **Use async-first where possible:** Update shared docs and dashboards; reserve synchronous meetings for decisions and complex discussions
2. **Write decisions in issues or docs:** Link decisions to the context (requirements, design, risks) for future reference
3. **Clarify assumptions early:** Product Manager and Developers should align on acceptance criteria before implementation begins
4. **Involve SMEs proactively:** Include domain expertise in planning, not just validation
5. **Share metrics and dashboards:** All roles should see progress, quality, and business metrics
6. **Escalate early:** Don't wait for crises; flag risks and dependencies at the planning stage

---

## When to Involve Each Role

| Phase | PM | PdM | Dev | UX | QA | SME | DevOps |
|-------|----|----|-----|----|----|-----|--------|
| Initiation | R | R | C | C | I | C | I |
| Planning | R | R | R | R | R | R | R |
| Design | C | R | R | R | I | C | C |
| Development | R | C | R | C | I | C | C |
| Testing | R | C | C | C | R | C | C |
| Deployment | R | C | C | I | C | I | R |
| Retrospective | R | R | R | C | R | I | C |

---

## Quick Reference: "Who Do I Talk To?"

- **"I have a question about the requirement"** → Product Manager
- **"I need to validate this design"** → UX Designer
- **"I need to understand the business rules"** → Subject Matter Expert
- **"I need to deploy this"** → DevOps Engineer
- **"Is this ready to ship?"** → QA / Product Manager
- **"We're behind schedule"** → Project Manager
- **"What should we prioritize?"** → Product Manager + Project Manager
