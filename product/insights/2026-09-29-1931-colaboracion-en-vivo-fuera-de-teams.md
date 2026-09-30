---
source: survey
survey_design: product/surveys/2026-09-22-1944-colaboracion-en-vivo-fuera-de-teams.md
results: product/surveys/2026-09-26-1800-respuestas-colaboracion-en-vivo-fuera-de-teams.csv
n: 210 completas (76 email, 134 panel); 182 trabajaron fuera de Teams, 28 "En ninguna"
opportunity: colaboracion-en-vivo-fuera-de-teams
date: 2026-09-29
---

# Análisis de encuesta: trabajo colaborativo fuera de Teams en reuniones de más de 5 participantes

## Denominador y límites

- **Export temprano:** respuestas del 23 al 25/09, antes de la primera revisión prevista (13/10) y del cierre (24/10). Es una lectura anticipada; conviene repetir el análisis al cierre.
- **Filas:** 249 (210 completas, 34 descalificadas, 5 parciales excluidas). Sin speeders evidentes (mínimo 75 s entre completas) ni straightlining.
- **Metas de n:**
  - Trabajaron fuera de Teams: 182 (meta ≥150, cumplida).
  - Por canal: email 76 y panel 134 (meta ≥30, cumplida).
  - **"En ninguna": 28 (meta ≥30, no cumplida; resultados direccionales).** Email aporta 11.
- **Tasa de respuesta:** el alcance del email sigue sin confirmar, no se calcula. El panel lleva 134 de 150 completas compradas.
- **Sesgos:** los dos canales son autoseleccionados; la firmografía del panel es autodeclarada. Todo lo que sigue es evidencia de esta muestra, no del segmento.

### Diferencias por canal (hablan de la muestra antes que del segmento)

| Indicador | Email | Panel |
|---|---|---|
| Q1 "En menos de la mitad" | 39% | 18% |
| Q1 "Más de la mitad" o "Todas" | 21% | 39% |
| Q4 artefacto creado para la reunión | 48% | 35% |
| Q8 dos o más externos | 5% | 16% |
| Q9 registrado en chat o notas de Teams | 23% | 7% |
| Q10 IA en reuniones: "No sabía que existía" | 5% | 16% |
| R3 acepta entrevista | 25% | 43% |

El email sobrerrepresenta a quienes salen poco de Teams y registran dentro de Teams, como anticipaba el diseño. **Los hallazgos centrales de O1 y O2 van en la misma dirección en los dos canales** (5 min o más: 26% email, 28% panel).

## O1. Origen del artefacto

- **Creíamos:** la mayoría de los artefactos se crea para la reunión (creencia 2).
- **Datos (n=182):** ya existía 53% (51% existía y siguió vivo); creado para la reunión 40% (24% siguió usándose, 15% de un solo uso); no sabe 7%.
- **Corte por tipo de herramienta (Q2):**

| Tipo de reunión | % de reuniones | Creado para la reunión |
|---|---|---|
| Solo herramientas persistentes (Jira, Docs/Sheets/Slides, dashboards, Confluence, Notion) | 64% (117) | 16% |
| Solo pizarra o votación (Miro, Mural, FigJam, Lucidspark, Slido/Mentimeter) | 26% (48) | 83% |
| Mixto u otro | 9% (17) | 76% |

- **Qué hace el grupo según el origen (Q5):**

| Actividad | Artefacto que ya existía | Creado para la reunión |
|---|---|---|
| Revisar datos o métricas | 52% | 7% |
| Editar un documento entre varios | 41% | 25% |
| Actualizar tareas o tickets | 36% | 8% |
| Votar o priorizar | 29% | 56% |
| Aportar ideas o notas | 16% | 47% |
| Agrupar u ordenar ideas | 5% | 47% |
| Anotar decisiones o acuerdos | 34% | 32% |

- **Decisión:** según la regla del diseño, la oportunidad se reformula. "Salir de Teams" son dos necesidades distintas: **trabajar sobre artefactos que ya viven afuera** (integración, alrededor de dos tercios) y **cocrear algo nuevo para priorizar y decidir** (colaboración en vivo, alrededor de un tercio).

## O2. Costo de acceso

- **Creíamos:** se pierden 5 minutos o más por reunión en accesos (creencia 2).
- **Datos (Q6, n=182):** menos de 1 min 19%, 1 a 2 min 27%, 3 a 4 min 20%, 5 a 9 min 21%, 10 o más 6%, no sabe 7%. **5 min o más: 27%.**
- La combinación de la creencia (artefacto creado para la reunión y 5 min o más) aparece en el 18%, y en el **11% sin externos**.

| Situación | 5 min o más |
|---|---|
| Hay externos (n=39) | 62% |
| Sin externos (n=143) | 18% |
| Sin externos, artefacto creado para la reunión (n=56) | 38% |
| Sin externos, artefacto que ya existía (n=87) | 6% |

