---
source: secondary
method: web
date: 2026-09-15
question: Qué venden y cuánto cobran las herramientas externas de colaboración visual (Miro, Mural, FigJam y alternativas); si su uso dominante es en vivo o asíncrono; qué evidencia pública hay sobre la fricción de acceso a artefactos externos en reuniones; y cómo monetizan los rivales la colaboración en reuniones.
opportunity: colaboracion-en-vivo-fuera-de-teams
---

# Research: la colaboración en vivo de las reuniones grandes se hace fuera de Teams

Método: búsqueda web con 4 agentes en paralelo (uno por carril), consultas del 15 y 16/09/2026. Tres afirmaciones centrales se revisaron a mano contra la fuente original (Miro 2020, notas de reunión de Teams, Whiteboard con externos). Lo que no tiene fuente queda marcado `[conocimiento del modelo, verificar]`.

Nota sobre el caso: el empaquetado del overview (plan "Max", salto de USD 8) es propio del caso de clase. Lo que aquí se dice sobre los planes reales de Microsoft (Teams Premium, E5, E7, Copilot) es contexto de mercado, no una descripción del producto del caso.

**Los tres hallazgos que cambian decisiones:**

1. **El mercado no justifica devolver la restricción de "tiempo real" al patrocinador, pero la matiza.** El uso de pizarras es mixto con peso real del uso en vivo: el único dato de uso publicado muestra dos tercios de los tableros de Miro con colaboración simultánea (2020), y Gartner (2025) todavía trata la reunión en vivo como el caso base. A la vez, la investigación sobre reuniones muestra un ciclo antes (asíncrono), durante (en vivo), después (asíncrono). Una solución solo en tiempo real cubre el tramo de la reunión y deja afuera la continuidad del artefacto, que es justo lo que decide la creencia [value] de la oportunidad (¿el artefacto se crea para la reunión o preexiste?).
2. **"Salir de Teams" no es falta de integración técnica, y la brecha documentada de Teams está en los externos.** Miro, Mural, FigJam y Lucidspark ya tienen app oficial con "share to stage" dentro de reuniones de Teams, y los tres líderes dejan editar gratis a personas externas. Microsoft, en cambio, excluye a los externos de las notas Loop y de Facilitator, y solo les deja usar Whiteboard durante la reunión y si el administrador lo habilita. La fricción de acceso aparece sobre todo con invitados, tableros privados y apps no aprobadas por IT; con miembros internos y SSO parece marginal. Dos consecuencias: (a) la explicación "externos" empuja hacia Bruno, la persona negativa, y hay que tratarla como señal de alarma; (b) la telemetría del 29% solo ve enlaces pegados en el chat, no las apps compartidas al stage, así que el análisis de datos propios de la agenda tiene un punto ciego.
3. **En el mercado, la cocreación en reuniones no es una palanca de upgrade: se regala.** Microsoft incluye Whiteboard y Loop en la base; Webex da pizarras gratis; Mural incluye su IA sin costo. Lo que sí se cobra en planes superiores es IA (Copilot, E7, AI Companion personalizado), seguridad (Teams Premium) y escala (participantes, pizarras ilimitadas). Los compradores ya tienen 36% de licencias SaaS sin uso y les cuesta demostrar el ROI de Copilot. Además, desde 09/2025 la Comisión Europea obliga a Microsoft a ofrecer suites sin Teams con diferencia de precio mayor, lo que agrega riesgo a atar una función de colaboración al plan más alto en cuentas con operación en el EEE. Esto debilita, sin tumbarla, la creencia [viability] de la oportunidad.

## Carril 1: competidores directos y oferta

