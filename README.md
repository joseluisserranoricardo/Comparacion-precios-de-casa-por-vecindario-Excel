# 🏠 Análisis Inmobiliario: Comparación de Valor por Vecindario

## 📝 Descripción del Proyecto
Este proyecto utiliza un modelo de datos avanzado en Excel para analizar el valor de mercado en diferentes zonas geográficas. Se analizó el precio de las viviendas utilizando el **Precio por Metro Cuadrado Habitable**, permitiendo una comparación justa entre propiedades de distintos tamaños.

---

## 🚀 Habilidades Técnicas Demostradas
* **Modelado de Datos Relacional:** Conexión de tablas de atributos (`test.csv`) con tablas de predicción de precios (`submission.csv`) mediante Power Pivot.
* **Cálculos Avanzados (DAX):** Creación de una medida personalizada para el cálculo dinámico de KPI de valor.
---

## 🔍 Análisis de Resultados (Insights)

### Brecha de Valor por Ubicación
El análisis revela una disparidad significativa en el valor del suelo:
* **Zonas Premium:** Vecindarios como **NridgHt** y **StoneBr** lideran el mercado con un promedio superior a **$160/m²**.
* **Zonas de Oportunidad:** Sectores como **IDOTRR** presentan los valores más bajos (~**$83/m²**), lo que representa una brecha de valor de casi el 100% basada únicamente en la ubicación.


## 🛠️ Implementación Técnica

### Medida DAX Principal
Para calcular el valor real por área, se utilizó la siguiente expresión en Power Pivot:
`Precio_m2_Habitable := DIVIDE(SUM(submission[SalePrice]), SUM(test[GrLivArea]), 0)`



---
