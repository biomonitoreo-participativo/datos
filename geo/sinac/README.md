## Conjuntos de datos
- Áreas de conservación
- Corredores biológicos

```shell
# Áreas de conservación
$ ogr2ogr \
    -makevalid \
    areas-conservacion.geojson \
    WFS:"http://geos1pne.sirefor.go.cr/wfs" "PNE:areas_conservacion"

# Áreas de conservación con geometrías simplificadas (100 m)
$ ogr2ogr \
    -simplify 100 \
    -makevalid \
    areas-conservacion-simplificadas_100m.geojson \
    WFS:"http://geos1pne.sirefor.go.cr/wfs" "PNE:areas_conservacion"


# Corredores biológicos
$ ogr2ogr \
    -makevalid \
    corredores-biologicos.geojson \
    WFS:"http://geos1pne.sirefor.go.cr/wfs" "PNE:corredoresbiologicos"
    
# Corredores biológicos con geometrías simplificadas (100 m)
$ ogr2ogr \
    -simplify 100 \
    -makevalid \
    corredores-biologicos-simplificadas_100m.geojson \
    WFS:"http://geos1pne.sirefor.go.cr/wfs" "PNE:corredoresbiologicos"    
```
