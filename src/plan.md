# Plan

## Zeitplan

```mermaid
gantt
 title LF7 + PV 2023/24
 dateFormat YYYY-MM-DD
 axisFormat %d.%m.
 section 8h Mo 23.10.
  Einführung                  :2023-10-23, 8h
 section 8h Mi 25.10.
  …                           :2023-10-25, 8h
 section 8h Do 26.10.
  …                           :2023-10-26, 8h
 section 8h Fr 27.10.
  Klassenarbeit               :milestone, 2023-10-27, 2h
  …                           :2023-10-27, 4h
  PV SOL Beispielprüfung      :2023-10-27, 2h
 section 5h Mo 27.11.
  …                           :2023-11-27, 5h
 section 6h Mi 29.11.
  …                           :2023-11-29, 6h
 section 8h Do 30.11.
  …                           :2023-11-30, 8h
 section 8h Mo 04.12.
  …                           :2023-12-04, 7h
 section 5h Di 05.12.
  …                           :2023-12-05, 5h
 section 8h Do 07.12.
  Klassenarbeit               :milestone, 2023-12-07, 2h
  …                           :2023-12-07, 6h
 section 2h Fr 08.12.
  PV SOL Beispielprüfung      :2023-12-08, 2h
 section 5h Mo 29.01.
  …                           :2024-01-29, 5h
 section 5h Di 30.01.
  …                           :2024-01-30, 5h
 section 8h Do 01.02.
  Projektabschluss            :2024-02-01, 7h
  PV Fragen                   :2024-02-01, 1h
 section 2h Fr 02.02.
  PV SOL Beispielprüfung      :2024-02-02, 2h
 section 5h Di 06.02.
  PV                          :2024-02-06, 5h
 section 2h Do 08.02.
  PV Fragen                   :2024-02-08, 2h
 section 4h Fr 09.02.
  PV                          :2024-02-09, 4h
```

## Leistungskontrollen

* Soll Notendichte: 7 
* Minimum Klassenarbeiten (>45min, doppelte Wertung): 2
* Sonstige Noten: >=3

> * **Fr 27.10. Klassenarbeit** ~90min (einseitig beschrifteter A4 Notizzettel + 1 einfacher Taschenrechner ohne Binärberechnungen)
>   * Zweierpotenzen
>   * Logische Verknüpfungen (Not, And, Or, XOr)
>     * Wahrheitswertetabelle
>     * Logik Gatter (Schaltung mit einfachen (Um-)Schaltern)
>   * Von-Neumann-Zyklus
>   * Berechnung von (Vor-)Widerständen
>   * Rechnernetze / Topologien

> * **Do 07.12. Klassenarbeit** ~90min (einseitig beschrifteter A4 Notizzettel)
>   * Grundlagen Programmierung (Variablen, While, If/Else)
>   * [Grundlagen Git](https://johannesloetzsch.github.io/linux-praktikum/versionskontrolle.html)
>   * OSI-Modell, insbesondere Physical Layer
>   * UART, I²C, SPI
>   * HTTP, MQTT

## Checkliste

### Mo 23.10.
> - [x] Dokumentation mit [hedgedoc](https://hedgedoc.c3d2.de/) und [mdBook](https://rust-lang.github.io/mdBook/)
> - [x] Git Kurzeinführung (machen wir später noch ausführlicher)
>   * [OhMyGit](https://ohmygit.org/)
> - [x] Allgemeine Infos (Unterrichtskonzept)
> - [x] Übersicht LF7 + PV
> - [x] Grundlagen CPS
> - [.] Schnittstellen
>   - [ ] Logik Gatter
>   - [ ] Von-Neumann-Zyklus

### Mi 25.10.
> - [x] Grundlagen digitaler Schaltungen
>   - [x] Logische Verknüpfungen (Not, And, Or, XOr)
>     - [x] Wahrheitswertetabelle
>     - [x] Logik Gatter (Schaltung mit einfachen (Um-)Schaltern)
>     - [x] Logik Gatter mit Resistor-Transistor-Logik
>       - [x] (Halb-)Addierer
>   - [x] Berechnung von (Vor-)Widerständen

### Do 26.10.
> - [x] Von-Neumann-Zyklus
> - [x] Rechnernetze -> Bussysteme
> - [x] Integration -> Schnittstellen
> -   [.] -> Standards

### Fr 27.10.
> - [x] Klassenarbeit
> - [x] Integration -> Schnittstellen -> Standards
> - [x] Sortieralgorithmen
> - [x] SOL: Klausuraufgabe

### Mo 27.11. + Mi 29.11.
> - [x] Einführung Raspberry Pi
> - [x] GPIO (Leds+Buttons)
> - [x] Grundlagen Programmierung

### Do 30.11.
> - [x] Vorstellung von Ergebnissen vom 29.11.
> - [x] OSI Modell
> - [x] Bitübertragung
> - [x] UART, I²C, SPI
> - [x] Vorschläge für weitere Raspberry-Projekte
> - [x] Zeit für Praxisprojekte mit Raspberry Pi

### Mo 4.12.
> - [x] HTTP, MQTT
> - [ ] [Grundlagen Git](https://johannesloetzsch.github.io/linux-praktikum/versionskontrolle.html)
> - [ ] CTF
> - [ ] Arduino?
### Di 5.12.
> - [ ] Wiederholung für Klassenarbeit
> - [ ] Zeit für Praxisprojekte
### Do 7.12.
> - [ ] Klassenarbeit
### Fr 8.12.
> - [ ] SOL: Klausuraufgabe? 
