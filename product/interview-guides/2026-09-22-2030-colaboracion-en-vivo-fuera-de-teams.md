---
opportunity: colaboracion-en-vivo-fuera-de-teams
source: product/opportunities/2026-09-15-2036-colaboracion-en-vivo-fuera-de-teams.md
research: product/research/2026-09-15-2126-colaboracion-en-vivo-fuera-de-teams.md
survey: product/surveys/2026-09-22-1944-colaboracion-en-vivo-fuera-de-teams.md
date: 2026-09-22
mode: exploration
status: draft
---

# Guía de entrevista: trabajo colaborativo en reuniones grandes, dentro y fuera de Teams

- **Objetivos de aprendizaje:**
  - **O1. Qué se hace afuera y por qué.** Qué actividad concreta hace el grupo sobre un artefacto compartido (aportar, agrupar, votar, editar, señalar datos) y por qué se hace donde se hace: función que falta en Teams, invitados externos, hábito o estándar del área, o el artefacto ya vive ahí. *Fuente:* creencia 1 del overview; fila `/design-interview` de la agenda de la oportunidad. *Decisión:* qué actividad tendría que cubrir cualquier solución.
  - **O2. Vida del artefacto.** Qué pasa con el tablero o documento antes, durante y después de la reunión. *Fuente:* creencia 2 del overview (parte "origen"); "qué sigue necesitando research primario" del research del 15/09. *Decisión:* si el artefacto mayormente preexiste, la oportunidad se reformula como integración y no como colaboración en vivo.
  - **O3. Cómo se llega a la decisión y dónde queda.** Cómo prioriza y decide el grupo, dónde se traba y qué trabajo le queda al Team Lead para que la decisión se registre y se cumpla. *Fuente:* corrección del 22/09 en `product/corrections.md` (la colaboración no se reduce a pizarras; incluye capacidades que ayuden a colaborar y decidir); objetivo O3 de la encuesta. *Decisión:* si el dolor está en converger y registrar la decisión, el espacio de solución se abre hacia facilitación y captura de decisiones, que es lo que el mercado sí cobra en planes superiores.
- **Fuera de alcance de esta guía:** el costo de acceso en minutos y el peso de los externos (lo cuantifica la encuesta, O2 de la encuesta) y el freno al upgrade desde IT (ronda aparte, perfil Damián).
- **Perfil del participante:** Team Lead o mando medio, empleado de la cuenta (no contratista ni IT), que conduce 2 o más reuniones de Teams de más de 5 participantes por semana, en cuentas Business Premium de 100+ licencias, sector tecnología, operación en 3+ países, facturación > USD 100M. Personas de referencia: Joaquín Lemus (segmento en foco, escéptico) y Carolina Restrepo (conducta parecida, otro sector). Ambas son sintéticas: sirven para preparar, no como evidencia.
- **Modo:** exploración. No hay idea ni prototipo que mostrar; la guía no tiene sección de estímulo.
- **Duración:** 30 minutos (lo que promete el opt-in de la encuesta).
- **Idioma de las entrevistas:** español, con trato de "tú" (participantes en México, Colombia, Argentina, Chile, Perú y España).

## Antes de cada entrevista

- Tener a mano las respuestas de la encuesta del participante: Q1 (cuánto sale), Q2 (herramienta), Q4 (origen del artefacto), Q6 (minutos), Q8 (externos), Q9 (dónde queda la decisión), Q10 (uso de lo nativo) y Q11/Q12 (abiertas). No leérselas: sirven para notar cuándo el relato contradice lo que marcó, y esa contradicción es un dato.
- Pedir consentimiento para grabar.

## Reglas para quien entrevista

