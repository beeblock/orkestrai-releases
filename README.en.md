# Orkestrai Releases

[Português](README.md) · **English** · [Español](README.es.md)

Official Orkestrai downloads for macOS, Windows, and Linux.

Change history: [CHANGELOG.en.md](CHANGELOG.en.md).

## Download

Open the [latest release](https://github.com/beeblock/orkestrai-releases/releases/latest)
and select the file for your platform:

- **macOS Apple Silicon** (M1/M2/M3/M4): `Orkestrai-*-arm64.dmg`
- **macOS Intel**: `Orkestrai-*.dmg` without `arm64` in the filename
- **Windows 64-bit**: `Orkestrai-Setup-*.exe`
- **Linux 64-bit**: `Orkestrai-*.AppImage`

On macOS without Apple signing, drag Orkestrai to Applications, try to open it,
and dismiss the warning. Then open **System Settings → Privacy & Security**,
scroll to **Security**, click **Open Anyway**, authenticate, and confirm
**Open**. The button is available for about one hour after the attempt. Do not
use the macOS `0.1.2` packages; their internal signature was fixed in `0.1.3`.

If the button does not appear, try opening the app again. As a last resort for
the package downloaded from this page, run in Terminal:

```bash
sudo xattr -rd com.apple.quarantine "/Applications/Orkestrai.app"
open "/Applications/Orkestrai.app"
```

Files ending in `*.zip`, `*.blockmap`, and `latest*.yml` are used by the
application's automatic update system. For a manual installation, use a DMG,
EXE, or AppImage file.

## Automatic updates

Orkestrai checks this repository when it starts and again every six hours. The
download is verified against the SHA-512 checksum published in the manifests
before the new version replaces the previous one. Workspaces, settings, and
voice models are stored in the user's data directory and are not removed during
an update.

On macOS without Apple code signing, the application detects the new release
but uses a manual download and never removes the current installation. Windows
and Linux support automatic replacement through the installers published here.

Versions `0.0.1` and `0.1.0` were packaged without the updater module. Install
`0.1.1` manually once to enable the corrected flow.

Website: [orkestrai.app](https://orkestrai.app)
