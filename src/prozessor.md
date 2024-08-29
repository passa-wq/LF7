# Prozessoren

> SOL „Funktionsweise von Prozessoren“
>
> Erkundigen Sie sich selbstständig darüber, wie es möglich ist, mittels Maschinen zu rechnen.
> Als Einstieg wird folgendes Video empfohlen: [A Computer Built With Dominos](https://www.youtube.com/watch?v=w6E7aQnA4Ws).
>
> Beantworten Sie die folgenden Fragen:
>
> 1. Wie funktioniert das Binärsystem?
> 2. Schreiben Sie die Zahlen 0-7 als Binärzahl auf.
> 3. Benennen Sie 4 verschiedene zweistellige logische Verknüpfungen (Logikgatter).
> 4. Was ist ein Halbaddierer?
> 5. Wieviele Eingänge und wieviele Ausgänge hat ein Halbaddierer?
> 6. Zeichnen oder beschreiben Sie eine Schaltung, wie ein Halbaddierer aus einfachen Logikgattern aufgebaut werden kann.
> 7. Finden Sie Möglichkeiten, wie Logikgatter mittels Murmeln, Wasser oder in Minecraft aufgebaut werden können?


## [Transistoren](https://de.wikipedia.org/wiki/Bipolartransistor)

![npn](https://upload.wikimedia.org/wikipedia/commons/thumb/f/f4/Diagrama_de_Transistor_NPN.svg/220px-Diagrama_de_Transistor_NPN.svg.png)

![npn](https://upload.wikimedia.org/wikipedia/commons/thumb/4/49/NPN_BJT_-_Structure_%26_circuit.svg/500px-NPN_BJT_-_Structure_%26_circuit.svg.png)


## [Gatter](https://www.leisering.net/4bit_va/inhaltsverzeichnis.html#anhb)


## [Von-Neumann-Zyklus](https://de.wikipedia.org/wiki/Von-Neumann-Zyklus)

[![cpu](https://upload.wikimedia.org/wikipedia/commons/2/2c/Proz1-d.png)](https://de.wikipedia.org/wiki/Prozessor#Verarbeitung_eines_einzelnen_Befehls)

1. `FETCH` (Befehlsabruf):
    * Nächsten Befehl (entsprechend Adresse im Befehlszähler) aus Arbeitsspeicher in das Befehlsregister laden und Befehlszähler inkrementieren
2. `DECODE`(Dekodierung):
    * Der Befehl wird durch das Steuerwerk in Schaltinstruktionen für das Rechenwerk aufgelöst
3. `FETCH OPERANDS`(Operandenabruf):
    * Operanden werden aus dem Speicher laden
4. `EXECUTE` (Befehlsausführung):
    * Arithmetische oder logische Operation wird vom Rechenwerk berechnet. *(Bei Sprungbefehlen und erfüllter Sprungbedingung wird der Befehlszähler angepasst)*
5. `WRITE BACK` (Rückschreiben des Resultats): Ergebnis der Berechnung wird in den Speicher zurückgeschrieben *(falls nötig)*


