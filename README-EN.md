# MyPlantUMLGanttExtension

A web-based Gantt project planner that generates **PlantUML** diagrams with advanced scheduling features.

**[Deutsche Version →](README.md)**

## Overview

This tool provides an interactive interface to create professional Gantt diagrams without writing PlantUML syntax directly. It's built as a single HTML file with embedded JavaScript, offering real-time diagram rendering and data persistence.

**Key Features:**
- 📊 **Real-time Gantt Chart Generation** – See your project timeline instantly as you build it
- 🎨 **Customizable Styling** – Color-code tasks, adjust zoom levels, hide weekends
- 📅 **Holiday & Closure Support** – Mark non-working days automatically
- 🔗 **Task Dependencies** – Link tasks sequentially with automatic date calculations
- 🎯 **Milestone Support** – Mark key project events
- 💾 **Data Persistence** – Browser storage saves your project state
- 📤 **Export/Import** – Clipboard integration for easy data sharing
- 🖼️ **SVG Export** – Download diagrams as scalable vector graphics

## How It Works

1. **Configure Your Project**
   - Set project title and start date
   - Define holidays/closure dates
   - Choose diagram scale (daily, weekly, monthly)

2. **Add Tasks**
   - Task name, start/end dates
   - Link tasks via dependencies
   - Assign colors and milestone markers
   - Reorder with up/down buttons

3. **Generate & Export**
   - UML source code updates live
   - Diagram renders automatically
   - Export as SVG or copy data to clipboard

## Supported Scales

- **Daily (Compact)** – 1x zoom, compact view
- **Daily (Standard)** – 2x zoom, default detail level
- **Daily (Detailed)** – 4x zoom, maximum granularity
- **Weekly** – 2x zoom, week-by-week overview
- **Monthly** – 4x zoom, high-level roadmap

## Technical Details

- **Frontend:** Vanilla JavaScript (ES6 modules)
- **Rendering:** PlantUML via `plantuml.js` module
- **Styling:** CSS3 with responsive grid layout
- **Storage:** Browser LocalStorage for data retention
- **Language:** German UI labels (easily customizable)

## File Structure

```
MyPlantUMLGanttExtension/
├── index.html          # Main application
├── plantuml.js         # PlantUML rendering engine
├── viz-global.js       # Visualization library
├── README.md           # German Documentation
└── README-EN.md        # English Documentation (this file)
```

## Usage

1. Open `index.html` in a modern web browser
2. Fill in project details in the left panel
3. Add tasks and configure dependencies
4. View the generated Gantt chart in real-time
5. Export as SVG or clipboard data

### Date Format

- **Input:** ISO format (YYYY-MM-DD) via date picker
- **Display:** German format (DD.MM.YYYY)
- **Holidays:** Comma-separated DD.MM.YYYY list

## Credits and License

This project uses **PlantUML** for diagram rendering:
- **PlantUML Project:** [plantuml.com](https://plantuml.com)
- PlantUML is released under the **GPL v3 license**
- This extension applies minor modifications to integrate with the web interface (maximum render size set to 16384)

This project respects the original PlantUML license and maintains compatibility with the GPL ecosystem.

---

**Built with ❤️ and absolutely vibe coded.** ✨
