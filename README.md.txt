Aprendizaje Supervisado

1. ¿Por qué es importante contar con una variable target en un problema de aprendizaje supervisado?
R:/ Porque el aprendizaje supervisado se basa en aprender una relación entre las variables independientes (características como área, habitaciones, ubicación) y una variable dependiente o target (precio). Sin el target no podemos entrenar el modelo, ya que no tendría un valor de referencia para comparar y ajustar sus predicciones.

2. ¿Qué representa el valor de la pendiente y la intersección en el modelo de regresión lineal aplicado al precio de casas?
R:/

La pendiente representa cuánto cambia el precio de la casa cuando una variable (ejemplo: área) aumenta en una unidad, manteniendo las demás constantes.

La intersección indica el valor del precio estimado cuando todas las variables independientes son cero (aunque en la práctica este valor no siempre tiene interpretación realista en bienes raíces).

3. ¿Cómo influye la calidad de los datos (valores atípicos, faltantes, ruido) en las predicciones de un modelo supervisado?
R:/ Los datos de baja calidad afectan fuertemente al modelo:

Valores atípicos distorsionan la pendiente o las relaciones aprendidas.

Datos faltantes reducen la información disponible y pueden sesgar el entrenamiento.

Ruido introduce variabilidad innecesaria, disminuyendo la capacidad del modelo de generalizar.

En los gráficos se observa que algunos precios son exageradamente altos en relación al área, lo que probablemente sean atípicos que afectan la predicción.

4. Si el modelo no predice correctamente, ¿qué técnicas podríamos aplicar para mejorar su desempeño?
R:/

Limpiar y normalizar los datos (eliminar outliers, imputar valores faltantes).

Probar modelos más complejos (Random Forest, XGBoost, Redes Neuronales).

Ajustar hiperparámetros con técnicas como GridSearch o RandomSearch.

Aplicar selección o ingeniería de características (por ejemplo, incluir ubicación, estrato, año de construcción).

Realizar cross-validation para validar robustez.

5. ¿Qué ventajas y limitaciones observas en el uso de la regresión lineal para problemas del mundo real?
R:/
Ventajas:

Fácil de interpretar.

Rápido de entrenar incluso con muchos datos.

Útil para identificar relaciones lineales claras.

Limitaciones:

No captura relaciones no lineales (ejemplo: precio vs área puede no crecer de forma lineal).

Muy sensible a outliers.

Supone independencia y homocedasticidad que no siempre se cumplen en datos reales.

Aprendizaje No Supervisado

1. ¿En qué se diferencia el proceso de clustering (KMeans) del de regresión lineal?
R:/

Regresión lineal busca predecir un valor numérico (target) a partir de variables.

Clustering (KMeans) agrupa observaciones similares en clústeres sin necesidad de un valor objetivo.

2. ¿Por qué no necesitamos una variable target en el aprendizaje no supervisado?
R:/ Porque el objetivo es descubrir patrones ocultos o estructuras en los datos (segmentos, grupos, tendencias) sin que haya una etiqueta que guíe el proceso.

3. ¿Qué significado tienen los centroides en KMeans?
R:/ Cada centroide representa el “punto medio” del clúster, es decir, el perfil promedio de los elementos de ese grupo. En el gráfico de segmentación, los centroides indican los valores promedio de área y precio de cada segmento de viviendas.

4. ¿Cómo podríamos interpretar los grupos generados en el análisis de segmentación de casas?
R:/

Clúster verde (izquierda abajo): Viviendas de bajo costo y menor área.

Clúster rojo (medio): Viviendas de precio y área intermedia.

Clúster azul (arriba): Viviendas más grandes y costosas.

Esto permite categorizar el mercado inmobiliario en segmentos económicos diferenciados.

5. ¿Qué beneficios tendría aplicar técnicas no supervisadas en una empresa que quiere conocer mejor a sus clientes?
R:/

Permite segmentar clientes en grupos homogéneos (ej. clientes premium, regulares, ocasionales).

Ayuda a diseñar estrategias de marketing personalizadas.

Mejora la fidelización al entender las necesidades de cada segmento.

Permite detectar patrones ocultos de consumo y oportunidades de negocio.

