# PJM GI Service Request Status Viewer

An interactive, browser-based dashboard for analyzing the **PJM Generation Interconnection (GI) queue** — covering both Cycle (TC1/TC2) and Serial (Legacy + Expedited) interconnection projects.

🔗 **Live Demo:** [aravi2.github.io/cycle-service-dashboard](https://aravi2.github.io/cycle-service-dashboard)

---

## What It Does

The dashboard parses an Excel export from PJM's [Cycle Service Request Status page](https://www.pjm.com/planning/m/cycle-service-request-status) and renders it across five interactive tabs:

| Tab | Description |
|-----|-------------|
| 🌐 GI Queue Overview | Portfolio-wide KPIs and fuel mix charts across all projects |
| 📊 Cycle Overview | Stage pipeline, status distribution, and attrition funnel for cycle projects |
| 🏢 TO Focus | Deep-dive into a selected Transmission Owner's project portfolio |
| ⚖️ TO Comparison | Side-by-side benchmarking across all Transmission Owners |
| 📋 Project Table | Searchable, sortable full project list |

### Key Features

- **No server required** — runs entirely in the browser; no data leaves your machine
- **Dual file support** — load both Cycle (TC1/TC2) and Serial queue Excel exports
- **Queue filter** — toggle between ALL | SERIAL | TC1 | TC2 views
- **Fuel mix charts** — Solar, Solar+Storage, Storage, Wind, Gas, Other breakdowns with MW Energy / MW Capacity toggle
- **TO Focus** — stage attrition funnel, serial queue status by type, and portfolio evolution charts
- **Info tooltips** — hover the ℹ badge on any chart title for a plain-language description

---

## How to Use

### Option A — Live (GitHub Pages)
1. Open [aravi2.github.io/cycle-service-dashboard](https://aravi2.github.io/cycle-service-dashboard)
2. Download the Cycle Excel file from [pjm.com/planning/m/cycle-service-request-status](https://www.pjm.com/planning/m/cycle-service-request-status) (Full Export → XLS, filter: Generation Interconnection)
3. Click **Load Cycle Excel** in the dashboard header and select the downloaded file
4. Optionally load a Serial queue export via **Load Serial Excel**

### Option B — Local
1. Download `index.html` from this repo (or clone it)
2. Double-click to open in any modern browser
3. Follow steps 2–4 above

---

## Data Source

All data comes from PJM's public **Cycle Service Request Status** page:
> https://www.pjm.com/planning/m/cycle-service-request-status

No login required. PJM updates this data periodically as projects progress through the interconnection queue.

---

## Archive

The `/archive` folder contains the earlier **Cycle Service Status Viewer Dashboard** — a simpler single-file version covering Cycle projects only, included for reference.

---

## Built With

- [SheetJS (xlsx 0.18.5)](https://sheetjs.com/) — in-browser Excel parsing
- [Chart.js 4.4.1](https://www.chartjs.org/) — all charts and visualizations
- [chartjs-plugin-datalabels 2.2.0](https://chartjs-plugin-datalabels.netlify.app/) — chart data labels
- Vanilla HTML/CSS/JS — zero build step, single file

---

*Developed for research use at the University of North Carolina at Charlotte.*
