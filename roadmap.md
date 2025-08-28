# Workspace Admin

* WS neu anlegen, umbenennen, löschen, Informationen abrufen
* Survey Content hochladen
  - allgemeine Daten / root
  - Units: hier nur Coding scheme
  - (keine Booklets, unnötig)
  - Fähigkeitsskalen
    + Itemliste
    + Methode für die Ermittlung des nominalen Skalenwertes (full-credit-ratio)
    + Parameter für die Methode (frequencies der Vergleichspopulation/mapping table)
    + Ordinalskalen (mapping der Fähigkeitswerte auf Stufen --> percent-rank)
  - Parameter für Kodierung
    + Wie soll man mit Missings umgehen (Falschkodierung)

? Soll gezielt Content gelöscht/ausgetauscht werden

# Kodier-Request

* Request-Body: alle Antworten einer Person
  - alle verfügbaren Units (ID und Alias), darin jeweils Array aller Antworten 
  - diese Person soll nicht identifizierbar sein, also keine ID oder so
* Response: Fähigkeiten
  - für alle Skalen im Workspace, auch wenn keine Items dazu der Testperson vorlagen
  - nominal und ordinal, so wie möglich
* Response: Kodierte Antworten