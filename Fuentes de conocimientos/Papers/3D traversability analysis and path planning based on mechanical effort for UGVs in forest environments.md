2024-12-04 12:55

Status: [[Terminada]]

Tags: [[Robótica Forestal]], [[Análisis de transversabilidad]], [[Planeación de trayectoria]], [[Esfuerzos mecánicos]], [[UGVs]], [[Navegación]], [[ROS]].

Autores: [[Alfonso E. Carvalho]], [[João Filipe Ferreira]], [[David Portugal]]

Categoría [[Clasificación del terreno]] [[Fuentes de conocimientos/Investigación original]]


# 3D traversability analysis and path planning based on mechanical effort for UGVs in forest environments

### ¿Qué se hizo?
Desarrollaron una metodología para el análisis de transversabilidad y con ello planear una trayectoria que procesa mapas tridimensionales de nube de puntos para computar el gradiente de información y con ello detectar obstáculos para generar trayectorias eficientes.

### ¿Cómo se hizo?

Con la información proporcionada por  un mapa tridimensional de nube de puntos de terreno previamente cargado en el sistema para preprocesarlo de tal modo que se filtren los puntos fuera del rango de trabajo del robot.

Desarrollaron siete módulos para ROS:
1. Preprocesamiento
2. Construcción de mapa mallado
3. Recorte vertical de la información 
4. Cálculo del mapa del gradiente
5. Estimación de los esfuerzos mecánicos 
6. Acoplamiento de la información 
7. Detección de obstáculos evidentes 

En el preprocesamiento se tomó un mapa tridimensional de puntos de nube para filtrarlo y usar solamente el área de trabajo del robot.

El módulo del mapa mallado genera con la información del preprocesamiento un mapa en dos dimensiones 

Con toda esta información y el procesamiento de la información se genera un mapa que muestra las zonas que requerirán mayor esfuerzo mecánico para la movilidad del robot, lo cual brinda información importante acerca del terreno donde el robot realizará su trabajo.

Los resultados se contrapusieron con la metodología de mapeo de elevación.
### ¿Qué se encontró? 

Que las trayectorias generadas por esta manera aunque sean diferentes a las generadas por la metodología de mapeo de elevación son diferentes los resultados en las métricas tienen poca variación con excepción del tiempo recorrido.

Esta metodología aunque provoca trayectos más largos el riesgo de una volcadura se minimiza, siendo uno de los problemas de los UGVs que al generar una trayectoria se genera la más corta sin importar el incremento en el riesgo.

# referencias

