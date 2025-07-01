# Fuga_Clientes_Prediccion_F1

🧭 1. Definición del problema
Objetivo: Predecir si un cliente abandonará el banco próximamente.

Tipo de problema: Clasificación binaria.

Métricas clave: F1-score (mínimo 0.59) y AUC-ROC.

📥 2. Carga y preparación de datos
Tareas:

Cargar el dataset (pandas).

Verificar tipos de datos, valores nulos y duplicados.

Codificar variables categóricas si es necesario.

Escalar variables numéricas si el modelo lo requiere.

Herramientas: pandas, numpy, scikit-learn.

⚖️ 3. Análisis del equilibrio de clases
Tareas:

Calcular proporción de clases (clientes que abandonan vs. no).

Visualizar con gráficos de barras o pastel.

Entrenar un modelo base (por ejemplo, LogisticRegression) sin tratar el desequilibrio.

Evaluar F1 y AUC-ROC.

Objetivo: Establecer una línea base para comparar mejoras posteriores.

🧠 4. Mejora del modelo y tratamiento del desequilibrio
Tareas:

Aplicar al menos dos técnicas:

Submuestreo de la clase mayoritaria.

Sobremuestreo con SMOTE o RandomOverSampler.

Probar diferentes modelos:

RandomForestClassifier

XGBoostClassifier

LogisticRegression con class_weight='balanced'

Usar validación cruzada o división entrenamiento/validación (por ejemplo, 80/20).

Ajustar hiperparámetros con GridSearchCV o RandomizedSearchCV.

Métricas de evaluación: F1-score, AUC-ROC, matriz de confusión.

🧪 5. Prueba final
Tareas:

Evaluar el mejor modelo en el conjunto de prueba.

Reportar F1 y AUC-ROC.

Comparar con el modelo base.

Interpretar resultados: ¿qué variables influyen más en la predicción?
