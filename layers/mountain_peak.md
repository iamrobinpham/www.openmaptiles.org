---
layout: page
category: layer
title: mountain_peak
etl_graph: media/etl_mountain_peak.png
mapping_graph: media/mapping_mountain_peak.png
sql_query: SELECT osm_id, geometry, name, name_en, name_de, ele, ele_ft, rank FROM layer_mountain_peak(ST_SetSRID('BOX3D(-20037508.34 -20037508.34, 20037508.34 20037508.34)'::box3d, 3857 ), 14, 1)
---
[Natural peaks](http://wiki.openstreetmap.org/wiki/Tag:natural%3Dpeak)

## Fields

### name_de

German name `name:de` if available, otherwise `name` or `name:en`.

### name

The OSM [`name`](http://wiki.openstreetmap.org/wiki/Key:name) value of the peak.

### ele_ft

Elevation (`ele`) in feets.

### name_en

English name `name:en` if available, otherwise `name`.

### rank

Rank of the peak within one tile (starting at 1 that is the most important peak).

### ele

Elevation (`ele`) in meters.




