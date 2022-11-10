# TSR-2022-1-Tarea-02-Investigaci-n-Algoritmo-Go-to-Point-

## Contenido

- [Objetivo](#objetivo)
- [Desarrollo](#desarrollo)
- [Autor](#autor)
- [Referencias](#referencias)

## Objetivo
Un robot móvil del tipo (2,0) se encuentra en el punto P(x0, y0) con una rotación de θ radianes en su eje Z. Se requiere llegar al punto P(x1, y1) sin importar su orientación (θ radianes de giro sobre su eje Z).

Investigar el algoritmo "Go to point simple" para cumplir con la tarea expuesta en el problema.
En la investigación se debe proponer el código del algoritmo usando los datos del problema.
Contestar a as preguntas:
¿Cuales son las ventajas y desventajas de utilizar la función atan2?
¿Cómo variaría el algoritmo si la orientación
"θ" en el P1 fuera necesaria?
¿A que tribuye los errores de orientación y distancia que se producen durante el movimiento?

## Desarrollo
Dados $\displaystyle P(x\index{0},y\index{0})}$ para llegar a \math-container{P(x\index{1},y\index{1}) se desea saber el ángulo que
el robot debe girar y lo que tiene que avanzar para llegar a su destino.

El robot primero gira y luego avanza. 
El angulo $\displaystyle \theta $ se calcula de la siguiente forma:
$\displaystyle \theta =\arctan\left(\frac{y_{1} -y_{0}}{x_{1} -x_{0}}\right)$

Posteriormente, debe avanzar una distancia:
$\displaystyle \sqrt{(x\index{1}-x\index{0})\power{2}+(y\index{1}-y\index{0})\power{2}}$