- **Quedan afuera (Q7):** en el 50% de las reuniones al menos una persona siguió mirando la pantalla de otro; 64% con externos, **47% sin externos**.
- **Cómo llegaron (Q3):** enlace en el chat 54%, ya abierta antes 22%, pantalla compartida 15%, app dentro de Teams 8%. La telemetría solo ve el primer caso: el 29% de reuniones con enlace externo está subestimado.
- **Decisión:** el umbral de 5 minutos no se sostiene para el uso interno. Donde se cumple es con externos (señal Bruno, persona negativa, no evidencia a favor). Dentro de la empresa el costo es de participación (alguien queda afuera), más que de minutos.

## O3. Qué se hace afuera y dónde queda la decisión

- **Actividades (Q5, n=182):** votar o priorizar 40%, editar entre varios 35%, revisar datos 34%, anotar decisiones 33%, aportar ideas 29%, actualizar tickets 25%, agrupar 22%, diagramar 13%. "Otro" 5% (revisar incidentes, roadmap, presupuesto, planning poker).
- **Dónde quedó lo decidido (Q9, múltiple):** no quedó registrado 24%, chat fuera de Teams 23%, Jira 23%, misma herramienta externa 15%, chat o notas de Teams 13%, acta 12%, correo 10%, no hubo decisiones 7%.
- **"Otro" en Q9 = 18%, por encima del umbral de 15%: la lista está incompleta.** 26 de las 32 respuestas "Otro" son resumen de IA, recap de Copilot, transcripción o grabación, casi siempre con una salvedad:
  > "En el recap de Copilot, que resume todo pero no distingue lo decidido" (R-097, panel)
  > "En el resumen de IA, que nadie leyó" (R-025, email)
  Para próximas olas: agregar la opción "En el resumen o recap de IA de la reunión".

### Q11: lo más difícil para trabajar juntos y decidir (95 respuestas, codificación múltiple)

| Tema | Menciones | Evidencia |
|---|---|---|
| Registro, seguimiento y continuidad de lo decidido (incluye 3 sobre resúmenes de IA que no separan decisión de conversación) | 34 | "Termino escribiendo el acta yo después de cada reunión y pasando las tareas a Jira a mano. Es trabajo que nadie ve" (R-124). "El resumen automático sirve para saber de qué se habló pero no para saber qué quedó decidido" (R-149) |
| Converger, votar, cerrar | 13 | "Votar. Usamos reacciones en el chat pero nadie sabe cuántos votaron ni qué ganó" (R-053) |
| Límites de lo nativo (Whiteboard sin votación ni plantillas, lenta, difícil de encontrar después) | 13 | "Armé una retro en la whiteboard de Teams y a la semana siguiente no la pude encontrar para continuar. Volvimos a Miro" (R-089) |
| Fuera de alcance (husos horarios, idioma, audio, demasiadas reuniones, rendimiento) | 12 | "Coordinar horarios entre 4 países" (R-075) |
| Acceso a la herramienta externa (4 con externos explícitos) | 11 | "Los permisos del Miro. Siempre hay alguien que no puede editar y pierde los primeros 10 minutos" (R-244) |
| Participación desigual y atención | 10 | "Hay 12 personas y opinan 3, el resto escucha o está en otra cosa" (R-049) |
| Compliance o regulación limita herramientas externas | 3 (+2 en Q12) | "Compliance no nos deja meter datos de clientes en Miro, así que o lo hacemos en Teams o no se hace" (R-190) |
| Sin problema o no aplica | 3 | "No hay problema real, funcionamos bien" (R-181) |

- **Decisión:** la actividad que cualquier solución tiene que cubrir es **priorizar y dejar registrada la decisión con dueño y fecha**, no solo la pizarra. Encaja con la corrección del 22/09 (IA para colaborar y decidir).

## O4. Conocimiento y uso de lo nativo (Q10, n=210)

| Función | No sabía | Sabe, nunca usó | Usó y dejó | Usa en algunas | Usa en la mayoría |
|---|---|---|---|---|---|
| Whiteboard | 8% | 27% | **43%** | 17% | 4% |
| Notas de la reunión (Loop) | **31%** | 28% | 14% | 20% | 8% |
| Apps de otras herramientas en la reunión | **40%** | 28% | 9% | 18% | 5% |
| Resumen o asistente de IA | 12% | 39% | 13% | 22% | 14% |

- **Whiteboard: problema de producto, no de descubrimiento.** La probaron y la dejaron. Motivos en Q11: no permite votar ni agrupar, faltan plantillas, no se encuentra la semana siguiente, se traba con más de 8 personas.
- **Notas y apps dentro de Teams: problema de descubrimiento.** Un tercio o más no sabía que existían.
- **Grupo "En ninguna" (n=28, direccional):** Whiteboard abandonada 50%. En Q12 parte del grupo no sale por compliance (R-009, R-143), no por conformidad; el resto vota a mano alzada, con reacciones o con Forms, o comparte un Excel.

## Insights, por impacto

## El dolor sin resolver es dónde termina la decisión, no entrar al tablero

