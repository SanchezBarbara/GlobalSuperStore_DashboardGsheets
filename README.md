# 📊 Inventory & Sales Dashboard – Global Superstore (Google Sheets)

Proyecto 1 – Análisis completo de ventas, ganancias y comportamiento de productos utilizando únicamente herramientas de **Google Sheets**, como tablas dinámicas, gráficos y funciones personalizadas.

---

## 📌 **Objetivo del Proyecto**

Transformar una base de datos de ventas internacionales en un **dashboard dinámico e interactivo** que permita:

- Analizar el rendimiento comercial por categorías, subcategorías y regiones.  
- Evaluar la rentabilidad y costos a lo largo del tiempo.  
- Identificar oportunidades de mejora mediante visualización y segmentación.

---

## 🧾 **Proceso de Limpieza y Preparación de Datos**

### 📍 **Entidad principal: `Master_Global_Super_Store`**

- Se eliminaron filas totalmente vacías (N° 6, 49, 114, 147, 182, 230, 268).  
- Se filtraron los años **2011 y 2012** por no ser relevantes para el análisis actual.  
- Se eliminaron columnas irrelevantes: `Columna1`, `Columna2`, y `Record`.  
- Los encabezados fueron normalizados con formato `Camel_Snake_Case`.  
- Se agregaron comentarios aclaratorios en campos de envío.  
- Se crearon columnas nuevas:  
  - `Total_Cost`: `Unit_Cost * Quantity`  
  - `Total_Sales`: `Total_Cost + Total_Profit`  
- Se cambió la fuente a **Arial** para mejorar la legibilidad.

### 📍 **Entidad secundaria: `M1_Product`**

- Limpieza de encabezados.  
- Se eliminó hipervínculo en `Product_Name`.  
- Se agregó columna auxiliar para extraer **ID numérico** del producto y medir su frecuencia.  
- Se calculó la media de repeticiones y se aplicó **formato condicional**.

---

## 📊 **Tablas Dinámicas Generadas**

Se desarrollaron vistas dinámicas para analizar:

- Ventas por Categoría  
- Ventas por Sub-Categoría  
- Ventas por Mercado  
- Ventas por Región  
- Ventas por Año
- Ventas por Método de Envío  
- Ventas por Prioridad 
- Ventas por Segmento  

**Extras:**  
- Total de cantidad de productos (`SUM`)  
- Cantidad de órdenes (`COUNT`)  
- Venta total por país y región

---

## 📈 **Gráficos del Dashboard**

- Column charts: ventas por Categoría, Subcategoría, Región y Mercado  
- Pie chart: ventas por Segmento  
- Line charts: evolución anual de ventas y rentabilidad  
- Bar charts: distribución por zonas  
- KPI visuales: Total de Ganancia, Costos Totales, Comparativa entre años  

---

## 📍 **Insights Destacados**

- **Francia, EE.UU. y Alemania**: los países con mayor volumen de ventas  
- **Canadá y Suiza**: regiones con menor rendimiento  
- El método de envío más empleado y las prioridades de orden están claramente segmentadas  
- El uso de filtros permite detectar promedios por pedido y oportunidades de optimización  

---

## 🚀 **Navegación del Dashboard**

- Interfaz intuitiva con **botón de “Back to Home”**  
- Sugerencia: usar el navegador en **80% de zoom** para mejor visualización  
- Todos los textos y visualizaciones están en **inglés**, ya que la empresa es internacional

---

## 🛠️ **Tecnologías Usadas**

- **Google Sheets** (pivot tables, charts, conditional formatting, formulas)  
- **Global Superstore Dataset**  
- Diseño limpio, profesional y orientado a negocios

---

## 🎯 **Conclusión**

Este proyecto demuestra la capacidad de análisis y visualización profesional utilizando solo herramientas gratuitas y accesibles como Google Sheets. Ideal para entornos sin herramientas BI avanzadas, pero con necesidades reales de reporting y toma de decisiones.
