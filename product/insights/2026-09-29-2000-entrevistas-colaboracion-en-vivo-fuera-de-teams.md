---
type: interview-synthesis
opportunity: colaboracion-en-vivo-fuera-de-teams
guide: product/interview-guides/2026-09-22-2030-colaboracion-en-vivo-fuera-de-teams.md
related: product/insights/2026-09-29-1931-colaboracion-en-vivo-fuera-de-teams.md (análisis de encuesta)
date: 2026-09-29
n: 10 entrevistas de exploración
sources:
  - product/interviews/2026-09-25-1000-tomas-aguirre.md (source: real, R-113, pool "confirman")
  - product/interviews/2026-09-25-1100-andres-quintero.md (source: real, R-170, pool "En ninguna")
  - product/interviews/2026-09-25-1600-lucia-fernandez.md (source: real, R-143, pool "En ninguna", compliance)
  - product/interviews/2026-09-28-0900-javier-molina.md (source: real, R-097, pool "confirman")
  - product/interviews/2026-09-28-0930-martina-rojas.md (source: real, R-224, pool "doble contradicción")
  - product/interviews/2026-09-28-1000-diego-paredes.md (source: real, R-036, pool "doble contradicción")
  - product/interviews/2026-09-28-1200-sofia-martinez.md (source: real, R-151, pool "doble contradicción")
  - product/interviews/2026-09-28-1400-paula-benitez.md (source: real, R-153, pool "En ninguna")
  - product/interviews/2026-09-28-1500-valeria-castro.md (source: real, R-024, pool "confirman")
  - product/interviews/2026-09-28-1700-ricardo-salinas.md (source: real, R-196, pool "En ninguna")
source: real
---

# Síntesis de entrevistas: colaboración en reuniones de más de 5 participantes

## Notas sobre el corpus

- 10 entrevistas reales, 26 a 34 min, 8 países de residencia de los equipos. Mezcla del pool de reclutamiento: 3 "confirman" la creencia 2, 3 "doble contradicción", 4 "En ninguna".
- **Tomás (R-113) corrigió su respuesta de encuesta:** había marcado que sale de Teams "en todas" las reuniones y aclaró que no es así ("Exageré un poco"). Conviene tenerlo en cuenta al leer el grupo "confirman".
- **Inconsistencia de fechas:** Paula (entrevista del 28/09) describe "el review de octubre", con notas armadas "el lunes 13". Posible error de transcripción o de fecha del archivo; no cambia el contenido del insight.
- Los encabezados de las entrevistas citan la guía `2026-09-23-2030-...`; el archivo existente es `2026-09-22-2030-...`.

## Insights, por impacto

## Cerrar la decisión no tiene dueño: el líder la reconstruye a mano y, cuando falla, cuesta días o semanas

**Recurrencia: 10 de 10.** Todos los entrevistados contaron un caso reciente en que algo decidido en la reunión terminó hecho distinto, tarde o no se hizo. 8 de 10 describen trabajo manual después de la reunión para dejarlo registrado: Tomás 20 min (Jira), Diego 20 min (correo), Andrés 30 min o más (correo), Lucía unos 30 min (Jira y correo), Javier unos 30 min (reescribe el recap), Valeria casi 1 h (Jira), Paula unos 10 min (corrige el resumen de IA), Sofía un par de minutos. Todos dicen "nadie más lo hace".

Los costos de las fallas: un cliente 4 días sin atención (Andrés), una incidencia 1 semana sin dueño (Lucía), una entrega 2 semanas tarde que movió una release (Javier), una campaña que siguió 3 días gastando (Diego), 2 semanas de trabajo que hubo que sacar (Sofía), 1 semana de 2 desarrolladores (Paula), 1 semana de un diseñador (Valeria), 2 días de arreglo y un fin de semana de guardia (Ricardo), una discusión reabierta de 20 min (Martina) y acuerdos perdidos que se volvieron a discutir (Tomás).

Hay tres modos de falla, y cada uno pide algo distinto:
1. **Dueño ambiguo** ("cada uno entendió que lo hacía el otro"): Andrés, Lucía, Ricardo.
2. **Registro tardío, escondido o en otro lugar**: correo que sale el miércoles (Diego), decisión en un hilo de comentarios marcado como resuelto y oculto (Sofía), el "por qué" solo en Slack (Martina), captura confusa pasada a Jira (Valeria).
3. **Registro incorrecto hecho por la IA**: ver el insight siguiente.

Implica explorar una capacidad que cierre la reunión con una lista de **decisión, responsable, fecha y motivo**, confirmada en vivo por el grupo antes de terminar, y que se publique donde vive el trabajo (Jira, Confluence, canal, correo). Métricas candidatas: minutos de trabajo del líder después de la reunión y decisiones sin responsable.

