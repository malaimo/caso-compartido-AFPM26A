---
status: framed
segment: Líderes (Team Leads, Engineering/Product/Design Leads, mandos medios) que conducen reuniones de más de 5 participantes en las que se toma una decisión que otros ejecutan, en cuentas Business Premium de 100+ licencias, sector tecnología, operación en 3+ países, facturación > USD 100M (12.400 cuentas, 2,1M licencias)
personas: carolina-restrepo (sufre), joaquin-lemus (sufre), rosa-elena-cabrera (sufre, como receptora), damian-sosa (no sufre, responde la viabilidad), bruno-tavella (no sufre)
---

# Opportunity: Las decisiones de las reuniones grandes no se cierran

En las reuniones de más de 5 participantes de las cuentas de tecnología multinacionales, nadie cierra la decisión con qué se decidió, quién lo hace, para cuándo y por qué: el líder la reconstruye a mano después (acta, Jira, correo, corrigiendo el recap de IA) y, cuando falla, lo decidido se ejecuta distinto, tarde o no se ejecuta, con costos de días o semanas. Importa ahora porque el recap de IA, que es lo que hoy se cobra en el plan superior, falla justo en separar decisiones de conversación, y el segmento convierte a Max por encima del promedio (3,1% contra 2,4%) sin que IT pueda nombrar qué valor concreto obtiene.

Reencuadre de `product/opportunities/2026-09-15-2036-colaboracion-en-vivo-fuera-de-teams.md` (descartada el 29/09/2026). La convergencia en vivo se encuadró aparte en `product/opportunities/2026-09-29-2050-convergencia-trabada-en-reuniones.md`.

## Segment and personas

- **Carolina Restrepo** (primary): sufre. Pasa 30 a 45 minutos después de cada refinamiento copiando decisiones a Jira y al acta; dos o tres veces por trimestre algo se pierde y el equipo construye lo que no era. Fuera de la firmografía (servicios financieros).
- **Joaquín Lemus** (primary): sufre. Las decisiones se registran en un hilo de Slack que Teams nunca ve; dos veces en el trimestre Madrid implementó una versión anterior (unos 4 días de retrabajo cada vez). Es la persona del segmento en foco.
- **Rosa Elena Cabrera** (tertiary): sufre, del lado de quien recibe. "Nadie escribe qué se decidió"; quiere salir sabiendo qué le toca y para cuándo. Fuera de la firmografía (logística, 180 empleados).
- **Damián Sosa** (secondary): no sufre. Responde la creencia de viabilidad: no puede defender el salto a Max sin un uso concreto que mostrar.
- **Bruno Tavella** (negative): no sufre este problema. Su dolor es entrar como externo, que no es el de esta oportunidad.
- **Faltante:** el participante de una cuenta del segmento que ejecuta lo decidido sin conducir la reunión (la "Gloria de soporte" de Valeria, el líder de Ecuador de Andrés). Hay evidencia real para construirla (`/derive-personas` sobre las entrevistas).

## Signals

| Signal | Provenance | Source |
|---|---|---|
| 10 de 10 líderes contaron un caso reciente en que algo decidido se ejecutó distinto, tarde o no se hizo; costos de 20 min a 2 semanas (cliente 4 días sin atención, release movida, 1 semana de 2 desarrolladores) | real | `product/insights/2026-09-29-2000-entrevistas-colaboracion-en-vivo-fuera-de-teams.md` (n=10) |
| 8 de 10 hacen trabajo manual después de la reunión para dejar registro (10 a 60 min) y dicen que "nadie más lo hace" | real | ídem |
| Tres modos de falla: dueño ambiguo (3), registro tardío, escondido o en otro lugar (4), registro incorrecto hecho por la IA (1 con costo, 6 con quejas) | real | ídem |
| 6 de 10 usan o probaron el recap de IA; ninguno lo usa como registro de decisiones; marca propuestas como decisiones, no dice quién se comprometió, no ve lo que pasó en el tablero | real | ídem |
| Registrar, seguir y retomar lo decidido es el tema más mencionado de lo más difícil (34 de 95 respuestas abiertas) | survey | `product/insights/2026-09-29-1931-colaboracion-en-vivo-fuera-de-teams.md` (n=210) |
| En el 24% de las reuniones lo decidido no quedó registrado; solo el 13% quedó dentro de Teams; 23% en chats fuera de Teams | survey | ídem (n=182) |
| 26 de 32 respuestas "Otro" sobre dónde quedó lo decidido son recap de IA o transcripción, casi siempre con salvedad ("resume todo pero no distingue lo decidido") | survey | ídem |
| Microsoft Research: la información de las reuniones se reutiliza de forma asíncrona (tareas, inclusión de ausentes) y notas y grabaciones cumplen mal ese papel | secondary | `product/research/2026-09-15-2126-colaboracion-en-vivo-fuera-de-teams.md` |
| En el mercado lo que se cobra en planes superiores es IA (Copilot, E7, AI Companion), no cocreación | secondary | ídem |
| 5% de pilotos de Copilot pasa a despliegue amplio; el ROI es difícil de demostrar | secondary | ídem (Gartner 2025) |
| Carolina pierde 30 a 45 min por refinamiento en traspasos; Joaquín pierde unos 4 días de retrabajo por decisión leída en el hilo equivocado | synthetic | `product/personas/carolina-restrepo.md`, `product/personas/joaquin-lemus.md` |
| Damián no puede defender el salto a Max (USD 110.000/año) porque solo tiene una lista de capacidades | synthetic | `product/personas/damian-sosa.md` |

## Business outcome

