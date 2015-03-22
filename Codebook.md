# CodeBook
Este es un 'Codebook' que describe las variables, los datos, y cualquier transformación o trabajo que se haya hecho para limpiar los datos.

## Fuente de los datos

Datos originales: https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip
Descripción original del conjunto de datos: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

## Data Set Information

El experimento se llevó a cabo con un grupo de 30 voluntarios de entre 19 a 48 años de edad. Cada persona realizó seis actividades (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) usando un smartphone (Samsung Galaxy S2 ) en la cintura. Usando el acelerómetro y el giroscopio del teléfono, se capturaron datos de aceleración lineal y velocidad angular en 3 ejes, a una tasa constante de 50Hz.

## Los daots

Los datos incluyen los siguientes archivos:

'README.txt'
'features_info.txt': Muestra la información acerca de las variables.
'features.txt': Lista de todas las características.
'activity_labels.txt': Enlaza las etiquetas de clase con el nombre de la actividad.
'train/X_train.txt': Set de entrenamiento.
'train/y_train.txt': Etiquetas de entrenamiento.
'test/X_test.txt': Set de pruebas.
'test/y_test.txt': Etiquetas de las pruebas.

Los siguientes archivos están disponibles para los datos de pruebas y entrenamiento.

'train/subject_train.txt': Cada fila indentifica al sujeto que realizó la actividad para cada muestra. Su rango va de 1 a 30.

'train/Inertial Signals/total_acc_x_train.txt': La señal de aceleración del acelerómetro del smartphone en el eje X está en unidad estándar 'g'. Cada fila muestra 128 elementos vectoriales. La misma descripción se aplica para los archivos 'total_acc_x_train.txt' y 'total_acc_z_train.txt', correspondientes a los ejes Y y Z, respectivamente.

'train/Inertial Signals/body_acc_x_train.txt': La señal de aceleración del cuerpo, obtenida de la sustracción de la gravedad de la aceleración total.

'train/Inertial Signals/body_gyro_x_train.txt': Vector de velocidad angular, medido por el giroscopio para cada muestra. La unidades son radianes/segundos.

Detalles de las transformaciones

1) Unir los datos de entrenamiento y las pruebas para crear un único set de datos.
2) Extraer solo las mediciones sobre la media y la desviación estándar para cada medida.
3) Usar nombres descriptivos para nombrar las actividades en el set de datos.
4) Etiquetar apropiadamente los datos con los nombres.
5) Crear un segundo tidy data set, con el promedio de cada variable para cada actividad y cada sujeto.

## How run_analysis.R implements the above steps:

Requiere los paquetes reshapre2 y data.table.
Cargar los set de datos de pruebas y entrenamiento (test & train)
Cargar las etiquetas de características y actividades (features & activity)
Extraer la media y la desviación estándar de las columnas, nombres y datos.
Procesar los datos.
Unir los datos.
