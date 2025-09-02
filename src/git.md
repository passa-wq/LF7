# Git

* [Download zu Git](https://git-scm.com/)

* [Die wichtigsten Git Befehle](https://johannesloetzsch.github.io/LF10b/versionierung.html)

* [OhMyGit — spielerisch Git lernen](https://ohmygit.org/)


## SOL-Aufgabe in ILIAS abgeben

```
Erarbeiten Sie sich die Grundlagen zu Git.

Von folgenden Subcommands sollten Sie wissen, was sie tun:

# Erstellt ein neues Git-Repository im aktuellen Ordner
git init

# Klont ein bestehendes Repository auf den lokalen Rechner
git clone

# Zeigt den aktuellen Zustand des Repositories an (geänderte Dateien etc.)
git status

# Fügt Änderungen zur Staging-Area hinzu, um sie zu committen
git add

# Zeigt die Unterschiede zwischen Arbeitsverzeichnis und Staging-Area
git diff

# Speichert die Änderungen aus der Staging-Area ins lokale Repository
git commit

 # Setzt die Datei auf den letzten Commit zurück (Änderungen verwerfen)
git restore




Empfehlung: Wenn Git für sie komplett neu ist, probieren sie zum lernen gerne die ersten Level von https://ohmygit.org/




Abgabe: Als Ergebnis wird erwartet, dass Sie zwischen folgenden beiden Aufgaben auswählen:




Variante 1:

a) erstellen Sie per "git init" ein neues git Repository

b) legen Sie die Dateien aus ihrem Arduine-Projekt in dem Repository ab

c) wählen Sie die Daten zum commit aus ("git add") und erstellen Sie einen commit

d) ändern Sie Dateien oder fügen Sie neue Dateien (z.B. eine README.md) hinzu

e) erstellen Sie einen zweiten commit mit den Änderungen

f) versuchen Sie Ihr git Repository auf einen Git-Server (z.B. https://github.com oder https://gitlab.com) hochzuladen. Wenn Sie erfolgreich sind, reicht als Abgabe ein Link

g) falls Sie mit f) nicht erfolgreich waren, erzeugen Sie ein zip-Archiv des Repositories und laden Sie dieses als Abgabe hoch

 

Variante 2:

a) erstellen Sie einen Github-Account (wenn Sie noch keinen haben)

b) forken Sie mein repository https://github.com/johannesloetzsch/LF7

c) clonen Sie ihren Fork auf ihren Computer

d) editieren Sie mindestens eine Datei (beheben Sie z.B. einen Tipp-/Rechtschreibfehler oder fügen sie zu einem Thema ergänzende Informationen wie einen nützlichen Link oder den Vorschlag einer Definition eines Begriffes hinzu)

e) commiten und pushen Sie die Änderungen

f) stellen Sie mir einen Pull-Request (das reicht als Abgabe)
```

SOL - Definition Musterlösung

```
git init - Initialisiert ein neues lokales und leeres Git-Repository.

git clone - Klont ein Repository in ein neues Verzeichnis. Dieses muss/wird mit der URL des Repositorys angegeben.

git status - Zeigt den Status des Arbeitsverzeichnisses und des Staging-Bereichs an. Es zeigt an, welche Dateien geändert wurden, welche Dateien zum Staging-Bereich hinzugefügt wurden und welche Dateien im Staging-Bereich sind.

git add - Fügt Dateien zum Staging-Bereich hinzu. Es gibt verschiedene Möglichkeiten, Dateien hinzuzufügen.

git diff - Zeigt die Unterschiede zwischen zwei Commits, zwischen einem Commit und dem Arbeitsverzeichnis oder zwischen zwei Branches an.

git commit - Erstellt einen neuen Commit. Dieser Commit ist nur lokal verfügbar und muss mit git push auf den Remote-Server hochgeladen werden.

git restore - Stellt Dateien aus dem Staging-Bereich oder dem letzten Commit wieder her.
```