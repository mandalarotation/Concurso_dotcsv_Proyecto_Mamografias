# Pix2pix para analisis de mamografias

Para este proyecto, se entrenó la red Pix2pix en dos sentidos, con dos objetivos diferenciados pero igualmente importantes:

## 1) Generar una mama realista a partir de un dibujo simple para encontrar una solución al problema de imágenes en medicina:

<img src="imagenes/5751717.png" width="900px"/>

Es complicado acceder a la información por imágenes médicas debido a las políticas de confidencialidad de los pacientes, lo cual, es claramente aceptable pero restringe la transmisión de conocimientos más allá de los resultados. Para fines investigativos en los que los resultados sean publicables, entrenar la red Pix2pix es una excelente alternativa para generar material educativo o imágenes que sirvan como data de entrenamiento para otros tipos de redes o problemas específicos.
 
## 2) Obtener un dibujo simple que represente las características mas importantes de la mama a partir de un estudio clínico:

<img src="imagenes/6548.png" width="900px"/>

Las imágenes en mamografía se tornan complicadas en su análisis ya que sus estructuras son difíciles de segmentar; esto hace que la sustracción de características sea tediosa si no se cuenta con herramientas de mayos complejidad. El uso de la Pix2pix permite automatizar el proceso de diferenciación de estructuras individuales para trabajar con este tipo de imágenes médicas.

## Recolección de las imagenes

Debido a la restricción de transmisión de información de centros radiológicos, se utilizaron en total 524 imágenes para el entrenamiento de ambos modelos; estas fueron recolectadas con el motor de búsqueda de imágenes de Google y Baidú usando palabras clave como "tomosintesis", "mamografía" o "cancer de mama" en siete idiomas distintos: español, ingles, ruso, alemán, mandarín, japonés e hindi.
Las imágenes recolectadas fueron tratadas manualmente con el fin de tener sus características morfológicas principales; este proceso, haciendo uso del software Autodesk Sketchbook. Algunas de las imágenes de prueba se escalaron además para poder ajustarlas a los requerimientos de tamaño de la red. Otros efectos propios de la imagen como la nitidez, la iluminación o las condiciones de formación se tuvieron en cuenta como factores determinantes en la variabilidad de resultados y la posibilidad de que estos pudieran enmascarar las características deseadas a la red.

<img src="imagenes/25775.png" width="900px"/>

[Dar click para ver el video donde se expone el procedimiento para delinear las imagenes](https://youtu.be/-59jc6V7aNs)

## Ejemplos de aplicación

### vista de la mama sin segementar

<img src="imagenes/4257545.png" width="900px"/>

### Vista de la mama segmentada

<img src="imagenes/2255.png" width="900px"/>

[Dar click para ver el código y el procedimiento detallado de como segmentar la mama](https://github.com/mandalarotation/Concurso_dotcsv_Proyecto_Mamografias/blob/master/Ejemplos/example_AtoB/example_tomosintesis.ipynb)

Por  razones de capacidad de almacenamiento en Github, los modelos ya entrenandos no vienen directamente en el repositorio, [clic para descargar los modelos entrenados.](https://drive.google.com/file/d/12bOJ5WMeZOCbBw6w0DDblljTDvXVLUdZ/view?usp=sharing).  Una vez descargados y extraídos, se ubicarán en la carpeta "modelos entrenados".  Siempre que se cargue un checkpoint en el código, verificar la dirección en la que quedó ubicado el modelo.

[Dar click para ver el video donde se expone el procedimiento para desarrollar los ejemplos, entrenar y utilizar las redes](https://youtu.be/oIyCk5IhObY)

## Autor

Jean Carlo Jiménez Giraldo (Estudiante Ing Industrial - Universidad Nacional de Colombia)

## Colaboradores

Andrés Usuga Hoyos (Estudiante maestría en física - Universidad Nacional de Colombia),
Javier de Jesús Morales Aramburo (Profesor de Física - Universidad Nacional de Colombia),
David Gomez Bohorquez (Estudiante Ing Industrial - Universidad Nacional de Colombia)

## Agradecimientos

DotCSV,
John William Branch Bedoya (Profesor de sistemas - Universidad Nacional de Colombia),
Esteban Gonzales (Estudiante Ing Industrial - Universidad Nacional de Colombia),
Brayhan Armando Quintero (Estudiante Ing Industrial - Universidad Nacional de Colombia),
Felipe Andrés Zuluaga (Estudiante Ing Industrial - Universidad Nacional de Colombia),
Yubar Daniel Marin ([semillero Unalytics](https://unalyticsteam.github.io/unalytics.github.io/) - Universidad Nacional de Colombia),
Esteban Bermudez ([semillero Unalytics](https://unalyticsteam.github.io/unalytics.github.io/) - Universidad Nacional de Colombia),
Todos los integrandes de ([semillero Unalytics](https://unalyticsteam.github.io/unalytics.github.io/) - Universidad Nacional de Colombia),
Luis Eduardo Oliveros - (Estudiante ing física - Universidad Nacional de Colombia),
ALberto Ceballos - (Estudiante Maestria Ing Sistemas - Universidad Nacional de Colombia),
Jairo Rodriguez - (Estudiante Ing física - Universidad Nacional de Colombia),Estefania Orrego Restrepo (Estudiante Maestría Ing Química - Universidad Nacional de Colombia)
 


## Referencias 

@article{pix2pix2016,
  title={Image-to-Image Translation with Conditional Adversarial Networks},
  author={Isola, Phillip and Zhu, Jun-Yan and Zhou, Tinghui and Efros, Alexei A},
  journal={arxiv},
  year={2016}
}

