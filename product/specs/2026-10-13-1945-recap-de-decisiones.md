---
feature: recap-de-decisiones
opportunity: decisiones-sin-cierre-en-reuniones
solutions: product/solutions/2026-09-29-2055-decisiones-sin-cierre-en-reuniones.md
tests: product/tests/2026-10-06-1914-decisiones-sin-cierre-en-reuniones.md
status: approved
---

# Recap de IA centrado en decisiones

## Problem

En las reuniones de más de 5 participantes, el recap de IA resume la conversación, no las decisiones: pone todo al mismo nivel, no dice quién se comprometió a qué y a veces marca propuestas como decisiones. Por eso el líder lo reescribe o arma el acta a mano (10 a 60 minutos, y "nadie más lo hace"), y cuando el equipo lee solo el recap, lo decidido se ejecuta distinto o tarde, con costos de días o semanas. Importa ahora porque el recap es lo que hoy se cobra en el plan superior y, tal como está, genera trabajo en vez de ahorrarlo.

> Evidencia: "El recap resume todo al mismo nivel. Dos páginas. No distingues qué se decidió de qué se comentó." (Javier Molina, `real`, product/interviews/2026-09-28-0900-javier-molina.md). En su planning, la dependencia acordada con fecha quedó como "se habló de la API de geocercas" y se entregó 2 semanas tarde.
> Evidencia: "marca como decisión cosas que eran solo ideas." Paula mandó el resumen al canal sin leerlo bien y el squad arrancó una integración que nadie había aprobado: 1 semana de 2 desarrolladores (Paula Benítez, `real`, product/interviews/2026-09-28-1400-paula-benitez.md).
> Evidencia: 6 de 10 entrevistados usan o probaron el recap y ninguno lo usa como registro de decisiones; 8 de 10 hacen trabajo manual posterior (`real`, n=10, product/insights/2026-09-29-2000-entrevistas-colaboracion-en-vivo-fuera-de-teams.md). 26 de 32 respuestas "Otro" sobre dónde quedó lo decidido son el recap, casi siempre con salvedad: "resume todo pero no distingue lo decidido" (`survey`, n=182, product/insights/2026-09-29-1931-colaboracion-en-vivo-fuera-de-teams.md).

## Who it's for

- **Joaquín Lemus** (primary, segmento en foco): sus decisiones terminan en un hilo de Slack que Teams no ve y Madrid ya implementó dos veces una versión anterior de un acuerdo.
- **Carolina Restrepo** (primary): pasa 30 a 45 minutos después de cada refinamiento copiando decisiones al acta y a Jira.
- **Rosa Elena Cabrera** (tertiary, quien recibe): quiere salir de la reunión sabiendo qué le toca y para cuándo; hoy "nadie escribe qué se decidió".

## User journey

Desde el punto de vista de Joaquín:

1. **Trigger:** termina el refinamiento semanal con 9 personas en Ciudad de México, Medellín y Madrid. Se decidieron tres cosas sobre el tablero de Jira compartido en pantalla y se descartó una propuesta.
2. **Hoy:** alguien del equipo abrió un hilo de Slack durante la reunión; el recap de Teams sale como resumen de la conversación y nadie lo usa como registro (persona `synthetic`; mismo patrón en Javier y Martina, `real`).
3. **Aviso:** al terminar la reunión, Joaquín ve en el chat de la reunión que la lista de decisiones está lista para revisar. Nadie más la ve todavía.
4. **Lectura:** abre la lista. Arriba, las decisiones con responsable, fecha y motivo. Aparte, las propuestas y los temas que quedaron abiertos. Cada ítem muestra la frase y el minuto de la transcripción de donde salió.
5. **Revisión:** corrige un responsable que la IA dejó como "sin responsable" y pasa a propuestas un "podríamos mover el release" que estaba como decisión (el error de Paula, `real`). Una decisión dice "Grafana: ese pico se investiga" y aparece marcada como "falta contexto de pantalla"; Joaquín escribe a qué gráfico se refería. Le lleva unos minutos, no la media hora del acta.
6. **Publicación:** publica la lista revisada en el chat de la reunión, donde la ven todos los invitados, incluidos los de Madrid y quienes no hablaron. Después copia la lista con un clic y la pega en la página de Confluence del equipo; los códigos de ticket que se dijeron en voz alta ya vienen como enlace.
7. **Outcome:** el equipo de Madrid lee una única lista revisada por Joaquín, con quién hace qué y para cuándo, en lugar del hilo equivocado. Joaquín no escribe acta ni reescribe el recap. **El valor llega en el paso 6.**

Lo que el viaje no cubre: publicar la lista sola en Jira, Confluence o Slack (A3, aparcada). La spec ofrece solo una salida manual (copiar y pegar en un paso). Si aun así Joaquín sigue reescribiendo la lista en Confluence, el ahorro se achica (ver creencia 15).

