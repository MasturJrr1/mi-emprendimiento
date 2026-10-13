# Spec de desarrollo — altima.str

> Guía: [Spec de desarrollo](../evaluacion/guias/fase-2-specs/07-spec-de-desarrollo.md)

## Insumos y prompt para el asistente

```text
Lee DESIGN.md, docs/09-spec-diseno.md y docs/10-spec-desarrollo.md.
En la carpeta stitch/ está el código exportado de Stitch de cada pantalla.
Construye el sitio siguiendo exactamente docs/10-spec-desarrollo.md:
solo HTML y CSS, la estructura de archivos y la navegación definidas,
las variables de :root con los valores de DESIGN.md y la estructura
semántica de cada página. Usa el código de Stitch solo como referencia
visual. Al terminar, revisa cada criterio de aceptación y dime cuáles
se cumplen y cuáles no.
```

## 1. Estructura de archivos

```text
mi-emprendimiento/
├── index.html              ← landing
├── tienda.html
├── producto.html
├── carrito.html
├── blog.html
├── articulo.html
├── nosotros.html           ← sobre altima.str
├── contacto.html
├── preguntas-frecuentes.html
├── terminos.html
├── privacidad.html
├── 404.html
├── DESIGN.md
├── css/
│   └── styles.css
├── img/
│   ├── productos/
│   └── blog/
├── stitch/                 ← código exportado de Stitch (solo referencia)
└── docs/
```

## 2. Páginas y navegación

- Navbar en todas las páginas: logo (lleva a index.html), Tienda, Colección, Novedades, Blog, buscador y carrito.
- Colección y Novedades no son páginas aparte: llevan a tienda.html con esa categoría marcada.
- Footer en todas las páginas: Tienda, Preguntas frecuentes, Guía de tallas, Contacto, Nosotros, Términos, Privacidad e Instagram.

| Desde | Elemento | Lleva a |
|---|---|---|
| index.html | Botón "Ver el drop" del hero | tienda.html (categoría Colección) |
| index.html | Botón "Ir a la tienda" del hero | tienda.html |
| index.html | Card de producto en Novedades | producto.html |
| tienda.html | Botón "Ver producto" de cada card | producto.html |
| producto.html | Botón "Agregar al carrito" | carrito.html |
| producto.html | Enlace "Guía de tallas" | preguntas-frecuentes.html |
| carrito.html | Enlace "Seguir comprando" | tienda.html |
| carrito.html | Botón "Continuar con la compra" | Muestra el mensaje "Pronto podrás pagar online" (el pago no está en esta versión) |
| carrito.html | Enlace "¿Dudas? Escríbenos por WhatsApp" | https://wa.me/569XXXXXXXX |
| blog.html | Card de artículo | articulo.html |
| articulo.html | Botón "Ver gorra" | producto.html |
| articulo.html | Cards de "Sigue leyendo" | articulo.html |
| Cualquier página | Enlace que no existe | 404.html |

## 3. Estructura semántica

Todas las páginas tienen la misma base: `<header>` con la navbar, un `<main>` y un `<footer>`.

### index.html

```html
<header> → navbar
<main>
  <section> hero del drop (h1 "Curado pa' la calle")
  <section> novedades (cada card es un <article>)
  <section> formulario de novedades (<form>)
</main>
<footer>
```

### tienda.html

```html
<header> → navbar
<main>
  <section> h1 "Tienda" + buscador + chips de categoría
  <aside>   filtros (silueta, talla, precio)
  <section> grilla de product cards (cada card es un <article>)
</main>
<footer>
```

### producto.html

```html
<header> → navbar
<main>
  <nav>     migas (Tienda / MLB / Yankees)
  <section> galería de fotos
  <section> h1 nombre, precio, talla, botón y sello "Original verificada"
  <section> "También te puede gustar" (cards en <article>)
</main>
<footer>
```

### carrito.html

```html
<header> → navbar
<main>
  <section> h1 "Tu carrito" + lista de productos
  <aside>   resumen del carrito con envío y total
</main>
<footer>
```

### blog.html

```html
<header> → navbar
<main>
  <section> h1 "Blog" + chips de categoría
  <section> grilla de cards de artículo (cada una es un <article>)
</main>
<footer>
```

### articulo.html

