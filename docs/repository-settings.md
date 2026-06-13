# GitHub Repository Settings

These settings should be applied by a GitHub account with admin access to `crabix-ai/CrabiX`.

The initial content can be pushed with write access, but `gh repo edit` requires repository administration permission.

## Desired Metadata

- Description: `CrabiX - local-first AI router and AI workspace for developers. One localhost endpoint for providers, local models, coding tools, agents, MCP, Skills, and AI Corp.`
- Homepage: `https://crabix.ai`
- Topics:
  - `ai-router`
  - `local-first`
  - `openai-compatible`
  - `llm`
  - `ai-agents`
  - `developer-tools`
  - `mcp`
  - `desktop-app`
  - `ai-workspace`

## Desired Features

- Issues: enabled.
- Discussions: enabled.
- Wiki: disabled.
- Projects: disabled.
- Pull requests: squash merge enabled, merge commit disabled, rebase merge disabled.
- Delete head branches after merge: enabled.

## Suggested Command

```bash
gh repo edit crabix-ai/CrabiX \
  --homepage https://crabix.ai \
  --description "CrabiX - local-first AI router and AI workspace for developers. One localhost endpoint for providers, local models, coding tools, agents, MCP, Skills, and AI Corp." \
  --enable-issues=true \
  --enable-discussions=true \
  --enable-projects=false \
  --enable-wiki=false \
  --enable-squash-merge=true \
  --enable-merge-commit=false \
  --enable-rebase-merge=false \
  --delete-branch-on-merge=true \
  --add-topic ai-router \
  --add-topic local-first \
  --add-topic openai-compatible \
  --add-topic llm \
  --add-topic ai-agents \
  --add-topic developer-tools \
  --add-topic mcp \
  --add-topic desktop-app \
  --add-topic ai-workspace
```

## Security Settings

Enable these in GitHub repository settings where available:

- Secret scanning.
- Secret scanning push protection.
- Dependabot alerts if dependencies are ever added.
- Code scanning only when the repository contains code or workflows worth scanning.

Do not add GitHub Actions until there is a real check or release automation to run.
