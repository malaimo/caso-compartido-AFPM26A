---
opportunity: decisiones-sin-cierre-en-reuniones
status: testing-several
chosen: cierre-confirmado-en-vivo, recap-de-decisiones
tests: product/tests/2026-10-06-1914-decisiones-sin-cierre-en-reuniones.md
---

# Solutions for: Las decisiones de las reuniones grandes no se cierran

Oportunidad: `product/opportunities/2026-09-29-2050-decisiones-sin-cierre-en-reuniones.md`

## What the evidence says now

- [value] (creencia 8 del overview): abierta, con base cualitativa fuerte. 10 de 10 entrevistados con una falla reciente y 8 de 10 con trabajo manual posterior de 10 a 60 min (`real`, n=10, `product/insights/2026-09-29-2000-entrevistas-colaboracion-en-vivo-fuera-de-teams.md`); tema más mencionado de la encuesta (34 de 95) y 24% de reuniones sin registro de lo decidido (`survey`, n=182, `product/insights/2026-09-29-1931-colaboracion-en-vivo-fuera-de-teams.md`). Falta cuantificar los umbrales a escala.
- [viability] (creencia 9) y creencia 4: abiertas, sin entrevistas con IT. El mercado cobra la IA en planes superiores, y a la vez su ROI es difícil de demostrar (`secondary`, `product/research/2026-09-15-2126-colaboracion-en-vivo-fuera-de-teams.md`).
- La restricción de "tiempo real" está en revisión con el patrocinador.

## Baseline: what people do today

El líder reconstruye la decisión a mano después de la reunión: acta o correo (Diego, Andrés), carga en Jira (Tomás, Valeria, Lucía), reescritura o corrección del recap de IA (Javier, Paula), o la decisión queda en un hilo de Slack que Teams no ve (Martina). Le lleva de 10 a 60 minutos y "nadie más lo hace" (`real`, n=10). En el 24% de las reuniones lo decidido no queda registrado en ningún lado (`survey`, n=182). Aun con ese trabajo, las fallas siguen: dueño ambiguo, registro tardío o escondido, registro incorrecto de la IA.

## Alternatives

### A1. Recap de IA centrado en decisiones (`recap-de-decisiones`)
Después de la reunión, la IA extrae la lista de decisión, responsable, fecha y motivo, separa propuesta de decisión y toma contexto de lo compartido en pantalla o en apps. El líder la revisa antes de publicarla. Ataca el registro incorrecto y el trabajo posterior. Para Carolina Restrepo y Joaquín Lemus (primary). Reemplaza reescribir el recap y armar el acta a mano.

### A2. Cierre confirmado en vivo (`cierre-confirmado-en-vivo`)
En los últimos minutos de la reunión todos ven la lista de decisión, responsable, fecha y motivo, y cada responsable confirma lo suyo antes de cortar. La lista puede empezar vacía o con un borrador. Ataca el dueño ambiguo, el registro tardío y lo decidido que no llega a quien no habló. Para los líderes (Carolina, Joaquín, primary) y para quien recibe (Rosa Elena Cabrera, tertiary). Reemplaza el "cada uno entendió que lo hacía el otro" y el correo días después.

### A3. Publicación automática donde vive el trabajo (`publicar-decisiones`)
El líder escribe la decisión una sola vez en Teams y se publica sola en Jira, Confluence, el canal o el correo, con enlace a la reunión. Ataca el registro escondido o en otro lugar y el copiado manual. Para Carolina y Joaquín (primary). Reemplaza pasar lo mismo a tres lugares. Une dos ideas del brief (captura y envío a Jira y al acta; publicar donde vive el trabajo) porque las mata la misma creencia.

### A4. Ritual de cierre con plantilla (`ritual-de-cierre`)
Sin software nuevo: una práctica recomendada en la que los últimos 5 minutos se lee en voz alta decisión, responsable y fecha, apoyada en una plantilla de las notas de reunión que ya existen. Se difunde con guía y material para líderes. Es lo más chico que podría funcionar. Para los líderes (primary). Reemplaza el correo posterior.

## Comparison

