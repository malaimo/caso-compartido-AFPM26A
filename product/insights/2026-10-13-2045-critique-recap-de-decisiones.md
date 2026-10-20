---
type: persona-critique
spec: product/specs/2026-10-13-1945-recap-de-decisiones.md
spec_version: revisión del 13/10/2026 (salida en un paso, códigos de ticket, marca "falta contexto de pantalla")
previous: product/insights/2026-10-13-2040-critique-recap-de-decisiones.md
panel: joaquin-lemus (primary), carolina-restrepo (primary)
date: 2026-10-13
source: synthetic
---

# Panel de crítica (segunda ronda): Recap de IA centrado en decisiones

Composición: 2 primary (Joaquín Lemus, Carolina Restrepo), el mismo panel de la primera ronda. Sigue sin voz tertiary ni negative.

Todo lo que sigue es `synthetic`: sirve para revisar la spec, no como evidencia de valor.

### Joaquín Lemus: Engineering Manager, checkout SaaS B2B · primary

**Overall rating:** 4/5 (antes 3/5)

**Strengths:**
- Copiar la lista con formato y pegarla en Confluence resuelve lo que me preocupaba de Loop. La decisión termina donde mi equipo busca, y de paso me resuelve encontrarla dentro de seis meses: Confluence ya es buscable.
- La marca "falta contexto de pantalla" es honesta. Prefiero que me avise a que publique "ese pico se investiga" sin decir de qué gráfico.
- Que no publique nada solo en otras herramientas me tranquiliza. No tengo que pelear con IT por permisos de integración.

**Concerns:**
- En la revisión de incidentes casi todo se decide mirando Grafana. Si la mitad de las decisiones viene marcada, completar cada una me lleva más de 5 minutos. La marca puede romper la promesa de la revisión corta.
- Los contratistas externos siguen en todo o nada. En el planning trimestral los que implementan son justamente ellos.
- Lo que se decide en el hilo de Slack durante la reunión sigue sin aparecer, y la lista no avisa que puede faltar algo.
- Copiar y pegar depende de que yo me acuerde. La primera semana lo hago; la cuarta, no sé.

**Suggestions:**
- Medir en T2 cuántas decisiones salen marcadas por reunión. Si son muchas, la marca se vuelve ruido.
- Elegir externo por externo quién ve la lista.
- Que la lista publicada diga "decisiones detectadas en la conversación" para que nadie asuma que incluye lo del chat o Slack.

Ahora sí lo probaría en el refinamiento. En incidentes tengo dudas hasta ver cuántas marcas salen.

### Carolina Restrepo: Team Lead de Operaciones de Producto · primary

**Overall rating:** 3/5 (sin cambio)

**Strengths:**
- La marca de pantalla me sirve en el refinamiento: "esta historia pasa al próximo sprint" ya no se pierde, me obliga a decir cuál.
- Cuando alguien dice el código del ticket, tenerlo como enlace me ahorra buscarlo en el tablero.
- Pegar la lista en el acta del equipo es inmediato. Esa parte de mi trabajo casi desaparece.

**Concerns:**
- En el refinamiento casi nadie dice el código en voz alta. Decimos "la de arriba", "la de pagos". El enlace va a aparecer poco y lo que más va a aparecer es la marca.
- Pegar una lista en Jira no actualiza los tickets. Cada decisión toca un ticket distinto y tengo que ir a cada uno. Me ahorra el acta, no Jira, que es donde se me pierden cosas.
- El enlace depende de que la cuenta tenga configurada la dirección de Jira. Eso lo hace IT, no yo, y la spec no dice quién ni cuándo.
- Sigue sin estar qué pasa si la reunión no se grabó. En muchas de mis reuniones no grabo.

**Suggestions:**
- Si la decisión tiene marca de pantalla y se compartió el tablero de Jira, dejarme elegir el ticket de una lista en vez de escribirlo.
- Dejar escrito en la spec quién configura la dirección de Jira y qué ve el organizador si no está configurada.
- Agregar el criterio de reunión sin transcripción: aviso claro, no lista vacía.

Mejoró para el acta, pero mi problema caro sigue siendo Jira, y esto todavía no lo toca.

## Síntesis

### Qué cambió desde la primera ronda
- **Joaquín sube de 3 a 4:** la copia a Confluence resuelve dónde vive la decisión y cómo encontrarla después. Sus dos preocupaciones grandes de la primera ronda quedaron cubiertas.
- **Carolina se queda en 3:** el acta casi desaparece, pero su costo principal (pasar decisiones a tickets de Jira) sigue igual. La copia sirve para documentos, no para actualizar tickets.

### Acuerdos
- **La marca de pantalla es útil pero puede ser frecuente.** Los dos esperan que aparezca mucho (incidentes en Grafana, refinamiento sobre Jira). Si aparece en la mayoría de las decisiones, la revisión pasa de 5 minutos y choca con el umbral de la hipótesis y de la creencia 14.
- **El enlace al ticket va a aparecer poco:** los códigos rara vez se dicen en voz alta.

### Conflictos
- **Documentos vs. tickets:** para Joaquín la salida a un documento alcanza; para Carolina no, porque su trabajo es actualizar tickets. Resolverlo para Carolina empuja hacia A3 (aparcada).
- **Externos:** sigue abierto desde la primera ronda (Joaquín quiere elegir uno por uno).

### Los 3 cambios de mayor impacto
1. **Medir la frecuencia de la marca en T2** (decisiones marcadas por reunión y minutos que suma a la revisión) y fijar qué proporción vuelve inviable la revisión corta. Es la duda nueva que abrió la revisión.
2. **Cerrar los casos sin criterio:** reunión sin transcripción, y quién configura la dirección de Jira y qué pasa si no está.
3. **Decidir si la necesidad de Carolina (actualizar tickets) entra en esta versión o queda explícitamente afuera.** Si queda afuera, dejarlo dicho en la spec: el ahorro es del acta, no de Jira. Si entra, es reabrir A3.

### Límite del panel
Solo primary, igual que la primera ronda. La configuración de Jira y el caso de los externos son de permisos: **Damián Sosa** (IT) es la voz que falta para eso.
