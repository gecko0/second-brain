# Type-Safe Errors With neverthrow

## Summary

neverthrow is a TypeScript/JavaScript library for modeling failures explicitly with `Result` and `ResultAsync` instead of unchecked exceptions.

## Key Points

- [supermacro/neverthrow](https://github.com/supermacro/neverthrow) provides type-safe error handling for JavaScript and TypeScript.
- Core types are `Result<T, E>`, `Ok`, and `Err`, representing successful and failed computations.
- `ResultAsync<T, E>` wraps `Promise<Result<T, E>>` so asynchronous operations can be composed with the same style as synchronous results.
- Useful APIs include `ok`, `err`, `okAsync`, `errAsync`, `map`, `mapErr`, `andThen`, `orElse`, `match`, `unwrapOr`, `fromThrowable`, `fromPromise`, `fromSafePromise`, and `safeTry`.
- The project recommends `eslint-plugin-neverthrow` to force explicit result consumption through methods such as `.match`, `.unwrapOr`, or unsafe unwraps.
- Useful when a codebase wants Rust-style error handling, explicit domain errors, composable validation/parsing flows, or fewer hidden `throw` paths in service code.
- License: MIT.

## Sources

- [supermacro/neverthrow on GitHub](https://github.com/supermacro/neverthrow)
- [neverthrow wiki](https://github.com/supermacro/neverthrow/wiki)
- [eslint-plugin-neverthrow](https://github.com/mdbetancourt/eslint-plugin-neverthrow)

## Related

- [YouTube Transcripts With YouTube.js](../node/youtube-transcripts-with-youtube-js.md)
- [Resources](../../README.md)
