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

## Additional Personas (proposed)

To improve clarity and accountability — especially on larger or cross-team initiatives — we propose adding the following personas. Each entry lists responsibilities and how they interact with existing roles.

### Technical Program Manager (TPM)
- Responsibilities:
  - Coordinate technical dependencies across multiple teams.
  - Maintain cross-team schedules and integration plans.
  - Drive risk identification and mitigation for technical integration points.
  - Track cross-team progress and unblock technical escalations.
- Interactions:
  - Works closely with Project Managers for schedule alignment and dependency tracking.
  - Partners with Developers and Tech Leads to surface technical risks and allocate work.
  - Collaborates with Product Managers on trade-offs between scope and delivery timelines.
  - Escalates to Product Lead or Sponsor when cross-team decisions require direction.

### Release Manager
- Responsibilities:
  - Own release windows, deployment orchestration, and rollback plans.
  - Maintain release checklists and ensure pre-release validations are complete.
  - Coordinate release communications to stakeholders and support teams.
- Interactions:
  - Coordinates with PMs for release timing and scope freezes.
  - Works with SRE/Operations on deployment pipelines and verification steps.
  - Ensures QA has completed necessary pre-release testing.
  - Notifies Support/Customer Success of upcoming changes and runbooks.

### Site Reliability Engineer (SRE) / Observability Lead
- Responsibilities:
  - Define operational readiness criteria for features (monitoring, alerting, runbooks).
  - Maintain observability standards and production runbooks.
  - Support post-release incident response and reliability improvements.
- Interactions:
  - Partners with Developers to ensure correct instrumentation and performance baselines.
  - Works with Release Manager on rollout strategies (canary, gradual).
  - Provides acceptance criteria related to reliability to PMs and TPMs.
  - Engages with Security when operational controls intersect with compliance.

### Data Analyst / Analytics Lead
- Responsibilities:
  - Define success metrics and measurement plans for features.
  - Specify event schema and instrumentation requirements.
  - Provide analysis and dashboards to evaluate feature impact.
- Interactions:
  - Works with Product Managers to define measurable success criteria.
  - Collaborates with Developers on event tracking and data validation.
  - Informs PM and stakeholders with data-driven prioritization recommendations.
  - Supports retrospective analysis to measure outcomes post-release.

### Design Lead / UX Researcher
- Responsibilities:
  - Ensure solutions meet usability and accessibility standards.
  - Run user research and validation sessions as needed.
  - Provide design specs and acceptance criteria for user-facing work.
- Interactions:
  - Collaborates with Product Managers on user needs and feature direction.
  - Works with Developers to refine implementation details and trade-offs.
  - Partners with QA on accessibility checks and usability test cases.

### Security & Compliance Liaison
- Responsibilities:
  - Surface security, privacy, and compliance requirements early in planning.
  - Conduct threat assessments and recommend mitigations.
  - Provide sign-off where regulatory or compliance controls are required.
- Interactions:
  - Works with Developers and SRE to remediate security findings.
  - Advises PMs/PdMs on scope impacts from compliance needs.
  - Coordinates with the Release Manager to ensure required controls are in place before production rollout.

### Support / Customer Success Liaison
- Responsibilities:
  - Convey customer feedback and critical issues to the delivery team.
  - Maintain support runbooks for new features and known issues.
  - Triage post-release incidents for severity and customer impact.
- Interactions:
  - Works with PM for prioritizing customer-impacting bugs or feature changes.
  - Coordinates with Release Manager for customer-facing communication.
  - Helps Developers reproduce customer issues and provides context.

### Business Analyst / Requirements Owner
- Responsibilities:
  - Translate stakeholder/business needs into clear acceptance criteria and process flows.
  - Document workflows, edge cases, and business rules.
  - Validate requirements with stakeholders before development.
- Interactions:
  - Partners with Product Managers to refine scope and success criteria.
  - Works with Developers and QA to ensure testable, unambiguous requirements.
  - Helps PMs ensure alignment between business objectives and delivery.

---

## How these additional personas improve outcomes
- Clear ownership reduces delays and ambiguous handoffs.
- Better onboarding: newcomers can quickly identify role responsibilities and decision paths.
- Improved risk management by making cross-cutting responsibilities explicit (security, reliability, data).
- More measurable outcomes when analytics ownership is explicit.
- Smoother releases when release coordination and SRE sign-off are part of the process.

---

## Suggested doc edits / next steps
- Add an "Additional Personas" section (as above) to this document, with each persona name, responsibilities, and interactions with existing roles.
- Provide a few example handoffs (e.g., feature -> release -> post-release monitoring) illustrating responsibilities for each step.
- Consider adding a checklist pattern that requires relevant persona sign-off for certain milestones (e.g., SRE sign-off for production readiness, Security sign-off for regulated data handling).
