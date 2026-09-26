💧 AquaMetric — Digital Water Quality Assessment & Treatment Support Tool

AquaMetric is a browser-based environmental tool for analysing measured water-quality data, comparing results with configured reference limits, visualising parameter status, and generating treatment-support recommendations.

🌐 Live Demo: https://whisper278.github.io/AquaMetric/index.html

Background & Motivation

AquaMetric was developed in connection with field research on Lake Digah (Dighyah), Absheron Peninsula, Azerbaijan.

The project grew from a practical problem encountered during water-quality research: laboratory measurements produce a large amount of chemical and physical data, while interpreting those results, identifying exceeded parameters, and connecting them to possible treatment approaches can be time-consuming.

AquaMetric turns measured laboratory/field results into an interactive assessment workflow.

Ecology → Water Chemistry → Environmental Assessment → Data Visualisation → Treatment Support → Web Development

What AquaMetric Does

Analyses measured water-quality parameters

Compares measurements with configured MPC/reference limits

Classifies parameters as Within Limit, Near Limit, or Exceeded

Provides an overall assessment of the analysed sample

Generates a Parameter vs MPC chart

Screens water suitability for several use categories

Screens for eutrophication-related concerns

Generates a treatment sequence based on exceeded parameters

Provides detailed treatment recommendations

Explains possible causes of abnormal values

Provides laboratory analytical methods where implemented

Stores recent analyses locally in the browser

Allows previous analyses to be loaded

Generates a printable analysis report

Supports English, Azerbaijani, and Russian

Runs entirely in the browser without a backend or database

Assessment Context

The application records:

Sample ID

Water body

Location

Sampling date

Sampling depth

Water temperature

It also provides three assessment profiles:

Drinking Water

Environmental / Surface Water Screening

Custom / Research

The environmental profile is explicitly presented as a screening context rather than a formal ecological classification.

Parameters

The current application contains 15 water-quality parameters.

Parameter

Formula / Unit

Configured reference

Carbonates

CO₃²⁻ · mg/L

≤ 300 mg/L

Bicarbonates

HCO₃⁻ · mg/L

≤ 400 mg/L

Phosphates

PO₄³⁻ · mg/L

≤ 3.5 mg/L

Sulphates

SO₄²⁻ · mg/L

≤ 500 mg/L

Chlorides

Cl⁻ · mg/L

≤ 350 mg/L

Ammonium

NH₄⁺ · mg/L

≤ 0.5 mg/L

Nitrates

NO₃⁻ · mg/L

≤ 45 mg/L

Nitrites

NO₂⁻ · mg/L

≤ 3.3 mg/L

Total Hardness

meq/L

≤ 7.0 meq/L

Dissolved Oxygen

O₂ · mg/L

≥ 4.0 mg/L

pH

—

6.5–8.5

Colour

degrees

≤ 20°

Turbidity

NTU

≤ 2.6 NTU

Odour

points

≤ 2 points

Taste

points

≤ 2 points

Note: These are the reference values currently configured in the application. They should not be interpreted as a complete regulatory classification for every type of water body.

Analysis Workflow

Water sample
     ↓
Enter sample metadata
     ↓
Enter measured parameters
     ↓
Select assessment profile
     ↓
Analyse sample
     ↓
Parameter status classification
     ↓
Overall assessment
     ↓
Chart + detailed results
     ↓
Water-use screening
     ↓
Treatment sequence
     ↓
Detailed treatment recommendations
     ↓
Report export

The application also identifies unmeasured parameters and indicates when an assessment is based on only part of the available parameter set.

Treatment Support

A major feature of the current version is the Treatment Sequence.

When parameters exceed their configured limits, AquaMetric dynamically builds a sequence of potential treatment stages. Depending on the results, the sequence can include:

Pre-filtration & solids removal

pH correction

Disinfection & organic removal

Nitrate removal

Softening

Specific ion removal

Phosphate removal

Final aeration & oxygen restoration

The application also contains detailed treatment information for individual parameters, including:

Cause

Possible causes of elevated or abnormal values.

Treatment

Potential treatment technologies and process approaches, including where implemented:

Reverse osmosis

Ion exchange

Nanofiltration

Electrodialysis

Chemical precipitation

Lime softening

Aeration

