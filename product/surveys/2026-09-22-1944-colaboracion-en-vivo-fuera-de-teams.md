---
opportunity: colaboracion-en-vivo-fuera-de-teams
source: product/opportunities/2026-09-15-2036-colaboracion-en-vivo-fuera-de-teams.md
research: product/research/2026-09-15-2126-colaboracion-en-vivo-fuera-de-teams.md
date: 2026-09-22
status: draft
---

# Encuesta: trabajo colaborativo fuera de Teams en reuniones de más de 5 participantes

- **Objetivos de aprendizaje:**
  - **O1. Origen del artefacto.** ¿El tablero o documento externo se crea para la reunión o ya existía y sigue viviendo afuera? *Decisión:* si mayormente preexiste, la oportunidad se reformula como integración y no como colaboración en vivo (creencia 2 del overview).
  - **O2. Costo de acceso.** Minutos hasta que todos entran, cuántos quedan afuera y cuánto pesan los externos. *Decisión:* confirma o tumba el umbral de 5 minutos; si la fricción se concentra en reuniones con externos, es señal Bruno (persona negativa) y no evidencia.
  - **O3. Qué se hace afuera y dónde queda la decisión.** Votar, priorizar, editar, revisar datos, registrar acuerdos. *Decisión:* qué actividad tendría que cubrir cualquier solución, incluidas capacidades de IA para colaborar y decidir (corrección del 22/09 en `product/corrections.md`), no solo pizarras.
  - **O4. Conocimiento y uso de lo nativo.** ¿Conocen y probaron Whiteboard, notas de reunión, apps de terceros dentro de Teams e IA en reuniones? *Decisión:* separa "no me sirve" de "no sé que existe" (creencia 3 del overview).
- **Encuestados:** Team Leads y mandos medios, empleados de la cuenta (no externos), que condujeron al menos una reunión de Teams de más de 5 participantes en el último mes, en cuentas Business Premium de 100+ licencias, sector tecnología, operación en 3+ países, facturación > USD 100M. La firmografía la garantiza el canal (lista de cuentas del segmento o filtro del panel), no se pregunta salvo en el panel.
- **Duración estimada:** 12 preguntas como máximo para quien trabaja afuera, 5 para quien no; ~5 minutos.
- **Nota de método:** las opciones de O3 salen de personas sintéticas y research secundario, no de entrevistas reales. Por eso cada lista tiene "Otro" y hay una pregunta abierta; si "Otro" supera el 15% en una pregunta, la lista está incompleta y se revisa con las entrevistas del 11/11.

## Filtro

S1. En el último mes, ¿condujiste u organizaste al menos una reunión de Microsoft Teams con más de 5 participantes? [opción única]
   - Sí
   - No
   → descalificar si "No"

S2. ¿Cuál describe mejor tu relación con la empresa donde trabajas? [opción única]
   - Soy empleado o empleada de la empresa
   - Soy contratista, consultor o proveedor externo
   - Otra
   → descalificar si no es "Soy empleado o empleada"

S3. *(solo enlace del panel)* ¿En qué sector está la empresa donde trabajas? [opción única]
   - Tecnología o software
   - Servicios financieros
   - Manufactura
   - Comercio o retail
   - Otro
   → descalificar si no es "Tecnología o software"

S4. *(solo enlace del panel)* ¿En cuántos países tiene equipos tu empresa? [opción única]
   - 1
   - 2
   - 3 o más
   - No lo sé
   → descalificar si "1", "2" o "No lo sé"

## Preguntas

Q1. En el último mes, en las reuniones de más de 5 participantes que condujiste, ¿en cuántas el grupo abrió o editó algo en una herramienta que no es Teams (por ejemplo un tablero, un documento o un gestor de tareas)? No cuenta si solo miraron una pantalla compartida. [opción única]
   - En ninguna → saltar a Q10
   - En menos de la mitad
   - En aproximadamente la mitad
   - En más de la mitad
   - En todas
   > Goal: O1 y O2 (define el segmento de corte: sale / no sale; "En ninguna" es el grupo que contradice la creencia)

