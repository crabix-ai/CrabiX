# Security Policy

## Reporting A Vulnerability

Please report security issues by email:

```text
support@crabix.ai
```

Do not open a public GitHub issue for vulnerabilities.

Include as much detail as you can:

- Affected version or release asset.
- Operating system.
- Steps to reproduce.
- Impact.
- Logs or screenshots, with secrets removed.
- Whether the issue is already public.

## Response Targets

| Stage | Target |
| --- | --- |
| Initial acknowledgement | 3 business days |
| Triage update | 7 business days |
| Fix or mitigation plan | Depends on severity and release status |

CrabiX's first public early release is live, so supported public versions are tied to the signed artifacts present in the current stable release channel.

## Supported Versions

| Version | Supported |
| --- | --- |
| Latest public release | Yes, when available |
| Older public releases | Best effort unless otherwise stated |
| Unreleased/private builds | No public support guarantee |

## Responsible Disclosure

Please give us a reasonable opportunity to investigate and fix the issue before public disclosure. We will credit reporters when appropriate and requested.

## Scope

In scope:

- Public CrabiX release binaries.
- Public website and repository security issues.
- `releases.crabix.ai` release delivery and public download metadata.
- Vulnerabilities that could expose local credentials, prompts, project data, routing config, or linked-device credentials.

Out of scope:

- Social engineering.
- Denial-of-service against public community channels.
- Vulnerabilities in third-party providers unless CrabiX behavior materially worsens the exposure.
- Reports that require access to private source code or private infrastructure without authorization.
