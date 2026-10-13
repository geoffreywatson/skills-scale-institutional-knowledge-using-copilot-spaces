# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

---

## Additional Personas

The original OctoAcme role definitions cover the core product and delivery path, but several operational, technical, and governance roles are required for multi-team execution. These personas make accountability clearer, improve handoffs, and reduce ambiguity during planning, execution, and incident response. They are not replacements for the existing roles; instead, they complement them by providing specialized leadership, quality, risk, and release coverage.

### Delivery Lead

The Delivery Lead keeps the team moving day to day. They coordinate sprint execution, surface blockers early, maintain backlog readiness, and ensure the team is aligned on priorities, dependencies, and follow-through from planning through retrospective.

Responsibilities
- Drive day-to-day execution of sprint or iteration work
- Track blockers, decisions, and cross-team dependencies
- Ensure backlog items have clear acceptance criteria and are ready for work
- Coordinate handoffs between design, engineering, QA, and release activities
- Support retrospective follow-through and action tracking

Expected interactions
- Works closely with PM and PdM to translate priorities into delivery plans
- Collaborates with Developers and QA to confirm scope and readiness
- Escalates unresolved cross-team blockers to the PM and relevant stakeholders
- Coordinates with Release Manager and Technical Lead for release readiness

Escalate to this persona when:
- A sprint is at risk due to unclear priorities or unblocked work
- Dependencies across teams are slowing delivery
- Follow-up action items from a retrospective need ownership

Suggested handoff/checklist items
- Updated sprint status and risks
- List of blocked items and owners
- Readiness summary for next sprint or release milestone

### Technical Lead / Architect

The Technical Lead provides technical direction and ensures the system design remains maintainable, secure, and aligned to the project goals. They act as a design authority for complex technical decisions and help the team avoid architectural drift.

Responsibilities
- Define and uphold technical direction and architectural guardrails
- Review major design decisions, technical proposals, and dependencies
- Approve complex technical solutions and trade-offs
- Support Developers with design guidance and risk identification
- Coordinate technical planning for integration points and platform constraints

Expected interactions
- Advises Developers and Product stakeholders on feasibility and trade-offs
- Works with Security Liaison on risk and compliance review needs
- Coordinates with SRE and Release Manager on operational readiness
- Participates in planning where architecture or technical dependencies are material

Escalate to this persona when:
- Key design decisions have business or technical trade-offs
- A solution introduces architectural risk or integration complexity
- There are questions about standards, scalability, or maintainability

Suggested handoff/checklist items
- Architectural decision record or design summary
- Technical dependency map and risk notes
- Sign-off on high-risk implementation choices

### QA Lead / Test Owner

The QA Lead ensures quality is built in from planning through release. They define the testing approach, verify acceptance criteria, and coordinate the testing cadence needed for reliable delivery and release confidence.

Responsibilities
- Define the test strategy for the project or release
- Own integration, functional, and release-level validation planning
- Ensure acceptance criteria are testable and measurable
- Coordinate manual QA and user acceptance testing where needed
- Report quality signals, defects, and release risk to PM and leadership

Expected interactions
- Works with Developers to validate stories and defect fixes
- Collaborates with Delivery Lead to align testing with sprint milestones
- Reports release or quality issues to PM and stakeholders
- Coordinates with Release Manager and Security Liaison when testing gates are involved

Escalate to this persona when:
- A user story does not have clear acceptance criteria or test coverage
- Release risk increases due to failed regression or smoke tests
- Quality concerns affect delivery confidence or launch readiness

Suggested handoff/checklist items
- Test strategy and coverage summary
- Release smoke test checklist
- Known defects, severity, and remediation owners

### Release Manager

The Release Manager owns the planned path to production. They coordinate deployment readiness, ensure rollback plans exist, and keep releases aligned with business and operational constraints.

Responsibilities
- Coordinate release windows and environment readiness
- Own the deployment runbook and rollback strategy
- Confirm pre-release checks and post-release verification are complete
- Communicate release status to stakeholders, PM, and support teams
- Coordinate deployment risk mitigation across teams

Expected interactions
- Works with Developers and QA to confirm release scope and quality gates
- Coordinates with Security Liaison and SRE for operational checks and approvals
- Reports release progress and issues to the PM and Sponsor
- Ensures release notes and stakeholder communication are prepared

Escalate to this persona when:
- A production or staging deployment needs coordination
- Rollback, contingency, or communication planning is required
- Release readiness is unclear across environments or teams

