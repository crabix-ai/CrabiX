# Product Overview

CrabiX is a local-first AI router and AI workspace for developers.

It gives AI tools one stable local endpoint:

```text
http://localhost:3721/v1
```

Instead of reconfiguring every tool when a provider hits limits or becomes slow, the user connects providers and local models to CrabiX once. Cursor, VS Code, Continue, Claude Code, Codex, Cline, OpenCode, custom scripts, and local model workflows can then use the same endpoint.

The public provider/tool catalog is described as 250+ providers and coding tools. Users connect only the providers, subscriptions, API keys, and local runtimes they own.

## Principles

- Local-first control plane.
- User-owned providers and API keys.
- No token markup.
- One endpoint for many tools.
- Transparent routing, fallback, usage, and provider health.
- Workspace and agent workflows on the same backend.
- Platform availability follows the public stable release feed; do not infer unpublished artifacts.

## Product Layers

| Layer | Summary |
| --- | --- |
| Provider Router | Routes AI requests across user-owned providers, accounts, local models, and combo models with 13 routing strategies. |
| Dashboard | Shows status, latency, usage, provider availability, and routing policy. |
| AI Workspace | Combines chat, projects, terminal, browser preview, Git, files, design context, MCP, Skills, plugins, voice, and agents. |
| `crabix launch` | Starts 15 supported coding-tool integrations through CrabiX-managed gateway configuration. |
| MCP, Skills, Plugins | Adds tools, reusable instructions, installable capability bundles, and expanded MCP config/import capacity on Pro. |
| CLI / Service Mode | Runs CrabiX as a headless gateway and agent runtime. |
| AI Corp | Models AI-first companies with teams, employees, goals, issues, routines, approvals, budgets, and activity. |
| CrabiX Link | Connects trusted devices through scoped pairing. |

## Audience

CrabiX is built for senior developers, staff engineers, indie builders, AI operators, and tech leads who use multiple AI tools and providers daily.

Common pain:

- Several AI subscriptions, but no unified control plane.
- Manual switching when Claude, Codex, Gemini, OpenRouter, Ollama, or another provider hits limits.
- Too many tool configs across IDEs, CLIs, agents, MCP servers, and scripts.
- Need for local privacy boundaries and auditable routing.

## Pricing

| Plan | Price | Includes |
| --- | --- | --- |
| Free | `$0` | Core routing, localhost endpoint, Smart + RoundRobin, chat/workspace basics, dashboard, basic agent runtime, basic MCP with up to 2 live sessions. |
| Pro | `$19/month` | All 13 routing strategies, combo models, expanded MCP config/imports, Skills, plugins, background agents, subagents, AI Corp automation, `crabix launch`, Git/design/preview workflows, extended stats, voice, CrabiX Link. |

CrabiX does not add token markup. Users pay model providers directly.

Paid purchases are handled by Paddle as merchant of record. Eligible first Pro purchases have a 14-day refund window as described at [crabix.ai/refund](https://crabix.ai/refund).

## Availability And Downloads

CrabiX's first public early release is live. Signed desktop builds are served through [crabix.ai/download](https://crabix.ai/download) when platform artifacts are present in the stable release channel.

Use [release-feed.json](https://crabix.ai/release-feed.json) for current stable-channel version, platform availability, artifact URLs, signatures, and checksums. Do not invent missing artifacts or release metadata.

## Comparisons

- LiteLLM is strongest as a mature server-side Python proxy. CrabiX is strongest as a desktop-first local control plane and workspace.
- OpenRouter is a hosted API marketplace. CrabiX is a local-first router for user-owned providers and local models; OpenRouter can be one provider inside CrabiX.
- Ollama is a local model runtime. CrabiX coordinates Ollama plus cloud providers, routing policy, dashboard, workspace, agents, and tool integrations.
