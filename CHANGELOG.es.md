# Changelog de Orkestrai

[Português](CHANGELOG.md) · [English](CHANGELOG.en.md) · [Español](CHANGELOG.es.md)

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
