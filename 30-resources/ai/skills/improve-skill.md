# improve

## Summary

`improve` is an agent skill by shadcn for auditing a codebase and writing self-contained implementation plans that other agents or humans can execute.

## Key Points

- [shadcn/improve](https://github.com/shadcn/improve/tree/main) uses a stronger model for codebase understanding, judgment, and planning, then hands execution to cheaper agents or humans.
- The skill writes plans to `plans/`; the plan is the primary output, not a direct source-code change.
- Usage modes include full audits, quick scans, deep scans, focused audits for areas like security or performance, branch-scoped audits, feature-direction suggestions, direct plan writing, plan review, execution handoff, and backlog reconciliation.
- Plans are intended to be self-contained, with file paths, current-state excerpts, repo conventions, verification gates, done criteria, STOP conditions, and a commit stamp for drift checks.
- Useful for maintaining a backlog of high-leverage codebase improvements while keeping implementation work reviewable and separately executable.
- Installation is documented as `npx skills add shadcn/improve` for agents that support the Agent Skills format.

## Sources

- [shadcn/improve on GitHub](https://github.com/shadcn/improve/tree/main)

## Related

- [Agent Skills](agent-skills.md)
- [Fallow Codebase Intelligence](../../development/fallow-codebase-intelligence.md)
- [Resources](../../README.md)
