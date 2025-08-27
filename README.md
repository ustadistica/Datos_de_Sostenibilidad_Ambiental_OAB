# Datos_de_Sostenibilidad_Ambiental_OAB

## 1. Introducción y Descripción general de los geoservicios del Observatorio Ambiental de Bogotá (OAB)

El Observatorio Ambiental de Bogotá (OAB) es una plataforma que recopila y organiza
diversos indicadores ambientales, facilitando el análisis del estado y la calidad del entorno
en la ciudad, así como la evaluación de los resultados de la gestión ambiental desarrollada
por el Distrito. El OAB es una herramienta digital de la Secretaría Distrital de Ambiente que
actúa como el portal oficial para la divulgación y reporte de información estadística
ambiental sobre la ciudad, manejando indicadores sobre el aire, agua, biodiversidad, suelo,
ruido ambiental, cambio climático y demás temas relacionados con la sostenibilidad. Su
objetivo principal es promover la gestión y la participación ambiental en Bogotá a través
de la divulgación de información precisa y actualizada, sirviendo como instrumento clave
para la toma de decisiones, la investigación académica, planificación urbana y participación
ciudadana al alcance de todos.


### Alcances y utilidades

•	Proporciona información básica e indicadores sobre el estado ambiental de la ciudad
y sobre la respuesta institucional a desafí¬os (metas) ambientales.

•	Genera las bases para el seguimiento y evaluación de polí¬ ticas públicas
ambientales.

•	Propicia un escenario mediante al cual la comunidad puede estar más y mejor
informada, y cualificar sus procesos de participación en la gestión ambiental.

•	Permite una interacción con la ciudadaní¬a a fin de que ésta participe proactivamente
en la generación de información ambiental y en proyectos ambientales de Bogotá
D.C.

### Tipo de información


Visores dinámicos: El Observatorio cuenta con una serie de visores geográficos que
funcionan como mapas interactivos, los cuales permiten consultar información
georeferenciada sobre aspectos ambientales de Bogotá. Por otro lado, contiene una serie
de redes de monitoreo y microsensores que aportan datos sobre el comportamiento de la
fauna y calidad de aire. Todo esto facilita la comprensión sobre las características naturales
de la ciudad, además ofrece recorridos en formato 360 que permiten explorar humedales,
parques y diferentes áreas de conservación natural.


Indicadores: El repositorio abarca diferentes indicadores ambientales que hacen
seguimiento periódicamente del estado y la gestión del ambiente, lo que permite evaluar el
estado sostenible de la ciudad. Estos indicadores se encuentran clasificados en diversas
categorías: agua, aire, biodiversidad, suelo, ruido ambiental, residuos, cambio climático y
salud ambiental; dichos indicadores están presentados en forma de gráficas y mapas
comparativos, cada uno contiene su respectiva ficha técnica, diccionario de variables,
unidades de medida, contextualización, periodicidad y fuente de información. Con esta estructura se facilita la comprensión de la información, convirtiéndose así, en una
herramienta clave para la toma de decisiones sostenibles.


Bases de datos: Es posible consultar y descargar bases de datos asociadas a los
indicadores, analizando así de donde nace la información. Estas bases contienen datos en
formatos abiertos (CSV, XLXS o WORLD jgw), lo que permite realizar análisis propios al
alcance de cualquier ciudadano. Entre los conjuntos de información se pueden encontrar
bases históricas sobre: calidad de aire, ruido ambiental, arbolado urbano, manejo de
desechos, calidad de cuerpos de agua, biodiversidad, precipitaciones, entre otros. Muchos
de los datos se encuentran con su propio análisis, ya que manejan gráficas, mapas
explicativos, investigaciones, referencias o reportes, explicando el contexto de la
información.




## Proyecto geoespacial


En el Observatorio Ambiental de Bogotá, dentro de la sección de geoservicios, aparecen principalmente tres:

1.	Visor Geográfico Ambiental (VGA) →  El Visor Geográfico Ambiental (VGA) es el núcleo de los geoservicios de la Secretaría Distrital de Ambiente y funciona como un sistema de información geográfica en línea. Facilita el acceso, consulta y análisis de más de cien capas temáticas sobre agua, aire, vegetación, arbolado urbano, áreas protegidas, calidad del suelo y eventos ambientales como incendios o disposición ilegal de residuos. Basado en software libre y alineado con IDECA, permite activar capas, explorar metadatos, descargar información, visualizar mapas en 3D, medir, imprimir mapas, añadir datos externos y realizar análisis básicos. Es una herramienta estratégica tanto para el público como para entidades distritales, gracias a su interoperabilidad con ortofotos, mapas base y servicios de geocodificación de IDECA.
   
