# Tecnologías del proyecto — Altima.str

> Guía: [Tecnologías del proyecto](../evaluacion/guias/fase-1-requerimientos/04-tecnologias.md)

## Stack

| Área | Herramienta | Para qué la uso |
|---|---|---|
| Construcción | HTML + CSS | Maquetar las páginas del sitio (landing, tienda, ficha, carrito, blog y artículo) sin frameworks ni gestor de contenido, con diseño *mobile first* porque Matías llega desde el celular. |
| Versionado | Git y GitHub | Guardar el historial de cambios de la documentación, las specs y el código, y entregar cada fase con commits descriptivos. |
| Publicación | GitHub Pages | Publicar el sitio gratis con un link que se pueda poner en la bio de Instagram de Altima.str. |
| Diseño | Whimsical | Armar el moodboard, calcar componentes de referentes (New Era, Hat Club) y dibujar los wireframes. |
| Diseño | Google Stitch | Generar el prototipo referencial en desktop y mobile a partir del `DESIGN.md`. |
| IA | Claude Code | Generar borradores de la documentación y las specs a partir de mis decisiones, y luego apoyar el paso a código. |
| Editor | GitHub (web) / VS Code | Editar los archivos Markdown y, en la etapa de código, el HTML y el CSS. |

## Qué es funcional y qué es prototipo

| Funcionalidad | Estado en esta versión |
|---|---|
| Navegación entre páginas (landing, tienda, categorías, ficha, blog, artículo, páginas legales) | Funcional |
| Guía de tallas (tabla de equivalencias cm ↔ talla New Era) | Funcional (contenido estático) |
| Consultar por WhatsApp (link `wa.me` con mensaje predefinido) | Funcional |
| Compartir un artículo (links de compartir de WhatsApp, X y Pinterest) | Funcional |
| Navegar el blog por categoría | Funcional (una página por categoría) |
| Formulario de la Drop List | Prototipo visual (sin guardar correos) |
| Buscar gorras | Prototipo visual |
| Filtrar gorras | Prototipo visual (las categorías sí son links funcionales) |
| Elegir talla y agregar al carrito | Prototipo visual |
| Carrito y pago | Prototipo visual |
| Calcular despacho por comuna | Prototipo visual |
| Comentar un artículo | Prototipo visual |
| Favoritos y aviso de reposición de stock | Prototipo visual |

## Integraciones para una versión real

- **Pasarela de pago chilena:** Webpay Plus (Transbank), Mercado Pago o Flow, para pagar con débito, crédito o saldo de Mercado Pago.
- **Plataforma de e-commerce o backend:** para el carrito, el stock por talla y los pedidos (por ejemplo, Shopify, WooCommerce o Jumpseller).
- **Despacho:** cálculo de tarifas y seguimiento con Starken, Chilexpress o Blue Express.
- **Email marketing:** Mailchimp o Brevo para la Drop List y los avisos de reposición.
- **WhatsApp Business:** atención y consultas de talla.
- **Instagram:** feed embebido y etiquetado de productos (Instagram Shopping).
- **Comentarios del blog:** un servicio externo como Disqus o Giscus.
- **Boleta electrónica:** emisión según el SII.

## Restricciones

- **Plazo:** Fase 1 hasta el 5 de octubre, specs hasta el 12 de octubre y prototipo en Stitch hasta el 14 de octubre de 2026. El código HTML + CSS se hace en la siguiente etapa del curso.
- **Marca:** la identidad visual usa **rosa pastel, café y azul marino**. Altima.str es revendedor: puede nombrar New Era y sus siluetas, pero no usar su logo como marca propia. Las fotos de producto deben ser propias.
- **Dispositivos:** diseño *mobile first*; la mayoría de las visitas llegarán desde el celular a través de Instagram y Pinterest. También debe verse bien en tablet y desktop.
- **Técnicas:** sin JavaScript ni backend en esta etapa, por lo que el pago, el carrito, la búsqueda y los comentarios quedan como prototipo.
- **Precios:** en pesos chilenos (CLP), con IVA incluido.
