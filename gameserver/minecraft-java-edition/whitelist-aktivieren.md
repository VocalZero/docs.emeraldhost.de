---
description: Whitelist auf Minecraft Server verwenden
---

# Whitelist aktivieren

### Voraussetzungen

* Zugang zum Server-Ordner (entweder über eine SFTP-Verbindung oder direkten Zugang zu den Server-Dateien)
  * Die SFTP-Zugangsdaten findest Du in der Übersicht Deines Gameservers.

### Schritte

1. Zugang zum Server-Ordner erhalten

* Wenn Du über eine SFTP-Verbindung verfügst, kannst Du Dich mit Deinen SFTP-Zugangsdaten anmelden.
* Wenn Du direkten Zugang zu den Server-Dateien hast, navigiere zu dem Verzeichnis, in dem sich der Minecraft-Server befindet.

2. Öffne die Server-Einstellungsdatei

* Die Datei "`server.properties`" befindet sich im Hauptverzeichnis des Minecraft-Servers.
* Öffne die Datei mit einem Text-Editor Deiner Wahl (z.B. Notepad, Sublime Text).

3. Aktiviere die Whitelist

* Suche nach der Zeile "`whitelist`".
* Ändere den Wert von "`false`" auf "`true`".
* Speichere die Änderungen.

4. Erstelle die Whitelist-Datei

* Im selben Verzeichnis wie die server.properties-Datei befindet sich die Datei "`whitelist.json`".
* Wenn diese Datei nicht vorhanden ist, erstelle eine neue Textdatei und nenne sie "`whitelist.json`".

5. Füge Spieler zur Whitelist hinzu

* Öffne die "`whitelist.json`"-Datei.
*   Jeder Spieler, der auf der Whitelist stehen soll, muss in einer neuen Zeile in folgendem Format hinzugefügt werden:

    ```json
    "SpielerName"
    ```
* Speichere die Änderungen.

6. Starte den Minecraft-Server neu

* Dies kann über das Webinterface oder durch Neustart des Servers erfolgen.

7. Überprüfe die Änderungen

* Verbinde Dich mit dem Server und überprüfe, ob nur die auf der Whitelist stehenden Spieler Zugang zum Server haben.

Das war's! Mit diesen Schritten solltest Du in der Lage sein, die Whitelist auf Deinem Minecraft-Server erfolgreich zu verwenden.
