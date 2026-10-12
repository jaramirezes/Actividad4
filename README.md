# Actividad4
Identificar e implementar el modelo preentrenado más adecuado para un caso de uso específico.

Desarrollo de un sistema de visión artificial basado en aprendizaje profundo para clasificar 14 categorías de daños de autos usando modelos en Hugging Face. El proceso automatiza la lectura de imagenes y XML por medio de Google Colab utilizando el dataset Car Damage Detection de Kaggle.

# Objetivo
El es mejorar la evaluación de daños de siniestros de autos, utilizando herramientas de inteligencia artificial como Hugging face, realizo el entrenamiento y la comparación de 3 modelos de visión por computadora: ViT (google/vit-base-patch16-224), ResNet-50 (microsoft/resnet-50) y ConvNeXt (facebook/convnext-tiny-224).

# Dataset y Scripts de Soporte
# Descripción del origen del dataset.
El dataset que utilizo es de kaggle, Car Damage Detection

Se encuentra en la siguiente página de Kaggle :
https://www.kaggle.com/code/samyukthamobile/car-damage-detection/input

# Estructura (descripción de cada campo).
dataset_siniestros_procesado.csv, contiene 2 campos :
Campo       Tipo de Dato	            Función
filename	  Cadena de texto (string)	Identificador del archivo de imagen.
label_real	Cadena de texto (string)	Categoría del tipo de daño del vehículo.

Contiene 390 imagenes con su correspondiente XML, siendo un total de 780 archivos contenidos en valid.zip el cual está anexo en este repositorio.

# Carga del dataset
Debemos descargar el archivo zip "valid.zip" en el equipo para utilizarlo en el proceso de comparación de modelos, lo descargamos en cualquier carpeta para despues seleccionarlo en la ejecución de la celda de código "Carga de modelos y datasets".

El archivo CSV se genera en la sesion de la nuve de Google con el nombre dataset_siniestros_procesado.csv, este archivo y las imagenes se borran al cerrar la sesion, por lo que se tiene que cargar nuevamente en cada ejecución.

Hay que realizar la autentificación en Hugging Face, para realiar el login.

El proceso lo lee y genera en base a los xml el archivo dataset_siniestros_procesado.csv, junto con las fotografías para entrenar el modelo.

En el Goggle Colab se deben de ir ejecutando los pasos en forma ejecutiva para correr el proceso.




