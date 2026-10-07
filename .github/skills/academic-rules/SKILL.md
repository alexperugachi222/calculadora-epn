name: academic-rules
description: Usala siempre que escribas, modifiques o revises cddigo o textos
que calculen o muestren notas, sumas de bimestres, estados acadomicos o la
calificacion requerida en el supletorio.

# Reglas academicas de la Calculadora de Supletorio

## Reglas
Cada bimestre se califica sobre 20 y admite hasta dos decimales
(0.00 a 20.00).
La suma de los dos bimestres es sobre 48.
Estado: suma < 18 Reprobado (no hay supletorio); 18 <= suma < 28 Supletorio
(de 18.00 a 27.99); suma >- 28 Aprobado. No uses 17.99 ni 27.99 como
limites: dejarian sumas sin estado,
El supletorio es sobre 40. Calificacion requerida - el mayor entre 24 y
(48 - suma). Solo existe cuando el estado es Supletorio.
Quien saca la requerida aprueba. La app solo informa: no guarda la nota del
supletorio.

# Exactitud numerica
. Los bordes de las reglas deben dar siempre el estado correcto. La forms de
representar, validar y comparar las notas la decide la spec, no el agente.
Rechara mis de dos decimales, valores negativos y valores mayores a 20.

##  Checklist de revision
- [ ] ¿Se prueban los bordes 17.99, 18.00, 27.99 y 28.00?
- [ ] ¿Se prueban 24.00 y 24.01 on la calificación requerida?
- [ ] ¿5e prueban 0.00, 20.00 y un tercer decimal (15.123)?
[ ] ¿Los bordes dan el estado correcto, sin errores de redondeo?
[ ] ¿Los mensajes son exactamente los de la spec?

## Al terminar
Indica que puntos del checklist has comprobado y como.