## Critical user stories

### Ver solo lo que se decidió, separado de lo que se conversó
Como Joaquín, quiero una lista de decisiones con responsable, fecha y motivo, separada de las propuestas y temas abiertos, para saber qué quedó decidido sin reescribir el recap.

Criterios de aceptación:
- [ ] Al terminar una reunión grabada o transcrita, la lista aparece en el mismo lugar donde hoy aparece el recap.
- [ ] Cada decisión muestra cuatro campos: decisión, responsable, fecha y motivo.
- [ ] Si en la reunión no se nombró responsable o fecha, el campo dice "sin responsable" o "sin fecha"; la IA nunca completa uno que no se dijo.
- [ ] Las propuestas no adoptadas y los temas postergados aparecen en una sección aparte, con otro título.
- [ ] Si en la reunión no se decidió nada, la lista dice "No se detectaron decisiones" y no inventa ninguna.
- [ ] Si en la reunión se dice en voz alta un código de ticket (por ejemplo "OPS-214") ligado a una decisión, la decisión lo muestra como enlace al ticket cuando la cuenta tiene configurada la dirección de su Jira, y como texto destacado cuando no.

Se apoya en: "El resumen de IA resume la conversación, no las decisiones, y a veces inventa decisiones" (product/insights/2026-09-29-2000-entrevistas-colaboracion-en-vivo-fuera-de-teams.md)

### Revisar y corregir la lista antes de que la vea nadie
Como Joaquín, quiero revisar y corregir cada ítem viendo de dónde salió, para que nada incorrecto llegue al equipo con mi nombre.

Criterios de aceptación:
- [ ] La lista queda visible solo para el organizador hasta que él la publica.
- [ ] Cada ítem muestra la frase y el minuto de la transcripción que lo originó, y lleva a ese punto de la grabación.
- [ ] El organizador puede editar cada campo, borrar un ítem, agregar uno que falte y mover un ítem entre "decisiones" y "propuestas".
- [ ] Un ítem con "sin responsable" queda marcado a la vista hasta que el organizador lo completa o lo deja así a propósito.
- [ ] Si el organizador no publica, la lista no se envía sola en ningún momento.
- [ ] Una decisión que se refiere a algo mostrado en pantalla sin nombrarlo ("esto", "esa historia", "ese gráfico") aparece marcada como "falta contexto de pantalla" hasta que el organizador la completa o la confirma tal como está.

Se apoya en: caso de Paula (propuesta enviada como decisión sin revisar) y "Desde entonces reviso el resumen antes de mandarlo, siempre" (product/interviews/2026-09-28-1400-paula-benitez.md); el resumen "no sabe qué número estábamos mirando" (Diego Paredes, `real`, product/interviews/2026-09-28-1000-diego-paredes.md) y "se discutieron prioridades" cuando la votación fue en el tablero (Valeria Castro, `real`); panel de crítica (product/insights/2026-10-13-2040-critique-recap-de-decisiones.md, `synthetic`).

### Publicar la lista revisada a todos los invitados
Como Joaquín, quiero publicar la lista revisada en el chat de la reunión, para que todo el equipo, incluso quien no habló o no estuvo, lea la misma versión.

Criterios de aceptación:
- [ ] Al publicar, la lista aparece en el chat de la reunión y la ven todos los invitados internos, hayan asistido o no.
- [ ] La lista publicada dice quién la revisó y cuándo, y enlaza a la reunión.
- [ ] El recap completo de la conversación sigue disponible por separado y no reemplaza a la lista.
- [ ] Si la reunión tuvo invitados externos, el organizador elige antes de publicar si los externos ven la lista; por defecto no la ven.
- [ ] Si el organizador edita la lista después de publicarla, el chat muestra la versión nueva y marca que cambió.
- [ ] El organizador puede copiar la lista publicada en un solo paso, con formato (decisión, responsable, fecha, motivo, ticket) y el enlace a la reunión, y al pegarla en Confluence, Slack o un correo conserva esa estructura.

Se apoya en: "que quede claro qué se decidió, que lo sepan todos, incluso los que no hablaron" (Sofía Martínez, `real`); caso de los invitados del cliente en R05 (product/tests/T1-resources/resultados-cierre-confirmado.md, `real`, contexto de A2); el registro termina en Jira, correo o Slack (Tomás, Valeria, Lucía, Diego, Martina, `real`) y el panel de crítica (`synthetic`) muestra que, sin una salida, el líder sigue copiando a mano.

### Saber qué me toca al salir de la reunión
Como Rosa Elena, quiero ver en la lista publicada las decisiones en las que soy responsable, para saber qué me toca y para cuándo sin reenviar correos para dejar constancia.

