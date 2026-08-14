# Day 1 Agile Plan

## Agile Scrum Approach

MedFlow AI will use short, evidence-driven Scrum iterations. Requirements and architecture are expected to evolve through stakeholder feedback, sprint reviews, risk discovery, test results, and retrospectives. Jira will be the authoritative planning system.

## Roles

- **Product Owner:** prioritizes value, acceptance criteria, and scope.
- **Scrum Master:** facilitates events, removes impediments, and protects continuous improvement.
- **Development Team:** collectively designs, implements, tests, secures, documents, and operates increments.
- **Stakeholders:** supervisor, faculty, users, and reviewers provide feedback and acceptance evidence.

## Initial Product Backlog

1. Repository and collaboration compliance
2. Architecture and requirements baseline
3. Authentication, JWT, and RBAC
4. Patient, doctor, and appointment workflows
5. Medical-record workflow
6. AI Service and specialized assistants
7. Supporting healthcare services
8. Testing and API documentation
9. CI/CD and DevSecOps
10. Containers, Kubernetes, monitoring, and hackathon evidence

## Sprint Concept

Each sprint will have one measurable goal and a potentially demonstrable increment. Stories must have acceptance criteria, dependencies, security considerations, estimates, and evidence expectations before selection.

## Jira Workflow

```text
Backlog -> Selected -> In Progress -> Code Review -> Testing -> Done
```

Issue types will include Epic, Story, Task, Bug, and Spike. Blocked work will be visibly flagged.

## Git Workflow and Traceability

```text
Jira Issue -> Git Branch -> Commit -> Pull Request -> Code Review -> Merge -> Deployment
```

- Branches: `main`, `develop`, and `feature/*`.
- Example: `feature/MED-101-authentication`.
- Example commit: `feat(MED-101): add JWT authentication flow`.
- `main` remains stable; feature work is reviewed before merge.
- Every member uses their own GitHub account.
- `review-1`, `review-2`, and `final` are future tags only.

## Daily Progress

The team will record completed work, next actions, blockers, Jira transitions, and relevant commit/PR links. Daily progress should reflect evidence rather than percentage guesses.

## Review Process

Sprint reviews will demonstrate actual increments and collect faculty/stakeholder feedback. Pull requests will check functionality, architecture, security, tests, and documentation. Work is not complete merely because code was written.

## Retrospective Process

The team will identify what helped, what caused delay, and one or two concrete improvements for the next sprint. Actions will have owners and follow-up dates.

## Day 1 Tasks

| Suggested Jira key | Task | Evidence |
|---|---|---|
| MED-001 | Establish repository identity and compliance | Exact naming and policy documented |
| MED-002 | Create mandatory project structure | Required folders and files present |
| MED-003 | Create README | Faculty-required content present |
| MED-004 | Baseline requirements | Requirements document reviewed |
| MED-005 | Baseline architecture | Architecture and constraints documented |
| MED-006 | Establish security baseline | Secret/data policy documented |
| MED-007 | Establish testing strategy | Planned test layers documented |
| MED-008 | Configure GitHub/Jira collaboration | Team access, branches, and Jira board verified manually |

