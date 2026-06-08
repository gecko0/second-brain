# Component Variants With Tailwind Variants

## Summary

Tailwind Variants is a first-class variant API for Tailwind CSS, useful for defining component design variations in a typed, reusable way.

## Key Points

- [Tailwind Variants](https://www.tailwind-variants.org/docs/introduction) provides a `tv()` helper for defining `base` styles, `variants`, `compoundVariants`, and `defaultVariants`.
- It is useful for design-system components where size, color, intent, state, and other visual variants should be expressed as data instead of scattered conditional class strings.
- The variant call returns a class builder, so component usage stays clean: call `button({ size: 'sm', color: 'secondary' })` instead of manually composing every Tailwind class.
- `slots` support multi-part components, letting one variant definition return class builders for parts such as `base`, `avatar`, `wrapper`, labels, and content regions.
- `class` / `className` overrides make local escape hatches explicit without abandoning the variant definition.
- `extend` supports component composition by merging classes, slots, variants, default variants, and compound variants from another component.
- TypeScript support provides autocomplete for slots, values, and breakpoints.
- It is framework-agnostic, not React-specific.
- It can use `tailwind-merge` for automatic Tailwind class conflict resolution; from v2 onward, `tailwind-merge` is an optional peer dependency.
- The docs position Tailwind Variants as inspired by Stitches and CVA, with Tailwind CSS v4 support covered in the docs.

## Example Pattern

```tsx
const button = tv({
  base: 'font-medium rounded-full active:opacity-80',
  variants: {
    color: {
      primary: 'bg-blue-500 text-white',
      secondary: 'bg-purple-500 text-white'
    },
    size: {
      sm: 'text-sm',
      md: 'text-base',
      lg: 'px-4 py-3 text-lg'
    }
  },
  compoundVariants: [{ size: ['sm', 'md'], class: 'px-3 py-1' }],
  defaultVariants: { size: 'md', color: 'primary' }
});
```

## Sources

- [Tailwind Variants introduction](https://www.tailwind-variants.org/docs/introduction)

## Related

- [Resources](../../README.md)