Comercial: **tasa de upgrade a Max** del segmento como métrica líder (3,1% hoy; 96,9% del segmento no subió). Un punto porcentual de las 2,1M licencias del segmento son unos USD 2M anuales (cálculo derivado, no señal). La hipótesis de negocio es que un cierre de decisiones que funcione es un valor que IT puede nombrar y medir (minutos de seguimiento, decisiones sin responsable), que es lo que hoy le falta a Damián.

## Constraints

- Presupuesto máximo USD 5M.
- Presentación en CollabCon en 5 meses (aprox. 16/02/2027).
- Límites declarados por el patrocinador: facilidad de uso, accesibilidad, compatibilidad con Microsoft 365, privacidad y seguridad corporativas, tiempo real, impacto mínimo en el rendimiento de la reunión.
- **"Tiempo real" en revisión:** las fallas de esta oportunidad ocurren en el cierre y después de la reunión (registro tardío, dueño ambiguo, lo decidido no llega a quien no estuvo). La restricción sigue vigente como hecho y se lleva al patrocinador con esta evidencia (ver agenda).
- Compliance: hay cuentas donde lo nativo es la única opción porque no pueden usar herramientas externas con datos de clientes (Lucía, España, `real`; R-190 y R-009, `survey`).
- Regulación en el EEE: desde 09/2025 Microsoft debe ofrecer suites sin Teams con mayor diferencia de precio; atar una función de Teams al plan superior en cuentas con operación en el EEE necesita confirmación de legal (`secondary`).

## Beliefs

Referenciadas de `product/overview.md`, el registro único:

- [product] [viability] (creencia 4) IT no sube a Max porque no puede ver qué valor concreto sacan sus Team Leads. La viabilidad de esta oportunidad es su instancia acotada.

Registradas para esta oportunidad:

- [opportunity: decisiones-sin-cierre-en-reuniones] [value] En el segmento, la mayoría de los líderes que conducen reuniones de más de 5 con decisiones dedica 10 minutos o más después de la reunión a registrarlas o pasarlas a mano (acta, Jira, correo, corregir el recap), y en sus equipos al menos una decisión por mes se ejecuta distinto, tarde o no se ejecuta por dueño ambiguo o registro incorrecto. Se falsa si la mediana del trabajo posterior es menor a 10 minutos o si esas fallas son menos que mensuales.
- [opportunity: decisiones-sin-cierre-en-reuniones] [viability] Resolver el cierre de decisiones mueve la tasa de upgrade a Max del segmento por encima del 3,1%. Se falsa si, en 5 a 8 entrevistas con IT de cuentas del segmento que no subieron, el freno declarado es precio y no valor visible, o si el cierre de decisiones no aparece entre lo que justificaría el salto.

## Research agenda

| Belief | Instrument | Decision it unlocks | By when |
|---|---|---|---|
| [value] | Datos propios: uso del recap de IA en cuentas que lo tienen (generado, abierto, editado, compartido) y reuniones de la misma serie donde se reabre un tema | Si el recap casi no se abre o se edita siempre, la solución no puede apoyarse en el recap tal como está | 15/10/2026 |
| [value] | `/design-survey` corta al pool de opt-in (64 elegibles) y como bloque en la próxima ola: minutos de trabajo después de la reunión, decisiones mal ejecutadas el último mes, modo de falla | Confirma o tumba los umbrales de 10 minutos y falla mensual a escala de encuesta | 28/10/2026 |
| [value] | `/design-interview` con 3 a 5 participantes que ejecutan sin conducir (del lado de Rosa Elena y la persona faltante) | Si quien recibe no sufre el problema, la solución es solo para el líder y el valor se achica | 11/11/2026 |
| [viability] | Entrevistas con IT (perfil Damián) en 5 a 8 cuentas del segmento que no subieron a Max | Si el freno es precio y no valor visible, esta oportunidad no sirve al upgrade y hay que moverla a retención | 11/11/2026 |
| (restricción) | Reunión con el patrocinador con la evidencia de cierre posterior a la reunión | Si "tiempo real" se mantiene, las alternativas quedan limitadas al cierre dentro de la llamada | 15/10/2026 |

Corte de decisión: **15/11/2026**, tres meses antes de CollabCon.

## Candidate ideas (not evaluated)

- Captura de decisiones y envío automático a Jira y al acta (del brief original, frustración de Carolina). `parked` como A3, ver [product/solutions/2026-09-29-2055-decisiones-sin-cierre-en-reuniones.md](../solutions/2026-09-29-2055-decisiones-sin-cierre-en-reuniones.md)
- Panel por cuenta que muestre a IT el valor de reunión obtenido (del brief original, frustración de Damián; apunta a la viabilidad). `parked` como A5, ver [product/solutions/2026-09-29-2055-decisiones-sin-cierre-en-reuniones.md](../solutions/2026-09-29-2055-decisiones-sin-cierre-en-reuniones.md)
- Recap de IA que separe propuesta de decisión y extraiga responsable, fecha y motivo (de la síntesis de entrevistas). `chosen` como A1, en prueba, ver [product/solutions/2026-09-29-2055-decisiones-sin-cierre-en-reuniones.md](../solutions/2026-09-29-2055-decisiones-sin-cierre-en-reuniones.md)
- Cierre de la reunión con lista de decisión, responsable, fecha y motivo confirmada en vivo por el grupo (de la síntesis de entrevistas). `chosen` como A2, en prueba, ver [product/solutions/2026-09-29-2055-decisiones-sin-cierre-en-reuniones.md](../solutions/2026-09-29-2055-decisiones-sin-cierre-en-reuniones.md)
- Publicar lo decidido donde vive el trabajo: Jira, Confluence, canal, correo (de la síntesis de entrevistas). `parked` como A3, ver [product/solutions/2026-09-29-2055-decisiones-sin-cierre-en-reuniones.md](../solutions/2026-09-29-2055-decisiones-sin-cierre-en-reuniones.md)
