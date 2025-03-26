# Integración de Datos - Reto Parcial

## Descripción del Proyecto

Este proyecto se centra en la **integración de datos** para la caracterización del riesgo asociado a la pérdida de productividad mensual en una empresa del sector palmicultor. Dado que la empresa cuenta con una base de datos escasa (**Datos Observados**), se empleará la integración de datos de fincas cercanas para mejorar la calidad del análisis.

## **Objetivos del Proyecto**
1. **Caracterizar el riesgo** mediante el muestreo de datos y la integración de bases de datos externas.
2. **Aplicar la Teoría de la Credibilidad** para estimar la confiabilidad en la integración de datos.
3. **Realizar estimaciones de pérdidas** con base en la Distribución de las Pérdidas (**LDA**), considerando:
   - **Frecuencia:** Número de unidades de cultivo con pérdida de productividad.
   - **Severidad:** Pérdida promedio por unidad en dinero ($).
4. **Aplicar el método de Montecarlo** para el muestreo de la distribución agregada de pérdidas con un nivel de confianza del **99,9%**.
5. **Crear un informe final en Excel** con los datos integrados en la base de Datos Observados.

## **Metodología y Técnicas Utilizadas**

### **1. Caracterización Primaria del Riesgo**
- Uso de **medidas de tendencia central y dispersión** para describir la distribución de las pérdidas:
  - Tamaño de la Muestra
  - Media
  - Varianza
  - Coeficiente de Asimetría
  - Coeficiente de Curtosis

### **2. Caracterización Empírica de las Distribuciones de Pérdidas**
- Determinación del **tipo de distribución** y **error de la muestra**.

### **3. Muestreo de la Distribución Agregada de Pérdidas**
- Uso del **método de Montecarlo** para evaluar pérdidas esperadas, no esperadas y catastróficas (**Percentil 99,9%**).
- Comparación de medidas de tendencia central **antes y después** del muestreo.

### **4. Integración de Bases de Datos con la Teoría de la Credibilidad**
- Integración de cada finca con la base de datos interna, asignando pesos según la **Teoría de la Credibilidad**.
- Evaluación de la **confiabilidad** en la integración de cada finca.

### **5. Desarrollo de Software Reutilizable**
- Creación de un procedimiento automatizado para la integración de datos cuando las estimaciones se deban realizar más de dos veces.

## **Resultados Esperados**
- Un conjunto de datos enriquecido con la integración de fuentes externas.
- Un informe en **Excel** con los datos procesados y caracterizados.
- Un procedimiento automatizado para la integración de datos en futuros análisis.

## **Requisitos Técnicos**
- **Lenguaje**: Python 3.x
- **Librerías**: `pandas`, `numpy`, `scipy`, `statsmodels`, `openpyxl`

## **Contacto**
Si tienes preguntas o comentarios, contáctanos en **juanvillamizar1503@gmail.com**


