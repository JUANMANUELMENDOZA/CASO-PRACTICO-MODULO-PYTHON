# CONTEXTO

## Análisis Predictivo de un Conjunto de Datos de jugadores de liga universitaria de Basketball

Se dispone de un conjunto de datos que describen Nombre, Universidad de origen, las condiciones físicas, posición en la duela y logros obtenidos durante el último año. Con base a lo anterior, los directivos de la liga, desean aportar información a los equipos de ligas mayores para reforzar la ofensiva y conservar los jugadores que más aportan.

## OBJETIVO

Determinar los jugadores que lograron más de 500 puntos durante la temporada y evaluar si el pronóstico si lo pueden lograr en adelante.

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
11. Utilizando clasificador regresión logística. Importamos librería, modelos, ypredict y son 1228 pruebas arroja una exactitud de 0.99. Asimismo, se obtiene y muestra matríz de confusión.
12. Utilizando maquina soporte vectorial. Importamos librería, modelos, ypredict y son 1228 pruebas arroja una exactitud de 0.99. Asimismo, se obtiene y muestra matríz de confusión.
13. Utilizando clasificador bosque aleatorio. Importamos librería, modelos, ypredict y son 1228 pruebas arroja una exactitud de 1.0. Asimismo, se obtiene y muestra matríz de confusión.
14. Utilizando K-nearest Neighbour (KNN). Importamos librería, modelos, ypredict y son 1228 pruebas arroja una exactitud de 0.98. Asimismo, se obtiene y muestra matríz de confusión.
15. Utilizando Naive Bayes Gaussian. Importamos librería, modelos, ypredict y son 1228 pruebas arroja una exactitud de 0.97. Asimismo, se obtiene y muestra matríz de confusión.
16. Se importan librerías y se obtienen curvas ROC y puntuación AUC
17. Comparación de modelos:
18. Regresión Logística:  0.999785047249799
19. Máquina de Soporte Vectorial:  0.999745241184947
20. Bosque Aleatorio:  1.0
21. K-Nearest Neighbors:  0.9972268441486412
22. Naive Bayes:  0.9966483293394581
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

![Captura de Pantalla 2024-10-07 a la(s) 8 24 25 p m](https://github.com/user-attachments/assets/c4540585-98e8-4443-ab0a-bbfba02abdd3)


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
