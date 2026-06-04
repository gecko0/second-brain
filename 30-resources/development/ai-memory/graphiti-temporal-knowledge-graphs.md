# Graphiti Temporal Knowledge Graphs

## Summary

Graphiti is an open-source framework for building and querying temporal context graphs for AI agents.

## Key Points

- [getzep/graphiti](https://github.com/getzep/graphiti) builds real-time knowledge graphs that track entities, facts, relationships, provenance, and how facts change over time.
- It is designed for agent memory and dynamic context retrieval, not static document-only RAG.
- Core concepts include entities, temporal relationship facts with validity windows, episodes as source/provenance records, and custom ontology via Pydantic models.
- Retrieval combines semantic search, keyword/BM25 search, and graph traversal for richer context than flat chunks or raw chat history.
- Useful capabilities to inspect: incremental graph construction, temporal fact invalidation, hybrid retrieval, custom entity/edge types, source provenance, and historical queries.
- The repo includes an MCP server so Claude, Cursor, and other MCP clients can use Graphiti-backed memory.
- Requirements include Python 3.10+, a graph backend such as Neo4j, FalkorDB, Kuzu, or Amazon Neptune, and an LLM provider. Graphiti defaults to OpenAI for inference and embeddings.
- Graphiti is the open-source engine behind Zep's temporal context graph infrastructure; Zep is the managed/production platform.

## Sources

- [getzep/graphiti on GitHub](https://github.com/getzep/graphiti)
- [Zep](https://www.getzep.com/)

## Related

- [AI SDK Tools](../ai-sdk/ai-sdk-tools.md)
- [Sim AI Agent Platform](../ai-agent-platforms/sim-ai-agent-platform.md)
- [Agent Skills](../../ai/skills/agent-skills.md)
- [Resources](../../README.md)
