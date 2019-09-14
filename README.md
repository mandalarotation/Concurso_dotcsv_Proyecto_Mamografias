# Pixtopix para analisis de mamografias

En este proyecto se entrena la red pixtopix en dos sentidos con dos objetivos distintos pero muy importantes

## 1) Generar una mama realista a partir de un dibujo simple:

<img src="imagenes/5751717.png" width="900px"/>

Este obejetivo busca encontrar una solución al problema de la poca disponiblidad de imagenes en medicina; por ejemplo para investigación es muy dificil poder acceder a dicha información y de poderse es muy común que nada de los procedimientos se puedan hacer públicos debido a la confidencialidad de los pacientes, entonces la trasmisión de conocimiento se ve bastante limitada y todo queda solo la publicación de los resultados, por dicha razón la pixtopix puede ser una excelente opción para generar material educativo y tambien para generar imagenes que despues pueden servir como data de entrenamiento para otro tipo de redes o problemas especificos.
 
## 2) Obtener un dibujo simple que represente las caracteristicas mas importantes de la mama a partir de una imagen realista de la misma: 

<img src="imagenes/6548.png" width="900px"/>

Uno de los mayores problemas a la hora de trabajar con estas imagenes es que aveces son dificiles de segmentar y sustraer ciertas caracteristicas se vuelve una tarea muy complicada incluso aveces imposible si no se cuenta con herramientas especiales, entonces la pixtopix es una buena opción para automatizar la sustracción de estas caracteristicas.

## Recolección de las imagenes

Para el entrenamiento de ambos modelos se utilizaron en total 524 imagenes todas ellas fueron recolectadas de google imagenes y baidú imagenes, buscando las palabras clave "tomosintesis", "mamografía" y "cancer de seno" en siete idiomas distintos; español, ingles,ruso,alemán,chino,japonés e hindú, despues de hacer la recoleción se procedió a delinear las caracteristicas a simple vista visibles con el software de dibujo autodesk sketchbook, es de recalcar tambien que algunas imágenes tuvieron que ser deformadas un poco para poderlas ajustar a los requerimientos de tamaño de la red, ademas como fueron recolectadas de diversas fuentes, tiene gran variabilidad en cuanto los efectos, la nitidez, la iluminación y las condiciones con que fueron tomadas, aún así se siguió adelante con el proceso, todo con la esperanza de que tanta variabilidad no resultara enmascarando a la red las caracteristicas de interes.

<iframe width="560" height="315" src="https://www.youtube.com/embed/-59jc6V7aNs" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>





