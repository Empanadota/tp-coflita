**Propósito**

Este archivo guía a agentes de IA (Copilot/AGENTs) para trabajar productiva y coherentemente en este repositorio. El proyecto actual contiene principalmente documentación estratégica y de producto para un e‑commerce de indumentaria deportiva (no hay código fuente detectable en el repositorio raíz). Antes de modificar o añadir implementaciones de software, confirma con el equipo dónde está el repositorio de código.

**Archivos clave (leer antes de actuar)**
- `context/COPY Creativo y Estratégico para Sitio Web de Indumentaria Deportiva.md`: copy y tono de la marca; mantener estilo aspiracional y orientado a conversión.
- `context/Funciones Esenciales para un Sitio Web de Indumentaria Deportiva.md`: lista de funcionalidades prioritarias (checkout, guías de tallas, imágenes, CDN).
- `context/Criterios de aceptación mínimos...Gherkin.md`: criterios de aceptación en formato Gherkin — añadir escenarios nuevos aquí cuando se implemente funcionalidad.
- `context/Este documento presenta los tickets...md`: backlog priorizado con IDs (ej. `INF-001`, `CON-001`, `CHK-001`) — actualizar estos tickets al proponer o aplicar cambios.
- `context/Las historias de usuario...md` y `context/Resumen ejecutivo...md`: contexto estratégico y requisitos de negocio.

**Big picture / arquitectura conceptual**
- Este repo actúa como el «source of truth» de producto y marketing para un e‑commerce D2C enfocado en athleisure. Los artefactos describen tres capas: Infraestructura & Rendimiento (CDN, optimización de imágenes), Producto & UX (ficha de producto, recomendador de tallas, UGC) y Checkout & Operaciones (pagos, inventario, soporte en tiempo real).
- Flujo de trabajo esperado: Producto/Marketing → Historias de usuario/Gherkin → Tickets priorizados (en el documento de tickets) → Implementación (en repositorio de código separado) → Actualizar criterios Gherkin y tickets.

**Convenciones y patrones específicos del proyecto**
- Documentación en español y con tono de marca (aspiracional). Mantener ese registro para cualquier copy o texto que se agregue.
- Historias de usuario usan formato `COMO / QUIERO / PARA` — respeta ese formato en nuevas historias.
- Los criterios de aceptación están en tablas Gherkin: si agregas un escenario, edita `context/Criterios de aceptación mínimos...Gherkin.md` con la misma estructura.
- Los tickets referenciados usan IDs con prefijos: `INF-`, `CON-`, `CHK-`, `FID-` — mencionar el ID apropiado cuando propongas cambios técnicos o de producto.

**Instrucciones prácticas para agentes (acciones concretas)**
- Si vas a proponer una implementación (ej.: recomendador de tallas): 1) Añade un comentario en el ticket `CON-001` (documento de tickets) con la arquitectura propuesta; 2) Añade/actualiza el escenario Gherkin en `context/Criterios de aceptación...`; 3) solicita el repositorio de código y los detalles de despliegue.
- Para cambios de copy: edita únicamente `context/COPY Creativo...md` o crea un nuevo archivo en `context/` con nombre claro `COPY <sección> - vN.md`; mantén tono aspiracional y CTA claros.
- Para propuestas de rendimiento (CDN, imágenes): referencia `INF-001` y documenta pasos de validación (métricas objetivo: carga < 2s).

**Ejemplos concretos extraídos del repositorio**
- Recomendador de tallas: referirse a `CON-001` (tickets) y al escenario Gherkin en `Criterios de aceptación...` antes de implementar; el documento sugiere uso de "lógica difusa".
- Optimización imágenes: `INF-002` describe compresión y redimensionado; usar esa referencia al proponer pipelines de optimización.

**Qué hacer si no hay código en este repo**
- Pregunta inmediatamente dónde está el repositorio de implementación (por ejemplo: frontend, backend, infra). No intentes crear artefactos de implementación en este repo sin confirmación.

**Checklist breve antes de crear PRs en repositorios de código relacionados**
- Confirmar ticket de referencia (ID) y actualizar documento de tickets.  
- Añadir/actualizar escenario Gherkin en `context/Criterios de aceptación...`.  
- Documentar cambios de infraestructura (CDN, optimización) con métricas objetivo (target < 2s).  
- Para copy: mantener tono, CTA y ejemplos de producto.  

Si algo en estas instrucciones no está claro o falta información (por ejemplo: ubicación del repo de código, políticas de commit o CI), dime exactamente qué sección quieres que expanda y lo ajusto.
