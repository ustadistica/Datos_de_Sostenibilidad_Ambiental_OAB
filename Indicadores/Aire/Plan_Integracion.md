# Plan de Integración de los 19 Indicadores de Aire – OAB

## 1. Introducción y Descripción general
El Observatorio Ambiental de Bogotá (OAB) es la plataforma oficial de la Secretaría Distrital de Ambiente para la divulgación de información estadística y geoespacial sobre el estado del ambiente en la ciudad. Dentro de sus categorías temáticas, los **indicadores de aire** constituyen una herramienta clave para evaluar la calidad del aire, su impacto en la salud pública y los avances en gestión ambiental y movilidad sostenible.

En total, el OAB dispone de **19 indicadores de aire** que abarcan desde la medición directa de contaminantes (PM10, PM2.5, SO₂, NO₂, CO, O₃), hasta indicadores de política pública y gestión (GEI, FNCE EP, VCBE, entre otros). Sin embargo, estos indicadores difieren en su **periodicidad** (mensual o anual) y en sus **años de inicio**, lo cual hace necesario un plan de integración que permita un análisis coherente y trazable.

---

## 2. Alcances y utilidades del plan
- **Consolidar información** en bases de datos temáticas que integren los 19 indicadores.  
- **Permitir comparaciones históricas**, respetando la periodicidad y fechas de inicio.  
- **Fortalecer el análisis ambiental**, tanto operativo (mensual) como estratégico (anual).  
- **Apoyar políticas públicas** mediante tableros de control diferenciados por tipo de indicador.    

---

## 3. Tipos de información a integrar
- **Series temporales mensuales**: reflejan cambios estacionales, alertas y tendencias cortas.  
- **Series temporales anuales**: permiten evaluar cumplimiento normativo y objetivos de largo plazo.  
- **Indicadores de gestión y agregados**: aportan contexto sobre mitigación, política pública y evaluación.  

---

## 4. Estrategias de integración propuestas

### 4.1. Integración por periodicidad (mensual / anual)
Esta clasificación organiza los indicadores según su frecuencia de actualización.

**Mensuales**  
- PM10PM – Promedio mensual (desde 2006/2007).  
- PM10PME – Promedio mensual por estación (desde 2014).  
- PM2.5PME – Promedio mensual por estación (≈2014-2015).  

**Anuales**  
- PM10PAE – Promedio anual por estación.  
- PM2.5PAE – Promedio anual por estación.  
- PM2.5PA – Promedio anual.  
- PM10 – Promedio anual.  
- SO₂ – Dióxido de Azufre anual.  
- NO₂ – Dióxido de Nitrógeno anual.  
- CO – Monóxido de Carbono anual.  
- O₃ – Ozono (8h) anual.  
- INGEI – Emisiones de GEI.  
- NIA – Infracciones en fuentes móviles.  
- FNCE EP – Entidades con fuentes no convencionales de energía.  
- FVPIGA – Vehículos públicos por tipo de funcionamiento.  
- VCBE – Vehículos de cero o bajas emisiones.  
- %ECPM10-OMSIII – Cumplimiento OMS en PM10.  
- %ECPM2.5-OMSIII – Cumplimiento OMS en PM2.5.  
- SEAIR – Subíndice del Estado del Aire.  


---

### 4.2. Integración por tipo de contaminante / variable ambiental
En este esquema los indicadores se agrupan según el contaminante o dimensión ambiental.

**Material particulado**  
- PM10 (PM, PAE, PMEM, PA).  
- PM2.5 (PME, PAE, PA).  
- %ECPM10-OMSIII.  
- %ECPM2.5-OMSIII.  

**Gases criterio**  
- SO₂.  
- NO₂.  
- CO.  
- O₃.  

**Gestión y movilidad**  
- INGEI.  
- NIA.  
- FNCE EP.  
- FVPIGA.  
- VCBE.  

**Agregados e índices de cumplimiento**  
- SEAIR – Subíndice del Estado del Aire.  
- %ECPM10-OMSIII.  
- %ECPM2.5-OMSIII.  


---

## 5. Metodología de construcción de las bases
1. **Recolección de datos** desde el portal OAB y visores asociados.  
2. **Estandarización**: nombre del indicador, periodicidad, unidad de medida y año de inicio.  
3. **Consolidación en bases temáticas**:  
   - Base mensual → PM10 y PM2.5.  
   - Base anual → gases criterio, GEI, gestión, SEAIR.  
4. **Construcción de series temporales** con filtros de cobertura (ej. 2006-hoy, 2014-hoy).  
5. **Visualización**: tableros dinámicos (Power BI, Tableau o R Shiny) con panel mensual y anual, además de vistas temáticas por contaminante.  

---


