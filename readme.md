# Spaniards in Berlin

## Export stats

Data obtained from Einwohnerregisterstatistik Berlin
https://www.statistik-berlin-brandenburg.de/webapi/jsf/tableView/tableView.xhtml#

For info, check https://www.statistik-berlin-brandenburg.de/webapi/metadata/EWRBEE/EWRBEE.html

- Planungsräume as rows
- Spanien as Filter
- Stichtag (all selected) as columns

Header and tail rows deleted, so only table left, LOR (including 8 digit identifier and name) plus value per date.
Stored in
./data/Export_from_Statis_BBB_with_deleted_rows.csv

LOR |	LOR Name |	31.12.2017 |	31.12.2007 |	31.12.2008
--- | --- | --- | --- | ---
01011101 |	Stülerstraße |	81 |	37 |	31
01011102 |	Großer Tiergarten |	7 |	4 |	3
01011103 |	Lützowstraße |	31 |	27 |	27
... | ... | ... | ... | ...

## KML and KMZ files
KML file and KMZ files for Berlin have been obtained from:
- http://www.stadtentwicklung.berlin.de/planen/basisdaten_stadtentwicklung/lor/de/download.shtml
- http://www.stadtentwicklung.berlin.de/planen/basisdaten_stadtentwicklung/lor/download/LOR_KMZ_4326.zip

Lizenz: (Creative Commons)
LOR Vektordaten der Senatsverwaltung für Stadtentwicklung und Umwelt Berlin stehen unter einer Creative Commons Namensnennung 3.0 Deutschland Lizenz.

Coordinates of areas in Berlin taken from the kml file:
./data/Mapa_de_Berlin.kml

simplekml used following this tutorial
http://www.simplekml.com/en/latest/tut_point.html

Icons taken from:
http://kml4earth.appspot.com/icons.html#kml-icons

## Markers
Different colours will be used depending on number of Spaniards in each area

name | href | Number
--- | --- | ---
icon['white'] | "http://maps.google.com/mapfiles/kml/paddle/wht-blank-lv.png" | = 0
icon['yellow'] | "http://maps.google.com/mapfiles/kml/paddle/ylw-blank-lv.png" | > 0 & < 10
icon['green'] | "http://maps.google.com/mapfiles/kml/paddle/grn-blank-lv.png" | > 10 & < 100
icon['blue'] | "http://maps.google.com/mapfiles/kml/paddle/blu-blank-lv.png" | > 100

<iframe src="https://www.google.com/maps/d/embed?mid=1sCSugR5wpVfeQS_k0NDB-ihedFjxIMDS" width="640" height="480"></iframe>