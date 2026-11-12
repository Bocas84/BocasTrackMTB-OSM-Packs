# BocasTrackMTB · paquetes regionales OSM

Este directorio prepara la distribución de paquetes OSM regionales para BocasTrackMTB.

## Fuente y licencia

Los datos se obtienen de extractos públicos de [Geofabrik](https://download.geofabrik.de/europe/spain.html), derivados de OpenStreetMap. Se distribuyen bajo la [ODbL](https://www.openstreetmap.org/copyright) y deben mostrarse con la atribución **© OpenStreetMap contributors**.

## Formato previsto

Cada región tendrá un paquete de red compacta compatible con el esquema `version / center / bounds / nodes / ways` que actualmente utiliza la red local de Málaga. La app podrá descargar el paquete seleccionado y usarlo para calcular rutas sin depender de Overpass para la red de caminos.

`regions.json` enumera las comunidades autónomas y las URLs PBF de origen. El PBF es la fuente de datos; todavía no es el paquete que la app debe descargar. El catálogo público de la app se publicará cuando estén convertidos y alojados los paquetes.

## Conversión local

El conversor base está en `../extract_osm_pbf.py`. Se conserva el PBF original de España como fuente local y se generarán paquetes por región; no se incluyen aquí el PBF nacional, el código fuente de la app ni datos personales.

