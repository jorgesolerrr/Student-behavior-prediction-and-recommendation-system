# **Sistema de predicción y recomendación para la enseñanza en Entornos Virtuales de Aprendizaje**

## Ciencias de la Computacion
## Universidad de La Habana
### Autor:
* Jorge Alejandro Soler González

## 1. Introducción

La formación de competencias profesionales es un aspecto fundamental en el proceso de instrucción en las instituciones educativas. En la actualidad, gracias a los avances tecnológicos, el aprendizaje se ha vuelto más accesible y flexible a través de los entornos virtuales de aprendizaje (EVA). Recientemente, la humanidad se encuentra aún dando solución a un problema global de pandemia que potenció la educación a distancia y todos sus mecanismos de enseñanza. En estos entornos es un reto para los profesores obtener una métrica que permita analizar y predecir el desempeño de cada estudiante durante un curso en el logro del aprendizaje de cada objetivo de estudio. Este instrumento permitiría proveer a tiempo una atención personalizada a los discentes, logrando una intervención oportuna que lograría conducir y afianzar la confianza del estudiante, a pesar de las brechas detectadas, en los resultados al finalizar el curso.

Los objetivos de predecir el desempeño que puede tener un estudiante dentro de un curso son:
* Es entender el aprendizaje académico del estudiante en su trayectoria en cada objetivo académico dentro del entorno
* Ayudar a los profesores a entender las condiciones y realidades académicas en las que están los estudiantes, y en el caso de la presente tesis:
* Implementar planes personalizados de recomendación basados en dicha predicción.

Una forma de detectar a los estudiantes que pudieran tener un desempeño medio o bajo dentro de un curso, es realizar predicciones tempranas de sus calificaciones en los diferentes temas que se abordan.

El uso de modelos de predicción para el análisis del aprendizaje, así como los sistemas de recomendación, presentan múltiples desafíos, especialmente el cómo obtener, procesar y usar los datos para construir el modelo. A este campo dentro de la analítica del aprendizaje se le llama: Minería de datos educacionales. En este estudio se proponen 2 grupos de indicadores fundamentales con métricas entre las que podemos mencionar: 
* Grupo A para la interacción del estudiante con el EVA:
    - Cantidad de veces que el estudiante ha ingresado a las actividades y recursos de la plataforma.
    - Nivel de participación en los tipos diferentes de actividades.
* Grupo B para la interacción del estudiante con el aula virtual:
    - Tiempo de acceso a los materiales que se orientan para el cumplimiento de un objetivo académico.
    - Tiempo que se demora en entregar una tarea o responder un cuestionario.
    - Resultado de la evaluación que se otorga por el docente en cada actividad interactiva de cada objetivo académico.

 Este preprocesamiento de los datos tiene significativa importancia ya que interviene directamente en la precisión y en el costo computacional del modelo.

En el contexto de la presente tesis, el objetivo principal es desarrollar un modelo predictivo y un sistema de recomendación a partir de los datos extraídos de un entorno virtual de aprendizaje. Para este estudio se utilizará el software Moodle como herramienta EVA donde se desarrollaron las aulas virtuales y por tanto poseen la información estadística. En resumen, la pertinencia del uso de este EVA se basa en ser de libre acceso, open source y el más utilizado a nivel mundial por las instituciones educativas. 

Como resultado de este trabajo se pretende predecir el comportamiento de un estudiante en un curso y, a partir de esta predicción, se busca ofrecer recomendaciones personalizadas adaptadas a las necesidades y preferencias individuales de cada alumno, con el fin de mejorar su experiencia en el proceso de enseñanza y aumentar su rendimiento académico.

Para lograr este objetivo se tendrán en cuenta los siguientes pasos:
1. Extraer los datos pertinentes del EVA utilizando conexión vía API a la información.
2. Procesar los datos obtenidos en el paso 1, proponiendo la utilización de una combinación de los siguientes métodos:
    * Método de peso de entropía (Entropy weight method)
    * Filtrado de varianza (Variance filtering)
    * Estrategia de fusión de características auto-adaptables
    
    Lo anterior, con el objetivo de obtener datos limpios que posibiliten aumentar la precisión y disminuir el costo computacional del modelo.
3. Construir el modelo: Implementación de algoritmo de aprendizaje de máquina (Machine learning) con SVC (Support vector classification).
4. Construir un sistema de recomendación, basado en el historial del estudiante en el entorno virtual y los requerimientos del curso donde se encuentra, a partir de la predicción obtenida en el paso 3.


