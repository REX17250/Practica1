---
name: explain-code
description: Explica en lenguaje claro qué hace un archivo, función o fragmento de código de este proyecto. Úsalo cuando el usuario pida entender, documentar o le den contexto sobre código existente (por ejemplo "explica App.jsx", "qué hace esta función", "no entiendo este componente").
---

# Explain Code

Explica el código señalado (archivo, función, componente o fragmento seleccionado) de forma clara y directa, adaptada a alguien que está aprendiendo.

## Pasos

1. Si el usuario no especifica un archivo o fragmento concreto, pregunta cuál quiere que expliques o usa la selección activa del editor si existe.
2. Lee el archivo completo (no solo el fragmento) para entender el contexto: imports, props, estado y cómo se usa desde otros archivos.
3. Explica, en este orden:
   - **Propósito**: qué problema resuelve este código en una o dos frases.
   - **Flujo**: cómo entran los datos, qué transforma, qué devuelve o renderiza.
   - **Puntos clave**: decisiones no obvias (hooks usados, por qué ese estado, efectos secundarios, dependencias).
   - **Conexiones**: qué otros archivos lo usan o de qué dependen (props que recibe, funciones que invoca).
4. Si detectas un bug evidente mientras explicas, menciónalo brevemente al final como nota aparte — no lo arregles a menos que se pida.

## Estilo

- Usa español, directo y sin relleno.
- Evita repetir el código línea por línea; enfócate en el "por qué", no en narrar el "qué" (los nombres ya lo dicen).
- Usa referencias tipo `archivo.jsx:12` para señalar líneas específicas.
- Si el código es simple, la explicación debe ser corta (unas pocas líneas). No alargues explicaciones triviales.