| Alternative | Desirable | Feasible | Viable | Riskiest belief |
|---|---|---|---|---|
| A1 `recap-de-decisiones` | mixed (real, n=10: 6 de 10 usan o probaron el recap y ninguno lo usa como registro; survey, n=182: 26 "Otro" sobre el recap. No resuelve el dueño ambiguo sin confirmación) | to check with tech (parte de un recap que ya existe en el plan superior; distinguir propuesta de decisión no está probado) | mixed (secondary: el mercado cobra la IA, pero su ROI cuesta demostrarse; el recap ya está arriba y el segmento sube solo 3,1%, así que tiene que ser visiblemente distinto) | La IA separa decisión de propuesta y asigna responsable con precisión suficiente. Se falsa si, sobre grabaciones reales, más de 1 de cada 5 decisiones extraídas es incorrecta o falta, o si la revisión del líder lleva más de 5 minutos |
| A2 `cierre-confirmado-en-vivo` | mixed, pain evidenced, relief not tested (real, n=10: ataca los tres modos de falla, dueño ambiguo en 3 casos, registro tardío o escondido en 4, y lo que no llega a quien no habló; synthetic: Rosa Elena como receptora) | to check with tech (cabe entera en la restricción de tiempo real del brief; podría apoyarse en las notas de reunión existentes) | mixed (secondary: una lista sola se parece a la cocreación que el mercado regala; gana valor de plan superior si la IA la redacta, assumption) | Los grupos reservan y usan 2 a 3 minutos al final para confirmar. Se falsa si en la mayoría de las reuniones el cierre se saltea por tiempo (real: reuniones que se alargan y priorizaciones que se traban son evidencia en contra) |
| A3 `publicar-decisiones` | mixed (real, n=10: elimina el copiado y el registro escondido en 4 de 10, no el dueño ambiguo ni el registro incorrecto; synthetic: Joaquín abandonó Loop por no sincronizar con Confluence) | to check with tech (depende de Jira y Confluence de terceros y de la aprobación del admin, secondary) | weak (secondary: integrar no es lo que se cobra; las herramientas externas ya integran) | Los líderes escriben la decisión en Teams y no directamente en Jira. Se falsa si en un piloto siguen escribiendo en la herramienta de destino |
| A4 `ritual-de-cierre` | mixed (real, n=10: ataca el dueño ambiguo sin costo, no el traspaso a Jira; los que dicen "es disciplina" describen fallas que la disciplina no evitó) | strong (real: las notas de reunión existen, 8% de uso en telemetría; survey, n=210: 31% no sabe que existen. Límites: se pierden si la serie se recrea, excluyen a externos, secondary) | weak (assumption: no hay nada que vender en Max) | Los líderes sostienen el ritual sin apoyo de la herramienta. Se falsa si en un piloto con 10 líderes menos de la mitad lo sigue haciendo al mes |

Ninguna columna sale toda en `strong`; la única celda `strong` de valor (A2) se revisó y se apoya en la misma evidencia real que las demás, cubriendo más modos de falla.

Revisión 06/10/2026: la celda Desirable de A2 baja de `strong` a `mixed` (pain evidenced, relief not tested). Se apoyaba solo en evidencia del problema; nadie reaccionó todavía a un cierre confirmado en vivo.

## Decision

Recomendación del agente: probar A2 y A1 en paralelo. A2 es la que mejor alivia el dolor (tres modos de falla, única que entra entera en la restricción de tiempo real) y su punto débil es la viabilidad; A1 es la que mejor defiende el upgrade y su punto débil es la precisión. Se complementan (la IA redacta, el grupo confirma), pero las mata una creencia distinta a cada una, así que se prueban por separado antes de juntarlas.

Decisión del usuario (29/09/2026): la misma, `testing-several` con A2 y A1.

Pruebas: diseñadas en `product/tests/2026-10-06-1914-decisiones-sin-cierre-en-reuniones.md` (T1 para A2, creencia 12; T2 para A1, creencia 14). El piloto de 4 semanas de A2 queda como paso siguiente de T1 si pasa.

Qué cambiaría la decisión: si el piloto muestra que el cierre se saltea por tiempo, queda A1 sola; si la precisión de A1 no alcanza, queda A2 con lista manual y la viabilidad se cae; si las entrevistas con IT dicen que el freno es precio, ninguna sirve al upgrade y la oportunidad se mueve a retención.

## Value proposition: cierre-confirmado-en-vivo (A2)

