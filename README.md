# 🛒 NovaRetail+ – Análisis de correlaciones: ¿qué comportamientos del cliente se asocian con el ingreso anual?

Este repositorio contiene el análisis del **Proyecto 7** del curso, correspondiente al caso de **NovaRetail+**, una plataforma de comercio electrónico en Latinoamérica.

El objetivo de este proyecto es explorar qué factores del comportamiento del cliente están más fuertemente asociados con el ingreso anual generado. Para ello, se analiza un dataset que contiene información demográfica, de uso y de interacción de los clientes, buscando identificar relaciones correlacionales clave que puedan informar estrategias de crecimiento y retención.

---

## 📂 Contenido del repositorio

| Archivo/Carpeta | Descripción |
|---|---|
| `S8_Student_Version-Project-NovaRetail.ipynb` | Notebook principal con la limpieza, el Análisis Exploratorio de Datos (EDA), las visualizaciones, el análisis de correlaciones y las conclusiones ejecutivas. |
| `README.md` | Este archivo. |

*(Nota: El archivo del dataset `novaretail_comportamiento_clientes_2024.csv` no se incluye en este repositorio, pero se puede cargar desde la ruta `/datasets/` mencionada en el notebook).*

---

## 🧠 Objetivo del análisis

- **Determinar qué factores** del comportamiento del cliente (visitas, compras, gasto en publicidad, etc.) tienen una mayor asociación con el **ingreso anual** que generan para la empresa.
- **Identificar relaciones** entre variables numéricas y categóricas utilizando diferentes coeficientes de correlación (Pearson, Spearman, Punto-biserial y V de Cramér).
- **Visualizar** las relaciones clave mediante mapas de calor y gráficos de dispersión para una interpretación más intuitiva.
- **Generar insights** y recomendaciones prácticas para el equipo de **Crecimiento y retención** de NovaRetail+.

---

## 📊 Etapas del análisis realizadas

1. **Carga y exploración inicial** → Carga del dataset, revisión de tipos de datos y valores faltantes.
2. **Preparación y limpieza** → Corrección de tipos de datos (ej. `edad` a `int64`), identificación de variables binarias y categóricas.
3. **Análisis Descriptivo** → Estadísticas resumen y diagnóstico de la distribución de las variables numéricas.
4. **Visualización de Relaciones** → Creación de un mapa de calor para visualizar correlaciones entre variables numéricas y gráficos de dispersión para los pares más relevantes.
5. **Cálculo de Coeficientes de Correlación** → Aplicación de Pearson, Spearman, Punto-biserial y V de Cramér para cuantificar la fuerza y dirección de las relaciones entre variables.
6. **Interpretación y Hallazgos** → Documentación de los principales hallazgos y su significado para el negocio.
7. **Limitaciones y Próximos Pasos** → Identificación de las limitaciones del análisis y propuestas para futuras investigaciones.

---

## 📈 Principales hallazgos

- **Relación Visitas vs. Gasto Publicitario:** Existe una correlación moderada (0.58) entre el número de visitas mensuales y el gasto en publicidad dirigida, sugiriendo que la publicidad llega a los usuarios más activos.
- **Relación Visitas vs. Ingreso Anual:** Se observa una correlación débil (0.34) entre las visitas y el ingreso anual, lo que indica que las visitas por sí solas no son un fuerte predictor del ingreso generado.
- **Membresía Premium vs. Ingreso Anual:** La membresía premium muestra una correlación muy baja (0.09) con el ingreso anual, lo que apunta a un valor percibido bajo del programa premium.
- **Satisfacción vs. Abandono:** La correlación entre satisfacción y abandono es prácticamente nula (-0.02), indicando que otros factores (como el precio o la competencia) son más determinantes en la decisión de abandonar la plataforma.
- **Variables Categóricas:** No existe una asociación relevante (V de Cramér de 0.012) entre el tipo de dispositivo y la región del cliente, sugiriendo un acceso homogéneo a la plataforma.

---

## 💡 Recomendaciones comerciales

- **Revisar la estrategia de publicidad dirigida:** Dado que el gasto publicitario se correlaciona con visitas pero no con el ingreso, se recomienda optimizar las campañas para enfocarse en la conversión a compras, no solo en el tráfico.
- **Potenciar el programa de membresía premium:** La baja correlación con el ingreso sugiere que el programa actual no es atractivo. Se recomienda rediseñar sus beneficios para ofrecer un valor más claro y tangible para los clientes.
- **Centrarse en la conversión de visitas a compras:** La debilidad de la relación entre visitas e ingreso sugiere que un embudo de conversión ineficiente podría estar frenando las ventas. Se recomienda analizar el funnel y optimizar la experiencia de compra.
- **Investigar las causas del abandono:** Dado que la satisfacción no es un factor determinante en el abandono, se deben realizar estudios (ej. encuestas) para identificar otras causas clave, como la competitividad de precios o la oferta de la competencia.
- **Segmentación por comportamiento:** Crear segmentos de clientes basados en su nivel de ingreso y actividad para personalizar las estrategias de marketing.

---

## ▶️ Cómo abrir el notebook en Google Colab

Haz clic en el siguiente botón:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/)

O:

1. Abre el archivo `S8_Student_Version-Project-NovaRetail.ipynb` en GitHub
2. Haz clic en **Open in Colab**

---

## 📘 Cómo reproducir el análisis

### Opción 1: En Google Colab (recomendado)

1. Abre el notebook en Google Colab
2. Ejecuta las primeras celdas, que ya cargan el dataset directamente desde la ruta `/datasets/`
3. Ejecuta todas las celdas en orden

### Opción 2: En Jupyter Notebook local

1. Clona este repositorio
2. Asegúrate de que el archivo `novaretail_comportamiento_clientes_2024.csv` esté en la ruta `/datasets/` o cambia la ruta en la celda de carga de datos.
3. Abre `S8_Student_Version-Project-NovaRetail.ipynb`
4. Ejecuta las celdas en orden

---

## 📦 Dependencias necesarias

```bash
pip install pandas numpy matplotlib seaborn scipy
