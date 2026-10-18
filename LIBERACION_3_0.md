# Sistema Juande 3.0 · Liberación inicial

Publicación autorizada por Juande el 17 de octubre de 2026, omitiendo las pruebas manuales previas solicitadas. No se presentan como verificadas.

## Incluido

26 originales y métodos operativos; análisis simplificado con Gemini; evidencias y revisión; fichas, integración en las tres secciones; correcciones de ROI/parlays. Se conserva el almacenamiento de producción `juande-mobile-reset-20261012-v1`, la copia privada de Supabase y el Radar publicado. Antes de escribir el estado local existente se guarda su texto exacto en `juande-release-3.0-before-20261017`. Si falla esa copia/lectura se bloquean escrituras del estado principal en la sesión. La copia es del navegador, no un respaldo externo.

## Conexiones y alcance

- Radar publicado y copia privada: proyecto productivo existente, sin migraciones ni escrituras de datos durante la liberación.
- IA y fichas: se reutiliza el servicio ya configurado en el proyecto Sistema Juande 3.0 Pruebas. Su nombre no cambia su acceso: sigue autenticado y restringido al propietario, con RLS y cinco reservas diarias compartidas entre las dos aplicaciones. No constituye un backend productivo aislado. Iniciar sesión aquí requiere la cuenta de investigación configurada; no se copian las sesiones de la cuenta del Radar.
- Google Free confirmado por captura; organización Supabase verificada Free. Sin pago, modelos alternativos, reintentos ni nuevos servicios. La función no comprueba Cloud Billing automáticamente; mantener Google sin facturación vinculada.
- No hay automatización de apuestas ni sincronización bidireccional completa. Guardar una ficha requiere revisión para clasificarla.

## Verificaciones y pendientes

Las suites del motor, servicio con proveedor simulado, recuperación y finanzas se ejecutan sobre esta versión. Se añaden comprobaciones de conservación de datos productivos y puente de nube. No se ha completado una investigación real con Gemini ni la aceptación visual en Safari iPhone. La conexión reporta configuración habilitada, lo que no acredita una inferencia correcta.

## Retorno

Commit productivo previo: `26fdf18ed108f353c79af3bdb78bb1a64783dd1b`, conservado en la rama `rollback/pre-oraculo-3-26fdf18`. El propietario corrigió el acceso y la creación de la rama fue confirmada antes de publicar. El retorno de código no debe borrar datos ni restablecer automáticamente una copia antigua. La clave principal y la conexión productiva se conservan para que la versión anterior lea su estado. No hay cambios de esquema que revertir.

## Verificación automática

50 grupos automatizados aprobados (71 escenarios), incluidos conservación del estado productivo y fallo de respaldo. Comprobados enlaces locales, IDs y sintaxis de todos los scripts inline y JavaScript modificado. Sin inferencia real de Gemini ni prueba visual de Safari. No se ejecutan operaciones de escritura sobre la base productiva durante la publicación.
