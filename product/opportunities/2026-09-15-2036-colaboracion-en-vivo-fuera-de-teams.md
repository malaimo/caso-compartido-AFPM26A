---
status: framed
segment: Team Leads y mandos medios que conducen reuniones de más de 5 participantes en cuentas Business Premium de 100+ licencias, sector tecnología, operación en 3+ países, facturación > USD 100M (12.400 cuentas, 2,1M licencias)
personas: carolina-restrepo (parcial), joaquin-lemus (segmento en foco, escéptico), rosa-elena-cabrera (afectada), damian-sosa (comprador)
---

# Opportunity: La colaboración en vivo de las reuniones grandes se hace fuera de Teams

En las reuniones de más de 5 participantes de las cuentas de tecnología multinacionales, los Team Leads sacan el trabajo colaborativo fuera de Teams hacia tableros y documentos de terceros, y pagan por eso minutos de reunión, participantes que quedan afuera y una decisión que Teams nunca ve. Importa ahora porque ese mismo segmento convierte a Max por encima del promedio (3,1% contra 2,4%) y la conversación de upgrade se juega en "capacidades avanzadas de reuniones" que hoy nadie puede nombrar.

## Segment and personas

- **Sufren el problema:** Team Leads y mandos medios que conducen. Carolina Restrepo es la persona más cercana en conducta (retro quincenal en Miro, equipo en tres países, 5 a 7 minutos por reunión perdidos en accesos, Whiteboard descartado hace dos años por falta de plantillas y votación).
- **Cargan el costo sin poder resolverlo:** los participantes de baja alfabetización digital. Rosa Elena Cabrera no sabe si hacer clic en el enlace externo y se queda mirando la pantalla compartida de otro. No es el segmento, es la factura del problema.
- **Decide la compra, no sufre el problema:** Damián Sosa (IT). Su dolor es adyacente: no puede nombrar qué sacarían sus Team Leads de Max.
- **No sufren este problema:** Bruno Tavella (persona negativa). Bruno quiere que *salir* hacia FigJam sea más cómodo. Construir para él financia la fuga. Si un hallazgo se apoya en invitados externos y consultores, es señal de alarma, no evidencia.
- **Persona faltante (cubierta):** ninguna de las cuatro personas originales pertenecía a la firmografía en foco. Carolina es servicios financieros, Damián manufactura, Rosa Elena logística de 180 empleados. Faltaba un Team Lead en cuenta de tecnología multinacional de más de USD 100M. Para cubrir ese hueco se generó **Joaquín Lemus** (`product/personas/joaquin-lemus.md`): Engineering Manager en una SaaS B2B de comercio electrónico (USD 420M, Business Premium, equipos en Ciudad de México, Medellín y Madrid). Está construido como escéptico de la creencia [value] de esta oportunidad: sus enlaces externos apuntan a artefactos que preexisten (Jira, Confluence, Grafana) y con SSO el acceso le cuesta segundos; solo el planning trimestral en FigJam la confirma. Su dolor está en interactuar entre varios con el artefacto compartido y en que las decisiones queden en Slack, fuera de Teams. Es sintético: sirve para preparar la ronda de entrevistas, no como evidencia.

## Signals

| Signal | Provenance | Source |
|---|---|---|
| 29% de las reuniones de >5 participantes comparte un enlace externo (Docs/Notion, Miro/Mural/FigJam, Jira, dashboards) | real | telemetría de chat de reunión, `product/overview.md` |
| Whiteboard 5% y notas 8% de uso, contra compartir pantalla 67% | real | telemetría de uso, `product/overview.md` |
| 41% de las reuniones tiene más de 8 participantes; 11,4 h/semana por usuario | real | telemetría, `product/overview.md` |
| Segmento en foco: 12.400 cuentas, 2,1M licencias; upgrade Premium→Max 3,1% contra 2,4% general | real | datos de cuentas y facturación |
| 37% de las organizaciones tiene Slack o Google Chat activo en al menos un equipo | real | dato de cuentas, `product/overview.md` |
| "Colaboración durante la reunión" es el 19% de las quejas post-reunión | survey | encuestas post-reunión, `product/overview.md` (n no declarado) |
| 3,6% bajó de plan o no renovó; tercer motivo declarado "el equipo ya usa otras herramientas", sin especificar cuáles | survey | datos de renovación y encuesta de salida, `product/overview.md` |
| Carolina pierde 5 a 7 minutos por retro en accesos a Miro, con 2 personas que nunca entran; descartó Whiteboard por falta de plantillas y votación | synthetic | `product/personas/carolina-restrepo.md` |
| Rosa Elena no abre los enlaces externos por miedo a romper algo y no participa | synthetic | `product/personas/rosa-elena-cabrera.md` |
| Damián no puede defender el salto a Max (USD 110.000/año) porque solo tiene una lista de capacidades, no un uso concreto | synthetic | `product/personas/damian-sosa.md` |
| Joaquín comparte enlaces a artefactos que preexisten (Jira, Confluence, Grafana) con acceso casi inmediato por SSO; solo pierde 8 a 12 minutos en el planning trimestral en FigJam | synthetic | `product/personas/joaquin-lemus.md` |
| "Mejorar la colaboración y la interacción en tiempo real mediante herramientas colaborativas integradas" | unverified | planteo de entrada, sin fuente nombrada |