Biological treatment

Disinfection

Source-control measures

Laboratory Method

Where implemented, the application provides analytical methods, measurement principles, procedures, reagents, and laboratory notes.

Treatment recommendations are technical support information, not automatically validated engineering designs. Actual treatment performance depends on the water matrix, concentration, flow rate, equipment, operating conditions, and engineering validation.

Data Visualisation

AquaMetric generates a Parameter vs MPC chart showing:

measured parameters

percentage relative to the configured reference

parameter status

the reference/MPC level

measured values and units

This provides a quick visual overview of parameters requiring attention.

Analysis History

The application uses browser localStorage for analysis history.

It can:

save recent analyses

retain sample metadata and measured values

display previous analyses

reload previous analyses

clear saved history

The current implementation retains the most recent 20 analyses locally.

No server-side database is required.

Multilingual Interface

The interface is available in:

🇬🇧 English

🇦🇿 Azerbaijani

🇷🇺 Russian

Reporting

AquaMetric includes a report workflow containing:

analysis date/time

overall assessment

measured values

reference limits

parameter status

unmeasured parameters

The current implementation provides a print-ready report that can be printed or saved through the browser.

Standards & Reference Framework

The interface identifies:

WHO Guidelines for Drinking-water Quality

EU Drinking Water Directive 2020/2184

The application uses configured reference values for automated comparison.

Because drinking-water standards and ecological surface-water assessment are different contexts, AquaMetric does not treat drinking-water limits as a complete ecological classification system for lakes or rivers.

Lake Digah Research Context

The project is inspired by field research conducted on Lake Digah, Absheron Peninsula, Azerbaijan.

The research context included:

spectrophotometric analysis

titrimetric analysis

Multiline Water Quality Meter 850081

AquaMetric provides a digital workflow for connecting measured water-quality data with assessment, visualisation, and treatment-support information.

Technology

HTML5

CSS3

Vanilla JavaScript

SVG-based visualisation

Browser localStorage

No backend

No database

No external JavaScript framework

Single-file web application

AI-Assisted Development

AquaMetric was developed using an AI-assisted / vibe-coding workflow.

The environmental problem, water-quality parameters, assessment structure, treatment workflow, and scientific context were defined from the project requirements and environmental research context, while AI-assisted coding was used to implement and iterate the web application.

The project therefore demonstrates both environmental/water-quality domain knowledge and practical use of modern AI-assisted software development.

Project Structure

AquaMetric/
├── index.html
└── README.md

The application is contained in index.html, including the interface, styles, multilingual content, assessment logic, chart generation, treatment recommendations, treatment sequence logic, history, and reporting functionality.

Running Locally

No installation is required.

git clone https://github.com/whisper278/AquaMetric.git
cd AquaMetric

Then open index.html in a modern web browser.

GitHub Pages

The application is deployed as a static website using GitHub Pages.

Live Demo:
https://whisper278.github.io/AquaMetric/index.html

Project Status

Current version: research-oriented prototype

The current version includes:

Sample metadata

Three assessment profiles

15 parameters

Multilingual interface

Parameter classification

Data visualisation

Water-use screening

Treatment sequence generation

Treatment recommendations

Laboratory-method information

Local analysis history

Report export

WHO/EU reference framework

Possible future development

Stronger source citation for individual limits and treatment claims

Additional environmental-water assessment frameworks

Sample comparison and time-series analysis

CSV import/export

GIS-based sampling locations

Expanded uncertainty/confidence information

External database storage

Python/Flask backend

Advanced statistical analysis

Integration with larger real-world laboratory datasets

Further engineering validation of treatment recommendations

Disclaimer

AquaMetric is an educational and research-support prototype.

It does not replace:

certified laboratory analysis

regulatory assessment

professional environmental consulting

drinking-water safety certification

detailed water-treatment engineering design

Treatment recommendations should be evaluated against the specific water matrix and validated through appropriate laboratory, pilot, and engineering testing before real-world implementation.

Author

Cavid Mammadov

Baku State University
Faculty of Ecology and Soil Science

Project focus:
Water Quality · Environmental Engineering · Environmental Data Analysis · AI-Assisted Development

Inspired by field research on Lake Digah, Absheron Peninsula, Azerbaijan.
