# Product Overview

CrabiX is a local-first AI router and AI workspace for developers.

It gives AI tools one stable local endpoint:

```text
http://localhost:3721/v1
```

Instead of reconfiguring every tool when a provider hits limits or becomes slow, the user connects providers and local models to CrabiX once. Cursor, VS Code, Continue, Claude Code, Codex, Cline, OpenCode, custom scripts, and local model workflows can then use the same endpoint.

## Principles

- Local-first control plane.
- User-owned providers and API keys.
- No token markup.
- One endpoint for many tools.
- Transparent routing, fallback, usage, and provider health.
- Workspace and agent workflows on the same backend.

## Product Layers

| Layer | Summary |
| --- | --- |
| Provider Router | Routes AI requests across user-owned providers, accounts, local models, and combo models. |
| Dashboard | Shows status, latency, usage, provider availability, and routing policy. |
| AI Workspace | Combines chat, projects, terminal, browser preview, Git, files, design context, MCP, Skills, plugins, voice, and agents. |
| `crabix launch` | Starts supported coding tools through CrabiX-managed gateway configuration. |
| MCP, Skills, Plugins | Adds tools, reusable instructions, and installable capability bundles. |
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
| Free | `$0` | Core routing, localhost endpoint, Smart + RoundRobin, chat/workspace basics, dashboard, basic agent runtime, basic MCP. |
| Pro | `$19/month` | All routing strategies, combo models, unlimited MCP, Skills, plugins, background agents, AI Corp automation, `crabix launch`, Git/design/preview workflows, voice, CrabiX Link. |

CrabiX does not add token markup. Users pay model providers directly.

## Comparisons

- LiteLLM is strongest as a mature server-side Python proxy. CrabiX is strongest as a desktop-first local control plane and workspace.
- OpenRouter is a hosted API marketplace. CrabiX is a local-first router for user-owned providers and local models; OpenRouter can be one provider inside CrabiX.
- Ollama is a local model runtime. CrabiX coordinates Ollama plus cloud providers, routing policy, dashboard, workspace, agents, and tool integrations.
