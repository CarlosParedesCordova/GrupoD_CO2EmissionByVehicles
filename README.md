# GrupoD_CO2EmissionByVehicles
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
5. RandomTree

Toman datos aleatorios del set de datos principal para crear N árboles de decisión a partir de muestras de datos seleccionadas al azar, con el fin de obtener predicciones de cada árbol para luego seleccionar la mejor, su filosofía se basa en muchos es mejor que uno. Los árboles son entrenados de forma ligeramente diferente y se fusionan para obtener predicciones más precisas y estables.
Cada árbol generado por el algoritmo contiene un grupo de observaciones aleatorias elegidas mediante bootstrap, que es una técnica estadística para obtener muestras de una población donde una observación se puede considerar en más de una muestra. Las observaciones no estimadas en los árboles (también conocidas como “out of the bag”) se utilizan para validar el modelo. Las salidas de todos los árboles se combinan en una salida final Y (conocida como ensamblado) que se obtiene mediante alguna regla (generalmente el promedio, cuando las salidas de los árboles del ensamblado son numéricas y, conteo de votos, cuando las salidas de los árboles del ensamblado son categóricas).


Tabla Comparativa entre los Algoritmos de Clasificación por Clase de Vehículo

![image](https://user-images.githubusercontent.com/46327676/153418207-6feca732-93d6-4387-9480-21b8865e401e.png)
