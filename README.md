# analysis-telecom

## 🎯 Objetivo del proyecto

El objetivo de este proyecto es analizar el comportamiento de los clientes de ConnectaTel, una empresa de telecomunicaciones con operaciones en Latinoamérica.

A través del análisis estadístico del uso de llamadas y mensajes, se busca identificar patrones de consumo, detectar comportamientos atípicos y comprender las diferencias entre segmentos de clientes según su edad, plan contratado y nivel de uso.

Los resultados del análisis permiten generar insights y recomendaciones orientadas a optimizar la oferta comercial y comprender mejor las necesidades de los usuarios.

---

## 📁 Datasets utilizados

El análisis utiliza tres fuentes de datos:

- **`plans.csv`**: catálogo de los planes disponibles, incluyendo precios, minutos, mensajes y beneficios incluidos.
- **`users_latam.csv`**: información de los clientes, incluyendo edad, ciudad, fecha de registro, plan contratado y fecha de churn.
- **`usage.csv`**: registros de actividad de los usuarios, incluyendo llamadas, mensajes, duración de llamadas y longitud de mensajes.

Los datasets se encuentran almacenados en la carpeta `datasets/` del repositorio.

---

## 🔎 Etapas del análisis

El proyecto se desarrolló siguiendo las siguientes etapas:

1. **Carga y exploración inicial**
   - Revisión de la estructura, dimensiones y tipos de datos de cada dataset.

2. **Identificación de problemas de calidad**
   - Análisis de valores nulos.
   - Detección de valores sentinel.
   - Validación de fechas y rangos inconsistentes.

3. **Limpieza y estandarización**
   - Tratamiento de valores sentinel.
   - Conversión de tipos de datos.
   - Corrección de fechas imposibles.
   - Evaluación de valores nulos según su contexto.

4. **Análisis estadístico descriptivo**
   - Cálculo de media, mediana, percentiles y medidas de dispersión.
   - Análisis de variables numéricas y categóricas.

5. **Visualización de distribuciones y detección de outliers**
   - Creación de histogramas y boxplots.
   - Análisis de la forma de las distribuciones.
   - Identificación de valores atípicos mediante el método IQR.

6. **Segmentación de clientes**
   - Clasificación de usuarios por grupo de edad.
   - Clasificación de usuarios según su nivel de uso.
   - Análisis cruzado entre edad y comportamiento de consumo.

7. **Análisis ejecutivo**
   - Interpretación de los principales hallazgos.
   - Identificación de segmentos comercialmente relevantes.
   - Desarrollo de recomendaciones orientadas al negocio.

---

## 🛠️ Herramientas utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook
- Google Colab

---

## ▶️ Cómo ejecutar el notebook + Guía de Reproducción

Puedes abrir y ejecutar el análisis directamente en Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/rojaspetit/analysis-telecom/blob/main/tt_telecom_connectatel_analysis.ipynb)

1. Haz clic en **Open In Colab**.
2. Ejecuta las celdas en orden:
   * Empieza por la celda "#importar librerías",
   * Ejecuta la celda "#cargar repositorio de github". De esta forma, podrás cargar los archivos necesarios para el análisis.
   * Continúa ejecutando en orden para reproducir exactamente la exploración, limpieza, cálculos, gráficos y análisis realizado.
