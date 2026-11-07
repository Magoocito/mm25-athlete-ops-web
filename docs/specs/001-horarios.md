# Spec 001 — Horarios de una fecha

Fase 1, datos de ejemplo y sin backend. No crea reserva ni cobra. Los datos van etiquetados como ficticios. No copiar nombres, sedes ni horarios reales, ni los de las capturas. Las capturas no se versionan.

## Evidencia de referencia (no es MM25)

Capturas de Spaces, «PRO Amateur Fútbol». No son requisitos de MM25.

Horarios: hay una fecha seleccionada y un listado con hora, duración, nombre, staff y ubicación. Botones vistos: Reservar y Completo. Aparece el indicador 26/28; su significado no está confirmado. No se observó el paso siguiente al reservar ni un panel del entrenador. No se infiere.

Planes: pestañas Club PRO, Reservas, Planes y Eventos, y precios S/500 (1 mes) y S/1200 (3 meses). Esos precios no se usan. La barra Mis sitios, Chat y Mi perfil queda fuera.

Daniel indica otras capturas con listado de negocios y filtro Todos, Administrador y Miembro. MM25 empieza con un solo negocio: se excluyen multinegocio, chat, recompensas y eventos.

## Decisión propuesta

El cliente elige entre horarios que publica el entrenador. En esta spec solo se listan sesiones de ejemplo de la fecha seleccionada. Cada sesión muestra hora, duración, nombre, entrenador, lugar y `cuposDisponibles` (entero explícito, no una fracción).

Si `cuposDisponibles` es 0, la etiqueta es «lleno» y no se puede seleccionar. Como máximo una selección, guardada en estado, más un resumen de la elegida. Elegir otra sesión con cupo sustituye la anterior y el resumen. No hay alta de reserva ni cobro.

## Criterios

1. Normal. Varias sesiones con cupo mayor que 0 muestran todos los campos. Elegir una actualiza el resumen con esa sesión.
2. Límite. Una sesión con `cuposDisponibles` en 0 muestra «lleno», no queda seleccionada y no admite selección.
3. Sin sesiones. La fecha no tiene sesiones: se ve que no hay horarios y no hay selección ni resumen.
4. Cambio. Con una sesión elegida, elegir otra con cupo reemplaza estado y resumen. La sesión llena sigue sin poder elegirse.

## Fuera de alcance

Planes Elite y Alto Rendimiento, pagos, cancelación, reprogramación, cupos reales, backend y el significado de 26/28.