*Para Q2 a Q9: "Piensa en la última reunión de más de 5 participantes que condujiste en la que el grupo trabajó en una herramienta fuera de Teams."*

Q2. ¿En qué herramienta trabajaron? [opción múltiple]
   - Miro
   - Mural
   - FigJam
   - Lucidspark
   - Google Docs, Sheets o Slides
   - Notion
   - Confluence
   - Jira u otro gestor de tareas
   - Un dashboard (Grafana, Power BI, Looker u otro)
   - Slido o Mentimeter
   - Otra: ____
   > Goal: O1 y O3

Q3. ¿Cómo llegaron los participantes a esa herramienta? [opción única]
   - Pegué (o alguien pegó) un enlace en el chat de la reunión
   - La abrí como app dentro de la reunión de Teams
   - Compartí mi pantalla y cada uno la abrió por su cuenta
   - Ya la tenían abierta antes de la reunión
   - Otro: ____
   > Goal: O2 (además mide el punto ciego de la telemetría, que solo ve enlaces pegados en el chat)

Q4. Ese tablero o documento... [opción única]
   - Se creó para esa reunión y no se volvió a usar
   - Se creó para esa reunión y se siguió usando después
   - Ya existía antes de la reunión y se siguió usando después
   - Ya existía antes de la reunión y no se volvió a usar
   - No lo sé
   > Goal: O1 (pregunta central de la creencia 2)

Q5. ¿Qué hizo el grupo en esa herramienta durante la reunión? [opción múltiple]
   - Aportar ideas o notas
   - Agrupar u ordenar ideas
   - Votar o priorizar
   - Editar un documento entre varios
   - Revisar datos o métricas y señalar algo puntual
   - Actualizar tareas o tickets
   - Dibujar un diagrama o flujo
   - Anotar decisiones o acuerdos
   - Otro: ____
   > Goal: O3

Q6. Desde que se compartió la herramienta, ¿cuánto tardaron todos los que tenían que participar en estar dentro? [opción única]
   - Menos de 1 minuto
   - Entre 1 y 2 minutos
   - Entre 3 y 4 minutos
   - Entre 5 y 9 minutos
   - 10 minutos o más
   - No lo sé
   > Goal: O2 (los tramos rodean el umbral de 5 minutos)

Q7. ¿Cuántos participantes no lograron entrar y siguieron la reunión mirando la pantalla de otra persona? [opción única]
   - Ninguno
   - 1
   - 2 o 3
   - 4 o más
   - No lo sé
   > Goal: O2

Q8. ¿Había en esa reunión personas de fuera de tu empresa (clientes, contratistas, consultores)? [opción única]
   - No
   - Sí, 1
   - Sí, 2 o más
   - No lo sé
   > Goal: O2 (control de señal Bruno: cruzar con Q6 y Q7)

Q9. ¿Dónde quedó registrado lo que se decidió en esa reunión? [opción múltiple]
   - En la misma herramienta externa
   - En Jira u otro gestor de tareas
   - En un chat fuera de Teams (Slack, WhatsApp u otro)
   - En el chat o las notas de la reunión de Teams
   - En un correo
   - En un documento de actas
   - No quedó registrado en ningún lado
   - No se tomaron decisiones
   - Otro: ____
   > Goal: O3 (dónde termina la decisión; perfil Joaquín)

Q10. *(todos)* ¿Cuál describe mejor tu experiencia con cada una de estas funciones de Teams? [matriz de opción única; misma escala en todas las filas]
   - Filas: Whiteboard · Notas de la reunión (Loop) · Apps de otras herramientas dentro de la reunión (por ejemplo Miro o FigJam en Teams) · Resumen o asistente de IA en la reunión (por ejemplo Copilot)
   - Escala: No sabía que existía · Sé que existe, nunca la usé en una reunión · La usé alguna vez y dejé de usarla · La uso en algunas reuniones · La uso en la mayoría de mis reuniones
   > Goal: O4

