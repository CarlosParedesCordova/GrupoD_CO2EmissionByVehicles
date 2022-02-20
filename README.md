# GrupoD_CO2EmissionByVehicles
# Integrantes
- Jimmy Jaramillo
- Carlos Paredes
- Alberto Ortega
- Jimmy Vicente
- Carlos Villavicencio
- Bryan Requenes

------------


# Dataset Seleccionado:
Emisiones de CO2 por vehículos

URL: https://www.kaggle.com/debajyotipodder/co2-emission-by-vehicles

## Detalles del Dataset
Este conjunto de datos captura los detalles de cómo las emisiones de CO2 de un vehículo pueden variar con las diferentes características. El conjunto de datos se tomó del sitio web oficial de datos abiertos del gobierno de Canadá. Esta es una versión compilada. Contiene datos sobre un período de 7 años. Hay un total de 7385 filas y 12 columnas. Hay pocas abreviaturas que se han utilizado para describir las características.

### Variables:
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

------------
# Requerimientos previos para la aplicación del Algoritmo
- Tener Instalado en el sistema operativo la aplicación "Weka".
- Archivos del Dataset para la aplicación del algoritmo y predicciones.
- Tener Instalado en el sistema operativo una hoja de cálculo denominada "Microsoft Excel".

# Video Explicativo
### 
https://www.youtube.com/watch?v=JNURdxkqoEM
### 
# Archivos Necesarios para la aplicación del Algoritmo
### 
Se encuentra en la carperta "CO2EmissionByVehiclesDataset"
### 


------------

#  Algoritmos Seleccionados
### 1. Decision Stump
Un Decision Stump (tronco de decisión) es un árbol de decisión que utiliza un solo atributo para la división en el caso de los atributos discretos, esto suele significar que el árbol sólo consta de un único nodo interior (es decir, la raíz sólo tiene hojas como nodos sucesores). Si el atributo es numérico, el árbol puede ser más complejo. Los nodos hoja de un árbol de decisión contienen el nombre de clase, mientras que un nodo que no es hoja es un nodo de decisión. El nodo de decisión es una prueba de atributo con cada rama (a otro árbol de decisión) siendo un valor posible del atributo. Este operador se puede aplicar tanto en conjuntos de datos nominales como numéricos. [2]

### 2. REPTree
Rep Tree es un algoritmo de aprendizaje que construye un árbol de decisión usando reducción de ganancia/varianza de la información v poda basada en la reducción del error. Debido a que este algoritmo se encuentra optimizado para ser rápido, ordena los valores numéricos sólo una vez. Los valores perdidos, se manejan dividiendo las instancias existentes en segmentos. Los parámetros que pueden ser establecidos son: número mínimo de instancias en cada hoja, la profundidad máxima del árbol y la cantidad de datos usada para la poda. [3]
### 3. Hoeffding Tree
El algoritmo del árbol de Hoeffding es un método de aprendizaje del árbol de decisión para la clasificación de datos de flujo porque es capaz de aprender de flujos de datos masivos. Los árboles de Hoeffding aprovechan el hecho de que una pequeña muestra a menudo puede ser suficiente para elegir un atributo de división óptimo. [4]
#### Características
- A diferencia de árboles de decisiones incrementales es que tiene sólidas garantías de rendimiento,
- El algoritmo toma como entrada una secuencia de ejemplos de entrenamiento, S, descrita por los atributos A, y el parámetro de precisión.
- Las únicas estadísticas que deben mantenerse en el algoritmo del árbol de Hoeffding son los recuentos n ijk para el valor v j del atributo A i con etiqueta de clase y k.

