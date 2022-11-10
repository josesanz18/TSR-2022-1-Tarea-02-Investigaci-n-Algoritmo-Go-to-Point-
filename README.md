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
### Algoritmo Go to point
Dados $\displaystyle P(x_{0},y_{0})$ para llegar a $\displaystyle P(x_{1},y_{1})$ se desea saber el ángulo que
el robot debe girar y lo que tiene que avanzar para llegar a su destino.

El robot primero gira y luego avanza. 
El angulo $\displaystyle \theta$ se calcula de la siguiente forma:
$$\displaystyle \theta =\arctan\left(\frac{y_{1} -y_{0}}{x_{1} -x_{0}}\right)$$

Posteriormente, debe avanzar una distancia:
$$\displaystyle \sqrt{(x_{1}-x_{0})^{2}+(y_{1}-y_{0})^{2}}$$

### Función atan2
Las ventajas de usar atan2 es que nos permite tener un dominio de $\displaystyle -\pi$ a $\displaystyle \pi$, siendo muy útil en la transformación de coordenadas cartesianas a polares

### Orientacion en P1
Para lograr llegar al punto destino con una orientación definida, sería necesario emplear el mismo algoritmo planteado anteriormente, y agregar un giro cuando ya haya alcanzado el punto.

## Autor
**Autor** Sánchez Espinosa José Manuel [Git hub profile](https://github.com/josesanz18)

##Referencias
