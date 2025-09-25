# Automatización para Descargar Bases de Datos Anuales del Indicador PM10 en Estaciones de Bogotá

## 1) Objetivo

El propósito de este desarrollo es automatizar la descarga de bases de datos anuales correspondientes al indicador PM10 de las estaciones de monitoreo ambiental de Bogotá. La meta es obtener, para cada estación, los datos desde el 1 de enero hasta el 31 de diciembre de cada año, comenzando en 2014 y llegando hasta el año actual, sin necesidad de hacerlo manualmente en la página web.

Para ello se utiliza Selenium para controlar el navegador web y realizar, de manera programática, las acciones que normalmente haría un usuario: abrir menús desplegables, seleccionar estaciones, marcar casillas de indicadores y escribir fechas.


## 2) Tecnologías Utilizadas

Se utilizó Python como lenguaje de programación junto con la librería Selenium, que permite controlar un navegador web de forma automatizada. Selenium hace posible simular las acciones que realizaría una persona (abrir menús, hacer clic, escribir fechas, marcar casillas) dentro de la página oficial donde se encuentran los datos de calidad del aire.
También se usaron estructuras de control como bucles for para repetir de forma sistemática la misma acción sobre varias estaciones y varios años.


## 3) Descripción del Funcionamiento

Se creó una función principal llamada “main” que concentra todo el proceso.

El script inicia abriendo la página web oficial de datos de calidad del aire de Bogotá(RMCAP).

Se configuran las opciones del navegador para que se ejecute correctamente la automatización.

Selección de estaciones:
Dentro de la página, el código recorre de forma automática la lista de estaciones de monitoreo de Bogotá. Para esto se utiliza un bucle que va seleccionando cada estación una por una.

Selección del indicador PM10:
Una vez seleccionada cada estación, el script ubica la opción correspondiente al indicador PM10 y la marca para que los datos descargados correspondan a ese indicador

Introducción de fechas:
El programa también ubica los campos de fecha en la página, borra cualquier valor previo y escribe el rango de fechas correspondiente a cada año. Este rango va del 01 de enero al 31 de diciembre. El bucle se encarga de repetir este proceso desde el año 2014 hasta el año actual.

Descarga de datos:

Finalmente, después de seleccionar estación, indicador y fechas, el script activa la opción de descarga de datos. Este proceso se repite para todas las estaciones y todos los años definidos.


## 4) Beneficios del Proceso Automatizado

Ahorro de tiempo: ya no es necesario seleccionar manualmente cada estación y cada año.

Uniformidad: garantiza que todos los datos se descarguen con el mismo criterio y formato.

Escalabilidad: si en el futuro se agregan más estaciones o más años, solo se ajustan las variables en el script.




## 5) Conclusión

Gracias al uso de Selenium y Python, se diseñó un proceso que replica de manera automática y sistemática la navegación y selección que antes debía hacer un usuario manualmente.
Esta herramienta permite obtener los datos del indicador PM10 de las estaciones de Bogotá desde el 01 de enero hasta el 31 de diciembre de cada año, comenzando en 2014 y llegando hasta el año actual, ahorrando tiempo y reduciendo errores en la recolección de información.
Finalmente, después de seleccionar estación, indicador y fechas, el script activa la opción de descarga de datos. Este proceso se repite para todas las estaciones y todos los años definidos.
