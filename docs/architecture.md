# Architecture: four levels, one owner

The method organizes AI work the way an engineering organization is organized. Each level has one
job, reads only what that job needs, and hands work down or results up through a fixed format.

| Level | Role | Scope | Typical output |
|---|---|---|---|
| Owner | The human | Every project | Decisions, approvals, merges |
| G · Maestro | One session for all projects | The method itself | Weekly standard and AI budget split, new routines, method changes |
| M · Project Manager | One session per project | One product | Briefs, PR review verdicts, weekly sprint report, decision board |
| P · Area agent / analyst | Specialist for a task | One area of one project | A pull request, or a measured analysis round |
| PP · Subagent | Narrow helper | One task | Structured JSON with evidence |

## Context in the right size

A session never loads the whole method. Each level gets a short card that says what it owns, what it
reads before acting, and what it must never do. A subagent's card fits on one screen. This keeps
sessions cheap and keeps their behavior predictable.

## Boundaries

- A PM works on one product repository only. Projects never see each other's code.
- The Maestro works outside every project. It writes to PMs, not to the products.
- Analysts and subagents read. Writes happen only where a level explicitly owns them.
- The owner is the only one who merges.

## Areas covered by specialists

UX/UI · Security · DevOps & operations · Back-end & data · Payments · Privacy · Performance ·
Text review · Multidisciplinary (end-user view) · Support & product growth.
