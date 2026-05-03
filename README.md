# Modelo Recomendador Espectro-Gráfico para Audios Musicales

**Autor:** Angelica Margarita Flores Islas  
**Asesor**: Tomás Pérez Becerra

Este repositorio contiene el desarrollo del **Proyecto Terminal** para la **Maestría en Ciencia de Datos (MCD)**. 
El objetivo principal es construir un sistema de recomendación musical basado en el análisis de características extraídas de espectrogramas de audio.

## 📂 Estructura del Proyecto

El repositorio está organizado de la siguiente manera:

* **`Dataframe/`**: Contiene el dataset de características extraídas.
    * `features.csv`: Características numéricas derivadas de los archivos de audio.
* **`Modelos/`**: Modelos entrenados y serializados para su reutilización.
    * `standardScaler_21abril2026.joblib`: Escalador de datos.
    * `modeloPCA_21abril2026.joblib`: Modelo de Reducción de Dimensionalidad (PCA).
    * `modeloKmeans_21abril2026.joblib`: Modelo de clustering para segmentación musical.
    * `modelosKnnClusters_21abril202...`: Modelos de vecinos cercanos para la recomendación final.
* **`Notebooks/`**: Flujo de trabajo documentado paso a paso.
    * `Obtención_de_Espectrogramas.ipynb`: Procesamiento de señales de audio raw.
    * `Exploración_del_dataset.ipynb`: Análisis exploratorio de datos (EDA).
    * `Simulación.ipynb`: Pruebas de funcionamiento del recomendador.
    * `EvaluaciónUsuario.ipynb`: Procesamiento de resultados de evaluación de satisfacción.
* **`Objetos/`**: Archivos temporales y procesados para optimizar el rendimiento.
    * `df_test_scaled.csv`, `df_train_pca.csv`: Datos listos para inferencia.

## 🛠️ Requisitos e Instalación

Para ejecutar los notebooks de este proyecto, se recomienda crear un entorno virtual e instalar las siguientes dependencias:

```bash
pip install numpy pandas matplotlib seaborn librosa scikit-learn joblib
