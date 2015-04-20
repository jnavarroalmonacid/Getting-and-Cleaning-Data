# Getting-and-Cleaning-Data

## Proyecto del Curso

Crear un Script de R, llamado run_analysis.R, que haga lo siguiente.

1) Unir los datos de entrenamiento y las pruebas para crear un único set de datos.

2) Extraer solo las mediciones sobre la media y la desviación estándar para cada medida.

3) Usar nombres descriptivos para nombrar las actividades en el set de datos.

4) Etiquetar apropiadamente los datos con los nombres.

5) Crear un segundo tidy data set, con el promedio de cada variable para cada actividad y cada sujeto.

## Pasos a seguir para el desarrollo

1. Descargar la fuente de los datos y almacenarlo en una carpeta en tu disco duro local. Obtendrás una carpeta llamada ```UCI HAR Dataset```.
2. Pon ```run_analysis.R``` en la carpeta ```UCI HAR Dataset```, luego configúrala como working directory usando ```setwd()```.
3. ejecuta ```source("run_analysis.R")```, y se generará  ```tiny_data.txt``` en el working directory.

## Dependencias

```run_analysis.R``` te ayudará a instalar las dependencias automáticamente:  ```reshape2``` y ```data.table```. 
