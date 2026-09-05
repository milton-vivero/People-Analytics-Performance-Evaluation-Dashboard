# People Analytics: Talent Performance & Compensation Insights 📊🇨🇴

Este repositorio contiene un dashboard ejecutivo de **People Analytics** desarrollado en **Power BI Desktop**, enfocado en la auditoría del rendimiento laboral, equidad salarial y distribución demográfica de una plantilla de 194 colaboradores.

## 🛠️ Pipeline de Transformación de Datos (Data Engineering)
El dataset original requirió un proceso exhaustivo de normalización y modelado de datos para alinearlo a las estructuras demográficas y financieras del mercado real:
* **Normalización Demográfica:** Se implementó una reestructuración de la base de datos para garantizar la diversidad del personal, aplicando un pool de 134 apellidos únicos en formato corporativo (`Apellidos, Nombres`), asegurando una distribución orgánica por departamento y eliminando sesgos de agrupación.
* **Calibración y Escala Salarial:** Se reescalaron las variables financieras a sueldos mensuales indexados en un rango estricto de **$482 a $2,000**, permitiendo un análisis preciso de la estructura de costos y compensaciones de la compañía.
* **Preservación de Historiales:** Se aseguró la integridad del modelo relacional mapeando correctamente los IDs únicos de empleado, manteniendo la coherencia en las evaluaciones y evitando la pérdida de registros históricos durante el proceso de limpieza en Power Query.

## 📊 Arquitectura del Dashboard
El reporte utiliza una interfaz corporativa optimizada (UI/UX de datos) estructurada en zonas clave:
1. **Métricas de Control (KPIs Dinámicos):** Conteo automatizado de personal (`COUNTROWS`), Promedio de Evaluación (`AVERAGE`), Porcentaje de Género exacto (`DIVIDE`) y Proyección de Horas Planificadas utilizando variables DAX avanzadas (`VAR` / `RETURN` / `COALESCE`) para mitigar valores en blanco.
2. **Auditoría de Desempeño:** Segmentación interactiva para evaluar grupos de rendimiento (*Excelente, Muy Bueno, Regular, Deficiente*).
3. **Análisis de Correlación:** Inclusión de un **Gráfico de Dispersión (Scatter Plot)** que cruza Edad vs. Salario para auditar visualmente las políticas de compensación interna.

## 🚀 Tecnologías Utilizadas
* Power BI Desktop
* DAX (Data Analysis Expressions)
* Power Query / M Language
* Python (Pandas) para la ingeniería de datos del origen
