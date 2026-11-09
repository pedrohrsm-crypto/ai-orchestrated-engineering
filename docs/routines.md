# Routines

Recurring work runs as scheduled tasks, each bound to its own fixed session.

| Routine | Cadence | What it does |
|---|---|---|
| Standard & budget | Weekly | Checks open PRs without merging, lists what is ready in merge order, writes the weekly standard to the PMs and splits the AI budget across projects |
| Sprint report | Weekly, per project | Flow, risks, decisions, review results, the board |
| Session health | Daily | Finds stuck or idle sessions and orphan tasks; raises cards on the decision board |
| Security check-up | Daily | Read-only checks on database policies, secrets and dependencies |
| UX/UI check-up | Weekly | Layout, themes, accessibility at the worst conditions |
| Support triage | Daily, per product | Classifies incoming messages and prepares reply drafts |
| Improvement window | Weekly | The only door for changing the method's rules |
| Session renewal | Weekly | Replaces long-running fixed sessions with fresh ones and moves their tasks |

## Why fixed sessions, renewed weekly

A routine that runs in a fresh session every time re-learns its setup. A session that runs forever
fills its context and degrades. A fixed session with a weekly renewal keeps the setup and caps the
context.

## Guards

- A repeated trigger during a running round is ignored, not duplicated.
- A routine checks its own result, not just that it ran.
- If something fails, it says what failed; it does not fill gaps with assumptions.