Suggested handoff/checklist items
- Deployment checklist and environment status
- Rollback plan and incident contact list
- Release notes and stakeholder announcement summary

### Security Liaison

The Security Liaison brings security considerations into the project from the beginning and during execution. They help teams meet security expectations without slowing delivery, and they provide a direct path to security review and remediation.

Responsibilities
- Represent Security in planning and delivery discussions
- Review risk, threat, and compliance considerations for the project
- Validate that security checks are included in CI and release gating
- Coordinate remediation planning for vulnerabilities or findings
- Support secure system design and deployment practices

Expected interactions
- Works with Technical Lead and Developers on threat modeling and secure design
- Coordinates with Release Manager to ensure release gates are satisfied
- Advises PM and Stakeholder Representative on compliance or risk trade-offs
- Escalates material risks to the Sponsor or security leadership if needed

Escalate to this persona when:
- A change introduces security, privacy, or compliance risks
- A vulnerability or security finding requires remediation and approval
- Security checks are missing from CI, deployment, or release readiness

Suggested handoff/checklist items
- Security review summary and findings
- Required controls or mitigations
- Sign-off needed before approval or production release

### Data / Analytics Lead

The Data / Analytics Lead ensures the project can measure success and learn from delivery. They define the metrics, instrumentation, dashboards, and analysis needed to validate whether customer and business outcomes are being achieved.

Responsibilities
- Define success metrics and instrumentation requirements
- Design and validate dashboards and reporting for the project
- Ensure analytics and event tracking are built into features where needed
- Support experimentation and post-launch evaluation
- Translate product outcomes into measurable signals for stakeholders

Expected interactions
- Works with PdM to define success metrics and measurement strategy
- Collaborates with Developers to ensure observability and telemetry are built in
- Supports PM and Sponsor with reporting on outcomes and risks
- Coordinates with QA on validation of analytics quality and reliability

Escalate to this persona when:
- Business success metrics are unclear or not measurable
- Key instrumentation or reporting is missing for a release
- Post-launch analysis is needed to understand customer impact

Suggested handoff/checklist items
- Metrics definition and business rationale
- Dashboard and instrumentation checklist
- Validation plan for reporting quality and data accuracy

### Stakeholder Representative (Business Sponsor)

The Stakeholder Representative, often the Business Sponsor, ensures the work remains aligned with business context and organizational priorities. They provide domain insight, decision-making authority, and sponsorship across the project lifecycle.

Responsibilities
- Provide business context and define success expectations
- Approve scope, milestones, and major trade-offs where needed
- Champion the work with broader stakeholder groups
- Help resolve cross-functional conflicts and decision bottlenecks
- Ensure business value and strategic alignment remain visible

Expected interactions
- Meets regularly with PM and PdM to review progress, trade-offs, and decisions
- Works with delivery leaders to confirm priorities and business readiness
- Provides strategic input when scope or sequencing changes are needed
- Coordinates escalation for business-impacting risks or approvals

Escalate to this persona when:
- Scope, priority, or funding decisions require sponsor attention
- Business impact is high and needs executive visibility
- A cross-functional decision is blocking delivery or launch

Suggested handoff/checklist items
- Sponsor briefing and decision summary
- Alignment on milestone changes or scope trade-offs
- Business approval for go/no-go decisions

---

## Responsibility Matrix

| Persona | Primary connection to existing roles | Key responsibility area |
| --- | --- | --- |
| Delivery Lead | PM, PdM, Developers, QA | Day-to-day execution and sprint flow |
| Technical Lead / Architect | Developers, Security Liaison, SRE | Technical direction and design integrity |
| QA Lead / Test Owner | Developers, Delivery Lead, PM | Quality strategy and release validation |
| Release Manager | PM, Developers, QA, Security | Deployment, runbooks, and release coordination |
| Security Liaison | Technical Lead, Developers, Release Manager | Security review, compliance, and risk mitigation |
| Data / Analytics Lead | PdM, Developers, PM | Metrics, instrumentation, and success measurement |
| Stakeholder Representative | PM, PdM, Sponsor, leadership | Business alignment, approvals, and strategic decisions |

This matrix helps teams understand who to engage for specific decisions, issues, and handoffs without duplicating ownership. In practice, these personas should be named and represented as needed per project, while the PM remains responsible for overall coordination and stakeholder communications.
