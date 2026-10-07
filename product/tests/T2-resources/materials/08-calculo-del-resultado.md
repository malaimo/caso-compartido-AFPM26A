# T2 · Comparación y cálculo del resultado

## 1. Comparar cada reunión (hoja `06-hoja-comparacion.csv`)
Lo hacen dos personas: alguien de tech y uno de los anotadores. Ninguna de las dos cambia la clave en este paso.

Para cada entrada de la clave con `tipo` decisión o compromiso, se busca el elemento de la IA que dice lo mismo (mismo contenido, aunque esté redactado distinto). El minuto ayuda a encontrarlo.
- **correcta:** está, con el mismo contenido, el mismo responsable y la misma fecha (o las dos dicen `sin responsable` / `sin fecha`). Una fecha relativa y su fecha calendario cuentan como la misma.
- **incorrecta-contenido / -responsable / -fecha:** está, pero algo de eso no coincide. Se marca la primera que falle, en ese orden. Si la IA inventó un responsable o una fecha que no se dijo, es incorrecta.
- **faltante:** ningún elemento de la IA la cubre.

Después, cada elemento de la IA que no quedó emparejado:
- **propuesta-como-decision:** coincide con una entrada `no-decision` de la clave (propuesta no adoptada, tema postergado, observación o versión reemplazada).
- **extra:** no coincide con nada de la clave (repetido, inventado, o algo que los anotadores no consideraron). Se registra, pero la fórmula del diseño no lo cuenta.

El motivo no se usa para clasificar.

## 2. Tasa de error (sobre todas las reuniones juntas)

```
D = entradas de la clave con tipo decisión o compromiso
error = (incorrectas + faltantes + propuestas-como-decision) / D
```

- Si D es menor que 30: resultado `inconclusive`. No se aplica la regla de decisión.
- Además del total, se reporta el error por reunión y por líder, y separado para decisiones y compromisos, para entender de dónde viene. El umbral se aplica solo al total.

## 3. Tiempo de revisión (hoja `07-hoja-revision.csv`)
- El líder recibe la lista de la IA de cada una de sus reuniones, una por vez, en una sesión por Teams.
- El cronómetro arranca cuando el líder abre la lista y para cuando dice que la publicaría tal como quedó.
- Se toma la **mediana de minutos por reunión** sobre todas las reuniones revisadas.

## 4. Regla de decisión (fija, del diseño)
| error | mediana de revisión | resultado |
|---|---|---|
| 20% o menos | 5 min o menos | **continue** |
| 20% o menos | más de 5 min | **change** |
| más de 20% y hasta 35% | cualquiera | **change** |
| más de 35% | cualquiera | **discard**: A1 se cae y A2 queda con lista manual |

`change` significa ajustar el prompt o la salida y repetir con transcripciones nuevas, nunca con las mismas.
