## Aplicación de Ciencia y Analítica de Datos con Python

## Título del Proyecto:Análisis Predictivo de un Conjunto de Datos de jugadores de Basketball
Los participantes del curso llevarán a cabo un proyecto de ciencia y analítica de datos utilizando Python. El objetivo es aplicar los conceptos teóricos y prácticos aprendidos durante el curso, desde la manipulación de datos con NumPy y Pandas, hasta la creación de visualizaciones, el desarrollo de modelos predictivos básicos, y su posterior evaluación y despliegue.

## Objetivo del Proyecto:
El proyecto final tiene como objetivo que los participantes seleccionen un conjunto de datos propios o de interés, realicen un análisis exploratorio, construyan un modelo predictivo y desarrollen visualizaciones para comunicar los resultados. Los datos pueden ser de áreas como:

Los participantes deberán crear una solución analítica que responda a una pregunta específica o problema utilizando las herramientas de análisis utilizadas, de manera indivual o en equipo de máximo 4 integrantes, pero TODOS deben entregar. 

## Entregables del Proyecto:
Cada equipo o participante debe entregar los siguientes elementos:

## Descripción del problema o pregunta:

**¿Qué intentas predecir, analizar o investigar con los datos seleccionados?**

Describe el contexto del conjunto de datos y por qué es relevante para el análisis.
Análisis Exploratorio de Datos (EDA):

Realiza un análisis inicial para comprender la estructura de los datos. Identifica valores faltantes, distribuciones y patrones.
Crea visualizaciones (gráficos de barras, histogramas, gráficos de dispersión) que ayuden a visualizar los datos y su distribución.
Preparación de los Datos:

Limpiar los datos: Manejar valores faltantes, duplicados o incorrectos.
Normalizar o escalar los datos si es necesario.
Convertir variables categóricas en variables numéricas (si aplica).
Modelado Predictivo:

Construir un modelo predictivo utilizando Scikit-learn. Ejemplos de modelos que pueden utilizar:
Regresión lineal para predicción de valores continuos.
Clasificación (Regresión logística, KNN) si la variable objetivo es categórica.
Explicar brevemente la elección del modelo.
Evaluación del Modelo:

Utilizar métricas como Precisión, Recall, F1 Score (si es un problema de clasificación) o Mean Squared Error (MSE) (si es un problema de regresión).
Mostrar gráficos como la Curva ROC (para clasificación) o gráfico de errores residuales (para regresión).
Visualización de Resultados:

Generar visualizaciones que resuman los resultados del análisis predictivo. Estas pueden incluir gráficos de dispersión con las predicciones, gráficos de barras, histogramas, etc.
Conclusiones y Recomendaciones:

Responder a la pregunta inicial o problema planteado con base en los resultados obtenidos.
Proporcionar posibles mejoras o recomendaciones para trabajos futuros.
Despliegue del Modelo:

(Opcional) Explica cómo podrías desplegar el modelo en un entorno productivo, como una API o una aplicación web.

## Rúbrica de Evaluación (Total: 100 puntos)
Criterio	Puntos	Descripción de la Evidencia Esperada
1. Descripción del Problema	10	- El participante describe claramente la pregunta o problema que el análisis intenta resolver. 
- Explicación de la relevancia del conjunto de datos seleccionado.
2. Análisis Exploratorio de Datos	20	- Se presentan gráficos para visualizar la distribución de los datos. 
- Identificación de valores atípicos o faltantes. 
- Comentarios sobre las relaciones entre variables.
3. Preparación de los Datos	15	- Los datos se limpian adecuadamente, con un enfoque claro en la eliminación de valores faltantes y duplicados. 
- Variables categóricas convertidas correctamente (si es necesario).
4. Modelado Predictivo	20	- Elección justificada del modelo (regresión, clasificación, etc.). 
- Implementación del modelo de aprendizaje automático correctamente ajustado. 
- Explicación de las variables utilizadas.
5. Evaluación del Modelo	15	- Utilización de las métricas adecuadas para evaluar el rendimiento del modelo. 
- Explicación clara de los resultados obtenidos y su interpretación.
6. Visualización de Resultados	10	- Las visualizaciones son claras y bien explicadas. 
- Los gráficos respaldan las conclusiones y proporcionan un resumen visual del análisis.
7. Conclusiones y Recomendaciones	10	- El análisis responde a la pregunta inicial. 
- Se proporcionan recomendaciones o ideas para mejorar el análisis o seguir trabajando con el conjunto de datos.
8. Despliegue del Modelo (Opcional)	10 (Opc.)	- Descripción clara de cómo el modelo podría ser implementado en un entorno productivo, por ejemplo, en una API o aplicación.

## Evidencias Esperadas

Código en Python utilizando Pandas, NumPy, Matplotlib/Seaborn y Scikit-learn para el análisis y modelado predictivo.

