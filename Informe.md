# **Sistema de prediccion y recomendación para el aprendizaje en Entorno Virtuales de Aprendizaje**

## Ciencias de la Computacion
## Universidad de La Habana
### Autor:
* Jorge Alejandro Soler González

## 1. Introducción

La educación es un aspecto fundamental en la vida de cualquier persona, y en la actualidad, gracias a los avances tecnológicos, y en los últimos tiempos a raíz de la pandemia del COVID-19, el aprendizaje se ha vuelto más accesible y flexible a través de los entornos virtuales de aprendizaje. En estos entornos es difícil para los profesores obtener el desempeño de un estudiante durante un curso, y proveer a tiempo una atención personalizada al mismo. Usualmente se obtiene la información del curso una vez que este concluye, y esta es la base de la falta de confianza y el pobre aprendizaje de un estudiante dentro de un curso.

Una forma de detectar a los estudiantes que van a tener un pobre desempeño dentro de un curso: es hacer predicciones tempranas de sus notas en los diferentes temas del mismo. El propósito de predecir el aprendizaje que puede tener un estudiante dentro de un curso: es entender el desempeño académico del estudiante en su trayectoria de aprendizaje dentro del entorno, ayudar a los profesores a entender las condiciones académicas en las que están los estudiantes, y en el caso de la presente tesis: implementar planes personalizados de recomendación basados en dicha predicción.

El uso de modelos de predicción para el análisis del aprendizaje así como los sistemas de recomendación presentan múltiples retos, especialmente el cómo obtener, procesar y usar los datos para construir el modelo. A este campo dentro de la analítica del aprendizaje se le llama: minería de datos educacionales. En este estudio se precisan 3 grupos de indicadores fundamentales: la interacción del estudiante con el medio, interaccion del estudiante con el curso y la interacción que pueda existir entre estudiante y profesor. Este preprocesamiento de los datos tiene significativa importancia ya que interviene directamente en la precisión y en el costo computacional del modelo.

En este contexto, la presente tesis tiene como objetivo principal desarrollar un modelo predictivo y un sistema de recomendación a partir de los datos extraidos de un entorno virtual de aprendizaje, para este estudio nos enfocaremos en Moodle, un LMS de libre acceso, open source y el más usado a nivel mundial.Se quiere predecir el comportamiento de un estudiante en un curso y a partir de esta predicción, se busca ofrecer recomendaciones personalizadas que se adapten a las necesidades y preferencias individuales de cada estudiante, con el fin de mejorar su experiencia de aprendizaje y aumentar su rendimiento académico.

Para lograr el objetivo se tendrán en cuenta los siguientes pasos:
1. Extraer los datos pertinentes del LMS
2. Procesar dichos datos: para esto se propone utilizar una combinación de los siguientes métodos:
    * método de peso de entropía (entropy weight method)
    * filtrado de varianza (variance filtering)
    * estrategia de fusión de características autoadaptable
    Todo esto con el objetivo de dejar los datos lo más limpios posible para aumentar la precisión y disminuir el costo computacional del modelo.
3. Construcción del modelo: algoritmo de aprendizaje de máquina (machine learning), SVC (support vector classification)
4. A partir de la predicción construir un sistema de recomendacion, basado en el historial del estudiante en el entorno virtual y los requerimientos del curso donde se encuentra.
