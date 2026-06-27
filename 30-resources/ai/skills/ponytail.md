# Ponytail

## Summary

Ponytail is an AI agent ruleset and skill package that pushes coding agents toward the smallest sufficient implementation: skip unnecessary work, prefer standard library and native platform features, reuse installed dependencies, and only write custom code when needed.

## Key Points

- [DietrichGebert/ponytail](https://github.com/DietrichGebert/ponytail) packages terse, senior-engineer-style coding guidance for agents across Codex, Claude Code, Copilot CLI, OpenCode, Gemini CLI, OpenClaw, Cursor, Windsurf, Cline, Aider, and Kiro.
- The core decision ladder is: does this need to exist, can the standard library do it, can the native platform do it, can an installed dependency do it, can one line do it, and only then write the minimum custom implementation.
- It explicitly preserves trust-boundary validation, data-loss handling, security, and accessibility; the goal is necessary code, not code golf.
- Commands include `/ponytail` mode switching, `/ponytail-review` for over-engineering review, `/ponytail-audit` for repo-wide over-engineering audit, `/ponytail-debt` for tracking deferred `ponytail:` shortcuts, and `/ponytail-help`.
- Codex installation is through the plugin marketplace: `codex plugin marketplace add DietrichGebert/ponytail`, then install Ponytail from `/plugins` and review its hooks from `/hooks`.
- Useful when agents tend to overbuild wrappers, abstractions, helper layers, configuration systems, or dependency-heavy solutions for simple tasks.

## Sources

- [DietrichGebert/ponytail on GitHub](https://github.com/DietrichGebert/ponytail)

## Related

- [Agent Skills](agent-skills.md)
- [Caveman Skill](caveman-skill.md)
- [Uncodixfy](uncodixfy.md)
- [improve](improve-skill.md)
- [Resources](../../README.md)
