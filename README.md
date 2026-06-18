# MyPlantUMLGanttExtension

Ein webbasierter Gantt-Projektplaner, der **PlantUML**-Diagramme mit erweiterten Planungsfunktionen generiert.

**[English Version →](README-EN.md)**

## Überblick

Dieses Tool bietet eine interaktive Schnittstelle zum Erstellen professioneller Gantt-Diagramme, ohne PlantUML-Syntax direkt zu schreiben. Es wird als einzelne HTML-Datei mit eingebettetem JavaScript bereitgestellt und bietet Echtzeit-Diagrammrendering und Datenpersistenz.

**Hauptfunktionen:**
- 📊 **Echtzeit-Gantt-Diagramm-Generierung** – Sehen Sie Ihren Projektplan sofort, während Sie ihn erstellen
- 🎨 **Anpassbare Gestaltung** – Farbcodierte Aufgaben, verstellbare Zoomstufen, Wochenenden ausblenden
- 📅 **Feiertags- und Schließtags-Unterstützung** – Markieren Sie automatisch arbeitsfrei Tage
- 🔗 **Aufgabenabhängigkeiten** – Verknüpfen Sie Aufgaben sequenziell mit automatischen Datumsberechnungen
- 🎯 **Meilenstein-Unterstützung** – Markieren Sie wichtige Projektereignisse
- 💾 **Datenpersistenz** – Browser-Speicher speichert Ihren Projektzustand
- 📤 **Exportieren/Importieren** – Zwischenablagen-Integration für einfaches Datensharing
- 🖼️ **SVG-Export** – Laden Sie Diagramme als skalierbare Vektorgrafiken herunter

## So funktioniert es

1. **Konfigurieren Sie Ihr Projekt**
   - Legen Sie Projekttitel und Startdatum fest
   - Definieren Sie Feiertage/Schließtage
   - Wählen Sie die Diagramm-Skalierung (täglich, wöchentlich, monatlich)

2. **Fügen Sie Aufgaben hinzu**
   - Aufgabenname, Start-/Enddatum
   - Verknüpfen Sie Aufgaben über Abhängigkeiten
   - Weisen Sie Farben und Meilenstein-Marker zu
   - Sortieren Sie mit Hoch-/Runter-Schaltflächen

3. **Generieren und Exportieren**
   - UML-Quellcode aktualisiert sich live
   - Diagramm wird automatisch gerendert
   - Exportieren Sie als SVG oder kopieren Sie Daten in die Zwischenablage

## Unterstützte Skalierungen

- **Täglich (Kompakt)** – 1x Zoom, kompakte Ansicht
- **Täglich (Standard)** – 2x Zoom, Standard-Detailstufe
- **Täglich (Detailliert)** – 4x Zoom, maximale Granularität
- **Wöchentlich** – 2x Zoom, Wochenübersicht
- **Monatlich** – 4x Zoom, Übersichts-Roadmap

## Technische Details

- **Frontend:** Vanilla JavaScript (ES6 Module)
- **Rendering:** PlantUML via `plantuml.js` Modul
- **Styling:** CSS3 mit responsivem Grid-Layout
- **Speicher:** Browser LocalStorage für Datenwiedervergabe
- **Sprache:** Deutsche UI-Labels (leicht anpassbar)

## Dateistruktur

```
MyPlantUMLGanttExtension/
├── index.html          # Hauptanwendung
├── plantuml.js         # PlantUML Rendering-Engine
├── viz-global.js       # Visualisierungsbibliothek
├── README.md           # Diese Datei (Deutsch)
└── README-EN.md        # English Version
```

## Verwendung

1. Öffnen Sie `index.html` in einem modernen Webbrowser
2. Füllen Sie die Projektdetails im linken Bereich aus
3. Fügen Sie Aufgaben hinzu und konfigurieren Sie Abhängigkeiten
4. Sehen Sie das generierte Gantt-Diagramm in Echtzeit
5. Exportieren Sie als SVG oder kopieren Sie Daten in die Zwischenablage

### Datumsformat

- **Eingabe:** ISO-Format (YYYY-MM-DD) via Datepicker
- **Anzeige:** Deutsches Format (DD.MM.YYYY)
- **Feiertage:** Komma-getrennte DD.MM.YYYY-Liste

## Mitwirkende und Lizenz

Dieses Projekt verwendet **PlantUML** für die Diagrammrenderei:
- **PlantUML Projekt:** [plantuml.com](https://plantuml.com)
- PlantUML wird unter der **GPL v3 Lizenz** veröffentlicht
- Diese Erweiterung wendet kleine Änderungen an, um die Integration mit der Weboberfläche zu ermöglichen

Dieses Projekt respektiert die ursprüngliche PlantUML-Lizenz und behält die Kompatibilität mit dem GPL-Ökosystem.

---

**Gebaut mit ❤️ und absolut vibe-coded.** ✨
