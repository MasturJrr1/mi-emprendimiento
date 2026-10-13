---
version: alpha
name: "altima.str"
description: "Design system de altima.str, tienda online de gorras New Era de colección y casuales para la comunidad streetwear en Chile."
colors:
  primary: "#3B2A20"
  primary-hover: "#2A1D16"
  on-primary: "#FFFFFF"
  secondary: "#1B2A41"
  on-secondary: "#FFFFFF"
  tertiary: "#F4C2C9"
  on-tertiary: "#3B2A20"
  tertiary-strong: "#A8505F"
  on-tertiary-strong: "#FFFFFF"
  neutral: "#FAF6F1"
  surface: "#FFFFFF"
  on-surface: "#3B2A20"
  on-surface-variant: "#6E625A"
  outline: "#D9D0C7"
  disabled: "#E6DFD8"
  on-disabled: "#5E544D"
  success: "#2F6B3F"
  on-success: "#FFFFFF"
  error: "#B3261E"
typography:
  headline-display:
    fontFamily: "Alfa Slab One"
    fontSize: 56px
    fontWeight: 400
    lineHeight: 1.05
  headline-lg:
    fontFamily: "Alfa Slab One"
    fontSize: 36px
    fontWeight: 400
    lineHeight: 1.15
  headline-md:
    fontFamily: "Alfa Slab One"
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.2
  title-sm:
    fontFamily: "Inter"
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.3
  body-md:
    fontFamily: "Inter"
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.6
  body-sm:
    fontFamily: "Inter"
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
  label-md:
    fontFamily: "Inter"
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1
  label-sm:
    fontFamily: "Inter"
    fontSize: 12px
    fontWeight: 600
    lineHeight: 1
rounded:
  sm: 4px
  md: 8px
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  2xl: 48px
  3xl: 64px
components:
  navbar:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-md}"
    height: 72px
    padding: 0 32px
  hero-drop:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-secondary}"
    typography: "{typography.headline-display}"
    padding: 64px 32px
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 12px 24px
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.on-primary}"
  button-primary-active:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-secondary}"
  button-primary-disabled:
    backgroundColor: "{colors.disabled}"
    textColor: "{colors.on-disabled}"
  button-secondary:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.primary}"
    typography: "{typography.label-md}"
    rounded: "{rounded.full}"
    padding: 12px 24px
  button-secondary-hover:
    backgroundColor: "{colors.neutral}"
    textColor: "{colors.primary}"
  link:
    backgroundColor: "{colors.neutral}"
    textColor: "{colors.tertiary-strong}"
    typography: "{typography.body-md}"
  chip-filter:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.full}"
    padding: 8px 16px
  chip-filter-hover:
    backgroundColor: "{colors.neutral}"
    textColor: "{colors.on-surface}"
  chip-filter-active:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-secondary}"
  input-field:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 12px 14px
  input-field-disabled:
    backgroundColor: "{colors.disabled}"
    textColor: "{colors.on-disabled}"
  tag-drop:
    backgroundColor: "{colors.tertiary}"
    textColor: "{colors.on-tertiary}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.full}"
    padding: 4px 10px
  tag-stock:
    backgroundColor: "{colors.tertiary-strong}"
    textColor: "{colors.on-tertiary-strong}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.full}"
    padding: 4px 10px
  card-product:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.title-sm}"
    rounded: "{rounded.md}"
    padding: "{spacing.md}"
  card-product-soldout:
    backgroundColor: "{colors.disabled}"
    textColor: "{colors.on-disabled}"
  badge-authentic:
    backgroundColor: "{colors.success}"
    textColor: "{colors.on-success}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.sm}"
    padding: 4px 8px
  card-article:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.title-sm}"
    rounded: "{rounded.md}"
    padding: "{spacing.md}"
  form-newsletter:
    backgroundColor: "{colors.tertiary}"
    textColor: "{colors.on-tertiary}"
    typography: "{typography.headline-md}"
    rounded: "{rounded.md}"
    padding: 48px 32px
  cart-summary:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: "{spacing.lg}"
  message-success:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.success}"
    typography: "{typography.body-sm}"
  message-error:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.error}"
    typography: "{typography.body-sm}"
  footer:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-secondary}"
    typography: "{typography.body-sm}"
    padding: 48px 32px
  page:
    backgroundColor: "{colors.neutral}"
    textColor: "{colors.on-surface}"
  text-secondary:
    backgroundColor: "{colors.neutral}"
    textColor: "{colors.on-surface-variant}"
---

# altima.str — Design system

## Overview

altima.str es una tienda online de gorras New Era originales: fitted de colección, ediciones especiales, colaboraciones y modelos casuales. Su usuario principal es Carlos, 25 años, estudiante y trabajador part-time que descubre gorras en Instagram y TikTok, compra desde el celular y quiere una gorra que lo diferencie, con la seguridad de que es original.

