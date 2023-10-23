# Schnittstellen

## Mensch — Cyber — Physik ???

### „Aus CPS-Sicht“

HCI vs M2M vs CPS

```mermaid
flowchart LR
  Mensch <--HCI--> Cyber
  subgraph CPS[Cyber-physisches System]
    subgraph Cyber[Cyber System]
      Maschine1 <--M2M--> Maschine2
    end
    subgraph PS[Physisches System]
      subgraph Schnittstelle
        Aktuator
        Sensor
      end
      subgraph Industrie[Industrie 2.0]
        Maschine0.1
        Maschine0.2
      end
      subgraph Welt[Rest der Welt]
        Materie([Materie])
        Energie([Energie])
      end
    end
    PS --messen--> Cyber
    Cyber --ansteuern--> PS
  end
  Mensch <-..-> PS
```

#### HCI
(**H**uman–**c**omputer **i**nteraction / **H**uman-**c**omputer **I**nterface)

-> **M**ensch-**M**aschine-**I**nteraktion / Benutzerschnittstelle

#### M2M
(Machine-to-Machine)

#### CPS
(**C**yber-**p**hysical **s**ystem)

#### [„Industrie 4.0“](https://de.wikipedia.org/wiki/Industrie_4.0)
1. industrielle Revolution bestand in der Mechanisierung mittels Wasser- und Dampfkraft
2. industrielle Revolution geprägt durch Massenfertigung mit Hilfe von Fließbändern und elektrischer Energie
3. industrielle Revolution oder digitale Revolution mit Einsatz von Elektronik und IT (v. a. die speicherprogrammierbare Steuerung und die CNC-Maschine)
4. industrielle Revolution: [Smart Factory](https://de.wikipedia.org/wiki/Smart_Factory) und [**I**ndustrial **i**nternet **o**f **t**hings](https://en.wikipedia.org/wiki/Industrial_internet_of_things)

![IIoT](https://upload.wikimedia.org/wikipedia/commons/d/d9/IIoT_Architecture.png)

### „Aus Sicht der Physik“

```mermaid
flowchart LR
  subgraph PS[Physisches System]
    subgraph Welt[Welt]
      subgraph Materie[Materie]
        subgraph IT-System
          Maschine1 <-..-> Maschine2
        end
        Mensch
        Maschine1 <-..-> Mensch
        Maschine2 <-..-> Mensch
      end
      Energie([Energie])
    end
    Energie([Energie]) <-..-> Materie([Materie])
    Regeln{{Physikalische Großen und Regeln}}
    Regeln --> Energie
    Regeln --> Mensch
    Regeln --> Maschine1
    Regeln --> Maschine2
  end
```

### „Aus Sicht eines [Prozessors](https://de.wikipedia.org/wiki/Prozessor#Verarbeitung_eines_einzelnen_Befehls)“
(**Rechnerarchitektur** / **Prozessorarchitektur**)

#### stark vereinfacht

```mermaid
flowchart TB
subgraph Welt
  subgraph Computersystem
    Arbeitsspeicher
    subgraph Devices
      subgraph Peripherie
        Speichermedien
        Netzwerkkarten
        HID[Human Interface Device]
      end
      Controller
      Koprozessoren
    end
    subgraph Prozessor
      Bus <--> Register
      Bus <--> Rechenwerk <--> Register
      Bus <--> Steuerwerk <--> Register
      Steuerwerk <--> Rechenwerk
    end
  end
  Arbeitsspeicher <--> Bus
  Devices <--> Bus
end
```

[![cpu](https://upload.wikimedia.org/wikipedia/commons/3/3a/ABasicComputer.svg)](https://en.wikipedia.org/wiki/Central_processing_unit#Structure_and_implementation)

#### detailierter

```mermaid
flowchart TB
  subgraph Motherboard[Motherboard / SoC]
    Arbeitsspeicher <--MMU--> Northbridge
    subgraph CPU-Chip
      Northbridge <--FSB--> Bus
      subgraph Prozessor-Kern
        Bus <--> Register
        Bus <--> Rechenwerk <--> Register
        Bus <--> Steuerwerk <--> Register
        Steuerwerk <--> Rechenwerk
      end
    end
    Northbridge <--DMI-->  Southbridge
  end
  subgraph Welt[Rest der Welt]
    subgraph Devices
      Device1
      Device2
      Device3
    end
  end
  Southbridge <--MMIO-->Device1 
  Southbridge <--PMIO--> Device2
  Register <--GPIO--> Device3
```

##### [SoC](https://de.wikipedia.org/wiki/System-on-a-Chip)
(**S**ystem-**o**n-a-**C**hip)

##### [FSB](https://de.wikipedia.org/wiki/Front_Side_Bus)
(**F**ront **S**ide **B**us)

##### [DMI](https://de.wikipedia.org/wiki/Direct_Media_Interface)
(**D**irect **M**edia **I**nterface)

##### [MMU](https://de.wikipedia.org/wiki/Memory_Management_Unit)
(**M**emory **M**anagement **U**nit)

##### [MMIO](https://de.wikipedia.org/wiki/Memory_Mapped_I/O)
(**M**emory-**m**apped **I**/**O**)

##### [PMIO](https://de.wikipedia.org/wiki/Memory_Mapped_I/O)
(**P**ort-**m**apped **I**/**O**)

##### [GPIO](https://de.wikipedia.org/wiki/GPIO)
(**G**eneral **P**urpose **I**nput/**O**utput)

[![cpu](https://upload.wikimedia.org/wikipedia/commons/2/2c/Proz1-d.png)](https://de.wikipedia.org/wiki/Prozessor#Verarbeitung_eines_einzelnen_Befehls)

#### [Von-Neumann-Zyklus](https://de.wikipedia.org/wiki/Von-Neumann-Zyklus)
1. `FETCH` (Befehlsabruf):
    * Nächsten Befehl (entsprechend Adresse im Befehlszähler) aus Arbeitsspeicher in das Befehlsregister laden und Befehlszähler inkrementieren
2. `DECODE`(Dekodierung):
    * Der Befehl wird durch das Steuerwerk in Schaltinstruktionen für das Rechenwerk aufgelöst
3. `FETCH OPERANDS`(Operandenabruf):
    * Operanden werden aus dem Speicher laden
4. `EXECUTE` (Befehlsausführung):
    * Arithmetische oder logische Operation wird vom Rechenwerk berechnet. *(Bei Sprungbefehlen und erfüllter Sprungbedingung wird der Befehlszähler angepasst)*
5. `WRITE BACK` (Rückschreiben des Resultats): Ergebnis der Berechnung wird in den Speicher zurückgeschrieben *(falls nötig)*



> Was ist die „richtige“ Sichtweise?
