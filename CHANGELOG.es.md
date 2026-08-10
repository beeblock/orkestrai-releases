# Changelog de Orkestrai

[Português](CHANGELOG.md) · [English](CHANGELOG.en.md) · [Español](CHANGELOG.es.md)

## 0.8.2 — 2026-08-10

- Vincula las sesiones rollout de Codex al directorio real del workspace para evitar conversaciones cruzadas entre proyectos concurrentes.
- Vincula las sesiones Kimi mediante el hash exacto de la ruta del workspace, no solo por el nombre de la carpeta final.
- Conserva mensajes completos de varias palabras sin comillas en `orkestrai ask`.
- Trata los timeouts y respuestas no confirmadas como fallos explícitos, no como consultas exitosas.
- Entrega automáticamente la finalización de `task done` al líder sin sobrescribir un borrador humano todavía no enviado.
- Valida conversaciones reales de Claude a Codex y de Codex a Claude mediante los transcripts correctos de los providers.

## 0.8.1 — 2026-08-10

- Corrige el dictado global desde el primer clic y agrega fijación, arrastre y desvío automático de paneles a la esfera de voz.
- Agrega búsqueda y desplazamiento a los selectores con catálogos grandes de modelos, como Devin.
- Mejora el contraste de Orkestrai Light en nodos, paneles, textos, iconos, marcas de providers, botones y hovers.
- Organiza los nodos seleccionados o todo el canvas de forma determinista y mantiene las conexiones detrás de los nodos.
- Iguala los colores de severidad de Uso en panel y nodo y carga resultados iniciales de Skills automáticamente.
- Valida conversaciones de providers antes de reanudar para evitar sesiones obsoletas y reinyección innecesaria de roles.
- Corrige el inicio de las CLIs en Windows, la selección de terminal con DPI y agrega barra de título y menú estilizados.

## 0.8.0 — 2026-08-10

- Agrega un nodo Uso persistente al canvas para las cuotas de Claude, Codex y Kimi.
- Configura provider de origen, fallback y límite compartidos con el líder mediante la acción `usage` de CLI y MCP.
- Agrega tres temas oscuros, uno claro y un editor de tokens semánticos con vista previa inmediata.
- Permite duplicar temas personalizados e importarlos/exportarlos como JSON validado entre instalaciones.
- Aplica los tokens globales al canvas, nodos, Central de Providers, Skills, documentación y Configuración.

## 0.7.0 — 2026-08-10

- Consolida todos los botones de providers en un menú Agentes responsivo y mantiene Shell directamente accesible.
- Permite fijar hasta cuatro agentes listos junto al menú en el orden preferido por el usuario.
- Conserva los agentes fijados globalmente entre workspaces y reinicios de la aplicación.
- Mantiene los agentes no disponibles accesibles mediante la Central de Providers sin ocupar espacio en la barra.

## 0.6.0 — 2026-08-10

- Añade Devin como provider nativo con detección de la CLI oficial, modelos de la cuenta, sesiones autónomas, trabajo headless y reanudación exacta de la conversación.
- Provisiona la skill y el puente MCP de Orkestrai en los directorios nativos del proyecto Devin.
- Usa transcripts ATIF locales para respuestas limpias y habladas, con sesiones concurrentes vinculadas por workspace.
- Inicia Cursor con confianza en el workspace y aprobación de MCP, y Antigravity de forma autónoma con esfuerzo seleccionable.

## 0.5.2 — 2026-08-10

- Permite grabaciones de dictado local de aproximadamente 15 minutos sin fallar con el antiguo límite de 512 KB del servidor empaquetado.
- Restaura los Portales guardados automáticamente cuando el dev server local inicia después del canvas y espera la página real antes de automatizar.
- Reserva IDs de conversación distintos para agentes Claude concurrentes, evitando transcripts cruzados y respuestas corruptas.
- Conserva errores útiles de los Portales y nunca envía el redibujado bruto de la TUI como respuesta de provider.
- No vuelve a inyectar roles al reanudar y activa solo agentes con tareas asignadas aún abiertas o al líder cuando hay trabajo sin responsable.
- Mantiene el servidor disponible mientras macOS espera el permiso de la carpeta del workspace y reintenta de forma segura el aprovisionamiento interrumpido.

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
