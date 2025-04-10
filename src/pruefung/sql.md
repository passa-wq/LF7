# [SQL](https://www.w3schools.com/sql)

## [Normalisierung](https://de.wikipedia.org/wiki/Normalisierung_(Datenbank))

Ziel: Konsistenzerhöhung durch Redundanzvermeidung


### [Erste Normalform (1NF)](https://de.wikipedia.org/wiki/Normalisierung_(Datenbank)#Erste_Normalform_(1NF))

Jedes Attribut der Relation muss einen **atomaren Wertebereich** haben, und die Relation muss **frei von Wiederholungsgruppen** sein

> Lösung: atomare Attributwertebereiche
* Felder (Spalten) mit zusammengesetzten Typen aufspalten -> atomaren Wertebereich
* -> Aus Datenbankeinträgen mit Listen (Wiederholungsgruppen) können mehrere Einträge werden


### [Zweite Normalform (2NF)](https://de.wikipedia.org/wiki/Normalisierung_(Datenbank)#Zweite_Normalform_(2NF))

Nichtschlüsselattribute müssen von **allen** Schlüsseln vollständig abhängen

> Lösung: Tabellen aufteilen


### [Dritte Normalform (3NF)](https://de.wikipedia.org/wiki/Normalisierung_(Datenbank)#Dritte_Normalform_(3NF))

Keine funktionalen Abhängigkeiten der Nichtschlüssel-Attribute untereinander (transitive Abhängigkeiten)

> Lösung: Tabellen weiter aufteilen