2.	Red de Monitoreo de Fauna → La Red de Monitoreo de Fauna es un geoservicio diseñado para registrar y dar a conocer la biodiversidad presente en Bogotá. Utiliza principalmente cámaras trampa instaladas en ecosistemas estratégicos como humedales, cerros orientales y parques ecológicos. Estas cámaras capturan imágenes y videos de animales silvestres en su entorno natural, sin necesidad de intervención humana, lo que permite identificar especies nativas, migratorias o incluso algunas en riesgo de amenaza. Además de visibilizar la fauna de la ciudad, esta red busca fomentar la conciencia ciudadana sobre la importancia de conservar los hábitats urbanos y periurbanos. 
   
3.	Red de Microsensores de Calidad del Aire →la Red de Microsensores de Calidad del Aire es un geoservicio de carácter participativo que involucra a la ciudadanía en el monitoreo ambiental. Funciona a través de dispositivos pequeños, portátiles y de bajo costo llamados microsensores, que se instalan en diferentes puntos de la ciudad para medir variables como material particulado, concentración de gases contaminantes y condiciones meteorológicas. Los datos generados complementan la información de las estaciones oficiales de la Secretaría Distrital de Ambiente y ayudan a construir un panorama más detallado sobre la calidad del aire en los barrios y localidades.


## Propuesta para la construcción de series temporales con indicadores de Agua, Aire y Cambio Climático del Observatorio Ambiental de Bogotá


El Observatorio Ambiental de Bogotá (OAB) ofrece un sistema de información con más de 400 indicadores que permiten analizar la situación ambiental de la ciudad. Entre los campos más relevantes para la gestión urbana sostenible se encuentran los indicadores de Agua, Aire y Cambio Climático, los cuales son esenciales para la planificación de políticas públicas, el seguimiento de los Objetivos de Desarrollo Sostenible (ODS) y la toma de decisiones basadas en evidencia.

Sin embargo, estos indicadores suelen estar disponibles de manera fragmentada y dispersa, dificultando el análisis longitudinal y comparativo. Por ello, proponemos una estrategia metodológica para organizar y construir series temporales por cada inidicador segmentando las tres ramas temáticas, con el fin de mejorar la trazabilidad histórica y el análisis prospectivo.


### Metodología propuesta

#### Recolección de indicadores

Se seleccionarán todos los indicadores disponibles en el OAB asociados a:

Agua: calidad, disponibilidad, consumo, fuentes hídricas, saneamiento.

Aire: calidad del aire, concentraciones de material particulado, gases contaminantes.

Cambio Climático: emisiones de gases de efecto invernadero, ozono, temperaturas promedio.

#### Consolidación en bases temáticas

Para cada rama se construirá una base de datos única:

Base Agua: contendrá todos los indicadores relacionados con el recurso hídrico en formato anual, mensual o diario, según disponibilidad.

Base Aire: integrará los indicadores de calidad atmosférica, organizados por estación de monitoreo y fecha.

Base Cambio Climático: concentrará los indicadores de emisiones, en formato anual, mensual o diario, según disponibilidad.


Cada base contará con campos estandarizados:

Nombre del indicador.

Unidad de medida.

Periodicidad (diaria, mensual, anual).

Valor.


#### Construcción de series temporales

Se organizarán los indicadores en series de tiempo, alineando cronológicamente los datos para identificar:

Tendencias de largo plazo.

Ciclos estacionales.

Comportamientos anómalos o extremos.


#### Segmentación y visualización

Cada indicador por rama (Agua, Aire y Cambio Climático) tendrá su propia serie temporal consolidada.



## Conclusion

Se han presentado dos propuestas con enfoques distintos para el manejo de la pagina del Observatorio Ambiental de Bogotá. Por un lado, la consolidación de series temporales a sus indicadores segmentadas por rama (Agua, Aire y Cambio Climático), que permitiría un análisis especializado y profundo en cada ámbito. Por otro, una enseñaza de los datos geocodifcados encontrados en la la pagina, que permitira entender como funciona los datos a diferentes usuarios estadísticos de la pagina OAB.
   
Ambos proyectos representan caminos válidos y estratégicos, pero con objetivos y alcances diferentes. La decisión final dependerá de las prioridades institucionales.
En ese sentido, corresponde a los responsables del proceso definir cuál de los dos proyectos se ajusta mejor a sus necesidades y capacidades de implementación.
