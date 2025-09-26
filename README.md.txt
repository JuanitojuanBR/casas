Conteste las siguientes preguntas:

 Aprendizaje Supervisado
1.	¿Por qué es importante contar con una variable target en un problema de aprendizaje supervisado?
R:/ La variable target proporciona las “etiquetas” con las que el modelo aprende.
- Define la función de pérdida a optimizar (qué significa acertar o errar).
- Permite evaluar el desempeño (ej. R², MAE, MSE) comparando predicción vs. realidad.
- Sin target, el algoritmo no puede ajustar parámetros para predecir un valor específico.
2.	¿Qué representa el valor de la pendiente y la intersección en el modelo de regresión lineal aplicado al precio de casas?
R:/
- Intersección (b₀): precio base estimado cuando las variables predictoras son 0.
- Pendiente (b₁ en univariado; coeficientes en multivariado): cambio esperado en el precio por cada unidad adicional de la característica (ej. $/m² o por habitación), manteniendo las demás constantes.

3.	¿Cómo influye la calidad de los datos (valores atípicos, faltantes, ruido) en las predicciones de un modelo supervisado?
R:/
- Atípicos: distorsionan coeficientes y métricas, generando sesgos.
- Faltantes: reducen información o inducen sesgos si se imputan mal.
- Ruido: incrementa la varianza del modelo y empeora la generalización.
- Escalado/errores de captura: producen inestabilidad y peores predicciones.

4.	Si el modelo no predice correctamente, ¿qué técnicas podríamos aplicar para mejorar su desempeño?
R:/
- Mejorar datos: limpiar outliers, imputar faltantes, añadir variables relevantes (ubicación, antigüedad, estado, etc.).
- Ingeniería de características: transformaciones (log), interacciones, polinomios.
- Regularización/algoritmos: Ridge/Lasso/ElasticNet o modelos no lineales (árboles, Random Forest, Gradient Boosting).
- Validación: k-fold CV, ajuste de hiperparámetros y evaluación robusta.

5.	¿Qué ventajas y limitaciones observas en el uso de la regresión lineal para problemas del mundo real?
R:/
- Ventajas: simple, interpretable, rápida, buen baseline, fácil de desplegar.
- Limitaciones: asume linealidad y errores homocedásticos; sensible a outliers y multicolinealidad; puede subajustar relaciones complejas/no lineales.

Aprendizaje No Supervisado

1.	¿En qué se diferencia el proceso de clustering (KMeans) del de regresión lineal?
R:/ KMeans agrupa datos sin etiquetas minimizando la variación intra‑cluster; la regresión lineal predice una variable continua utilizando ejemplos etiquetados (target) y ajusta coeficientes para minimizar error de predicción.

2.	¿Por qué no necesitamos una variable target en el aprendizaje no supervisado?
R:/ Porque el objetivo es descubrir estructuras o patrones latentes en los datos (grupos, asociaciones) sin una verdad de referencia. Los algoritmos se guían por medidas internas (distancias/similitud), no por etiquetas externas.

3.	¿Qué significado tienen los centroides en KMeans?
R:/ Son los puntos medios de cada cluster en el espacio de características (promedios). Representan el “perfil típico” del grupo y sirven para asignar nuevas observaciones al cluster más cercano.

4.	¿Cómo podríamos interpretar los grupos generados en el análisis de segmentación de casas?
R:/ Por rangos de mercado basados en tamaño/precio:
- Cluster económico: menor área y menor precio.
- Cluster medio: área y precio intermedios.
- Cluster premium: mayor área y mayor precio.
Se recomienda revisar centroides y estadísticas por cluster para perfilar cada segmento.

5.	¿Qué beneficios tendría aplicar técnicas no supervisadas en una empresa que quiere conocer mejor a sus clientes?
R:/
- Segmentación para marketing y ofertas personalizadas.
- Mejora de pricing, cross‑sell/upsell y recomendadores.
- Detección de nichos y oportunidades; reducción de churn.
- Identificación de anomalías/comportamientos inusuales.
