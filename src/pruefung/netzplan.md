# [Netzplan](https://de.wikipedia.org/wiki/Netzplantechnik)
(LF2)

![](https://upload.wikimedia.org/wikipedia/de/1/1f/NetzplanKnoten.png)

> FAZ = frühester Anfangszeitpunkt (FB = frühester Beginn)
>
> FEZ = frühester Endzeitpunkt (FE = frühestes Ende)
>
> D = Dauer
>
> GP = Gesamtpuffer (= SAZ - FAZ oder= SEZ - FEZ)
>
> = *Zeitspanne, die ein Vorgang gegenüber seinem frühesten Beginn (bzw. Dauer) verschoben werden kann, ohne das Projektende zu gefährden*
>
> FP = freie Puffer(= FAZ des Nachfolgers - FEZ des aktuellen Vorgangs)
>
> = *Zeit, die den frühestmöglichen Beginn bzw. Ende des Nachfolgers nicht gefährdet*
>
> SAZ = spätester Anfangszeitpunkt (SB = spätester Beginn)
>
> SEZ = spätester Endzeitpunkt (SE = spätestes Ende)

![Beispiel](https://upload.wikimedia.org/wikipedia/commons/3/33/NetzplanBsp.png)

## Befüllung

1. Vorwärtsterminierung
* Sonderfall erster Vorgang: **FAZ** des **ersten Vorganges**: **0**
* **FEZ = FAZ + Dauer**
* **FAZ** = **FEZ** des **vorangegangenen Vorganges**
  * *bei mehreren Vorgängern: der höchste Wert*
2. Rückwärtsterminierung
* Sonderfall letzter Vorgang: **SEZ** des **letzten Vorganges**: **FEZ**
* **SEZ** = **SAZ** des **nachfolgenden Schrittes**
   * *bei mehreren Nachfolgern: der niedrigste Wert*
* **SAZ = SEZ - Dauer**

## Aufgaben
* Herbst 2021: Aufgabe 1
