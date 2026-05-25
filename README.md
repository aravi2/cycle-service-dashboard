# Cycle Service Status Viewer Dashboard

An interactive, browser-based dashboard for tracking **PJM Generation Interconnection Cycle projects** (TC1 & TC2) — built as a personal tool to make sense of the PJM queue data without needing any software beyond a web browser.

🔗 **Live Demo:** [aravi2.github.io/cycle-service-dashboard](https://aravi2.github.io/cycle-service-dashboard)

---

## What It Does

Load any Excel export from PJM's [Cycle Service Request Status page](https://www.pjm.com/planning/m/cycle-service-request-status) and instantly get an interactive view of the interconnection queue across four tabs:

| Tab | Description |
|-----|-------------|
| 📊 Cycle Overview | Stage pipeline, status distribution, fuel mix, and stage attrition funnel |
| 🏢 TO Focus | Deep-dive into a selected Transmission Owner's project portfolio |
| ⚖️ TO Comparison | Side-by-side benchmarking across Transmission Owners |
| 📋 Project Table | Searchable, sortable full project list |

### Key Features

- **No server, no install** — just open the HTML file in any browser; no data leaves your machine
- **Cycle filter** — toggle between TC1 and TC2 cycles
- **Fuel mix charts** — Solar, Solar+Storage, Storage, Wind, Gas, Other breakdowns
- **Stage attrition funnel** — visualize how projects move (or drop) through the interconnection stages
- **TO Focus** — stage breakdown, fuel mix, and comparison vs. cycle average for any Transmission Owner

---

## How to Use

1. Open the [live dashboard](https://aravi2.github.io/cycle-service-dashboard) or download `index.html` and open it locally
2. Go to [pjm.com/planning/m/cycle-service-request-status](https://www.pjm.com/planning/m/cycle-service-request-status)
3. Set **Project Type** filter to *Generation Interconnection*, then click **Full Export → XLS**
4. Click **Load Excel** in the dashboard and select the downloaded file — charts populate instantly

---

## Data Source

All data comes from PJM's public **Cycle Service Request Status** page — no login required, updated periodically by PJM as projects progress through the interconnection queue.

---

## Built With

- [SheetJS (xlsx 0.18.5)](https://sheetjs.com/) — in-browser Excel parsing
- [Chart.js 4.4.1](https://www.chartjs.org/) — charts and visualizations
- Vanilla HTML / CSS / JS — zero build step, single file, works offline
