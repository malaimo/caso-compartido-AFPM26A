---
opportunity: decisiones-sin-cierre-en-reuniones
solutions: product/solutions/2026-09-29-2055-decisiones-sin-cierre-en-reuniones.md
status: designed
---

# Solution tests for: Las decisiones de las reuniones grandes no se cierran

## Why test
Dos alternativas en prueba, A2 `cierre-confirmado-en-vivo` y A1 `recap-de-decisiones`. Las dos tienen el dolor evidenciado (`real`, n=10; `survey`, n=182), pero nadie reaccionó todavía a ninguna de las dos soluciones. De A2 no sabemos si los grupos hacen el cierre cuando la reunión se alarga. De A1 no sabemos si la IA separa decisión de propuesta con precisión suficiente; la única reacción que hay es al recap actual, y es negativa. Quedan fuera de este archivo la creencia 9 (viabilidad, entrevistas con IT) y la restricción de "tiempo real" (si se mantiene, A1 queda afuera); las dos siguen en la agenda de la oportunidad.

## T1. cierre-confirmado-en-vivo: cierre manual en reuniones reales durante 2 semanas
- **Test status:** designed
- **Belief under test:** "[feature: cierre-confirmado-en-vivo] [usability] Los grupos del segmento reservan y usan 2 a 3 minutos al final de la reunión para confirmar la lista de decisiones. Se falsa si, en un piloto de 4 semanas con 8 a 10 líderes, el cierre se saltea en más de la mitad de las reuniones con decisiones." (creencia 12 de `product/overview.md`). Este test es un primer paso más chico que el piloto que nombra la creencia: usa el mismo umbral (más de la mitad salteado) con menos líderes y menos tiempo.
- **Risk:** [usability]
- **Test type:** concierge (cierre manual, sin herramienta nueva)
- **What we do:**
  1. Sesión de 15 minutos con cada líder: se le explica el cierre (en los últimos minutos, mostrar en pantalla la lista de decisión, responsable, fecha y motivo en las notas de reunión existentes, y pedir a cada responsable que confirme en voz alta "es mío" antes de cortar).
  2. El líder lo aplica en todas sus reuniones de más de 5 participantes con decisiones durante 2 semanas, sin recordatorios nuestros durante la reunión.
  3. Después de cada reunión con decisiones, el líder completa la hoja de captura (2 minutos) y comparte la lista de las notas.
  4. Al final, entrevista de 15 minutos con cada líder sobre las reuniones donde el cierre no se hizo: por qué.
- **With whom:** 5 líderes del segmento (Business Premium, 100+ licencias, tecnología, 3+ países) que conducen reuniones de más de 5 con decisiones al menos 2 veces por semana, reclutados del pool de opt-in de la encuesta (64 elegibles). Objetivo: 10 a 15 reuniones con decisiones en total; menos de 8 reuniones vuelve el resultado `inconclusive`.
- **Material needed:** (1) guía de una página para el líder con el guion del cierre; (2) plantilla de la lista en las notas de reunión existentes (decisión, responsable, fecha, motivo, confirmado sí/no); (3) hoja de captura por reunión: fecha, cantidad de participantes, duración prevista y real, si hubo decisiones, si el cierre se hizo completo / parcial / se salteó, minutos que llevó, motivo si se salteó (tiempo, se olvidó, incomodidad, otro), cuántas decisiones quedaron y cuántas cambiaron de responsable o fecha al confirmarse; (4) guion de la entrevista final. Se deja afuera a propósito: borrador de IA, publicación en Jira u otras herramientas, recordatorios automáticos, cualquier interfaz nueva.
- **Material:** pendiente (`/build-solution-test`)
- **Duration:** 2 semanas de uso, más 1 semana de reclutamiento y sesiones iniciales.
- **Signal and threshold:** proporción de reuniones con decisiones en las que el cierre se hizo completo (lista visible y cada responsable confirmó). Pasa si se hizo completo en al menos la mitad de las reuniones y la mediana de duración del cierre es de 3 minutos o menos. Falla si se salteó o quedó parcial en más de la mitad.
- **Decision rule:** continue si el cierre se hizo completo en al menos la mitad de las reuniones con mediana de 3 minutos o menos · change si se hizo en al menos la mitad pero la mediana supera 3 minutos, o si falla y el motivo dominante es olvido o incomodidad (probar una versión con borrador previo o recordatorio) · discard si falla y el motivo dominante es falta de tiempo (reuniones que se alargan): A2 se cae y queda A1 sola, como prevé el archivo de soluciones.
- **Expected provenance:** real
- **Next step if it passes:** el piloto de 4 semanas con 8 a 10 líderes del archivo de soluciones, para la creencia 13 ([value]: las decisiones mal ejecutadas bajan al menos a la mitad contra el mes anterior), con su propio diseño. Si en ese piloto el ritual sin herramienta alcanza, se revisa si vale construir algo (A4).