## Business outcome

Métricas que mira la dirección para este segmento: **tasa de upgrade a Max**, **retención en la renovación** e **ingreso por licencia**. Se toma el upgrade a Max como métrica líder de esta oportunidad: es donde hay recorrido (96,9% del segmento no subió) y es la única que se puede falsar contra un número propio. Orden de magnitud: cada punto porcentual de las 2,1M licencias del segmento convertido a Max son unos USD 2M anuales (cálculo derivado, no señal).

## Constraints

- Presupuesto máximo USD 5M.
- Presentación en CollabCon, la conferencia anual, en 5 meses (aprox. 16/02/2027).
- Límites declarados para cualquier solución futura: facilidad de uso, accesibilidad, compatibilidad con Microsoft 365, privacidad y seguridad corporativas, tiempo real, impacto mínimo en el rendimiento de la reunión.
- **Nota sobre "tiempo real":** es una restricción del patrocinador, no un hallazgo. Recorta el espacio de solución antes de investigar y deja fuera de entrada cualquier respuesta asíncrona al mismo problema (que es adonde apunta la creencia 4 del overview). Queda registrada como hecho, no como conclusión.

## Beliefs

Referenciadas de `product/overview.md`, el registro único:

- [product] [value] (creencia 1) Los Team Leads comparten enlaces externos porque la colaboración nativa no cubre lo que necesitan hacer en vivo. Esta oportunidad es su instancia acotada al segmento.
- [product] [viability] (creencia 4) IT no sube a Max porque no puede ver qué valor concreto sacan sus Team Leads. Adyacente: explica por qué el resultado elegido es el upgrade.

Registradas para esta oportunidad:

- [opportunity: colaboracion-en-vivo-fuera-de-teams] [value] En las cuentas del segmento, la mayoría de los Team Leads que comparten un enlace externo en reuniones de más de 5 participantes lo hacen sobre un artefacto creado para esa reunión, y pierden 5 minutos o más por reunión en accesos y entradas fallidas. Se falsa si el artefacto mayormente preexiste y tiene vida propia fuera de la reunión, o si el costo de acceso resulta marginal.
- [opportunity: colaboracion-en-vivo-fuera-de-teams] [viability] Resolver este problema mueve la tasa de upgrade a Max del segmento por encima del 3,1% actual. Se falsa si las cuentas del segmento con más uso de enlaces externos no suben de plan en mayor proporción que las que no los usan, o si IT declara que el freno es precio y no valor visible.

## Research agenda

| Belief      | Instrument                                                                                                                                                                 | Decision it unlocks                                                                                                | By when    |
| ----------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ | ---------- |
| [value]     | Datos propios: analizar los enlaces del 29% (dominio y antigüedad del recurso cuando el dominio lo permita) y el silencio inicial de la reunión tras pegarlos              | Si el artefacto preexiste, esta oportunidad se reformula como integración y no como colaboración en vivo           | 30/09/2026 |
| [viability] | Datos propios: cruzar tasa de upgrade entre cuentas del segmento con alto y bajo uso de enlaces externos                                                                   | Si no hay correlación, el problema puede ser real y aun así no mover el upgrade, y hay que buscar otro resultado   | 30/09/2026 |
| [value]     | `/research-market`: qué venden y cuánto cobran Miro, Mural y FigJam, y si su uso dominante es en vivo o asíncrono                                                          | Si el mercado muestra uso mayormente asíncrono, la restricción de tiempo real vuelve al patrocinador para revisión | 14/10/2026 |
| [value]     | `/design-survey` a Team Leads del segmento (n≈300, con bloque de opt-in para entrevistas): cuántos salen, cada cuánto, cuántos minutos, cuántos quedan afuera              | Confirma o tumba el umbral de 5 minutos y la mayoría de artefactos creados para la reunión                         | 28/10/2026 |
| [value]     | `/design-interview` con 8 a 12 Team Leads reclutados del opt-in, priorizando los que contradicen la creencia (los que no salen, y los que salen y dicen que no les cuesta) | Qué actividad concreta se hace afuera, que es lo que cualquier solución tendría que cubrir                         | 11/11/2026 |
| [viability] | Entrevistas con IT (perfil Damián) en 5 a 8 cuentas del segmento que no subieron a Max                                                                                     | Si el freno es precio y no valor visible, esta oportunidad no sirve a este resultado                               | 11/11/2026 |

Corte de decisión: **15/11/2026**, tres meses antes de CollabCon.

## Candidate ideas (not evaluated)

- "Herramientas colaborativas integradas" en la reunión (del planteo de entrada)
- Whiteboard con plantillas, votación y movimiento rápido de tarjetas (frustración de Carolina)
- Captura de decisiones y envío automático a Jira y al acta (frustración de Carolina, apunta a otro problema)
- Panel por cuenta que muestre a IT el valor de reunión obtenido (frustración de Damián, apunta a la creencia 4 del registro)
