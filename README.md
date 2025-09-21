# Regresion_Logistica

En este repositorio encontrarás una práctica sobre **regresión logística**, un modelo que se utiliza cuando queremos **predecir clases**. La idea es que el modelo genera **probabilidades** y, a partir de un **umbral**, decidimos si una observación pertenece a la clase 0 o a la clase 1.

Para evaluar qué tan bueno es nuestro modelo, se utilizan diferentes métricas:

* **Accuracy (Exactitud):** mide el porcentaje total de predicciones correctas (positivas y negativas).
* **Sensitivity (Sensibilidad):** mide qué tan bien el modelo identifica los casos positivos, es decir, la proporción de verdaderos positivos detectados.
* **Specificity (Especificidad):** mide qué tan bien el modelo identifica los casos negativos, es decir, la proporción de verdaderos negativos detectados.

Además, se utiliza la **curva ROC** (*Receiver Operating Characteristic*), que muestra el balance entre la sensibilidad y la especificidad a distintos umbrales. El **AUC (Área Bajo la Curva)** resume en un solo valor qué tan bien el modelo puede diferenciar entre las dos clases: mientras más cercano esté a **1**, mejor es el desempeño del modelo.

La base de datos proviene de la **Encuesta Nacional de Inclusión Financiera (ENIF) 2024**, realizada por el **INEGI**. Esta encuesta fue aplicada a un total de **13,303 personas**, quienes respondieron preguntas sobre diversas características de su vivienda y situación económica.

Para más información, consulta este [link](https://www.inegi.org.mx/app/descarga/ficha.html?tit=2534415&ag=0&f=csv).

La base de datos contiene tanto variables categóricas como numéricas. Algunas de las más relevantes son:
* **`p0_4_1A`**: Número de automóviles en la vivienda (numérica).
* **`p0_4_2`**: Si la vivienda tiene acceso a internet (categórica: 1 = Sí, 2 = No).
* **`p1_1`**: Año de construcción de la vivienda (numérica).
* **`p1_2`**: Si las personas comparten el mismo gasto para comida (categórica: 1 = Sí, 2 = No).
* **`p1_3`**: Número de grupos de personas con gasto separado para comida (numérica).
* **`folio`**: Folio único de registro (categórica).
* **`ent`**: Estado donde se encuentra la vivienda (categórica).
* **`tloc`**: Tamaño de localidad (categórica).
* **`region`**: Región geográfica del país (categórica).

Nuestra **variable de interés** es si la vivienda **tiene automóvil o no**, lo cual se modela como una variable binaria (0 = No tiene auto, 1 = Sí tiene auto).

En este repositorio encontrarás los siguientes documentos:

* [Archivo en ipynb](Regresion_Logistica.ipynb)
* [Archivo en HTML](Regresion_Logistica.html)
* [Base de datos](conjunto_de_datos_tvivienda_enif2024.csv)
