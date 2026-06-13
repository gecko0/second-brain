# OpenUI Generative UI Framework

## Summary

OpenUI is an open-source framework for generating rich, structured UI from LLM output. It is useful when a product needs model-generated interfaces that render as real components instead of plain text or loose JSON.

## Key Points

- [OpenUI](https://github.com/thesysdev/openui) describes itself as a full-stack Generative UI framework with a compact streaming-first language, React runtime, built-in component libraries, and ready-to-use chat interfaces.
- The core idea is OpenUI Lang: the model emits a structured, streamable UI language that a React renderer can progressively parse and display as tokens arrive.
- Components define what the model is allowed to generate. The framework can generate prompt instructions from the registered component library, giving the LLM constrained UI affordances instead of arbitrary markup.
- Built-in libraries include common rich UI primitives such as charts, forms, tables, and layouts, while still allowing custom component libraries.
- This looks especially relevant for rich UI generation from LLMs because it combines controlled rendering, typed component contracts, streaming UI, and lower-token output than JSON-style formats.
- The project includes packages for React runtime/rendering, headless chat state and streaming adapters, prebuilt chat layouts, and a CLI for scaffolding apps and generating system prompts.
- Quick-start command from the project: `npx @openuidev/cli@latest create --name genui-chat-app`.

## Sources

- [thesysdev/openui GitHub repository](https://github.com/thesysdev/openui)
- [OpenUI documentation](https://www.openui.com/)

## Related

- [Storybook Component Workshop](storybook-component-workshop.md)
- [Component Variants With Tailwind Variants](component-variants-with-tailwind-variants.md)
- [AI Product Design Patterns](../../design/ai-product-design-patterns.md)
- [AI UI Intent Capture](../../design/ai-ui-intent-capture.md)
