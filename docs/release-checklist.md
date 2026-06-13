# Release Checklist

Use this checklist before publishing public binaries.

## Preflight

- Version number is final.
- Release branch/tag is built from the intended commit.
- Windows, macOS, and Linux artifacts are produced from the release build pipeline.
- No development config, secrets, test provider keys, or private endpoints are bundled.
- App version, release notes, website copy, and repository copy agree.

## Security

- Binaries are signed or notarized where supported.
- Checksums are generated and attached as `SHA256SUMS`.
- Security-sensitive changes are called out in release notes.
- `SECURITY.md` reporting instructions are current.
- No GitHub Actions workflow uses broad token permissions without a reason.

## GitHub Release

- Create the release as a draft first.
- Attach all platform assets.
- Attach `SHA256SUMS`.
- Add release notes with platform support and known issues.
- Mark prerelease only when the build is not intended as the default public download.
- Publish only after all assets are attached.

## Website And Public Docs

- [crabix.ai](https://crabix.ai) download buttons work.
- `README.md` download status is current.
- `docs/downloads.md` status is current.
- `llms.txt` status is current.
- `https://github.com/crabix-ai/CrabiX/releases/latest` resolves without 404.

## Smoke Checks

- Fresh install on Windows.
- Fresh install on macOS.
- Fresh install on at least one Linux distribution.
- App launches.
- Local endpoint binds to `127.0.0.1`.
- Provider setup flow opens.
- Downloaded binary hash matches `SHA256SUMS`.
