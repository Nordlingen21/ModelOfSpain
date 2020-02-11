# ModelOfSpain

El objetivo de este repositorio es distribuir en un formato cómodo y fácil de trabajar distintas fuentes de información públicas sobre variables socioeconómicas a nivel sección censal.

La sección censal es una delimitación geográfica que en España se utiliza para organizar las mesas electorales. Cada sección abarca unos 1.500 o 2.000 electores y se actualizan con cada convocatoria electoral. La delimitación de las secciones censales la realiza el Instituto Nacional de Estadística (INE).

Varias secciones censales se agrupan en distritos. Los distritos se agrupan en municipios y los municipios en provincias. Finalmente las provincias forman las comunidades autónomas por lo que es posible construir todas las divisiones geográficas administrativas a partir de las secciones censales.

![Renta de cada hogar por sección censal en Alcobendas](/Assets/Ejemplo.PNG)

## Nomenclatura

Las secciones censales se identifican mediante 10 dígitos con un formato PPMMMDDSSS donde:

- PP identifica cada una de las 52 provincias. Están ordenadas basándose en los nombres que se utilizaban antes del desarrollo autonómico por lo que Cantabria ocupa el lugar que correspondería alfabéticamente a Santander. Las provincias se crearon como demarcaciones electorales a imagen de los departamentos en Francia. El objetivo era que cada zona eligiera sus diputados aunque se mantuvieron bastantes peculiaridades históricas como el condado de Treviño, Villaverde o el Rincón de Ademuz.

- MMM identifica cada uno de los más de 8.000 municipios que hay en España. Los municipios tienen tamaños muy diferentes ya que tienen orígenes históricos por lo que algunos están prácticamente despoblados y otros contienen millones de habitantes.

- DD sirve para diferenciar los más de 10.000 distritos. El distrito es una unidad estadística que racionaliza los municipios ya que los municipios pequeños normalmente sólo contienen un distrito pero los grandes tienen muchos, como Madrid, donde hay 21 distritos diferentes.

- SSS finalmente identifica la sección censal, de las que hay unas 40.000 en España. Las secciones sufren modificaciones con cada elección para amoldarse a las variaciones de la población. Se busca que siempre contengan entre 1.500 y 2.000 electores. Debido a esto último la superficie de las secciones censales es muy variable. En las ciudades son muy pequeñas mientras que en zonas rurales pueden tener una gran extensión.

## Diferencia entre códigos postales y códigos de municipio.

Tanto los códigos postales que gestiona Correos como los identificadores de municipio que gestiona el INE utilizan los dos primeros dígitos para guardar la información de la provincia.

Ahí acaban las similitudes.

En el caso de Correos los 3 siguientes dígitos son un identificador de una ruta postal, que no se genera con ningún criterio de población o extensión. Sólo busca optimizar la ruta que recorre el cartero cuando hace el reparto.


## Proyecto de QGIS

##Fuentes:

Geografía de las secciones censales.

Renta por sección censal

Censo por sección censal
