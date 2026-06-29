# Agent Instructions

This repository is the public CrabiX product and downloads repository.

## Purpose

- Keep public product information, release downloads, community files, security policy, and agent-readable context accurate.
- Do not add private application source code, secrets, provider keys, internal credentials, unpublished roadmap claims, or fake adoption metrics.
- Treat [https://crabix.ai/llms.txt](https://crabix.ai/llms.txt), [https://crabix.ai/llms-full.txt](https://crabix.ai/llms-full.txt), and [https://crabix.ai/agent-feed.json](https://crabix.ai/agent-feed.json) as the canonical public product facts.

## Product Truths

- Correct spelling: CrabiX.
- Category: local-first AI router and AI workspace for developers.
- Local endpoint: `http://localhost:3721/v1`.
- Pricing: Free at `$0`, Pro at `$19/month`.
- No token markup. Users pay providers directly.
- Status: first public early release is live. Signed desktop builds are served through canonical `crabix.ai/download` URLs backed by `releases.crabix.ai`.
- Canonical download hub: `https://crabix.ai/download`.
- Canonical release feed: `https://crabix.ai/release-feed.json`.
- Do not invent testimonials, enterprise logos, user counts, benchmark numbers, or revenue.
- Use "local-first control plane" rather than "all models run locally". Cloud providers receive prompts when selected.

## Editing Rules

- Keep public copy in English.
- Prefer concise, technical, credible wording.
- If changing download claims, update `README.md`, `docs/downloads.md`, and `llms.txt` together.
- If changing security, privacy, billing, or legal claims, update `SECURITY.md`, `docs/security-local-first.md`, and public site facts together.
- Do not add GitHub Actions unless there is a real automated check to run and the workflow follows least-privilege permissions.

## Release Rule

Before publishing a release, use [docs/release-checklist.md](docs/release-checklist.md).
