# UML
(LF5)

## [Entity-Relationship-Modell (ERM)](https://de.wikipedia.org/wiki/Entity-Relationship-Modell)

* Entität (Entity)
* Eigenschaft (Attribute)
* Beziehung (Relationship)
  * Kardinalität

### Beispiel
![](https://upload.wikimedia.org/wikipedia/de/a/ab/Er-diagramm.svg)

### Aufgaben
* Herbst 2023: Aufgabe 4

## Klassendiagramm

* Klassen
* Schnittstellen (Interface)
* Attribute
* Methoden
* Sichtbarkeiten
  * **+** Public
  * **~** Package
  * **#** Protected (Zugriff durch Klasse selbst und ihre Unterklassen)
  * **-** Private
* Datentypen

* Relationen:

```mermaid
classDiagram
classA <|-- classB : Vererbung
Interface <|.. classC : Implementierung
classD -- classE : Assoziation
classF <-- classG : gerichtete Assoziation
Ganzes o-- Teil : Aggregation
Ganzes *-- Existenzabhängiges Teil : Composition
classH <.. classI : Abhängigkeit
```

* Kardinalitäten

### Beispiel
![](https://upload.wikimedia.org/wikipedia/commons/f/fe/UmlCd_Klassendiagramm-1.svg)

### Aufgaben
* Herbst 2023: Aufgabe 4

## [Anwendungsfalldiagramm (Use Case)](https://de.wikipedia.org/wiki/Anwendungsfalldiagramm)

* Akteure
* Systemgrenzen
* Anwendungsfälle
* Assoziation
* include-Beziehungen, extend-Beziehungen

### Beispiel
![](https://upload.wikimedia.org/wikipedia/commons/5/51/Uml-UseCase-Beispiel2.svg)

### Aufgaben
* Herbst 2023: Aufgabe 1

## Weitere

### Sequenzdiagramm

![](https://upload.wikimedia.org/wikipedia/commons/c/c8/UmlSequenzdiagramm-3.svg)

### [Zustandsdiagramm](https://de.wikipedia.org/wiki/Zustandsdiagramm_(UML))

![](https://upload.wikimedia.org/wikipedia/commons/2/2d/Uml-Zustandsdiagramm-6.svg)

# [Programmablaufplan (PAP)](https://de.wikipedia.org/wiki/Programmablaufplan) / Flowchart

* Start/Stop
* Operation
* Ein-/Ausgabe
* (Unterprogramm)
* Entscheidungen
* Pfeile

### Beispiel
![](https://upload.wikimedia.org/wikipedia/commons/6/6b/Flowchart_de.svg)

[![](https://imgs.xkcd.com/comics/flow_charts.png)](https://xkcd.com/518/)

[![](https://imgs.xkcd.com/comics/flowcharts.png)](https://xkcd.com/1488/)
