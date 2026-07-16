# Mythos — Public Release Artifacts

This repository hosts the installer + auto-updater artifacts for [Mythos](https://mythos.kabalrpg.com).

Source code lives in a private repository. This repo exists so the in-app auto-updater has a public URL to fetch signed artifacts from.

Every release includes:

- **macOS** — `.app.tar.gz` (auto-updater payload) + `.sig` (minisign signature)
- **Windows** — `.exe` (NSIS installer) + `.msi` + `.sig`s
- **Linux** — `.AppImage` (self-contained portable binary) + `.sig`

To download the initial installer, visit [mythos.kabalrpg.com](https://mythos.kabalrpg.com) or grab it from the [Releases page](https://github.com/holsat/mythos-releases/releases) directly.

