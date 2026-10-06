# Microsoft Teams

mode: existing · commercial

Herramienta de comunicación y colaboración de Microsoft 365: chat, reuniones, llamadas y archivos, integrada con Word, Excel, PowerPoint y Outlook. En el mercado desde 2017, en producción, con cientos de millones de usuarios activos mensuales. Se vende como licencia por usuario dentro de los planes de M365 (Business Basic → Standard → Premium → Max; el salto Premium → Max cuesta USD 8/usuario/mes), con renovación anual por cuenta.

## Para quién

Organizaciones que ya usan Microsoft 365. El **comprador** es el área de IT, que contrata y despliega; los empleados reciben la herramienta instalada, sin elegirla. El 71% de las cuentas tiene menos de 100 licencias, el 24% entre 100 y 1.000, y el 5% con más de 1.000 concentra el 58% de las licencias totales.

Dentro de la organización, el **usuario que conduce** son los Team Leads y mandos medios: convocan y dirigen las reuniones, el módulo más usado. El resto participa.

## Lo que sabemos

- Reuniones es el módulo dominante: 82% de usuarios activos participa en ≥1 reunión/semana; chat diario 64%; archivos 31%; llamadas 1:1 22% — *telemetría de uso*.
- El usuario corporativo promedio pasa 11,4 h/semana en reuniones; 41% de las reuniones tiene >8 participantes y 23% dura más de una hora — *telemetría*.
- Uso de funciones de reunión: compartir pantalla 67%, chat 44%, reacciones 38%, grabación 21%, salas pequeñas 9%, notas 8%, Whiteboard 5% — *telemetría*.
- En el 29% de las reuniones de >5 participantes se comparte en el chat un enlace externo: Google Docs/Notion, Miro/Mural/FigJam, Jira, dashboards o presentaciones — *telemetría de chat de reunión*.
- El 37% de las organizaciones tiene Slack o Google Chat activo en al menos un equipo — *dato de cuentas*.
- Los archivos viven en SharePoint; el 46% de los tickets del módulo Archivos es "no encuentro el archivo" — *tickets de soporte*.
- Quejas post-reunión: audio/video 34%, "demasiadas reuniones / demasiado largas" 26%, colaboración durante la reunión 19%, notificaciones y ruido 12%, otros 9% — *encuestas post-reunión*.
- Renovación últimos 12 meses: 94% renovó, 2,4% subió de plan, 3,6% bajó o no renovó. Motivos de baja, en orden: "pagamos por funciones que no usamos", "costo", "el equipo ya usa otras herramientas" (sin especificar) — *datos de renovación y encuesta de salida*.

## Creencias no verificadas

Ordenadas por impacto × incertidumbre; la primera es la próxima a atacar.

Orden de ataque al 29/09/2026: 9, 4, 8, 11, 10, 6, 7. Las 1, 2, 3 y 5 ya tienen evidencia en contra.

1. [product] [value] Los Team Leads comparten enlaces externos (Miro, Docs, Jira) en las reuniones grandes porque la colaboración nativa de Teams no cubre lo que necesitan hacer en vivo — no por hábito ni porque esos artefactos ya vivan afuera. Si Teams cubriera esa necesidad, dejarían de salir. — weakened by [product/insights/2026-09-29-1931-colaboracion-en-vivo-fuera-de-teams.md] (2026-09-29)
   — contradicted by [product/insights/2026-09-29-2000-entrevistas-colaboracion-en-vivo-fuera-de-teams.md] (2026-09-29)

2. [opportunity: colaboracion-en-vivo-fuera-de-teams] [value] En las cuentas del segmento en foco (Business Premium, 100+ licencias, tecnología, 3+ países, facturación > USD 100M), la mayoría de los Team Leads que comparten un enlace externo en reuniones de más de 5 participantes lo hacen sobre un artefacto creado para esa reunión, y pierden 5 minutos o más por reunión en accesos y entradas fallidas. Se falsa si el artefacto mayormente preexiste y tiene vida propia fuera de la reunión, o si el costo de acceso resulta marginal. — weakened by [product/insights/2026-09-29-1931-colaboracion-en-vivo-fuera-de-teams.md] (2026-09-29)
   — contradicted by [product/insights/2026-09-29-2000-entrevistas-colaboracion-en-vivo-fuera-de-teams.md] (2026-09-29)
   (oportunidad descartada el 2026-09-29, reencuadrada en decisiones-sin-cierre-en-reuniones y convergencia-trabada-en-reuniones)

3. [product] [value] El bajo uso de Whiteboard (5%) y notas (8%) se debe a que los Team Leads no las consideran adecuadas para su reunión, no a que no sepan que existen. Más descubrimiento no cambiaría el uso. — weakened by [product/insights/2026-09-29-1931-colaboracion-en-vivo-fuera-de-teams.md] (2026-09-29)
   — contradicted by [product/insights/2026-09-29-2000-entrevistas-colaboracion-en-vivo-fuera-de-teams.md] (2026-09-29)

