---
feature: recap-de-decisiones
spec: product/specs/2026-10-13-1945-recap-de-decisiones.md
exposure-plan: product/exposure-plans/2026-10-13-2047-recap-de-decisiones.md
level: 1
status: designed
created: 2026-10-20
---

# Métricas: Recap de IA centrado en decisiones (nivel 1)

**Nivel:** 1, lista privada de decisiones, solo lectura. Duración: 2 semanas.
**Creencia del nivel:** los líderes ven en la lista lo que se decidió en su reunión, y les parece que corregirla da menos trabajo que escribir su propia acta.

## Audiencia objetivo

Organizadores de reuniones grabadas o transcritas de más de 5 participantes, en cuentas Max que cumplen la firmografía del segmento (tecnología, 100+ licencias, operación en 3+ países, facturación mayor a USD 100M). Se excluyen las cuentas con operación en el Espacio Económico Europeo mientras legal no confirme.

- El segmento de la oportunidad son cuentas Business Premium, pero la función se ata a Max: se mide la parte del segmento que ya está en Max.
- El mecanismo es incremental: el nivel llega a todas las cuentas Max y el segmento se aplica como filtro del análisis, no de la exposición.
- **Quiénes cuentan:** solo organizadores. En el nivel 1 la lista es privada y los participantes no la ven.
- **Tamaño:** desconocido (pregunta abierta para el equipo).

## Frecuencia esperada

Semanal: al menos una reunión con decisiones por semana. `assumption`.
Base: el 90% de quienes respondieron conduce 2 o más reuniones de más de 5 por semana (190 de 210; `survey`, product/surveys/2026-09-26-1800-respuestas-colaboracion-en-vivo-fuera-de-teams.csv). No está medido cuántas de esas reuniones tienen decisiones.

## acquisition

- **Señal:** el organizador abre la lista de decisiones de una reunión suya.
- **Definición ampliada:** cuenta abrir la vista de la lista. No cuentan que la lista se haya generado ni que el aviso se haya mostrado (estados internos).
- **Cálculo:** organizadores de la audiencia que abrieron al menos una lista en las 2 semanas ÷ organizadores de la audiencia con al menos una reunión elegible en esas 2 semanas.
- **Target:** 70%. `assumption`. Tiene que estar por encima del 60% de reapertura que pide el plan. Referencia: 6 de 10 entrevistados usan o probaron el recap (`real`, n=10) y la lista aparece en el mismo lugar. No hay línea base de apertura del recap actual.
- **Lectura secundaria, reapertura:** organizadores de la audiencia con 2 o más reuniones elegibles que abrieron la lista en 2 reuniones o más ÷ organizadores de la audiencia con 2 o más reuniones elegibles. Target 60%; por debajo de 40% se detiene. Lee los criterios de reapertura del plan.

## activation

- **Señal:** el organizador recorre completa la lista de una reunión con al menos una decisión detectada.
- **Umbral de señal:** abre la lista y llega a la sección de propuestas y temas abiertos.
  - **Justificación:** para reconocer la lista como lo que se decidió (creencia del nivel) hay que leerla entera. Llegar a propuestas muestra que vio la separación entre decisión y conversación, que es lo que el recap actual no hace.
  - **Excluye:** abrir y cerrar sin bajar, y las listas con "No se detectaron decisiones".
- **Cálculo:** organizadores de la audiencia que cumplen el umbral en al menos una reunión en las 2 semanas ÷ organizadores de la audiencia con al menos una reunión elegible.
- **Target:** 50%. `assumption`. Para responder con fundamento si a la lista le falta poco o nada, primero hay que haberla leído entera. Con acquisition en 70%, implica que unos 7 de cada 10 que la abren la recorren.

## retention

- **Señal:** el organizador vuelve a cumplir el umbral de activation en una semana posterior.
- **Definición ampliada:** cuenta volver a obtener valor, no volver a abrir.
- **Ventana:** semanal.
- **Cálculo:** organizadores de la audiencia que cumplen activation en la semana 1 y en la semana 2 ÷ organizadores de la audiencia con al menos una reunión elegible en cada una de las dos semanas.
- **Target:** 40%. `assumption`. Equivale a que 4 de cada 5 activados vuelvan. La lista aparece sola después de cada reunión, así que volver no cuesta nada extra.
- **Cohorte para la curva:** organizadores agrupados por la semana de su primera activation. En el nivel 1 hay 2 puntos; la misma cohorte se sigue durante el nivel 2 (misma audiencia) para tener 4 semanas de curva.

## satisfaction

- **Instrumento:** pregunta en el producto, al final de la lista.
- **Pregunta:** "¿Cuánto le falta a esta lista para usarla como registro de lo que se decidió?"
  - Nada, la usaría así
  - Poco, corregiría algunos ítems
  - Mucho, tendría que rehacerla
  - Campo opcional: "¿Qué le falta?"
- **Momento:** al llegar a la sección de propuestas (al cumplir activation), como máximo una vez por semana y por organizador.
- **Corte:** satisfecho = "Nada" o "Poco". Si un organizador responde dos veces, cuenta la última.
- **Cálculo:** organizadores que responden "Nada" o "Poco" ÷ organizadores de la audiencia que respondieron. Se informa al lado la tasa de respuesta (respondieron ÷ activados).
- **Target:** 50%, el criterio de avance del plan.

## Reconciliación con el plan de exposición

| Criterio del nivel 1 | Métrica que lo lee |
|---|---|
| Avanzar: al menos el 60% de los organizadores con 2 o más reuniones abre la lista en 2 o más | acquisition, lectura de reapertura, target 60% |
| Avanzar: al menos la mitad responde que le falta poco o nada | satisfaction, target 50% |
| Detener: menos del 40% vuelve a abrirla | acquisition, lectura de reapertura, por debajo de 40% |
| Detener: la mayoría responde que tendría que rehacerla | satisfaction, más del 50% "Mucho" |

Sin contradicciones entre targets y criterios.

## Métricas de negocio

- **Tasa de upgrade a Max del segmento:** 3,1% hoy (product/overview.md, creencia 9). La audiencia del nivel 1 ya está en Max, así que este nivel no la mueve. Se sigue durante y después del nivel 3, como dice el plan.

## Eventos a instrumentar

| Evento | Propiedades | Lo usa |
|---|---|---|
| `decision_list_generated` | meeting_id, organizer_id, account_id, participant_count, decision_count, proposal_count, timestamp | denominadores; filtro de listas sin decisiones |
| `decision_list_opened` | meeting_id, user_id, account_id, entry_point, timestamp | acquisition, reapertura |
| `decision_list_section_viewed` | meeting_id, user_id, section (decisions, proposals), timestamp | activation, retention |
| `decision_list_source_clicked` | meeting_id, user_id, item_id, timestamp | análisis (verificación contra la transcripción) |
| `decision_list_survey_shown` | meeting_id, user_id, timestamp | tasa de respuesta |
| `decision_list_survey_answered` | meeting_id, user_id, answer (none, little, redo), comment, timestamp | satisfaction |

Los nombres de eventos son una propuesta y se ajustan a la convención de instrumentación del producto.

## Condiciones previas al revelado

- T2 (precisión de la extracción, creencia 14) sigue sin correr y el plan la pone como condición previa al nivel 1.
- Confirmación de legal sobre el Espacio Económico Europeo.
