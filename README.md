﻿# GrupoD_CO2EmissionByVehicles
# Integrantes
- Jimmy Jaramillo
- Carlos Paredes
- Alberto Ortega
- Jimmy Vicente
- Carlos Villavicencio
- Bryan Requenes

# Dataset Seleccionado:
Emisiones de CO2 por vehículos
Link: https://www.kaggle.com/debajyotipodder/co2-emission-by-vehicles

# Herramienta: Weka

Este conjunto de datos captura los detalles de cómo las emisiones de CO2 de un vehículo pueden variar con las diferentes características. El conjunto de datos se tomó del sitio web oficial de datos abiertos del gobierno de Canadá. Esta es una versión compilada. Contiene datos sobre un período de 7 años. Hay un total de 7385 filas y 12 columnas. Hay pocas abreviaturas que se han utilizado para describir las características.

# Variables:
- Compañia del Vehiculo 
- Modelo de Carro
- Clase de vehículo según su utilidad, capacidad y peso
- Tamaño del motor utilizado en litros
- Número de cilindros
- Tipo de transmisión con número de marchas
- Tipo de combustible utilizado
- Consumo de combustible en vías urbanas (L/100 km)
- Consumo de combustible en carreteras (L/100 km)
- El consumo combinado de combustible (55% ciudad, 45% carretera) se muestra en L/100 km

#  Algoritmos Seleccionados
1. Decision Stump
2. REPTree
3. Hoeffding Tree
  
    El algoritmo del árbol de Hoeffding es un método de aprendizaje del árbol de
    decisión para la clasificación de datos de flujo porque es capaz de aprender de
    flujos de datos masivos. Los árboles de Hoeffding aprovechan el hecho de que
    una pequeña muestra a menudo puede ser suficiente para elegir un atributo de
    división óptimo [4].
    
    Características

    - A diferencia de árboles de decisiones incrementales es que tiene sólidas
    garantías de rendimiento,
    - El algoritmo toma como entrada una secuencia de ejemplos de
    entrenamiento, S, descrita por los atributos A, y el parámetro de
    precisión.
    - Las únicas estadísticas que deben mantenerse en el algoritmo del árbol
    de Hoeffding son los recuentos n ijk para el valor v j del atributo A i con
    etiqueta de clase y k. 
  
4. J48

    La clasificación es el proceso de construir un modelo de clases a partir de un conjunto de registros que contienen etiquetas de clase. El algoritmo de árbol de decisión         sirve   para averiguar el comportamiento del vector de atributos para una serie de instancias. También sobre la base de las instancias de entrenamiento se encuentran las         clases para las instancias recién generadas. Las características adicionales de J48 son la contabilización de los valores perdidos, la poda de los árboles de decisión,           los rangos de valores de atributos continuos, la derivación de reglas. [1]

5. RandomTree

    Toman datos aleatorios del set de datos principal para crear N árboles de decisión a partir de muestras de datos seleccionadas al azar, con el fin de obtener predicciones de     cada árbol para luego seleccionar la mejor, su filosofía se basa en muchos es mejor que uno. Los árboles son entrenados de forma ligeramente diferente y se fusionan para         obtener predicciones más precisas y estables.
    Cada árbol generado por el algoritmo contiene un grupo de observaciones aleatorias elegidas mediante bootstrap, que es una técnica estadística para obtener muestras de una       población donde una observación se puede considerar en más de una muestra. Las observaciones no estimadas en los árboles (también conocidas como “out of the bag”) se             utilizan para validar el modelo. Las salidas de todos los árboles se combinan en una salida final Y (conocida como ensamblado) que se obtiene mediante alguna regla               (generalmente el promedio, cuando las salidas de los árboles del ensamblado son numéricas y, conteo de votos, cuando las salidas de los árboles del ensamblado son               categóricas).


# Tabla Comparativa entre los Algoritmos de Clasificación por Clase de Vehículo

![image](https://user-images.githubusercontent.com/46327676/153418207-6feca732-93d6-4387-9480-21b8865e401e.png)


# Pasos
![image](https://user-images.githubusercontent.com/46327676/153757719-cdc7928f-696b-46d7-91dc-241b2dd9a316.png)
![image](https://user-images.githubusercontent.com/46327676/153757836-093b9b34-1721-4478-8e8a-eb0849b4a22f.png)
![image](https://user-images.githubusercontent.com/46327676/153757909-22be296a-5b17-4bc6-8aed-a69ee6f382d6.png)
![image](https://user-images.githubusercontent.com/46327676/153757955-f42a8b03-c0ca-455c-9310-6735c66e2a78.png)
![image](https://user-images.githubusercontent.com/46327676/153758184-54ff54a5-7644-4e55-8f60-b9d76881c96f.png)
![image](https://user-images.githubusercontent.com/46327676/153758247-bcd94d5b-e843-4d2b-8e4f-544106cb025c.png)