> Evidencia: "En mi correo quedó, pero el líder de Ecuador entendió que lo pasaba yo, y yo entendí que lo pasaba él. Nadie lo pasó." (Andrés Quintero). "Es trabajo mío, nadie más lo hace. Y si no lo hago, vuelve a pasar." (Javier Molina). "Lo que nos falla es cómo se cierra la reunión: que quede claro qué se decidió, que lo sepan todos, incluso los que no hablaron." (Sofía Martínez)

## El resumen de IA resume la conversación, no las decisiones, y a veces inventa decisiones

**Recurrencia: 6 de 10** lo usan o lo probaron (Lucía, Javier, Martina, Diego, Paula, Valeria). Ninguno lo usa como registro de decisiones. Fallas concretas: no dice quién se comprometió a qué (Lucía); pone todo al mismo nivel en dos páginas (Javier); es largo y nadie lo lee (Martina); no sabe qué número o filtro se estaba mirando (Diego); no ve lo que pasó en el tablero, como la votación (Valeria), ni lo decidido en Slack (Martina); y **marca propuestas como decisiones** (Paula, con 1 semana de 2 desarrolladores perdida). El caso de Javier muestra el riesgo de que el equipo lea solo el recap: la dependencia acordada con fecha quedó como "se habló de la API de geocercas" y se entregó 2 semanas tarde.

Esta es la capacidad que ya existe en el plan superior, y hoy genera trabajo en vez de ahorrarlo. Implica mejorar el recap para: separar propuesta de decisión, extraer responsable, fecha y motivo, tomar contexto de lo que se compartió en pantalla o en apps (votos, filtros, gráficos) y pedir confirmación del líder antes de publicarse. Coincide con la encuesta (26 respuestas "Otro" en Q9 sobre recap o resumen de IA, casi siempre con salvedades).

> Evidencia: "marca como decisión cosas que eran solo ideas. Alguien dice 'podríamos pasar el release al 20' y en el resumen aparece 'se decidió pasar el release al 20'." (Paula Benítez). "El recap resume todo al mismo nivel. Dos páginas. No distingues qué se decidió de qué se comentó." (Javier Molina). "como la votación fue en el tablero, el resumen decía algo como 'se discutieron prioridades'." (Valeria Castro)

## Converger es lo más débil: se vota a mano, se traba, decide el líder y el desacuerdo aparece después

**Recurrencia:** en 6 de 10 la priorización se trabó y la cerró el líder por falta de tiempo (Tomás, Andrés, Lucía, Javier, Martina, Sofía), con trabas de 10 a 20 min. 4 votan contando manos o reacciones de Teams (Andrés, Lucía, Ricardo) o con un tablero que no limita votos (Valeria: dos personas votaron dos veces y se discutió 10 min si valía). 8 de 10 nombran personas que casi no intervinieron: nuevos, juniors, gente de otro país u horario, gente sin acceso.

El costo aparece después: Gloria (soporte) planteó una semana más tarde, en un café, la objeción que no dijo en la reunión, justo sobre lo que se descartó (Valeria); un dev escribió por privado que no estaba de acuerdo (Martina); un tech lead aceptó "con cara de que no" (Sofía). Implica una forma nativa, dentro de la llamada, de que cada persona marque su prioridad o vote (con límite de votos y conteo automático), y de que el líder vea quién no opinó. Es la actividad que la encuesta ya ubicaba primera (votar o priorizar, 40%).

Matiz: Paula y Ricardo no deciden en reuniones grandes a propósito ("Con dieciséis personas no se puede decidir nada"); deciden en reuniones de 3 o 4. Para ellos la reunión grande es para informar.

> Evidencia: "no hay forma de que cada uno marque su prioridad sin que se transforme en conversación. Hablamos veinte minutos. Al final decidí yo." (Martina Rojas). "Una objeción importante, y yo ni me enteré en la reunión." (Valeria Castro). "Contar reacciones de nueve personas con la mitad sin cámara... a ver, funciona, pero no te fías del todo del número." (Lucía Fernández)

## Whiteboard se abandona sobre todo porque se pierde entre reuniones; la continuidad es lo que retiene a Miro

**Recurrencia:** 5 de 10 usaron la pizarra de Teams. 4 la abandonaron (Tomás, Javier, Sofía, Ricardo) y Lucía la sigue usando solo porque compliance le prohíbe herramientas externas. **3 de los 5 no la encontraron para la reunión siguiente** (Tomás buscó 15 min y perdió los acuerdos; Lucía buscó con el grupo esperando; Sofía pasó las notas a mano desde una captura) y Ricardo supone que "sigue en algún lado". La causa que describen es la misma: queda atada al chat de esa reunión y desaparece si la serie se recrea o se convoca otra. Paula tiene el mismo problema con las notas de la reunión al reprogramar. A eso se suman: sin votación (Tomás, Javier, Lucía), sin plantillas (Tomás, Javier), lenta con 9 a 14 personas (Tomás, Javier, Sofía, Ricardo) y agrupar lleva 10 min arrastrando notas (Lucía).

