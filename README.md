[README.md](https://github.com/user-attachments/files/27099660/README.md)
# 💧 AquaMetric — Digital Water Quality Analyser

A web-based tool for analysing water quality by comparing ion concentrations against WHO and EU drinking water standards.

🌐 **Live Demo:** [whisper278.github.io/AquaMetric/AquaMetric%20(1).html](https://whisper278.github.io/AquaMetric/index.html)

---

## About

AquaMetric is a universal water quality analysis tool that can be used for **any water body** — lakes, rivers, reservoirs, groundwater, or tap water. Simply enter your laboratory results and receive an instant assessment.

The tool was originally inspired by real field research conducted at **Lake Dighyah** on the Absheron Peninsula in Azerbaijan — one of the first hydrochemical studies of this water body. However, the application is designed to work with water samples from anywhere in the world.

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

## Research Background

The project is based on a scientific study of **Lake Dighyah** (Absheron Peninsula, Azerbaijan). Water samples were collected and analysed using:

- Spectrophotometry
- Titrimetric analysis
- Multiline Water Quality Meter 850081

Key findings from the study:
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

Or download `AquaMetric.html` and open it locally in any browser.

---

## Tech Stack

- HTML5, CSS3, JavaScript (vanilla)
- No dependencies — single file application

---

*Developed as part of an environmental research project on the hydrochemical state of Lake Dighyah, Absheron Peninsula, Azerbaijan.*
