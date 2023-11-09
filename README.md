# Titulo: Redes neuronales convolucionales para la detección de Salmonella spp. en aves de corral
### Especialización en Analítica y Ciencia de datos
### Universidad de Antioquia (2023-II)
### Autor: Melissa Ortega Alzate

# Paso a paso de la implementación y como ejecutar el script:
Para el procesamiento de los datos, primero se importan las librerías necesarias y se define una función para visualizar diagramas de barras y figuras aleatorias del conjunto de imágenes.

Luego se carga y limpia el archivo que contiene las etiquetas de las imágenes, procedimiento que incluye conocer el tamaño y tipo de datos de cada columna, verificar duplicados y cambiar el nombre de las columnas. Así como, el número de imágenes en la carpeta, su tamaño, formato y tipo.

Más adelante se encuentra la sección de visualización, allí se grafica un diagrama de barras para para visualizar la distribución de instancias respecto a las categorías de la variable de salida. Además, se usa la función definida que permite ver imágenes aleatorias para conocer 16 imágenes y sus clases.

En el preprocesamiento de las imágenes, se utiliza un ciclo para cargar y estandarizar cada imagen dividiendo los pixeles por 255. Además, se establece el tamaño de todas como 224x224 pixeles en caso de que alguna estuviera por fuera de esta especificación. En este ciclo se crea una lista, en donde cada elemento corresponde a una imágen de tamaño (224, 224, 3). Luego, la lista es convertida a un tensor de tamaño (5027, 224, 224, 3). Sin embargo, en el Notebook de Collab será de (20, 224, 224, 3).

Se dumifica la variable de salida, obteniendo 1 para las imágenes clasificadas con Salmonella y 0 para las imágenes saludables. Con lo anterior, se obtiene un archivo .csv modificado con las clases y tensor (arreglo de numPy multidimensional) con las imágenes.

Finalmente, el tensor con las imágenes es asignado a X y las etiquetas a y, para ser divididas en los trenes de entrenamiento y prueba. Ambas variables será posteriormente utilizadas para el entrenamiento de un modelo de Red Neuronal Convolucional.

### Nota 1
El Notebook "ME03_data_preparation_collab" de Google Collaboratory usa los archivos del repositorio como insumo para su ejecución. Sin embargo, es una muestra pequeña y algunas celdas cambian parcialmente para poder establecer esta conexión.

En el Notebook "ME03_data_preparation_local" se muestra un script ejecutado con las celdas y código como debe ser ejecutado en un ambiente local y con todas las imágenes disponibles. Por favor, revisar también.

### Nota 2
En GitHub se cargó una muestra de 20 imágenes, 10 de cada clase.


### Estándares de desarrollo
- Usar ramas diferentes para cada issue
- Usar la guía de estilos de [Python de Google](https://google.github.io/styleguide/pyguide.html)
- Mantener los commits cortos y con descripción