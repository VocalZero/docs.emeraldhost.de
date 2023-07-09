---
description: Verwendung von Behavior und Resource Packs auf Minecraft Bedrock Server
---

# Behavior und Resource Packs hinzufügen

#### Voraussetzungen

* Zugang zum Server-Ordner (entweder über eine SFTP-Verbindung oder direkten Zugang zu den Server-Dateien)
  * Die SFTP-Zugangsdaten findest Du in der Übersicht Deines Gameservers.
* Ein Behavior Pack im Format .mcpack oder .mcaddon
* Texteditor (wie Notepad, Notepad++, Windows Editor oder Visual Studio Code)

#### Schritte

1. Server stoppen
2. Behavior Pack herunterladen und entpacken

* Lade ein Behavior Pack Deiner Wahl herunter und entpacke die Dateien mit einem geeigneten Programm. (wie WinRAR oder 7-Zip)

3. Behavior und Resource Packs auf den Server hochladen

* Verbinde Dich mit Deinem Server über das FTP-Tool. Lade den Behavior Pack Ordner in /behavior\_packs und den Resource Pack Ordner (falls vorhanden) in /resources\_packs hoch.

4. Server neu starten
5. Neue JSON-Dateien erstellen

* Erstelle zwei neue Dateien mit den Namen "`world_resource_packs.json`" und "`world_behavior_packs.json`".

6. Resource Pack Informationen kopieren

* Öffne im Resource Pack Ordner die Datei "manifest.json". Kopiere die UUID und Versionsnummer und füge sie in die "world\_resource\_packs.json" Datei ein. Achte auf die richtige Formatierung.

7. Behavior Pack Informationen kopieren

* Wiederhole den gleichen Vorgang für die "`world_behavior_packs.json`" Datei und den zugehörigen Behavior Pack Ordner.

8. JSON-Dateien auf den Server hochladen

* Lade beide `.json`-Dateien in den World-Unterordner auf Deinem Server hoch.

9. Server neu starten
10. Überprüfen der Änderungen

* Starte Deinen Server und stelle sicher, dass die Packs korrekt installiert sind.

Jetzt kannst Du loslegen und Spaß haben! Mit diesen Schritten solltest Du in der Lage sein, Behavior und Resource Packs auf Deinem Minecraft Bedrock Server erfolgreich zu verwenden.
