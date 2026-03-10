# Telecom X — Análisis de Evasión de Clientes (Churn)

## Descripción del proyecto

Este proyecto tiene como objetivo analizar el comportamiento de los clientes de **Telecom X** para identificar factores asociados a la **evasión de clientes (churn)**.

La empresa enfrenta una alta tasa de cancelación de servicios y requiere comprender qué variables pueden estar relacionadas con este fenómeno. Para ello se realizó un proceso de **ETL (Extract, Transform, Load)** y un **análisis exploratorio de datos (EDA)** utilizando Python.

El resultado de este análisis servirá como base para futuros modelos predictivos que permitan anticipar la cancelación de clientes y diseñar estrategias de retención.

---

# Objetivos del análisis

- Extraer datos desde un archivo **JSON** proporcionado por la empresa.
- Transformar y limpiar los datos para su análisis.
- Explorar patrones relacionados con el churn.
- Generar visualizaciones que permitan comprender el comportamiento de los clientes.
- Identificar posibles factores asociados a la cancelación del servicio.

---

# Tecnologías utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Google Colab / Jupyter Notebook

---

# Estructura del proyecto

TelecomX-Churn-Analysis/
│
├── TelecomX_Data.json
├── Challenge_Telecom_I.ipynb
├── README.md


**Descripción de archivos**

- **TelecomX_Data.json**  
  Dataset proporcionado para el análisis de churn.

- **TelecomX_ETL_Churn.ipynb**  
  Notebook donde se desarrolla todo el proceso de análisis:
  
  - Extracción de datos
  - Transformación y limpieza
  - Análisis exploratorio
  - Visualización de resultados
  - Informe final

- **README.md**  
  Documentación del proyecto.

---

# Proceso de análisis

El análisis se desarrolló siguiendo las etapas del proceso **ETL**:

## 1. Extracción
Los datos fueron cargados desde un archivo JSON y convertidos en un **DataFrame de Pandas** para su manipulación.

## 2. Transformación
Durante esta etapa se realizaron las siguientes tareas:

- Normalización de nombres de columnas
- Conversión de variables categóricas
- Conversión de variables numéricas
- Tratamiento de valores nulos
- Preparación del dataset para análisis

## 3. Carga y análisis
Se realizaron diferentes análisis exploratorios para entender los patrones de churn en los clientes.

Entre los análisis realizados se incluyen:

- Tasa general de churn
- Churn por tipo de contrato
- Churn por método de pago
- Distribución de permanencia de clientes
- Relación entre permanencia y cargos mensuales
- Churn por tipo de servicio de internet

---

# Principales insights

A partir del análisis se identificaron los siguientes hallazgos:

### 1. Alta tasa de churn
La tasa general de churn observada fue aproximadamente **26.58%**, lo que indica que una proporción considerable de clientes cancela el servicio.

### 2. Tipo de contrato
Los clientes con contratos **Month-to-month** presentan tasas significativamente más altas de churn en comparación con contratos de largo plazo.

### 3. Permanencia del cliente
Los clientes con **menor tiempo de permanencia (tenure)** tienden a abandonar el servicio con mayor frecuencia.

### 4. Método de pago
Algunos métodos de pago presentan mayores tasas de churn, lo que podría indicar fricciones en el proceso de pago o perfiles de clientes con menor fidelización.

---

# Ejemplos de visualizaciones

El proyecto incluye diferentes gráficos para comprender los patrones de churn, entre ellos:

- Distribución de churn
- Churn por tipo de contrato
- Churn por método de pago
- Distribución de permanencia de clientes
- Relación entre permanencia y cargos mensuales

Estas visualizaciones permiten identificar tendencias y posibles factores asociados a la evasión de clientes.

---

# Cómo ejecutar el proyecto

## Opción 1 — Google Colab

1. Abrir Google Colab
2. Subir el archivo `Challenge_Telecom_I.ipynb`
3. Subir el archivo `TelecomX_Data.json`
4. Ejecutar todas las celdas del notebook
