# Prototipos Coflita

Repositorio con prototipos de diseño para un e‑commerce de indumentaria deportiva.

Descripción breve:
- `designs/T01/index.html`: Página home / catálogo con carrusel, filtros y listado de productos.
- `designs/T02/index.html`: Página de checkout (resumen del pedido y formulario de pago con efectos modernos 3D).
- `designs/T02/styles.css`: Estilos del prototipo de checkout.

Objetivo:
Proveer prototipos visuales y de interacción (HTML/CSS/JS) para validar UX, estilos y flujo de compra antes de implementar en el repositorio de código.

Cómo probar localmente:
1. Abrir `designs/T01/index.html` en un navegador (doble clic sobre el archivo o `Ctrl+O` en el navegador y seleccionar el archivo).
2. En la cabecera, hacer click en "Carrito 🛒" para navegar al checkout: `designs/T02/index.html`.
3. En la página de checkout se puede completar el formulario (simulación) y presionar "Completar Compra" para ver la confirmación (modal).

Notas de implementación:
- El formulario de pago es una simulación: no hay integración real con pasarelas. Evitar usar datos reales de tarjeta en este prototipo.
- Se implementaron pequeñas validaciones y formateo (número de tarjeta y expiración) para mejorar la experiencia de prueba.
- Los estilos usan gradientes y transformaciones 3D para dar sensación de profundidad en las tarjetas de producto.

Siguientes pasos recomendados:
- Añadir `index2.html` de compatibilidad si hay rutas externas que lo referencian.
- Integrar lectura de carrito desde `localStorage` o un endpoint para poblar dinámicamente la lista de productos.
- Añadir pruebas visuales o screenshots en `designs/T02/README.md` si se requieren ejemplos de diseño.

Contacto:
- Equipo de Producto: contacto@ejemplo.com

