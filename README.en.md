# Orkestrai Releases

[Português](README.md) · **English** · [Español](README.es.md)

Official Orkestrai downloads for macOS, Windows, and Linux.

## Download

Open the [latest release](https://github.com/beeblock/orkestrai-releases/releases/latest)
and select the file for your platform:

- **macOS Apple Silicon** (M1/M2/M3/M4): `Orkestrai-*-arm64.dmg`
- **macOS Intel**: `Orkestrai-*.dmg` without `arm64` in the filename
- **Windows 64-bit**: `Orkestrai-Setup-*.exe`
- **Linux 64-bit**: `Orkestrai-*.AppImage`

Files ending in `*.zip`, `*.blockmap`, and `latest*.yml` are used by the
application's automatic update system. For a manual installation, use a DMG,
EXE, or AppImage file.

## Automatic updates

Orkestrai checks this repository when it starts and again every six hours. The
download is verified against the SHA-512 checksum published in the manifests
before the new version replaces the previous one. Workspaces, settings, and
voice models are stored in the user's data directory and are not removed during
an update.

On macOS without Apple code signing, the application may redirect you to the
manual download. Windows and Linux support automatic replacement through the
installers published here.

Website: [orkestrai.app](https://orkestrai.app)
