---
title: "Compensations in Manas overtime"
date: 2024-08-08 10:00:00 +0000
layout: default
---

## Breve historia de los salarios y compensaciones en Manas

Manas fue cambiando la forma en la que definió los salarios en sus 20 años de historia.
Durante los primeros 8 años 2003-2011 fue una estrategia tradicional, el CEO definía los salarios, siempre abierto a comentarios, sugerencias, críticas, pero al final una sola persona decidía.

Este modelo empezó a crujir cuando Manas empezó a crecer y se hacia imposible visualizar desde una sola persona las tareas de todos.

Como solución a este problema se creó [Asignum](https://github.com/manastech/asignum) que dio inicio a una nueva fase en la cual los salarios eran definidos exclusivamente por los pares. 

Fue exitosa como estrategia para la distribución de los fondos disponibles y a la vez fue una herramienta muy fuerte de cohesión interna, en general primaba la idea de cuidarnos entre nosotros.

Este modelo encontró su límite hacia 2018 luego de otra crisis de crecimiento, Manas necesitaba crecer, tener más senior devs, pero los salarios que Manas podía ofrecer estaban fuera de los rangos de mercado.

Para superar esta situación se modificó el sistema agregando 3 componentes más a la 
revisión de pares
- Componente básico por país
- Rubrica de competencias
- Roles


## Asignum times 

Asignum fue la herramienta interna que creó Manas para distribuir internamente.
[Repo de asignum](https://github.com/manastech/asignum)

Qué quería evitar
- Evitar los sesgos personales de uno decidiendo por varios
- Superar las escalas salariales siempre lentas, siempre estancas
- Esquivar los sesgos provocados por los sistemas de recompensas
- No babysitear adultos

Qué quería lograr
- Que todos participen 
- Que haya menos disconformidad con los salarios (partimos de la base de que es imposible que no haya algune disconforme, la idea es reducir esa disconformidad no evitarla)
- Que dependa menos de factores subjetivos (o que dependa de una subjetividad grupal que no es propiedad de ningún sujeto)

> _El resultado de la suma de las optimizaciones individuales es la mejor optimización a la que podemos aspirar dada la naturaleza distribuida del conocimiento colectivo._

Features que rindieron buenos frutos
- Compartir comentarios (Agregó un montón de valor a nivel grupal la posibilidad de dejar mensajes anónimos) 
- Distribuir en rondas (para corregir)
 
[Demo de Asignum](http://localhost:3000/)

Desde Asignum en adelante en Manas se fijó el hábito de tener rondas de asignaciones/compensaciones
Las rondas para definir salarios eran eventos importantísimos donde todos se tomaban muy en serio el trabajo, había estrategias muy diversas, obviamente algunos se habían armado su propia app para procesar los datos.

### Asignum limits

Asignum empezó a ser un problema cuando los salarios se empezaron a estancar.

Gracias al sistema de reparto por pares los salarios en Manas resultaron ser muy similares, los juniors que recién entraban ganaban solo 4 veces menos de lo que ganaba el senior con más experiencia. Más allá de cuán de acuerdo estabamos personalmente con esa situación, era un problema que nos alejaba del mercado en el que estábamos trabajando.

Se intentó mantener asignum modificando la cantidad de dinero disponible para que cada persona distribuya, de haberse hecho antes tal vez hubiera funcionado, pero al momento en el que se implementó era demasiado tarde.

## El último draft: los 4 componentes

El sistema actual surgió como respuesta a la crisis de crecimiento, no borró del todo al viejo asignum pero lo relegó a un rol menor.
Se basa en 4 componentes
- Componente básico (crítico para una empresa global)
- Rúbrica de competencias
- Roles y responsabilidades
- Peer review (Asignum)

[Herramienta actual de compensaciones](https://compensation.manas.tech/)

### El componente básico

Es algo así como un costo de vida por ciudad/país como para garantizar que los que trabajen para Manas puedan comer caliente.... 
Se calcula con herramientas como [numbeo](https://www.numbeo.com/cost-of-living/country_result.jsp?country=Argentina) [Big Mac Index](https://www.economist.com/big-mac-index)

### La rúbrica

Es un modelo muy interesante adaptado de la [rubrica de medium](https://docs.google.com/spreadsheets/d/1EO-Dbsayn8Nz9Ii3MKcwRbt-EIJ2MjQdpoyhh0tBdZk/edit?gid=2049640133#gid=2049640133). 
La idea es que se puede actualizar periodicamente de manera didtribuida, cualquiera puede pedir una review de un track de cualquier compañero (solo para promoverlo, no para bajarlo)

Tiene de bueno que:
- Es público, todos lo ven
- Es abierto, todos pueden participar
- Es transparente, todos pueden ver los detalles que definen cada track y cada milestone

Tiene de malo que:
- Las condiciones inciales influyen demasiadoL: si empezás con 30 puntos va a ser muy dificil que superes los 90, vas a tener que pedir 10 reviews en un año.
- Es costoso de mantener: cuando se pide una review hay que fundamentar el pedido, elegir jurado, esprar a que el jurado se junte para evaluarlo, que hagan la devolución y eso toma tiempo, lo cual refuerza el punto anterior.
- Sesgo de personalidad: No todos tienen la actitud para pedir una review.

Posibles mejoras:
- Limitar la cantidad de tracks: hay superposiciones entre algunos.
- Consensuar señales y ejemplos para que las reviews sean más rápidas

### Los roles

Es un modelo de escala clásico, que no está mal si combina con otros
[Ver detalle](https://compensation.manas.tech/role)

### El peer review

Es el mismo asignum de siempre, con la particularidad de que el aumento conseguido por este medio se considera bono y se resetea en cada asignación.

