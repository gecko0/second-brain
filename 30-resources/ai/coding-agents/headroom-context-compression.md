# Headroom Context Compression

## Summary

Headroom is a context-compression layer for AI agents that reduces tokens from tool outputs, logs, RAG chunks, files, and conversation history before they reach the LLM.

## Key Points

- [chopratejas/headroom](https://github.com/chopratejas/headroom) provides library, proxy, agent wrapper, MCP server, and cross-agent memory surfaces for compressing agent context.
- The project positions itself around 60-95% fewer tokens while preserving the ability to retrieve original content when needed.
- Main usage modes include Python and TypeScript libraries, `headroom proxy`, `headroom wrap claude|codex|cursor|aider|copilot`, and MCP tools such as `headroom_compress`, `headroom_retrieve`, and `headroom_stats`.
- Compression routes by content type, including JSON, code/AST, and prose, with cached originals available through reversible retrieval.
- It also includes `headroom learn`, which can mine failed sessions and write corrections to agent instruction files such as `CLAUDE.md` or `AGENTS.md`.
- Useful to evaluate for long-running coding-agent work, noisy tool output, codebase exploration, RAG pipelines, and reducing context/output token costs.

## Sources

- [chopratejas/headroom on GitHub](https://github.com/chopratejas/headroom)
- [Headroom documentation](https://headroom-docs.vercel.app/)

## Related

- [Claude Code Leak Repo](claude-code-leak-repo.md)
- [Agent Skills](../skills/agent-skills.md)
- [Fallow Codebase Intelligence](../../development/fallow-codebase-intelligence.md)
- [Resources](../../README.md)
