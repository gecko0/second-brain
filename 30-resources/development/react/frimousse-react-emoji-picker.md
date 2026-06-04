# Frimousse React Emoji Picker

## Summary

Frimousse is a lightweight, unstyled, composable emoji picker for React. Captured because the project appears unmaintained, but the community is adding useful extensions, including custom emoji support.

## Key Points

- [liveblocks/frimousse](https://github.com/liveblocks/frimousse) provides a React emoji picker that is dependency-free, tree-shakable, virtualized, accessible, and intended to be styled by the consuming app.
- It supports React 18 and 19, TypeScript 5.1+, npm installation via `frimousse`, and a pre-built `shadcn/ui` component install path.
- [Issue #5](https://github.com/liveblocks/frimousse/issues/5) requests custom emojis, similar to Slack or Discord.
- [The linked issue comment](https://github.com/liveblocks/frimousse/issues/5#issuecomment-4337508650) says Glue has been using a customized Frimousse implementation in production and points to [PR #32](https://github.com/liveblocks/frimousse/pull/32).
- [PR #32](https://github.com/liveblocks/frimousse/pull/32), titled `feat: add custom emoji category support`, was open as of 2026-06-02 and adds opt-in custom emoji categories, frequently-used emojis, unified search, custom emoji types, search scoring, and documentation.
- Treat the custom emoji extension as community work until merged upstream. For production use, expect to evaluate the fork/PR directly or carry a patch.

## Sources

- [liveblocks/frimousse on GitHub](https://github.com/liveblocks/frimousse)
- [Support custom emojis issue #5](https://github.com/liveblocks/frimousse/issues/5)
- [Issue comment about Glue production use](https://github.com/liveblocks/frimousse/issues/5#issuecomment-4337508650)
- [Custom emoji support PR #32](https://github.com/liveblocks/frimousse/pull/32)

## Related

- [Icon Libraries](../../design/icon-libraries.md)
- [Resources](../../README.md)
