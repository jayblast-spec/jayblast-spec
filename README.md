<div align="center">

<img alt="Michael, Founder, ArkNet Digital" src="https://capsule-render.vercel.app/api?type=waving&color=0:020617,55:0B1E3D,100:1D4ED8&height=200&section=header&text=Michael%20Ogunleye&fontSize=52&fontColor=FFFFFF&fontAlignY=36&desc=Founder%2C%20ArkNet%20Digital&descSize=20&descAlignY=58&animation=fadeIn" width="100%">

## Michael · Founder, ArkNet Digital

**Developer tools · AI-agent infrastructure · MCP tooling · Security tooling**

<img alt="Developer tools, AI-agent infrastructure, MCP tooling, security tooling" src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=19&duration=2800&pause=700&color=38BDF8&center=true&vCenter=true&width=820&lines=Developer+tools+that+catch+silent+breakage+in+CI;AI-agent+infrastructure+%C2%B7+MCP+tooling+%C2%B7+security+tooling;8+open-source+libraries+on+npm%2C+tested+against+the+real+thing;Real+problem+%E2%86%92+narrow+wedge+%E2%86%92+shipped+and+measured">

<p>
  <a href="https://arknet.digital"><img alt="arknet.digital" src="https://img.shields.io/badge/arknet.digital-Website-1D4ED8?style=for-the-badge&logo=googlechrome&logoColor=white"></a>
  <a href="https://www.linkedin.com/in/michael-o-ogunleye-997938371"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-Michael%20O.%20Ogunleye-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"></a>
  <a href="mailto:michael@arknet.digital"><img alt="Email" src="https://img.shields.io/badge/Email-michael%40arknet.digital-0EA5E9?style=for-the-badge&logo=gmail&logoColor=white"></a>
</p>

<p>
  <img alt="Open-source libraries" src="https://img.shields.io/badge/open--source%20libraries-8%20on%20npm-020617?style=flat-square&logo=npm&logoColor=CB3837">
  <img alt="Live products" src="https://img.shields.io/badge/live%20products-6-020617?style=flat-square&logo=vercel&logoColor=white">
  <img alt="Focus" src="https://img.shields.io/badge/focus-agents%20%C2%B7%20MCP%20%C2%B7%20CI%20safety%20%C2%B7%20security-020617?style=flat-square">
  <img alt="Profile views" src="https://komarev.com/ghpvc/?username=jayblast-spec&style=flat-square&color=1D4ED8&label=profile%20views">
</p>

</div>