- **No nombrar primero** Whiteboard, Loop, Copilot, IA ni ninguna función de Teams. Si el participante las menciona, preguntar por lo que pasó cuando las usó, no por su opinión.
- **No defender Teams** ni explicar funciones. Si el participante se queja, preguntar "¿qué pasó después?", no corregir.
- **Anclar todo en una reunión concreta** y reciente. Si el participante generaliza ("normalmente..."), volver: "¿y en esa reunión en particular?".
- **Señal Bruno:** si la razón de salir de Teams son los invitados externos, anotarlo y preguntar si lo mismo pasa en reuniones sin externos. Una explicación que solo vale con externos es señal de alarma, no evidencia (ver oportunidad, persona negativa).
- **Otras herramientas de reunión:** si el participante menciona reuniones que hace en Slack, Meet u otra herramienta, anotarlo sin profundizar. Mudar la reunión entera fuera de Teams es otra línea ("el equipo ya usa otras herramientas") y esta guía no la cubre.
- **Costo de acceso:** si aparecen los minutos perdidos en permisos o entradas, anotarlos sin profundizar (lo cuantifica la encuesta).
- **No explicar funciones de Teams** aunque el participante pregunte si existen ("¿eso hay en Teams?"). Responder "cuéntame cómo lo resolvieron" y seguir.

## Calentamiento (3 min)

W1. Cuéntame brevemente qué hace tu equipo y qué reuniones conduces en una semana típica.
   - Probes: ¿Cuántas personas suelen estar? ¿Desde cuántos países?
   > Confirma perfil (conduce reuniones de más de 5, equipo multipaís). La presencia de externos ya está en la encuesta (Q8); no preguntarla acá.

## Cuerpo

*Ancla para todo el cuerpo:* "Quiero que pensemos en una reunión concreta: la última reunión de Teams de más de 5 personas que condujiste en la que el grupo trabajó junto sobre algo, por ejemplo un tablero, un documento, una lista o unos datos."

> El ancla dice "reunión de Teams" para que nadie elija una reunión hecha en Slack u otra herramienta, pero no menciona "fuera de Teams" a propósito: sirve igual para quien sale y para quien no sale, y deja que la herramienta aparezca en el relato.
>
> *Definición para quien entrevista:* "fuera de Teams" es cualquier trabajo sobre una herramienta que no es de Teams, se vea en pantalla compartida o por enlace. Compartir pantalla de Jira es "fuera" aunque ocurra en la llamada. No usar esta definición con el participante; sirve para clasificar lo que cuenta.

### O1. Qué se hace afuera y por qué (11 min)

**Creencia en riesgo:** los Team Leads sacan el trabajo colaborativo de Teams porque la colaboración nativa no cubre lo que necesitan hacer en vivo, no por hábito, por externos ni porque el artefacto ya viva afuera.
**Estamos equivocados si** la razón que aparece en los relatos es "así se hace en el área", "el tablero ya estaba ahí", "lo pidió el cliente o el contratista", o si nunca probaron nada dentro de Teams y no saben qué hay (eso es desconocimiento, creencia 3, no falta de función).

Q1. Llévame por esa reunión desde que empezó: ¿qué tenían que lograr y qué hizo el grupo, paso a paso?
   - ¿Dónde estaba eso sobre lo que trabajaban?
   - ¿Cómo lo veía el resto: en tu pantalla compartida o cada uno lo abría por su lado?
   - ¿Qué hacía la gente ahí concretamente: escribir, mover cosas, votar, señalar algo?
   - ¿Quién tocaba y quién solo miraba? ¿Por qué?
   - ¿Hubo alguien que casi no intervino? ¿Qué hacía mientras tanto?

Q2. ¿Cómo terminaron usando [la herramienta que nombró] para esa parte?
   > *Si el artefacto es el sistema de trabajo del equipo (Jira, Grafana, Confluence, un dashboard), no preguntar por qué se eligió: la respuesta es "ahí vive todo". Hacer solo el tercer probe y pasar a Q2b.*
   - ¿Quién la eligió y cuándo?
   - ¿Siempre se hace ahí o fue esa vez?
   - ¿Alguna vez intentaron hacer eso mismo de otra forma? ¿Qué pasó?
   - Solo si no apareció antes: ¿alguna vez esa parte se hizo con algo de la propia reunión de Teams, sin abrir otra herramienta? ¿Cómo fue?

