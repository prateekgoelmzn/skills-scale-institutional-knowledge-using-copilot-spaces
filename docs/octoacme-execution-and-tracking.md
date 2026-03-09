# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

---

## Team Rhythm

Consistent ceremonies keep the team aligned and surface blockers early.

| Ceremony | Cadence | Duration | Owner | Purpose |
|---|---|---|---|---|
| Daily Standup | Daily | 15 min | Scrum Master | Progress, blockers, dependencies |
| Weekly Delivery Sync | Weekly | 30 min | Project Manager | Progress updates, risk review |
| Sprint / Milestone Review | End of each sprint | 1 hr | Product Manager | Demo, stakeholder feedback |
| Retrospective | End of each sprint | 1 hr | Scrum Master | Process improvement |
| Backlog Refinement | Weekly | 30–45 min | Product Manager + Tech Lead | Groom and estimate upcoming work |

> **Example standup format:**
> 1. What did I complete since yesterday?
> 2. What will I work on today?
> 3. Do I have any blockers or dependencies?

---

## Workflows

### Project Board
Use a GitHub Projects board (or equivalent) with the following columns:

```
Backlog → Ready → In Progress → In Review → QA → Done
```

**Column definitions:**
- **Backlog:** All captured work, not yet prioritized
- **Ready:** Prioritized and groomed; ready to be picked up
- **In Progress:** Actively being worked on (limit WIP per developer)
- **In Review:** PR open and awaiting code review
- **QA:** Feature complete; undergoing manual or automated QA
- **Done:** Accepted by Product Manager and deployed or releasable

### Pull Request Workflow

All code changes follow this workflow:

1. Create a feature branch from `main` (or the agreed base branch): `git checkout -b feat/issue-123-mobile-checkout`
2. Implement the change, keeping PRs small (≤ 400 lines when possible)
3. Include in the PR description:
   - Link to the issue or ticket: `Closes #123`
   - Summary of changes
   - Acceptance criteria and how they were verified
   - Screenshots or recordings for UI changes
4. Ensure CI passes (tests, linting, security scanning) before requesting review
5. Request review from at least one team member (Technical Lead for architectural changes)
6. Address review feedback; re-request review if significant changes were made
7. Merge only after approval and green CI

> **Example PR description template:**
>
> ```
> ## Summary
> Redesigned the mobile checkout step-indicator component.
>
> ## Changes
> - Replaced legacy stepper with new accessible component
> - Added aria-labels for screen reader support
>
> ## Verification
> - [x] Unit tests updated and passing
> - [x] Manual QA on iOS Safari and Chrome Android
> - [x] Accessibility audit passed (axe DevTools)
>
> Closes #123
> ```

---

## Quality & Testing

| Test Type | When | Owner |
|---|---|---|
| Unit tests | For every new function or class | Developer |
| Integration tests | When services interact | Developer |
| End-to-end (E2E) smoke tests | Before each release | QA / Developer |
| Accessibility audit | For all UI changes | UX Designer + Developer |
| Security scanning | Every CI run | Automated (CI) |
| Manual QA / Acceptance | Feature completion | Product Manager + QA |

> **Example definition of "done":**
> - Unit and integration tests written and passing
> - Code reviewed and approved
> - Acceptance criteria verified by Product Manager
> - No critical/high security findings in CI scan
> - Deployed to staging and smoke-tested

---

## Reporting & Metrics

Track the following signals to stay informed and catch drift early.

### Delivery Metrics
- **Velocity:** Story points or issues completed per sprint
- **Burndown:** Remaining work vs. time in sprint
- **Cycle time:** Average time from "In Progress" to "Done"
- **PR lead time:** Average time from PR open to merge

### Product / Business Metrics
- Success metrics defined in the Project One-pager (e.g., mobile checkout abandonment rate)
- Error rates, latency, and uptime from production dashboards

> **Example weekly status update format:**
>
> | Metric | Last Week | This Week | Trend |
> |---|---|---|---|
> | Sprint velocity | 34 pts | 38 pts | ↑ |
> | Open blockers | 2 | 1 | ↓ |
> | PR cycle time | 2.1 days | 1.8 days | ↓ |
> | Checkout abandonment | 28% | 26% | ↓ |

---

## Blocker Escalation

Use this escalation path when a blocker cannot be resolved at the team level.

| Level | Trigger | Owner | Action |
|---|---|---|---|
| Level 1 | Blocker identified | Developer / Scrum Master | Raise in daily standup; team attempts to resolve within 24 hours |
| Level 2 | Not resolved after 24 hours | Project Manager | Escalate to Product Lead and dependent team leads |
| Level 3 | Business-impacting; sprint at risk | Project Manager + Sponsor | Sponsor-level escalation; may require scope or timeline adjustment |

> **Example Level 2 escalation note:**
>
> > "The third-party payment API is returning 500 errors for 15% of requests. Our team has contacted the vendor (ticket #API-4521). Estimated resolution is 48 hours. We may need to defer the mobile checkout release by one sprint. Requesting Product Lead input on priority."

---

## Execution Checklist

Complete the relevant items at each stage of execution.

### Sprint Start
- [ ] Sprint goal defined and communicated to the team
- [ ] All "Ready" tickets have clear acceptance criteria
- [ ] WIP limits set and understood by the team
- [ ] Branching and PR conventions documented in the repo (e.g., `CONTRIBUTING.md`)

### During Sprint
- [ ] Daily standups held; blockers recorded in the impediment log
- [ ] Project board kept up-to-date by all team members
- [ ] Risk register reviewed and updated weekly
- [ ] CI configured and passing for all open PRs (tests, lint, security scan)

### Sprint End
- [ ] Sprint review / demo conducted with stakeholders
- [ ] All "Done" items accepted by the Product Manager
- [ ] Retrospective held; at least one improvement action recorded
- [ ] Delivery metrics captured (velocity, cycle time)
- [ ] Success metrics checked against targets from the Project One-pager

### Release Readiness
- [ ] All acceptance criteria verified
- [ ] E2E smoke tests passing on staging
- [ ] Release notes drafted
- [ ] Rollback plan documented
- [ ] Monitoring and alerting confirmed active post-deploy
