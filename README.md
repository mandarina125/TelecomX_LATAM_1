# 📊 Telecom X – Análisis de Evasión de Clientes (Churn)

Este proyecto forma parte de un desafío del curso de Ciencia de Datos, cuyo objetivo es **analizar los factores que influyen en la pérdida de clientes** de una empresa de telecomunicaciones y proponer recomendaciones para reducir el *churn*.

---

## 📌 Objetivo del Proyecto
Identificar patrones y variables que influyen en la cancelación del servicio, aplicando un flujo **ETL (Extracción, Transformación y Carga)** y un **Análisis Exploratorio de Datos (EDA)** con Python, para generar conclusiones y recomendaciones.

---

## 🛠️ Tecnologías Utilizadas
- **Python 3**
- **Pandas** – Manipulación de datos
- **Matplotlib** y **Seaborn** – Visualización
- **Jupyter Notebook**
- **JSON** – Formato de datos de entrada

---

## 🔄 Flujo del Proyecto

### 1️⃣ Extracción de Datos
- Carga del dataset en formato JSON desde fuente local.
- Normalización de datos anidados con `pd.json_normalize()`.

### 2️⃣ Transformación y Limpieza
- Conversión de tipos de datos (`TotalCharges` a numérico).
- Eliminación de duplicados por `customerID`.
- Tratamiento de valores nulos.
- Ajuste de etiquetas para mayor legibilidad (ej. `SeniorCitizen` a "Sí"/"No").

### 3️⃣ Análisis Exploratorio de Datos (EDA)
- Distribución general del churn (26.6% de cancelaciones).
- Comparación por variables categóricas:
  - **Tipo de contrato**: Mayor churn en contratos mensuales (~1500 clientes).
  - **Método de pago**: Mayor churn en clientes que usan cheque electrónico.
  - **Tipo de Internet**: Fibra óptica presenta mayor tasa de cancelación.
  - **Género**: No hay diferencias significativas.
  - **SeniorCitizen**: Segmento relevante para explorar con mayor detalle.
- Visualizaciones: `countplot`, gráficos de proporciones y diagramas circulares.

### 4️⃣ Conclusiones e Insights
- El **contrato mensual** es un factor clave de cancelación.
- **Cheque electrónico** está asociado a mayor churn.
- **Fibra óptica** podría implicar expectativas más altas y menor tolerancia a fallos.
- No hay relación directa entre **género** y churn.

### 5️⃣ Recomendaciones
- Incentivar migración de contratos mensuales a anuales.
- Promover métodos de pago automáticos.
- Mejorar experiencia de usuarios de fibra óptica mediante encuestas y soporte proactivo.
- Implementar alertas internas para clientes con perfil de alto riesgo.

---

---

## 🚀 Ejecución del Proyecto
1. Clonar este repositorio:
   ```bash
   git clone https://github.com/<usuario>/<repositorio>.git


## 📂 Estructura del Repositorio
