#                                         PROYECTO II DATA SCIENCE - DATATHON

![image](https://user-images.githubusercontent.com/93155829/199801185-4a4ffb2c-af31-491a-9475-d7a23787832e.png)

Hola! Bienvenidos al README que contiene una descripcion del proyecto realizado. 

# Consigna

El objetivo que teniamos que cumplir con este proyecto es, dado un conjunto de Datasets con informacion sobre propiedades en venta en Colombia, armar con diferentes algoritmos de Machine Learning, un modelo de clasificación que permita clasificar el precio de las propiedades en venta. Para esto, específicamente, debe predecir la categorización de las propiedades entre baratas o caras, considerando como criterio el valor promedio de los precios (la media).Antes de armar nuestro modelo de machine learning, tambien fue necesario un preprocesamiento de los datos.

Veamos a continuacion mas en detalle todo lo mencionado anteriormente. 

# Tratamiento de los datos

![image](https://user-images.githubusercontent.com/93155829/199806440-ae8edce0-2eb2-4f9c-b954-7c9792522b97.png)

Las herramientas usadas fueron Python (librerias como Pandas, numpy, skelearn, matplotlib, seaborn, geopandas, folium), Jupyter notebooks, etc. 
Con estas, fueron ingestados a nuestro sistemas los dos archivos .csv dados por el equipo de soyHenry (uno para el testeo, y otro para el entrenamiento). 

El preprocesamiento es uno de los estadios más importantes en el flujo de trabajo de un data scientist. Suele demandar, en promedio, entre el 60% y 70% de nuestro tiempo. La distinción entre un buen y un mal modelo de Machine Learning, antes que por la elección de un algoritmo específico, estará dada por un correcto preprocesamiento de datos.

Si queremos un modelo predictivo de calidad, debemos darle datos de calidad. Podemos elegir el algoritmo más sofisticado y complejo, optimizar los hiperparámetros tratando de encontrar las mejores combinaciones posibles, pero si al modelo lo alimentamos con datos que carecen de sentido, no podemos esperar que sus predicciones sí lo tengan.

El preprocesamiento de los datos tiene diferentes etapas que mas adelante veremos en detalle. Sin embargo, una instacia 'Cero' podriamos decirle es explorar el dataset. Esto quiere decir, analizar los datos, ver los tipos de datos, sacar medidas, ver objetivos, hacer graficos, etc.

  1. Tratamiento de valores nulos:
  
  En esta etapa utilizamos una funcion que nos mostraba el porcentaje de valores nulos por columna. Frente a esto encontramos que muchas columnas contenian registros nulos como otros no.(Las decisiones concretas estan perfectamente explicadas en el archivo llamado preprocesamiento_data.ipynb)
  En esta etapa, se tommaron dos decisiones fundamentales: La eliminacion de los datos con problemas (ya sean filas o columnas) y la imputacion de valores puntuales en los campos faltantes. 
  
  2. Valores atipicos:
  
  También denominados outliers o valores extremos. Son aquellos datos que difieren significativamente del resto de las observaciones. Para detectarlos se utilizaron diferentes graficos sobre las columnas, y alli se pueden visualizar diferentes anomalias. Nuevamente, cada decision esta fundamentada en el Jupyter Notebook. 
  
  3. Escalado/Normalizacion:
  
  Es probable que, en nuestro dataset, contemos con distintas variables, medidas en diferentes unidades y con distintas escalas. Esto puede confundir a los modelos de ML, ya que no entienden de unidades. Ante esta situacion, se trato de normalizar y aplicar tecnicas de procesamiento de lenguaje natural sobre las columnas de tipo string. 
  
  4. Codificacion de variables categoricas. 

  Como sabemos, los modelos de Machine Learning solo entienden de números. Para ello, debemos transformar nuestros atributos del dataset que contenga     datos cualitativos en cuantitativos. En nuestro dataset, encontramos una columna sobre la que se hizo esta etapa. Para esta etapa, se utilizo el algoritmo de machine learning llamado OneHotEncoder. 
  

# ARMADO DEL MODELO

![image](https://user-images.githubusercontent.com/93155829/199995508-322b9e23-4bdb-426c-9b49-d521638c9a30.png)

Para nuestro modelo hemos elegido un algoritmo de clasificacion: Arboles de decision. Con todos los pasos que son necesarios para el armado de nuestro modelo hemos se ha llegado a lo que se queria: un archivo .csv con una sola columna llamada pred, que contenga justamente las predicciones. Ademas de esto, podemos ver algunas metricas obtenidas para ver si nuestra prediccion fue buena o no. 

# CONCLUSION

El machine learning es una de las tecnologías de la inteligencia artificial más poderosas de todos los tiempos. Esto se debe principalmente a sus potentes capacidades de predicción y planificación que aporta el también llamado aprendizaje automático. Tiene su base en un proceso de enseñanza-aprendizaje, que consiste en suministrarle a la computadora grandes volúmenes de datos para que esta aprenda de forma automática alguna tarea u oficio determinado, por ello el machine learning se relaciona con el análisis big data y el data science.








