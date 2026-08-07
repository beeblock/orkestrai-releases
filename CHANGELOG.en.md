# Orkestrai Changelog

[Português](CHANGELOG.md) · [English](CHANGELOG.en.md) · [Español](CHANGELOG.es.md)

## 0.1.2 — 2026-08-07

- Changes automatic Usage refresh from 60 seconds to 5 minutes.
- Aligns the server cache to prevent duplicate provider requests.
- Keeps the manual refresh button fetching fresh data immediately.
- Reduces the risk of Claude HTTP 429 responses during long sessions.

## 0.1.1 — 2026-08-07

- Includes `electron-updater` in the installed application.
- Fixes the incorrect diagnosis that automatic updates only exist outside the package.
- Sends manual tasks to the leader with title, description, and every image.
- Installations on `0.0.1` and `0.1.0` must install this version manually once.

## 0.1.0 — 2026-08-07

- First public cross-platform release with manifests and SHA-512 validation.
- Adds local multilingual voice, the Ports panel, and global leader dictation.
