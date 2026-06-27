# Frontend Slides

## Summary

Frontend Slides is a coding-agent skill for creating polished single-file HTML presentations from scratch or by converting PowerPoint files.

## Key Points

- [zarazhangrui/frontend-slides](https://github.com/zarazhangrui/frontend-slides) packages a presentation-generation workflow as a Claude Code plugin and reusable `SKILL.md` for other local coding agents.
- The skill is aimed at non-designers who want web-based decks without writing CSS or JavaScript directly.
- Output is designed as fixed 16:9 HTML slides with inline CSS/JS, no build step, and no framework dependency.
- Key workflow: gather content, generate visual style previews, let the user choose a direction, then build the full deck.
- It can also convert existing PowerPoint files by extracting text, images, and notes before generating a web slideshow.
- Included style systems cover dark, light, specialty, and bold template-pack directions, with anti-generic-AI aesthetics as an explicit goal.
- Claude Code installation is documented through a custom plugin marketplace source, while other agents can read the repo and start from `SKILL.md`.

## Sources

- [zarazhangrui/frontend-slides on GitHub](https://github.com/zarazhangrui/frontend-slides)

## Usage References

- [YouTube video about Frontend Slides](https://www.youtube.com/watch?v=jvB2F_hYkXA)

## Related

- [Agent Skills](agent-skills.md)
- [drawio-skill](drawio-skill.md)
- [Napkin AI Visual Storytelling](../../design/napkin-ai-visual-storytelling.md)
- [Resources](../../README.md)
