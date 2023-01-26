# Proyecto-Machine-Learning

El fin de este proyecto era predecir el precio de las propiedades en E.U si era low, medium y high.
Se hizo el preprocesamiento de datos y el análisis exploratorio de datos, y surgieron unas dudas acerca del dataset ya que habian valores
nulos en columnas importantes, como latitud y longitud y otras caracteristicas de las propiedades. Más alla de esto en las columnas price habian propiedades con un valor de 0$ para resolver este inconveniente se utilizó la imputación de estos valores con el método de los quartiles, aun asi quedaron algunos valores en 0$, entonces decidí eliminar dichas filas ya que no conocia la procedencia de estos datos y podrian afectar mi modelo.
También en la columna sqfeet habian outlier por ejemplo propiedades sin dimensiones donde las medidas eran de 0 metros cuadrados y aun asi tenian un precio, debido a esto se volvio a utilizar el metodo de imputación de los quartiles y estos valores se imputaron.
Se creo la columna Category_price que tenia en su contenido numeros binarios 0 para propiedades que no fuesen low y 1 para propiedades que fuesen low.
Finalmente se uso randomForest un modelo de machine learnig para la predicción, se creo un dataframe con los valores predichos y se guardo en un csv.

