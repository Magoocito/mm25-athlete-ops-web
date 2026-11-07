# MM25 — Híbrido Alto Rendimiento

El cliente elige horarios de fútbol publicados por el entrenador. Esta etapa refuerza componentes, props y estado en React, con prácticas evaluadas y Spec-Driven Development. El alumno intenta primero; hay pistas antes de la solución. No se avanza de fase automáticamente.

## Stack

React 19, TypeScript, Vite 8 y Tailwind 4 (`package.json`, `vite.config.ts`, `src/index.css`). Entrada: `index.html` → `src/main.tsx` → `src/App.tsx` (un título). En dependencias, sin uso en `src/`: `react-router-dom`, `axios`, `react-hook-form` y `zod`. Scripts: `dev`, `build`, `lint`, `preview`. No hay script de tests.

## Alcance

MM25 es independiente de Wix: sin SDK ni APIs de Wix. Servidor y datos propios quedan para después; la tecnología está pendiente. Independencia no significa hosting ni notificaciones gratis.

Un solo negocio. Fuera: multinegocio, chat, recompensas y eventos. Cupos reales, pagos, cancelación y lo no acordado siguen pendientes.

Planes acordados, todavía no implementados:

- Elite: S/300, 2 entrenamientos por semana, ciclo de 4 semanas, personalizado, evaluación y seguimiento.
- Alto Rendimiento: S/350 al mes, 3 clases por semana y 12 al mes, grupos reducidos, evaluación, seguimiento y recuperación. El anuncio dice que no son reprogramables.

No usar precios de la referencia ajena (S/500 y S/1200). Fase 1: datos de ejemplo, sin backend. Un rol en la interfaz no es seguridad.

## Estado

Implementación pendiente. Spec de fase 1: `docs/specs/001-horarios.md`.

## Cómo retomar

Móvil en la nube y laptop en el IDE se alinean con Git (commit, push y pull). Los archivos locales no se sincronizan solos.

## Metodología

Ciclo: spec, criterios, intento del alumno, pruebas, explicación y corrección. React y SDD se evalúan por separado. El estado se practica con [Full Stack Open](https://fullstackopen.com/en/part1/a_more_complex_state_debugging_react_apps). Especificar se practica con [MIT 6.031](https://web.mit.edu/6.031/www/sp21/classes/06-specifications/). No es un curso oficial de SDD con IA.

## Pregunta inicial

Para seleccionar un horario, ¿qué hay que guardar en el estado y qué puede seguir solo en la lista? Contesta antes de codear.