> 🔨 **Currently building:** [OwnEnvoy](https://ownenvoy-two.vercel.app), an authority and consent layer for voice agents, and the next releases of the MCP tooling below.

## 🧭 The Thesis

Complex systems rarely fail because of one missing feature. They fail at the intersections: strategy and execution, speed and security, intelligence and governance, growth and resilience.

> **How should critical systems be designed for a world defined by greater technological complexity, interconnected risk, and uncertainty?**

I treat product strategy, architecture, security, data, interface and deployment as one connected problem. The operating principle is simple: **evidence over ambition.** Ideas become working systems as early as possible. They are deployed, tested against real behavior, improved when the evidence supports it, and retired when it doesn't.

## 📊 At a Glance

| Signal | Current surface |
|---|---|
| Open-source libraries | **8** TypeScript packages on npm, each with CI, a test suite and docs |
| MCP tooling | A conformance suite ([mcp-conform](https://github.com/jayblast-spec/mcp-conform)), a live badge registry ([mcp-registry](https://jayblast-spec.github.io/mcp-registry/)) and a version bridge |
| Live products | [Negotiator](https://ainegotiator.digital), [OwnEnvoy](https://ownenvoy-two.vercel.app), [BE PRESIDENT](https://powerfulseat.online), [GrantScout](https://grant-scout-jayblast.vercel.app), [ExposureWatch](https://exposurewatch-sigma.vercel.app), [SmartInvite](https://smartinvite.vercel.app) |
| Core domains | AI agents, developer tooling, security, founder infrastructure, simulation |
| Architecture | TypeScript, Node.js, Next.js, Tailwind CSS, Supabase Postgres with explicit row-level security, Vercel |

## 🛠️ Open-Source Infrastructure

The process mattered more than the output. Before writing a line of any of these, I tested candidate ideas against the ecosystem that already exists: I searched for prior art, read the alternatives, and killed the idea if the gap wasn't real. Inside pure AI-agent tooling, seventeen candidates went through that filter and fifteen were already solved well by something shipping. Widening the search into adjacent infrastructure (CRDTs, the WebAssembly Component Model, vector databases, Postgres tooling) produced the eight below. Each one fills a specific missing capability with a source I can point to: a cited paper, a spec changelog, or an existing tool's stated non-goals.

These are libraries and CLIs other developers install and build on, not UI products. Every one ships with a test suite run against the real underlying library or protocol rather than mocks, plus CI and documentation.

<table>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/jayblast-spec/agora">agora</a></h3>
      <p><b>Governance for multi-agent systems</b></p>
      <p>Propose, vote, veto and quorum primitives layered on MCP and A2A without changing either spec. Fills the governance gap documented in <a href="https://arxiv.org/abs/2606.31498">arXiv:2606.31498</a>.</p>
      <a href="https://www.npmjs.com/package/agora-protocol"><img alt="npm agora-protocol" src="https://img.shields.io/npm/v/agora-protocol?style=flat-square&color=1D4ED8&label=npm"></a>
      <a href="https://github.com/jayblast-spec/agora/actions/workflows/ci.yml"><img alt="CI" src="https://img.shields.io/github/actions/workflow/status/jayblast-spec/agora/ci.yml?branch=main&style=flat-square&label=CI"></a>
      <img alt="MIT" src="https://img.shields.io/badge/license-MIT-0B1E3D?style=flat-square">
      <p><a href="https://github.com/jayblast-spec/agora">Source</a> · <a href="https://jayblast-spec.github.io/agora/">Docs</a> · <a href="https://www.npmjs.com/package/agora-protocol">npm</a></p>
    </td>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/jayblast-spec/gatewayproof">gatewayproof</a></h3>
      <p><b>Conformance suite for LLM gateways</b></p>
      <p>Catches the streaming, usage, cost, concurrency and error-propagation bugs in OpenAI-compatible gateways that an eyeball review of a diff won't.</p>
      <a href="https://www.npmjs.com/package/gatewayproof"><img alt="npm gatewayproof" src="https://img.shields.io/npm/v/gatewayproof?style=flat-square&color=1D4ED8&label=npm"></a>
      <a href="https://github.com/jayblast-spec/gatewayproof/actions/workflows/ci.yml"><img alt="CI" src="https://img.shields.io/github/actions/workflow/status/jayblast-spec/gatewayproof/ci.yml?branch=main&style=flat-square&label=CI"></a>
      <img alt="MIT" src="https://img.shields.io/badge/license-MIT-0B1E3D?style=flat-square">
      <p><a href="https://github.com/jayblast-spec/gatewayproof">Source</a> · <a href="https://jayblast-spec.github.io/gatewayproof/">Docs</a> · <a href="https://www.npmjs.com/package/gatewayproof">npm</a></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/jayblast-spec/mcp-versionbridge">mcp-versionbridge</a></h3>
      <p><b>Compatibility bridge for MCP</b></p>
      <p>Lets a client on the pre-2026-07-28 <code>initialize</code> handshake talk to a 2026-07-28 MCP server, with no changes to either side.</p>
      <a href="https://www.npmjs.com/package/mcp-versionbridge"><img alt="npm mcp-versionbridge" src="https://img.shields.io/npm/v/mcp-versionbridge?style=flat-square&color=1D4ED8&label=npm"></a>
      <a href="https://github.com/jayblast-spec/mcp-versionbridge/actions/workflows/ci.yml"><img alt="CI" src="https://img.shields.io/github/actions/workflow/status/jayblast-spec/mcp-versionbridge/ci.yml?branch=main&style=flat-square&label=CI"></a>
      <img alt="MIT" src="https://img.shields.io/badge/license-MIT-0B1E3D?style=flat-square">
      <p><a href="https://github.com/jayblast-spec/mcp-versionbridge">Source</a> · <a href="https://jayblast-spec.github.io/mcp-versionbridge/">Docs</a> · <a href="https://www.npmjs.com/package/mcp-versionbridge">npm</a></p>
    </td>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/jayblast-spec/pglite-diff">pglite-diff</a></h3>
      <p><b>Migration regression testing</b></p>
      <p>Diffs two migration paths' query results on real Postgres-in-WASM, so regressions fail CI before they touch production. Ships as a GitHub Action.</p>
      <a href="https://www.npmjs.com/package/pglite-diff"><img alt="npm pglite-diff" src="https://img.shields.io/npm/v/pglite-diff?style=flat-square&color=1D4ED8&label=npm"></a>
      <a href="https://github.com/jayblast-spec/pglite-diff/actions/workflows/ci.yml"><img alt="CI" src="https://img.shields.io/github/actions/workflow/status/jayblast-spec/pglite-diff/ci.yml?branch=main&style=flat-square&label=CI"></a>
      <img alt="MIT" src="https://img.shields.io/badge/license-MIT-0B1E3D?style=flat-square">
      <p><a href="https://github.com/jayblast-spec/pglite-diff">Source</a> · <a href="https://jayblast-spec.github.io/pglite-diff/">Docs</a> · <a href="https://www.npmjs.com/package/pglite-diff">npm</a></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/jayblast-spec/wit-breaking">wit-breaking</a></h3>
      <p><b><code>buf breaking</code> for WebAssembly</b></p>
      <p>Classifies changes between two WebAssembly Component Model WIT interfaces as breaking or safe. Ships as a GitHub Action.</p>
      <a href="https://www.npmjs.com/package/wit-breaking"><img alt="npm wit-breaking" src="https://img.shields.io/npm/v/wit-breaking?style=flat-square&color=1D4ED8&label=npm"></a>
      <a href="https://github.com/jayblast-spec/wit-breaking/actions/workflows/ci.yml"><img alt="CI" src="https://img.shields.io/github/actions/workflow/status/jayblast-spec/wit-breaking/ci.yml?branch=main&style=flat-square&label=CI"></a>
      <img alt="MIT" src="https://img.shields.io/badge/license-MIT-0B1E3D?style=flat-square">
      <p><a href="https://github.com/jayblast-spec/wit-breaking">Source</a> · <a href="https://jayblast-spec.github.io/wit-breaking/">Docs</a> · <a href="https://www.npmjs.com/package/wit-breaking">npm</a></p>
    </td>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/jayblast-spec/embedguard">embedguard</a></h3>
      <p><b>Embedding-model swap guard</b></p>
      <p>Catches a silent embedding-model swap under a vector index, with dimension checks and canary-probe drift detection, before it corrupts similarity search.</p>
      <a href="https://www.npmjs.com/package/embedguard"><img alt="npm embedguard" src="https://img.shields.io/npm/v/embedguard?style=flat-square&color=1D4ED8&label=npm"></a>
      <a href="https://github.com/jayblast-spec/embedguard/actions/workflows/ci.yml"><img alt="CI" src="https://img.shields.io/github/actions/workflow/status/jayblast-spec/embedguard/ci.yml?branch=main&style=flat-square&label=CI"></a>
      <img alt="MIT" src="https://img.shields.io/badge/license-MIT-0B1E3D?style=flat-square">
      <p><a href="https://github.com/jayblast-spec/embedguard">Source</a> · <a href="https://jayblast-spec.github.io/embedguard/">Docs</a> · <a href="https://www.npmjs.com/package/embedguard">npm</a></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/jayblast-spec/automerge-lens">automerge-lens</a></h3>
      <p><b>CRDT debugging for Automerge</b></p>
      <p>Explains why an Automerge merge resolved the way it did, and fuzzes application order to catch convergence violations.</p>
      <a href="https://www.npmjs.com/package/automerge-lens"><img alt="npm automerge-lens" src="https://img.shields.io/npm/v/automerge-lens?style=flat-square&color=1D4ED8&label=npm"></a>
      <a href="https://github.com/jayblast-spec/automerge-lens/actions/workflows/ci.yml"><img alt="CI" src="https://img.shields.io/github/actions/workflow/status/jayblast-spec/automerge-lens/ci.yml?branch=main&style=flat-square&label=CI"></a>
      <img alt="MIT" src="https://img.shields.io/badge/license-MIT-0B1E3D?style=flat-square">
      <p><a href="https://github.com/jayblast-spec/automerge-lens">Source</a> · <a href="https://www.npmjs.com/package/automerge-lens">npm</a></p>
    </td>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/jayblast-spec/yjs-lens">yjs-lens</a></h3>
      <p><b>Convergence checks for Yjs</b></p>
      <p>Verifies the convergence guarantee holds for a set of Yjs updates (the CRDT behind Tiptap, BlockNote and Jupyter collaboration) and summarizes causal history.</p>
      <a href="https://www.npmjs.com/package/yjs-lens"><img alt="npm yjs-lens" src="https://img.shields.io/npm/v/yjs-lens?style=flat-square&color=1D4ED8&label=npm"></a>
      <a href="https://github.com/jayblast-spec/yjs-lens/actions/workflows/ci.yml"><img alt="CI" src="https://img.shields.io/github/actions/workflow/status/jayblast-spec/yjs-lens/ci.yml?branch=main&style=flat-square&label=CI"></a>
      <img alt="MIT" src="https://img.shields.io/badge/license-MIT-0B1E3D?style=flat-square">
      <p><a href="https://github.com/jayblast-spec/yjs-lens">Source</a> · <a href="https://www.npmjs.com/package/yjs-lens">npm</a></p>
    </td>
  </tr>
</table>

### MCP conformance suite

| Project | What it does | Links |
|---|---|---|
| [mcp-conform](https://github.com/jayblast-spec/mcp-conform) | Runs a real MCP client against a server over stdio or Streamable HTTP and checks it against the Model Context Protocol spec. | [![CI](https://img.shields.io/github/actions/workflow/status/jayblast-spec/mcp-conform/test.yml?branch=master&style=flat-square&label=CI)](https://github.com/jayblast-spec/mcp-conform/actions/workflows/test.yml) |
| [mcp-registry](https://github.com/jayblast-spec/mcp-registry) | A public registry of MCP servers, tested daily with mcp-conform, that publishes live conformance badges. | [Registry](https://jayblast-spec.github.io/mcp-registry/) · [![Registry](https://img.shields.io/github/actions/workflow/status/jayblast-spec/mcp-registry/registry.yml?branch=master&style=flat-square&label=daily%20run)](https://github.com/jayblast-spec/mcp-registry/actions/workflows/registry.yml) |

## 📚 Research and Specs I Build On

Each tool starts from a documented gap. These are the sources behind the most important ones. I'm not an author of them; I build on them.

| Source | What it showed | What I built |
|---|---|---|
| [*Governance Gaps in Agent Interoperability Protocols: What MCP, A2A, and ACP Cannot Express*](https://arxiv.org/abs/2606.31498) (arXiv:2606.31498) | No major agent protocol can express propose, vote, veto or quorum | [agora](https://github.com/jayblast-spec/agora) |
| [Model Context Protocol specification](https://modelcontextprotocol.io) | The 2026-07-28 revision replaced the old `initialize` handshake | [mcp-versionbridge](https://github.com/jayblast-spec/mcp-versionbridge), [mcp-conform](https://github.com/jayblast-spec/mcp-conform) |
| [WebAssembly Component Model](https://component-model.bytecodealliance.org) | WIT interfaces had no breaking-change checker like `buf breaking` or `oasdiff` | [wit-breaking](https://github.com/jayblast-spec/wit-breaking) |
| [A2A protocol](https://a2a-protocol.org) | Agent-to-agent messaging with no shared deliberation primitives | [agora](https://github.com/jayblast-spec/agora) A2A adapter |

## 🚀 Live Products

<table>
  <tr>
    <td width="33%" valign="top">
      <h4><a href="https://ainegotiator.digital">Negotiator</a></h4>
      <p>Cheapest-price finder that ranks seller quotes for a product, with comparisons run in an isolated sandbox.</p>
      <a href="https://ainegotiator.digital"><img alt="Live" src="https://img.shields.io/badge/live-ainegotiator.digital-22C55E?style=flat-square"></a>
    </td>
    <td width="33%" valign="top">
      <h4><a href="https://ownenvoy-two.vercel.app">OwnEnvoy</a></h4>
      <p>Authority and consent for voice agents: governed mandates, consented voice sessions and verifiable receipts.</p>
      <a href="https://ownenvoy-two.vercel.app"><img alt="Live" src="https://img.shields.io/badge/live-OwnEnvoy-22C55E?style=flat-square"></a>
    </td>
    <td width="33%" valign="top">
      <h4><a href="https://powerfulseat.online">BE PRESIDENT</a></h4>
      <p>Global leadership and governance simulator.</p>
      <a href="https://powerfulseat.online"><img alt="Live" src="https://img.shields.io/badge/live-powerfulseat.online-22C55E?style=flat-square"></a>
    </td>
  </tr>
  <tr>
    <td width="33%" valign="top">
      <h4><a href="https://github.com/jayblast-spec/grant-scout">GrantScout</a></h4>
      <p>AI agent that finds real funding programs for solo, non-incorporated founders.</p>
      <a href="https://grant-scout-jayblast.vercel.app"><img alt="Live" src="https://img.shields.io/badge/live-GrantScout-22C55E?style=flat-square"></a>
    </td>
    <td width="33%" valign="top">
      <h4><a href="https://github.com/jayblast-spec/exposure-watch">ExposureWatch</a></h4>
      <p>Privacy-first check of whether an email or password has appeared in a known breach.</p>
      <a href="https://exposurewatch-sigma.vercel.app"><img alt="Live" src="https://img.shields.io/badge/live-ExposureWatch-22C55E?style=flat-square"></a>
    </td>
    <td width="33%" valign="top">
      <h4><a href="https://smartinvite.vercel.app">SmartInvite</a></h4>
      <p>Invitation and RSVP infrastructure.</p>
      <a href="https://smartinvite.vercel.app"><img alt="Live" src="https://img.shields.io/badge/live-SmartInvite-22C55E?style=flat-square"></a>
    </td>
  </tr>
</table>

**Hackathon agents (live):** [Brightkin Studio Director](https://brightkin-studio-director.vercel.app) ([source](https://github.com/jayblast-spec/brightkin-studio-director)), a Director and Compliance agent network on Google ADK and Gemini · [Publish Window Keeper](https://publish-window-keeper.vercel.app) ([source](https://github.com/jayblast-spec/publish-window-keeper)), cooldown and rate-limit math with Gemini reasoning.

<details>
<summary><b>📦 Earlier product builds (source available, archived)</b></summary>
<br>

| Area | Projects |
|---|---|
| AI and operational intelligence | [BriefOS](https://github.com/jayblast-spec/briefos) · [MeetingMind](https://github.com/jayblast-spec/meetingmind) · [OpsIntel](https://github.com/jayblast-spec/opsintel) · [Orbit](https://github.com/jayblast-spec/orbit) |
| Founder and business infrastructure | [FounderSignal](https://github.com/jayblast-spec/FounderSignal) · [PitchReady](https://github.com/jayblast-spec/pitchready) · [Startup Doc Generator](https://github.com/jayblast-spec/startup-doc-generator) · [InvoiceKit](https://github.com/jayblast-spec/invoicekit) · [RoleForge](https://github.com/jayblast-spec/roleforge) |
| Security and trust | [AgentProof](https://github.com/jayblast-spec/agentproof) · [ContractLens](https://github.com/jayblast-spec/contractlens) · [ThreatPulse](https://github.com/jayblast-spec/threatpulse) · [SafeLink](https://github.com/jayblast-spec/safelink) · [TrustSignal](https://github.com/jayblast-spec/trustsignal) · [BreachCost](https://github.com/jayblast-spec/breachcost) · [PortGuard](https://github.com/jayblast-spec/portguard) |
| Developer and data tools | [DevPulse](https://github.com/jayblast-spec/devpulse) · [SubnetPilot](https://github.com/jayblast-spec/subnetpilot) · [Africa Map](https://github.com/jayblast-spec/africa-map) |

</details>

## 🏛️ Architecture Principles

- **Systems first.** Product, data, security, interface and deployment are designed as one architecture.
- **Security by design.** Authentication and authorization fail closed; row-level security is explicit wherever Supabase is used.
- **Evidence before expansion.** A system earns further investment through verified behavior, not presentation.
- **Production over prototypes.** "Built" means local evidence. "Deployed" means the production surface has been checked against the promised behavior.
- **Operational clarity.** Loading, empty, error and recovery states are part of the product, not finishing work.
- **Claims require evidence.** No fabricated volume, SLA, benchmark, adoption or performance claims.
- **Secrets stay server-side.** Credentials belong in environment variables and secret managers, never in repositories, prompts or client code.

## 🧰 Some of My Building Stack

<p align="center">
  <img alt="Tech stack" src="https://skillicons.dev/icons?i=ts,js,python,nodejs,react,nextjs,tailwind,supabase,postgres,vercel,githubactions,git&theme=dark&perline=12">
</p>

| Layer | | Role |
|---|:---:|---|
| TypeScript / JavaScript | <img src="https://cdn.simpleicons.org/typescript/007ACC" width="24" alt="TypeScript"> | Libraries, product interfaces and services |
| Python | <img src="https://cdn.simpleicons.org/python/3776AB" width="24" alt="Python"> | Automation, data processing, integrations and AI workflows |
| Next.js / React | <img src="https://cdn.simpleicons.org/nextdotjs/9CA3AF" width="24" alt="Next.js"> | App shell, routing, server rendering and interactive interfaces |
| Node.js | <img src="https://cdn.simpleicons.org/nodedotjs/5FA04E" width="24" alt="Node.js"> | Serverless APIs, CLIs, backend services and automation |
| Supabase / PostgreSQL | <img src="https://cdn.simpleicons.org/supabase/3ECF8E" width="24" alt="Supabase"> | Data, auth, storage and explicit row-level security |
| MCP / A2A | <img src="https://cdn.simpleicons.org/modelcontextprotocol/9CA3AF" width="24" alt="Model Context Protocol"> | Agent protocols, conformance testing and adapters |
| WebAssembly | <img src="https://cdn.simpleicons.org/webassembly/654FF0" width="24" alt="WebAssembly"> | Component Model interfaces and Postgres-in-WASM testing |
| Vercel | <img src="https://cdn.simpleicons.org/vercel/9CA3AF" width="24" alt="Vercel"> | Deployment, serverless functions, cron and edge |
| Groq / OpenAI | <img src="https://www.google.com/s2/favicons?domain=groq.com&sz=64" width="24" alt="Groq"> | Fast inference, reasoning, structured generation and agent workflows |
| GitHub Actions | <img src="https://cdn.simpleicons.org/githubactions/2088FF" width="24" alt="GitHub Actions"> | CI, published Actions and delivery automation |

## ⚙️ Operating Discipline

```text
Observed problem
  -> System model
  -> Narrow testable intervention
  -> Smallest evidence-producing build
  -> Production deployment
  -> Measure behavior and failure modes
  -> Correct, expand, integrate, or retire
```

Technology does not manufacture demand. Architecture does not remove uncertainty. The discipline is to expose both to reality early enough to learn.

## 📈 GitHub Activity

<div align="center">

<img alt="GitHub stats" height="170" src="https://github-readme-stats.vercel.app/api?username=jayblast-spec&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=38BDF8&icon_color=1D4ED8&text_color=C9D1D9&custom_title=Michael%20Ogunleye%27s%20GitHub%20Stats">
<img alt="Top languages" height="170" src="https://github-readme-stats-navy.vercel.app/api/top-langs/?username=jayblast-spec&layout=compact&theme=dark&hide_border=true&bg_color=0D1117&title_color=38BDF8&text_color=C9D1D9">

<img alt="GitHub streak" src="https://streak-stats.demolab.com?user=jayblast-spec&theme=dark&hide_border=true&background=0D1117&ring=1D4ED8&fire=38BDF8&currStreakLabel=38BDF8">

<img alt="Contribution activity graph" width="100%" src="https://github-readme-activity-graph.vercel.app/graph?username=jayblast-spec&theme=tokyo-night&hide_border=true&bg_color=0D1117&color=38BDF8&line=1D4ED8&point=FFFFFF&area=true&custom_title=Michael%20Ogunleye%27s%20Contribution%20Graph">

<img alt="Trophies" src="https://github-trophies.vercel.app/?username=jayblast-spec&theme=algolia&no-frame=true&no-bg=true&margin-w=8&row=1&column=7">

<img alt="Contribution snake" width="100%" src="https://raw.githubusercontent.com/jayblast-spec/jayblast-spec/output/github-contribution-grid-snake-dark.svg">

</div>

## 🌍 ArkNet Digital

ArkNet Digital is the long-term systems initiative behind this work. Its scope extends beyond individual software products toward the convergence of **digital infrastructure, artificial intelligence, cybersecurity, continuity systems, distributed intelligence, energy, mobility and physical resilience**.

The central question is not how to react better after disruption. It is what should be built **before disruption makes the need obvious**.

[Explore ArkNet Digital →](https://arknet.digital)

## 📬 Contact

| Purpose | Where |
|---|---|
| ArkNet Digital | [arknet.digital](https://arknet.digital) |
| Professional profile | [LinkedIn: Michael O. Ogunleye](https://www.linkedin.com/in/michael-o-ogunleye-997938371) |
| Strategic, institutional or product correspondence | [michael@arknet.digital](mailto:michael@arknet.digital) |
| Repositories and shipped systems | [github.com/jayblast-spec](https://github.com/jayblast-spec?tab=repositories) |

<div align="center">

**Build for the system that exists. Architect for the one that is coming.**

<img alt="ArkNet Digital" src="https://capsule-render.vercel.app/api?type=waving&color=0:1D4ED8,55:0B1E3D,100:020617&height=120&section=footer&text=ArkNet%20Digital&fontSize=26&fontColor=FFFFFF&fontAlignY=70" width="100%">

</div>
