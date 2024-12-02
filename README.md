
# Machine Learning de Extremo a Extremo: Predicción de la Calidad del Vino

Este repositorio contiene un Jupyter Notebook que demuestra un **ejemplo de extremo a extremo** para entrenar modelos de machine learning utilizando datos tabulares. El proyecto se centra en predecir la calidad del vino portugués "Vinho Verde" en función de sus propiedades fisicoquímicas.

## Descripción General

Este tutorial incluye los siguientes pasos:
1. Visualizar los datos utilizando **Seaborn** y **Matplotlib**.
2. Realizar una búsqueda paralela de hiperparámetros para entrenar múltiples modelos.
3. Explorar los resultados de la búsqueda de hiperparámetros con **MLflow**.
4. Registrar el modelo con mejor rendimiento en **MLflow**.
5. Aplicar el modelo registrado a un nuevo conjunto de datos utilizando un **Spark UDF**.

El conjunto de datos utilizado proviene del [Repositorio de Aprendizaje Automático de UCI](https://archive.ics.uci.edu/ml/datasets/wine+quality), presentado originalmente en:
> Cortez et al., 2009 - *Modeling wine preferences by data mining from physicochemical properties*.

## Conjunto de Datos

El notebook procesa dos conjuntos de datos:
- **Calidad del Vino Blanco**
- **Calidad del Vino Tinto**

Estos conjuntos de datos se combinan en un único DataFrame con una característica binaria adicional `is_red` que indica el tipo de vino.

## Requisitos

- Un clúster ejecutando **Databricks Runtime 15.4 LTS ML** o superior.
- Librerías de Python: `pandas`, `numpy`, `seaborn`, `matplotlib`, `MLflow`, y `pyspark`.
- Acceso a los conjuntos de datos de vino blanco y vino tinto (enlaces proporcionados en el notebook).

**Nota**: Si tu entorno está habilitado para Unity Catalog, utiliza la versión de este notebook adaptada para dichos entornos ([AWS](https://docs.databricks.com/mlflow/end-to-end-example.html) | [Azure](https://docs.microsoft.com/azure/databricks/mlflow/end-to-end-example) | [GCP](https://docs.gcp.databricks.com/mlflow/end-to-end-example.html)).

## Cómo Usarlo

1. Clona este repositorio y abre el notebook en tu entorno Jupyter o espacio de trabajo de Databricks.
2. Sigue los pasos descritos en el notebook para preprocesar los datos, entrenar modelos y evaluar resultados.
3. Utiliza la interfaz de seguimiento de MLflow para explorar el rendimiento de los modelos y registrar el mejor modelo.

## Resultados

- Modelos de machine learning entrenados con ajuste de hiperparámetros.
- Un modelo registrado en MLflow.
- Visualizaciones de distribuciones de datos y resultados del entrenamiento.

## Referencias

- [Repositorio de Aprendizaje Automático de UCI - Conjunto de Datos de Calidad del Vino](https://archive.ics.uci.edu/ml/datasets/wine+quality)
- [Documentación de Ejemplo de Extremo a Extremo de Databricks MLflow](https://docs.databricks.com/mlflow/end-to-end-example.html)

## Licencia

Este proyecto se distribuye bajo la Licencia MIT.


# MLOps_vino-Project
