# AIMyChats releases

Build artifacts for **AIMyChats**, the local-first WeChat desktop client from
[`oneprolabs/devify-desktop`](https://github.com/oneprolabs/devify-desktop).

This repository holds release assets only. Source code, issues and pull requests live in the
private source repository.

## Releases

- **`alpha`** — the rolling prerelease consumed by the in-app updater. It contains the signed
  macOS app, the updater archive (`.app.tar.gz`), its `.sig`, and `latest.json`.
- **`v*`** — milestone builds published for manual installation.

Release assets are produced by `.github/workflows/release-macos.yml` in the source repository.

## Installing

1. Download the DMG from the desired release.
2. macOS Gatekeeper blocks the first launch because the app is not notarised: Control-click the
   app → **Open**, then confirm.
3. Grant **Full Disk Access** to `AIMyChats.app` in System Settings → Privacy & Security before
   reading local WeChat databases.