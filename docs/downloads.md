# Downloads

Canonical download hub:

```text
https://crabix.ai/download
```

As of 2026-06-30, CrabiX's first public early release is live. Signed desktop builds are served through canonical crabix.ai download URLs when their platform artifacts are present in the stable release channel.

## Release Metadata

CrabiX download pages are backed by the stable release manifest on releases.crabix.ai and normalized for agents through the website release feed:

```text
https://releases.crabix.ai/channels/stable/latest.json
https://crabix.ai/release-feed.json
https://crabix.ai/.well-known/release-feed.json
```

Agents and docs should cite only artifacts, checksums, signatures, sizes, versions, dates, and release notes present in those feeds.

## Canonical Platform URLs

| Platform | URL | Asset type |
| --- | --- | --- |
| macOS Apple Silicon | `https://crabix.ai/download/macos/aarch64/latest` | Signed DMG |
| macOS Intel | `https://crabix.ai/download/macos/x86_64/latest` | Signed DMG |
| Windows x64 | `https://crabix.ai/download/windows/x86_64/latest` | Signed installer |
| Windows ARM | `https://crabix.ai/download/windows/aarch64/latest` | Signed installer |
| Linux AppImage | `https://crabix.ai/download/linux/x86_64/appimage/latest` | AppImage |
| Debian / Ubuntu | `https://crabix.ai/download/linux/x86_64/deb/latest` | `.deb` package |
| Fedora / RHEL | `https://crabix.ai/download/linux/x86_64/rpm/latest` | `.rpm` package |

Platform URLs can return 404 when the matching artifact is not present in the current stable release channel. A URL being canonical does not mean the artifact is currently available.

## Release Notes

Keep release notes human-readable and include:

- Version and release date.
- Supported platforms.
- New features.
- Fixes.
- Known issues.
- Checksums and signatures when present in the release manifest.
- Security notes when relevant.

## Verification

For every public binary release:

1. Download from the canonical crabix.ai platform URL.
2. Read `https://crabix.ai/release-feed.json`.
3. Verify the version, platform, artifact URL, checksum, updater signature, and signature path when those fields are present.
4. On macOS and Windows, prefer signed and notarized builds when available.
5. Avoid third-party mirrors unless CrabiX explicitly links them from [crabix.ai](https://crabix.ai) or this repository.

## Website Sync

When release or download claims change, verify:

- [crabix.ai/download](https://crabix.ai/download) and platform pages reflect the current stable release metadata.
- [crabix.ai/release-feed.json](https://crabix.ai/release-feed.json) includes only real stable-channel artifacts.
- `README.md` download status is current.
- `llms.txt` is updated if public facts change.
- `docs/release-checklist.md` is complete before publishing a new public release.
