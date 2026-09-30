---
status: framed
segment: Líderes (Team Leads, Engineering/Product/Design Leads, mandos medios) que conducen reuniones de más de 5 participantes en las que el grupo prioriza o decide, en cuentas Business Premium de 100+ licencias, sector tecnología, operación en 3+ países, facturación > USD 100M (12.400 cuentas, 2,1M licencias)
personas: carolina-restrepo (sufre), joaquin-lemus (sufre, parcial), rosa-elena-cabrera (sufre, como quien queda afuera), damian-sosa (no sufre, responde la viabilidad), bruno-tavella (no sufre)
---

# Opportunity: En las reuniones grandes el grupo no logra converger

En las reuniones de más de 5 participantes donde el grupo tiene que priorizar o decidir, no hay una forma de que cada uno marque su prioridad sin que se vuelva conversación: se vota contando manos o reacciones, la priorización se traba 10 a 20 minutos y la cierra el líder por tiempo, parte de los presentes no llega a opinar y el desacuerdo aparece después. Para converger, los equipos salen a pizarras y herramientas de votación externas. Importa ahora porque "el equipo ya usa otras herramientas" es el tercer motivo de baja o no renovación, y la pizarra nativa se prueba y se abandona.

Reencuadre de `product/opportunities/2026-09-15-2036-colaboracion-en-vivo-fuera-de-teams.md` (descartada el 29/09/2026). El cierre de decisiones se encuadró aparte en `product/opportunities/2026-09-29-2050-decisiones-sin-cierre-en-reuniones.md`.

## Segment and personas

- **Carolina Restrepo** (primary): sufre. Retro quincenal en Miro por falta de votación y plantillas en Whiteboard; los de Lima hablan la mitad que los de Bogotá. Fuera de la firmografía (servicios financieros).
- **Joaquín Lemus** (primary): sufre en parte. Solo converge en grupo en el planning trimestral (22 personas, FigJam, dos contratistas mirando la pantalla); no lo vive como su problema principal.
- **Rosa Elena Cabrera** (tertiary): sufre, del lado de quien queda afuera. No abre el enlace externo y no participa; en 7 de 11 reuniones no habla. Fuera de la firmografía.
- **Damián Sosa** (secondary): no sufre. Responde la viabilidad: quiere eliminar el shadow IT y defender "una sola plataforma" en la renovación.
- **Bruno Tavella** (negative): no sufre este problema. Quiere que converger en FigJam, fuera de Teams, sea más cómodo; construir para él financia la fuga. Los hallazgos que dependen de externos son señal de alarma.
- **Faltante:** el participante de una cuenta del segmento que no llega a opinar (nuevo, junior, de otro país u horario, sin acceso). Hay evidencia real para construirla (`/derive-personas` sobre las entrevistas).

## Signals

| Signal | Provenance | Source |
|---|---|---|
| En 6 de 10 la priorización se trabó (10 a 20 min) y la cerró el líder por falta de tiempo | real | `product/insights/2026-09-29-2000-entrevistas-colaboracion-en-vivo-fuera-de-teams.md` (n=10) |
| 8 de 10 nombran personas que casi no intervinieron; en 3 casos la objeción apareció después (café, mensaje privado, "con cara de que no") | real | ídem |
| 4 de 10 votan contando manos o reacciones, o con un tablero que no limita votos | real | ídem |
| Whiteboard: 4 de 5 que la usaron la abandonaron; 3 de 5 no la encontraron para la reunión siguiente; sin votación ni plantillas, lenta con 9 a 14 personas | real | ídem |
| Quienes siguen en Miro lo explican por la continuidad entre sesiones | real | ídem (Tomás, Javier) |
| Votar o priorizar es la actividad más hecha fuera de Teams (40%); en artefactos creados para la reunión, votar 56%, aportar ideas 47%, agrupar 47% | survey | `product/insights/2026-09-29-1931-colaboracion-en-vivo-fuera-de-teams.md` (n=182) |
| El 26% de las reuniones que salen de Teams usa solo pizarra o votación, y el 83% de esos artefactos se crea para la reunión | survey | ídem |
| En el 47% de las reuniones internas al menos una persona siguió mirando la pantalla de otro | survey | ídem (n=143) |
| Whiteboard: 8% no la conocía, 43% la usó y la dejó | survey | ídem (n=210) |
| 3,6% bajó o no renovó; tercer motivo "el equipo ya usa otras herramientas", sin especificar cuáles | survey | `product/overview.md` (n no declarado) |
| En el mercado la cocreación en reuniones va en la base o gratis (Whiteboard, Loop, Webex, IA de Mural) | secondary | `product/research/2026-09-15-2126-colaboracion-en-vivo-fuera-de-teams.md` |
| Miro, Mural, FigJam y Lucidspark ya tienen app con votación dentro de reuniones de Teams | secondary | ídem |
| Whiteboard 5% de uso en reuniones | real | telemetría, `product/overview.md` |

