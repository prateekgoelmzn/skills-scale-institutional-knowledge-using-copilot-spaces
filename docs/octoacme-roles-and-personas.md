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

## Technical Lead

### Role Summary
The Technical Lead is the most senior engineer on a project team. They guide architectural decisions, set technical standards, and ensure code quality while actively contributing to development.

### Responsibilities
- Define and document the technical architecture and key design decisions
- Review and approve significant code changes and architectural pull requests
- Mentor developers and promote engineering best practices
- Identify and mitigate technical risks early in the project lifecycle
- Serve as the primary technical liaison between engineering and Product/Project Management

### Goals
- Ensure technical decisions align with long-term system health and scalability
- Reduce technical debt through proactive design and review
- Maintain a high engineering bar across the team

### Typical Communication
- Architecture decision records (ADRs) and design documents
- Code review feedback and pair programming sessions
- Technical briefings for Product Managers and Project Managers
- Participation in sprint planning and retrospectives

---

## UX Designer

### Role Summary
UX Designers are responsible for the user experience of products — from research and wireframes to final design assets and usability validation.

### Responsibilities
- Conduct user research, interviews, and usability testing
- Create wireframes, prototypes, and high-fidelity design mockups
- Define and maintain the design system and component library
- Collaborate with developers to ensure faithful implementation of designs
- Advocate for accessibility and inclusive design standards

### Goals
- Deliver intuitive, accessible experiences that meet user needs
- Reduce friction and support task completion for end users
- Ensure design consistency across the product

### Typical Communication
- Design review sessions with developers and Product Managers
- Usability test reports and user research summaries
- Figma or similar design tool links shared in PRs and tickets
- Participation in sprint demos to validate implementation fidelity

---

## Business Analyst

### Role Summary
Business Analysts bridge the gap between business stakeholders and the delivery team. They translate business needs into clear, actionable requirements that the team can execute against.

### Responsibilities
- Elicit and document business requirements from stakeholders
- Create and maintain user stories, acceptance criteria, and process flows
- Validate that delivered features meet business intent
- Facilitate requirements workshops and stakeholder reviews
- Maintain a shared understanding of scope and priorities

### Goals
- Ensure business requirements are captured accurately and completely
- Reduce ambiguity and rework caused by unclear requirements
- Support sign-off and acceptance of delivered features

### Typical Communication
- Requirements documents, user story maps, and process diagrams
- Collaborative grooming sessions with Product Managers and Developers
- Stakeholder review meetings and sign-off sessions
- Traceability matrices linking requirements to delivered features

---

## Scrum Master / Agile Coach

### Role Summary
The Scrum Master or Agile Coach facilitates agile ceremonies, removes impediments, and continuously improves team processes. They protect the team's focus and foster a culture of continuous improvement.

### Responsibilities
- Facilitate sprint ceremonies: planning, daily standups, reviews, and retrospectives
- Identify and remove impediments that block team progress
- Coach the team on agile principles and practices
- Track and report sprint metrics (velocity, burndown, cycle time)
- Shield the team from external interruptions and scope changes mid-sprint

### Goals
- Enable a high-performing, self-organizing team
- Improve delivery predictability and flow efficiency
- Foster psychological safety and a continuous improvement mindset

### Typical Communication
- Sprint ceremonies and retrospective action items
- Impediment logs and escalation when needed
- Agile metrics dashboards shared with stakeholders
- One-on-one coaching conversations with team members

---

## Support Engineer

### Role Summary
Support Engineers are the first line of defence for production issues. They triage incoming incidents, resolve customer-impacting problems, and work with the development team to implement permanent fixes.

### Responsibilities
- Monitor production systems and respond to incidents and alerts
- Triage and prioritize support tickets and bug reports
- Reproduce issues and provide detailed reproduction steps to developers
- Communicate clearly with customers and stakeholders during incidents
- Contribute to runbooks, FAQs, and knowledge-base articles

### Goals
- Minimize customer impact from production issues
- Reduce mean time to resolution (MTTR) for incidents
- Improve system reliability through feedback loops with engineering

### Typical Communication
- Incident reports and post-mortems
- Support ticket updates and customer-facing status messages
- Bug reports filed in the project backlog with reproduction steps
- Handoff notes during on-call rotations

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- When crafting a Copilot Space, select the persona(s) most relevant to your question or workflow to receive tailored, role-aware responses.

### Persona Interaction Map
The table below summarizes how each role typically interacts with others during a project lifecycle.

| Role | Primary Collaborators | Key Handoffs |
|---|---|---|
| Developer | Technical Lead, UX Designer, Business Analyst | Code → Code Review → QA → Release |
| Product Manager | Business Analyst, Project Manager, Stakeholders | Roadmap → Backlog → Acceptance |
| Project Manager | All roles | Status reports, risk register, escalation |
| Technical Lead | Developers, Product Manager, Architects | ADRs, design reviews, technical sign-off |
| UX Designer | Product Manager, Developers, Business Analyst | Wireframes → Mockups → Implementation review |
| Business Analyst | Product Manager, Developers, Stakeholders | Requirements → User stories → Acceptance criteria |
| Scrum Master / Agile Coach | All roles | Sprint ceremonies, impediment removal |
| Support Engineer | Developers, Technical Lead, Customers | Incidents → Bug reports → Post-mortems |

