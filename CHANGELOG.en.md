# Orkestrai Changelog

[Português](CHANGELOG.md) · [English](CHANGELOG.en.md) · [Español](CHANGELOG.es.md)

## 0.5.0 — 2026-08-10

- Adds local dictation to every editable field, with the existing canvas-leader behavior as the no-focus fallback.
- Allows an agent provider to be changed without losing the member's role, floor, layout, or connections.
- Expands preset roles into complete operating protocols and applies them automatically when the PTY starts.
- Delivers complete unassigned task briefings to the leader at startup and requires Kanban-first delegation.
- Distinguishes task completion, project completion, and attention in native notifications.
- Shows task titles, stages, and assignees in Floors and fixes large shape text while editing.

## 0.4.0 — 2026-08-09

- Adds Cursor, Antigravity, and Cline as native providers alongside Claude, Codex, Kimi, and OpenCode.
- Adds Provider Center with local detection, OS-aware setup, official sign-in guidance, models, effort, and resume capabilities.
- Makes English the default for new installations and asks for the user's language first in onboarding.
- Starts preset terminals with each provider's autonomous full-access flags and repairs older default terminals safely.

## 0.3.0 — 2026-08-09

- Adds up to ten custom Kanban stages shared by the UI, CLI, MCP bridge, leader, and team.
- Adds complete Campaign, Brand and design, and Content and SEO presets for multidisciplinary teams.
- Adds the Orkestrai Contributing consensus team with Claude, Codex, Kimi, and specialist agents.

## 0.2.0 — 2026-08-09

- Adds the preset library with ready-made Product, React, Next.js, SvelteKit, Svelar, and Laravel teams.
- Adds twelve installable specialist roles and portable preset skills.
- Adds the operational Floors overview and localized native desktop menus.
- Refreshes Settings and Documentation with the product visual system.

## 0.1.4 — 2026-08-08

- First macOS release signed with Developer ID Application and notarized by Apple.
- Verifies authority, Team ID, Hardened Runtime, Gatekeeper, and the notarization ticket before publishing Apple Silicon and Intel builds.
- Removes the damaged-app and unidentified-developer warnings from new Mac downloads.
- Mac users on `0.1.3` or earlier need to install `0.1.4` manually once; subsequent signed versions can update through the app.
- Publishes the same release to the legacy and main feeds to prepare future update migration.

## 0.1.3 — 2026-08-07

- Fixes the partial ad-hoc signature in the macOS `0.1.2` packages, which Gatekeeper reported as a damaged application.
- Adds complete signing and deep validation of macOS bundles, DMGs, and ZIPs before publication.
- Blocks automatic replacement on Macs without a Developer ID and preserves the current installation.
- On the first launch of the ad-hoc package, try to open the app, dismiss the warning, then use System Settings → Privacy & Security → Security → **Open Anyway**; authenticate and confirm **Open**. Windows was not affected.

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
