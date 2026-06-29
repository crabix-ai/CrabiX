# Product Overview

CrabiX is an AI OneApp: a cross-platform app for managing AI agents and AI-first companies. You set a task and how much freedom the agent gets, see every step in an execution trail, and approve, redirect, or stop the work.

Slogan: **Any model. Same agent. Your rules.**

Principle: pay for the app and the control plane, not for a markup on tokens. Models, providers, and data stay yours.

## Four Layers

| Layer | Summary |
| --- | --- |
| Agent management | One CrabiX agent on a full runtime: tools, background runs, subagents, queue and steer, execution trail. Autonomy levels L0 Observe to L4 Full Access; risky steps wait for approval. Every edit is a diff with Undo. |
| AI Corp | Teams of AI employees with goals, issues, routines, approvals, and budgets. Optional. |
| Workspace | Desktop, web, and CLI as thin clients over one local backend. Chats, projects, code, terminal, Git, Preview, Design, MCP, skills, plugins, and a signed marketplace. CrabiX Launch connects Claude Code, Codex, VS Code, Cline, OpenCode, and Continue. CrabiX Link opens the same workspace from a phone. |
| AI gateway | One endpoint at `http://localhost:21000/v1` with OpenAI, Anthropic, and Ollama compatible APIs across user-owned providers, subscriptions, API keys, and local models. 430+ providers in the catalog, 14 routing strategies, combo models, fallback, usage accounting. |

Local runtimes also cover on-device LLMs, speech (STT/TTS), and media generation on supported hardware.

## Autonomy Levels

| Level | Name | Meaning |
| --- | --- | --- |
| L0 | Observe | Read only. |
| L1 | Ask | Writes to the project; risky steps need approval. |
| L2 | Allowlist | Pre-approved actions run on their own, everything else asks. |
| L3 | Approve for me | A reviewer model checks each step against policy rules. |
| L4 | Full Access | No sandbox limits. |

Company, device, and temporary limits set ceilings; the lowest one wins.

## Audience

Developers and AI operators who use AI daily, hold several AI subscriptions and local models, and run coding tools such as Claude Code, Codex, Cursor, VS Code, Cline, or OpenCode. Their problem is control, not answer quality: what the agent may do, what it already did, who stops it, and what it cost.

## Pricing

One plan with everything included: `$21/month` or `$189/year`, after a 7-day free trial. No free tier, no tiers, no add-ons. After a trial without a subscription the app locks; local data stays on disk.

CrabiX adds no token markup. Users pay model providers directly. Paid purchases are handled by Paddle as merchant of record; refund terms are at [crabix.ai/refund](https://crabix.ai/refund).

## Availability

The first public release, 26.10.24, is live for macOS (Apple Silicon, Intel), Windows (x64, ARM64), and Linux (x86_64, ARM64; AppImage, `.deb`, `.rpm`). Use [release-feed.json](https://crabix.ai/release-feed.json) for current versions, artifacts, signatures, and checksums.

## Comparisons

- Cursor, Claude Code, and Codex bring their own model and bill. CrabiX is the layer above: one agent and one set of rules on whichever model the user already pays for, and CrabiX Launch can point those tools at the same providers.
- LiteLLM and OpenRouter are gateways. In CrabiX the gateway is the foundation, not the product; OpenRouter can be one provider inside it.
- Ollama is a local model runtime. CrabiX uses it as a provider under the same agent and rules.