### 4. J48
La clasificación es el proceso de construir un modelo de clases a partir de un conjunto de registros que contienen etiquetas de clase. El algoritmo de árbol de decisión sirve para averiguar el comportamiento del vector de atributos para una serie de instancias. También sobre la base de las instancias de entrenamiento se encuentran las clases para las instancias recién generadas. Las características adicionales de J48 son la contabilización de los valores perdidos, la poda de los árboles de decisión, los rangos de valores de atributos continuos, la derivación de reglas. [5]
### 5. Random tree
Toman datos aleatorios del set de datos principal para crear N árboles de decisión a partir de muestras de datos seleccionadas al azar, con el fin de obtener predicciones de cada árbol para luego seleccionar la mejor, su filosofía se basa en muchos es mejor que uno. Los árboles son entrenados de forma ligeramente diferente y se fusionan para obtener predicciones más precisas y estables. Cada árbol generado por el algoritmo contiene un grupo de observaciones aleatorias elegidas mediante bootstrap, que es una técnica estadística para obtener muestras de una población donde una observación se puede considerar en más de una muestra. Las observaciones no estimadas en los árboles (también conocidas como “out of the bag”) se utilizan para validar el modelo. Las salidas de todos los árboles se combinan en una salida final Y (conocida como ensamblado) que se obtiene mediante alguna regla (generalmente el promedio, cuando las salidas de los árboles del ensamblado son numéricas y, conteo de votos, cuando las salidas de los árboles del ensamblado son categóricas).[6]
###
# Herramienta: Weka
![image](https://i0.wp.com/buconda.com/wp-content/uploads/2019/06/weka2.png?fit=262%2C132&ssl=1)

Weka es una colección de algoritmos de aprendizaje automático para tareas de minería de datos. Contiene herramientas para la preparación de datos, clasificación, regresión, agrupación, minería de reglas de asociación y visualización. Weka es un software de código abierto publicado bajo la Licencia Pública General de GNU. [1]
------------
# Tabla Comparativa entre los Algoritmos de Clasificación por Clase de Vehículo
![image](https://user-images.githubusercontent.com/46327676/153418207-6feca732-93d6-4387-9480-21b8865e401e.png)
------------
# Pasos a seguir para la aplicación del Algoritmo
#### 1. Se ingresa a Explorer donde permite el acceso a la mayoría de las funcionalidades integradas en Weka de una manera sencilla.
![image](https://user-images.githubusercontent.com/46327676/153769648-93a2a24f-74ab-4dd4-b490-2a22579d3ab9.png)
#### 2.Lo primero que vamos hacer es cargar los datos en el área de trabajo, para ello selccionamos la opción "Open File"
![image](https://user-images.githubusercontent.com/46327676/153769697-36074706-fa17-41d7-a473-88a21ddee4a5.png)
#### 3. Seleccionamos formato del archivo dataset en este ejemplo el formato es ".CSV"
#### 4. Se procede a selecionar el archivo detaset y se lo abre
![image](https://user-images.githubusercontent.com/46327676/153769784-63e6724d-938d-4670-b540-a94a0651836a.png)
#### 5. Se ingresa al area "Classify" 
#### 6. Seleccionamos la clase que vamos aplicar en el algoritmo "Vehicle Class"
#### 7. Elección del clasificador
![image](https://user-images.githubusercontent.com/46327676/153769854-6b929fe8-6dbf-45b7-bb7a-6bac080149b5.png)
#### 8. Seleccionamos la carpeta "trees" con el fin de seleccionar el algoritmo elegido una vez realizado la tabala comparativa.
#### 9. El algoritmo para la aplicación es el "J48"
![image](https://user-images.githubusercontent.com/46327676/153769941-a482ac47-e09d-4a5d-b86f-df13a1f1acf0.png)
#### 10. En las opciones para realizar el test seleccionamos la opción "Cross-validation" donde se  calcula el porcentaje de aciertos esperado haciendo una validación cruzada de k hojas (podemos seleccionar el k,que por omisión es de 10).
![image](https://user-images.githubusercontent.com/46327676/153785800-292cb7fd-fcec-4d40-8017-c896e465b9a7.png)
#### 11. Seleccionamos la opción "Start" para ejecutar 
#### 12. Una vez realizado el test podemos observar el porcentaje de aciertos en este caso constamos con un 90.9276%
#### 13. Se puede observar el porcentaje de aciertos desglosados por clase
![image](https://user-images.githubusercontent.com/46327676/153786575-a5c088da-454a-487c-8de6-61633187e27e.png)
#### 14. Pulsando el botón contrario del ratón se desplegara la siguiente ventana emergente 
#### 15. Pulsa sobre la opción visualizar Árbol de Decisión
![image](https://user-images.githubusercontent.com/46327676/153788492-2a582f0b-710f-42b3-952e-a6ae255c1a96.png)
![image](https://user-images.githubusercontent.com/46327676/153787882-8b9507d4-ba33-49c7-bff3-7aa6f0653cd4.png)
#### 16. Esta opción permite visualizar los error clasificados
![image](https://user-images.githubusercontent.com/46327676/153788559-e37fd189-00b8-4586-ba8e-b2021aa8f988.png)
![image](https://user-images.githubusercontent.com/46327676/153787993-a8195192-ab1f-4a75-a33c-9be96e4b7766.png)
## Predicciones con Nuevos Datos
#### 17. Seleccionamos Supplied test set "Set.." este apartado los atributos de los datos son escritos en un nuevo archivo de formato .CSV sobre el cual se efectuara la clasificación
![image](https://user-images.githubusercontent.com/46327676/153789466-1e8d21fe-7ee2-4955-b28c-1c7d1651be04.png)
#### 18. Abrimos el archivo
#### 19. Seleccionamos el archivo con nuevos datos(para realizar una predicción con el archivo que se va aplicar se debera hacer cambios en el campo que va ha desear predecir en  este caso es "Vehicle Class" como se puede observar en la siguiente imagen se deber cambiar el valor del campo seleccionado por un "?" con el fin de que la herramienta haga su predicción una vez ya aplicado el algoritmo del dataset
![image](https://user-images.githubusercontent.com/46327676/153908193-90cceb09-0f71-4d42-94bb-eaa1c957589c.png)
#### 20. Se abre el arhcivo 
![image](https://user-images.githubusercontent.com/46327676/153790035-3ecd9c92-03ac-46e6-a7b0-efbbddebec7d.png)
#### 21. Seleccionamos la clase en este caso "Vehicle Class"
#### 22. Se puede observa la cantidad de atributos que posee en dataset en este caso son 12.
![image](https://user-images.githubusercontent.com/46327676/153790438-7fed3faf-8121-49cf-afa0-2dd9d23463a2.png)
#### 23. Entramos a More options..
#### 24. Se abre una pantalla emergente donde se mostrara varias opciones de clasificacion, vamos a la de predicciones en el apartado "Choose" seleccionamos el tipo formato del archivo con nuevos datos para poder observar las predicciones que se realizaran, para mejor visualización se selecciono plaintext
![image](https://user-images.githubusercontent.com/46327676/153907656-def7332a-7874-4b36-8baf-2e6b6a1317c9.png)
#### 25. Una vez ya aplicado el algoritmo J48 de todo el dataset se puede realizar la predicción con un nuevo conjunto de datos como se puede observar la predicción de estos datos
![image](https://user-images.githubusercontent.com/46327676/153909124-f38549ea-dd5b-4209-a685-e8a2c61d91c1.png)
------------
# Conclusión
- Existen diferentes metodos para realizar clasificacion de datos, y algoritmos dentro de los mismos, por lo cual unos pueden funcionar mejor en ciertos casos que otros logrando una mayor eficiencia, por lo cual es importante selecionar el adecuado acorde a la tarea que necesitemos realizar, para este dataset en especifico se realizo mediante arboles de descicion que fueron generados mediante el algoritmo J48, para lo cual haciendo uso de los datos acerca de los vehiculos como peso, transmicion, consumo y demas, nos permite predecir con un 90% de precision que tipo de vehiculo es.
------------

#  Bibliografia

- [1] “Weka 3 - data mining with open source machine learning software in java”, Waikato.ac.nz. [En línea]. Disponible en: https://www.cs.waikato.ac.nz/ml/weka/. [Consultado: 18-feb-2022].
- [2] RapidMiner GmbH, “Decision stump - RapidMiner documentation”, Rapidminer.com. [En línea]. Disponible en: https://docs.rapidminer.com/latest/studio/operators/modeling/predictive/trees/decision_stump.html. [Consultado: 08-feb-2022].
- [3] Bae, B. P. (2015). Using machine learning algorithms for housing price prediction: The case of Fairfax County, Virginia housing data. Expert Syst. Appl, 42(6), 2928–2934.
- [4] “What is Hoeffding Tree Algorithm?”, Tutorialspoint.com. [En línea]. Disponible en: https://www.tutorialspoint.com/what-is-hoeffding-tree-algorithm. [Consultado: 18-feb-2022].
- [5] IHYA, R. y Namir, A. (2019). J48 Algorithms of machine learning for predicting user's the acceptance of an E-orientation Systems.
- [6] RapidMiner GmbH, “Random tree - RapidMiner documentation”, Rapidminer.com. [En línea]. Disponible en: https://docs.rapidminer.com/latest/studio/operators/modeling/predictive/trees/random_tree.html. [Consultado: 18-feb-2022].
