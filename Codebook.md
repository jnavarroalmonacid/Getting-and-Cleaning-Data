# CodeBook
<<<<<<< HEAD

This is a code book that describes the variables, the data, and any transformations or work that you performed to clean up the data.

## The data source

* Original data: https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip
* Original description of the dataset: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

## Data Set Information
=======
Este es un 'Codebook' que describe las variables, los datos, y cualquier transformación o trabajo que se haya hecho para limpiar los datos.

## Fuente de los datos

Datos originales: https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip
Descripción original del conjunto de datos: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones
>>>>>>> origin/master

## Información del set de datos

El experimento se llevó a cabo con un grupo de 30 voluntarios de entre 19 a 48 años de edad. Cada persona realizó seis actividades (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) usando un smartphone (Samsung Galaxy S2 ) en la cintura. Usando el acelerómetro y el giroscopio del teléfono, se capturaron datos de aceleración lineal y velocidad angular en 3 ejes, a una tasa constante de 50Hz.

<<<<<<< HEAD
## The data
=======
## Los datos
>>>>>>> origin/master

Los datos incluyen los siguientes archivos:

- 'README.txt'

<<<<<<< HEAD
- 'features_info.txt': Shows information about the variables used on the feature vector.

- 'features.txt': List of all features.

- 'activity_labels.txt': Links the class labels with their activity name.

- 'train/X_train.txt': Training set.

- 'train/y_train.txt': Training labels.

- 'test/X_test.txt': Test set.

- 'test/y_test.txt': Test labels.
=======
'features_info.txt': Muestra la información acerca de las variables.

'features.txt': Lista de todas las características.

'activity_labels.txt': Enlaza las etiquetas de clase con el nombre de la actividad.

'train/X_train.txt': Set de entrenamiento.

'train/y_train.txt': Etiquetas de entrenamiento.

'test/X_test.txt': Set de pruebas.

'test/y_test.txt': Etiquetas de las pruebas.
>>>>>>> origin/master

Los siguientes archivos están disponibles para los datos de pruebas y entrenamiento.

<<<<<<< HEAD
- 'train/subject_train.txt': Each row identifies the subject who performed the activity for each window sample. Its range is from 1 to 30.

- 'train/Inertial Signals/total_acc_x_train.txt': The acceleration signal from the smartphone accelerometer X axis in standard gravity units 'g'. Every row shows a 128 element vector. The same description applies for the 'total_acc_x_train.txt' and 'total_acc_z_train.txt' files for the Y and Z axis.

- 'train/Inertial Signals/body_acc_x_train.txt': The body acceleration signal obtained by subtracting the gravity from the total acceleration.

- 'train/Inertial Signals/body_gyro_x_train.txt': The angular velocity vector measured by the gyroscope for each window sample. The units are radians/second.

## Transformation details
=======
'train/subject_train.txt': Cada fila indentifica al sujeto que realizó la actividad para cada muestra. Su rango va de 1 a 30.

'train/Inertial Signals/total_acc_x_train.txt': La señal de aceleración del acelerómetro del smartphone en el eje X está en unidad estándar 'g'. Cada fila muestra 128 elementos vectoriales. La misma descripción se aplica para los archivos 'total_acc_x_train.txt' y 'total_acc_z_train.txt', correspondientes a los ejes Y y Z, respectivamente.

'train/Inertial Signals/body_acc_x_train.txt': La señal de aceleración del cuerpo, obtenida de la sustracción de la gravedad de la aceleración total.

'train/Inertial Signals/body_gyro_x_train.txt': Vector de velocidad angular, medido por el giroscopio para cada muestra. La unidades son radianes/segundos.

Detalles de las transformaciones
>>>>>>> origin/master

1) Unir los datos de entrenamiento y las pruebas para crear un único set de datos.

<<<<<<< HEAD
1. Merges the training and the test sets to create one data set.
2. Extracts only the measurements on the mean and standard deviation for each measurement.
3. Uses descriptive activity names to name the activities in the data set
4. Appropriately labels the data set with descriptive activity names.
5. Creates a second, independent tidy data set with the average of each variable for each activity and each subject.

## How ```run_analysis.R``` implements the above steps:

* Require ```reshapre2``` and ```data.table``` librareis.
* Load both test and train data
* Load the features and activity labels.
* Extract the mean and standard deviation column names and data.
* Process the data. There are two parts processing test and train data respectively.
* Merge data set.
=======
2) Extraer solo las mediciones sobre la media y la desviación estándar para cada medida.

3) Usar nombres descriptivos para nombrar las actividades en el set de datos.

4) Etiquetar apropiadamente los datos con los nombres.

5) Crear un segundo tidy data set, con el promedio de cada variable para cada actividad y cada sujeto.

## Como run_analysis.R realiza los pasos descritos:

Requiere los paquetes reshapre2 y data.table.
Cargar los set de datos de pruebas y entrenamiento (test & train)
Cargar las etiquetas de características y actividades (features & activity)
Extraer la media y la desviación estándar de las columnas, nombres y datos.
Procesar los datos.
Unir los datos.
>>>>>>> origin/master
