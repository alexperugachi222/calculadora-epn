# Decisiones - HU-001: Registrar una materia

## 1. Rango permitido para la nota

- **Pregunta:** ¿Qué rango de valores se acepta para la nota del primer bimestre?
- **Respuesta:** De 0 a 10, incluyendo ambos extremos.
- **Motivo:** Define cuándo una nota está dentro del rango válido y permite aceptar los valores límite.

## 2. Formato de la nota

- **Pregunta:** ¿Qué formato se permite para ingresar la nota?
- **Respuesta:** Se aceptan números enteros o decimales con hasta dos cifras decimales, usando punto como separador (por ejemplo, `8.25`).
- **Motivo:** Establece un formato de entrada concreto y la precisión admitida.

## 3. Datos incompletos o inválidos

- **Pregunta:** ¿Cómo debe responder la aplicación ante nombre vacío, nota vacía o nota inválida?
- **Respuesta:** Mostrar un mensaje junto al campo que se debe corregir, mantener abierto el formulario y conservar lo ingresado; no guardar la materia.
- **Motivo:** Indica qué corregir sin perder los datos que ya ingresó el estudiante y evita guardar información inválida.

## 4. Detección de materias repetidas

- **Pregunta:** ¿Cuándo se debe considerar repetido el nombre de una materia?
- **Respuesta:** Cuando coincide ignorando diferencias entre mayúsculas y minúsculas y los espacios al inicio o al final.
- **Motivo:** Evita duplicados que solo difieren por el uso de mayúsculas o espacios exteriores.

## 5. Respuesta ante una materia repetida

- **Pregunta:** ¿Cómo debe responder la aplicación al intentar guardar una materia repetida?
- **Respuesta:** Mostrar un mensaje junto al nombre, no guardar la materia y mantener el formulario para que se pueda corregir.
- **Motivo:** Explica el problema en el campo relevante y permite corregirlo sin volver a ingresar los datos.

## 6. Nombre guardado y mostrado

- **Pregunta:** ¿Cómo se deben tratar los espacios al inicio y al final del nombre al guardar?
- **Respuesta:** Eliminarlos y guardar y mostrar el nombre ya limpio.
- **Motivo:** Mantiene coherentes el nombre que se muestra y el criterio usado para detectar duplicados.

## 7. Error al guardar en el dispositivo

- **Pregunta:** ¿Qué debe ocurrir si falla el guardado en el dispositivo?
- **Respuesta:** Mostrar un mensaje claro del error, conservar los datos del formulario y no indicar que la materia quedó guardada.
- **Motivo:** Evita comunicar un guardado exitoso que no ocurrió y permite reintentar sin perder lo ingresado.
