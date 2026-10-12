# Actividad4
Identificar e implementar el modelo preentrenado más adecuado para un caso de uso específico.

Desarrollo de un sistema de visión artificial basado en aprendizaje profundo para clasificar 14 categorías de daños de autos usando modelos en Hugging Face. El proceso automatiza la lectura de un zip para cargar imagenes y XML en la nube de Google Colab, el dataset utilizado es Car Damage Detection de Kaggle.

# Objetivo
Es mejorar la evaluación de daños de siniestros de autos, utilizando herramientas de inteligencia artificial como Hugging face, realizando el entrenamiento y la comparación de 3 modelos de visión por computadora: ViT (google/vit-base-patch16-224), ResNet-50 (microsoft/resnet-50) y ConvNeXt (facebook/convnext-tiny-224).

# Dataset y Scripts de Soporte
# Descripción del origen del dataset.
El dataset que utilizo es de kaggle, Car Damage Detection

Se encuentra en la siguiente página de Kaggle :
https://www.kaggle.com/code/samyukthamobile/car-damage-detection/input

# Estructura (descripción de cada campo).
dataset_siniestros_procesado.csv, contiene 2 campos :

| Campo | Tipo de Dato | Función |
| :--- | :--- | :--- |
| `filename` | Cadena de texto (`string`) | Identificador del archivo analizado. |
| `label_real` | Cadena de texto (`string`) | Categoría del tipo de daño del vehículo. |

El dataset contiene 390 imagenes con su correspondiente XML, siendo un total de 780 archivos contenidos en valid.zip el cual está anexo en este repositorio.

# Carga del dataset
Debemos descargar el archivo zip "valid.zip" en el equipo, para utilizarlo en el script Actividad_4_entrega.IPYNB de comparación de modelos, lo descargamos en cualquier carpeta para despues seleccionarlo en la ejecución de la celda de código "Carga de modelos y datasets", este proceso se realiza en Google Colab y se explica paso a paso a continuación:

# Entorno de ejcución
Google Colab, se requiere conexión a Hugging Face.

# Pasos de ejecución

1) En Goggle Colab abrimos el script Actividad_4_entrega.IPYNB
2) Se deben de ejecutar las celdas de código de manera consecutiva para correr el proceso.
3) Nos conectamos a Hugging Face
4) Continuamos ejecutando las celdas
5) Al llegar a la celda "Carga de modelos y datasets", nos pide seleccionar el archivo.
6) Nos aparece el mensaje que dice "Por favor, selecciona tu archivo .zip con las imágenes y los XMLs:" y damos click a la caja "Elejir Archivos", buscamos el archivo valid.zip descagado previamente en nuestra computadora y lo seleccionamos.
Nota : Si no seleccionamos el archivo zip el proceso estará detenido esperando la carga.
7) Continuamos ejecutando las celdas hasta finaliar todas las celdas.

El archivo CSV se genera en la sesion de la nube de Google con el nombre dataset_siniestros_procesado.csv, este archivo y las imagenes se borran al cerrar la sesion de Goggle, por lo que se tiene que cargar nuevamente el zip en cada ejecución.