Q2b. ¿Hay otra reunión tuya de más de 5 personas en la que el grupo trabaje de otra forma sobre algo compartido? Cuéntame la última.
   - ¿Dónde estaba eso sobre lo que trabajaban?
   - ¿Quién lo armó y para qué reunión?
   - ¿Por qué ahí y no en otro lado?
   - ¿Qué pasó la última vez que intentaron hacer eso de otra forma?
   > Q2b existe porque el mismo Team Lead puede salir de Teams en una reunión y no en otra (refinamiento sobre Jira vs. retro o planning en un tablero armado para la sesión). Una sola reunión ancla no alcanza para ver el motivo.

*Variante si en ninguna de las dos reuniones se trabajó sobre algo fuera de la llamada:* Q2 → "Esa parte, ¿cómo la resolvieron sin salir de la llamada?" Probes: ¿qué funcionó?, ¿qué costó?, ¿alguna vez usaron otra herramienta y la dejaron? ¿por qué?

### O2. Vida del artefacto (6 min)

**Creencia en riesgo:** el artefacto externo se crea para esa reunión (y por eso el problema es colaborar en vivo).
**Estamos equivocados si** el tablero o documento ya existía, lo usan otras personas fuera de la reunión y sigue vivo después (Jira, Confluence, dashboards). En ese caso el problema es de integración, no de colaboración en vivo.

*Qué artefacto:* Q3 y Q4 van sobre el artefacto creado para la reunión, si apareció en Q2 o Q2b. Si no hubo ninguno, sobre el que el grupo editó. Si nadie editó nada, sobre el principal que se compartió. Nombrarlo al preguntar ("ese Miro", "ese doc").

Q3. Ese tablero o documento, ¿de dónde salió? Cuéntame qué pasó con él antes de la reunión.
   - ¿Quién lo armó, cuándo y cuánto le llevó?
   - ¿Existía de antes para otra cosa?
   - ¿Quién más lo usa fuera de estas reuniones?

Q4. ¿Y después de la reunión? ¿Cuándo fue la última vez que alguien lo abrió, y para qué?
   - ¿Dónde está hoy?
   > Lo que se copia a otro lugar (Jira, actas, hilos) se pregunta en Q6, no acá.

### O3. Cómo se llega a la decisión y dónde queda (7 min)

**Creencia en riesgo:** lo que más le cuesta al Team Lead es que el grupo converja a una decisión y que esa decisión quede registrada y se cumpla, y hoy eso ocurre fuera de Teams.
**Estamos equivocados si** las decisiones salen sin fricción y quedan registradas donde trabaja el equipo sin trabajo manual del Team Lead, o si no recuerda ninguna decisión perdida o mal ejecutada en los últimos meses. En ese caso, la facilitación y la captura de decisiones no son la palanca.

Q5. En esa reunión, ¿qué se decidió?
   - ¿Cómo llegaron a eso?
   - ¿Quién terminó decidiendo, y en qué momento quedó decidido?
   - ¿Hubo un momento en que se trabó? ¿Qué hiciste para destrabarlo?
   - Cuando algo no se cierra en la reunión, ¿qué pasa con eso después? ¿Cuándo se terminó decidiendo?

Q6. Una vez decidido, ¿qué pasó para que eso quedara registrado y se cumpliera? ¿Quién lo hizo y dónde quedó?
   - ¿Qué parte te tocó a ti y cuánto te llevó?
   - ¿Queda en algún otro lugar además de ese?
   - ¿Alguien se enteró tarde o entendió otra cosa?
   - Piensa en la última vez que algo que se decidió en una reunión terminó hecho distinto de lo acordado. ¿Qué pasó entre la reunión y eso?
   > La pregunta no asume que el Team Lead registra la decisión (a veces lo hace alguien del equipo en un hilo) y el último probe habla del caso, no de su desempeño: preguntado como falla propia, la respuesta se vuelve defensiva.

