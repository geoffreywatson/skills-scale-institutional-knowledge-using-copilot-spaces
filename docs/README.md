# OctoAcme Project Management Docs

This README aggregates OctoAcme's project management process documents and provides a short summary of the approach to make it easier for contributors and stakeholders to find and use these resources.

## Project management processes (summary)

OctoAcme uses a structured, iterative delivery lifecycle that begins with a clear initiation step and continues through planning, execution, release, and continuous improvement. Project initiation focuses on validating the business need, naming stakeholders, and defining measurable success criteria in a short Project One‑pager. Approved initiatives move into planning where work is broken into prioritized backlog items with acceptance criteria, estimates, and a Definition of Done to ensure consistent scope and handoffs.

During execution the team operates with regular short cadences (daily standups, weekly delivery syncs, and milestone demos) and uses a project board to visualize flow (Backlog → Ready → In Progress → In Review → QA → Done). Pull request practices emphasize small, reviewable changes protected by automated CI checks and at least one approval before merge. The Project Manager coordinates schedules, risks, and cross‑team dependencies while Product Managers own outcomes and prioritization; developers and QA focus on implementation, tests, and verification.

Communication is lightweight and purposeful: frequent team syncs, a single source of truth in the docs, weekly stakeholder updates, and explicit escalation paths for blockers. Risk is tracked in a simple risk register (impact, likelihood, owner, mitigation) and reported during regular syncs. Quality assurance is integrated into the workflow with unit and integration tests, CI and security scans, smoke tests before releases, and manual QA for acceptance when needed. Releases follow a checklist-driven approach with rollback and post‑deploy verification steps.

Finally, OctoAcme embeds continuous improvement: retrospectives after sprints and releases capture action items that are tracked back into the backlog, and teams measure the impact of process changes to iterate on how they work.

## Process documents

- docs/octoacme-project-management-overview.md
- docs/octoacme-project-initiation.md
- docs/octoacme-project-planning.md
- docs/octoacme-execution-and-tracking.md
- docs/octoacme-risks-and-communication.md
- docs/octoacme-release-and-deployment.md
- docs/octoacme-retrospective-and-continuous-improvement.md
- docs/octoacme-roles-and-personas.md

## How to contribute

If you'd like to add or update content, please file an issue using the repository's process doc issue template: .github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml. In that issue include which document to update, a summary of the change, the rationale, and any proposed content. Use the acceptance criteria on the template to confirm the change aligns with existing docs and improves clarity.
