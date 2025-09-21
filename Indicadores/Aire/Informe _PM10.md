# Informe sobre la disponibilidad de datos para el indicador PM10 – OAB

## Búsqueda de bases de datos de aire para indicadores OAB

Con el objetivo de identificar las bases de datos detrás de los indicadores de aire del **Observatorio Ambiental de Bogotá (OAB)**, se realizó la búsqueda y análisis del **Material Particulado Inferior a 10 Micras (PM10)**, uno de los indicadores clave de calidad del aire en la ciudad.

---

### Descripción del indicador

El **PM10** mide la concentración media de partículas en suspensión con diámetro aerodinámico menor o igual a 10 micras (PM10) en el aire ambiente de Bogotá.  
Este contaminante es relevante porque está asociado con efectos negativos en la salud humana, en particular sobre el sistema respiratorio y cardiovascular.

---

### Fórmula / cálculo del indicador

El valor se calcula a partir de los registros horarios de concentración de **PM10** generados por las estaciones de la **Red de Monitoreo de Calidad del Aire de Bogotá (RMCAB)**.  

Para que un promedio anual o del intervalo deseado sea considerado válido, se exige que al menos el **75 % de los datos esperados** en este periodo estén disponibles en la estación correspondiente.  

\[
PM10 = \frac{\sum_{i=1}^{n} C_i}{n}
\]

donde:  
- \( C_i \) = concentración horaria de PM10 (µg/m³).  
- \( n \) = número de registros horarios válidos.  

---

### Fuentes de datos

- **Red de Monitoreo de Calidad del Aire de Bogotá (RMCAB):** sistema de estaciones fijas que genera registros horarios de PM10, PM2.5, O₃, NO₂, CO, SO₂, entre otros.  
- **Datos Abiertos Bogotá:** contiene algunos indicadores procesados en formato espacial (geográfico), útiles para SIG como QGIS, pero no los registros tabulares que permiten replicar los cálculos.  
- **Portal RMCAB:** a través de la herramienta [Station Report](http://rmcab.ambientebogota.gov.co/Report/stationreport), es posible descargar los datos horarios de cada contaminante, seleccionando manualmente parámetros como estación, contaminante, fechas y formato de salida.  

---

### Situación actual

- En el **OAB** y en **Datos Abiertos Bogotá** se publican directamente los indicadores ya consolidados, pero **no están disponibles los datos crudos** en formato tabular.  
- En el portal de la **RMCAB**, los datos horarios de **PM10** sí pueden descargarse manualmente. Allí se encuentran registros actualizados **hasta julio del presente año**. No obstante, se observa que la actualización de los meses siguientes avanza lentamente, lo que puede deberse a procesos internos de validación y consolidación de la información.  

---

### Posibilidad de automatización

Dado que la descarga en RMCAB requiere ajustes manuales (tipo de datos, contaminante, fechas, formato), si se desea contar con un flujo de trabajo reproducible sería necesario implementar un proceso de **web scraping** que permita automatizar la selección de parámetros y la descarga periódica de los archivos.

---

## Conclusión

El indicador **PM10** del OAB se calcula a partir de datos horarios de la RMCAB, aplicando un promedio anual sujeto a la regla de **75 % de cobertura mínima**. Sin embargo, los datos crudos no están en OAB ni en Datos Abiertos Bogotá en formato tabular, sino únicamente en el portal de la RMCAB mediante descargas manuales.  
Aunque actualmente la información llega solo hasta julio, esto no representa una falta de datos sino un **ritmo de actualización lento**. Para garantizar actualizaciones sistemáticas y replicar el cálculo del indicador, se recomienda explorar estrategias de **automatización con web scraping** sobre el portal RMCAB.  
