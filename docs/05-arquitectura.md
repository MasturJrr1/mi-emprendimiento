# Arquitectura de la información — Altima.str

> Guía: [Arquitectura de la información](../evaluacion/guias/fase-1-requerimientos/05-arquitectura.md)

## Mapa de sitio

```text
Inicio (landing: drop destacado, formulario Drop List, últimos artículos)
│
├── Tienda (todas las gorras)
│   ├── Nuevos drops
│   ├── Fitted 59FIFTY
│   ├── Snapbacks y ajustables (9FIFTY / 9FORTY)
│   ├── Side patch y bordados
│   ├── Ediciones limitadas y colabs
│   ├── Resultados de búsqueda
│   ├── Ficha de producto
│   │   ├── Selector de talla + disponibilidad
│   │   ├── Fotos reales de autenticidad
│   │   ├── Calcular despacho
│   │   └── Consultar por WhatsApp
│   ├── Favoritos
│   └── Carrito
│       └── Checkout (prototipo)
│
├── Guía de tallas
│
├── Blog
│   ├── Tallas y cuidado
│   ├── Estilo y outfits
│   ├── Cultura y drops
│   ├── Autenticidad
│   └── Artículo (comentarios + compartir + productos relacionados)
│
├── Nosotros (quiénes somos y garantía de originalidad)
├── Contacto (WhatsApp, formulario e Instagram)
├── Preguntas frecuentes (tallas, envíos, cambios, autenticidad)
├── Cambios y devoluciones
├── Términos y condiciones
├── Política de privacidad
└── Página 404
```

**Navegación principal (menú):** Tienda · Nuevos drops · Guía de tallas · Blog · Contacto, con buscador, favoritos y carrito siempre visibles en el *header*.
**Footer:** Nosotros · Preguntas frecuentes · Cambios y devoluciones · Términos y condiciones · Política de privacidad · Instagram · WhatsApp.

## User flows

> Guía: [User flow](../evaluacion/guias/fase-1-requerimientos/06-user-flow.md)

### Flujo 1: compra

Matías ve en una historia de Instagram de Altima.str una gorra 59FIFTY de los Yankees en café con *side patch* y quiere comprarla en su talla.

```text
Historia de Instagram → toca el link
→ Inicio (landing) → ve el hero del drop → [Ver la tienda]
→ Tienda → abre la categoría "Side patch y bordados"
→ Filtra por equipo "New York Yankees" y color "Café"
→ Toca la gorra → Ficha de producto
→ Revisa las fotos reales de etiquetas y undervisor
→ ¿Conoce su talla?
    ├── Sí → elige "7 3/8"
    └── No → [Ver guía de tallas] → Guía de tallas → mide su cabeza (58,7 cm)
             → ve que es 7 3/8 → [Volver al producto] → elige "7 3/8"
→ ¿Hay stock en su talla?
    ├── Sí → ingresa su comuna en [Calcular despacho] → ve el precio final
    │        → [Agregar al carrito] → Carrito → revisa el total → [Ir a pagar] → Checkout (prototipo)
    └── No → [Avísame cuando vuelva] → deja su correo → sigue en la Tienda
```

### Flujo 2: contenido

Matías encuentra en Pinterest un pin del artículo "Cómo reconocer una New Era original" y termina comprando o consultando.

```text
Pin en Pinterest → toca el pin
→ Artículo "Cómo reconocer una New Era original: 6 detalles" (categoría Autenticidad)
→ Lee el artículo → [Compartir] por WhatsApp con un amigo
→ Deja un comentario preguntando por el sticker de la visera
→ Ve "Gorras de este artículo" al final
→ ¿Quiere comprar ya?
    ├── Sí → toca una gorra → Ficha de producto → elige talla → [Agregar al carrito] → Carrito
    └── No → [Únete a la Drop List] → deja su correo → recibe el aviso del próximo drop
→ Si tiene dudas → [Consultar por WhatsApp] → Contacto (chat de WhatsApp)
```

## Categorías

> Guía: [Categorías de productos y temas del blog](../evaluacion/guias/fase-1-requerimientos/07-categorias.md)

### Categorías de productos

| Categoría | Productos |
|---|---|
| Nuevos drops | Las últimas gorras que llegaron, de cualquier silueta (por ejemplo, 59FIFTY Chicago White Sox "Pink Undervisor", 9FIFTY Lakers en azul marino). |
| Fitted 59FIFTY | Gorras cerradas por talla (6 7/8 a 8) de MLB, NBA y NFL: Yankees, Dodgers, Red Sox, Bulls, Raiders, entre otras. |
| Snapbacks y ajustables | 9FIFTY (snapback, visera plana) y 9FORTY (ajustable, visera curva) para quienes no quieren preocuparse de la talla. |
| Side patch y bordados | Gorras con parches laterales conmemorativos (World Series, All-Star Game, aniversarios) y bordados especiales en el panel trasero o en la visera. |
| Ediciones limitadas y colabs | Colaboraciones de temporada y modelos de tiradas cortas (por ejemplo, colecciones exclusivas de tiendas de EE. UU. o colabs con marcas y artistas). |

*Además de las categorías, la tienda se puede filtrar por equipo o liga, talla, color, color del *undervisor* y precio.*

### Categorías del blog

| Categoría | Idea de artículo | Necesidad o motivación de la proto-persona | Producto relacionado |
|---|---|---|---|
| Tallas y cuidado | "Cómo saber tu talla de 59FIFTY con una huincha de medir (y qué hacer si estás entre dos tallas)" | Necesidad: comprar la talla correcta sin probársela. Frustración: equivocarse de talla. | Fitted 59FIFTY + Guía de tallas |
| Estilo y outfits | "5 outfits streetwear para combinar una gorra café (vistos en Pinterest)" | Motivación: armar su outfit con la gorra que cierra el *fit*. | Gorras en tonos café y rosa pastel |
| Cultura y drops | "¿Qué es un *side patch* y por qué esas gorras valen más?" | Motivación: exclusividad y coleccionismo; conocer la historia detrás de cada edición. | Side patch y bordados |
| Autenticidad | "Cómo reconocer una New Era original: 6 detalles que debes revisar antes de comprar" | Frustración: miedo a las réplicas y a los revendedores poco confiables. | Ediciones limitadas y colabs |