```html
<header> → navbar
<main>
  <article> h1, fecha, imagen y texto del artículo
    <section> "La gorra de este look" (producto relacionado)
    <section> compartir
  </article>
  <section> "Sigue leyendo"
</main>
<footer>
```

Las páginas de nosotros, contacto, preguntas frecuentes, términos, privacidad y 404 usan la misma base, con un `h1` y el contenido en `<section>`.

## 4. Organización del CSS

Todo va en un solo archivo, `css/styles.css`. Las fuentes (Alfa Slab One e Inter) se cargan desde Google Fonts.

```css
:root {
  /* los valores salen de DESIGN.md */

  /* Colores */
  --color-primary: #3B2A20;        /* café oscuro */
  --color-primary-hover: #2A1D16;
  --color-secondary: #1B2A41;      /* azul marino */
  --color-accent: #F4C2C9;         /* rosa pastel */
  --color-accent-strong: #A8505F;  /* rosa viejo */
  --color-bg: #FAF6F1;             /* hueso */
  --color-surface: #FFFFFF;
  --color-text: #3B2A20;
  --color-text-soft: #6E625A;
  --color-border: #D9D0C7;
  --color-disabled: #E6DFD8;
  --color-success: #2F6B3F;
  --color-error: #B3261E;

  /* Tipografía */
  --font-title: 'Alfa Slab One', serif;
  --font-body: 'Inter', sans-serif;

  /* Espaciados */
  --space-xs: 4px;
  --space-sm: 8px;
  --space-md: 16px;
  --space-lg: 24px;
  --space-xl: 32px;
  --space-2xl: 48px;
  --space-3xl: 64px;

  /* Radios */
  --radius-sm: 4px;
  --radius-card: 8px;
  --radius-pill: 9999px;
}
```

- Clases en inglés con guiones, con los mismos nombres de los componentes de `DESIGN.md`: `.navbar`, `.hero-drop`, `.btn-primary`, `.btn-secondary`, `.chip-filter`, `.tag-drop`, `.tag-stock`, `.product-card`, `.article-card`, `.cart-summary`, `.footer`.
- Breakpoints: mobile hasta 767 px, tablet desde 768 px y desktop desde 1024 px.
- Se diseña primero para mobile (mobile first).

## 5. Criterios de aceptación

**Navegación**
- [ ] La navbar y el footer son iguales en todas las páginas.
- [ ] Se puede completar el flujo de compra: landing → tienda → producto → carrito.
- [ ] Se puede completar el flujo de contenido: blog → artículo → producto.
- [ ] Están las 12 páginas de la estructura de archivos.
- [ ] No hay enlaces rotos.

**Funcionalidades**
- [ ] La landing tiene el hero del drop y un formulario de correo con la oferta del 10 %.
- [ ] La tienda tiene buscador, chips de categoría (MLB, NBA, NFL, Colección, Colaboraciones, Novedades) y filtros por silueta, talla y precio.
- [ ] La tienda tiene una sección de gorras de colección y ediciones especiales.
- [ ] La ficha de producto muestra fotos, precio, selector de talla, stock, sello "Original verificada", costo de envío y botón "Agregar al carrito".
- [ ] El carrito muestra subtotal, envío y total antes de comprar.
- [ ] El artículo muestra la gorra del look con un botón que lleva a la ficha de producto.

**Diseño**
- [ ] Todos los colores del CSS salen de las variables de `:root`, con los valores de `DESIGN.md`.
- [ ] Los títulos usan Alfa Slab One y los textos, Inter.
- [ ] El sitio usa solo HTML y CSS propios (sin Tailwind ni el CSS exportado de Stitch).
- [ ] El precio es visible en todas las product cards.
- [ ] Ningún texto va en blanco o en rosa pastel sobre fondo claro.
- [ ] Los botones tienen estado hover.

**Responsive**
- [ ] En mobile la tienda muestra 2 productos por fila; en tablet, 2; en desktop, 3.
- [ ] En mobile los enlaces de la navbar van en un menú hamburguesa.
- [ ] No hay scroll horizontal en 375 px de ancho.

**Accesibilidad y publicación**
- [ ] Todas las imágenes tienen `alt` descriptivo (por ejemplo, "Gorra Yankees 59FIFTY negra con undervisor verde").
- [ ] Cada página tiene un solo `h1`.
- [ ] Los botones y enlaces tienen al menos 44 px de alto en mobile.
- [ ] El sitio está publicado en GitHub Pages.
