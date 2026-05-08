# 💧 AquaMetric — Digital Water Quality Analyser

A web-based tool for analysing water quality by comparing ion concentrations against WHO and EU drinking water standards.

🌐 **Live Demo:** [whisper278.github.io/AquaMetric/AquaMetric%20(1).html](https://whisper278.github.io/AquaMetric/index.html)

---

## About

AquaMetric is a universal water quality analysis tool that can be used for **any water body** — lakes, rivers, reservoirs, groundwater, or tap water. Simply enter your laboratory results and receive an instant assessment.

The application allows researchers, environmentalists, and students to input water sample data and instantly receive a quality assessment with practical recommendations for water use.

---

## Features

- ✅ Analyses 11 key water quality parameters
- 🌍 Available in **3 languages**: English, Azerbaijani, Russian
- 📊 Compares values against MPC (Maximum Permissible Concentration) limits
- 🔍 Classifies water suitability for: drinking, irrigation, industrial use, fishery
- ⚠️ Detects eutrophication risk
- 💻 Runs entirely in the browser — no installation required

---

## Parameters Analysed

| Parameter | Formula | MPC Limit |
|-----------|---------|-----------|
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

## Motivation

The idea for AquaMetric came from a real problem encountered during field research on **Lake Dighyah** (Absheron Peninsula, Azerbaijan) — a water body with almost no publicly available hydrochemical data. During the study, there was a clear lack of accessible tools to quickly evaluate water quality and communicate results in a meaningful way.

That experience highlighted a broader issue: many water bodies around the world — especially in undermonitored regions — lack systematic environmental assessment. AquaMetric was built to help address this gap, making water quality analysis accessible to researchers, students, and environmentalists regardless of location.

The Lake Dighyah study used the following methods:
- Spectrophotometry
- Titrimetric analysis
- Multiline Water Quality Meter 850081

Key findings that shaped the app's design:
- **Sulphates** and **carbonates** exceeded MPC limits
- **Total hardness** was significantly above the norm (11.8–13.4 meq/L vs. 7.0 meq/L limit)
- **Nitrates, nitrites, and ammonium** were within acceptable ranges
- Phosphate levels were close to the limit, indicating **eutrophication risk**

---

## Standards Used

- WHO Drinking Water Guidelines (4th Edition)
- EU Drinking Water Directive 2020/2184

---

## How to Use

1. Open the [live demo](https://whisper278.github.io/AquaMetric/AquaMetric%20(1).html)
2. Enter your water sample values
3. Click **Analyse Water Sample**
4. View detailed results and water suitability assessment

Or download `AquaMetric.html` and open it locally in any browser — no internet connection required.

---

## Tech Stack

- HTML5, CSS3, JavaScript (vanilla)
- No dependencies — single file application

---

*Built to make water quality assessment more accessible — inspired by field research on Lake Dighyah, Absheron Peninsula, Azerbaijan.*
