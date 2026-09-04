# Quicker Connect Button — 26.2 Fork

Ein clientseitiger Fabric-Mod für Minecraft 26.2, der einen frei konfigurierbaren Schnellverbindungs-Button im Hauptmenü bereitstellt.

Diese Version wird als eigenständiger Fork von [JamCoreModdings Quicker Connect Button](https://github.com/JamCoreModding/quicker-connect-button) gepflegt und auf aktuelle Minecraft-/Fabric-Versionen angepasst.

## Funktionen

- Mit einem Klick zu einem konfigurierten Server verbinden
- Button rechts neben den normalen Menü-Buttons anzeigen
- Optional den Einzelspieler-, Mehrspieler- oder Realms-Button ersetzen
- Eigener Button-Text oder automatische Übersetzung von „Connect“
- Unterstützung für Server mit Resource Packs: aktivieren, deaktivieren oder nachfragen
- Konfiguration über Mod Menu oder direkt als JSON5-Datei

## Kompatibilität

| Komponente | Version |
| --- | --- |
| Minecraft | 26.2 |
| Mod Loader | Fabric Loader 0.19.5 oder neuer |
| Fabric API | 0.159.0+26.2 oder neuer |
| Architectury API | 21.0.7 oder neuer |
| JamLib | 2.3.1+26.2.x oder neuer |
| Java | 25 oder neuer |

Der Fork wird derzeit ausschließlich für Fabric veröffentlicht und getestet. NeoForge ist in diesem Build deaktiviert.

## Installation

1. Installiere Minecraft 26.2 mit Fabric Loader.
2. Installiere [Fabric API](https://modrinth.com/mod/fabric-api), [Architectury API](https://modrinth.com/mod/architectury-api) und [JamLib](https://modrinth.com/mod/jamlib).
3. Lade die aktuelle Datei `quickerconnectbutton-fabric-*.jar` aus den [Releases](https://github.com/CelduinX/quicker-connect-button/releases) herunter.
4. Lege alle JAR-Dateien in den `mods`-Ordner deiner Minecraft-Installation.

[Mod Menu](https://modrinth.com/mod/modmenu) ist optional und ermöglicht den Zugriff auf die Konfiguration direkt im Spiel.

## Konfiguration

Mit Mod Menu lässt sich die Konfiguration grafisch bearbeiten. Alternativ kann `config/quickerconnectbutton.json5` manuell angepasst werden:

```json5
{
  // Leer lassen, um den Schnellverbindungs-Button zu deaktivieren
  ip: "play.example.net",

  // Port zwischen 0 und 65535
  port: 25565,

  // RIGHT, REPLACE_MULTIPLAYER_BUTTON, REPLACE_SINGLEPLAYER_BUTTON oder REPLACE_REALMS_BUTTON
  buttonLocation: "RIGHT",

  // Leer lassen, um den Standardtext „Connect“ zu verwenden
  text: "",

  // ENABLED, DISABLED oder PROMPT
  resourcePackBehaviour: "PROMPT"
}
```

Die Datei wird beim Start automatisch angelegt, sobald die Mod geladen wurde.

## Entwicklung

Voraussetzungen:

- JDK 25
- Internetzugriff zum Auflösen der Gradle- und Minecraft-Abhängigkeiten

Fabric-JAR bauen:

```powershell
./gradlew.bat :fabric:build
```

Die fertigen Dateien liegen anschließend in `fabric/build/libs/`.

## Links

- [Releases](https://github.com/CelduinX/quicker-connect-button/releases)
- [Issues](https://github.com/CelduinX/quicker-connect-button/issues)
- [Quellcode](https://github.com/CelduinX/quicker-connect-button)
- [Originalprojekt](https://github.com/JamCoreModding/quicker-connect-button)

## Credits und Lizenz

Die ursprüngliche Mod stammt von [JamCoreModding](https://github.com/JamCoreModding). Dieser Fork steht weiterhin unter der [MIT-Lizenz](LICENSE).
