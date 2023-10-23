# OSI Modell
(**O**pen **S**ystems **I**nterconnection `model`)

> Was ist ein Modell?
> Wofür sind Modelle wichtig?

## [7 OSI Layer](https://de.wikipedia.org/wiki/OSI-Modell#Die_sieben_Schichten)

|   | OSI-Schicht                | Einordnung           |                | TCP/IP-Referenzmodell | Protokollbeispiele    | Einheiten | Kopplungselemente |
|---|----------------------------|----------------------|----------------|-----------------------|-----------------------|-----------|-------------------|
| 7 | Anwendung (Application)    |                      |                |                       |                       |           |                   |
| 6 | Darstellung (Presentation) |                      |                |                       |                       |           |                   |
| 5 | Sitzung (Session)          | Anwendungsorientiert |                | Anwendung             |                       |           |                   |
|   |                            |                      |                |                       |                       |           |                   |
|   |                            |                      |                |                       | **HTTP**, MQTT, DHCP, DNS | Daten     |                   |
| 4 | Transport                  | Transportorientiert  |                | Transport             | **TCP**, UDP          | (TCP) Segmente, (UDP) Datagrame | |
| 3 | Vermittlung (Network)      |                      | Ende-zu-Ende   | Internet              | **IPv4**, IPv6, ICMP  | Pakete    | Router, Layer-3-Switch |
|   |                            |                      |                |                       |                       |           |                   |
|   |                            |                      |                |                       |                       |           |                   |
| 2 | Sicherung (Data Link)      |                      | Punkt-zu-Punkt | Netzzugriff           | ARP, **MAC**, IEEE 802.11 (WLAN) | Rahmen (Frames) | Bridge, Layer-2-Switch, Wireless Access Point                  |
| 1 | Bitübertragung (Physical)  |                      |                |                       | RS-232 (Serielle Schnittstelle), 1000BASE-T (**Twisted-Pair GbE**), 100GBASE-LR4 (*Glasfaser*) | Bits, Symbole | Leitungen, Stecker, Hubs, Repeater |
