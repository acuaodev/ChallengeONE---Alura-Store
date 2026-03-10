# 📊 Challenge Data Science — Análisis de Tiendas AluraStore

Proyecto de análisis de datos desarrollado como parte del **Challenge 1 de Data Science** de Alura Latam. El objetivo es ayudar al Sr. Juan a decidir cuál de sus 4 tiendas debería vender para iniciar un nuevo emprendimiento, con base en métricas de rendimiento extraídas de los datos históricos de ventas.

---

## 🎯 Objetivo

Analizar el desempeño de las 4 tiendas de la cadena **AluraStore** a partir de sus datos de ventas e identificar cuál presenta el menor rendimiento global, para recomendar su venta al Sr. Juan.

---

## 🗂️ Estructura del proyecto

```
Challenge01 - Store/
│
├── Challenge - AluraStore.ipynb   # Notebook principal con todo el análisis
└── README.md                      # Este archivo
```

---

## 📋 Análisis realizados

| #  | Análisis                           | Descripción                                                         |
|----|------------------------------------|---------------------------------------------------------------------|
| 1  | **Ingresos totales**               | Suma de la columna `Precio` por tienda                              |
| 2  | **Ventas por categoría**           | Agrupación por `Categoría del Producto` con conteo de ventas        |
| 3  | **Calificación promedio**          | Promedio de la columna `Calificación` por tienda                    |
| 4  | **Productos más y menos vendidos** | `value_counts()` sobre la columna `Producto` por tienda             |
| 5  | **Costo de envío promedio**        | Promedio de `Costo de envío` pagado por el cliente, por tienda      |

---

## 📈 Visualizaciones generadas

- **Barras** — Ingreso total por tienda
- **Línea con puntos** — Calificación promedio por tienda (con línea de promedio global)
- **Barras agrupadas** — Ventas por categoría comparando las 4 tiendas
- **Dispersión** — Relación entre ingreso total y costo de envío promedio
- **Barras horizontales** — Productos más y menos vendidos por tienda

---

## 🔍 Resultados principales

| Indicador                   | Tienda 1        | Tienda 2        | Tienda 3        | Tienda 4        |
|-----------------------------|-----------------|-----------------|-----------------|-----------------|
| Ingreso total               | $1,150,880,400 🥇| $1,116,343,500  | $1,098,019,600  | $1,038,375,700 🔴|
| Calificación promedio       | 3.98 🔴          | 4.04            | 4.05 🥇          | 4.00            |
| Costo de envío promedio     | $26,019 🔴       | $25,216         | $24,806         | $23,459 🥇       |

---

## ✅ Conclusión y recomendación

Se recomienda que el **Sr. Juan venda la Tienda 4**, ya que es la que presenta el peor desempeño general:

- 💸 **Menores ingresos totales** de toda la cadena (~$1,038M), con una diferencia significativa respecto al resto.
- ⭐ **Calificación intermedia** (4.00), sin destacar positivamente frente a Tienda 2 (4.04) y Tienda 3 (4.05).
- 📦 Su único punto positivo —el **menor costo de envío** promedio ($23,459)— no se traduce en mejores resultados comerciales ni en mayor satisfacción del cliente.
- 🛍️ Mix de productos con categorías de bajo rendimiento: es la única tienda donde **Instrumentos musicales** figura como la categoría menos vendida.

Las demás tiendas presentan ingresos y calificaciones superiores, lo que las hace más rentables y con mayor potencial de crecimiento.

---

## 🛠️ Tecnologías utilizadas

| Herramienta     | Uso                                          |
|-----------------|----------------------------------------------|
| Python 3        | Lenguaje principal del análisis              |
| Pandas          | Carga, limpieza y manipulación de datos      |
| Matplotlib      | Generación de gráficos y visualizaciones     |
| Google Colab    | Entorno de ejecución del notebook            |

---

## 📦 Datos

Los datos provienen del repositorio oficial del challenge:

```
https://github.com/alura-es-cursos/challenge1-data-science-latam
```

Cada tienda dispone de su propio archivo CSV que es cargado directamente desde GitHub usando `pd.read_csv(url)`.

---

## 🚀 Cómo ejecutar

1. Abre el notebook `Challenge - AluraStore.ipynb` en **Google Colab** (o Jupyter).
2. Ejecuta las celdas en orden, comenzando por la importación de datos.
3. No es necesario descargar los archivos CSV: se cargan automáticamente desde el repositorio de Alura.

---
