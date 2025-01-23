2024-12-05 15:04

Status: [[En Proceso]]

Tags: [[Análisis de transversabilidad]], [[Segmentación semántica]], [[Ambientes de terracería]], [[Mapeo de elevación]], [[Mapeo de costo]], [[ROS]].

Autores: [[Tiga Ho Yin Leung]], [[Dmitry Ignatyev]], [[Argyrios Zolotas]].

Categoría: [[Investigación original]]


# Hybrid terrain traversability analysis in off-road environments

### ¿Qué se hizo?
Usaron segmentación semántica para la clasificación de terreno en terracería para identificar los diferentes tipos de terreno que rodean al robot, con esto el robot puede optimizar su trayectoria. A su vez mediante la valoración de las propiedades geométricas con ayuda de un mapa de elevación permite considerar las capacidades físicas del robot dentro de un análisis de transversabilidad.



### ¿Cómo se hizo?

Usaron procesamiento de imágenes junto con una nube de puntos de LiDAR y la información proveniente de sensores proprioreceptivos.

El trabajo lo dividieron en tres módulos principales, segmentación semántica, Mapeo de elevación y generación de mapa de transversabilidad.

El módulo de segmentación semántica toma una image RGB tiene como salida una máscara semántica colorizada que indica la localización de los diferentes tipos de terreno en el plano 2D. El módulo de Mapeo de elevación se utiliza después para generar un mapa centrado en el robot a 2.5D. La posición de las “mallas” están relacionadas con un marco de referencia coordinado tridimensional y cada malla contiene la información de altura correspondiente a cada posición. En el módulo de generación de mapa de transversabilidad se incorporan las salidas de los módulos anteriores permitiendo la generación de un mapa de costo.

Los módulos fueron generados en ROS.
### ¿Qué se logró? 

Lograron a partir de las imágenes obtener una ruta de traversabilidad donde las áreas con colores menos profundo son las zonas que se pueden transitar con mayor facilidad mientras que las zonas más oscuras representan mayor costo. 

Un aspecto a resaltar es que esta metodología no es en línea, es decir en tiempo real, por lo que esto representa un área de oportunidad.
# referencias

