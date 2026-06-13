# Uncodixfy

## Summary

Uncodixfy is an AI agent skill and prompt rule set by cyxzdev for improving generated UI design. It is useful when asking Codex, Claude Code, or another coding agent to generate frontend code without falling back to generic AI-dashboard aesthetics.

## Key Points

- The repository provides both a standalone `Uncodixfy.md` rule set and a `SKILL.md` agent skill.
- Its main purpose is to block common AI UI habits such as floating cards, oversized rounded corners, glass panels, decorative labels, generic gradients, fake charts, hero sections inside dashboards, and overproduced SaaS layouts.
- The design direction is restrained and product-oriented: simple sidebars, headers, sections, buttons, cards, forms, tables, tabs, icons, typography, spacing, borders, shadows, and transitions.
- The skill describes its target feel as closer to Linear, Raycast, Stripe, and GitHub than to a generic AI-generated dashboard.
- Installation is documented with `npx skills add cyxzdev/Uncodixfy`; the repository says it can then be invoked with `/uncodixfy`.
- Use this as a guardrail when generating HTML, CSS, React, Vue, Svelte, or other frontend UI code, especially for internal tools and dashboards.

## Sources

- [cyxzdev/Uncodixfy on GitHub](https://github.com/cyxzdev/Uncodixfy)
- [Uncodixfy SKILL.md](https://raw.githubusercontent.com/cyxzdev/Uncodixfy/main/SKILL.md)
- [Uncodixfy rule set](https://raw.githubusercontent.com/cyxzdev/Uncodixfy/main/Uncodixfy.md)

## Related

- [Agent Skills](agent-skills.md)
- [AI Product Design Patterns](../../design/ai-product-design-patterns.md)
- [Storybook Component Workshop](../../development/frontend/storybook-component-workshop.md)
