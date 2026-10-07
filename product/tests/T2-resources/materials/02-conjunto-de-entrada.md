# T2 · Conjunto de transcripciones de entrada

## Qué entra
- Reuniones reales ya grabadas en Teams, con transcripción.
- Más de 5 participantes.
- Con al menos una decisión (según quien la aporta).
- Conducidas por un líder del pool de opt-in que dio su consentimiento, y con el permiso de su cuenta.
- Grabadas antes de empezar el test (nadie cambia su forma de conducir por el test).

## Cuántas
- 12 a 15 reuniones de 4 a 5 líderes (3 por líder como máximo, para que ningún estilo de conducción pese demasiado).
- Mínimo para leer el resultado: 30 decisiones en la clave. Objetivo: 40 o más. Si al terminar la clave hay menos de 40, se suman reuniones antes de correr la IA.

## Cómo se prepara cada transcripción
1. Se exporta la transcripción automática de Teams sin editar el texto. No se corrigen errores de reconocimiento de voz: la IA va a recibir lo mismo que recibiría en el producto.
2. Si el líder lo pide, se reemplazan nombres de personas externas y de clientes por nombres ficticios, de forma consistente en todo el archivo.
3. Se guarda con un id (`R01`, `R02`, …), fecha de la reunión, duración y cantidad de participantes en el encabezado.
4. Se registra en el inventario de abajo. El archivo con la relación entre id, líder y cuenta queda fuera de esta carpeta.

## Inventario

| id | líder (código) | fecha | duración | participantes | procedencia | consentimiento | decisiones en la clave |
|---|---|---|---|---|---|---|---|
| R1 | (a confirmar) | 2026-10-01 | 42 min | 7 | (a confirmar) | (a confirmar) | |
| R2 | (a confirmar) | 2026-10-02 | 38 min | 9 | (a confirmar) | (a confirmar) | |
| R3 | (a confirmar) | 2026-10-05 | 55 min | 8 | (a confirmar) | (a confirmar) | |
| … | | | | | | | |

R1 a R3 son los archivos de `product/tests/T2-resources/`. Procedencia: `real` si es una grabación de un líder del pool; cualquier otra cosa se marca como tal y no cuenta para el resultado `real` del test.
