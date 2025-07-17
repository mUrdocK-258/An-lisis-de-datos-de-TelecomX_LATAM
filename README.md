# 📊 Análisis de Evasión de Clientes – TelecomX LATAM

Este proyecto tiene como propósito identificar los factores que influyen en la **evasión de clientes (churn)** en una empresa de telecomunicaciones de Latinoamérica. Se utiliza un enfoque exploratorio de análisis de datos (EDA) con Python, junto a visualizaciones estadísticas, para descubrir patrones relevantes que permitan mejorar la retención de clientes.

---

## 🧠 Objetivo del Proyecto

Comprender y analizar el comportamiento de los clientes mediante:

- Exploración de datos limpios del cliente.
- Análisis de variables demográficas y de uso de servicios.
- Visualización de la relación entre distintas variables y la evasión.
- Generación de insights útiles para modelos de predicción futuros.

---

## 📁 Estructura del Proyecto

TelecomX_LATAM/
│
├── TelecomX_LATAM.ipynb # Notebook principal con todo el análisis exploratorio
├── datos_clientes_limpios.csv # Dataset base con columnas limpias y transformadas (no incluido)
└── README.md # Este archivo descriptivo del proyecto


---

## 🧰 Herramientas Utilizadas

- **Python 3.11**
- `pandas` – manipulación de datos
- `numpy` – operaciones numéricas
- `matplotlib` y `seaborn` – visualización de datos
- `plotly` – gráficos interactivos
- `scikit-learn` – para pasos iniciales de codificación y normalización (opcional)

---

## 📦 Contenido del Análisis

### 🔹 1. Carga y comprensión del dataset
- Exploración de columnas como género, tipo de contrato, servicios contratados, antigüedad, entre otras.
- Conversión de variables categóricas a un formato interpretable (por ejemplo: de `"Female"` a `"Femenino"`).

### 🔹 2. Limpieza y transformación
- Estandarización de valores como `"Sin servicio de internet"` a `0`.
- Recuento del total de servicios contratados por cliente (columna `Cantidad_Servicios`).
- Conversión de tipos de datos inconsistentes.

### 🔹 3. Análisis univariado y bivariado
- Distribución de la evasión por género, contrato, método de pago y edad.
- Gráficos de barra y torta para variables categóricas.
- Histogramas para variables numéricas.

### 🔹 4. Análisis de correlación
- Uso de `df.corr()` para identificar qué variables están más relacionadas con la evasión (`Abandono`).
- Visualización con mapa de calor (`heatmap`) para facilitar la interpretación.

---

## 📊 Ejemplos de Visualizaciones

- Distribución de clientes que abandonan según su tipo de contrato.
- Relación entre `Cargo_Mensual` y tasa de evasión.
- Mapa de calor con las correlaciones entre variables numéricas.
- Gráficos comparativos de clientes con y sin servicios específicos.

---

## 🚧 Posibles Problemas Detectados

- Algunos campos contienen texto como `'Sin servicio de internet'`, lo cual dificulta las operaciones numéricas si no se transforman previamente.
- El tipo de dato de ciertas columnas puede no ser consistente (`str` en lugar de `int`), lo que genera errores en operaciones como `.sum()` o `.corr()`.

---

## 📌 Recomendaciones Futuras

- Incluir modelos predictivos (Regresión logística, Árboles de decisión, Random Forest).
- Usar técnicas de Feature Engineering para mejorar las predicciones.
- Implementar un dashboard con **Streamlit**, **Dash** o **Power BI**.
- Evaluar impacto de cada servicio en la permanencia de los clientes.

---

## 🧾 Notas Técnicas

- Este proyecto está desarrollado como un **notebook de Jupyter** completamente ejecutable paso a paso.
- El dataset debe estar previamente limpio y en formato `.csv` para su correcto funcionamiento.
- Asegúrate de tener instaladas las librerías necesarias (`pandas`, `seaborn`, `plotly`, etc).

---

## 📬 Autor

**Nombre:** [Tu Nombre Aquí]  
**Email:** [tunombre@correo.com]  
**LinkedIn:** [https://linkedin.com/in/tu_usuario](https://linkedin.com/in/tu_usuario)

---

## 🗂 Licencia

Este proyecto es de uso académico y educativo. Puedes reutilizarlo mencionando la fuente.  
© 2025 – TelecomX LATAM – Proyecto de análisis de datos.
