# T2 · Clave a ciegas: procedimiento y reglas de anotación

La clave es la lista de respuestas correctas contra la que se compara la IA. La arman dos personas, cada una por su lado, **sin ver nunca la salida de la IA** (ni de esa reunión ni de ninguna otra). La salida de la IA se genera recién cuando la clave de todas las reuniones está cerrada.

## Procedimiento
1. Las dos personas leen estas reglas y anotan juntas una reunión de práctica que **no** forma parte del conjunto, para alinear criterios. No se toca nada de las reglas después de este paso.
2. Cada una anota cada transcripción por separado en su copia de `04-clave-plantilla.csv`.
3. Se juntan las dos anotaciones. Lo que coincide entra a la clave. Lo que no coincide (una persona lo marcó y la otra no, o distinto responsable, fecha o tipo) se anota como desacuerdo.
4. El líder de esa reunión resuelve cada desacuerdo (unos 15 minutos). Su respuesta es la final. El líder solo ve los puntos en desacuerdo, no la clave completa.
5. Se registra cuántos puntos hubo en desacuerdo por reunión (sirve para saber qué tan clara es la definición de decisión).

## Qué cuenta como decisión
Una entrada de la clave es algo que, **al terminar la reunión**, quedó acordado y cambia lo que alguien va a hacer o lo que el equipo va a hacer. Incluye:
- **Decisión:** una elección sobre alcance, plan, prioridad o forma de trabajar ("la exportación a PDF pasa al 3.5", "todo incidente entra solo por el portal").
- **Compromiso:** una tarea que alguien toma o recibe en la reunión, aceptada ahí ("Iván le pasa la lista completa a Paula hoy").

Las dos cuentan en el denominador. Se marca el tipo en la columna `tipo` para poder separarlas en el análisis.

## Qué NO cuenta como decisión
Se anota igual en la clave, con `tipo = no-decision`, para poder reconocerlo si la IA lo presenta como decisión:
- **Propuesta no adoptada:** alguien propone y nadie con autoridad la acepta, o hay una objeción que queda sin resolver ("propongo que los viernes no haya despliegues" seguido de un "no estoy de acuerdo").
- **Tema postergado:** "lo vemos después", "lo hablamos la próxima", "déjame revisar y te digo".
- **Observación o riesgo:** "anotemos que hay riesgo en QA".
- **Decisión reemplazada en la misma reunión:** la versión anterior de algo que se cambió más tarde (ver abajo).

Solo se anotan como `no-decision` los puntos que alguien podría confundir con una decisión. No hace falta anotar cada comentario.

## Casos frecuentes
- **Cambio durante la reunión:** si algo se decide y después se cambia, la clave tiene una sola decisión con la versión final. La versión anterior va como `no-decision`.
- **Una frase, varias decisiones:** si una misma intervención decide dos cosas con distinto responsable, son dos entradas ("la migración se mueve al martes, Hernán a cargo" y "Natalia avisa a los clientes grandes").
- **Votación que elige temas:** si se elige qué temas trabajar y después cada tema se convierte en una acción con responsable, se anotan solo las acciones. No se cuenta la elección por separado.
- **Responsable:** la persona que queda a cargo. Si se nombra a alguien que ayuda, el responsable sigue siendo el primero. Si el responsable es alguien externo (un cliente), se anota igual. Si no quedó nadie a cargo, se escribe `sin responsable`.
- **Fecha:** se copia como se dijo ("el viernes", "mañana", "en la semana") y, cuando se puede, se agrega la fecha calendario según la fecha de la reunión. Si no se dijo, se escribe `sin fecha`.
- **Motivo:** se anota si se dijo, en pocas palabras. Si no se dijo, `sin motivo`. El motivo no se usa para decidir si una extracción es correcta (ver `08-calculo-del-resultado.md`).
- **Minuto:** el momento de la transcripción donde la decisión queda cerrada. Sirve para comparar después.

## Formato
Una fila por entrada en `04-clave-plantilla.csv`. Una copia por persona y por reunión, y una clave final por reunión.
