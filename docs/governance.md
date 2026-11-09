# Governance

## Decisions with codes

Every item waiting on the owner gets a code by type and number:

| Prefix | Type |
|---|---|
| D | Decision |
| A | Approval |
| AÇ | Action |
| C | Check |
| F | Work front |
| R | Risk |

This lets the owner answer a whole list in one line ("D3 yes, A2 no, AÇ1 after Friday") and keeps
every answer traceable. Codes are never reused.

## One board that asks for attention

Each project has a board; a single "Depends on you" view gathers everything waiting on the owner,
across projects, with the recommendation of the agent that raised it.

## Standing decisions

Decisions that change how the system works (who writes where, how long sessions live, what ends a
project) are recorded in one list, with the date and where they were decided. Agents read it before
acting.

## How the method changes

- A lesson needs evidence and, to become a rule, a second occurrence.
- Proposals collect during the week; one weekly improvement window turns them into a pull request.
- The owner merges it. Versions are tagged only when a project closes.

## Integration

Agents open pull requests. A PM reviews against the project rules and returns a verdict. CI runs.
The owner merges, in the order the weekly standard recommends. No agent merges, rebases shared
history or pushes to `main`.
