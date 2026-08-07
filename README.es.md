# Orkestrai Releases

[Português](README.md) · [English](README.en.md) · **Español**

Descargas oficiales de Orkestrai para macOS, Windows y Linux.

## Descargar

Accede a la [versión más reciente](https://github.com/beeblock/orkestrai-releases/releases/latest)
y elige el archivo correspondiente a tu plataforma:

- **macOS Apple Silicon** (M1/M2/M3/M4): `Orkestrai-*-arm64.dmg`
- **macOS Intel**: `Orkestrai-*.dmg` sin `arm64` en el nombre
- **Windows de 64 bits**: `Orkestrai Setup *.exe`
- **Linux de 64 bits**: `Orkestrai-*.AppImage`

Los archivos `*.zip`, `*.blockmap` y `latest*.yml` son utilizados por el sistema
de actualización automática de la aplicación. Para una instalación manual,
utiliza un archivo DMG, EXE o AppImage.

## Actualizaciones automáticas

Orkestrai verifica este repositorio al iniciarse y nuevamente cada seis horas.
La descarga se valida mediante el checksum SHA-512 publicado en los manifests
antes de que la nueva versión sustituya a la anterior. Los workspaces, ajustes
y modelos de voz se guardan en el directorio de datos del usuario y no se
eliminan durante una actualización.

En macOS sin firma de código de Apple, la aplicación puede redirigirte a la
descarga manual. Windows y Linux permiten la sustitución automática mediante
los instaladores publicados aquí.

Sitio web: [orkestrai.app](https://orkestrai.app)
