# Color y tipografía — altima.str

> Guía: [Color y tipografía](../evaluacion/guias/fase-2-specs/05-color-y-tipografia.md)

## Paleta

| Rol | Color | HEX | Uso |
|---|---|---|---|
| Principal | Café oscuro | #3B2A20 | Logo, botones principales, navbar y títulos |
| Secundario | Azul marino | #1B2A41 | Fondos de secciones destacadas (hero, footer), botones secundarios y bordes |
| Acento | Rosa pastel | #F4C2C9 | Etiquetas de drop y stock ("Quedan 2"), contador del carrito, fondos de badges y detalles. Siempre con texto café o marino encima |
| Acento oscuro | Rosa viejo | #A8505F | Enlaces y textos en rosa sobre fondo claro, y etiquetas con texto blanco |
| Fondo | Hueso | #FAF6F1 | Fondo general del sitio y de las tarjetas |
| Texto | Café oscuro | #3B2A20 | Textos y párrafos |
| Texto suave | Café grisáceo | #6E625A | Bajadas, datos secundarios de producto y tiempo de lectura |
| Éxito | Verde | #2F6B3F | "Agregado al carrito", suscripción confirmada, sello "Original verificada" |
| Error | Rojo | #B3261E | Errores de formulario y aviso de "Agotada" |

Proporción (regla 60-30-10): 60 % hueso y café (fondo y texto), 30 % azul marino y 10 % rosa, que se guarda para lo que tiene que llamar la atención.

## Contraste

Calculado con la fórmula de WCAG (la misma que usa el verificador de WebAIM).

| Combinación | Ratio | Resultado |
|---|---|---|
| Texto café #3B2A20 sobre fondo hueso #FAF6F1 | 12.7:1 | AA ✅ |
| Texto suave #6E625A sobre fondo hueso #FAF6F1 | 5.5:1 | AA ✅ |
| Texto blanco sobre botón principal café #3B2A20 | 13.7:1 | AA ✅ |
| Texto blanco sobre azul marino #1B2A41 | 14.4:1 | AA ✅ |
| Rosa pastel #F4C2C9 sobre azul marino #1B2A41 (logo, títulos en hero) | 9.2:1 | AA ✅ |
| Texto café #3B2A20 sobre etiqueta rosa pastel #F4C2C9 | 8.7:1 | AA ✅ |
| Rosa pastel #F4C2C9 sobre fondo hueso #FAF6F1 | 1.5:1 | Solo detalles y fondos, nunca texto ❌ |
| Texto blanco sobre rosa pastel #F4C2C9 | 1.6:1 | No alcanza AA ❌ |
| Enlace rosa viejo #A8505F sobre fondo hueso #FAF6F1 | 4.9:1 | AA ✅ |
| Texto blanco sobre rosa viejo #A8505F | 5.3:1 | AA ✅ |
| Verde éxito #2F6B3F sobre fondo hueso #FAF6F1 | 5.9:1 | AA ✅ |
| Rojo error #B3261E sobre fondo hueso #FAF6F1 | 6.1:1 | AA ✅ |

El rosa pastel no sirve para texto sobre fondos claros ni como fondo de texto blanco. Por eso se suma el **rosa viejo #A8505F**, que mantiene el tono rosado de la marca y cumple AA en enlaces y etiquetas con texto blanco. El rosa pastel queda para fondos de etiquetas (con texto café) y para el logo sobre fondos oscuros.

## Tipografía

- **Títulos:** [Alfa Slab One](https://fonts.google.com/specimen/Alfa+Slab+One), slab serif muy gruesa y de impacto, con un solo peso (400). Se usa en el logo, títulos y nombres de drops.
- **Textos:** [Inter](https://fonts.google.com/specimen/Inter), sans serif muy legible en pantallas chicas. Se usa en párrafos, precios, filtros, formularios y botones.

| Elemento | Desktop | Mobile | Peso |
|---|---|---|---|
| h1 | 3.5rem | 2.25rem | 400 (Alfa Slab One) |
| h2 | 2.25rem | 1.75rem | 400 (Alfa Slab One) |
| h3 | 1.5rem | 1.25rem | 400 (Alfa Slab One) |
| Párrafo | 1rem | 1rem | 400 (Inter) |
| Botón | 1rem | 1rem | 600 (Inter, en mayúsculas) |

Alfa Slab One ya es muy pesada en 400, así que no lleva negrita. No se usa en párrafos ni en textos menores a 1.25rem, porque a ese tamaño sus remates se empastan.

## Justificación

La paleta nace de mezclar colores rudos, el café oscuro y el azul marino, que le dan a altima.str peso, calle y ese aire de pieza de colección de las gorras New Era. El rosa pastel dosifica esa rudeza: aparece poco, en etiquetas, drops y detalles, y eso es lo que le da identidad propia a la marca y la hace reconocible en el feed. Así la marca no se queda en un solo gusto: le habla al coleccionista que busca tonos sobrios y también al que quiere algo distinto. El fondo hueso evita el blanco frío y calza con lo cercano de la tienda.

Alfa Slab One es la fuente más llamativa que encontramos para el streetwear: es gruesa, ancha y con remates como la tipografía de las camisetas de béisbol y de los letreros de barrio, y se ve fuerte en una gorra, en un drop o en una historia de Instagram. Para que el sitio siga siendo fácil de leer, la acompaña Inter en los textos, de modo que Carlos pueda revisar precios, tallas y condiciones de envío sin esfuerzo desde su celular.
