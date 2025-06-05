2024-12-01 11:26

Status: [[Terminada]]

Tags:[[Sensores]], [[Vehículos autónomos]], [[Clasificación del terreno]], [[deep learning]], [[GPS]], [[redes neuronales]] 

Autores: [[Fabio Vulpi]], [[Annalisa Milella]], [[Roberto Marani]], [[Giulio Reina]]

Categoría [[Fuentes de conocimientos/Investigación original]]


# Recurrent and convolutional neural networks for deep terrain classification by autonomous robots

### ¿Qué se hizo?
Propusieron una manera de identificación de terreno sin necesidad de visión computarizada ni información de profundidad a partir de sensores proprioreceptivos  mediante redes neuronales recurrentes o redes neuronales convolucionales.


### ¿Cómo se hizo?
Usaron la plataforma experimental husky que se muestra en la figura 1 del paper, la plataforma cuenta con encoders para medir el la velocidad angular de las ruedas, sensores eléctricos de corriente para medir de manera indirecta el par de torsión y un módulo inercial xsens Mti-300. La plataforma cuenta también con sensores exteroceptivos como una cámara estereográfica, GPS, y un láser para exteriores que no fueron usados en el proyecto.

Dos tipos de información se recabó: información de la IMU con un rate de 50Hz y la información de las ruedas con un rate de 15Hz.

La tabla uno muestra los tipos de terrenos y la cantidad de ventanas (partition windows) que se usaron para el entrenamiento

Usaron redes neuronales convolucionales (CNN) para diez canales de entrada correspondiendo a los diferentes sensores. *Se hizo uso de la transformada de Fourier la cual contiene coeficientes complejos*


### ¿Qué se encontró? 
Los resultados obtenidos se compararon con resultados obtenidos con  *Support vector machine* (SVM), la cual es una técnica ampliamente utilizada en problemas de clasificación

# referencias
https://doi.org/10.1016/j.jterra.2020.12.002


