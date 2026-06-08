# CSS Design Tokens With Open Props

## Summary

Open Props is a CSS custom-property library of reusable design tokens. It looks useful as inspiration for token naming and lightweight CSS systems, but is not a default adoption choice.

## Key Points

- [Open Props](https://open-props.style/) provides framework-agnostic CSS variables for colors, sizes, typography, shadows, borders, gradients, easing, animations, media queries, z-index values, and other low-level design primitives.
- It is non-prescriptive: components still define their own structure and styling, while Open Props supplies consistent token values such as `var(--radius-2)`, `var(--size-fluid-3)`, `var(--shadow-2)`, and `var(--animation-fade-in)`.
- Useful for studying how a compact token set can make plain CSS more consistent without adopting a full component library.
- It can be consumed through CDN imports, npm package imports, PostCSS, JavaScript objects, JSON/design-token files, Figma token formats, Style Dictionary, and web-component/shadow-DOM-oriented builds.
- Individual PropPacks make it possible to import only selected token groups such as colors, sizes, shadows, easing, animations, gradients, or media queries.
- PostCSS JIT Props can ship only the props actually used.
- Treat as a reference and occasional utility, not a planned dependency, unless a project specifically needs a small CSS-variable token foundation.
- License: MIT.

## Sources

- [Open Props](https://open-props.style/)
- [Open Props on GitHub](https://github.com/argyleink/open-props)

## Related

- [Component Variants With Tailwind Variants](component-variants-with-tailwind-variants.md)
- [Storybook Component Workshop](storybook-component-workshop.md)
- [Icon Libraries](../../design/icon-libraries.md)
- [Resources](../../README.md)
