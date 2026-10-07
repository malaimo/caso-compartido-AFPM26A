# T2 · Prompt de extracción

## Reglas de la corrida
- **Un solo prompt, fijo**, el mismo para todas las reuniones. Se congela antes de cerrar la clave y no se ajusta mirando ninguna transcripción del conjunto.
- Entrada: la transcripción completa de la reunión, tal como sale de Teams (no el recap actual de Teams).
- Se registra en `06-hoja-comparacion.csv` el modelo, su versión y la temperatura (0). Una corrida por reunión; no se elige "la mejor de varias".
- Si la salida no respeta el formato, se registra como falla de formato y se vuelve a correr una sola vez. Si falla de nuevo, todas las decisiones de esa reunión cuentan como faltantes.
- Si después de ver resultados se cambia el prompt, esta corrida no se repite con estas transcripciones: se prueba con transcripciones nuevas, como dice la regla de decisión.

## Prompt

```
Vas a leer la transcripción de una reunión de trabajo. Tu tarea es armar la lista de lo que quedó decidido al terminar la reunión.

Incluye:
- Decisiones: elecciones sobre alcance, plan, prioridad o forma de trabajar que la reunión dejó acordadas.
- Compromisos: tareas que una persona tomó o recibió en la reunión y que quedaron aceptadas.

No incluyas:
- Propuestas que nadie aceptó, o que recibieron una objeción que no se resolvió.
- Temas que quedaron para más adelante ("lo vemos después", "lo hablamos la próxima", "te digo").
- Observaciones o riesgos que solo se mencionaron.
- Versiones anteriores de algo que se cambió más tarde en la misma reunión. Incluye solo la versión final.

Para cada elemento indica:
- decision: qué se decidió, en una frase.
- responsable: la persona a cargo, con el nombre que aparece en la transcripción. Si nadie quedó a cargo, escribe "sin responsable". No lo deduzcas.
- fecha: el plazo tal como se dijo. Si no se dijo, escribe "sin fecha". No lo deduzcas.
- motivo: por qué se decidió, si se dijo, en pocas palabras. Si no se dijo, escribe "sin motivo".
- minuto: la marca de tiempo de la transcripción donde quedó cerrado.

Si una misma intervención decide dos cosas con distinto responsable, sepáralas en dos elementos.

Responde solo con una tabla en Markdown con estas columnas, en este orden, sin texto antes ni después:
| # | decision | responsable | fecha | motivo | minuto |

Fecha de la reunión: {fecha_reunion}

Transcripción:
{transcripcion}
```

## Qué recibe el líder en la revisión
La tabla tal como la devolvió la IA, sin la columna `minuto`, más la transcripción por si quiere consultarla. Ningún cambio de redacción de nuestra parte.