4. [product] [viability] IT no sube a Max porque no puede ver qué valor concreto sacan *sus* Team Leads de las "capacidades avanzadas de reuniones". Si ese valor fuera visible por cuenta, la tasa de upgrade superaría el 2,4%.

5. [opportunity: colaboracion-en-vivo-fuera-de-teams] [viability] Resolver este problema mueve la tasa de upgrade a Max del segmento por encima del 3,1% actual. Se falsa si las cuentas del segmento con más uso de enlaces externos no suben de plan en mayor proporción que las que no los usan, o si IT declara que el freno es precio y no valor visible. — weakened by [product/research/2026-09-15-2126-colaboracion-en-vivo-fuera-de-teams.md] (2026-09-16)
   (oportunidad descartada el 2026-09-29, reencuadrada en decisiones-sin-cierre-en-reuniones y convergencia-trabada-en-reuniones)

6. [product] [value] Los mandos medios aceptarían reemplazar parte de sus reuniones por alternativas asíncronas dentro de Teams (resúmenes, decisiones, seguimiento) si la herramienta las ofreciera — la queja "demasiadas reuniones" es una oportunidad de producto, no un problema cultural fuera de alcance.

7. [product] [viability] La baja de plan por "pagamos por funciones que no usamos" se concentra en cuentas de menos de 100 licencias cuyo plan no coincide con su uso real — es un problema de ajuste de plan, no de producto.

8. [opportunity: decisiones-sin-cierre-en-reuniones] [value] En el segmento, la mayoría de los líderes que conducen reuniones de más de 5 con decisiones dedica 10 minutos o más después de la reunión a registrarlas o pasarlas a mano (acta, Jira, correo, corregir el recap), y en sus equipos al menos una decisión por mes se ejecuta distinto, tarde o no se ejecuta por dueño ambiguo o registro incorrecto. Se falsa si la mediana del trabajo posterior es menor a 10 minutos o si esas fallas son menos que mensuales.

9. [opportunity: decisiones-sin-cierre-en-reuniones] [viability] Resolver el cierre de decisiones mueve la tasa de upgrade a Max del segmento por encima del 3,1%. Se falsa si, en 5 a 8 entrevistas con IT de cuentas del segmento que no subieron, el freno declarado es precio y no valor visible, o si el cierre de decisiones no aparece entre lo que justificaría el salto.

10. [opportunity: convergencia-trabada-en-reuniones] [value] En la mayoría de las reuniones de más de 5 del segmento donde el grupo prioriza o decide, la priorización se traba 10 minutos o más y la cierra el líder por tiempo, o al menos un participante presente no llega a expresar su prioridad. Se falsa si eso pasa en menos de la mitad de esas reuniones.

11. [opportunity: convergencia-trabada-en-reuniones] [viability] El uso de herramientas externas para converger (pizarras y votación) pesa en la baja o no renovación: las cuentas del segmento que bajaron o no renovaron por "el equipo ya usa otras herramientas" tienen más uso de esas herramientas en reuniones que las que renovaron. Se falsa si no hay diferencia.

12. [feature: cierre-confirmado-en-vivo] [usability] Los grupos del segmento reservan y usan 2 a 3 minutos al final de la reunión para confirmar la lista de decisiones. Se falsa si, en un piloto de 4 semanas con 8 a 10 líderes, el cierre se saltea en más de la mitad de las reuniones con decisiones. (de product/solutions/2026-09-29-2055-decisiones-sin-cierre-en-reuniones.md)

13. [feature: cierre-confirmado-en-vivo] [value] Que cada responsable confirme su decisión antes de cortar reduce las decisiones mal ejecutadas. Se falsa si, en el mismo piloto, las decisiones ejecutadas distinto, tarde o no ejecutadas no bajan al menos a la mitad contra el mes anterior. (de product/solutions/2026-09-29-2055-decisiones-sin-cierre-en-reuniones.md)

14. [feature: recap-de-decisiones] [feasibility] La IA extrae decisión, responsable y fecha y separa propuesta de decisión con precisión suficiente para publicarse tras una revisión corta. Se falsa si, sobre grabaciones reales, más de 1 de cada 5 decisiones extraídas es incorrecta o falta, o si la revisión del líder lleva más de 5 minutos. (de product/solutions/2026-09-29-2055-decisiones-sin-cierre-en-reuniones.md)

15. [feature: recap-de-decisiones] [value] Los líderes publican la lista de decisiones de la IA, revisada, en lugar de armar su propio registro. Se falsa si, mostrada la lista de su propia reunión, menos de la mitad la publica o la manda en lugar de su acta, correo o carga en Jira. (de product/tests/2026-10-06-1914-decisiones-sin-cierre-en-reuniones.md)
