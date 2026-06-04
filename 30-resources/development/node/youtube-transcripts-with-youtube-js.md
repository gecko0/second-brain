# YouTube Transcripts With YouTube.js

## Summary

YouTube.js is a JavaScript client for YouTube's internal InnerTube API. It can be used from Node.js to inspect videos and attempt transcript/caption extraction, but recent YouTube bot-guarding makes server-side transcript fetching unreliable from non-residential IP addresses.

## Key Points

- [LuanRT/YouTube.js](https://github.com/LuanRT/YouTube.js) is the source repository for `youtubei.js`, a JavaScript/TypeScript client for YouTube's internal API.
- The library works in Node.js, Deno, modern browsers, and other runtimes, but it is unofficial and depends on YouTube internals.
- [Issue #1102](https://github.com/LuanRT/YouTube.js/issues/1102) tracks `info.getTranscript()` failing with HTTP 400 against `youtubei/v1/get_transcript` when called from a Node.js server.
- The issue discussion attributes the failure to YouTube bot detection / transcript API guarding. The practical consequence is that transcript extraction is not reliable from typical server, cloud, CI, or other non-residential IP addresses.
- Reported workarounds include using caption tracks instead of the transcript API, fetching timedtext XML from caption `base_url`, setting `generate_session_locally: true`, disabling cache with `new UniversalCache(false)`, using proxy-aware `fetch` / `undici`, and routing through residential proxies.
- Treat all workarounds as fragile. Captions may include accessibility context such as music or laughter markers, may differ from transcripts, and may still be rate-limited or blocked.
- For product designs, avoid depending on backend-only YouTube transcript extraction unless residential egress, user-side/browser capture, a third-party transcript provider, or an alternate transcription pipeline is acceptable.

## Sources

- [LuanRT/YouTube.js on GitHub](https://github.com/LuanRT/YouTube.js)
- [Issue #1102: getTranscript status 400](https://github.com/LuanRT/YouTube.js/issues/1102)

## Related

- [Resources](../../README.md)
