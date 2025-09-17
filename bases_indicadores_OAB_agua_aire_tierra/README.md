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

## Teecer paso: Consumo Residencial de Agua por Habitante (CRAPH)

Para este indicador se identificó que los datos provienen de tres entidades:

Departamento Administrativo Nacional de Estadística (DANE) – Censo 2018

Secretaría Distrital de Planeación (SDP) – Proyecciones y retroproyecciones de población

Empresa de Acueducto y Alcantarillado de Bogotá (EAAB)

De la Secretaría Distrital de Planeación se consiguió la base “Proyecciones y retroproyecciones de Población (2005–2035)”, disponible en Datos Abiertos Bogotá.
Se realizó la suma de los totales de cabeceras municipales por año para obtener el valor que en el indicador aparece como PUT (Población Urbana Total). Sin embargo, al comparar este valor predicho con el cuadro demográfico del Censo 2018 del DANE, se encontró que existe discrepancia (el valor predicho es erróneo frente al censo).

Adjunto link de la base de datos utilizada para el PUT

https://datosabiertos.bogota.gov.co/dataset/proyecciones-y-retroproyecciones-de-poblacion-2005-2035


Situación actual del TACR

No se logró conseguir directamente el TACR (Total de agua consumida para uso residencial en el área urbana) en ninguna base abierta. Se plantea que el OAB pudo haberlo calculado como multiplicación de dos valores (por ejemplo, consumo per cápita × población), pero esto es solo una hipótesis.
Para aclarar este punto se recomienda enviar un correo al OAB solicitando la metodología exacta usada para derivar el TACR, ya que sin esa información no se tienen completamente los datos detrás del indicador CRAPH.

#### Correo redactado:

Asunto: Solicitud de información sobre el cálculo del indicador TACR

Estimados/as responsables del Observatorio Ambiental de Bogotá,

Reciban un cordial saludo.

Somos un grupo de estudiantes de la Facultad de Estadística de la Universidad Santo Tomás, de la asignatura Consultoría e Investigación. Como parte de un trabajo académico estamos analizando los indicadores de agua publicados por el OAB, en particular el Consumo Residencial de Agua por Habitante (CRAPH).

Al revisar las fuentes de datos identificamos las entidades de origen (DANE, SDP y EAAB) y logramos ubicar las proyecciones de población en Datos Abiertos Bogotá. Sin embargo, no hemos podido encontrar la base que respalde directamente el valor del TACR (Total de Agua Consumida para Uso Residencial en el Área Urbana) reportado en el indicador.

Por lo anterior, quisiéramos amablemente solicitarles:

Que nos indiquen cuál es la metodología utilizada para calcular el TACR.

En caso de ser posible, que nos orienten sobre la fuente o bases de datos específicas de donde se obtiene el volumen total de agua consumida para uso residencial en el área urbana.

Esta información nos permitirá comprender de forma correcta el proceso de construcción del indicador, con fines estrictamente académicos.

Agradecemos de antemano su atención y colaboración.

Atentamente,

Facultad de Estadística – Universidad Santo Tomás