| Proveedor | Planes y precio (USD/usuario/mes, anual) | Personas externas | Integración con Teams | IA | Posicionamiento |
|---|---|---|---|---|---|
| Miro | Free (3 tableros editables) / Starter 8 / Business 20 / Enterprise a medida desde 30 miembros | Guests gratis e ilimitados (editan desde Business); Visitors por enlace sin cuenta | Share to stage, abrir tablero en la reunión, votación y temporizador, calendario, pestañas; requiere aprobación del admin | Créditos por plan, extras pagos | "AI Innovation Workspace" |
| Mural | Free (3 murales) / Team+ 9 (12,99 mensual) / Business 17,99 / Enterprise a consultar | Visitors en todos los planes; Guests desde Business | App para reuniones y pestañas; detalle del stage desconocido | Incluida sin costo desde Team+ (fair use) | "Visual AI platform" |
| FigJam | Asiento Collab 3 (Professional) / 5 (Organization y Enterprise); Starter con 3 archivos | "Open sessions" de 24 h sin cuenta (planes pagos) | Share to stage con edición completa, pestañas | Ordenar y resumir stickies (pago), créditos por asiento | "Online whiteboard… ideate and brainstorm" |
| Lucidspark | desconocido | Deben iniciar sesión en el stage | Panel lateral y share to stage en todos los planes | Agrupar temas y resumir | "Where ideas ignite" |
| Zoom Whiteboard | Basic gratis (3 pizarras) / Plus desde 2,07 | desconocido | desconocido | AI Companion sin costo en planes pagos | "Keeps ideas, people, and work connected" |
| Google | Jamboard cerrado (31/12/2024); delega en FigJam, Miro y Lucidspark | n/a | n/a | n/a | n/a |
| Microsoft (referencia) | Whiteboard y Loop incluidos en M365; la IA requiere Copilot | Whiteboard con externos solo durante la reunión y si el admin lo habilita; notas Loop y Facilitator sin externos | Nativo | Copilot en Whiteboard (Suggest, Categorize, Summarize) y Facilitator, con licencia | "The visual collaboration canvas in Microsoft 365" |

