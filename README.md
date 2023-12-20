# CoW Project Management

Tracks/coordinate effort/tasks that targets CoW Protocol / Cow Swap as a product across implementations (production readiness, scalability, etc).

## Teams

The CoW Team is currently split in the following subteams:

- Backend (services)
- Solvers
- Frontend

## Work Tracking and Reporting Guidelines

### Requirements

The current reporting requirements are 2 folds:

#### 1. Weekly Reporting

Weekly reporting by subteam of progress on milestones.

#### 2. Monthly Reporting

Monthly reporting is now handled by the <insert> insight team.

### Terminology

| Name            | Number of                               | Timeframe                              | Team Scope                                   | Owner                       | Description                                                                 |
|-----------------|-----------------------------------------|----------------------------------------|----------------------------------------------|-----------------------------|-----------------------------------------------------------------------------|
| Priority Track  | 3-5                                     | Set yearly                             | Whole Team                                   | CTO                   | Focus set for the year, must be aligned with Logos Collective's priorities. |
| (Key) Milestone | 1-3 per year                            | Set yearly-ish                         | Most subteams                                | CTO                   | Key achievements for the CoW Protocol project, historical milestones.               |
| Epic            | Several per milestone                   | Set for a milestone, delivered monthly | Several subteams or external team (e.g. DST) | Team Member (likely a lead) | Chunk of a _Milestone_ across all clients.                                  |
| Task            | Many per Epic                           | Set monthly-ish, delivered weekly      | One subteam or individual                    | Team Member                 | May be one or several piece of work, client specific.                       |  

Owner = person responsible for the delivery and related reporting, may not be doing all the work.

### GitHub Usage

A _Milestone_:
- MUST have a matching GH issue in the https://github.com/cowprotocol/pm repo with `milestone` label assigned.
- MUST have a GH Milestone in https://github.com/cowprotocol/pm repo, to which relevant _Epics_ are added.
- SHOULD have a roadmap to delivery done at planning phase, the GH milestone is then used to track progress.

An _Epic_:
- MUST have a matching GH issue in the https://github.com/cowprotocol/pm with `epic` label assigned.
- MUST have a label with format `E:<epic name>` created across all relevant https://github.com/cowprotocol/ repos (see [labels.yml](./.github/labels.yml)).
- SHOULD be added to a GH Milestone.
- SHOULD have a `Planned Start` and `Due Date` set (these are GitHub projects fields you can find in the `Projects` section of the issue view sidebar).
- MAY list _Tasks_ present in other repos.

A _Task_:
- MAY be tracked as a todo item in a GH Issue (_Task_ or _Epic_),
- OR MAY be tracked as a single GH issue
  - that MUST be labelled with related _Epic_ label (`E:...`),
- OR MAY be tracked as a GH Pull Request
    - that MUST be labelled with related _Epic_ label (`E:...`),
- MUST have an _acceptance criteria_ and/or a list of _tasks_ (that can be other GH issues).

Finally, for _Tasks_ that do not belong to a given _Epic_ or _Milestone_:
- MUST have either labels:
  - `bug`: This is a bug, likely reported by a user
  - `enhancement`: This is an enhancement out of the scope of the technical roadmap, likely reported by a user
    - Major enhancements should be carefully reviewed and prioritized.
  - `documentation`: Documentation improvement or correction.
  - `dependencies`: Upgrade dependencies in a timely manner to avoid time wasting when the dependency upgrade becomes critical.


Which means, in terms of _navigation_:

- Work for a Milestone is described in the related GitHub issue and tracked in the GitHub milestone.
- In the GitHub milestone, we have a list of _Epics_ to be achieved, the _Epics_ are being closed as the work is done across all clients.
- To look at remaining work for an _Epic_, one need to look at all issues/PRs (_Tasks_) with the corresponding _Epic_ label (`E:...`)

## Milestones

https://github.com/cowprotocol/pm/milestones

