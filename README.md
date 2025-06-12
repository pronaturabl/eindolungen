# KURZ

 - Werkzeug "Show Map Tips" auswählen

 - Layer "Ausdolungspotenzial" auswählen

-> Mit dem Cursor über den gewünschten Abschnitt fahren.

In der Sprechblase wird ein Verweis auf allfällige Bilder in den
entsprechenden Bereichten angezeigt.


# Ausdolungspotenzial im Kanton Baselland

Rund die Hälfte aller kleineren Fliessgewässer im Kanton Baselland ist
eingedolt. Man schätzt, dass es rund 500 Kilometer Fliessgewässer
sind. Es handelt sich nicht in allen Fällen um Bäche. Manche sind auch
sogenannte Drainagen, also Entwässerungsläufe, die nicht das ganze
Jahr Wasser führen.

Pro Natura Baselland hat sich in der Aktion Gummistiefelland zum Ziel
gesetzt, möglichst viele davon wieder ans Tageslicht zu holen. Arthur
Rohrbach hat 2012 ein kantonales Inventar der eingedolten
Fliessgewässer erstellt.

Die Befunde aus letzterer Inventarisierung wurden mit dem Gewässernetz
des Kanton Baselland nach den Gewässernummern zusammengefügt und bei
allen offenen Gewässerabschnitten (mit „-“) entfernt. Zusätzlich sind
die Ausdolungsprojekte von Pro Natura Baselland im Rahmen der Aktion
„Gummistiefelland“ in den Bemerkungen festgehalten. Somit ist das
Ausdolungspotenzial spezifischer Gewässerabschnitte auf einem Layer
ersichtlich. Da Drainagen oft keine Gewässernummer besitzen, und nicht
im Kantonalen Gewässerkataster eingezeichnet sind, konnte diese
Information nicht georeferenziert werden, sind jedoch noch in der
Datei BL_Eindolungsinventar aufgeführt.

## Technische Anforderungen

 - QGIS (Long Term Release) Prizren
 - WMTS aus dem Plugin Swisslocator.



## Daten

### ProNaturaInventarEingedolteGewaesser.gpkg

Um für das Eindolungsinventar des Kantons Baselland Georeferenzen zu
setzten, wurden die Tabellen von Pro Natura mit dem Gewässerinventar
des Kantons über die Gewässernummer zusammengefügt.

Die Daten des Eindolungsinventars mit dem Prefix "PNBL_" versehen

Die Wichtigsten Attribute sind wie folgt:

| Variable                   | Legende                                                                                                                                |
|----------------------------|----------------------------------------------------------------------------------------------------------------------------------------|
| ART_VERL                   | Art des Gewässerverlaufs                                                                                                               |
| TYP_ART                    | Gewässerart                                                                                                                            |
| GEW_NR                     | Gewässernummer                                                                                                                         |
| GEMEINDE                   | Gemeindename                                                                                                                           |
| TYP_BED                    | Gewässertyp                                                                                                                            |
| TYP_VERL                   | Verlaufstyp                                                                                                                            |
| Priorität                  | Priorität zur Ausdolung und Renaturierung der Gewässer nach dem Wasserbaukonzept Basellandschaft 2021                                  |
| Länge_m                    | Länge [m] des Gewässerabschnittes                                                                                                      |
| Gew_Nr                     | Gewässernummer aus kantonalem Gewässeregister                                                                                          |
| Gew_Name                   | Gewässername                                                                                                                           |
| PNBL_l_total               | Gesamte Länge des Gewässer auf Gemeindeboden                                                                                           |
| PNBL_l_offen               | Länge [m] des Gewässers offen                                                                                                          |
| PNBL_l_offiziell_eingedolt | Länge [m] des Gewässers offiziell eingedolt                                                                                            |
| PNBL_l_inoff_eingedolt     | Länge [m] des Gewässers inoffiziell eingedolt                                                                                          |
| PNBL_mögliche Ausdolung    | Länge [m] des Gewässers, die ausgedolt werden könnte                                                                                   |
| PNBL_Parzellen             | Parzellen                                                                                                                              |
| PNBL_Ausdolungspotenzial   | Ausdolungspotenzial aus den Beobachtungen bei der Erhebung 2012 von Pro Natura Baselland.                                              |
|                            | 6 = extrem hoch                                                                                                                        |
|                            | 5 = sehr hoch                                                                                                                          |
|                            | 4 = hoch                                                                                                                               |
|                            | 3 = genügend                                                                                                                           |
|                            | 2 = mässig                                                                                                                             |
|                            | 1 = gering                                                                                                                             |
|                            | 0 = kein                                                                                                                               |
|                            | - = Ausdolung nicht möglich, da bereits offene Gewässer (als offenes Gewässer gilt: TYP_VERL alle Kategorien die nicht "eingedolt")    |
|                            | ? = Potenzial unklar, aber im Inventar                                                                                                 |
|                            | NULL = Potenzial unklar und nicht im Inventar                                                                                          |
| PNBL_Bemerkung             | Bemerkungen aus den Beobachtungen bei der Erhebung 2012 von Pro Natura Baselland. Teils nachgeführt bei bekannten Ausdolungsprojekten. |
| PNBL_Foto im Bericht       | Wenn Bilder erstellt wurden, sind sie im                                                                                               |
|                            | Dokument (Ordner Berichte) unter "Informationsblatt" zu finden. Mit Beschriftung der Gewässernummer oder der Seitenzahl                |
| PNBL_Link zu GeoView BL    |                                                                                                                                        |
| PNBL_Informationsblatt     | Dokumentname des Berichts für jede Gemeinde separat. <GEMEINDE>_Eindolungen_Bericht.doc                                                |
| PNBL_Eigentümer            |                                                                                                                                        |
| PNBL_Bewirtschafter        |                                                                                                                                        |
| PNBL_Bezirk                |                                                                                                                                        |



Weitere Erklärungen zum Gewässernetz BL sind unter https://www.geo.bl.ch/datenbeschrieb_geodatenprodukt/50_Gewaessernetz_ESRI_Shapefile.pdf
zugänglich.

## Datenquelle: BL_Eindolungesinventar.csv

ACHTUNG WIRD NICHT NACHGEPFLEGT!  

Die Daten sind hier nur der Vollständigkeit zuliebe
abgelegt. Informationen für jede Gemeinde einzeln von Arthur Rohrbach
zusammengetragen. Alle Gemeinden aneinandergehängt.

## Varia

Author*innen:

Thomas Fabbro, thomas.fabbro@pronatura.ch
Maja Pfund, majapfund@bluewin.ch
