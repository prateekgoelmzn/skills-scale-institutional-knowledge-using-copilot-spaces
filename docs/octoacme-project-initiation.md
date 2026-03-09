# OctoAcme — Project Initiation Guide

## Purpose
Define the initial steps to validate and authorize work, align stakeholders, and create a lightweight plan.

## When to use
Whenever a new project idea or feature proposal is ready to be explored.

## Goals
- Confirm business need and measurable outcome
- Identify stakeholders & champions
- Define success criteria and initial timeline
- Decide go/no-go for planning

## Initiation Steps

Follow these steps in order. Each step has a clear owner and output.

### Step 1 — Capture the Idea
**Owner:** Product Manager or Business Analyst  
**Output:** Draft Project One-pager

Document the problem and proposed solution at a high level. Focus on the *why* before the *what*.

> **Example:** The OctoAcme checkout flow has a 30% drop-off rate on mobile. We believe a redesigned mobile checkout page will reduce drop-off by 15% over 90 days.

### Step 2 — Identify Stakeholders
**Owner:** Project Manager  
**Output:** Stakeholder list & RACI

List everyone who is affected by, or needs to approve, the project. Define their role using RACI (Responsible, Accountable, Consulted, Informed).

> **Example RACI for the checkout redesign:**
>
> | Name / Role | R | A | C | I |
> |---|---|---|---|---|
> | UX Designer | ✓ | | | |
> | Product Manager | | ✓ | | |
> | Technical Lead | | | ✓ | |
> | Support Engineer | | | | ✓ |

### Step 3 — Define Success Metrics
**Owner:** Product Manager with input from Business Analyst  
**Output:** Measurable success criteria added to the One-pager

Metrics should be SMART (Specific, Measurable, Achievable, Relevant, Time-bound).

> **Example:** Reduce mobile checkout drop-off rate from 30% to ≤ 15% within 90 days of launch, measured via analytics dashboard.

### Step 4 — Assess Risks & Dependencies
**Owner:** Technical Lead + Project Manager  
**Output:** Initial risk list

Identify the top 3–5 risks and any dependencies on other teams or systems.

> **Example risks:**
> - Third-party payment SDK may require upgrade (dependency on vendor release cycle)
> - Design and engineering capacity constrained during Q3 product freeze

### Step 5 — Estimate Resources & Timeline
**Owner:** Project Manager with input from Technical Lead and UX Designer  
**Output:** High-level timeline with key milestones

Use T-shirt sizing (S / M / L / XL) for effort at this stage. A detailed plan is produced during Planning.

> **Example timeline:**
> - Week 1–2: Discovery & design wireframes
> - Week 3–4: Development
> - Week 5: QA & accessibility review
> - Week 6: Staged rollout & monitoring

### Step 6 — Stakeholder Alignment & Go/No-Go
**Owner:** Project Manager  
**Output:** Alignment confirmation (email, meeting notes, or signed-off One-pager)

Present the One-pager to the sponsor and key stakeholders. Capture the decision.

---

## Minimum Deliverables

The following artifacts must exist before moving to the Planning phase:

| Artifact | Owner | Status |
|---|---|---|
| Project One-pager | Product Manager | Required |
| Stakeholder list & RACI | Project Manager | Required |
| High-level timeline & milestones | Project Manager | Required |
| Initial risk list | Technical Lead + Project Manager | Required |
| Resource needs & rough effort | Technical Lead | Required |

---

## Project One-pager Template

Copy this template and fill it in during Step 1–5.

```
Project name:
Problem statement:
  (What problem are we solving and for whom?)
Objective / Goal (SMART):
  (What does success look like in measurable terms?)
Success metrics:
  (e.g., Reduce error rate by 20% within 60 days of launch)
Primary stakeholders:
  (Names and roles — use RACI format if needed)
Suggested timeline / milestones:
  (High-level, e.g., Discovery → Design → Build → QA → Release)
Quick risks & dependencies:
  (Top 3–5 risks and any external dependencies)
Proposed team / roles:
  (e.g., 1 × Technical Lead, 2 × Developers, 1 × UX Designer)
```

> **Filled-in example:**
>
> **Project name:** Mobile Checkout Redesign  
> **Problem statement:** 30% of mobile users abandon checkout before completing payment.  
> **Objective:** Reduce mobile checkout abandonment to ≤ 15% by end of Q3.  
> **Success metrics:** Abandonment rate tracked daily via analytics; measured over 90 days post-launch.  
> **Primary stakeholders:** Head of Product (Accountable), UX Designer (Responsible), Technical Lead (Consulted).  
> **Suggested timeline:** Week 1–2 Discovery, Week 3–4 Build, Week 5 QA, Week 6 Rollout.  
> **Risks:** Payment SDK upgrade dependency; design capacity constraint in Q3.  
> **Proposed team:** 1 × Technical Lead, 2 × Developers, 1 × UX Designer, 1 × Business Analyst.

---

## Initiation Checklist

Complete all items before requesting Planning phase approval.

### Documentation
- [ ] One-pager completed and reviewed by Product Lead
- [ ] Stakeholder list and RACI documented
- [ ] Initial risk list created (minimum 3 risks)
- [ ] High-level timeline with milestones defined

### Alignment
- [ ] Sponsor / Stakeholder alignment confirmed (email or meeting notes attached)
- [ ] Team availability verified for the proposed timeline
- [ ] Budget or resource constraints identified and noted

### Technical Readiness
- [ ] Technical Lead has reviewed feasibility
- [ ] External dependencies identified and owners contacted
- [ ] Compliance or security requirements noted (if applicable)

### Repository Setup
- [ ] Repository or project board skeleton created
- [ ] Initial artifacts added to `docs/` (this One-pager as a minimum)
- [ ] Team members added with appropriate permissions

### Decision Gate
- [ ] Go/No-Go decision recorded and communicated to all stakeholders

---

## Decision Gate

Move to Planning when **all** of the following are true:

- Success metrics are clear and measurable
- Stakeholders agree on priority and scope
- Team availability is confirmed for the proposed timeline
- At least a draft risk list exists
- The Go/No-Go decision has been formally recorded
