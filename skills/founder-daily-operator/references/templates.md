# Ops folder templates

Create these on first run. Replace anything in [brackets].

## PROJECT_REGISTRY.md

```
# Project Registry

| Project | Folder | Stage | Owner | Overnight agents |
|---|---|---|---|---|
| [Project A] | projects/[project-a] | [pilot / live / raising] | [name] | [e.g. supplier follow-up, site QA] |
| [Project B] | projects/[project-b] | | | |
```

## AUTOMATION_GOVERNANCE.md

```
# Automation Governance

## Agents
| Agent | Schedule | Reads | Writes | May act externally? |
|---|---|---|---|---|
| Daily operator | Weekdays [6:00] | everything in ops/ | the five master files only | No |
| [Overnight agent] | [time] | [folders] | projects/[x]/reports/ | [No / drafts only] |

## Founder channel
[Where the operator sends its 4 to 6 line summary, e.g. a text or chat to the founder only. Leave blank to write the summary into DAILY_OPERATOR_REPORT.md instead.]

## Escalate, never act
Money · orders · legal or production commitments · stakeholder messages · deploys · live pricing · anything needing a login
```

## MASTER_CURRENT_STATE.md

```
# Current State: [date]

## [Project A]
- Status: [one line]
- Changed since last run: [one line]
- Blocker: [one line, or none]
```

## MASTER_TASK_QUEUE.md

```
# Task Queue (ranked by leverage)

1. [Task] · [project] · [owner] · [why it ranks here]
2.
```

## MASTER_APPROVAL_QUEUE.md

```
# Approval Queue (true escalations only)

- [ ] [What needs approval] · [project] · [amount or risk] · [deadline]
```

## projects/[project]/CURRENT_STATE.md

```
# [Project]: Current State
- Stage:
- This week's goal:
- Last change:
- Open blockers:
```

## projects/[project]/TASK_QUEUE.md

```
# [Project]: Tasks
- [ ] [task] · [owner] · [due]
```

## projects/[project]/APPROVAL_QUEUE.md

```
# [Project]: Waiting on the founder
- [ ] [item] · [why] · [deadline]
```
