# Fallow Codebase Intelligence

## Summary

Fallow is an open-source codebase intelligence tool for TypeScript and JavaScript repositories. It produces deterministic static-analysis evidence for code quality, cleanup, architecture, dependency hygiene, duplication, and PR review.

## User Context

- Captured on 2026-06-08 as a good tool to use with AI agents.

## Key Points

- [fallow-rs/fallow](https://github.com/fallow-rs/fallow) is aimed at humans, CI pipelines, editors, and AI agents that need structured repository evidence instead of guesses.
- Free static analysis covers unused code, duplication, complexity hotspots, architecture drift, dependency hygiene, and cleanup opportunities.
- Optional runtime intelligence adds production execution evidence for hot paths, cold paths, and deletion confidence.
- Useful agent-facing surfaces include JSON output, typed output contracts, an MCP server, an LSP, and an Agent Skill.
- Relevant agent workflow: generate or edit code, run `fallow audit --format json`, inspect findings and actions, apply safe fixes, then hand better evidence to a human reviewer.
- Useful commands to remember: `npx fallow`, `npx fallow audit --format json`, `npx fallow health --score --hotspots --targets`, `npx fallow dead-code`, and `npx fallow fix --dry-run --format json`.

## Sources

- [fallow-rs/fallow on GitHub](https://github.com/fallow-rs/fallow)
- [Fallow documentation](https://docs.fallow.tools/)

## Usage References

- [YouTube video on using Fallow](https://www.youtube.com/watch?v=t3my5ByUhFU) describes how to use Fallow.

## Related

- [Agent Skills](../ai/skills/agent-skills.md)
- [AI SDK Tools](ai-sdk/ai-sdk-tools.md)
- [Resources](../README.md)