Informe escrito en el cual se detalle cada uno de los pasos del proyecto, las decisiones tomadas y las conclusiones alcanzadas.
Visualizaciones gráficas que respalden el análisis y resumen los resultados.

## Comentarios

Este proyecto permite a los participantes aplicar de forma integral lo aprendido durante el curso de Ciencia y Analítica de Datos con Python, trabajando con sus propios datos o seleccionando un conjunto de datos de su interés. Esto les brinda la oportunidad de obtener experiencia práctica en la manipulación de datos, construcción de modelos predictivos, evaluación de resultados y presentación de sus hallazgos de manera clara y concisa. Entrega tardía al dia siguiente, misma hora. 

# CONTEXTO
## Análisis Predictivo de un Conjunto de Datos de jugadores de liga universitaria de Basketball

Se dispone de un conjunto de datos que describen Nombre, Universidad de origen, las condiciones físicas, posición en la duela y logros obtenidos durante el último año. Con base a lo anterior, los directivos de la liga, desean aportar información a los equipos de ligas mayores para reforzar la ofensiva y conservar los jugadores que más aportan.

## OBJETIVO

Determinar los jugadores que lograron más de 500 puntos durante la temporada y pronosticar si lo pueden lograr en adelante.

## RESULTADOS

Se preparó la base de datos xls y se convirtió a csv. Posteriormente utilizando COLAB se cargó dicha base de datos y tomando como referencia el EJERCICIO 7 (gracias por compartir), se ejecutó de la siguiente forma.

1. Importar base de datos y librerías.
2. Revisar base de datos, 12 columnas y 3070 filas.
3. Revisar el tipo de columnas, 3 object y 9 int64.
4. Obtener datos estadísticos de la base de datos, como son, valores min y max, mediana, desviación estándar, quartíles.
5. Eliminar columnas object.
6. Visualización con histogramas de las 9 columnas.
7. Obtener matríz de correlaciones de jugadores.
8. Seleccionar y eliminar columna mayor500, asimismo, eliminar columna id.
9. División y entrenamiento, Xtrain, Xtest, ytrain, ytest. Test size del 40%.
10. Con randomForest, se calculan y grafican 7 variables.
11. Utilizando clasificador regresión logística. Importamos librería, modelos, ypredict y son 1228 pruebas arroja una exactitud de 1.0. Asimismo, se obtiene y muestra matríz de confusión.
12. Utilizando maquina soporte vectorial. Importamos librería, modelos, ypredict y son 1228 pruebas arroja una exactitud de 0.99. Asimismo, se obtiene y muestra matríz de confusión.
13. Utilizando clasificador bosque aleatorio. Importamos librería, modelos, ypredict y son 1228 pruebas arroja una exactitud de 1.0. Asimismo, se obtiene y muestra matríz de confusión.
14. Utilizando K-nearest Neighbour (KNN). Importamos librería, modelos, ypredict y son 1228 pruebas arroja una exactitud de 0.99. Asimismo, se obtiene y muestra matríz de confusión.
15. Utilizando Naive Bayes Gaussian. Importamos librería, modelos, ypredict y son 1228 pruebas arroja una exactitud de 0.96. Asimismo, se obtiene y muestra matríz de confusión.
16. Se importan librerías y se obtienen curvas ROC y puntuación AUC
17. Comparación de modelos:
18. Regresión Logística:  1.0
19. Máquina de Soporte Vectorial:  0.999659982810242
20. Bosque Aleatorio:  1.0
21. K-Nearest Neighbors:  0.9975679326010372
22. Naive Bayes:  0.9973932015451893
23. Se muestran las curvas ROC

24. **CONCLUSIONES**
25. El gráfico muestra que el algoritmo Random Forest obtuvo el mejor AUC. Por lo tanto, está claro que este modelo realizo un mejor trabajo a la hora de clasificar a jugadores con más de 500 pts.

