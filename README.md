# 📊 Control de Desempeño y Rendimiento Laboral — Periodo 2023

> Dashboard interactivo desarrollado en **Power BI** para el monitoreo integral del desempeño, evaluación y productividad del talento humano.

---

## 🎯 Objetivo

Proporcionar una visión consolidada y dinámica del rendimiento de los colaboradores, permitiendo a los líderes y el área de Recursos Humanos tomar decisiones basadas en datos sobre:

- Distribución del talento por departamento y género.
- Niveles de desempeño individual y grupal.
- Carga horaria planificada vs. resultados cuantitativos.

---

## 📸 Vista del Dashboard

<img width="768" height="433" alt="image" src="https://github.com/user-attachments/assets/235a1206-5ae7-4387-90ca-df87fe650464" />


---

## 🏆 KPIs Principales

| Indicador | Valor | Descripción |
| --- | --- | --- |
| **Total de Colaboradores** | 187 | Número total de empleados activos en el periodo. |
| **Promedio de Evaluación** | 91,59 | Puntuación media del desempeño general. |
| **% Mujeres** | 55,08% | Participación femenina en la plantilla. |
| **% Varones** | 44,92% | Participación masculina en la plantilla. |
| **Total de Horas Planificadas** | 37 mil | Horas asignadas a los proyectos y operaciones. |

---

## 📁 Estructura de Datos

### Tabla: `Colaboradores`

| Campo | Tipo | Descripción |
| --- | --- | --- |
| `ID Empleado` | Entero | Identificador único del colaborador. |
| `Nombre Empleado` | Texto | Nombre completo (Apellido Paterno, Apellido Materno, Nombres). |
| `Edad` | Entero | Edad del colaborador. |
| `Género` | Texto | Femenino / Masculino. |
| `Departamento` | Texto | Área funcional a la que pertenece. |
| `Nombre Supervisor` | Texto | Líder directo del colaborador. |
| `Fecha Ingreso` | Fecha | Fecha de vinculación a la empresa. |
| `Salario` | Decimal | Remuneración mensual. |
| `Evaluación` | Entero | Puntuación de desempeño (0–100). |
| `Grupo de Evaluación` | Texto | Clasificación: *DEFICIENTE, BUENO, MUY BUENO, EXCELENTE*. |

---

## 📐 Medidas DAX Implementadas

- **% Mujeres** — Porcentaje de colaboradoras femeninas.
- **% Varones** — Porcentaje de colaboradores masculinos.
- **Promedio Evaluación** — Media aritmética de las puntuaciones.
- **Total de Colaboradores** — Conteo de registros activos.
- **Total de Horas Planificadas** — Suma de horas asignadas por departamento.
- **Total Mujeres / Total Varones** — Conteos absolutos por género.
- **Tiempo en el Cargo** — Antigüedad calculada desde la fecha de ingreso.
- **EvaluacionNoBlancos** — Validación de registros con evaluación registrada.

---

## 📈 Visualizaciones Incluidas

| Gráfico | Tipo | Insight |
| --- | --- | --- |
| **Resultados por Departamento** | Gráfico circular | Promedio de evaluación por departamento con % de participación. |
| **Horas Planificadas por Departamento** | Barras horizontales | Distribución de la carga horaria por área. |
| **Resultados Cuantitativos** | Barras horizontales | Cantidad de colaboradores por grupo de evaluación. |

---

## 🎛️ Filtros Interactivos

El panel lateral permite segmentar la información por:

- ✅ **Género** — Femenino / Masculino
- ✅ **Grupo de Evaluación** — DEFICIENTE, BUENO, MUY BUENO, EXCELENTE
- ✅ **Departamento** — Tecnología, Talento Humano, Servicio al Cliente, Riesgos y Cumplimiento, Operaciones, Marketing, Logística, Contabilidad, Comercial, Administración y Finanzas, Gerencia General, Compras.

> 💡 *Botón "Borrar todas las segmentaciones" para restablecer los filtros con un solo clic.*

---

## 🚀 Cómo Usar

1. Abre el archivo `.pbix` en **Power BI Desktop**.
2. Actualiza la fuente de datos apuntando a tu base de datos o archivo Excel.
3. Publica en **Power BI Service** para compartir con tu equipo.
4. Utiliza los filtros laterales para explorar los datos por segmento.

---

## 🛠️ Tecnologías Utilizadas

<p align="left">
<img src="https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI"/>
<img src="https://img.shields.io/badge/DAX-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white" alt="DAX"/>
<img src="https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white" alt="Excel"/>
</p>

---

## 👤 Autor

**Milton Vivero** — Human Resources

> *Dashboard diseñado para el área de Talento Humano con fines de control, seguimiento y toma de decisiones estratégicas.*

---

## 📄 Licencia

Este proyecto es de uso interno. Para uso comercial o distribución externa, contactar al autor.

---

<p align="center">
<i>"Los datos bien visualizados cuentan la historia que los números solos no pueden contar."</i>
</p>
