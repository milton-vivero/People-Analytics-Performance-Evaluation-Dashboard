## 🎯 Impacto en el Negocio y Toma de Decisiones

Este dashboard no solo muestra métricas; transforma los datos de Talento Humano en decisiones estratégicas para la empresa:

*   **Optimización de Costos de Planilla:** Permite a la dirección financiera identificar de forma inmediata qué departamentos consumen la mayor parte del presupuesto operativo y cruzarlo con sus resultados de desempeño.
*   **Estrategia de Retención de Talento:** Al analizar la **Tasa de Ausencia** y el **Porcentaje de Personal Insatisfecho**, el equipo de Recursos Humanos puede diseñar planes de bienestar enfocados en los departamentos más críticos para reducir la rotación laboral.
*   **Auditoría de Desempeño y Capacitación:** Las tarjetas de **Promedio de Evaluación** segmentadas por departamento ayudan a detectar qué equipos necesitan programas de entrenamiento técnico inmediatos para elevar su productividad.

---

## 🛠️ Fórmulas y Lógica DAX Utilizada

Para garantizar la precisión de los indicadores empresariales mostrados en el reporte, se estructuraron las siguientes medidas y cálculos personalizados:

*   **Tiempo Promedio en el Cargo:** 
    `Tiempo en el Cargo (Años) = DIVIDE(SUM(Colaboradores[Años_Puesto]), [Total de Colaboradores])`
*   **Tasa de Ausentismo Global:** 
    `Tasa de Ausencia = DIVIDE([Total_Horas_Ausentismo], [Total_Horas_Planificadas])`
