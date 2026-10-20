---
feature: recap-de-decisiones
spec: product/specs/2026-10-13-1945-recap-de-decisiones.md
mechanism: incremental
created: 2026-10-13
---

# Plan de exposición: Recap de IA centrado en decisiones

**Spec:** `product/specs/2026-10-13-1945-recap-de-decisiones.md` (approved)
**Mecanismo:** desarrollo incremental (elegido por el equipo)

## Hipótesis

Tomada tal cual de la spec:

> Creemos que los líderes del segmento que conducen reuniones de más de 5 con decisiones van a publicar la lista de decisiones de la IA, revisada en 5 minutos o menos, en lugar de armar su propia acta, correo o carga en Jira, porque el recap actual les genera trabajo (reescribirlo o corregirlo, 10 a 60 minutos) y una lista con responsable y fecha que pueden verificar contra la transcripción se los ahorra.
> Nos equivocamos si, mostrada la lista de su propia reunión, menos de la mitad de los líderes la publica en lugar de su registro habitual, o si la mediana de revisión supera los 5 minutos.

## Secuencia de creencias

1. **Los líderes reconocen la lista como lo que se decidió** en su reunión. Si no la ven así, revisarla no tiene sentido.
2. **Los líderes la corrigen en 5 minutos o menos y detectan las propuestas marcadas como decisión** (creencia 16 más la parte de tiempo de la hipótesis). Si no, publicar es riesgoso o no ahorra nada.
3. **Los líderes publican la lista en lugar de su propio registro** (creencia 15, el centro de la hipótesis).
4. **Los responsables usan la lista publicada para saber qué les toca.** Esto va más allá de la hipótesis: es el lado de quien recibe, que todavía no tiene evidencia real.

## Niveles

### Nivel 1: Lista privada de decisiones, solo lectura
- **Qué se revela:** después de la reunión, el organizador ve, en el mismo lugar que el recap, la lista de decisiones con decisión, responsable, fecha y motivo. Incluye:
  - propuestas y temas abiertos en una sección aparte;
  - "sin responsable" y "sin fecha" cuando no se dijeron;
  - "No se detectaron decisiones" cuando no hubo ninguna;
  - códigos de ticket como enlace o texto destacado;
  - la marca "falta contexto de pantalla";
  - la frase y el minuto de origen, con enlace a la grabación.

  **Queda oculto:** editar, publicar, copiar y notificar.
- **Creencia:** los líderes ven en la lista lo que se decidió en su reunión, y les parece que corregirla da menos trabajo que escribir su propia acta.
- **Audiencia:** todos los organizadores de reuniones grabadas o transcritas de más de 5 participantes en cuentas del plan superior.
- **Duración:** 2 semanas.
- **Validación:**
  - **Avanzar si:** al menos el 60% de los organizadores con 2 o más reuniones abre la lista en 2 reuniones o más, y al menos la mitad responde en el producto que "le falta poco o nada para usarla como registro".
  - **Detener si:** menos del 40% vuelve a abrirla, o la mayoría responde que "tendría que rehacerla".

### Nivel 2: Revisión y corrección
- **Qué se revela:** todo lo del nivel 1, más:
  - editar cada campo;
  - borrar y agregar ítems;
  - mover ítems entre decisiones y propuestas;
  - completar el contexto de pantalla;
  - "sin responsable" marcado a la vista hasta que se resuelva.

  La lista sigue siendo visible solo para el organizador. **Queda oculto:** publicar, copiar y notificar.
- **Creencia:** los líderes terminan la revisión en 5 minutos o menos y corrigen las propuestas que la IA marcó como decisión antes de dar la lista por buena.
- **Audiencia:** la misma del nivel 1.
- **Duración:** 2 semanas.
- **Validación:**
  - **Avanzar si:** la mediana de revisión es de 5 minutos o menos, y en una auditoría de una muestra de listas revisadas contra su transcripción (con consentimiento) quedan sin corregir 1 de cada 4 propuestas marcadas como decisión, o menos.
  - **Detener si:** la mediana supera los 5 minutos, o quedan sin corregir más de 1 de cada 4.

