# Changelog de Orkestrai

[Português](CHANGELOG.md) · [English](CHANGELOG.en.md) · [Español](CHANGELOG.es.md)

## 0.5.1 — 2026-08-10

- Descarta IDs locales de PTY obsoletos después de reiniciar la aplicación y conserva el ID de conversación de cada provider.
- Recrea las terminales y reanuda sus conversaciones automáticamente, en lugar de dejar todos los nodos con error de sesión inexistente.
- Hace que la recuperación sea determinista mediante un código WebSocket estable y la persistencia del ID de la sesión reemplazada.

## 0.5.0 — 2026-08-10

- Añade dictado local en todos los campos editables y mantiene al líder del canvas como fallback cuando no hay campo enfocado.
- Permite cambiar el provider de un agente sin perder rol, piso, layout ni conexiones del miembro.
- Amplía los roles de presets con protocolos operativos completos y los aplica automáticamente al iniciar la PTY.
- Entrega al líder los briefings completos de tareas sin responsable al iniciar y exige delegar primero mediante el kanban.
- Distingue tarea completada, proyecto completado y atención en las notificaciones nativas.
- Muestra títulos, etapas y responsables en Pisos y corrige la edición de texto grande en las formas.

## 0.4.0 — 2026-08-09

- Añade Cursor, Antigravity y Cline como providers nativos junto con Claude, Codex, Kimi y OpenCode.
- Añade la Central de Providers con detección local, setup por sistema, inicio de sesión oficial, modelos, esfuerzo y reanudación.
- Define inglés como idioma predeterminado en instalaciones nuevas y pregunta primero el idioma en el onboarding.
- Inicia terminales de presets con las flags autónomas de acceso total y repara terminales predeterminadas antiguas de forma segura.

## 0.3.0 — 2026-08-09

- Añade hasta diez etapas personalizadas del kanban compartidas por UI, CLI, MCP, líder y equipo.
- Añade presets completos de Campaña, Brand y diseño y Contenido y SEO para equipos multidisciplinares.
- Añade el equipo de consenso Orkestrai Contributing con Claude, Codex, Kimi y agentes especialistas.

## 0.2.0 — 2026-08-09

- Añade la Biblioteca de presets con equipos listos de Producto, React, Next.js, SvelteKit, Svelar y Laravel.
- Añade doce roles especialistas instalables y skills portátiles en los presets.
- Añade la vista operativa de Pisos y menús de escritorio nativos traducidos.
- Actualiza Configuración y Documentación con el sistema visual del producto.

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