*Variante si en esa reunión no se decidió nada:* "Piensa en la última reunión grande de Teams en la que sí se tomó una decisión", y seguir con Q5.

## Cierre (3 min)

C1. ¿Hay algo sobre cómo trabaja tu equipo en las reuniones que no te pregunté y debería haberte preguntado?
C2. ¿Conoces a otro líder que conduzca reuniones grandes de una forma muy distinta a la tuya? ¿Aceptaría una conversación como esta?
   > Apunta a sumar participantes que contradicen la creencia.
C3. Agradecer y explicar qué pasa con lo que compartió.

## Mapa objetivo → pregunta

| Objetivo | Preguntas | Decisión que alimenta |
|---|---|---|
| Perfil | W1 | Confirmar que el participante es del segmento |
| O1 | Q1, Q2, Q2b | Qué actividad cubrir y por qué hoy sale |
| O2 | Q3, Q4 | Colaboración en vivo o integración |
| O3 | Q5, Q6 | Si la facilitación y la captura de decisiones son la palanca |
| Reclutamiento | C1, C2 | Cobertura y próximos participantes |

## Plan de reclutamiento

**Canales.** La fuente principal son los encuestados que aceptaron conversar en el bloque de opt-in de la encuesta (`product/surveys/2026-09-22-1944-colaboracion-en-vivo-fuera-de-teams.md`). Esos opt-ins vendrán de los canales definidos en la sección **Distribución** de esa encuesta (email a organizadores del segmento y panel B2B); no se repiten acá. Candidatos elegibles: R3 = "Sí", R1 = "No" (no es IT), R2 = "2 o 3" o "4 o más".

Selección por respuestas, primero los que contradicen la creencia (enseñan más):

| Grupo | Criterio en la encuesta | Entrevistas |
|---|---|---|
| No salen | Q1 = "En ninguna" | 3 a 4 |
| Salen, pero el artefacto preexiste o no les cuesta | Q1 ≠ "En ninguna" y (Q4 = "Ya existía..." o Q6 = "Menos de 1 minuto" / "Entre 1 y 2 minutos") | 3 a 4 |
| Salen y confirman | Q4 = "Se creó para esa reunión..." y Q6 ≥ "Entre 5 y 9 minutos" | 2 a 4 |

Dentro de cada grupo: priorizar Q8 = "No" (reuniones sin externos), mezclar los dos canales de la encuesta y cubrir al menos 3 países, con al menos una persona en España (operación en el EEE, riesgo regulatorio señalado en el research).

**Canal propio solo para lo que la encuesta no cubre.** Si el 28/10 el grupo "No salen" tiene menos de 3 opt-ins, pedir al mismo panel B2B una cuota específica de Team Leads que no usan herramientas externas en reuniones, filtrados con el screener de abajo. Es el hueco que la propia encuesta ya anticipa.

**Screener** (para reclutas del panel fuera de la encuesta, o para confirmar por correo antes de agendar):

1. En el último mes, ¿cuántas reuniones de Microsoft Teams de más de 5 participantes condujiste por semana, en promedio? [0 o 1 / 2 o 3 / 4 o más] → **descalificar** si "0 o 1".
2. ¿Cuál describe mejor tu rol? [Lidero un equipo o área dentro de la empresa / Administro Microsoft 365 o Teams (IT) / Soy consultor, contratista o trabajo sobre todo con clientes externos / Otro] → **descalificar** todo lo que no sea "Lidero un equipo o área". El perfil de consultor es el de Bruno (persona negativa).
3. ¿En qué sector está tu empresa y en cuántos países tiene equipos? [Tecnología o software y 3 o más países / otra combinación] → **descalificar** si no es tecnología con 3 o más países.

