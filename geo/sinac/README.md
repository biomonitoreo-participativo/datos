## Conjuntos de datos
- Áreas de conservación
- Corredores biológicos

```shell
# Áreas silvestres protegidas
$ ogr2ogr \
    -makevalid \
    areas-conservacion.geojson \
    WFS:"http://geos1pne.sirefor.go.cr/wfs" "PNE:areas_conservacion"

# Corredores biológicos
$ ogr2ogr \
    -makevalid \
    corredores-biologicos.geojson \
    WFS:"http://geos1pne.sirefor.go.cr/wfs" "PNE:corredoresbiologicos"
```
