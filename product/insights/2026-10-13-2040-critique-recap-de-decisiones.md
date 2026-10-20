---
type: persona-critique
spec: product/specs/2026-10-13-1945-recap-de-decisiones.md
panel: joaquin-lemus (primary), carolina-restrepo (primary)
date: 2026-10-13
source: synthetic
---

# Panel de crítica: Recap de IA centrado en decisiones

Composición: 2 primary (Joaquín Lemus, Carolina Restrepo). Panel elegido por el usuario. Sin voz tertiary ni negative, así que la lectura tiende a ser complaciente en compra, permisos y alcance (ver cierre).

Todo lo que sigue es `synthetic`: sirve para revisar la spec, no como evidencia de valor.

### Joaquín Lemus: Engineering Manager, checkout SaaS B2B · primary

**Overall rating:** 3/5

**Strengths:**
- Separar decisiones de propuestas es justo lo que me falta. Si la lista hubiera dicho "Madrid implementa la versión 2 del acuerdo, responsable Iker, para el viernes", me ahorraba dos veces 4 días de retrabajo.
- Que cada ítem muestre la frase y el minuto me da confianza para revisar rápido. No tengo que volver a escuchar la grabación entera.
- Que la IA ponga "sin responsable" en vez de inventar uno está bien. Prefiero un hueco visible a un nombre equivocado.
- Una sola versión revisada por mí, que lea todo el equipo, es lo que hoy no existe: hoy hay un hilo y nadie sabe cuál es el bueno.

**Concerns:**
- La lista termina en el chat de la reunión de Teams. Mi equipo vive en Slack y la documentación técnica en Confluence. Ya me pasó con Loop: la página de decisiones quedó huérfana a la semana porque no estaba donde la gente busca. Esto puede terminar igual.
- Quiero encontrar por qué decidimos algo dentro de seis meses. En un chat de reunión, eso se pierde en el scroll. La spec no dice cómo se encuentra una decisión vieja.
- En el planning trimestral tengo 4 contratistas de Madrid con cuenta externa. Si por defecto los externos no ven la lista, justo los que implementan se quedan sin ella.
- Parte de lo que se decide queda en el hilo de Slack que se abre durante la reunión. La transcripción no lo ve, así que la lista va a estar incompleta y no me va a avisar.
- En la revisión de incidentes decimos "ese pico" mirando Grafana. Si la lista no sabe qué se estaba mirando, la decisión queda sin contenido.

**Suggestions:**
- Como mínimo, poder copiar la lista con formato y enlace a la reunión para pegarla en Confluence o Slack en un paso, aunque no haya integración.
- Una vista de las listas publicadas de una misma serie de reuniones, buscable, para encontrar decisiones viejas.
- Que el organizador elija externo por externo quién ve la lista, no todo o nada.
- Cuando una decisión hace referencia a algo de la pantalla ("esto", "ese gráfico"), marcarla para que yo la complete en la revisión.

Me sirve si me saca del hilo de Slack, pero si la lista queda encerrada en Teams, mi equipo la va a ignorar igual que ignora el recap de hoy.

### Carolina Restrepo: Team Lead de Operaciones de Producto · primary

**Overall rating:** 3/5

**Strengths:**
- Me ahorra el acta. Si la revisión me lleva 5 minutos en vez de 30 a 45, recupero las tardes de martes y jueves.
- La notificación al responsable me gusta: hoy soy yo la que persigue a cada uno para recordarle lo que le tocó.
- Una lista publicada con "revisada por Carolina" le muestra a mi jefe que mis reuniones terminan en decisiones, no solo en asistencia.

**Concerns:**
- La mitad de mi trabajo después del refinamiento es pasar las decisiones a Jira. La spec deja Jira afuera, así que me ahorra el acta pero sigo copiando a mano. Es justo donde se me pierden cosas dos o tres veces por trimestre.
- En el refinamiento hablamos sobre el tablero de Jira en pantalla: "esta historia pasa al próximo sprint". Sin contexto de pantalla, la lista va a decir "una historia pasa al próximo sprint" y no sabré cuál.
- La retro la hago en Miro con votación por puntos. Lo que se decide ahí no se dice en voz alta, se vota. La lista no lo va a ver.
- Solo grabo las reuniones importantes. Si la lista depende de que haya grabación o transcripción, en muchas de mis reuniones no va a existir. La spec no dice qué pasa si no se grabó.

**Suggestions:**
- Si alguien dice en voz alta el código de un ticket (por ejemplo "OPS-214"), que la decisión lo muestre como enlace. Ya con eso, pasar a Jira se hace mucho más rápido.
- Decir en la spec qué ve el organizador cuando la reunión no tuvo transcripción: un aviso claro, no una lista vacía que parezca "no hubo decisiones".
- Dejar explícito que esto no sirve para decisiones tomadas por votación en un tablero, para que nadie lo espere.

Lo usaría desde la primera semana para el acta, pero no lo veo como el fin del trabajo manual mientras Jira siga quedando afuera.

## Síntesis

### Acuerdos (señal más fuerte)
- **Lo que valoran es lo mismo:** decisiones separadas de propuestas, la frase y el minuto como prueba, y "sin responsable" en vez de inventar. Ese es el núcleo de la spec y los dos lo confirman.
- **El valor se cae si la lista no llega a donde vive el trabajo.** Joaquín por Confluence y Slack, Carolina por Jira. Los dos dicen que, sin una salida, siguen copiando a mano. Esto apunta directo a la creencia 15 (que publiquen la lista en lugar de su registro propio) y a A3, que está aparcada.
- **Decisiones que dependen de la pantalla quedan sin contenido.** Grafana para Joaquín, el tablero de Jira para Carolina. El contexto de pantalla quedó fuera de esta versión por T2, y el panel muestra que eso pega en el caso más común de los dos.

### Conflictos (tensiones de diseño para decidir)
- **Externos:** Joaquín necesita que sus contratistas externos vean la lista; la regla por defecto "externos no ven" viene del caso de los invitados del cliente y de compliance. Opción intermedia: elegir externo por externo.
- **Velocidad hoy vs. registro a largo plazo:** Carolina quiere ahorrar tiempo esta semana; Joaquín quiere encontrar decisiones dentro de seis meses. La spec cubre lo primero y no lo segundo.

### Los 3 cambios de mayor impacto
1. **Agregar una salida mínima sin integración:** copiar la lista con formato y enlace a la reunión, y mostrar como enlace los códigos de ticket que se dicen en voz alta. No reabre A3, pero baja el riesgo de la creencia 15. Si se decide no hacerlo, dejar explícito en la spec que el ahorro es solo del acta.
2. **Marcar las decisiones que dependen de la pantalla** ("esto", "esa historia") para que el organizador las complete en la revisión. Mantiene el alcance de T2 y evita que una decisión sin contenido se publique como correcta (se conecta con la creencia 16).
3. **Cubrir dos casos que hoy no tienen criterio:** reunión sin transcripción (aviso claro, no lista vacía) y listas de la misma serie fáciles de encontrar después, también si la serie se recrea (el mismo problema que hizo abandonar Whiteboard).

### Límite del panel
Solo primary. Faltan las voces de quien paga y de quien recibe: **Damián Sosa** (IT, decide el salto a Max) y **Rosa Elena Cabrera** (tertiary, recibe la lista). Son las que pueden poner en duda la viabilidad y la historia de quien recibe.
