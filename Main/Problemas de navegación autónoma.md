2024-11-22 16:13

Status:[[En Proceso]]

Autor: [[OR Carrasco]]

Categoría: [[Marco teórico]]


Tags: [[Navegación]], [[Kalman]], [[Tags/Localización|Localización]], [[Planeación de trayectoria]], [[Seguimiento de trayectoria]], [[Ingeniería de control]].

Autores: [[OR Carrasco]]

Estoy escribiendo con el tecladito
# Problemas de navegación autónoma

### Localización


La navegación autónoma en exteriores tiene como complicaciones tres problemas principales, la localización, la planeación de trayectorias y el sorteo de obstáculos. El problema de localización radica en cómo el sistema puede conocer su ubicación y orientación; para conocer su ubicación una técnica que se usa con frecuencia es el posicionamiento global satelital y para dar aún más certeza de las mediciones es posible la implementación de receptores fijos que trabajen en conjunto con el receptor del sistema móvil. Otra práctica común es usar múltiples sensores y fusionar los resultados tratando las mediciones como distribuciones normales que se procesarán a través de diferentes algoritmos como lo es el filtro Kalman. 

Es importante resaltar que aunque los filtros tipo Kalman sean ampliamente usados en el ámbito de la robótica no son las únicas técnicas empleadas para el problema de localización en un sistema de navegación autónoma, el filtro Kalman pertenece a una familia de filtros llamada filtros Bayesianos. También están los algoritmos markovianos que funcionan en base a un mallado del terreno.


# Referencias..

 
 

 
 Ff