## T2. recap-de-decisiones: precisión de la extracción contra una clave a ciegas
- **Test status:** designed
- **Belief under test:** "[feature: recap-de-decisiones] [feasibility] La IA extrae decisión, responsable y fecha y separa propuesta de decisión con precisión suficiente para publicarse tras una revisión corta. Se falsa si, sobre grabaciones reales, más de 1 de cada 5 decisiones extraídas es incorrecta o falta, o si la revisión del líder lleva más de 5 minutos." (creencia 14 de `product/overview.md`)
- **Risk:** [feasibility]
- **Test type:** technical-test
- **What we do:**
  1. Juntar transcripciones de reuniones reales ya grabadas, de más de 5 participantes y con decisiones, de líderes del segmento que den su consentimiento.
  2. Armar la clave a ciegas: dos personas marcan, en cada transcripción, cada decisión con su responsable, fecha (si se dijo) y motivo, sin ver la salida de la IA. Lo que no coincide lo resuelve el líder de esa reunión.
  3. Correr la extracción (prompt sobre el recap o la transcripción) y comparar con la clave.
  4. Darle a cada líder la lista de su reunión y medir cuánto tarda en dejarla lista para publicar.
- **With whom:** owner: tech. Datos: 12 a 15 reuniones de 4 a 5 líderes del pool de opt-in (pueden ser los mismos de T1, sobre grabaciones previas al test), con al menos 40 decisiones en la clave; menos de 30 vuelve el resultado `inconclusive`. Revisión: los líderes de esas reuniones.
- **Material needed:** (1) el prompt de extracción con formato de salida fijo (decisión, responsable, fecha, motivo); (2) el conjunto de transcripciones; (3) la clave a ciegas con sus reglas de anotación (qué cuenta como decisión y qué como propuesta); (4) hoja de comparación por decisión: correcta, incorrecta (responsable o contenido equivocado, o propuesta marcada como decisión), faltante; (5) hoja de captura del tiempo de revisión por reunión. Se deja afuera a propósito: interfaz de revisión, publicación, contexto de pantalla o apps compartidas (se prueba después si esto pasa).
- **Material:** pendiente (`/build-solution-test`)
- **Duration:** 2 semanas (1 para la clave, 1 para correr, comparar y medir la revisión).
- **Signal and threshold:** tasa de error = (decisiones incorrectas + faltantes + propuestas marcadas como decisión) / decisiones en la clave. Pasa si la tasa de error es de 20% o menos y la mediana de revisión del líder es de 5 minutos o menos por reunión.
- **Decision rule:** continue si error de 20% o menos y revisión de 5 minutos o menos · change si el error está entre 20% y 35%, o si el error pasa pero la revisión supera 5 minutos (ajustar el prompt o la salida y repetir el test con transcripciones nuevas) · discard si el error supera 35%: A1 se cae y A2 queda con lista manual, como prevé el archivo de soluciones.
- **Expected provenance:** real
- **Next step if it passes:** prototype-shown para la creencia 15 de `product/overview.md` ("[feature: recap-de-decisiones] [value] Los líderes publican la lista de decisiones de la IA, revisada, en lugar de armar su propio registro. Se falsa si, mostrada la lista de su propia reunión, menos de la mitad de los líderes la publica o la manda en lugar de su acta, correo o carga en Jira."), con su propio diseño.

## Results

## Decision
