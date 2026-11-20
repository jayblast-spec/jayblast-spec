# Michael Ogunleye

**Founder of [ArkNet Digital](https://arknet.digital).** I build developer tools, AI-agent infrastructure and security tooling: small, well-tested TypeScript libraries that catch the failures ordinary unit tests miss, published on npm with CI and docs.

## What I work on

- **AI agents and MCP:** protocol conformance testing, version bridging, and governance primitives for multi-agent systems.
- **CI safety nets:** tools that run in a pipeline and fail the build before a silent breaking change reaches production (LLM gateways, database migrations, WebAssembly interfaces, embedding models).
- **Local-first and CRDT tooling:** debugging and convergence checks for Automerge and Yjs.
- **Product delivery:** taking an idea from spec to a shipped, documented product for clients through ArkNet Digital.

## Selected projects

| Project | What it does | Links |
|---|---|---|
| [agora](https://github.com/jayblast-spec/agora) | Propose, vote, veto and quorum primitives for multi-agent systems, layered on MCP and A2A without changing either spec. | [Docs](https://jayblast-spec.github.io/agora/) · [npm](https://www.npmjs.com/package/agora-protocol) |
| [gatewayproof](https://github.com/jayblast-spec/gatewayproof) | Conformance test suite for OpenAI-compatible LLM gateways: streaming, usage, cost, concurrency and error handling. | [Docs](https://jayblast-spec.github.io/gatewayproof/) · [npm](https://www.npmjs.com/package/gatewayproof) |
| [mcp-conform](https://github.com/jayblast-spec/mcp-conform) + [mcp-registry](https://github.com/jayblast-spec/mcp-registry) | Runs a real MCP client against a server and checks it against the spec; the registry publishes daily conformance badges. | [Registry](https://jayblast-spec.github.io/mcp-registry/) |
| [mcp-versionbridge](https://github.com/jayblast-spec/mcp-versionbridge) | Lets an MCP client on the older `initialize` handshake talk to a 2026-07-28 MCP server with no changes to either side. | [Docs](https://jayblast-spec.github.io/mcp-versionbridge/) · [npm](https://www.npmjs.com/package/mcp-versionbridge) |
| [pglite-diff](https://github.com/jayblast-spec/pglite-diff) | Diffs query results of two SQL setups on isolated in-memory Postgres so migration regressions fail CI. | [Docs](https://jayblast-spec.github.io/pglite-diff/) · [npm](https://www.npmjs.com/package/pglite-diff) |
| [wit-breaking](https://github.com/jayblast-spec/wit-breaking) | Detects breaking changes between two WebAssembly Component Model WIT interfaces, like `buf breaking` for WIT. | [Docs](https://jayblast-spec.github.io/wit-breaking/) · [npm](https://www.npmjs.com/package/wit-breaking) |
| [embedguard](https://github.com/jayblast-spec/embedguard) | Catches silent embedding-model swaps under a vector index with dimension checks and canary-probe drift detection. | [Docs](https://jayblast-spec.github.io/embedguard/) · [npm](https://www.npmjs.com/package/embedguard) |
| [automerge-lens](https://github.com/jayblast-spec/automerge-lens) · [yjs-lens](https://github.com/jayblast-spec/yjs-lens) | Explain CRDT merge outcomes and fuzz update order to catch convergence violations in Automerge and Yjs. | [npm](https://www.npmjs.com/package/automerge-lens) · [npm](https://www.npmjs.com/package/yjs-lens) |

**Stack:** TypeScript, Node.js, Next.js, React, Postgres and Supabase, Vercel, GitHub Actions.

## Contact

- Website: [arknet.digital](https://arknet.digital)
- LinkedIn: [Michael O. Ogunleye](https://www.linkedin.com/in/michael-o-ogunleye-997938371)