Del otro lado, Tomás y Javier explican que están en Miro por la continuidad: un tablero por trimestre, un frame por sesión, y revisar los acuerdos anteriores al arrancar. Implica que la prioridad de Whiteboard no es solo votar y plantillas, sino **anclar el tablero y las notas al equipo o la serie, no a una instancia de reunión**, con acceso directo a la sesión anterior. Para cuentas con compliance estricto (Lucía, España) lo nativo es la única opción, así que su calidad decide si la actividad se hace o no.

Aparte, hay un problema de descubrimiento en otras funciones: Valeria no sabía que existía la pizarra, Andrés no conocía las notas de reunión (y le parecieron prácticas), Ricardo no sabía que se pueden usar apps dentro de la reunión, Diego sabe que Loop existe pero nunca lo abrió.

> Evidencia: "Esa continuidad es la razón por la que estamos en Miro. Si tuviera que empezar de cero cada vez, perdería el hilo." (Tomás Aguirre). "Resulta que queda atada al chat de esa reunión, y como la segunda sesión fue una convocatoria nueva, pues ahí no aparecía." (Lucía Fernández). "lo nativo es lo único que tengo. Necesito que funcione mejor, no que me digan que hay otra cosa fuera." (Lucía Fernández)

## Sobre artefactos que ya existen, entrar no cuesta: cuesta señalar y que todo pase por una sola persona

**Recurrencia:** con herramientas con SSO (Jira, Power BI, Confluence) entrar lleva alrededor de 1 minuto (Martina, Diego, Sofía). Los 5 a 10 minutos de acceso aparecen solo con pizarras con licencias o cuentas separadas (Tomás 5 a 7 min, Javier más de 10, Valeria 6 a 8), y su consecuencia principal no son los minutos sino la gente que queda afuera dictando por chat o mirando la pantalla de otro (Tomás, Javier, Lucía, Valeria). En cambio, 4 de 10 describen perder tiempo en señalar sobre pantalla compartida (Tomás en Jira, Andrés en Excel, Diego en Power BI, Valeria en Figma) y 5 de 10 trabajan con una sola persona que edita y el resto dicta (Andrés, Martina, Tomás, Lucía, Javier).

El error de señalar tiene costo real: Andrés cerró la fila equivocada y al cliente le llegó la notificación de cierre con el caso abierto. Diego perdió 10 a 15 min porque cada uno miraba el dashboard con un filtro distinto. Javier agrega el costo de saltar entre ventanas durante toda la reunión, no solo al inicio. Implica que, para la necesidad de "trabajar sobre lo que ya vive afuera", la palanca no es traer Jira o Power BI a Teams, sino que cualquier participante pueda **señalar sobre lo compartido** y que todos vean la misma vista. La métrica para reuniones internas es participación efectiva, no tiempo de entrada (coincide con la encuesta: 47% de reuniones internas con alguien mirando la pantalla de otro).

> Evidencia: "Ellos ven mi pantalla. No pueden marcar nada, no pueden señalar. Si pudieran apuntar con algo, me dirían 'esta' y listo." (Andrés Quintero). "la gente que no entra al tablero no es poca. En casi todas hay alguien mirando desde afuera, y esa gente no opina. Eso me preocupa más que los minutos." (Valeria Castro)

## Señales que acotan

- **Las decisiones grandes se toman en reuniones chicas** (Paula, Ricardo). Una solución pensada para decidir con 15 personas no les sirve; sí les sirve que lo decidido llegue a todos.
- **"Demasiadas reuniones" como dolor principal** (Ricardo: 27 h por semana, "la mitad de esas podrían ser un correo"; Andrés: 1,5 h que debería durar 40 min). No se exploró si aceptarían alternativas asíncronas dentro de Teams.
- **"Es disciplina, no herramienta"** (Diego; Sofía al principio, que luego cambia a "lo que nos falla es cómo se cierra la reunión"). Ambos describen fallas que una herramienta sí podría prevenir (filtro compartido, decisión oculta en hilo resuelto).
- Martina: "no veo para qué querría otra herramienta". Lo que pide es cierre con decisión y motivo en el ticket, no una pizarra nueva.

## Relación con el análisis de encuesta

Las entrevistas refuerzan los cinco insights de la encuesta del mismo día, y agregan el "por qué": el dolor de registro es de dueño y de formato (insight 1), el recap falla por no separar propuesta de decisión y no ver el artefacto (insight 2), y Whiteboard se abandona por persistencia antes que por falta de funciones (insight 4).
