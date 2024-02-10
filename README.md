Code to convert BGT (https://nl.wikipedia.org/wiki/Basisregistratie_Grootschalige_Topografie) to seperate gpkg-files concerning Street furniture (dutch: straatmeubilair)

step 1: download https://www.pdok.nl/downloadviewer/-/article/basisregistratie-grootschalige-topografie-bgt-  , Deel NL, citygml, Met plaatsbepalingspunten 
step2: convert gml to gpg in WGIS: bgt_straatmeubilair.gml --> QGIS --> bgt_straatmeubilair.gpkg
step 3: run bgt.dms in GeoDMS 14.8.0 (https://github.com/ObjectVision/GeoDMS/releases/tag/v14.8.0)
step 4: export container items: /bank/geometry , /picknicktafel/geometry , /openbaartoilet/geometry , /speelvoorziening/geometry to gpkg format with gdal lib
