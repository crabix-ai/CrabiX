# GitHub Repository Settings

Status: applied and verified on 2026-06-13 with the active `crabix-ai` GitHub account.

This file records the intended public repository settings so future maintainers can audit or reapply them.

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

## Verified State

Verified through `gh repo view` and `gh api repos/crabix-ai/CrabiX`:

```json
{
  "homepage": "https://crabix.ai",
  "has_issues": true,
  "has_discussions": true,
  "has_projects": false,
  "has_wiki": false,
  "allow_squash_merge": true,
  "allow_merge_commit": false,
  "allow_rebase_merge": false,
  "delete_branch_on_merge": true,
  "permissions": {
    "admin": true
  }
}
```

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
