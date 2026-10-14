# Arquitectura de la información — altima.str

> Guía: [Arquitectura de la información](../evaluacion/guias/fase-1-requerimientos/05-arquitectura.md)

## Mapa de sitio

```text
Inicio (landing)
├── Tienda
│   ├── Todas las gorras
│   ├── Gorras por equipo
│   │   ├── MLB
│   │   ├── NBA
│   │   └── NFL
│   ├── Gorras de colección
│   ├── Colaboraciones y ediciones especiales
│   ├── Novedades
│   └── Detalle del producto
│       ├── Fotografías
│       ├── Precio y características
│       ├── Disponibilidad
│       └── Agregar al carrito
├── Carrito de compras
│   └── Resumen del pedido
├── Blog
│   ├── Streetwear y tendencias
│   ├── Cultura de las gorras
│   ├── Guías de estilo
│   └── Colecciones y lanzamientos
├── Sobre altima.str
├── Contacto
├── Preguntas frecuentes
├── Términos y condiciones
├── Política de privacidad
└── Página 404 (página no encontrada)
```

## User flows

> Guía: [User flow](../evaluacion/guias/fase-1-requerimientos/06-user-flow.md)

### Flujo 1: compra

```text
Inicio
  ↓
Entrar a la tienda
  ↓
Explorar categorías o buscar una gorra
  ↓
Aplicar filtros según preferencias
  ↓
Seleccionar un producto
  ↓
Revisar fotografías, precio y características
  ↓
¿El producto cumple sus expectativas?
  ├── No → Volver al catálogo
  └── Sí
       ↓
Agregar al carrito
       ↓
Revisar el resumen del pedido
       ↓
Continuar a la compra
       ↓
Ingresar datos de envío y seleccionar medio de pago
       ↓
Confirmar pedido
       ↓
Compra finalizada
```

*Nota: los pasos de carrito, pago y confirmación representan el flujo esperado para una versión comercial. Solo estarán operativos cuando se implementen las integraciones correspondientes.*

### Flujo 2: contenido

```text
Inicio
  ↓
Entrar al blog
  ↓
Explorar categorías de contenido
  ↓
Seleccionar un artículo
  ↓
Leer el contenido
  ↓
¿Encuentra información de su interés?
  ├── No → Volver al blog y explorar otros artículos
  └── Sí
       ↓
Consultar productos relacionados
       ↓
Seleccionar una gorra
       ↓
Revisar el producto en la tienda
       ↓
Agregar al carrito o continuar explorando
```

## Categorías

> Guía: [Categorías de productos y temas del blog](../evaluacion/guias/fase-1-requerimientos/07-categorias.md)

### Categorías de productos

| Categoría | Productos |
|---|---|
| Gorras MLB | Modelos New Era de equipos de las Grandes Ligas de Béisbol, como Yankees, Dodgers y Red Sox. |
| Gorras NBA | Modelos relacionados con equipos de la NBA, según disponibilidad del catálogo. |
| Gorras NFL | Modelos relacionados con equipos de la NFL, según disponibilidad del catálogo. |
| Gorras de colección | Modelos especiales, ediciones limitadas y diseños buscados por coleccionistas. |
| Colaboraciones y ediciones especiales | Gorras pertenecientes a colaboraciones oficiales y colecciones especiales disponibles. |
| Novedades | Modelos incorporados recientemente al catálogo. |

### Categorías del blog

| Categoría | Idea de artículo | Necesidad o motivación de la proto-persona | Producto relacionado |
|---|---|---|---|
| Streetwear y tendencias | Cómo combinar una gorra New Era con un outfit urbano | Quiere expresar su estilo personal y diferenciarse mediante su vestimenta. | Gorras MLB y modelos clásicos |
| Cultura de las gorras | Por qué las gorras New Era son un referente de la moda urbana | Busca conocer la historia y el significado cultural de las gorras que utiliza. | Gorras clásicas de equipos deportivos |
| Guías de estilo | Cómo elegir una gorra según tu estilo y la forma en que te gusta usarla | Necesita orientación para escoger un modelo que combine con su ropa. | Diferentes modelos y estilos de gorras |
| Colecciones y lanzamientos | Qué debes saber antes de comprar una gorra de colección | Quiere descubrir modelos especiales y conocer sus características antes de comprar. | Gorras de colección y ediciones especiales |
| Cuidado de productos | Cómo limpiar y conservar una gorra para mantenerla en buen estado | Quiere proteger su compra y prolongar la vida útil de su gorra. | Gorras New Era del catálogo |
| Equipos y cultura deportiva | Cómo elegir una gorra según tu equipo favorito | Busca representar sus gustos deportivos mediante un accesorio. | Gorras MLB, NBA y NFL |

## Criterios de organización

- **Navegación sencilla:** las secciones principales estarán disponibles desde el menú para que el usuario pueda acceder rápidamente a la tienda, el blog y el contacto.
- **Catálogo organizado:** los productos se agruparán por equipos, colecciones y novedades para facilitar la búsqueda.
- **Información clara:** cada producto tendrá su propia ficha con fotografías, precio, características y disponibilidad.
- **Contenido relacionado:** los artículos del blog podrán dirigir al usuario hacia productos vinculados con sus intereses.
- **Confianza y transparencia:** las páginas de contacto, preguntas frecuentes, términos y privacidad ayudarán a resolver dudas y comunicar las condiciones de compra.
- **Diseño adaptable:** la estructura estará pensada para funcionar en celulares, tablets y computadores.
