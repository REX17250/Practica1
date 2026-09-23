---
name: react-component
description: Genera un nuevo componente funcional de React para este proyecto (tienda-react), siguiendo las mismas convenciones que ProductCard.jsx y Cart.jsx (props destructuradas, sin TypeScript, clases CSS en App.css). Úsalo cuando el usuario pida crear un componente nuevo, una tarjeta, una sección o una vista dentro de src/.
---

# React Component (local)

Crea componentes de React consistentes con el estilo ya establecido en `src/` de este proyecto.

## Convenciones del proyecto (observadas en ProductCard.jsx y Cart.jsx)

- Function component declarado como `function Nombre({ propsDestructuradas }) { ... }`, con `export default Nombre` al final.
- Sin TypeScript, sin PropTypes: las props se documentan solo con nombres claros.
- JSX simple: sin fragmentos innecesarios, un elemento raíz semántico (`<article>`, `<aside>`, `<section>`, etc. — no abusar de `<div>`).
- Los estilos van como clases en `src/App.css` (no CSS-in-JS, no módulos `.module.css`, no Tailwind). El nombre de clase en kebab-case describe el bloque (`.card`, `.cart-item`, `.add-btn`).
- Los manejadores de eventos se reciben como props desde el padre (`onAdd`, `onRemove`, `onQty`), el componente hijo no maneja estado global ni hace fetch.

## Pasos al crear un componente nuevo

1. Preguntar (si no es obvio del pedido) qué props recibe y qué debe renderizar.
2. Crear el archivo `src/NombreComponente.jsx` siguiendo el patrón de arriba.
3. Agregar al final de `src/App.css` las clases CSS nuevas que use el componente, reutilizando variables de color/espaciado ya presentes en el archivo en vez de inventar nuevas si algo similar ya existe.
4. Si el componente necesita integrarse en `App.jsx`, mostrar también el cambio necesario en el import y en el JSX donde se monta, pero no modificar lógica de negocio existente sin que se pida.
5. No agregar librerías nuevas (sin styled-components, sin UI kits) — el proyecto es intencionalmente vanilla React + CSS plano.

## Estilo de respuesta

- Entrega el código directo, sin explicaciones largas salvo que el usuario pida entender decisiones.
- Si el pedido es ambiguo (por ejemplo qué datos recibe el componente), pregunta antes de inventar una API de props.