El tema más mencionado en Q11 (34 de 95) es registrar, seguir y retomar lo decidido. En el 24% de las reuniones lo decidido no quedó en ningún lado y solo el 13% quedó dentro de Teams. Donde hay IA, el recap resume todo pero no distingue lo decidido de lo conversado, así que el Team Lead lo corrige o arma el acta a mano. Implica explorar una capacidad de IA que identifique decisiones, dueños y fechas y las conecte con la reunión siguiente, candidata a valor de Max.

> Evidencia: 26 respuestas "Otro" en Q9 sobre resumen, recap o transcripción; "El resumen de IA me ayuda pero marca como decisión cosas que eran solo ideas, lo tengo que revisar siempre" (R-153, email)

## "Salir de Teams" son dos necesidades con soluciones distintas

El 64% de las reuniones trabaja sobre herramientas persistentes que ya existían (84% preexistentes: revisar datos, editar, actualizar tickets); el 26% usa pizarras o votación creadas para la reunión (83%: votar, aportar y agrupar ideas). La primera necesidad es de integración y la segunda de cocreación en vivo. La oportunidad actual mezcla las dos y debería separarse.

> Evidencia: cruce Q2 × Q4 y Q4 × Q5 (n=182)

## El costo de 5 minutos existe con externos; adentro el costo es que alguien queda afuera

Con externos, el 62% tarda 5 minutos o más; sin externos, el 18%. En cambio, en el 47% de las reuniones internas al menos una persona sigue la sesión mirando la pantalla de otro. Para el segmento interno, la métrica relevante es participación efectiva, no tiempo de entrada.

> Evidencia: Q6 × Q8 y Q7 × Q8; "Con la agencia externa perdemos 5 o 10 minutos solo en que entren al FigJam" (R-072, panel)

## Whiteboard falla por lo que le falta; notas y apps fallan por descubrimiento

Solo el 8% no conocía Whiteboard y el 43% la abandonó, con motivos concretos (votación, plantillas, persistencia). Notas y apps dentro de Teams tienen 31% y 40% de desconocimiento. Son palancas distintas: capacidades para Whiteboard, descubrimiento para notas y apps.

> Evidencia: Q10; "Probamos la whiteboard de Teams hace un tiempo, no tenía plantillas ni votación y a la retro siguiente no la encontramos. Desde ahí todo en Miro" (R-113, panel)

## La telemetría ve alrededor de la mitad del trabajo fuera de Teams

Solo el 54% llegó a la herramienta por un enlace en el chat; el resto la tenía abierta, la abrió desde pantalla compartida o como app. El 29% de la telemetría es un piso, no el tamaño real, y hay que ajustarlo antes de usarlo como métrica base.

> Evidencia: Q3 (n=182)

## Preguntas de "por qué" para entrevistas

1. ¿Por qué no se confía en el recap de IA? ¿Qué hace que algo cuente como "decisión registrada"?
2. ¿Por qué se abandonó Whiteboard, si Miro y FigJam existen como apps dentro de Teams?
3. En los artefactos que ya existían: ¿qué se pierde al trabajar con ellos desde la reunión?
4. El grupo que no sale de Teams: ¿lo hace por compliance o por conformidad? (España y EEE en particular)
5. ¿Quién queda afuera en las reuniones internas y por qué (dispositivo, permisos, no ve el enlace)?

## Pool de reclutamiento

Elegibles: aceptaron entrevista (R3), no son de IT (R1) y conducen 2 o más reuniones por semana (R2). **64 personas** (48 panel, 16 email), 58 con contacto. Excluidos: 6 de IT y 7 que conducen poco. Los contactos quedan en el CSV de resultados y no se copian aquí.

**Contradicen la creencia 2, entrevistar primero:**
- Doble contradicción (artefacto que ya existía y menos de 3 min) (17): R-128, R-094, R-240, R-235, R-234, R-229, R-224, R-194 (sin contacto), R-180, R-176, R-151, R-144, R-131, R-102, R-247, R-036, R-057.
- "En ninguna" (12): R-153, R-170, R-135, R-143, R-046, R-009, R-196, R-120, R-085, R-088, R-242, R-110 (sin contacto). R-009 y R-143 mencionan compliance.
- Una sola contradicción (Q4 ya existía o Q6 menos de 3 min) (18): R-132, R-159, R-171, R-173, R-042, R-230, R-201, R-227, R-065, R-013, R-086, R-089, R-090, R-093, R-074, R-244, R-238, R-228.

**Confirman la creencia (17):** R-245, R-019, R-011, R-024, R-076, R-031, R-205, R-204, R-038, R-077, R-113, R-103, R-070, R-101, R-099, R-097, R-006.

## Contraste con el overview

- Creencia 2 [opportunity]: weakened. El artefacto mayormente ya existía (53% contra 40%); 5 min o más en el 27%, 11% en la combinación sin externos.
- Creencia 1 [product]: weakened. En el 53% de los casos el artefacto ya vivía afuera; la falta de cobertura nativa solo se sostiene para la cocreación en pizarra.
- Creencia 3 [product]: weakened. Se sostiene para Whiteboard (8% no la conocía, 43% la abandonó) pero no para las notas (31% no sabía que existían).
