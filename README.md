# 💧 AquaMetric — Digital Water Quality Analyser

A web-based tool for analysing water quality by comparing ion concentrations against WHO and EU drinking water standards.

🌐 **Live Demo:** [whisper278.github.io/AquaMetric/index.html](https://whisper278.github.io/AquaMetric/index.html)

---

## Background & Motivation

This project grew out of hands-on field research conducted on **Lake Dighyah** (Absheron Peninsula, Azerbaijan) — a water body with virtually no publicly available hydrochemical data.

During the study, water samples were collected and analysed using:
- **Spectrophotometry**
- **Titrimetric analysis**
- **Multiline Water Quality Meter 850081**

The research revealed significant findings:
- Sulphates and carbonates **exceeded MPC limits**
- Total hardness was **far above the norm** (11.8–13.4 meq/L vs. 7.0 meq/L limit)
- Phosphate levels were approaching the limit, indicating **eutrophication risk**

A clear gap emerged during this work: there were no accessible, practical tools to quickly evaluate water quality results and communicate them in a meaningful way. AquaMetric was built to fill that gap.

---

## About

AquaMetric is a universal water quality analysis tool that works for **any water body** — lakes, rivers, reservoirs, groundwater, or tap water. It is aimed at researchers, environmentalists, and students who need fast, reliable assessments without specialised software.

---

## Features

- ✅ Analyses **11 key water quality parameters**
- 🌍 Available in **3 languages**: English, Azerbaijani, Russian
- 📊 Compares values against **MPC (Maximum Permissible Concentration)** limits
- 🔍 Classifies water suitability for: **drinking, irrigation, industrial use, fishery**
- ⚠️ Detects **eutrophication risk**
- 💻 Runs entirely in the browser — **no installation required**

---

## Parameters Analysed

| Parameter | Formula | MPC Limit |
|---|---|---|
| Carbonates | CO₃²⁻ | ≤ 300 mg/L |
| Bicarbonates | HCO₃⁻ | ≤ 400 mg/L |
| Phosphates | PO₄³⁻ | ≤ 3.5 mg/L |
| Sulphates | SO₄²⁻ | ≤ 500 mg/L |
| Chlorides | Cl⁻ | ≤ 350 mg/L |
| Ammonium | NH₄⁺ | ≤ 0.5 mg/L |
| Nitrates | NO₃⁻ | ≤ 45 mg/L |
| Nitrites | NO₂⁻ | ≤ 3.3 mg/L |
| Total Hardness | — | ≤ 7.0 meq/L |
| Dissolved Oxygen | O₂ | ≥ 4.0 mg/L |
| pH | — | 6.5 – 8.5 |

---

## Standards Used

- WHO Drinking Water Guidelines (4th Edition)
- EU Drinking Water Directive 2020/2184

---

## How to Use

1. Open the [live demo](https://whisper278.github.io/AquaMetric/index.html)
2. Enter your water sample values
3. Click **Analyse Water Sample**
4. View results and water suitability assessment

Alternatively, download `index.html` and open it locally in any browser — no internet connection required.

---

## Tech Stack

- HTML5, CSS3, JavaScript (vanilla)
- No external dependencies — single-file application

---

## Project Status

This is v1.0. Planned improvements include:
- Python (Flask) backend with data visualisation (Plotly)
- Analysis history with database storage
- PDF/CSV export of results

---

*Inspired by field research on Lake Dighyah, Absheron Peninsula, Azerbaijan — a region where environmental monitoring data is critically scarce.*
