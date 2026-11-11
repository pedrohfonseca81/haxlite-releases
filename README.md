# haxlite

Native HaxBall client. This repository only hosts the builds; the app updates itself from here.

## Download

Get the file for your system from the [latest release](https://github.com/pedrohfonseca81/haxlite-releases/releases/latest):

| System | File |
|---|---|
| Windows (x64 / ARM) | `haxlite-<version>-windows-x86_64.zip` / `-windows-arm64.zip` |
| Linux (x64 / ARM) | `haxlite-<version>-linux-x86_64.tar.gz` / `-linux-arm64.tar.gz` |
| macOS (Intel and Apple Silicon) | `haxlite-<version>-macos-universal.dmg` |

The builds are not code-signed:

- **Windows:** SmartScreen warns on first run: *More info → Run anyway*.
- **macOS:** right-click the app → *Open*, or run `xattr -dr com.apple.quarantine /Applications/haxlite.app`.

## Updates

haxlite checks this repository when it opens and every few hours, downloads new versions in the background and applies them on the next restart. Every update is verified against a signature built into the app, and if a new version fails to start the previous one is restored. Automatic updates and beta versions can be toggled in *Settings → Misc*.

The `manifest` release holds the signed update manifests (`stable.json`, `beta.json`); it is not a version to download.
