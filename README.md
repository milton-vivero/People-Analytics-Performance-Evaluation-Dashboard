# People Analytics: Talent Performance & Compensation Insights 📊🇨🇴

Este repositorio contiene un dashboard ejecutivo de **People Analytics** desarrollado en **Power BI Desktop**, enfocado en la auditoría del rendimiento laboral, equidad salarial y distribución demográfica de una plantilla de 194 colaboradores.

## 🛠️ Desafío de Ingeniería y Limpieza de Datos (Data Cleansing)
El dataset original presentaba serias inconsistencias generadas por modelos de IA (clústeres artificiales de apellidos repetidos y salarios fuera de la escala real del mercado). Como Analista de Datos, apliqué un pipeline de transformación en **Python** y **Power Query** para garantizar la integridad del modelo:
* **Diversificación Demográfica Absoluta:** Se eliminó la redundancia masiva reemplazando el pool por 134 apellidos colombianos únicos (*Restrepo, Gaviria, Ospina, Betancur*), garantizando que **no existan apellidos repetidos** en la corporación.
* **Calibración Salarial Realista:** Se reescalaron los ingresos anuales a sueldos mensuales indexados en un rango estricto de **$482 a $2,000**, permitiendo un análisis de compensación limpio.
* **Integridad Referencial:** Se preservó el historial de translados y promociones mapeando correctamente los IDs únicos a sus respectivas evaluaciones sin corromper el modelo relacional.

## 📊 Arquitectura del Dashboard
El reporte utiliza una paleta corporativa morada (Purple UI) estructurada en zonas de control visual:
1. **KPIs Laterales Dinámicos:** Conteo automatizado de personal (`COUNTROWS`), Promedio de Evaluación (`AVERAGE`), Porcentaje de Género exacto (`DIVIDE`) y Proyección Teórica de Horas Planificadas utilizando variables DAX (`VAR` / `RETURN` / `COALESCE`).
2. **Análisis de Distribución:** Segmentación única para auditar grupos de desempeño (*Excelente, Muy Bueno, Regular, Deficiente*).
3. **Análisis de Correlación Avanzada:** Inclusión de un **Gráfico de Dispersión (Scatter Plot)** que cruza Edad vs. Salario para auditar la equidad de compensación interna de la empresa.

## 🚀 Tecnologías Utilizadas
* Power BI Desktop (Agosto 2026)
* DAX (Data Analysis Expressions)
* Power Query / M Language
* Python (Pandas) para la limpieza del origen de datos