La interfaz debe sentirse como la tienda del amigo que sabe de gorras: coleccionable, urbana, auténtica y curada. Colores rudos (café oscuro y azul marino) dosificados con rosa pastel, títulos en una slab gruesa y mucho espacio para que la gorra sea la protagonista.

## Colors

- **Primary (#3B2A20) café oscuro:** logo, botones principales, títulos y texto. No se usa como fondo de secciones completas.
- **Secondary (#1B2A41) azul marino:** fondo del hero, del footer y de los chips activos. Sobre él el texto va en blanco o en rosa pastel.
- **Tertiary (#F4C2C9) rosa pastel:** etiquetas de drop, contador del carrito y fondo del formulario de novedades, siempre con texto café encima. Nunca como color de texto sobre fondos claros (1.5:1) ni con texto blanco encima (1.6:1).
- **Tertiary-strong (#A8505F) rosa viejo:** enlaces sobre fondo claro y etiquetas de stock ("Quedan 2") con texto blanco.
- **Neutral (#FAF6F1) hueso:** fondo general de todas las páginas.
- **Surface (#FFFFFF):** tarjetas, inputs, navbar y resumen del carrito.
- **On-surface-variant (#6E625A):** textos secundarios, como bajadas, silueta de la gorra y tiempo de lectura.
- **Success (#2F6B3F):** sello "Original verificada" y mensajes de confirmación.
- **Error (#B3261E):** errores de formulario y avisos de producto agotado.
- Proporción 60-30-10: 60 % hueso y blanco, 30 % azul marino y café, 10 % rosa.

## Typography

- **Títulos: Alfa Slab One** (solo peso 400, ya es muy gruesa). Se usa en el logo, h1, h2, h3 y nombre de los drops. Nunca en párrafos ni en tamaños menores a 20px.
- **Textos: Inter.** Párrafos, precios, filtros, formularios, etiquetas y botones.
- Escala: `headline-display` 56px (h1, en mobile 36px), `headline-lg` 36px (h2, en mobile 28px), `headline-md` 24px (h3, en mobile 20px), `title-sm` 16px (nombres de producto y artículo), `body-md` 16px (párrafos), `body-sm` 14px (datos secundarios), `label-md` 16px (botones, en mayúsculas) y `label-sm` 12px (etiquetas, en mayúsculas).

## Layout

- Ancho máximo del contenido: 1200px, centrado. Márgenes laterales de 32px en desktop, 24px en tablet y 16px en mobile.
- Espaciado en múltiplos de 4px usando la escala de `spacing`. Entre secciones: `3xl` (64px) en desktop y `2xl` (48px) en mobile.
- **Mobile (hasta 767px):** una columna. Navbar con logo, ícono de búsqueda y carrito; los enlaces van en un menú hamburguesa. Grilla de productos de 2 columnas. Filtros en un panel que se abre con el botón "Filtrar". En la ficha de producto, la galería va arriba y el botón "Agregar al carrito" queda fijo abajo. El resumen del carrito va bajo los productos.
- **Tablet (768 a 1023px):** grilla de productos y artículos de 2 columnas. Filtros en panel desplegable. Navbar completa.
- **Desktop (desde 1024px):** grilla de productos de 3 columnas con filtros en una columna izquierda de 240px. Blog en 3 columnas. Ficha de producto en 2 columnas (galería a la izquierda, información a la derecha). Carrito en 2 columnas (productos a la izquierda, `cart-summary` de 360px a la derecha).

## Elevation & Depth

- La jerarquía se marca con capas de color y bordes, no con sombras fuertes.
- Tarjetas e inputs llevan borde de 1px en `outline` (#D9D0C7) sobre el fondo hueso.
- Solo en hover, `card-product` y `card-article` suben 2px con una sombra suave (0 4px 12px, café al 12 %).
- El hero y el footer en azul marino marcan el inicio y el cierre de cada página.

## Shapes

- Botones, chips y etiquetas: `rounded.full` (forma de píldora).
- Tarjetas, inputs, formulario de novedades y resumen del carrito: `rounded.md` (8px).
- Sello "Original verificada": `rounded.sm` (4px).
- Las imágenes de producto son cuadradas (1:1) y las de artículos van en 16:9.

## Components

### Navbar (`navbar`)

Logo ALTIMA.STR en Alfa Slab One, enlaces Tienda, Colección, Novedades y Blog, buscador `input-field`, ícono de cuenta y carrito con contador en `tag-drop`. Debajo, una franja con "Envíos a todo Chile · 100% originales New Era".

- Siempre visible arriba (sticky).
- El contador del carrito solo aparece si hay al menos 1 producto.
- El enlace de la página actual va subrayado.

### Hero de drop (`hero-drop`)

Fondo azul marino, `tag-drop` con el nombre del drop, título en `headline-display` rosa pastel, bajada en blanco, `button-primary` "Ver el drop" y `button-secondary` "Ir a la tienda", e imagen grande de la gorra a la derecha.

- El título tiene máximo 5 palabras.
- Siempre muestra cuántas unidades quedan del drop.

### Botones (`button-primary`, `button-secondary`)

Texto en mayúsculas, `label-md`, forma de píldora, alto mínimo de 44px.

- Hover: `button-primary-hover` (café más oscuro).
- Active: `button-primary-active` (azul marino).
- Disabled: `button-primary-disabled`, por ejemplo cuando no se eligió talla.
- Máximo un `button-primary` por bloque.

### Enlace (`link`)

Texto en rosa viejo, subrayado en hover.

### Chips de filtro (`chip-filter`)

Categorías de la tienda (Todas, MLB, NBA, NFL, Colección, Colaboraciones, Novedades) y del blog.

- Hover: `chip-filter-hover`.
- Active: `chip-filter-active` (azul marino con texto blanco). Solo un chip activo a la vez.

### Campo de texto (`input-field`)

Buscador, correo y datos de envío. Borde de 1px en `outline`, que pasa a café de 2px al enfocar.

- Disabled: `input-field-disabled`.
- Si hay error, el borde va en `error` y se muestra un `message-error` debajo.

### Etiquetas (`tag-drop`, `tag-stock`)

- `tag-drop` (rosa pastel con texto café): "Colección", "Nueva", "Drop 004".
- `tag-stock` (rosa viejo con texto blanco): "Quedan 2", "Agotada".
- Siempre en mayúsculas y máximo 2 etiquetas por tarjeta.

### Product card (`card-product`)

Hasta 2 etiquetas, imagen cuadrada, nombre en `title-sm`, silueta en `body-sm` color `on-surface-variant`, precio en `title-sm` y `button-secondary` "Ver producto".

- El precio siempre es visible.
- El nombre ocupa máximo 2 líneas; si es más largo termina en "…".
- Agotada: `card-product-soldout`, imagen en escala de grises, `tag-stock` "Agotada" y el botón cambia a "Avisarme cuando vuelva".
- Hover: sube 2px con sombra y la imagen pasa a la foto de lado (side patch).

### Sello de autenticidad (`badge-authentic`)

Ícono de check y texto "Original verificada". Va en la ficha de producto, junto al botón de compra.

### Card de artículo (`card-article`)

Imagen 16:9, `tag-drop` con la categoría, título en `title-sm` (máximo 2 líneas) y tiempo de lectura en `body-sm`.

- Hover: sube 2px con sombra.
- Toda la tarjeta es clickeable.

### Formulario de novedades (`form-newsletter`)

Fondo rosa pastel, título en `headline-md` "Entérate primero de cada drop", bajada con la oferta (10 % en la primera gorra), `input-field` de correo, `button-primary` "Suscribirme", casilla de consentimiento y texto de privacidad.

- El botón queda deshabilitado hasta marcar el consentimiento.
- Al enviar se muestra `message-success` "Listo, te avisaremos del próximo drop".

### Resumen del carrito (`cart-summary`)

Selector de región y comuna para calcular el envío, subtotal, envío, total en `headline-md`, `button-primary` "Continuar con la compra" y `link` "¿Dudas? Escríbenos por WhatsApp".

- El total siempre incluye el envío calculado.
- Si el carrito está vacío, el botón queda deshabilitado.

### Mensajes (`message-success`, `message-error`)

Texto en `body-sm` con ícono, bajo el elemento que los genera. Siempre dicen qué pasó y qué hacer.

### Footer (`footer`)

Fondo azul marino. Arriba, tres sellos: 100% originales, Envíos a todo Chile y Pago seguro. Abajo, logo y frase "Pa' usar o pa' guardar.", redes (Instagram, TikTok, WhatsApp) y columnas de enlaces Tienda, Ayuda (Preguntas frecuentes, Guía de tallas, Contacto) y Legal (Términos, Privacidad).

## Do's and Don'ts

- **Do:** la gorra siempre es la protagonista; las fotos de producto ocupan el mayor espacio de cada tarjeta.
- **Do:** mostrar precio, talla y stock sin que Carlos tenga que preguntar por mensaje.
- **Do:** usar el rosa pastel solo como acento, en el 10 % de la pantalla.
- **Do:** escribir textos cortos, en tono chileno y cercano ("Pa' usar o pa' guardar", "Quedan 2").
- **Don't:** poner texto blanco o rosa pastel sobre fondos claros.
- **Don't:** usar Alfa Slab One en párrafos o en textos menores a 20px.
- **Don't:** usar logos de equipos como identidad de la marca; solo aparecen en las fotos de producto.
- **Don't:** fondos neón, degradados o más de dos tipografías.