**Cuántas.** Entre 8 y 12 entrevistas de 30 minutos, del 28/10 al 11/11/2026 (la encuesta cierra el 24/10). Cortar antes si hay saturación: cuando tres entrevistas seguidas no traen una actividad, un motivo o un destino de la decisión nuevos. Corte de decisión de la oportunidad: 15/11/2026.

## Pretest notes

### 2026-09-22: dos corridas sintéticas (Carolina Restrepo y Joaquín Lemus)

Prueba del diseño de la guía, no evidencia. Ambas corridas sobre la versión original, sin cambios entre una y otra.

- **Carolina Restrepo** (servicios financieros; fuera del perfil por sector, sirve para estructura). Duró entre 36 y 40 min.
- **Joaquín Lemus** (segmento en foco, usa Slack, contratistas externos en el planning). Duró entre 32 y 34 min.

**Qué cambió:**
- **Ancla restringida a reuniones de Teams**, más una definición de "fuera de Teams" para quien entrevista: compartir pantalla de una herramienta externa también cuenta como fuera. En las dos corridas la repregunta "¿se hizo dentro de la llamada de Teams?" confundió ("sí fue en Teams, compartí pantalla"). Joaquín preguntó si la reunión ancla podía ser un huddle de Slack.
- **Nueva Q2b (segunda reunión) y la variante "no sale" pasa a depender de la reunión, no de la persona.** En las dos corridas el caso del artefacto creado para la reunión (la retro en Miro de Carolina, el planning en FigJam de Joaquín) apareció recién en la última repregunta de Q4, y nadie lo exploró. O1 pasa de 9 a 11 min.
- **Nota en Q2 para artefactos que son el sistema de trabajo del equipo.** Con Grafana, las tres repreguntas de elección dieron respuestas de una línea ("es donde están las métricas").
- **Nota sobre qué artefacto usar en Q3 y Q4.** En las dos corridas hubo dos artefactos ("¿cuál, el Jira o el doc?").
- **Q6 reescrita:** ya no da por hecho que el Team Lead registra la decisión (Joaquín: "¿Yo? Directamente, nada"). El probe sobre decisiones perdidas habla del caso y no de la persona (Carolina respondió a la defensiva). Se agregó "¿queda en algún otro lugar?" (grabaciones, hilos).
- **Q5 separada en qué y cómo.** Las opciones "votación, alguien, consenso" pasan a pregunta abierta (Joaquín: "ninguna de esas"). Se agregó un probe para lo que no se cierra ("lo seguimos por chat / en el hilo").
- **Repeticiones eliminadas:** "¿se copió algo a otro lugar?" en Q4 (lo cubre Q6), "¿participaron todos por igual?" en Q5 (lo cubre Q1), "otras reuniones" en Q4 (lo cubre Q2b) y externos en W1 (lo cubre la encuesta, Q8). O2 pasa de 7 a 6 min y O3 de 8 a 7.
- **La repregunta de Q1 sobre "quienes no llegaron a participar"** se reescribió porque daba algo por hecho (Carolina entendió "los que no llegaron").
- **Tres reglas nuevas:** otras herramientas de reunión, costo de acceso y no explicar funciones de Teams. Se anotan, no se profundizan.

**Qué quedó igual a propósito:**
- La repregunta de Q1 "señalar algo": sacó el dolor de no poder señalar en pantalla compartida sin inducirlo.
- La regla "señal Bruno": separó el problema de externos (FigJam) del día a día.
- Q3 y Q4: produjeron exactamente lo que la guía dice que la invalida (artefacto que ya existía y tiene vida propia).
- La regla de no nombrar primero Loop o Whiteboard.
- La migración de reuniones completas a Slack no se agrega como pregunta: no cabe en 30 min y es otra línea. Queda como nota.

**Pendiente:** volver a probar la versión revisada (sugerido: Bruno, para ver si el screener y la señal Bruno lo detectan, o Carolina para confirmar que Q2b funciona). Una persona sintética no mide si la redacción se entiende ni si la gente real se abre.
