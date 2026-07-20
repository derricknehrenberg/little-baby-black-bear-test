# Little Baby Black Bear Test

Interactive analysis of the draft **Gunnison ↔ Crested Butte (GCB) long-distance bike route** against
OpenStreetMap, in support of the DOI/USDA long-distance bike route self-nomination
(EXPLORE Act — Bicycling on Long-Distance Trails; nominations close Aug 3, 2026).

**Live report:** the published page serves `index.html` — the current revision
(`LittleBabyBlackBear.kml`, rev. Tim Kugler / Gunnison Trails, analyzed 2026-07-20).

- `index.html` / `littlebabyblackbear-osm-analysis.html` — current revised route (126 mi)
- `gcb-osm-analysis.html` — the July 16 first draft (117 mi), kept for comparison

Each drawn route is densified to 10 m intervals and matched against all OSM `highway=*` ways in the
corridor (25 m tolerance), classifying every stretch as existing trail / 4WD track / road, or
no-OSM-match (proposed or unmapped). OSM ways sharing a name are joined into single segments.
KML source files are not published here.

## GIS exports (analyzed segments)

- `LittleBabyBlackBear-segments.kml` — styled KML, one placemark per joined segment (Google Earth / CalTopo / ArcGIS)
- `LittleBabyBlackBear-segments-shp.zip` — Shapefile, one row per segment part (WGS84; fields: name, class, section, part_mi, seg_mi, osm_ways)
- `LittleBabyBlackBear-segments-gdb.zip` — Esri File Geodatabase, layer `gcb_segments`, same schema
