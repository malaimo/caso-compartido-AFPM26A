---
source: real
participant: Ricardo Salinas
role: Director de Ingeniería de Plataforma, Lumen Cloud (proveedor SaaS de infraestructura, unos 2.000 empleados, México, Estados Unidos, Colombia y España)
country: México
survey_respondent: R-196
survey_channel: panel
guide: product/interview-guides/2026-09-23-2030-colaboracion-en-vivo-fuera-de-teams.md
date: 2026-09-28
duration: 26 min
mode: exploration
interviewer: Equipo de producto
---

# Entrevista: Ricardo Salinas

**Entrevistador:** Gracias por conectarte, Ricardo. Para arrancar, cuéntame brevemente qué hace tu equipo y qué reuniones conduces en una semana típica.

**Ricardo:** Plataforma. Somos los que mantenemos la infraestructura sobre la que corren los productos: clústeres, bases de datos, redes, observabilidad. Tengo unas sesenta personas, en cuatro países. Reuniones conduzco... muchas. Cuatro o cinco grandes por semana, fácil, sin contar las que no conduzco.

**Entrevistador:** Quiero que pensemos en una reunión concreta: la última reunión de Teams de más de cinco personas que condujiste en la que el grupo trabajó junto sobre algo, un documento, una lista, unos datos.

**Ricardo:** Es que todas son iguales, la neta. Nos conectamos, cada quien habla de lo suyo, y ya.

**Entrevistador:** Entiendo. Si tuvieras que elegir una sola, la más reciente, ¿cuál sería?

**Ricardo:** Pues la sync semanal de plataforma, el martes pasado. Esa es la más grande: dieciséis personas. Los líderes de cada célula, los dos arquitectos, gente de México, de Bogotá, de Austin y dos de Madrid.

**Entrevistador:** Llévame por esa reunión desde que empezó. ¿Qué tenían que lograr y qué hizo el grupo?

**Ricardo:** Cada célula da su estado: qué avanzó, qué está bloqueado, qué necesita de otro equipo. Son como cuatro minutos por célula, aunque siempre se alargan. Y al final, si hay algo que priorizar entre equipos, lo vemos ahí. En pantalla no había nada. A veces alguien comparte una gráfica de Grafana si hubo un incidente, pero el martes no. Todo hablado. Tampoco hay un documento de la sync, cada líder trae sus notas y ya, lo que se dice se queda en la llamada.

**Entrevistador:** Mencionaste que al final priorizan. ¿Cómo lo hicieron el martes?

**Ricardo:** Había dos pedidos de otros equipos y capacidad para uno. Pregunté quién prefería el primero y levantaron la mano, la manita de Teams. Yo cuento. Salieron nueve contra siete, algo así.

**Entrevistador:** ¿Quién hablaba y quién no?

**Ricardo:** Hablan los mismos cuatro o cinco de siempre. Los de Madrid casi nunca, por la hora, para ellos ya es noche. Los demás tienen la cámara apagada y, pues, supongo que están trabajando en otra cosa. Yo haría lo mismo.

**Entrevistador:** Esa parte de votar, ¿siempre se resolvió así, hablando y con la mano?

**Ricardo:** Sí. Bueno, una vez probamos la pizarra de Teams, en un taller de arquitectura, hace como un año. Éramos doce. Se trabó, las notas tardaban en aparecer, y no encontré cómo agruparlas. Perdimos quince minutos y volvimos a la plática. No la volví a abrir. Y lo que habíamos puesto ahí, ni idea, supongo que sigue en algún lado. Nadie lo fue a buscar.

**Entrevistador:** ¿Alguna vez usaron otra herramienta dentro de la reunión para eso?

**Ricardo:** No. ¿Se puede? No sabía que se podían meter otras herramientas en la reunión. Pero tampoco me hace falta, la verdad.

**Entrevistador:** Cuéntame cómo lo resuelven ustedes y seguimos. ¿Hay otra reunión tuya de más de cinco personas donde el grupo trabaje de otra forma?

**Ricardo:** No realmente. Mira, te voy a ser sincero, lo que a mí me pesa no es cómo trabajamos en la reunión. Es la cantidad. Tengo veintisiete horas de reuniones a la semana. Veintisiete. Es la mitad de mi calendario. Y la mitad de esas podrían ser un correo. Mi equipo está igual, se la pasan en llamadas y luego me preguntan por qué no avanzamos.

**Entrevistador:** Lo anoto, es importante. En esta conversación me voy a quedar en lo que pasa dentro de esas reuniones, si te parece. En la sync del martes, ¿qué se decidió?

**Ricardo:** Lo del pedido que ganó la votación. Y nada más, porque las decisiones grandes no se toman ahí. Se toman después, con los dos arquitectos, en una llamada aparte, los tres. Ahí sí decidimos en serio. Con dieciséis personas no se puede decidir nada, cada quien jala para su lado.

**Entrevistador:** Y lo que deciden ustedes tres, ¿qué pasa para que quede registrado y se cumpla?

**Ricardo:** Uno de los arquitectos escribe un ADR en el repositorio, a veces. O yo lo aviso en la siguiente sync. Depende.

**Entrevistador:** Piensa en la última vez que algo que se decidió en una reunión terminó hecho distinto de lo acordado. ¿Qué pasó entre la reunión y eso?

**Ricardo:** Uy... déjame pensar. No sé si me acuerdo de una. Es que pasa, pero no te sé decir cuál.

**Entrevistador:** No hay prisa.

**Ricardo:** Ah, ya. La migración de Postgres, en septiembre. Teníamos que mover las bases de facturación a los clústeres nuevos. En la sync se dijo el orden: primero las réplicas de lectura, después las primarias. Bueno, eso entendí yo que se dijo. El equipo de Bogotá empezó por las primarias y el de México por las réplicas. Cuando nos dimos cuenta ya había una base primaria migrada sin sus réplicas. Fueron dos días arreglando eso y un fin de semana con guardia extra.

**Entrevistador:** ¿Qué pasó entre la reunión y la migración?

**Ricardo:** Nada, ese es el punto. Se habló en la sync, cada uno se fue con su versión y nadie lo escribió. Yo pensé que el arquitecto iba a hacer el ADR y él pensó que yo lo iba a mandar por correo. Pero te digo, el problema de fondo es que había demasiada gente en la reunión. Con dieciséis personas, cada quien escucha lo que quiere.

**Entrevistador:** ¿Hay algo sobre cómo trabaja tu equipo en las reuniones que no te pregunté y debería haberte preguntado?

**Ricardo:** No, creo que ya lo dije. Menos reuniones.

**Entrevistador:** ¿Conoces a otro líder que conduzca reuniones grandes de una forma muy distinta a la tuya?

**Ricardo:** Si quieren saber de colaboración, hablen con los tech leads, no conmigo. Ellos son los que hacen las sesiones de diseño, las retros, todo eso. Le puedo pasar tu contacto a Daniela, que lidera la célula de redes, ella usa tableros y esas cosas.

**Entrevistador:** Te lo agradezco mucho. Gracias por el tiempo, Ricardo. Esto se junta con otras conversaciones para entender cómo trabajan los equipos en reuniones grandes, y te podemos compartir lo que salga.

**Ricardo:** Va. Gracias.