![Captura de Pantalla 2024-10-08 a la(s) 7 03 28 p m](https://github.com/user-attachments/assets/a60ea1a1-e238-4d96-a16c-39a7044b475e)


**CODIGO**
![Captura de Pantalla 2024-10-08 a la(s) 6 42 03 p m](https://github.com/user-attachments/assets/98911c55-dc95-4eee-9853-77bf7613dc86)

![Captura de Pantalla 2024-10-08 a la(s) 6 42 46 p m](https://github.com/user-attachments/assets/de72ccee-058c-434b-b01d-8ad10f75eaa9)

![Captura de Pantalla 2024-10-08 a la(s) 6 43 42 p m](https://github.com/user-attachments/assets/7e95b3d7-75d7-4df7-a610-31d8dce7cb5d)

![Captura de Pantalla 2024-10-08 a la(s) 6 44 10 p m](https://github.com/user-attachments/assets/5425fb94-f1a4-4707-8b46-a9b33ebdc562)

![Captura de Pantalla 2024-10-08 a la(s) 6 44 44 p m](https://github.com/user-attachments/assets/18b1ea4a-b9be-475f-9051-b381247d34c2)

![Captura de Pantalla 2024-10-08 a la(s) 6 45 17 p m](https://github.com/user-attachments/assets/ccaff2fb-12ba-4752-9b3d-13d4c71a7e14)

![Captura de Pantalla 2024-10-08 a la(s) 6 45 46 p m](https://github.com/user-attachments/assets/92f95138-ab8f-4cc5-b85f-5f3e96331503)

![Captura de Pantalla 2024-10-08 a la(s) 6 46 22 p m](https://github.com/user-attachments/assets/34579366-880b-42fb-94ba-60d0f9b5e587)

![Captura de Pantalla 2024-10-08 a la(s) 6 47 14 p m](https://github.com/user-attachments/assets/abbafe94-a277-47f6-b818-9d46545ec4d8)

![Captura de Pantalla 2024-10-08 a la(s) 6 47 37 p m](https://github.com/user-attachments/assets/3d71f6ad-e83f-4222-8103-48415481caa6)

![Captura de Pantalla 2024-10-08 a la(s) 6 47 55 p m](https://github.com/user-attachments/assets/d2d19f59-4cfe-46f6-b92e-60474da84e11)

![Captura de Pantalla 2024-10-08 a la(s) 6 48 25 p m](https://github.com/user-attachments/assets/3da623f4-567d-46f8-a460-7495a7c4b0be)

![Captura de Pantalla 2024-10-08 a la(s) 6 49 01 p m](https://github.com/user-attachments/assets/9833f06a-11fd-4882-a071-7de698c33186)

![Captura de Pantalla 2024-10-08 a la(s) 6 49 24 p m](https://github.com/user-attachments/assets/3560179b-f837-4ce7-9654-65bea4d93529)

![Captura de Pantalla 2024-10-08 a la(s) 6 49 43 p m](https://github.com/user-attachments/assets/7a077df9-f71d-4536-a5c7-f007182deb6d)

![Captura de Pantalla 2024-10-08 a la(s) 6 50 24 p m](https://github.com/user-attachments/assets/3d08ebac-df7e-4493-966d-0fbcf9767987)

![Captura de Pantalla 2024-10-08 a la(s) 6 50 51 p m](https://github.com/user-attachments/assets/f6dad875-ecea-4699-a569-335999056227)

![Captura de Pantalla 2024-10-08 a la(s) 6 51 07 p m](https://github.com/user-attachments/assets/8c938d8c-f92f-4970-8199-b1775fce3fdc)

![Captura de Pantalla 2024-10-08 a la(s) 6 52 15 p m](https://github.com/user-attachments/assets/55238cb0-6718-4666-a8c5-24295657c3ff)

![Captura de Pantalla 2024-10-08 a la(s) 6 52 41 p m](https://github.com/user-attachments/assets/9e5640ed-2e02-4303-a5fe-3b31e13b924b)

![Captura de Pantalla 2024-10-08 a la(s) 6 53 15 p m](https://github.com/user-attachments/assets/5176bb07-0a65-4945-b187-fb2d4b6dfb88)

![Captura de Pantalla 2024-10-08 a la(s) 6 53 33 p m](https://github.com/user-attachments/assets/d442bf87-367a-4433-9189-de25891cca0c)

![Captura de Pantalla 2024-10-08 a la(s) 6 54 03 p m](https://github.com/user-attachments/assets/fd430103-75ef-4f94-b5fd-7f341efa385f)

![Captura de Pantalla 2024-10-08 a la(s) 6 54 21 p m](https://github.com/user-attachments/assets/9e74502a-ecd6-4202-add6-93ec96e5c22d)

![Captura de Pantalla 2024-10-08 a la(s) 6 54 47 p m](https://github.com/user-attachments/assets/757c07ea-98f7-4c1b-b302-769e75f72603)

![Captura de Pantalla 2024-10-08 a la(s) 6 55 16 p m](https://github.com/user-attachments/assets/4f2970ec-4263-4e0b-9218-40a4e51cc654)

![Captura de Pantalla 2024-10-08 a la(s) 6 56 10 p m](https://github.com/user-attachments/assets/c7586687-d183-4b7c-9e08-6441d526844d)

![Captura de Pantalla 2024-10-08 a la(s) 6 56 48 p m](https://github.com/user-attachments/assets/524b760d-08dd-45d8-949f-44a5421079ce)

![Captura de Pantalla 2024-10-08 a la(s) 6 57 23 p m](https://github.com/user-attachments/assets/e7768262-f4d2-45d6-af2e-ad01e11d76f1)
