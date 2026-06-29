# Security And Local-First Model

CrabiX is designed as a local-first control plane for AI tools, providers, agents, and workspace workflows.

## What Stays Local By Default

The following data is intended to stay on the user's machine unless explicitly sent to a provider, support channel, sync/sharing feature, or linked device:

- API keys and provider credentials.
- Provider routing configuration.
- Prompts and responses stored in local history.
- Project files and workspace context.
- MCP configuration.
- Skills and plugin configuration.
- Local agent execution trail.
- AI Corp companies, teams, employees, issues, routines, approvals, budgets, and activity.

The public privacy policy separates local app data from website, account, billing, support, and optional product data. See [crabix.ai/privacy](https://crabix.ai/privacy).

Provider keys are intended to stay on the user's machine, using the operating system keyring where available: macOS Keychain, Windows Credential Manager, or Linux keyutils, with an encrypted fallback when no keyring is available.

## What Cloud Providers Still See

Local-first does not mean every model runs locally.

When the selected route is a cloud provider, that provider receives the prompt, context, and tool output needed to answer the request. Use local providers such as Ollama or LM Studio when you want inference to stay on your machine.

CrabiX as a company does not need to proxy prompts through its own hosted service for normal local use. Cloud providers still process requests under their own terms when selected.

## Local Endpoint

The default public positioning is:

```text
http://localhost:3721/v1
```

The local gateway binds to `127.0.0.1` by default rather than all network interfaces.

Security-sensitive wording:

- Say "local-first control plane".
- Say "gateway binds to `127.0.0.1` by default" when describing default exposure.
- Do not say "all data never leaves your machine" without the provider nuance above.

## Billing Boundary

CrabiX charges for the software/control plane, not provider tokens. Paid purchases are handled by Paddle as merchant of record. CrabiX does not store full payment card numbers. Refund terms are at [crabix.ai/refund](https://crabix.ai/refund).

## Cross-Device Access

CrabiX Link is intended to use trusted-device pairing and scoped authorization. Do not expose the local gateway publicly without an explicit secure access layer.

## Reporting Vulnerabilities

Read [../SECURITY.md](../SECURITY.md). Do not open public issues for vulnerabilities.
