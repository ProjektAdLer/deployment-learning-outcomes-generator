# Neue Version deployen

Im allgemeinen ist hier die [Release-Checkliste](https://wiki.projekt-adler.eu/de/Organisation/release-checkliste) gültig, analaog zu den anderen AdLer Produkten. Diese geht in vielen Punkten nochmals genauer auf Details ein.

Die folgende Liste fasst die wichtigsten Punkte zusammen:

1) Neues Release bauen
   1) Im Repo [LearningOutcomesGenerator](https://github.com/ProjektAdLer/LearningOutcomesGenerator) auf Releases klicken, dann "Draf new Release"
   2) Choose a tag -> neue Versionsnummer angeben ohne weiter Zeichen (nach [semantic versioning](https://semver.org/)), dann auf "Create new tag" klicken
   3) Release Title ebenfalls auf die Versionsnummer setzen
   4) In der großen Textbox Changelog nach [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) erstellen
   5) "Publish Release" klicken
2) In diesem Repo in der Datei "docker-compose.yml" die Versionsnummer am Ende der Zeile, die mit "image" startet auf den Wert von Schritt 1.2 setzen
3) Änderung auf den Main-Branch comitten und ca 5 Minuten warten
