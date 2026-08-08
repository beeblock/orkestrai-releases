# Changelog de Orkestrai

[Português](CHANGELOG.md) · [English](CHANGELOG.en.md) · [Español](CHANGELOG.es.md)

## 0.1.4 — 2026-08-08

- Primera release para macOS firmada con Developer ID Application y notarizada por Apple.
- Valida autoridad, Team ID, Hardened Runtime, Gatekeeper y el ticket de notarización antes de publicar las versiones Apple Silicon e Intel.
- Elimina los avisos de aplicación dañada o desarrollador no identificado de las nuevas descargas para Mac.
- Los usuarios de Mac en `0.1.3` o anterior necesitan instalar `0.1.4` manualmente una vez; las siguientes versiones firmadas pueden actualizarse desde la aplicación.
- Publica la misma release en los feeds legado y principal para preparar la migración de actualizaciones futuras.

## 0.1.3 — 2026-08-07

- Corrige la firma ad-hoc parcial de los paquetes macOS `0.1.2`, que Gatekeeper reportaba como una aplicación dañada.
- Añade firma completa y validación profunda de bundles, DMGs y ZIPs macOS antes de publicar.
- Bloquea el reemplazo automático en Mac sin Developer ID y preserva la instalación actual.
- En el primer inicio del paquete ad-hoc, intenta abrir la app, cierra el aviso y usa Ajustes del Sistema → Privacidad y seguridad → Seguridad → **Abrir de todos modos**; autentícate y confirma **Abrir**. Windows no fue afectado.

## 0.1.2 — 2026-08-07

- Cambia la actualización automática del panel Uso de 60 segundos a 5 minutos.
- Alinea la caché del servidor para evitar consultas duplicadas a los providers.
- Mantiene el botón de actualización manual obteniendo datos nuevos inmediatamente.
- Reduce el riesgo de respuestas HTTP 429 de Claude durante sesiones largas.

## 0.1.1 — 2026-08-07

- Incluye `electron-updater` en la aplicación instalada.
- Corrige el diagnóstico incorrecto de que las actualizaciones automáticas solo existen fuera del paquete.
- Envía las tareas manuales al líder con título, descripción y todas las imágenes.
- Las instalaciones `0.0.1` y `0.1.0` deben instalar esta versión manualmente una vez.

## 0.1.0 — 2026-08-07

- Primera release pública multiplataforma con manifests y validación SHA-512.
- Añade voz multilingüe local, el panel Puertos y el dictado global para el líder.
