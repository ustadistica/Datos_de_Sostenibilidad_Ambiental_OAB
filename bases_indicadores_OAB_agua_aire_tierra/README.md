# Búsqueda de Bases de Datos de Agua para Indicadores OAB

Con el objetivo de identificar las bases de datos detrás de los indicadores de agua del Observatorio Ambiental de Bogotá (OAB), se realizaron varias búsquedas y pruebas. A continuación, se describen los casos evaluados:

## Primer caso: Indicador WQI (Water Quality Index)

Se localizó información del WQI en el portal de Datos Abiertos como dato espacial.

Las imágenes adjuntas muestran:

<img width="911" height="646" alt="Captura de pantalla 2025-09-17 a la(s) 12 59 02 a m" src="https://github.com/user-attachments/assets/69d30753-9ab0-4304-8790-f1d670ded1e9" />

Mapa de los ríos (en formato geográfico): líneas que representan los diferentes tramos de ríos monitoreados.

<img width="2048" height="1280" alt="Captura de pantalla 2025-09-17 a la(s) 12 59 24 a m" src="https://github.com/user-attachments/assets/678ffaa9-f422-48e4-9510-f418479f1ccd" />


Tabla de atributos: con columnas como “río”, “nombre”, “tramo”, fechas y valores asociados.

Sin embargo, esta información está en formato espacial (shapefile) y no corresponde al tipo de tabla consolidada requerida para la tarea (por ejemplo, series de tiempo por estación en formato tabular).

Por este motivo, se descartó esta opción para la tarea actual.

## Segundo caso: Pozos

Se revisó también la base de datos de pozos con información de monitoreo.

Al igual que con el WQI, se encontró en formato espacial (capas geográficas) y no como tabla de valores fácilmente manipulables.

Dada esta limitación, tampoco se visualizó ni se usó para la tarea.
