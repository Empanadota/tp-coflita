Este documento presenta los *tickets* ordenados de forma lineal por prioridad, asegurando que se cumplen primero los requisitos críticos de **rendimiento y conversión** definidos en las historias de usuario y los criterios de aceptación (Gherkin) previamente establecidos.

---

## **TICKETS LINEALES (PRIORIZADOS) PARA E-COMMERCE DE INDUMENTARIA DEPORTIVA**

### **FASE 1: INFRAESTRUCTURA Y RENDIMIENTO (Velocidad Récord)**

La prioridad más alta es garantizar que el sitio cargue rápidamente (menos de dos segundos), ya que los sitios lentos impactan negativamente en el SEO y aumentan los costos de adquisición \[13, 26 (59, 61)\].

| TICKET ID | Título del Ticket | Requisitos Cumplidos |
| ----- | ----- | ----- |
| **INF-001** | **Implementación y Optimización de CDN** | **Requisito Gherkin:** El tiempo de carga debe ser **menor a dos segundos**. **Acción:** Usar una Red de Distribución de Contenido (CDN) para distribuir la entrega de contenido y asegurar experiencias rápidas a nivel global \[26 (62, 63), 31 (24, 25)\]. |
| **INF-002** | **Optimización Masiva de Imágenes y Archivos** | **Historia de Usuario:** COMO Diseñador Web, QUIERO comprimir, redimensionar y reducir el tamaño de las imágenes \[31 (22, 23)\], PARA mejorar significativamente la velocidad de carga \[31 (22, 23)\]. **Acción:** Comprimir, redimensionar y reducir el tamaño de las imágenes, ya que representan el 50-75% del peso de las páginas \[20 (52, 53), 26 (74, 75)\]. |
| **INF-003** | **Configuración de Carga Diferida (*Lazy Loading*) y Limpieza de Código** | **Historia de Usuario:** COMO Desarrollador de UX, QUIERO habilitar la carga diferida \[31 (21)\], PARA posponer la carga de contenido suplementario (como reseñas) y mejorar el rendimiento \[26 (78, 79)\]. **Acción:** Eliminar aplicaciones de terceros innecesarias, ya que perjudican el rendimiento al ejecutarse en segundo plano \[26 (76, 77), 31 (20)\]. |

### **FASE 2: CONVERSIÓN CRÍTICA (Ficha de Producto y Tallas)**

Esta fase se enfoca en resolver el principal punto de dolor de la indumentaria (*el ajuste incorrecto*) y proporcionar la información necesaria para que el cliente decida añadir al carrito \[19 (7, 32), 24 (33, 34)\].

| TICKET ID | Título del Ticket | Requisitos Cumplidos |
| ----- | ----- | ----- |
| **CON-001** | **Desarrollo del Sistema de Recomendación de Tallas** | **Criterio Gherkin Principal:** El sistema, basado en lógica difusa, debe **sugerir la mejor talla** después de que el usuario proporcione las medidas de su cuerpo (busto, cintura, cadera). **Historia de Usuario:** COMO Comprador de Indumentaria, QUIERO ingresar mis medidas corporales, PARA elegir la talla correcta y reducir el riesgo de devolución \[29 (1-3)\]. |
| **CON-002** | **Implementación de Guía de Tallas Detallada y Visual** | **Criterio Gherkin Secundario:** Debe estar accesible una **guía de tallas clara y detallada** que incluya medidas específicas \[14 (4, 5)\]. **Acción:** Asegurar que la guía de tallas es utilizada para reducir el riesgo de devolución \[3 (7, 8)\]. |
| **CON-003** | **Integración de Imágenes de Alta Calidad y Videos Ligeros** | **Historia de Usuario:** COMO Comprador Visual, QUIERO ver vídeos ligeros que muestren el producto en movimiento o *lifestyle* \[29 (2, 3)\], PARA facilitar mi decisión de compra \[29 (2, 3)\]. **Acción:** Asegurar imágenes de alta calidad con diferentes ángulos y detalles \[15 (4), 24 (18, 20)\]. |
| **CON-004** | **Desarrollo de Ficha de Producto con Información Completa y Certificaciones** | **Criterio Gherkin Principal:** El producto debe tener una **descripción completa** que incluya materiales, cuidados y **certificaciones** (como VEGANO o *eco-friendly*) \[15 (4, 8)\]. **Acción:** Incluir detalles técnicos relevantes, características de la suela y tipos de cierre \[5 (13), 24 (30)\]. |
| **CON-005** | **Integración de Módulo de Valoraciones y Reseñas (Prueba Social)** | **Criterio Gherkin Secundario:** Deben estar visibles las **valoraciones y reseñas** de los clientes (prueba social) \[15 (4, 9)\]. **Historia de Usuario:** COMO Cliente en una página de producto, QUIERO ver las valoraciones y reseñas de otros compradores, PARA generar credibilidad y tener mayor convicción \[29 (2, 3, 12)\]. |