Criterios de aceptación:
- [ ] Las decisiones en las que el responsable es la persona que mira la lista aparecen destacadas o primero.
- [ ] El responsable recibe una notificación de Teams cuando se publica una lista con una decisión a su nombre.
- [ ] Si una decisión tiene "sin responsable", nadie recibe notificación por ella.

Se apoya en: "Nadie escribe qué se decidió" (Rosa Elena Cabrera, `synthetic`, product/personas/rosa-elena-cabrera.md); el equipo de México leyó el recap y no el hilo (Javier Molina, `real`). La necesidad de quien ejecuta sin conducir no está validada con evidencia real todavía (agenda de la oportunidad, entrevistas al 11/11/2026).

## Hypothesis

Creemos que los líderes del segmento que conducen reuniones de más de 5 con decisiones van a publicar la lista de decisiones de la IA, revisada en 5 minutos o menos, en lugar de armar su propia acta, correo o carga en Jira, porque el recap actual les genera trabajo (reescribirlo o corregirlo, 10 a 60 minutos) y una lista con responsable y fecha que pueden verificar contra la transcripción se los ahorra.
Nos equivocamos si, mostrada la lista de su propia reunión, menos de la mitad de los líderes la publica en lugar de su registro habitual, o si la mediana de revisión supera los 5 minutos.

## Alternatives considered

Explored in: product/solutions/2026-09-29-2055-decisiones-sin-cierre-en-reuniones.md
- A2 `cierre-confirmado-en-vivo`: en prueba en paralelo (T1), no descartada. Ataca el dueño ambiguo, que esta alternativa no resuelve sin confirmación del grupo.
- A3 `publicar-decisiones`: parked. Resuelve solo el copiado y el registro escondido, y es la más débil en viabilidad. Vuelve como capa de salida si los líderes piden llevar la lista a Jira o Confluence. El copiar en un paso de esta spec no es A3: no publica nada solo ni se integra con otra herramienta.
- A4 `ritual-de-cierre`: parked. Se usa como prueba manual de A2.
- A5 `panel-valor-it`: parked. No alivia el dolor del líder y depende de que otra alternativa genere el dato.

## Tested before spec

Tested in: product/tests/2026-10-06-1914-decisiones-sin-cierre-en-reuniones.md
- T2 precisión de la extracción contra una clave a ciegas: diseñada, materiales armados, no corrida. Riskiest belief not tested (declared) · creencia 14 [feasibility].
- La spec mantiene lo que T2 va a medir: extracción desde la transcripción, salida fija de decisión, responsable, fecha y motivo, revisión del líder antes de publicar. Deja afuera, igual que T2, el contexto de pantalla o apps compartidas (votos en el tablero, filtros de un dashboard); se agrega después si T2 pasa.
- Revisión 13/10/2026 (panel de crítica): la extracción suma dos salidas, el código de ticket dicho en voz alta y la marca "falta contexto de pantalla". T2 no se corrió, así que ningún resultado se invalida, pero el prompt y la hoja de comparación de T2 tienen que incluir estas dos salidas para que la prueba cubra esta versión. La marca no agrega contexto de pantalla: solo avisa que falta.

## Assumptions

Referenciadas de `product/overview.md`:

- [feature: recap-de-decisiones] [feasibility] (creencia 14) La IA extrae decisión, responsable y fecha y separa propuesta de decisión con precisión suficiente para publicarse tras una revisión corta. Se falsa si, sobre grabaciones reales, más de 1 de cada 5 decisiones extraídas es incorrecta o falta, o si la revisión del líder lleva más de 5 minutos. **Sin probar (T2 no corrida).**
- [feature: recap-de-decisiones] [value] (creencia 15) Los líderes publican la lista de decisiones de la IA, revisada, en lugar de armar su propio registro. Se falsa si, mostrada la lista de su propia reunión, menos de la mitad la publica o la manda en lugar de su acta, correo o carga en Jira.
- [feature: recap-de-decisiones] [usability] (creencia 16) Al revisar la lista, el líder detecta y corrige las propuestas marcadas como decisión antes de publicar. Se falsa si, mostrada una lista con errores sembrados de su propia reunión, el líder publica sin corregir más de 1 de cada 4.
- [opportunity: decisiones-sin-cierre-en-reuniones] [value] (creencia 8) El trabajo posterior y las fallas mensuales existen a escala del segmento.
- [opportunity: decisiones-sin-cierre-en-reuniones] [viability] (creencia 9) Resolver el cierre de decisiones mueve la tasa de upgrade a Max del segmento por encima del 3,1%.

Restricciones abiertas (no son creencias, las decide alguien más):
- **"Tiempo real":** esta alternativa trabaja después de la reunión. Si el patrocinador mantiene la restricción, la spec queda fuera de alcance (solutions file, Decision).
- **Espacio Económico Europeo (UE, Islandia, Liechtenstein y Noruega):** atar una función de Teams al plan superior en cuentas con operación en esa zona necesita confirmación de legal (oportunidad, Constraints).
