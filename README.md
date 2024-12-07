# prueba_tecnica_lulo

### Descripción:

Este repositorio muestra cómo conectarse a la API de http://api.tvmaze.com para extraer lo datos de todo el mes de Enero 2024, luego se guardan los datos extraidos en un JSON, posteriormente se realizar un profiling con su respectivo análisis para asi tomar decisiones y realizar una limpieza de los datos de ser necesario. Despues los dataframes generados se guardan en archivos parquet con compresión snappy ya que tiene una alta velocidad en escritura y lectura de los datos. Por ultimo se leen los archivos parquet para que los datos puedan ser almacenados en una base de datos diseñada para el ejercicio y asi responder a unas preguntas usando operaciones de agregación. 

### Instalación:

1. Instalar Jupyter, Python y SQLite
2. Intalar las librerias a utilizar en python utilizando los siguientes comandos:
    !pip install requests
   
    !pip install json
   
    !pip install ydata-profiling
   
    !pip install fastparquet
   
    !pip install pandas
   
    !pip install numpy
   
    !pip instal sqlite3
   
    !pip install unittest

### Contenido:

1. data/ En esa carpeta encontrará los archivos parquet, de los dataframes utilizados.
2. db/ Aquí encontrará la base de datos en sqlite, ademas, de un script de las consultas utilizadas para responder a las preguntas usando operaciones de agregación.
3. json/ En esa carpeta encontrará los archivos JSON, cada uno de ellos contiene la información extraida de la APi por día.
4. profiling/ Encontrará los archivos HTML de los profiling generados, además un documento de texto (Análisis_profiling.docx) con el análisis de la información suministrada en el HTML
5. src/ Se almacenan los notebooks creados para el desarrollo del ejercicio.
6. model/ Contiene la imagen con el diagrama entidad-relación de la base de datos

### Ejecución:

1. Ejecutar el notebook prueba_tecnica.ipynb
2. Ejecutar el notebook read_parquet_sql.ipynb
3. Ejecutar el notebook pruebas_unitarias.ipynb


#### Desarrollado por: Laura Camila Rincón
