# AquaMetric — Digital Water Quality Assessment & Treatment Support Tool

**Live demo:** [https://whisper278.github.io/AquaMetric/](https://whisper278.github.io/AquaMetric/)

AquaMetric is a browser-based environmental tool for analysing measured water-quality data, comparing results with configured reference limits, visualising parameter status, and generating treatment-support recommendations.

## Quick start

```bash
npm install
npm run dev
```

Open [http://127.0.0.1:43127](http://127.0.0.1:43127).

No backend or database is required. You can also open `index.html` directly in a modern browser. Older frozen UI: `classic.html`.

## Background

Laboratory and field measurements produce large chemical and physical datasets. Interpreting those results, identifying exceeded parameters, and linking them to possible treatment approaches is time-consuming. AquaMetric turns measured results into an interactive assessment workflow:

**Ecology → Water Chemistry → Environmental Assessment → Data Visualisation → Treatment Support → Web Development**

## What it does

- Analyses measured water-quality parameters
- Compares measurements with configured MPC / reference limits
- Classifies parameters as Within Limit, Near Limit, or Exceeded
- Provides an overall assessment of the analysed sample
- Generates a Parameter vs MPC chart
- Screens water suitability for several use categories
- Screens for eutrophication-related concerns
- Generates a treatment sequence based on exceeded parameters
- Provides detailed treatment recommendations (cause, treatment, lab method)
- Stores recent analyses in browser `localStorage` (last 20)
- Imports and exports sample data as CSV
- Compares two samples (history or current form) with parameter deltas
- Generates a printable analysis report
- Supports English, Azerbaijani, and Russian

## Assessment context

The application records sample metadata:

- Sample ID
- Water body
- Location
- Sampling date
- Sampling depth
- Water temperature

Three assessment profiles:

1. **Drinking Water**
2. **Environmental / Surface Water Screening**
3. **Custom / Research**

The environmental profile is a screening context, not a formal ecological classification.

## Parameters (15)

| Parameter | Formula / Unit | Configured reference |
|---|---|---|
| Carbonates | CO₃²⁻ · mg/L | ≤ 300 mg/L |
| Bicarbonates | HCO₃⁻ · mg/L | ≤ 400 mg/L |
| Phosphates | PO₄³⁻ · mg/L | ≤ 3.5 mg/L |
| Sulphates | SO₄²⁻ · mg/L | ≤ 500 mg/L |
| Chlorides | Cl⁻ · mg/L | ≤ 350 mg/L |
| Ammonium | NH₄⁺ · mg/L | ≤ 0.5 mg/L |
| Nitrates | NO₃⁻ · mg/L | ≤ 45 mg/L |
| Nitrites | NO₂⁻ · mg/L | ≤ 3.3 mg/L |
| Total Hardness | meq/L | ≤ 7.0 meq/L |
| Dissolved Oxygen | O₂ · mg/L | ≥ 4.0 mg/L |
| pH | — | 6.5–8.5 |
| Colour | degrees | ≤ 20° |
| Turbidity | NTU | ≤ 2.6 NTU |
| Odour | points | ≤ 2 points |
| Taste | points | ≤ 2 points |

These are the reference values currently configured in the application. They should not be interpreted as a complete regulatory classification for every type of water body.

## Standards & reference framework

The interface identifies:

- WHO Guidelines for Drinking-water Quality (GDWQ 2026)
- EU Drinking Water Directive 2020/2184

A normative comparison table shows how project limits relate to WHO and EU values where applicable. Drinking-water standards and ecological surface-water assessment are different contexts — AquaMetric does not treat drinking-water limits as a complete ecological classification system for lakes or rivers.

## Themes

AquaMetric supports **Light** and **Dark** themes (toggle in the top bar):

- **Light** — coastal teal palette
- **Dark** — classic AquaMetric neon-lab palette

Secondary tools live under the **⋯** menu and open as separate screens (with Back):

- CSV import / export / template
- Compare samples
- Analysis history
- WHO / EU standards reference

## CSV import / export

Use **Export CSV** / **Import CSV** from the **⋯** menu, or download the **CSV template**.

Wide format (one sample per row):

```csv
sample_id,water_body,location,date,depth,temperature,profile,CO3,HCO3,PO4,...
S-001,Reservoir A,Site 1,2024-06-15,0.5 m,24 °C,environmental,120,280,5.2,...
```

Tall format is also accepted (`parameter,value`). After import, review values and click **Analyse**.

## Sample comparison

The **Compare Samples** panel lets you pick Sample A and Sample B from analysis history (or the current form) and shows:

- measured values side by side
- absolute delta (Δ)
- trend (improved / worsened / unchanged)
- status change relative to MPC

Useful for comparing samples across sampling dates.

## Treatment support

When parameters exceed configured limits, AquaMetric builds a treatment sequence that may include:

- Pre-filtration & solids removal
- pH correction
- Disinfection & organic removal
- Nitrate removal
- Softening
- Specific ion removal
- Phosphate removal
- Final aeration & oxygen restoration

Detailed per-parameter information covers possible causes, treatment technologies, and laboratory methods where implemented.

Treatment recommendations are technical support information, not automatically validated engineering designs.

## Technology

- HTML5 / CSS3 / Vanilla JavaScript
- SVG-based visualisation
- Browser `localStorage`
- Vite for local development
- No backend, database, or external JS framework
- Single-page web application (`index.html`)

## Project structure

```
AquaMetric/
├── index.html       # Current app (light/dark themes)
├── classic.html     # Frozen snapshot of earlier dark UI
├── package.json
├── vite.config.js
└── README.md
```

Theme preference is stored in `localStorage`. Open `classic.html` if you want the older layout.

## Author

**Cavid Mammadov**  
Baku State University · Faculty of Ecology and Soil Science  

Project focus: Water Quality · Environmental Engineering · Environmental Data Analysis · AI-Assisted Development

## Disclaimer

AquaMetric is an educational and research-support prototype. It does not replace certified laboratory analysis, regulatory assessment, professional environmental consulting, drinking-water safety certification, or detailed water-treatment engineering design.