### Nivel 3: Publicar en el chat y copiar en un paso
- **Qué se revela:** todo lo anterior, más:
  - publicar en el chat de la reunión para todos los invitados internos;
  - elegir si los externos ven la lista (por defecto no);
  - aviso de quién revisó y cuándo;
  - versión nueva marcada cuando se edita después de publicar;
  - copiar en un paso con formato y enlace a la reunión.

  **Queda oculto:** el destacado para el responsable y las notificaciones.
- **Creencia:** los líderes publican la lista revisada en lugar de armar su propia acta, correo o carga en Jira.
- **Audiencia:** la misma de los niveles anteriores. Todos los invitados internos ven las listas que se publiquen.
- **Duración:** 3 semanas.
- **Validación:**
  - **Avanzar si:** al menos la mitad de los líderes del segmento publica la lista en la mitad o más de sus reuniones con decisiones, y en un seguimiento declara que no armó un registro aparte (o que solo pegó la lista copiada).
  - **Detener si:** menos de la mitad publica, o publican pero siguen escribiendo su acta o reescribiendo la lista en Confluence o Jira.

### Nivel 4: Lo que me toca
- **Qué se revela:** todo lo anterior, más:
  - las decisiones del responsable que mira la lista aparecen destacadas o primero;
  - notificación de Teams al responsable cuando se publica una decisión a su nombre;
  - las decisiones "sin responsable" no generan notificación.
- **Creencia:** los responsables que no conducen la reunión usan la lista publicada para saber qué les toca y para cuándo, sin pedir ni mandar una confirmación aparte.
- **Audiencia:** los responsables nombrados en listas publicadas, dentro de la misma población.
- **Duración:** 2 semanas.
- **Validación:**
  - **Avanzar si:** al menos el 60% de los responsables notificados abre la lista dentro del primer día hábil, y los líderes informan menos mensajes de "¿qué me toca?" o menos correos de constancia.
  - **Detener si:** menos del 30% la abre, o los líderes siguen mandando recordatorios igual que antes.

## Mecanismo de revelado

Se usa incremental, como pidió el equipo. Esto es lo que implica:
- Cada nivel llega a toda la población desplegada. No se puede limitar al segmento en foco, así que el segmento se mide filtrando el análisis, no la exposición.
- Tampoco se pueden excluir cuentas con operación en el Espacio Económico Europeo mientras legal no confirme. Esa exclusión tiene que resolverse en el despliegue, o bloquea el nivel 1.
- La auditoría del nivel 2 depende de conseguir consentimiento en una muestra, no de una cohorte aparte.

## Validaciones en paralelo

- **T2, precisión de la extracción (creencia 14).** Es condición previa al nivel 1. Con incremental, una lista que falla en más de 1 de cada 5 decisiones llega a todos a la vez. Hay que correr T2 con el prompt y la hoja de comparación actualizados (código de ticket y marca "falta contexto de pantalla") antes de desplegar.
- **Espacio Económico Europeo.** Legal tiene que confirmar si se puede atar la función al plan superior en cuentas con operación en esa zona.
- **Restricción de "tiempo real".** El patrocinador tiene que confirmar que acepta una solución posterior a la reunión. Si no, la spec queda fuera de alcance.
- **Tasa de upgrade a Max (creencia 9) y escala del trabajo posterior (creencia 8).** No las prueba este plan. Hay que seguir el upgrade del segmento por encima del 3,1% durante y después del nivel 3.
- **Costo de extracción por reunión.** Al exponer a toda la población desde el nivel 1, hay que estimar el costo antes de desplegar.

## Preguntas abiertas para el equipo de producto

- ¿Podemos conseguir consentimiento para auditar transcripciones en el nivel 2? ¿Con cuántas cuentas?
- ¿Qué canal usamos para la pregunta en el producto del nivel 1 y el seguimiento del nivel 3?
- ¿Cuántas cuentas tienen configurada la dirección de su Jira? Eso decide cuántos tickets salen como enlace.
- ¿El nivel 4 espera a las entrevistas a quienes ejecutan sin conducir (11/11/2026)?
- ¿El agente de código mantiene el contexto entre iteraciones? Incremental depende de eso.
- ¿Hay datos de uso del recap actual que sirvan como línea base para la apertura y el tiempo de revisión?
