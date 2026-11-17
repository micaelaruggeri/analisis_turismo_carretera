# 🏁 Turismo Carretera (1937–2026): Trayectoria, Efectividad y Hegemonías

Proyecto integrador de **Análisis y Exploración de Datos** sobre la evolución histórica del Turismo Carretera (TC) de Argentina desde su temporada inaugural en 1937 hasta 2026.

**Autora:** Lic. Micaela Leslie Ruggeri  
**Asignatura:** Prácticas Profesionalizantes — Análisis y Exploración de Datos (TP N.º 2, N.º 3 y N.º 4)

---

## 🔗 Accesos Directos

* 📊 **[Ver Dashboard Interactivo en Looker Studio](https://datastudio.google.com/reporting/a9947963-a667-49fb-96a7-52809a092520)**
* 📄 **[Ver Informe Ejecutivo Completo](https://docs.google.com/document/d/19xCgcdYFb7Ucs20VjzIEZKhsrWEfJrQKKpGW40fHwC8/edit?usp=sharing)**
* 📄 **[Ver Colab](https://colab.research.google.com/drive/1FOisoPyzhQnqMhcR2XEkenE-41SZG3uA?usp=sharing)**
  

---

## 📌 Objetivo del Proyecto

Evaluar si la obtención de campeonatos en el Turismo Carretera guarda una relación lineal con el volumen de carreras disputadas y las victorias acumuladas, analizando cómo evolucionó la competitividad de la categoría a través de sus distintas eras técnicas, qué marcas dominaron cada etapa y cuál fue el peso real de los preparadores y motoristas detrás de cada título.

---

## 🗂️ Estructura del Repositorio

* `dataset_original_tc.csv` *(raw)*: Dataset crudo extraído de los registros históricos de la ACTC y Wikipedia previo a la depuración.
* `pilotos_tc_limpio.csv`: Dataset principal depurado con 70 registros históricos (40 campeones oficiales y 30 figuras históricas destacadas sin títulos) e indicadores calculados.
* `preparadores_tc_limpio.csv`: Tabla dimensional auxiliar con el desglose individual de motoristas y chasistas asociados a cada consagración.
* `Historia_del_TC.ipynb`: Notebook de Google Colab con el proceso completo de auditoría, limpieza (ETL), ingeniería de características, análisis exploratorio y validación cruzada de métricas.
* `Historia_del_TC.pdf`: Exportación estática de las 5 páginas del dashboard de Data Studio.
* `Informe_Ejecutivo_TC.pdf`: Documento resumen con el contexto, decisiones de limpieza, hallazgos principales, diseño del dashboard y limitaciones del análisis.
---

## 🔍 Principales Hallazgos

1. **Mayor paridad competitiva en la Era Moderna:** La efectividad promedio individual de los 40 campeones históricos es del **11,54 %** (y del **12,16 %** en el período previo 1937–2009), mientras que en la *Era Moderna* (2010–2026) desciende al **7,98 %** —una caída relativa del **34,3 %**—, reflejando un escenario mucho más parejo y exigente.
2. **Trayectoria sin corona:** El análisis de dispersión permitió aislar pilotos con altísimo volumen de triunfos que nunca lograron el título, encabezados por **Fabián Acuña** (18 victorias en 278 finales) y **Marcos Ciani** (18 victorias en 132 finales).
3. **Alternancia de hegemonías por marca:** Sobre **84 campeonatos** analizados, **Ford** lidera el historial con **46 títulos (54,8 %)** seguido por **Chevrolet** con **26 (31,0 %)**, **Dodge (7)** y **Torino (5)**. Sin embargo, el corte por eras evidencia el cambio de dominio en el siglo XXI hacia Chevrolet (impulsado por Guillermo Ortelli y Agustín Canapino).
4. **Concentración técnica en preparadores clave:** El éxito mecánico se concentra en un grupo reducido de referentes históricos, liderados por **Jorge Pedersoli** (24 títulos en 10 pilotos distintos), **Hermanos Gálvez** (14), **José Miguel Herceg** (14), **Johnny Laboritto** (13) y **Alberto Canapino** (9).

---

## 🛠️ Herramientas Utilizadas

* **Python (Google Colab):** `pandas`, `numpy` para limpieza, normalización, modelado dimensional y controles de integridad.
* **Data Studio:** Diseño de dashboard multipágina con KPIs comparativos por período, gráficos de dispersión, barras apiladas y rankings.
