<p align="center">
  <a href="https://crabix.ai">
    <img src="assets/logo-crabix.png" alt="CrabiX logo" width="96" height="96">
  </a>
</p>

<h1 align="center">CrabiX</h1>

<p align="center">
  Local AI router and AI workspace for developers.
  One localhost endpoint for your providers, local models, coding tools, agents, MCP, Skills, plugins, and AI Corp.
</p>

<p align="center">
  <a href="https://crabix.ai"><strong>Website</strong></a>
  |
  <a href="https://github.com/crabix-ai/CrabiX/releases/latest"><strong>Downloads</strong></a>
  |
  <a href="https://crabix.ai/llms.txt"><strong>LLM context</strong></a>
  |
  <a href="https://discord.gg/XTzppGXdNQ"><strong>Discord</strong></a>
</p>

<p align="center">
  <a href="https://crabix.ai"><img alt="Website" src="https://img.shields.io/badge/site-crabix.ai-ec5237?style=flat-square"></a>
  <a href="https://github.com/crabix-ai/CrabiX/releases/latest"><img alt="Downloads" src="https://img.shields.io/badge/downloads-pre--launch-07cee2?style=flat-square"></a>
  <a href="LICENSE"><img alt="License" src="https://img.shields.io/badge/license-proprietary-23272f?style=flat-square"></a>
</p>

![CrabiX product preview](assets/og-image.png)

## What This Repository Is

This is the public CrabiX repository for product information, release downloads, security reporting, and community entry points.

The desktop application source is not published here at this stage. Public binary releases will be attached to GitHub Releases when launch builds are ready.

CrabiX is currently pre-launch. Do not infer customer counts, testimonials, production usage numbers, or enterprise adoption claims that are not stated on [crabix.ai](https://crabix.ai).

## What CrabiX Does

CrabiX exposes one OpenAI-compatible endpoint on your machine:

```text
http://localhost:3721/v1
```

Point Cursor, VS Code, Continue, Claude Code, Codex, Cline, OpenCode, custom scripts, or local model workflows at that endpoint. CrabiX routes requests through the providers and local models you own, applies routing strategy and fallback, and keeps the control plane local.

Core product principles:

- Local-first control plane.
- User-owned providers, subscriptions, API keys, and local models.
- No token markup.
- One endpoint for many tools.
- Transparent provider routing, fallback, and usage visibility.
- Workspace, agents, MCP, Skills, plugins, and AI Corp on the same local backend.

## Download Status

Public builds are not published yet. The canonical download page is:

```text
https://github.com/crabix-ai/CrabiX/releases/latest
```

Planned launch assets:

| Platform | Asset | Status |
| --- | --- | --- |
| Windows | `.exe` | Coming at launch |
| macOS | `.dmg` | Coming at launch |
| Linux | `.AppImage` | Coming at launch |
| Debian / Ubuntu | `.deb` | Coming at launch |
| Fedora / RHEL | `.rpm` | Coming at launch |
| Android | `.apk` or store listing | Coming after mobile launch |
| iOS | App Store listing | Coming after mobile launch |

See [docs/downloads.md](docs/downloads.md) for the release and verification plan.

## Product Map

| Layer | What it gives you |
| --- | --- |
| Provider Router | 13 routing strategies, combo models, fallback, health, latency, local OpenAI-compatible API |
| Cost and Provider Dashboard | One view of provider status, limits, latency, usage, and routing policy |
| AI Workspace | Chat, projects, terminal, browser preview, files, Git, design context, tools, and agents |
| `crabix launch` | Start supported coding tools through the CrabiX gateway without hand-editing each config |
| MCP, Skills, Plugins | External tools, reusable instructions, and installable bundles |
| CLI / Service Mode | Headless gateway and agent workflows from the terminal |
| AI Corp | Companies, teams, AI employees, goals, issues, routines, approvals, budgets, and activity |
| CrabiX Link | Trusted cross-device access through scoped pairing |

## Screenshots

| Provider dashboard | Agents dashboard |
| --- | --- |
| ![CrabiX providers sidebar](assets/screenshots/providers-sidebar.png) | ![CrabiX agents dashboard](assets/screenshots/agents-dashboard.png) |

| Agent issues | Projects |
| --- | --- |
| ![CrabiX agent issues](assets/screenshots/agents-issues.png) | ![CrabiX projects home](assets/screenshots/projects-home.png) |

## Pricing

CrabiX has two public plans:

| Plan | Price | Best for |
| --- | --- | --- |
| Free | `$0` | Core routing, localhost endpoint, chat/workspace basics, provider dashboard, basic agent runtime, basic MCP |
| Pro | `$19/month` | All routing strategies, combo models, unlimited MCP, Skills, plugins, background agents, AI Corp automation, `crabix launch`, Git/design/preview workflows, voice, CrabiX Link |

CrabiX does not add token markup. You pay providers directly through your own subscriptions, API keys, and local model runtimes.

## Security And Privacy

CrabiX is local-first. API keys, provider credentials, prompts, responses, project files, chat history, MCP config, and routing config are intended to stay on your machine unless you send data to a selected provider, support channel, or explicit sharing/sync feature.

Important nuance: local-first does not mean every model runs locally. Cloud providers still receive prompts when you route to a cloud provider. Use local providers such as Ollama or LM Studio when you want inference to stay on device.

Security reports: read [SECURITY.md](SECURITY.md) and email [support@crabix.ai](mailto:support@crabix.ai). Please do not open public GitHub issues for vulnerabilities.

## Links For Humans And Agents

- Website: [crabix.ai](https://crabix.ai)
- Downloads: [GitHub Releases](https://github.com/crabix-ai/CrabiX/releases/latest)
- LLM context: [crabix.ai/llms.txt](https://crabix.ai/llms.txt)
- Full LLM context: [crabix.ai/llms-full.txt](https://crabix.ai/llms-full.txt)
- Agent feed: [crabix.ai/agent-feed.json](https://crabix.ai/agent-feed.json)
- Product docs in this repo: [docs/README.md](docs/README.md)
- Security model: [docs/security-local-first.md](docs/security-local-first.md)

## Community

- Discord: [discord.gg/XTzppGXdNQ](https://discord.gg/XTzppGXdNQ)
- X: [@crabix_ai](https://x.com/crabix_ai)
- YouTube: [@crabix_ai](https://youtube.com/@crabix_ai)
- Telegram channel: [t.me/crabix_ai](https://t.me/crabix_ai)
- Telegram chat: [t.me/crabix_ai_chat](https://t.me/crabix_ai_chat)

## Company

CrabiX is operated by VISIONER PTE. LTD., UEN 202314121N, Singapore.

Support: [support@crabix.ai](mailto:support@crabix.ai)

## License

This repository contains proprietary product materials, brand assets, screenshots, and release metadata. See [LICENSE](LICENSE).
