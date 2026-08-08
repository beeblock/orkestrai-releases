# Orkestrai Releases

[Português](README.md) · [English](README.en.md) · **Español**

Este es el feed legado de Orkestrai. Las nuevas releases y descargas oficiales
se publican en el [repositorio principal](https://github.com/beeblock/orkestrai/releases).
La release `0.1.4` permanecerá aquí como puente para las instalaciones que aún
consultan esta dirección.

Historial de cambios: [CHANGELOG.es.md](CHANGELOG.es.md).

## Descargar

Accede a la [versión más reciente](https://github.com/beeblock/orkestrai/releases/latest)
y elige el archivo correspondiente a tu plataforma:

- **macOS Apple Silicon** (M1/M2/M3/M4): `Orkestrai-*-arm64.dmg`
- **macOS Intel**: `Orkestrai-*.dmg` sin `arm64` en el nombre
- **Windows de 64 bits**: `Orkestrai-Setup-*.exe`
- **Linux de 64 bits**: `Orkestrai-*.AppImage`

En macOS sin firma de Apple, arrastra Orkestrai a Aplicaciones, intenta abrirla
y cierra el aviso. Después abre **Ajustes del Sistema → Privacidad y seguridad**,
ve a **Seguridad**, haz clic en **Abrir de todos modos**, autentícate y confirma
**Abrir**. El botón está disponible durante aproximadamente una hora después
del intento. No utilices los paquetes macOS `0.1.2`; su firma interna fue
corregida en `0.1.3`.

Si el botón no aparece, intenta abrir la app de nuevo. Como último recurso para
el paquete descargado de esta página, ejecuta en Terminal:

```bash
sudo xattr -rd com.apple.quarantine "/Applications/Orkestrai.app"
open "/Applications/Orkestrai.app"
```

Los archivos `*.zip`, `*.blockmap` y `latest*.yml` son utilizados por el sistema
de actualización automática de la aplicación. Para una instalación manual,
utiliza un archivo DMG, EXE o AppImage.

## Actualizaciones automáticas

Las versiones hasta `0.1.3` verifican este repositorio al iniciarse y nuevamente
cada seis horas. La versión `0.1.4` migra la aplicación al feed del repositorio
principal.
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
