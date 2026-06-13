# 2026 Public Repository Research

Date: 2026-06-13

Task: configure `crabix-ai/CrabiX` as a public product and downloads repository for CrabiX.

## Sources Used

Context7:

- GitHub Docs via `/github/docs`: repository README/community health/security policy guidance and releases/release assets guidance.
- GitHub CLI manual via `/websites/cli_github_manual`: `gh repo edit` metadata flags.

Brave Search:

- GitHub Docs, "Best practices for repositories": https://docs.github.com/en/repositories/creating-and-managing-repositories/best-practices-for-repositories
- GitHub Docs, "About community profiles for public repositories": https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/about-community-profiles-for-public-repositories
- GitHub Docs, "Managing releases in a repository": https://docs.github.com/en/repositories/releasing-projects-on-github/managing-releases-in-a-repository
- GitHub Blog, "What's coming to our GitHub Actions 2026 security roadmap": https://github.blog/news-insights/product-news/whats-coming-to-our-github-actions-2026-security-roadmap/
- llms.txt proposal: https://llmstxt.org/
- 2026 llms.txt ecosystem discussion showing it is useful for agent discovery but not a guaranteed search ranking lever: https://www.elementera.com/blog/what-is-llms-txt-how-implement-for-ai-bots-2026-guide

Local product sources:

- Live site: https://crabix.ai
- Live LLM context: https://crabix.ai/llms.txt
- Live full LLM context: https://crabix.ai/llms-full.txt
- Live agent feed: https://crabix.ai/agent-feed.json
- Website project: `/Users/alex/dev/crabix-website`

## Findings

1. The public repo needs a strong README, not only files. GitHub documentation treats README as the primary orientation surface. Third-party 2026 README guidance converges on the same pattern: quick hook, visual proof, install/download path, why it exists, and clear next links.

2. Downloads should be routed through GitHub Releases. GitHub Releases are meant to package software, release notes, and binary assets. The stable user-facing path is `/releases/latest`; the REST latest endpoint returns the latest non-draft, non-prerelease release. As of this setup, the latest release API returns 404 because no release exists yet, so the repo must say pre-launch honestly.

3. Community health files matter even for a product repository. README, SECURITY, CONTRIBUTING, CODE_OF_CONDUCT, issue templates, support links, and a clear license stance reduce ambiguity for users and AI agents.

4. Security defaults should stay minimal. GitHub's 2026 Actions security roadmap emphasizes central policy, limited triggers, scoped permissions, and supply-chain auditability. Because this repository has no build/test automation yet, adding GitHub Actions now would create surface area without value.

5. `llms.txt` is useful as a low-cost agent discovery layer. It is an emerging convention, not an official ranking standard. The right use here is not SEO magic; it is a concise product fact file for coding agents and LLM retrieval.

6. Repository metadata should be configured. Homepage, description, topics, issues, discussions, disabled wiki, and disabled projects improve the GitHub first impression and navigation.

## Decision

Configure this repository as a public product and release hub:

- Polished `README.md` with visual assets, product map, download status, pricing, security, and community links.
- `docs/` for downloads, release checklist, product overview, security model, and research rationale.
- `llms.txt` and `AGENTS.md` for agent-readable context and future agent edits.
- GitHub community health files: `SECURITY.md`, `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, `SUPPORT.md`, issue templates, PR template.
- Proprietary license statement because the desktop app source is not published here.
- No GitHub Actions yet.

## Follow-Up For First Release

- Publish release assets as a draft first, attach all binaries and checksums, then publish.
- Update `README.md`, `docs/downloads.md`, and `llms.txt` when `/releases/latest` resolves.
- Consider enabling immutable releases if the repository release process requires strict supply-chain guarantees.
- Revisit GitHub Actions only when there is a real check or release automation to run.
