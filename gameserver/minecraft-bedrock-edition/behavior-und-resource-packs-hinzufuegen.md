---
description: Verwendung von Behavior und Resource Packs auf Minecraft Bedrock Server
---

# Behavior und Resource Packs hinzufügen

#### Voraussetzungen

* Zugang zum Server-Ordner (über FTP-Tool wie FileZilla)
* Ein Behavior Pack im Format .mcpack oder .mcaddon
* Texteditor (wie Notepad oder Sublime Text)

#### Schritte

1. Server stoppen
2. Behavior Pack herunterladen und entpacken

* Lade ein Behavior Pack deiner Wahl herunter und entpacke die Dateien mit einem geeigneten Programm.

3. Behavior und Resource Packs auf den Server hochladen

* Verbinde dich mit deinem Server über das FTP-Tool. Lade den Behavior Pack Ordner in /behavior\_packs und den Resource Pack Ordner (falls vorhanden) in /resources\_packs hoch.

4. Server neu starten
5. Neue JSON-Dateien erstellen

* Erstelle zwei neue Dateien mit den Namen "world\_resource\_packs.json" und "world\_behavior\_packs.json".

6. Resource Pack Informationen kopieren

* Öffne im Resource Pack Ordner die Datei "manifest.json". Kopiere die UUID und Versionsnummer und füge sie in die "world\_resource\_packs.json" Datei ein. Achte auf die richtige Formatierung.

7. Behavior Pack Informationen kopieren

* Wiederhole den gleichen Vorgang für die "world\_behavior\_packs.json" Datei und den zugehörigen Behavior Pack Ordner.

8. JSON-Dateien auf den Server hochladen

* Lade beide .json-Dateien in den World-Unterordner auf deinem Server hoch.

9. Server neu starten
10. Überprüfen der Änderungen

* Starte deinen Server und stelle sicher, dass die Packs korrekt installiert sind.

Jetzt kannst du loslegen und Spaß haben! Mit diesen Schritten solltest du in der Lage sein, Behavior und Resource Packs auf deinem Minecraft-Server erfolgreich zu verwenden.