## Business outcome

Comercial: **retención en la renovación** del segmento. El research indica que la cocreación no se cobra en el mercado, así que esta oportunidad no se defiende como palanca de upgrade sino como defensa contra la baja por "el equipo ya usa otras herramientas" y contra el shadow IT que le rompe a IT el discurso de una sola plataforma.

## Constraints

- Presupuesto máximo USD 5M.
- Presentación en CollabCon en 5 meses (aprox. 16/02/2027).
- Límites declarados por el patrocinador: facilidad de uso, accesibilidad, compatibilidad con Microsoft 365, privacidad y seguridad corporativas, tiempo real, impacto mínimo en el rendimiento de la reunión. En esta oportunidad "tiempo real" no recorta nada: converger ocurre durante la reunión.
- Compliance: en cuentas que no pueden usar herramientas externas, lo nativo es la única opción y su calidad decide si la actividad se hace (Lucía, España, `real`; R-190, R-009, R-143, `survey`).
- Externos: Microsoft deja a los externos usar Whiteboard solo durante la reunión y si el admin lo habilita (`secondary`). Cualquier alcance que dependa de externos acerca la oportunidad a Bruno.

## Beliefs

Referenciadas de `product/overview.md`, el registro único:

- [product] [value] (creencia 1) Los Team Leads comparten enlaces externos porque la colaboración nativa no cubre lo que necesitan en vivo. Contradicha en general; se sostiene solo para la cocreación en pizarra, que es el terreno de esta oportunidad.
- [product] [value] (creencia 3) El bajo uso de Whiteboard se debe a que no la consideran adecuada. Contradicha para notas y apps (descubrimiento); para Whiteboard la evidencia apunta a lo que le falta.

Registradas para esta oportunidad:

- [opportunity: convergencia-trabada-en-reuniones] [value] En la mayoría de las reuniones de más de 5 del segmento donde el grupo prioriza o decide, la priorización se traba 10 minutos o más y la cierra el líder por tiempo, o al menos un participante presente no llega a expresar su prioridad. Se falsa si eso pasa en menos de la mitad de esas reuniones.
- [opportunity: convergencia-trabada-en-reuniones] [viability] El uso de herramientas externas para converger (pizarras y votación) pesa en la baja o no renovación: las cuentas del segmento que bajaron o no renovaron por "el equipo ya usa otras herramientas" tienen más uso de esas herramientas en reuniones que las que renovaron. Se falsa si no hay diferencia.

## Research agenda

| Belief | Instrument | Decision it unlocks | By when |
|---|---|---|---|
| [viability] | Datos propios: sumar a la telemetría las apps de terceros compartidas al stage (hoy solo se ven enlaces en el chat) y cruzar uso de pizarras y votación externas con baja o no renovación y su motivo | Si no hay diferencia, la oportunidad no sirve a la retención y se estaciona | 15/10/2026 |
| [value] | `/design-survey` corta al pool de opt-in y como bloque en la próxima ola: última reunión de priorización, cuánto se trabó, quién cerró, cuántos no marcaron su prioridad | Confirma o tumba "la mayoría de las reuniones de priorización" a escala de encuesta | 28/10/2026 |
| [value] | `/design-interview` con 3 a 5 participantes que no conducen, incluidos los que casi no opinan | Si quien no opina no lo vive como problema, el dolor es solo del líder y cambia qué hay que resolver | 11/11/2026 |
| [viability] | Entrevistas con IT (perfil Damián), en la misma ronda de la otra oportunidad: si converger en herramientas externas pesa en la renovación y en su discurso de una sola plataforma | Si IT no lo conecta con la renovación, el resultado elegido no es el correcto | 11/11/2026 |

Corte de decisión: **15/11/2026**, tres meses antes de CollabCon.

## Candidate ideas (not evaluated)

- "Herramientas colaborativas integradas" en la reunión (del planteo de entrada del brief original)
- Whiteboard con plantillas, votación y movimiento rápido de tarjetas (del brief original, frustración de Carolina)
- Tablero y notas anclados al equipo o la serie, no a una instancia de reunión, con acceso a la sesión anterior (de la síntesis de entrevistas)
- Votación nativa dentro de la llamada con límite de votos y conteo automático (de la síntesis de entrevistas)
- Ver quién no opinó durante la priorización (de la síntesis de entrevistas)
