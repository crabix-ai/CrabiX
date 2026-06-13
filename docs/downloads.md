# Downloads

Canonical download URL:

```text
https://github.com/crabix-ai/CrabiX/releases/latest
```

As of 2026-06-13, CrabiX is pre-launch and no public release asset has been published.

## Planned Launch Assets

| Platform | Asset type | Notes |
| --- | --- | --- |
| Windows | `.exe` | Desktop installer. |
| macOS | `.dmg` | Desktop disk image. |
| Linux | `.AppImage` | Portable Linux desktop build. |
| Debian / Ubuntu | `.deb` | Package for apt-based distributions. |
| Fedora / RHEL | `.rpm` | Package for rpm-based distributions. |
| Android | `.apk` or store listing | Mobile companion after mobile launch. |
| iOS | App Store listing | Mobile companion after mobile launch. |

## Release Asset Naming

Use predictable names so links, docs, scripts, and humans can identify platform and architecture:

```text
CrabiX_<version>_windows_x64.exe
CrabiX_<version>_macos_universal.dmg
CrabiX_<version>_linux_x64.AppImage
CrabiX_<version>_linux_amd64.deb
CrabiX_<version>_linux_x86_64.rpm
SHA256SUMS
```

Keep release notes human-readable and include:

- Version and release date.
- Supported platforms.
- New features.
- Fixes.
- Known issues.
- Checksums.
- Security notes when relevant.

## Verification

For every public binary release:

1. Download from GitHub Releases only.
2. Compare the file hash against `SHA256SUMS`.
3. On macOS and Windows, prefer signed and notarized builds when available.
4. Avoid third-party mirrors unless CrabiX explicitly links them from [crabix.ai](https://crabix.ai) or this repository.

## Website Sync

The website download buttons point to:

```text
https://github.com/crabix-ai/CrabiX/releases/latest
```

When the first release goes live, verify:

- [crabix.ai](https://crabix.ai) download buttons open the latest release.
- `README.md` no longer says "no public release asset has been published".
- `llms.txt` is updated if status changes.
- `docs/release-checklist.md` is complete.