### **FASE 3: OPTIMIZACIÓN DEL CHECKOUT Y GESTIÓN**

Esta fase aborda la fricción en el proceso de pago para evitar el abandono del carrito (60-80% de las veces) \[18 (6), 23 (7)\].

| TICKET ID | Título del Ticket | Requisitos Cumplidos |
| ----- | ----- | ----- |
| **CHK-001** | **Habilitación de la Opción "Pago como Invitado"** | **Criterio Gherkin Principal:** Puedo completar la compra seleccionando la opción de **"Pago como Invitado"** \[16 (7, 10, 12)\]. **Historia de Usuario:** COMO Comprador Impulsivo, QUIERO finalizar mi compra sin la obligatoriedad de crear una cuenta, PARA minimizar la fricción y evitar el abandono del carrito \[29 (2, 4, 5)\]. |
| **CHK-002** | **Implementación de Múltiples Opciones de Pago y Financiación** | **Criterio Gherkin Secundario:** Se deben ofrecer **múltiples opciones de pago seguras**, incluyendo la opción de **pago a plazos o financiación** \[16 (10, 12)\]. **Historia de Usuario:** COMO Cliente con presupuesto limitado, QUIERO tener acceso a opciones de pago a plazos o financiación, PARA facilitar el cierre de la venta de productos de alto precio \[29 (2, 4, 5)\]. |
| **CHK-003** | **Visibilidad del Resumen del Pedido y Certificados de Confianza** | **Criterio Gherkin Secundario:** El resumen del pedido debe ser **visible durante todo el proceso** para reforzar la confianza \[16 (10, 12)\]. **Acción:** Mostrar certificados de seguridad visibles (como SSL) y logotipos de medios de pago reconocidos \[23 (10)\]. |
| **CHK-004** | **Integración de Soporte en Tiempo Real durante el Checkout** | **Acción:** Contar con chat en vivo o soporte visible durante el *checkout* para resolver dudas y evitar abandonos \[11 (36), 19 (45), 25 (57)\]. |
| **CHK-005** | **Configuración de Gestión de Inventario y Pedidos (Backend)** | **Acción:** Implementar funciones para seguir las ventas y **gestionar el inventario y los pedidos** de manera efectiva \[22 (4), 31 (17, 18)\]. |

### **FASE 4: FIDELIZACIÓN Y CRECIMIENTO (Lifestyle y Comunidad)**

Esta fase se centra en vender el estilo de vida y fomentar la lealtad para aumentar la recurrencia \[17 (1, 2), 18 (8-10)\].

| TICKET ID | Título del Ticket | Requisitos Cumplidos |
| ----- | ----- | ----- |
| **FID-001** | **Desarrollo e Implementación del Programa de Membresía** | **Historia de Usuario:** COMO Cliente Leal de la Marca, QUIERO acceder a **lanzamientos exclusivos y beneficios** de un programa de membresía (ej. NikePlus), PARA fortalecer mi conexión emocional \[30 (10, 13-15)\]. **Acción:** Ofrecer acceso temprano a lanzamientos y beneficios exclusivos (descuentos, regalos) \[8 (9, 22), 25 (47, 49-51)\]. |
| **FID-002** | **Creación y Lanzamiento del Blog *Customer Centricity*** | **Historia de Usuario:** COMO Interesado en la salud, QUIERO acceder a un blog *customer centricity*, PARA encontrar **contenido de valor sobre bienestar, salud y ejercicio** \[30 (13-15)\]. **Acción:** Implementar una estrategia de *inbound marketing* centrada en el cliente \[18 (11, 12)\]. |
| **FID-003** | **Integración del Contenido Generado por el Usuario (UGC)** | **Historia de Usuario:** COMO Cliente que busca inspiración, QUIERO ver **Contenido Generado por el Usuario (UGC)** integrado en la ficha de producto, PARA ser atraído por el contenido *lifestyle* \[30 (3, 12, 14, 16)\]. **Acción:** Integrar fotos de clientes luciendo los productos (desde Instagram, por ejemplo) dentro de la ficha de producto \[24 (42)\]. |
| **FID-004** | **Fomento de la Comunidad Online** | **Historia de Usuario:** COMO Miembro de la comunidad, QUIERO conectarme con otros entusiastas (ej. Nike Run Club), PARA compartir logros y fortalecer mi vínculo emocional con la marca \[30 (15)\]. |
| **FID-005** | **Configuración de Email Marketing para Carrito Abandonado** | **Acción:** Implementar herramientas de email marketing (como Claviyo) para gestionar flujos esenciales como el **carrito abandonado** \[25 (58)\]. |

