# TICKET T01 — Página Home: Diseño Moderno con Efectos 3D

ID: `T01`

Resumen:

Crear la página principal (home) con un diseño moderno y efectos 3D sutiles. Incluir header con logo, barra de búsqueda, filtro para resultados y botón al carrito (link vacío para añadir posteriormente). Añadir un carrusel de ofertas, sección "¡¡¡Visto Recientemente!!!" con productos, sección "Novedades" y footer con contacto ficticio.

Propósito:

Proveer un prototipo visual que sirva como referencia para la implementación front-end del sitio e‑commerce.

Entregables:

- `designs/T01/index.html` (prototipo estático)
- `designs/T01/styles.css` (estilos y efectos 3D)

Criterios de aceptación (mínimos):

1. El header contiene: logo (placeholder), barra de búsqueda, un control de filtro y un botón de carrito con `href=""` (vacío).
2. Existe un carrusel de imágenes para mostrar ofertas y que sea navegable.
3. Debe aparecer el título "¡¡¡Visto Recientemente!!!" alineado a la izquierda, seguido de una grilla de productos (mínimo 6 items) con imagen, nombre y precio.
4. Debe aparecer la sección "Novedades" con otros productos (mínimo 4 items).
5. Footer con email y teléfono ficticios.
6. Diseño con efectos 3D y sombras sutiles; responsive básico.

Escenario Gherkin (ejemplo):

```
Funcionalidad: Ver Home prototipo

Escenario: Mostrar la home con header, carrusel, secciones y footer
  Dado que el diseñador ha generado el prototipo en `designs/T01`
  Cuando abro `designs/T01/index.html` en el navegador
  Entonces veo el header con logo, búsqueda, filtro y botón de carrito
  Y veo un carrusel de ofertas navegable
  Y veo la sección "¡¡¡Visto Recientemente!!!" con productos
  Y veo la sección "Novedades" con al menos 4 novedades
  Y veo un footer con email y teléfono ficticios
```

Notas de diseño:

- Efectos 3D aplicados mediante `transform: perspective(...) translateZ(...)` y sombras.
- Imágenes en el prototipo usan placeholders; sustituir por assets reales en la implementación.
- El botón del carrito tiene `href=""` para que se pueda enlazar cuando exista la página de carrito.

Ruta al prototipo: `designs/T01/index.html`

Asignado a: (pendiente)

Prioridad: Alta (fase 2 — CON-00x / ops de UX)
