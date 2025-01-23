2024-11-23 12:51

Status:  [[En Proceso]]

Categoría: [[Reviews]]

Tags:[[Inteligencia artificial]], [[Vehículos autónomos]],[[Fusión de data]], [[Machine learning]], [[Sensores]], [[LiDAR]].

Autores: [[Semih Beycimen]], [[Dmitry Ignatyev]], [[Argyrios Zolotas]]


# A comprehensive survey of unmanned ground vehicle terrain transversability for unstructured environments and sensor insight

## *Este paper es un review*

### ¿Qué es el análisis de transversabilidad en el terreno?

##### *Esta información se obtuvo del preámbulo* 
- Los terrenos tienen diferentes características, unos pueden tener tierra firme, tierra suelta, ser pedregosos, fangosos, lodosos, e incluso esas características pueden presentar cambios debido a cuestiones temporales como lo podría ser una lluvia.

- Dada la variedad de superficies en las que un vehículo se puede ver expuesto su capacidad de navegación se puede ver alterada por la incertidumbre del estado del terreno.

- El análisis de transversabilidad en el terreno consiste la  **clasificación del terreno**, **el mapeo del terreno** y el **costo de la transversabilidad**
- El análisis se puede realizar con técnicas de **aprendizaje** (*machine learning*, *deep learning* o *reinforcement learning*) o *procedimientos analíticos*.



### ¿Cómo se clasifican los terrenos?

#### *Esto viene en el capítulo 2 terrain transversability analysis*
- Los terrenos se pueden clasificar con varios métodos como métodos basados en geometría, basados en la apariencia incluso una mezcla de ambos. También es posible el uso de métodos de [[Machine learning]] o [[deep learning]].

Los métodos basados en apariencia parten de sistemas de visión computarízada o incluso sistemas de LiDAR. Al usar cámaras RGB es posible provocar alto contraste en las imágenes para su clasificación y así lograr la identificación de obstáculos, tipo de suelo etc.

- El uso de segmentación semántica es una práctica común para identificar los elementos del terreno para clasificar el terreno.

Otra alternativa a los métodos basados en apariencia son los métodos basados en geometría. 


### ¿Qué se encontró? 


# referencias

https://doi.org/10.1016/j.jestch.2023.101457