- **Pain relieved:** la decisión que cada uno entendió distinto y nadie ejecutó ("el líder de Ecuador entendió que lo pasaba yo, y yo entendí que lo pasaba él. Nadie lo pasó", Andrés, `real`), el registro que llega días después o queda escondido (Diego, Sofía, `real`) y lo decidido que no llega a quien no habló (Sofía, `real`; Rosa Elena, `synthetic`).
- **Gain created:** la reunión termina con cada decisión con un responsable que dijo "es mío", una fecha y un motivo, visible para todos antes de cortar.
- **Replaces:** el correo o el acta del líder días después y la suposición de que "quedó claro". Se cambiaría porque el registro de hoy llega tarde y sin la confirmación de quien ejecuta, y aun así el líder le dedica de 10 a 60 minutos.
- **Deliberately does not:** redactar la lista con IA (eso es A1), publicar en Jira u otras herramientas (A3, aparcada), ni ayudar a converger antes de decidir (es otra oportunidad, `convergencia-trabada-en-reuniones`).

## Value proposition: recap-de-decisiones (A1)

- **Pain relieved:** el recap que "resume todo al mismo nivel, dos páginas" (Javier, `real`), que marca propuestas como decisiones (Paula: 1 semana de 2 desarrolladores, `real`) y que el líder tiene que reescribir o corregir (8 de 10 hacen trabajo manual posterior, `real`).
- **Gain created:** una lista corta de decisión, responsable, fecha y motivo lista para revisar en minutos, separada de lo que solo se conversó.
- **Replaces:** reescribir el recap o armar el acta a mano. Se cambiaría porque el recap actual genera trabajo en vez de ahorrarlo, y la corrección manual lleva de 10 a 60 minutos.
- **Deliberately does not:** publicar sin revisión del líder, confirmar con el grupo (eso es A2), ni integrarse con Jira u otras herramientas (A3).

## Beliefs

Referenciadas de `product/overview.md`:

- [opportunity: decisiones-sin-cierre-en-reuniones] [value] (creencia 8) En el segmento, la mayoría de los líderes que conducen reuniones de más de 5 con decisiones dedica 10 minutos o más después de la reunión a registrarlas o pasarlas a mano, y en sus equipos al menos una decisión por mes se ejecuta distinto, tarde o no se ejecuta por dueño ambiguo o registro incorrecto.
- [opportunity: decisiones-sin-cierre-en-reuniones] [viability] (creencia 9) Resolver el cierre de decisiones mueve la tasa de upgrade a Max del segmento por encima del 3,1%.

Propuestas para el registro (solo las que resuelven las pruebas):

- [feature: cierre-confirmado-en-vivo] [usability] Los grupos del segmento reservan y usan 2 a 3 minutos al final de la reunión para confirmar la lista de decisiones. Se falsa si, en un piloto de 4 semanas con 8 a 10 líderes, el cierre se saltea en más de la mitad de las reuniones con decisiones.
- [feature: cierre-confirmado-en-vivo] [value] Que cada responsable confirme su decisión antes de cortar reduce las decisiones mal ejecutadas. Se falsa si, en el mismo piloto, las decisiones ejecutadas distinto, tarde o no ejecutadas no bajan al menos a la mitad contra el mes anterior.
- [feature: recap-de-decisiones] [feasibility] La IA extrae decisión, responsable y fecha y separa propuesta de decisión con precisión suficiente para publicarse tras una revisión corta. Se falsa si, sobre grabaciones reales, más de 1 de cada 5 decisiones extraídas es incorrecta o falta, o si la revisión del líder lleva más de 5 minutos.

## Discarded or parked

- A3 `publicar-decisiones`: parked. Resuelve solo el copiado y el registro escondido, no el dueño ambiguo ni el registro incorrecto, y es la más débil en viabilidad. Vuelve como capa de salida de A1 o A2 si las pruebas funcionan y los líderes piden llevar la lista a Jira o Confluence.
- A4 `ritual-de-cierre`: parked como alternativa; se usa como prueba manual de A2. Si el piloto muestra que el ritual sin herramienta alcanza, pasa a ser la respuesta más barata y hay que rever si vale construir algo.
- A5 `panel-valor-it` (panel por cuenta que muestre a IT el valor de reunión obtenido): parked. No alivia el dolor del líder y depende de que otra alternativa genere el dato; ataca la creencia 4 y la viabilidad. Vuelve cuando haya dato que mostrar y cuando las entrevistas con IT respondan la creencia 4.
