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

    La clasificación es el proceso de construir un modelo de clases a partir de un conjunto de registros que contienen etiquetas de clase. El algoritmo de árbol de decisión         sirve   para averiguar el comportamiento del vector de atributos para una serie de instancias. También sobre la base de las instancias de entrenamiento se encuentran las         clases para las instancias recién generadas. Las características adicionales de J48 son la contabilización de los valores perdidos, la poda de los árboles de decisión,           los rangos de valores de atributos continuos, la derivación de reglas. [1]

5. RandomTree

    Toman datos aleatorios del set de datos principal para crear N árboles de decisión a partir de muestras de datos seleccionadas al azar, con el fin de obtener predicciones de     cada árbol para luego seleccionar la mejor, su filosofía se basa en muchos es mejor que uno. Los árboles son entrenados de forma ligeramente diferente y se fusionan para         obtener predicciones más precisas y estables.
    Cada árbol generado por el algoritmo contiene un grupo de observaciones aleatorias elegidas mediante bootstrap, que es una técnica estadística para obtener muestras de una       población donde una observación se puede considerar en más de una muestra. Las observaciones no estimadas en los árboles (también conocidas como “out of the bag”) se             utilizan para validar el modelo. Las salidas de todos los árboles se combinan en una salida final Y (conocida como ensamblado) que se obtiene mediante alguna regla               (generalmente el promedio, cuando las salidas de los árboles del ensamblado son numéricas y, conteo de votos, cuando las salidas de los árboles del ensamblado son               categóricas).


# Tabla Comparativa entre los Algoritmos de Clasificación por Clase de Vehículo

![image](https://user-images.githubusercontent.com/46327676/153418207-6feca732-93d6-4387-9480-21b8865e401e.png)


# Pasos a seguir para la aplicación del Algoritmo

1. Se ingresa a Explorer donde permite el acceso a la mayoría de las funcionalidades integradas en Weka de una manera sencilla.
###
![image](https://user-images.githubusercontent.com/46327676/153769648-93a2a24f-74ab-4dd4-b490-2a22579d3ab9.png)
###
2.Lo primero que vamos hacer es cargar los datos en el área de trabajo, para ello selccionamos la opción "Open File"
###
![image](https://user-images.githubusercontent.com/46327676/153769697-36074706-fa17-41d7-a473-88a21ddee4a5.png)
###
3. Seleccionamos formato del archivo dataset en este ejemplo el formato es ".CSV"
###
4. Se procede a selecionar el archivo detaset y se lo abre
###
![image](https://user-images.githubusercontent.com/46327676/153769784-63e6724d-938d-4670-b540-a94a0651836a.png)
###
5.Se ingresa al area "Classify" 
###
6.Seleccionamos la clase que vamos aplicar en el algoritmo "Vehicle Class"
###
7.Elección del clasificador
###
![image](https://user-images.githubusercontent.com/46327676/153769854-6b929fe8-6dbf-45b7-bb7a-6bac080149b5.png)
###
8.Seleccionamos la carpeta "trees" con el fin de seleccionar el algoritmo elegido una vez realizado la tabala comparativa.
###
9.El algoritmo para la aplicación es el "J48"
###
![image](https://user-images.githubusercontent.com/46327676/153769941-a482ac47-e09d-4a5d-b86f-df13a1f1acf0.png)
###
10.En las opciones para realizar el test seleccionamos la opción "Cross-validation" donde se  calcula el porcentaje de aciertos esperado
haciendo una validación cruzada de k hojas (podemos seleccionar el k,que por omisión es de 10)
###
![image](https://user-images.githubusercontent.com/46327676/153785800-292cb7fd-fcec-4d40-8017-c896e465b9a7.png)
###
11.Seleccionamos la opción "Start" para ejecutar 
12.Una vez realizado el test podemos observar el porcentaje de aciertos en este caso constamos con un 90.9276%
13.Se puede observar el porcentaje de aciertos desglosados por clase
![image](https://user-images.githubusercontent.com/46327676/153786575-a5c088da-454a-487c-8de6-61633187e27e.png)
