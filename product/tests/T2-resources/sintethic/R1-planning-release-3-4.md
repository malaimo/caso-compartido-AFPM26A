---
reunion: R1
titulo: Planning del release 3.4
fecha: 2026-10-01
duracion: 42 minutos
participantes: 7
---

# Planning del release 3.4

Transcripción automática de Teams. Participantes: Gabriela Ortiz (líder de producto, conduce), Tomás Ibarra (tech lead), Laura Méndez (desarrolladora), Hernán Silva (desarrollador), Camila Reyes (QA), Pablo Duarte (diseño), Natalia Vega (soporte).

**[00:00:12] Gabriela Ortiz:** Bueno, arrancamos, que tenemos media agenda. Hoy cerramos el alcance del 3.4. Tomás, ¿cómo venimos con la exportación a PDF?

**[00:00:31] Tomás Ibarra:** Mal. La librería que elegimos no maneja bien las tablas largas. Laura estuvo probando otra, pero no llegamos con todo para el 3.4.

**[00:00:52] Laura Méndez:** Sí, con la nueva librería las tablas salen bien, pero me falta la paginación. Calculo una semana más, como mínimo.

**[00:01:10] Gabriela Ortiz:** Entonces no la metemos en el 3.4. La exportación a PDF pasa al 3.5. ¿Alguien tiene algo en contra?

**[00:01:18] Natalia Vega:** Del lado de soporte, tengo dos clientes que la estaban esperando. Pero prefiero que salga bien.

**[00:01:26] Gabriela Ortiz:** Ok. Pasa al 3.5. Laura, ¿te encargas de avisar a soporte con el detalle de qué va a cambiar, para que Natalia le responda a esos clientes?

**[00:01:35] Laura Méndez:** Sí, se lo mando a Natalia el viernes.

**[00:01:39] Natalia Vega:** Perfecto, gracias.

**[00:02:05] Camila Reyes:** Una cosa antes de seguir. Con lo que entra en el 3.4 vamos a estar muy justos de QA. Podríamos sumar a alguien de otro equipo para la regresión.

**[00:02:20] Tomás Ibarra:** Puede ser, pero los otros equipos también están cerrando.

**[00:02:27] Gabriela Ortiz:** Anotemos que hay riesgo en QA. Sigamos con la agenda y si sobra tiempo lo vemos.

**[00:03:40] Gabriela Ortiz:** Segundo tema: la migración de la base de reportes. Hernán, ¿qué necesitas?

**[00:03:52] Hernán Silva:** Una ventana de mantenimiento de dos horas. Mi propuesta es el sábado a la mañana, que hay poco tráfico.

**[00:04:05] Tomás Ibarra:** El sábado me parece bien.

**[00:04:09] Gabriela Ortiz:** Dale, sábado entonces. Hernán, quedas a cargo de la migración.

**[00:04:14] Hernán Silva:** Listo.

**[00:05:30] Pablo Duarte:** Sobre la pantalla de filtros nueva: hice dos versiones, una con los filtros a la izquierda y otra arriba. ¿Las vemos ahora?

**[00:05:41] Gabriela Ortiz:** Muéstralas rápido.

**[00:05:44] Pablo Duarte:** *(comparte pantalla)* Esta es la de la izquierda y esta la de arriba.

**[00:06:30] Tomás Ibarra:** La de arriba es más fácil de construir, reusa el componente que ya tenemos.

**[00:06:41] Camila Reyes:** A mí me gusta más la de la izquierda, se ve todo de una vez.

**[00:06:50] Gabriela Ortiz:** Vamos con la de arriba para el 3.4, por tiempo. La de la izquierda la dejamos para pensar más adelante.

**[00:06:58] Pablo Duarte:** Ok, ajusto el diseño de la de arriba.

**[00:07:02] Gabriela Ortiz:** ¿Para cuándo lo tienes?

**[00:07:05] Pablo Duarte:** Para el martes.

**[00:09:15] Natalia Vega:** Quería traer un tema de soporte. Nos llegan muchos tickets por el error de sesión expirada. Habría que revisar cuánto dura la sesión.

**[00:09:28] Tomás Ibarra:** Eso es configuración, no es difícil. Pero tiene que verlo alguien de infraestructura, no nosotros.

**[00:09:36] Gabriela Ortiz:** Sí, eso hay que resolverlo, decidido: lo subimos de 30 minutos a 8 horas. Que lo vea alguien de infra.

**[00:09:44] Hernán Silva:** ¿Le escribo a alguien de infra o lo hace otro?

**[00:09:47] Gabriela Ortiz:** Después vemos quién. Sigamos.

**[00:12:20] Hernán Silva:** Volviendo a la migración. Me acaban de confirmar en el chat que el sábado hay un proceso de cierre contable que usa esa base. No podemos tocarla el sábado.

**[00:12:34] Tomás Ibarra:** Uh. ¿Y el martes a la noche?

**[00:12:39] Hernán Silva:** El martes a la noche sí, de 22 a 24.

**[00:12:44] Gabriela Ortiz:** Entonces la migración se mueve al martes a la noche. Hernán sigue a cargo. Natalia, avisa a los clientes grandes que el martes de 22 a 24 los reportes no van a estar.

**[00:12:55] Natalia Vega:** Ok, lo mando mañana.

**[00:15:10] Tomás Ibarra:** Último tema mío. El monitoreo de errores nuevo. Yo me encargo de dejarlo configurado antes del release.

**[00:15:20] Gabriela Ortiz:** ¿Cuándo sale el release?

**[00:15:22] Tomás Ibarra:** El viernes de la semana que viene.

**[00:15:25] Gabriela Ortiz:** Perfecto, entonces el monitoreo antes de eso.

**[00:18:40] Camila Reyes:** ¿Retomamos lo de QA?

**[00:18:44] Gabriela Ortiz:** Nos quedamos sin tiempo. Lo hablamos la próxima, o por chat. Gracias a todos.

**[00:18:50] Tomás Ibarra:** Gracias.