Fuentes:
- Miro: precios, guests, IA [verificado: https://miro.com/pricing/, 2026-09-16]; guests gratis [verificado: https://help.miro.com/hc/en-us/articles/360021415119-Collaboration-with-Guests, 2026-09-16]; app de Teams [verificado: https://miro.com/marketplace/microsoft-teams/, 2026-09-16]; aprobación del admin [verificado: https://help.miro.com/hc/en-us/articles/4406387211538-Microsoft-Teams-Meetings-integration-User-guide-, 2026-09-16]; posicionamiento [verificado: https://miro.com/, 2026-09-16]. Precio con pago mensual (10 y 24) [conocimiento del modelo, verificar].
- Mural: planes, externos [verificado: https://www.mural.co/pricing, 2026-09-16]; Teams [verificado: https://www.mural.co/partners/microsoft/teams, 2026-09-16]; IA [verificado: https://www.mural.co/mural-ai, 2026-09-16]; posicionamiento [verificado: https://www.mural.co/, 2026-09-16].
- FigJam: tipos de asiento [verificado: https://www.figma.com/pricing-faq/, 2026-09-16]; precios por asiento, tomados de un agregador de terceros porque la página oficial no mostró cifras [verificado: https://www.stackscored.com/pricing/graphic-design/figma/, 2026-09-16]; open sessions [verificado: https://help.figma.com/hc/en-us/articles/8538436879767-Run-meetings-in-FigJam, 2026-09-16]; Teams [verificado: https://help.figma.com/hc/en-us/articles/7405452518423-Figma-and-Microsoft-Teams, 2026-09-16]; IA [verificado: https://help.figma.com/hc/en-us/articles/18711926790423-Sort-and-summarize-stickies-with-FigJam-AI, 2026-09-16].
- Lucidspark: IA y posicionamiento [verificado: https://lucid.co/lucidspark, 2026-09-16]; Teams [verificado: https://help.lucid.co/hc/en-us/articles/15997078015124-Integrate-Lucid-with-Microsoft-Teams, 2026-09-16]. Precios: la página no cargó.
- Zoom Whiteboard [verificado: https://www.zoom.com/en/products/online-whiteboard/, 2026-09-16].
- Google Jamboard [verificado: https://workspaceupdates.googleblog.com/2023/09/the-next-phase-of-digital-whiteboarding-for-google-workspace.html, 2026-09-16].
- Microsoft: Whiteboard con externos [verificado: https://support.microsoft.com/en-us/whiteboard/collaborate-with-external-participants-in-a-teams-meeting, 2026-09-16]; notas de reunión, "External attendees won't be able to access or edit meeting notes" [verificado: https://support.microsoft.com/en-us/teams/meetings/take-meeting-notes-in-microsoft-teams, 2026-09-16]; Facilitator [verificado: https://support.microsoft.com/en-us/teams/copilot/facilitator-in-microsoft-teams-meetings, 2026-09-16]; Copilot en Whiteboard [verificado: https://support.microsoft.com/en-us/whiteboard/welcome-to-copilot-in-whiteboard, 2026-09-16].

**Qué prueba su existencia:** hay un mercado pago y maduro de colaboración visual en vivo, con planes de empresa que venden SSO, SCIM y residencia de datos; colaborar con externos es un requisito central de la categoría; la IA de agrupar y resumir ya es estándar. Google eligió delegar en vez de competir, señal de que la categoría es difícil de ganar para una plataforma de comunicaciones.

**Qué no prueba:** que los Team Leads del segmento salgan por falta de funciones y no por hábito, por artefactos previos o por pedido de externos; que las apps dentro de Teams se usen o funcionen bien con más de 5 personas (no hay datos de adopción); que un Whiteboard mejorado los haga dejar Miro, Mural o FigJam.

## Carril 2: ¿uso en vivo o asíncrono?

Veredicto: **mixto, con peso relevante del uso en vivo**. Confianza media-baja: no hay datos independientes y lo cuantitativo es de fabricantes o antiguo.

- Miro: "Since March, between 64% and 67% of Miro boards have been used by teams to work together at the same time", contra alrededor de 50% antes de la pandemia; las sesiones de 10 a 19 usuarios simultáneos crecieron 943% entre marzo y junio de 2020 [verificado: https://miro.com/blog/collaboration-trends/, 2026-09-16]. Dato del fabricante, del pico de pandemia, y que un tablero se use "a la vez" alguna vez no dice qué parte del uso es en vivo.
- Miro, lanzamiento de Talktrack (09/2023): "our users were using it async as much as sync, and the trend was on the rise", sin cifras. Es mensaje de marketing de un producto asíncrono [verificado: https://miro.com/blog/official-launch-miro-talktrack/, 2026-09-16].
- Encuesta de Miro sobre preferencias (sin n declarado, 02/2024): se prefieren asíncronas el feedback individual (60%) y las retrospectivas (55%); síncronos el arranque de proyectos (65%) y la resolución de problemas técnicos (60%). Mide preferencia, no uso [verificado: https://miro.com/blog/asynchronous-work-tasks/, 2026-09-16]. Dato relevante para Carolina, cuya retro es en vivo.
- Gartner, Market Guide for Visual Collaboration Applications (27/10/2025), citado por Lucid: recomienda usar estas herramientas "beyond live meetings". Supone que la reunión en vivo es el uso base [verificado: https://lucid.co/blog/takeaways-gartner-market-guide-for-visual-collaboration, 2026-09-16]. Cita elegida por un fabricante.
- Microsoft Research, "Meeting Bridges" (2024; 13 entrevistas, encuesta a 198 trabajadores, codiseño con 16): la información de las reuniones se reutiliza de forma asíncrona para archivo, tareas, inclusión de ausentes y colaboración posterior; notas y grabaciones cumplen mal ese papel [verificado: https://arxiv.org/abs/2402.03259, 2026-09-16].
- Microsoft Work Trend Index 2025 (31.000 personas, 31 países, más telemetría de M365): 60% de las reuniones son improvisadas; 30% cruzan varias zonas horarias, 8 puntos más que en 2021 [verificado: https://www.microsoft.com/en-us/worklab/work-trend-index/2025-the-year-the-frontier-firm-is-born, 2026-09-16].
- Shopify eliminó en 2023 las reuniones recurrentes de más de 2 personas y calcula 320.000 horas recortadas; una sola empresa, cifra propia [verificado: https://www.bloomberg.com/news/newsletters/2023-02-14/how-shopify-cut-320-000-hours-of-unnecessary-meetings, 2026-09-16].
- FigJam: no hay cifra pública que separe FigJam ni que distinga uso en vivo y asíncrono. Desconocido.
- ¿El artefacto se crea para la reunión o preexiste? Sin dato cuantitativo. Desconocido. Es plausible que Jira y Docs sean sobre todo preexistentes y las pizarras más de sesión [conocimiento del modelo, verificar].

## Carril 3: alternativas, no consumo y fricción de acceso

**Minutos perdidos por accesos:** ninguna fuente pública los mide. Desconocido.

Contexto:
- 37% de las reuniones empieza tarde (Rogelberg y colaboradores; 195 empleados sobre más de 300 reuniones, y un segundo estudio con 665), sin minutos promedio [verificado: https://www.bps.org.uk/research-digest/scourge-meeting-late-comers, 2026-09-16].
- Más del 71% de los líderes de TI reporta problemas técnicos en reuniones (Logitech 2026, sin n, dato de proveedor) [verificado: https://www.itpro.com/software/business-apps/clunky-workplace-tech-is-ruining-meetings-and-impacting-productivity, 2026-09-16].

**Dónde la fricción parece significativa:**
- Apps de terceros en Teams: no bloqueadas por defecto (salvo entornos de gobierno), pero el admin puede bloquearlas y el usuario debe pedir habilitación [verificado: https://learn.microsoft.com/en-us/microsoftteams/manage-apps, 2026-09-16].
- Tableros privados de Miro: "No access to board. Ask the board owner to grant you permission"; la red corporativa también puede bloquear [verificado: https://help.miro.com/hc/en-us/articles/5225385943954-I-can-t-access-or-edit-a-Miro-board, 2026-09-16].
- Invitados en Whiteboard y Loop: en Microsoft Q&A, "guests… cannot access or edit whiteboards, even if they are part of the team", y la respuesta sugiere exportar a PNG o usar Miro [verificado: https://learn.microsoft.com/en-us/answers/questions/1803142/using-whiteboard-while-working-with-guests-in-a-te, 2026-09-16]. Loop con externos requiere enlaces para personas específicas y uso compartido externo habilitado [verificado: https://learn.microsoft.com/en-us/microsoft-365/loop/loop-permission?view=o365-worldwide, 2026-09-16].
- Anécdota de facilitador en la comunidad de Miro: 80% entró al tablero y el resto quedó atascado en avisos de registro (n=1, señal) [verificado: https://community.miro.com/ask-the-community-45/guests-can-t-access-public-board-with-the-link-i-send-them-4375, 2026-09-16].

**Dónde parece marginal:**
- Whiteboard compartido en una reunión de Teams no crea enlace ni pide permisos; los externos colaboran de forma temporal, "similar to PowerPoint Live" [verificado: https://learn.microsoft.com/en-us/microsoft-365/whiteboard/manage-sharing-organizations?view=o365-worldwide, 2026-09-16].
- Miembros internos con SSO y enlaces "cualquiera de la organización": probablemente segundos [conocimiento del modelo, verificar]. Coincide con lo que se le atribuyó a Joaquín (sintético).

**Quejas sobre la opción nativa (señal, no hecho):**
- Capterra, Microsoft Whiteboard (4,4/5, 158 reseñas): "Tends to crash when other software applications are open… lagging when video camera was used"; "Templates… are not a very good quality"; dibujar sirve de verdad solo con tableta [verificado: https://www.capterra.com/p/203470/Microsoft-Whiteboard/reviews/, 2026-09-16].
- La guía oficial de talleres de Whiteboard menciona plantillas, reacciones, Follow y Raise Hand, pero no temporizador ni votación [verificado: https://support.microsoft.com/en-us/whiteboard/running-workshops-with-microsoft-whiteboard, 2026-09-16]. Si Whiteboard tiene votación hoy: desconocido.

**Qué se hace en lugar de eso:**
- Compartir pantalla es la salida que recomienda la propia comunidad de Miro ante usuarios nuevos [verificado: https://community.miro.com/ask-the-community-45/new-to-miro-and-first-team-meeting-via-zoom-on-a-miro-board-help-14125, 2026-09-16].
- Encuestas dentro de la reunión: Slido ("no need to install anything") y Mentimeter tienen app para Teams [verificado: https://www.slido.com/microsoft-teams-polling, 2026-09-16] [verificado: https://www.mentimeter.com/integrations/microsoft-teams, 2026-09-16]. Forms y PowerPoint Live nativos [conocimiento del modelo, verificar].
- No consumo (solo conversar, el facilitador maneja el tablero): sin datos. Desconocido.

**Alfabetización digital y accesibilidad:**
- En EE. UU., 13% de los trabajadores no tiene habilidades digitales y 18% muy limitadas (PIAAC 2012-14, publicado 2020; datos antiguos, no de usuarios de Teams) [verificado: https://nationalskillscoalition.org/blog/news/nearly-1-in-3-workers-lack-foundational-digital-skills-new-report-finds/, 2026-09-16].
- Miro declara auditorías WCAG 2.2 AA y admite que "a lot depends on the board creator or meeting facilitator" [verificado: https://help.miro.com/hc/en-us/articles/19506114302354-Overview-of-Miro-Accessibility, 2026-09-16].
- Relación entre baja alfabetización digital y no abrir enlaces externos en reuniones (el caso de Rosa Elena): sin evidencia. Desconocido.

**Costo de cambiar de app (indirecto, no mide salir de la reunión):**
- HBR 2022: unas 1.200 alternancias diarias entre apps y casi 4 h semanales de reorientación (137 usuarios, 3 empresas Fortune 500) [verificado: https://hbr.org/2022/08/how-much-time-and-energy-do-we-waste-toggling-between-applications, 2026-09-16].
- Atlassian State of Teams 2025 (12.000 trabajadores): 25% del tiempo buscando información [verificado: https://www.atlassian.com/blog/state-of-teams-2025, 2026-09-16].

## Carril 4: precios, modelos de negocio y tendencias

**Microsoft (contexto real, no el empaquetado del caso):**
- Teams separado de las suites en el mundo desde 01/04/2024; los clientes existentes pueden seguir renovando suites con Teams [verificado: https://www.microsoft.com/en-us/licensing/news/microsoft365-teams-ww, 2026-09-16].
- Subida de precios el 01/07/2026 para clientes nuevos y renovaciones (E3, E5, Business Basic y Standard, F1 y F3, entre otros), justificada con Copilot Chat, Defender e Intune [verificado: https://www.microsoft.com/en-us/licensing/news/2026-m365-packaging-pricing-updates-faq, 2026-09-16] [verificado: https://www.microsoft.com/en-us/microsoft-365/blog/2025/12/04/advancing-microsoft-365-new-capabilities-and-pricing-update/, 2026-09-16]. Cifras por SKU según terceros: M365 E3 de 36 a 39, E5 de 57 a 60, Business Basic de 6 a 7 [verificado: https://samexpert.com/microsoft-365-july-2026-price-increase/, 2026-09-16].
- Business Premium con Copilot: 32 con Teams, 28,80 sin Teams [verificado: https://www.microsoft.com/en-us/microsoft-365/business/with-copilot-plans-and-pricing, 2026-09-16].
- Teams Premium, complemento de 10: resumen inteligente, traducción en vivo, notas con IA, cifrado de extremo a extremo, marca de agua, marca corporativa. Ninguna función de cocreación en vivo [verificado: https://www.microsoft.com/en-us/microsoft-teams/premium, 2026-09-16].
- M365 E7 "Frontier Suite", 99, disponible desde 01/05/2026: E5 más Copilot, Agent 365 y seguridad avanzada [verificado: https://blogs.microsoft.com/blog/2026/03/09/introducing-the-first-frontier-suite-built-on-intelligence-trust/, 2026-09-16].
- Resultados del 4.º trimestre del año fiscal 2026: "Premium offerings, including Copilot, E5, and early traction in E7, drove ARPU growth"; Teams no aparece como motor [verificado: https://www.microsoft.com/en-us/investor/events/fy-2026/earnings-fy-2026-q4, 2026-09-16].

**Qué gatean los rivales:**

| Proveedor | Incluido en la base | Plan superior o complemento |
|---|---|---|
| Microsoft | Whiteboard, componentes y espacios de Loop | Copilot en reuniones (Copilot o E7); recap, traducción y seguridad (Teams Premium, 10) |
| Zoom | Pizarra limitada; AI Companion en planes pagos | Pizarras ilimitadas (Business y superiores); Whiteboard Plus (complemento); Custom AI Companion (12) |
| Google | Salas, encuestas, preguntas; Gemini desde Standard | Grabación (Standard+); 500 a 1.000 participantes; transmisión en vivo (Enterprise) |
| Slack | Huddle 1:1 | Huddles grupales con canvas y notas IA (Pro+); IA agéntica (Business+) |
| Webex | Pizarras, incluso en el plan gratuito | 1.000 asistentes y AI Assistant (Enterprise) |

Fuentes: Zoom Whiteboard por plan [verificado: https://library.zoom.com/zoom-workplace/zoom-whiteboard/zoom-whiteboard-explainer, 2026-09-16]; Custom AI Companion, fuente de terceros [verificado: https://businessmodelanalyst.com/zoom-free-ai-retention-price/, 2026-09-16]; Google [verificado: https://workspace.google.com/pricing, 2026-09-16] [verificado: https://workspace.google.com/blog/product-announcements/empowering-businesses-with-AI, 2026-09-16]; Slack [verificado: https://slack.com/pricing, 2026-09-16] [verificado: https://slack.com/help/articles/4402059015315-Use-huddles-in-Slack, 2026-09-16]; Webex [verificado: https://pricing.webex.com/us/en/, 2026-09-16].

**Qué mueve los upgrades en empresas:**
- Zylo SaaS Management Index 2026: 36% de las licencias SaaS sin uso; las unidades de negocio controlan el 81% del gasto y TI el 15% [verificado: https://zylo.com/news/2026-saas-management-index, 2026-09-16].
- Gartner 2025 (187 líderes de TI): solo el 5% de quienes terminaron un piloto de Copilot pasaba a despliegue amplio; el ROI es "quite challenging" de demostrar [verificado: https://www.techpartner.news/news/gartner-microsoft-copilot-hype-offset-by-roi-and-readiness-realities-618118, 2026-09-16].
- Zoom: el segmento Enterprise crece 7,8% con expansión neta de 99% (2.º trimestre del año fiscal 2027) [verificado: https://www.globenewswire.com/news-release/2026/08/25/3350878/0/en/zoom-communications-reports-financial-results-for-the-second-quarter-of-fiscal-year-2027.html, 2026-09-16]. Un analista externo atribuye la recuperación a empezar a cobrar la IA por niveles; es interpretación, no causa probada [verificado: https://businessmodelanalyst.com/zoom-free-ai-retention-price/, 2026-09-16].

**Tendencias:**
- Consolidación: las plataformas de reunión suman pizarras, documentos y agentes (Zoom Workplace, canvas en huddles de Slack, Whiteboard en Teams). A la inversa, Miro se reposiciona como espacio de IA (Flows, Sidekicks, MCP; 10/2025) [verificado: https://miro.com/newsroom/miro-puts-ai-where-teams-work/, 2026-09-16].
- Antimonopolio en la UE: el 12/09/2025 la Comisión aceptó compromisos de Microsoft por 7 años (10 para interoperabilidad): suites sin Teams a precio "appreciably lower", con la diferencia de precio un 50% mayor, e interoperabilidad y portabilidad para competidores [verificado: https://ec.europa.eu/commission/presscorner/api/files/document/print/en/ip_25_2048/IP_25_2048_EN.pdf, 2026-09-16]. Aplica al EEE; el segmento opera en 3+ países y puede incluir España (el caso sintético de Joaquín tiene equipo en Madrid). Implicación a confirmar con legal.

## Impacto en creencias

Primero las que la agenda de la oportunidad pedía resolver con este research.

| Creencia (de overview.md) | Veredicto | Evidencia |
|---|---|---|
| **2.** [opportunity] [value] La mayoría de los enlaces externos del segmento apuntan a un artefacto creado para esa reunión, y se pierden 5+ minutos por reunión en accesos | no dice nada | No hay dato público de minutos perdidos ni de artefactos creados vs. preexistentes. Sí acota dónde se esperaría la fricción: significativa con invitados, tableros privados y apps no aprobadas; marginal con miembros internos y SSO [verificado: Microsoft Learn, ayuda de Miro, 2026-09-16]. El ciclo de vida de los artefactos es mixto [verificado: arxiv 2402.03259, 2026-09-16]. |
| Fila de agenda: "si el mercado muestra uso mayormente asíncrono, la restricción de tiempo real vuelve al patrocinador" | no se activa | Uso mixto con peso relevante en vivo: Miro 64-67% de tableros con colaboración simultánea (2020) [verificado: miro.com/blog/collaboration-trends, 2026-09-16]; Gartner 2025 trata la reunión en vivo como caso base [verificado: lucid.co, 2026-09-16]. No hay evidencia de uso mayormente asíncrono; tampoco confirma que el tiempo real alcance, porque el artefacto vive antes y después. |
| **5.** [opportunity] [viability] Resolver el problema mueve el upgrade a Max del segmento por encima de 3,1% | contradice (débil) | En el mercado la cocreación en reuniones va en la base o gratis (Whiteboard y Loop incluidos; Webex gratis; IA de Mural sin costo); lo que se cobra arriba es IA, seguridad y escala [verificado: páginas de precios de Microsoft, Zoom, Google, Slack, Webex, 2026-09-16]. Microsoft atribuye su ARPU a Copilot, E5 y E7, no a Teams [verificado: resultados FY26 Q4, 2026-09-16]. Riesgo regulatorio en el EEE al atar funciones de Teams a planes [verificado: Comisión Europea IP/25/2048, 2026-09-16]. No descarta que funcione en *este* segmento: son otros productos y otros compradores. |
| **1.** [product] [value] Los Team Leads comparten enlaces externos porque la colaboración nativa no cubre lo que necesitan en vivo, no por hábito ni porque los artefactos ya vivan afuera | apoya (débil) | Brechas documentadas en lo nativo: externos excluidos de notas Loop y Facilitator, Whiteboard con externos solo durante la reunión [verificado: support.microsoft.com, 2026-09-16]; guía de talleres sin votación ni temporizador [verificado: support.microsoft.com, 2026-09-16]; quejas de rendimiento y plantillas [verificado: Capterra, 2026-09-16]. Pero existen apps de Miro, Mural, FigJam y Lucid dentro de Teams, así que no descarta hábito ni artefactos que ya viven afuera. Si la brecha principal son los externos, el hallazgo se apoya en el perfil de Bruno (persona negativa). |
| **3.** [product] [value] El bajo uso de Whiteboard y notas se debe a que no se consideran adecuadas, no a desconocimiento | apoya (débil) | Reseñas con quejas de calidad de plantillas, rendimiento y dibujo [verificado: Capterra, 2026-09-16]; un moderador de Microsoft Q&A recomienda usar Miro para trabajar con invitados [verificado: learn.microsoft.com/answers, 2026-09-16]. Nada separa "inadecuado" de "desconocido" en el uso real. |
| **4.** [product] [viability] IT no sube a Max porque no ve el valor concreto que sacan sus Team Leads | apoya (débil) | 36% de licencias SaaS sin uso [verificado: Zylo 2026, 2026-09-16]; ROI de Copilot difícil de demostrar y solo 5% de pilotos pasa a despliegue amplio [verificado: Gartner vía techpartner.news, 2026-09-16]. Es evidencia sobre IA y SaaS en general, no sobre reuniones ni sobre el segmento. |
| **6.** [product] [value] Los mandos medios aceptarían reemplazar reuniones por alternativas asíncronas dentro de Teams | no dice nada | Hay tendencia de oferta asíncrona (Talktrack de Miro, notas IA en huddles de Slack, Facilitator) y más reuniones fragmentadas por zonas horarias [verificado: WTI 2025, 2026-09-16], pero nada sobre la aceptación de los mandos medios. |
| **7.** [product] [viability] La baja por "funciones que no usamos" se concentra en cuentas de menos de 100 licencias | no dice nada | Solo contexto general de licencias sin uso [verificado: Zylo 2026, 2026-09-16]; nada por tamaño de cuenta. |

## Qué sigue necesitando research primario

**Datos propios (ajuste al análisis del 30/09 ya previsto en la agenda):**
- La telemetría del 29% solo ve enlaces pegados en el chat. Sumar el uso de apps de terceros compartidas al stage (Miro, Mural, FigJam, Lucid) para no subestimar la salida.
- Cruzar esas reuniones con la proporción de participantes externos o invitados y con si el tenant tiene la app de terceros aprobada. Si la salida se concentra en reuniones con externos, es señal Bruno.

**Encuesta (`/design-survey`, cuántos, cada cuánto, cuánto):**
- Frecuencia de salida a herramientas externas en reuniones de más de 5 personas y qué herramienta.
- Si el artefacto se creó para esa reunión o ya existía, y si sigue en uso después.
- Minutos hasta que todos entran y cuántas personas no llegan a entrar.
- Proporción de externos o invitados en esas reuniones.
- Si probaron Whiteboard o una app de terceros dentro de Teams, y si saben que existen (separa creencia 3 de desconocimiento).

**Entrevistas con Team Leads (`/design-interview`, por qué y qué hacen hoy):**
- Qué actividad concreta hacen afuera (votar, agrupar, dibujar, editar un doc) y por qué no la hacen en Teams: función faltante, externos, hábito, o el artefacto ya vive ahí.
- Qué pasa con el artefacto antes y después de la reunión (la bisagra entre tiempo real y continuidad).
- Priorizar a quienes contradicen la creencia: los que no salen, y los que salen y dicen que no les cuesta.

**Entrevistas con IT (perfil Damián):**
- Si el freno al upgrade es precio o valor visible, y si una función de colaboración en reuniones sería defendible como motivo de upgrade frente a IA y seguridad.
- Política sobre apps de terceros en Teams y sobre acceso de externos.
- En cuentas con operación en el EEE, cómo pesan las suites sin Teams en la decisión.
