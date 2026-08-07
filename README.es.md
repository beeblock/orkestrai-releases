# Orkestrai Releases

[Português](README.md) · [English](README.en.md) · **Español**

Descargas oficiales de Orkestrai para macOS, Windows y Linux.

Historial de cambios: [CHANGELOG.es.md](CHANGELOG.es.md).

## Descargar

Accede a la [versión más reciente](https://github.com/beeblock/orkestrai-releases/releases/latest)
y elige el archivo correspondiente a tu plataforma:

- **macOS Apple Silicon** (M1/M2/M3/M4): `Orkestrai-*-arm64.dmg`
- **macOS Intel**: `Orkestrai-*.dmg` sin `arm64` en el nombre
- **Windows de 64 bits**: `Orkestrai-Setup-*.exe`
- **Linux de 64 bits**: `Orkestrai-*.AppImage`

En macOS sin firma de Apple, arrastra Orkestrai a Aplicaciones y usa Control/clic
derecho en la app → **Abrir** en el primer inicio. No utilices los paquetes
macOS `0.1.2`; su firma interna fue corregida en `0.1.3`.

Los archivos `*.zip`, `*.blockmap` y `latest*.yml` son utilizados por el sistema
de actualización automática de la aplicación. Para una instalación manual,
utiliza un archivo DMG, EXE o AppImage.

## Actualizaciones automáticas

Orkestrai verifica este repositorio al iniciarse y nuevamente cada seis horas.
La descarga se valida mediante el checksum SHA-512 publicado en los manifests
antes de que la nueva versión sustituya a la anterior. Los workspaces, ajustes
y modelos de voz se guardan en el directorio de datos del usuario y no se
eliminan durante una actualización.

En macOS sin firma de código de Apple, la aplicación detecta la nueva release,
pero usa una descarga manual y nunca elimina la instalación actual. Windows y
Linux permiten la sustitución automática mediante los instaladores publicados
aquí.

Las versiones `0.0.1` y `0.1.0` se empaquetaron sin el módulo de actualización.
Instala `0.1.1` manualmente una sola vez para habilitar el flujo corregido.

Sitio web: [orkestrai.app](https://orkestrai.app)
