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

En el caso de Correos los 3 siguientes dígitos a los que llamaremos XRR son un identificador de una ruta postal, que no se genera con ningún criterio de población o extensión. Sólo busca optimizar la ruta que recorre el cartero cuando hace el reparto.

En cambio el INE utiliza los dígitos MMM para identificar los municipios. Esto supone que el 28015 puede correspondes a:

- Un código postal de madrid capital.
- Un código INE que corresponde a un municipio de la provincia de Madrid.

Es decir, correos utiliza PPXRR y el INE, si nos limitamos a la parte municipal de su codificación utiliza PPMMM.

Por cierto, históricamente el dígito X de correos tomaba el valor 0 en las capitales de provincia y 1, 2, 3... en el resto. Por eso el Código Postal 28015 tiene que estar situado en Madrid capital.


## Proyecto de QGIS

Próximamente subiré un proyecto en Qgis, un software cartográfico open source, donde acceder tanto a la geometría de las secciones censales como a diferentes indicadores.

Puedes instalar Qgis desde [este enlace][Qgis download].

[Qgis download]: https://www.qgis.org/es/site/forusers/download.html

## Fuentes:

Puedes descargar la información de las secciones censales directamente desde la [web del INE aquí][SC].

El callejero lo puedes obtener en la misma [web del INE aquí][SC].

[SC]: https://www.ine.es/ss/Satellite?L=es_ES&c=Page&cid=1259952026632&p=1259952026632&pagename=ProductosYServicios%2FPYSLayout

La renta por sección censal está disponible como estadística experimental en esta [otra web del INE][Atlas renta].

[Atlas renta]: https://www.ine.es/experimental/experimental.htm

Los datos del censo de 2011 los puedes descargar en [otra página más del INE][Censo].

[Censo]: https://www.ine.es/censos2011_datos/cen11_datos_microdatos.htm