Q11. *(todos)* En tus reuniones de más de 5 participantes, ¿qué es lo más difícil de lograr que el grupo trabaje junto y llegue a una decisión? [abierta, opcional]
   > Goal: O3 (y material para priorizar entrevistas)

Q12. *(solo quienes respondieron "En ninguna" en Q1)* Cuando en esas reuniones el grupo necesita aportar ideas, priorizar o decidir, ¿cómo lo hacen hoy? [abierta, opcional]
   > Goal: O3 y O4 (qué hace el grupo que contradice la creencia)

D1. ¿En qué país trabajas? [opción única: México · Colombia · Argentina · Chile · Perú · España · Estados Unidos · Otro: ____]
   > Goal: corte por región; España identifica cuentas con operación en el EEE (riesgo regulatorio señalado en el research)

## Filtro + opt-in (reclutamiento de entrevistas)

R1. ¿Tu trabajo incluye administrar Microsoft 365 o Teams para tu empresa (área de IT)? [Sí / No]
   → no es candidato si "Sí" (IT se entrevista en una ronda aparte)

R2. En una semana típica, ¿cuántas reuniones de más de 5 participantes conduces? [0 o 1 / 2 o 3 / 4 o más]
   → no es candidato si "0 o 1"

R3. ¿Aceptarías una conversación de 30 minutos sobre cómo trabajan tus equipos en las reuniones? [Sí / No]

R4. Si respondiste que sí, ¿cómo te contactamos? [abierta, opcional: nombre y correo]

*Para el análisis: etiquetar a los candidatos que contradicen la creencia (Q1 "En ninguna", Q4 "Ya existía...", Q6 "Menos de 1 minuto" o "Entre 1 y 2 minutos") y entrevistarlos primero, como pide la agenda.*

## Distribución

| Canal | A quién llega y su sesgo | Alcance aprox. | Enlace |
|---|---|---|---|
| Email a organizadores del segmento (usuarios de las 12.400 cuentas del segmento, identificados por telemetría como organizadores de reuniones de >5 participantes, con permiso de contacto) | Team Leads que siguen conduciendo en Teams (perfiles Carolina y Joaquín). Canal propio: sobrerrepresenta a quienes están conformes con Teams y abren correos de Microsoft; subrepresenta a quienes ya movieron reuniones o decisiones a Slack o Meet | unknown (a confirmar con datos) | `?canal=email` |
| Panel B2B externo (Respondent o User Interviews), filtrado por Engineering o Product Manager en empresas de tecnología > USD 100M, 3+ países, que usan Teams en el trabajo | Managers del perfil sin relación con la marca: reduce sesgo de complacencia y alcanza a los que se fueron de Teams. Sesgo: panelistas profesionales motivados por el incentivo; la firmografía es autodeclarada (no se puede verificar plan Business Premium ni facturación) | 150 (cuota comprada) | `?canal=panel` |

- **Meta de n:** ≥150 Team Leads que trabajaron en una herramienta externa en el último mes (Q1 distinto de "En ninguna"); ≥30 que no lo hicieron; ≥30 por canal. Por debajo de 30 en un segmento, los resultados son direccionales.
- **Chequeo de alcance:** el panel aporta como máximo 150 completas, así que el email tiene que dar al menos otras 150. Con una tasa de respuesta de 2% a 5% en email frío a usuarios, hacen falta entre 3.000 y 7.500 contactos con permiso. Confirmar ese número con datos antes de enviar. Riesgo aparte: si casi todos salen, el grupo "En ninguna" puede no llegar a 30; revisarlo el 13/10 y, si falta, pedir al panel una cuota específica de quienes no usan herramientas externas.
- **Primera revisión:** 13/10/2026
- **Cierre:** 24/10/2026, o antes si se alcanza la meta (análisis antes del 28/10 de la agenda).
